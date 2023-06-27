# Comparing `tmp/lacss-0.4.0.tar.gz` & `tmp/lacss-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.4.0.tar", max compression
+gzip compressed data, was "lacss-0.4.1.tar", max compression
```

## Comparing `lacss-0.4.0.tar` & `lacss-0.4.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1062 2023-06-22 13:00:42.813886 lacss-0.4.0/LICENSE
--rw-r--r--   0        0        0     2428 2023-06-22 13:00:42.825176 lacss-0.4.0/README.md
--rw-r--r--   0        0        0       65 2023-06-22 13:00:42.925221 lacss-0.4.0/lacss/__init__.py
--rw-r--r--   0        0        0       70 2023-06-26 19:35:53.100988 lacss-0.4.0/lacss/data/__init__.py
--rw-r--r--   0        0        0      208 2023-06-24 16:51:58.532392 lacss-0.4.0/lacss/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7981 2023-06-24 16:51:58.552630 lacss-0.4.0/lacss/data/__pycache__/augment.cpython-38.pyc
--rw-r--r--   0        0        0     5789 2023-06-26 16:14:31.717177 lacss-0.4.0/lacss/data/__pycache__/generator.cpython-38.pyc
--rw-r--r--   0        0        0     5681 2023-06-24 16:51:58.969925 lacss-0.4.0/lacss/data/__pycache__/parser.cpython-38.pyc
--rw-r--r--   0        0        0    11408 2023-06-26 19:35:53.107988 lacss-0.4.0/lacss/data/augment.py
--rw-r--r--   0        0        0     7747 2023-06-26 19:35:53.116426 lacss-0.4.0/lacss/data/generator.py
--rw-r--r--   0        0        0     9160 2023-06-24 16:49:56.373088 lacss-0.4.0/lacss/data/parser.py
--rw-r--r--   0        0        0     6991 2023-06-26 19:35:53.125780 lacss-0.4.0/lacss/deploy.py
--rw-r--r--   0        0        0       74 2023-06-22 13:00:42.985435 lacss-0.4.0/lacss/losses/__init__.py
--rw-r--r--   0        0        0      214 2023-06-22 13:02:41.734572 lacss-0.4.0/lacss/losses/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5053 2023-06-24 16:51:59.021079 lacss-0.4.0/lacss/losses/__pycache__/auxiliary.cpython-38.pyc
--rw-r--r--   0        0        0     3294 2023-06-26 16:14:32.412481 lacss-0.4.0/lacss/losses/__pycache__/detection.cpython-38.pyc
--rw-r--r--   0        0        0     4932 2023-06-26 12:17:08.113151 lacss-0.4.0/lacss/losses/__pycache__/instance.cpython-38.pyc
--rw-r--r--   0        0        0     5248 2023-06-26 19:35:53.135636 lacss-0.4.0/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0     2423 2023-06-26 19:35:53.144009 lacss-0.4.0/lacss/losses/detection.py
--rw-r--r--   0        0        0     5493 2023-06-26 19:35:53.152564 lacss-0.4.0/lacss/losses/instance.py
--rw-r--r--   0        0        0       56 2023-06-22 13:00:43.028217 lacss-0.4.0/lacss/metrics/__init__.py
--rw-r--r--   0        0        0      219 2023-06-22 13:02:43.184589 lacss-0.4.0/lacss/metrics/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5311 2023-06-24 16:51:59.886534 lacss-0.4.0/lacss/metrics/__pycache__/ranked.cpython-38.pyc
--rw-r--r--   0        0        0     5103 2023-06-26 19:35:53.161969 lacss-0.4.0/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      216 2023-06-22 13:00:43.059681 lacss-0.4.0/lacss/modules/__init__.py
--rw-r--r--   0        0        0      435 2023-06-22 13:02:43.238041 lacss-0.4.0/lacss/modules/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2245 2023-06-26 16:14:32.902258 lacss-0.4.0/lacss/modules/__pycache__/auxiliary.cpython-38.pyc
--rw-r--r--   0        0        0     3049 2023-06-22 13:02:43.270904 lacss-0.4.0/lacss/modules/__pycache__/common.cpython-38.pyc
--rw-r--r--   0        0        0     6420 2023-06-22 13:02:43.307157 lacss-0.4.0/lacss/modules/__pycache__/convnext.cpython-38.pyc
--rw-r--r--   0        0        0     4814 2023-06-22 13:02:43.323531 lacss-0.4.0/lacss/modules/__pycache__/detector.cpython-38.pyc
--rw-r--r--   0        0        0     3461 2023-06-24 16:51:59.937245 lacss-0.4.0/lacss/modules/__pycache__/lacss.cpython-38.pyc
--rw-r--r--   0        0        0     2932 2023-06-22 13:02:43.350421 lacss-0.4.0/lacss/modules/__pycache__/lpn.cpython-38.pyc
--rw-r--r--   0        0        0     3578 2023-06-22 13:02:43.367407 lacss-0.4.0/lacss/modules/__pycache__/resnet.cpython-38.pyc
--rw-r--r--   0        0        0     4253 2023-06-22 13:02:43.383527 lacss-0.4.0/lacss/modules/__pycache__/segmentor.cpython-38.pyc
--rw-r--r--   0        0        0     2211 2023-06-22 13:02:43.288536 lacss-0.4.0/lacss/modules/__pycache__/unet.cpython-38.pyc
--rw-r--r--   0        0        0     2075 2023-06-26 19:35:53.170430 lacss-0.4.0/lacss/modules/auxiliary.py
--rw-r--r--   0        0        0     2261 2023-06-22 13:00:43.114039 lacss-0.4.0/lacss/modules/common.py
--rw-r--r--   0        0        0     6646 2023-06-22 13:00:43.126366 lacss-0.4.0/lacss/modules/convnext.py
--rw-r--r--   0        0        0     6580 2023-06-22 13:00:43.134266 lacss-0.4.0/lacss/modules/detector.py
--rw-r--r--   0        0        0     4120 2023-06-26 19:35:53.181137 lacss-0.4.0/lacss/modules/lacss.py
--rw-r--r--   0        0        0     3339 2023-06-22 13:00:43.156519 lacss-0.4.0/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3771 2023-06-22 13:00:43.167303 lacss-0.4.0/lacss/modules/resnet.py
--rw-r--r--   0        0        0     5254 2023-06-22 13:00:43.186704 lacss-0.4.0/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     1979 2023-06-22 13:00:43.193776 lacss-0.4.0/lacss/modules/unet.py
--rw-r--r--   0        0        0      174 2023-06-22 13:00:43.204051 lacss-0.4.0/lacss/ops/__init__.py
--rw-r--r--   0        0        0      270 2023-06-22 13:02:42.172883 lacss-0.4.0/lacss/ops/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2142 2023-06-24 16:51:59.057060 lacss-0.4.0/lacss/ops/__pycache__/boxes.cpython-38.pyc
--rw-r--r--   0        0        0     3480 2023-06-24 16:51:59.075805 lacss-0.4.0/lacss/ops/__pycache__/image.cpython-38.pyc
--rw-r--r--   0        0        0     2457 2023-06-24 16:51:59.103646 lacss-0.4.0/lacss/ops/__pycache__/locations.cpython-38.pyc
--rw-r--r--   0        0        0     5806 2023-06-22 13:02:42.251931 lacss-0.4.0/lacss/ops/__pycache__/masks.cpython-38.pyc
--rw-r--r--   0        0        0     3885 2023-06-24 16:51:59.139415 lacss-0.4.0/lacss/ops/__pycache__/nms.cpython-38.pyc
--rw-r--r--   0        0        0    10189 2023-06-24 23:33:38.687451 lacss-0.4.0/lacss/ops/__pycache__/patches.cpython-38.pyc
--rw-r--r--   0        0        0      672 2023-06-22 13:02:42.295307 lacss-0.4.0/lacss/ops/__pycache__/uda.cpython-38.pyc
--rw-r--r--   0        0        0     2321 2023-06-26 19:35:53.190870 lacss-0.4.0/lacss/ops/boxes.py
--rw-r--r--   0        0        0     3289 2023-06-26 19:35:53.198904 lacss-0.4.0/lacss/ops/image.py
--rw-r--r--   0        0        0     2843 2023-06-26 19:35:53.211864 lacss-0.4.0/lacss/ops/locations.py
--rw-r--r--   0        0        0     5967 2023-06-22 13:00:43.238207 lacss-0.4.0/lacss/ops/masks.py
--rw-r--r--   0        0        0     4732 2023-06-26 19:35:53.222000 lacss-0.4.0/lacss/ops/nms.py
--rw-r--r--   0        0        0    11768 2023-06-26 19:35:53.231134 lacss-0.4.0/lacss/ops/patches.py
--rw-r--r--   0        0        0      225 2023-06-22 13:00:43.270685 lacss-0.4.0/lacss/ops/uda.py
--rw-r--r--   0        0        0       63 2023-06-22 13:00:43.284052 lacss-0.4.0/lacss/tracking/__init__.py
--rw-r--r--   0        0        0     3340 2023-06-22 13:00:43.292844 lacss-0.4.0/lacss/tracking/predict.py
--rw-r--r--   0        0        0     6741 2023-06-22 13:00:43.306733 lacss-0.4.0/lacss/tracking/smc.py
--rw-r--r--   0        0        0     5646 2023-06-22 13:00:43.323766 lacss-0.4.0/lacss/tracking/utils.py
--rw-r--r--   0        0        0       99 2023-06-22 13:00:43.333394 lacss-0.4.0/lacss/train/__init__.py
--rw-r--r--   0        0        0      257 2023-06-22 13:02:42.316230 lacss-0.4.0/lacss/train/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6686 2023-06-22 13:02:42.529439 lacss-0.4.0/lacss/train/__pycache__/loss.cpython-38.pyc
--rw-r--r--   0        0        0      648 2023-06-22 13:02:43.199772 lacss-0.4.0/lacss/train/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0     4118 2023-06-22 13:02:42.813109 lacss-0.4.0/lacss/train/__pycache__/strategy.cpython-38.pyc
--rw-r--r--   0        0        0    12176 2023-06-26 16:14:32.368821 lacss-0.4.0/lacss/train/__pycache__/trainer.cpython-38.pyc
--rw-r--r--   0        0        0      718 2023-06-22 13:00:43.345992 lacss-0.4.0/lacss/train/data/__init__.py
--rw-r--r--   0        0        0      851 2023-06-22 13:02:42.337930 lacss-0.4.0/lacss/train/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4005 2023-06-22 13:02:42.353245 lacss-0.4.0/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     6093 2023-06-22 13:02:42.371233 lacss-0.4.0/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     5561 2023-06-22 13:02:42.399155 lacss-0.4.0/lacss/train/data/__pycache__/data_handler.cpython-38.pyc
--rw-r--r--   0        0        0    11577 2023-06-22 13:02:42.414539 lacss-0.4.0/lacss/train/data/__pycache__/dataset.cpython-38.pyc
--rw-r--r--   0        0        0     3319 2023-06-22 13:02:42.437553 lacss-0.4.0/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     2515 2023-06-22 13:02:42.454501 lacss-0.4.0/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     3562 2023-06-22 13:02:42.482462 lacss-0.4.0/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     3167 2023-06-22 13:02:42.502701 lacss-0.4.0/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     6796 2023-06-22 13:02:42.385721 lacss-0.4.0/lacss/train/data/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     4076 2023-06-22 13:00:43.353833 lacss-0.4.0/lacss/train/data/array_adapter.py
--rw-r--r--   0        0        0     5529 2023-06-22 13:00:43.360856 lacss-0.4.0/lacss/train/data/data_adapter.py
--rw-r--r--   0        0        0     6287 2023-06-22 13:00:43.369351 lacss-0.4.0/lacss/train/data/data_handler.py
--rw-r--r--   0        0        0    10656 2023-06-22 13:00:43.388157 lacss-0.4.0/lacss/train/data/dataset.py
--rw-r--r--   0        0        0     2599 2023-06-22 13:00:43.431971 lacss-0.4.0/lacss/train/data/generator_adapter.py
--rw-r--r--   0        0        0     2105 2023-06-22 13:00:43.446554 lacss-0.4.0/lacss/train/data/list_adapter.py
--rw-r--r--   0        0        0     3440 2023-06-22 13:00:43.456684 lacss-0.4.0/lacss/train/data/tf_dataset_adapter.py
--rw-r--r--   0        0        0     2566 2023-06-22 13:00:43.469261 lacss-0.4.0/lacss/train/data/torch_dataloader_adapter.py
--rw-r--r--   0        0        0     6394 2023-06-22 13:00:43.494227 lacss-0.4.0/lacss/train/data/utils.py
--rw-r--r--   0        0        0     6834 2023-06-22 13:00:43.502914 lacss-0.4.0/lacss/train/loss.py
--rw-r--r--   0        0        0      222 2023-06-22 13:00:43.517371 lacss-0.4.0/lacss/train/metric.py
--rw-r--r--   0        0        0     4018 2023-06-22 13:00:43.524618 lacss-0.4.0/lacss/train/strategy.py
--rw-r--r--   0        0        0    13001 2023-06-26 19:35:53.238863 lacss-0.4.0/lacss/train/trainer.py
--rw-r--r--   0        0        0     6392 2023-06-26 19:35:53.249659 lacss-0.4.0/lacss/utils.py
--rw-r--r--   0        0        0      810 2023-06-26 19:38:12.530900 lacss-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 lacss-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-22 13:00:42.813886 lacss-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2428 2023-06-22 13:00:42.825176 lacss-0.4.1/README.md
+-rw-r--r--   0        0        0       65 2023-06-22 13:00:42.925221 lacss-0.4.1/lacss/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-27 19:54:42.795534 lacss-0.4.1/lacss/data/__init__.py
+-rw-r--r--   0        0        0      190 2023-06-27 19:47:56.226635 lacss-0.4.1/lacss/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7981 2023-06-26 19:53:37.181410 lacss-0.4.1/lacss/data/__pycache__/augment.cpython-38.pyc
+-rw-r--r--   0        0        0     5839 2023-06-26 19:53:37.207035 lacss-0.4.1/lacss/data/__pycache__/generator.cpython-38.pyc
+-rw-r--r--   0        0        0     5681 2023-06-27 16:23:45.927971 lacss-0.4.1/lacss/data/__pycache__/parser.cpython-38.pyc
+-rw-r--r--   0        0        0    11408 2023-06-26 19:35:53.107988 lacss-0.4.1/lacss/data/augment.py
+-rw-r--r--   0        0        0     7747 2023-06-26 19:35:53.116426 lacss-0.4.1/lacss/data/generator.py
+-rw-r--r--   0        0        0     8975 2023-06-27 19:54:42.804698 lacss-0.4.1/lacss/deploy.py
+-rw-r--r--   0        0        0       74 2023-06-22 13:00:42.985435 lacss-0.4.1/lacss/losses/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-22 13:02:41.734572 lacss-0.4.1/lacss/losses/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5053 2023-06-26 19:53:37.570269 lacss-0.4.1/lacss/losses/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     3294 2023-06-26 19:53:37.842923 lacss-0.4.1/lacss/losses/__pycache__/detection.cpython-38.pyc
+-rw-r--r--   0        0        0     4905 2023-06-27 19:48:13.187810 lacss-0.4.1/lacss/losses/__pycache__/instance.cpython-38.pyc
+-rw-r--r--   0        0        0     5248 2023-06-26 19:35:53.135636 lacss-0.4.1/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0     2423 2023-06-26 19:35:53.144009 lacss-0.4.1/lacss/losses/detection.py
+-rw-r--r--   0        0        0     5601 2023-06-27 19:54:42.814188 lacss-0.4.1/lacss/losses/instance.py
+-rw-r--r--   0        0        0       56 2023-06-22 13:00:43.028217 lacss-0.4.1/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-22 13:02:43.184589 lacss-0.4.1/lacss/metrics/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5311 2023-06-26 19:53:38.336584 lacss-0.4.1/lacss/metrics/__pycache__/ranked.cpython-38.pyc
+-rw-r--r--   0        0        0     5103 2023-06-26 19:35:53.161969 lacss-0.4.1/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      216 2023-06-22 13:00:43.059681 lacss-0.4.1/lacss/modules/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-22 13:02:43.238041 lacss-0.4.1/lacss/modules/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2245 2023-06-26 19:53:38.371089 lacss-0.4.1/lacss/modules/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     3049 2023-06-22 13:02:43.270904 lacss-0.4.1/lacss/modules/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0     6420 2023-06-22 13:02:43.307157 lacss-0.4.1/lacss/modules/__pycache__/convnext.cpython-38.pyc
+-rw-r--r--   0        0        0     4814 2023-06-22 13:02:43.323531 lacss-0.4.1/lacss/modules/__pycache__/detector.cpython-38.pyc
+-rw-r--r--   0        0        0     3443 2023-06-26 21:02:19.236756 lacss-0.4.1/lacss/modules/__pycache__/lacss.cpython-38.pyc
+-rw-r--r--   0        0        0     2932 2023-06-22 13:02:43.350421 lacss-0.4.1/lacss/modules/__pycache__/lpn.cpython-38.pyc
+-rw-r--r--   0        0        0     3578 2023-06-22 13:02:43.367407 lacss-0.4.1/lacss/modules/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0     4253 2023-06-27 17:33:27.254646 lacss-0.4.1/lacss/modules/__pycache__/segmentor.cpython-38.pyc
+-rw-r--r--   0        0        0     2211 2023-06-22 13:02:43.288536 lacss-0.4.1/lacss/modules/__pycache__/unet.cpython-38.pyc
+-rw-r--r--   0        0        0     2075 2023-06-26 19:35:53.170430 lacss-0.4.1/lacss/modules/auxiliary.py
+-rw-r--r--   0        0        0     2261 2023-06-22 13:00:43.114039 lacss-0.4.1/lacss/modules/common.py
+-rw-r--r--   0        0        0     6646 2023-06-22 13:00:43.126366 lacss-0.4.1/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     6580 2023-06-22 13:00:43.134266 lacss-0.4.1/lacss/modules/detector.py
+-rw-r--r--   0        0        0     4120 2023-06-26 19:59:28.277578 lacss-0.4.1/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     3339 2023-06-22 13:00:43.156519 lacss-0.4.1/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3771 2023-06-22 13:00:43.167303 lacss-0.4.1/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     5254 2023-06-27 17:32:18.960037 lacss-0.4.1/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     1979 2023-06-22 13:00:43.193776 lacss-0.4.1/lacss/modules/unet.py
+-rw-r--r--   0        0        0      174 2023-06-22 13:00:43.204051 lacss-0.4.1/lacss/ops/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-22 13:02:42.172883 lacss-0.4.1/lacss/ops/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2142 2023-06-26 19:53:37.599646 lacss-0.4.1/lacss/ops/__pycache__/boxes.cpython-38.pyc
+-rw-r--r--   0        0        0     3480 2023-06-26 19:53:37.613942 lacss-0.4.1/lacss/ops/__pycache__/image.cpython-38.pyc
+-rw-r--r--   0        0        0     2457 2023-06-26 19:53:37.639373 lacss-0.4.1/lacss/ops/__pycache__/locations.cpython-38.pyc
+-rw-r--r--   0        0        0     5806 2023-06-22 13:02:42.251931 lacss-0.4.1/lacss/ops/__pycache__/masks.cpython-38.pyc
+-rw-r--r--   0        0        0     3885 2023-06-26 19:53:37.704140 lacss-0.4.1/lacss/ops/__pycache__/nms.cpython-38.pyc
+-rw-r--r--   0        0        0    10189 2023-06-26 19:53:37.661239 lacss-0.4.1/lacss/ops/__pycache__/patches.cpython-38.pyc
+-rw-r--r--   0        0        0      672 2023-06-22 13:02:42.295307 lacss-0.4.1/lacss/ops/__pycache__/uda.cpython-38.pyc
+-rw-r--r--   0        0        0     2321 2023-06-26 19:35:53.190870 lacss-0.4.1/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     3289 2023-06-26 19:35:53.198904 lacss-0.4.1/lacss/ops/image.py
+-rw-r--r--   0        0        0     2843 2023-06-26 19:35:53.211864 lacss-0.4.1/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5967 2023-06-22 13:00:43.238207 lacss-0.4.1/lacss/ops/masks.py
+-rw-r--r--   0        0        0     4732 2023-06-26 19:35:53.222000 lacss-0.4.1/lacss/ops/nms.py
+-rw-r--r--   0        0        0    11768 2023-06-26 19:35:53.231134 lacss-0.4.1/lacss/ops/patches.py
+-rw-r--r--   0        0        0      225 2023-06-22 13:00:43.270685 lacss-0.4.1/lacss/ops/uda.py
+-rw-r--r--   0        0        0       63 2023-06-27 18:55:24.517866 lacss-0.4.1/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0     3340 2023-06-22 13:00:43.292844 lacss-0.4.1/lacss/tracking/predict.py
+-rw-r--r--   0        0        0    12669 2023-06-27 19:54:42.820854 lacss-0.4.1/lacss/tracking/seqnms.py
+-rw-r--r--   0        0        0     6741 2023-06-22 13:00:43.306733 lacss-0.4.1/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2023-06-22 13:00:43.323766 lacss-0.4.1/lacss/tracking/utils.py
+-rw-r--r--   0        0        0       99 2023-06-22 13:00:43.333394 lacss-0.4.1/lacss/train/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-22 13:02:42.316230 lacss-0.4.1/lacss/train/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6686 2023-06-22 13:02:42.529439 lacss-0.4.1/lacss/train/__pycache__/loss.cpython-38.pyc
+-rw-r--r--   0        0        0      648 2023-06-22 13:02:43.199772 lacss-0.4.1/lacss/train/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     4118 2023-06-27 19:48:09.272553 lacss-0.4.1/lacss/train/__pycache__/strategy.cpython-38.pyc
+-rw-r--r--   0        0        0    12131 2023-06-27 19:48:09.311593 lacss-0.4.1/lacss/train/__pycache__/trainer.cpython-38.pyc
+-rw-r--r--   0        0        0      718 2023-06-22 13:00:43.345992 lacss-0.4.1/lacss/train/data/__init__.py
+-rw-r--r--   0        0        0      851 2023-06-22 13:02:42.337930 lacss-0.4.1/lacss/train/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4005 2023-06-22 13:02:42.353245 lacss-0.4.1/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6093 2023-06-22 13:02:42.371233 lacss-0.4.1/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     5561 2023-06-22 13:02:42.399155 lacss-0.4.1/lacss/train/data/__pycache__/data_handler.cpython-38.pyc
+-rw-r--r--   0        0        0    11577 2023-06-22 13:02:42.414539 lacss-0.4.1/lacss/train/data/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     3319 2023-06-22 13:02:42.437553 lacss-0.4.1/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     2515 2023-06-22 13:02:42.454501 lacss-0.4.1/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3562 2023-06-22 13:02:42.482462 lacss-0.4.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3167 2023-06-22 13:02:42.502701 lacss-0.4.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6796 2023-06-22 13:02:42.385721 lacss-0.4.1/lacss/train/data/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     4076 2023-06-22 13:00:43.353833 lacss-0.4.1/lacss/train/data/array_adapter.py
+-rw-r--r--   0        0        0     5529 2023-06-22 13:00:43.360856 lacss-0.4.1/lacss/train/data/data_adapter.py
+-rw-r--r--   0        0        0     6287 2023-06-22 13:00:43.369351 lacss-0.4.1/lacss/train/data/data_handler.py
+-rw-r--r--   0        0        0    10656 2023-06-22 13:00:43.388157 lacss-0.4.1/lacss/train/data/dataset.py
+-rw-r--r--   0        0        0     2599 2023-06-22 13:00:43.431971 lacss-0.4.1/lacss/train/data/generator_adapter.py
+-rw-r--r--   0        0        0     2105 2023-06-22 13:00:43.446554 lacss-0.4.1/lacss/train/data/list_adapter.py
+-rw-r--r--   0        0        0     3440 2023-06-22 13:00:43.456684 lacss-0.4.1/lacss/train/data/tf_dataset_adapter.py
+-rw-r--r--   0        0        0     2566 2023-06-22 13:00:43.469261 lacss-0.4.1/lacss/train/data/torch_dataloader_adapter.py
+-rw-r--r--   0        0        0     6394 2023-06-22 13:00:43.494227 lacss-0.4.1/lacss/train/data/utils.py
+-rw-r--r--   0        0        0     6834 2023-06-22 13:00:43.502914 lacss-0.4.1/lacss/train/loss.py
+-rw-r--r--   0        0        0      222 2023-06-22 13:00:43.517371 lacss-0.4.1/lacss/train/metric.py
+-rw-r--r--   0        0        0     4018 2023-06-27 19:00:57.668124 lacss-0.4.1/lacss/train/strategy.py
+-rw-r--r--   0        0        0    12919 2023-06-27 19:54:42.831348 lacss-0.4.1/lacss/train/trainer.py
+-rw-r--r--   0        0        0     6392 2023-06-26 19:35:53.249659 lacss-0.4.1/lacss/utils.py
+-rw-r--r--   0        0        0      810 2023-06-27 19:55:50.890419 lacss-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 lacss-0.4.1/PKG-INFO
```

### Comparing `lacss-0.4.0/LICENSE` & `lacss-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/README.md` & `lacss-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/data/__pycache__/augment.cpython-38.pyc` & `lacss-0.4.1/lacss/data/__pycache__/augment.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:04 2023 UTC, .py size: 11408 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bc1e 9764 902c 0000  U..........d.,..
+00000000: 550d 0d0a 0000 0000 99e8 9964 902c 0000  U..........d.,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6403 6404 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6405 6406 8400 5a05 6407  m.Z...d.d...Z.d.
 00000050: 6408 8400 5a06 6409 640a 8400 5a07 640b  d...Z.d.d...Z.d.
 00000060: 640c 9c01 640d 640e 8402 5a08 640f 640b  d...d.d...Z.d.d.
 00000070: 6410 9c02 6411 6412 8402 5a09 640b 640b  d...d.d...Z.d.d.
```

### Comparing `lacss-0.4.0/lacss/data/__pycache__/generator.cpython-38.pyc` & `lacss-0.4.1/lacss/data/__pycache__/generator.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 15:28:02 2023 UTC, .py size: 7683 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 82ae 9964 031e 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 99e8 9964 431e 0000  U..........dC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6401 6c06 6d07 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6401 6c09 5a0a 6400 6401 6c0b  ..d.d.l.Z.d.d.l.
 00000070: 5a0c 6400 6404 6c0d 6d0e 5a0e 0100 6405  Z.d.d.l.m.Z...d.
@@ -281,82 +281,85 @@
 00001180: 2904 7222 0000 0072 4600 0000 7264 0000  ).r"...rF...rd..
 00001190: 0072 7600 0000 721c 0000 0072 7500 0000  .rv...r....ru...
 000011a0: 721d 0000 00da 1f64 6174 6173 6574 5f66  r......dataset_f
 000011b0: 726f 6d5f 7369 6d70 6c65 5f61 6e6e 6f74  rom_simple_annot
 000011c0: 6174 696f 6e73 bf00 0000 7310 0000 0000  ations....s.....
 000011d0: 0308 010e 020e 010e 0116 0112 fc04 fe72  ...............r
 000011e0: 7700 0000 6301 0000 0000 0000 0000 0000  w...c...........
-000011f0: 0009 0000 0007 0000 0063 0000 0073 c800  .........c...s..
-00001200: 0000 7400 7c00 8301 4400 5dba 5c02 7d01  ..t.|...D.].\.}.
+000011f0: 0009 0000 0007 0000 0063 0000 0073 e200  .........c...s..
+00001200: 0000 7400 7c00 8301 4400 5dd4 5c02 7d01  ..t.|...D.].\.}.
 00001210: 5c02 7d02 7d03 7401 a002 7c02 a101 a003  \.}.}.t...|.....
 00001220: 6401 a101 7d04 7c04 6402 1d00 7d04 7404  d...}.|.d...}.t.
 00001230: 7c04 6a05 8301 6403 6b02 7250 7c04 6400  |.j...d.k.rP|.d.
 00001240: 6400 8502 6400 6400 8502 6400 6603 1900  d...d.d...d.f...
 00001250: 7d04 7401 a002 7c03 a101 7d05 7404 7c05  }.t...|...}.t.|.
 00001260: 6a05 8301 6404 6b02 727e 7c05 6400 6400  j...d.k.r~|.d.d.
 00001270: 8502 6400 6400 8502 6405 6603 1900 7d05  ..d.d...d.f...}.
 00001280: 6700 7d06 6700 7d07 7406 7c05 8301 4400  g.}.g.}.t.|...D.
 00001290: 5d20 7d08 7c06 a007 7c08 6406 1900 a101  ] }.|...|.d.....
 000012a0: 0100 7c07 a007 7c08 6407 1900 a101 0100  ..|...|.d.......
-000012b0: 718e 7c01 7c04 7c07 7c06 7c05 6408 9c05  q.|.|.|.|.|.d...
-000012c0: 5600 0100 7108 6400 5300 2909 4e72 2500  V...q.d.S.).Nr%.
-000012d0: 0000 e9ff 0000 0072 0500 0000 7206 0000  .......r....r...
-000012e0: 0072 0100 0000 7224 0000 00da 0863 656e  .r....r$.....cen
-000012f0: 7472 6f69 64a9 0572 6900 0000 720f 0000  troid..ri...r...
-00001300: 0072 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
-00001310: 2908 726f 0000 0072 3e00 0000 723f 0000  ).ro...r>...r?..
-00001320: 0072 4000 0000 7212 0000 0072 0e00 0000  .r@...r....r....
-00001330: 7204 0000 0072 3900 0000 2909 5a08 6473  r....r9...).Z.ds
-00001340: 5f66 696c 6573 7272 0000 005a 0869 6d67  _filesrr...Z.img
-00001350: 5f66 696c 6572 6700 0000 da03 696d 6772  _filerg.....imgr
-00001360: 4e00 0000 7230 0000 0072 4b00 0000 da04  N...r0...rK.....
-00001370: 7072 6f70 721c 0000 0072 1c00 0000 721d  propr....r....r.
-00001380: 0000 00da 1769 6d67 5f6d 6173 6b5f 7061  .....img_mask_pa
-00001390: 6972 5f67 656e 6572 6174 6f72 cd00 0000  ir_generator....
-000013a0: 7326 0000 0000 0114 0110 0108 010e 0116  s&..............
-000013b0: 020a 010e 0116 0204 0104 010c 010e 0110  ................
-000013c0: 0302 0102 0102 0102 0102 fb72 7d00 0000  ...........r}...
-000013d0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-000013e0: 000a 0000 000b 0000 0073 7600 0000 7400  .........sv...t.
-000013f0: 6a01 6a02 6a03 8700 8701 8702 6603 6401  j.j.j.......f.d.
-00001400: 6402 8408 7400 6a04 6700 7400 6a05 6403  d...t.j.g.t.j.d.
-00001410: 8d02 7400 6a04 7c02 7400 6a06 6403 8d02  ..t.j.|.t.j.d...
-00001420: 7400 6a04 6400 6404 6702 7400 6a06 6403  t.j.d.d.g.t.j.d.
-00001430: 8d02 7400 6a04 6400 6405 6702 7400 6a06  ..t.j.d.d.g.t.j.
-00001440: 6403 8d02 7400 6a04 7c02 6400 6404 8502  d...t.j.|.d.d...
-00001450: 1900 7400 6a07 6403 8d02 6406 9c05 6407  ..t.j.d...d...d.
-00001460: 8d02 5300 2908 4e63 0000 0000 0000 0000  ..S.).Nc........
-00001470: 0000 0000 0000 0000 0400 0000 1300 0000  ................
-00001480: 7312 0000 0074 0074 0188 0088 0283 0266  s....t.t.......f
-00001490: 0188 018e 0153 0072 7400 0000 2902 727d  .....S.rt...).r}
-000014a0: 0000 00da 037a 6970 721c 0000 00a9 03da  .....zipr.......
-000014b0: 0869 6d67 6669 6c65 7372 7600 0000 da09  .imgfilesrv.....
-000014c0: 6d61 736b 6669 6c65 7372 1c00 0000 721d  maskfilesr....r.
-000014d0: 0000 0072 5900 0000 eb00 0000 725a 0000  ...rY.......rZ..
-000014e0: 007a 2d64 6174 6173 6574 5f66 726f 6d5f  .z-dataset_from_
-000014f0: 696d 675f 6d61 736b 5f70 6169 7273 2e3c  img_mask_pairs.<
-00001500: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00001510: 7226 0000 0072 0500 0000 725b 0000 0072  r&...r....r[...r
-00001520: 7a00 0000 725c 0000 0029 0872 0c00 0000  z...r\...).r....
-00001530: 725f 0000 0072 6000 0000 7261 0000 0072  r_...r`...ra...r
-00001540: 5e00 0000 7262 0000 0072 2500 0000 722b  ^...rb...r%...r+
-00001550: 0000 0029 0472 8000 0000 7281 0000 0072  ...).r....r....r
-00001560: 6400 0000 7276 0000 0072 1c00 0000 727f  d...rv...r....r.
-00001570: 0000 0072 1d00 0000 da1b 6461 7461 7365  ...r......datase
-00001580: 745f 6672 6f6d 5f69 6d67 5f6d 6173 6b5f  t_from_img_mask_
-00001590: 7061 6972 73e7 0000 0073 1200 0000 0003  pairs....s......
-000015a0: 0801 0e02 0e01 0e01 1201 1201 16fb 04fe  ................
-000015b0: 7282 0000 0029 014e 2917 723c 0000 0072  r....).N).r<...r
-000015c0: 6d00 0000 da09 6675 6e63 746f 6f6c 7372  m.....functoolsr
-000015d0: 0200 0000 da07 6f73 2e70 6174 6872 0300  ......os.pathr..
-000015e0: 0000 5a0a 696d 6167 6569 6f2e 7632 da02  ..Z.imageio.v2..
-000015f0: 7632 723e 0000 0072 4200 0000 7237 0000  v2r>...rB...r7..
-00001600: 00da 0a74 656e 736f 7266 6c6f 7772 0c00  ...tensorflowr..
-00001610: 0000 da0f 736b 696d 6167 652e 6d65 6173  ....skimage.meas
-00001620: 7572 6572 0400 0000 721e 0000 0072 5400  urer....r....rT.
-00001630: 0000 7256 0000 0072 6500 0000 7273 0000  ..rV...re...rs..
-00001640: 0072 7700 0000 727d 0000 0072 8200 0000  .rw...r}...r....
-00001650: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-00001660: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00001670: 0000 7326 0000 0008 0108 010c 010c 020c  ..s&............
-00001680: 0108 0108 010c 0608 100a 4508 2608 0106  ..........E.&...
-00001690: fc0a 1908 2008 ff0a 0e08 1b08 ff         .... ........
+000012b0: 718e 7c01 7c04 a003 6401 a101 7408 6a09  q.|.|...d...t.j.
+000012c0: 7c07 6401 6408 8d02 6409 1700 7408 a009  |.d.d...d...t...
+000012d0: 7c06 a101 7c05 640a 9c05 5600 0100 7108  |...|.d...V...q.
+000012e0: 6400 5300 290b 4e72 2500 0000 e9ff 0000  d.S.).Nr%.......
+000012f0: 0072 0500 0000 7206 0000 0072 0100 0000  .r....r....r....
+00001300: 7224 0000 00da 0863 656e 7472 6f69 6472  r$.....centroidr
+00001310: 2600 0000 720b 0000 00a9 0572 6900 0000  &...r......ri...
+00001320: 720f 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
+00001330: 3100 0000 290a 726f 0000 0072 3e00 0000  1...).ro...r>...
+00001340: 723f 0000 0072 4000 0000 7212 0000 0072  r?...r@...r....r
+00001350: 0e00 0000 7204 0000 0072 3900 0000 7237  ....r....r9...r7
+00001360: 0000 00da 0761 7361 7272 6179 2909 5a08  .....asarray).Z.
+00001370: 6473 5f66 696c 6573 7272 0000 005a 0869  ds_filesrr...Z.i
+00001380: 6d67 5f66 696c 6572 6700 0000 da03 696d  mg_filerg.....im
+00001390: 6772 4e00 0000 7230 0000 0072 4b00 0000  grN...r0...rK...
+000013a0: da04 7072 6f70 721c 0000 0072 1c00 0000  ..propr....r....
+000013b0: 721d 0000 00da 1769 6d67 5f6d 6173 6b5f  r......img_mask_
+000013c0: 7061 6972 5f67 656e 6572 6174 6f72 cd00  pair_generator..
+000013d0: 0000 7326 0000 0000 0114 0110 0108 010e  ..s&............
+000013e0: 0116 020a 010e 0116 0204 0104 010c 010e  ................
+000013f0: 0110 0302 0108 0110 0108 0102 fb72 7e00  .............r~.
+00001400: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
+00001410: 0000 000a 0000 000b 0000 0073 7600 0000  ...........sv...
+00001420: 7400 6a01 6a02 6a03 8700 8701 8702 6603  t.j.j.j.......f.
+00001430: 6401 6402 8408 7400 6a04 6700 7400 6a05  d.d...t.j.g.t.j.
+00001440: 6403 8d02 7400 6a04 7c02 7400 6a06 6403  d...t.j.|.t.j.d.
+00001450: 8d02 7400 6a04 6400 6404 6702 7400 6a06  ..t.j.d.d.g.t.j.
+00001460: 6403 8d02 7400 6a04 6400 6405 6702 7400  d...t.j.d.d.g.t.
+00001470: 6a06 6403 8d02 7400 6a04 7c02 6400 6404  j.d...t.j.|.d.d.
+00001480: 8502 1900 7400 6a07 6403 8d02 6406 9c05  ....t.j.d...d...
+00001490: 6407 8d02 5300 2908 4e63 0000 0000 0000  d...S.).Nc......
+000014a0: 0000 0000 0000 0000 0000 0400 0000 1300  ................
+000014b0: 0000 7312 0000 0074 0074 0188 0088 0283  ..s....t.t......
+000014c0: 0266 0188 018e 0153 0072 7400 0000 2902  .f.....S.rt...).
+000014d0: 727e 0000 00da 037a 6970 721c 0000 00a9  r~.....zipr.....
+000014e0: 03da 0869 6d67 6669 6c65 7372 7600 0000  ...imgfilesrv...
+000014f0: da09 6d61 736b 6669 6c65 7372 1c00 0000  ..maskfilesr....
+00001500: 721d 0000 0072 5900 0000 eb00 0000 725a  r....rY.......rZ
+00001510: 0000 007a 2d64 6174 6173 6574 5f66 726f  ...z-dataset_fro
+00001520: 6d5f 696d 675f 6d61 736b 5f70 6169 7273  m_img_mask_pairs
+00001530: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00001540: 613e 7226 0000 0072 0500 0000 725b 0000  a>r&...r....r[..
+00001550: 0072 7a00 0000 725c 0000 0029 0872 0c00  .rz...r\...).r..
+00001560: 0000 725f 0000 0072 6000 0000 7261 0000  ..r_...r`...ra..
+00001570: 0072 5e00 0000 7262 0000 0072 2500 0000  .r^...rb...r%...
+00001580: 722b 0000 0029 0472 8100 0000 7282 0000  r+...).r....r...
+00001590: 0072 6400 0000 7276 0000 0072 1c00 0000  .rd...rv...r....
+000015a0: 7280 0000 0072 1d00 0000 da1b 6461 7461  r....r......data
+000015b0: 7365 745f 6672 6f6d 5f69 6d67 5f6d 6173  set_from_img_mas
+000015c0: 6b5f 7061 6972 73e7 0000 0073 1200 0000  k_pairs....s....
+000015d0: 0003 0801 0e02 0e01 0e01 1201 1201 16fb  ................
+000015e0: 04fe 7283 0000 0029 014e 2917 723c 0000  ..r....).N).r<..
+000015f0: 0072 6d00 0000 da09 6675 6e63 746f 6f6c  .rm.....functool
+00001600: 7372 0200 0000 da07 6f73 2e70 6174 6872  sr......os.pathr
+00001610: 0300 0000 5a0a 696d 6167 6569 6f2e 7632  ....Z.imageio.v2
+00001620: da02 7632 723e 0000 0072 4200 0000 7237  ..v2r>...rB...r7
+00001630: 0000 00da 0a74 656e 736f 7266 6c6f 7772  .....tensorflowr
+00001640: 0c00 0000 da0f 736b 696d 6167 652e 6d65  ......skimage.me
+00001650: 6173 7572 6572 0400 0000 721e 0000 0072  asurer....r....r
+00001660: 5400 0000 7256 0000 0072 6500 0000 7273  T...rV...re...rs
+00001670: 0000 0072 7700 0000 727e 0000 0072 8300  ...rw...r~...r..
+00001680: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00001690: 0072 1d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000016a0: 0100 0000 7326 0000 0008 0108 010c 010c  ....s&..........
+000016b0: 020c 0108 0108 010c 0608 100a 4508 2608  ............E.&.
+000016c0: 0106 fc0a 1908 2008 ff0a 0e08 1b08 ff    ...... ........
```

### Comparing `lacss-0.4.0/lacss/data/__pycache__/parser.cpython-38.pyc` & `lacss-0.4.1/lacss/data/__pycache__/parser.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:49:56 2023 UTC, .py size: 9160 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b41e 9764 c823 0000  U..........d.#..
+00000000: 550d 0d0a 0000 0000 af0c 9b64 c823 0000  U..........d.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a04 6412 6407 6408 8401 5a05  d...Z.d.d.d...Z.
 00000050: 6413 6409 640a 8401 5a06 6414 640c 640d  d.d.d...Z.d.d.d.
 00000060: 8401 5a07 640e 640f 8400 5a08 6415 6410  ..Z.d.d...Z.d.d.
 00000070: 6411 8401 5a09 6401 5300 2916 e900 0000  d...Z.d.S.).....
```

### Comparing `lacss-0.4.0/lacss/data/augment.py` & `lacss-0.4.1/lacss/data/augment.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/data/generator.py` & `lacss-0.4.1/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/deploy.py` & `lacss-0.4.1/lacss/deploy.py`

 * *Files 15% similar despite different names*

```diff
@@ -88,14 +88,34 @@
 
 @partial(jax.jit, static_argnums=0)
 def _predict(apply_fn, params, image):
     return apply_fn(dict(params=params), image)
 
 
 class Predictor:
+    """ Main interface for model deployment.
+
+    Attributes:
+        module: The underlying FLAX module 
+        params: Model weights.
+        detector: The detector submodule for convinence. It is common to 
+            modidify this submodule to find optimal parameters for detection.
+            Note this submodule is weight-less.
+    
+    Constructor:
+        url: A URL of the saved model. URLs for build-in pretrained models can be found
+            in lacss.deploy.model_urls
+        precompile_shape: Optionally supply the image shape for precompiling. Otherwise 
+            the model will be recompiled for every new input image shape.
+    
+    Usage Example:
+        url = lacss.deploy.model_urls["livecell"]
+        predictor = lacss.deploy.Predictor(url)
+        label = predictor.predict_label(image)
+    """
     def __init__(self, url, precompile_shape=None):
         self.model = load_from_pretrained(url)
 
         if precompile_shape is not None:
             logging.info("Prcompile the predictor for image shape {precompile_shape}.")
             logging.info("This will take several minutes.")
 
@@ -104,14 +124,16 @@
             except:
                 precompile_shape = [precompile_shape]
             for shape in precompile_shape:
                 x = np.zeros(shape)
                 _ = self.predict(x)
 
     def __call__(self, inputs, **kwargs):
+        """ Perform model prediction
+        """
         inputs_obj = Inputs.from_value(inputs)
 
         return self.predict(*inputs_obj.args, **inputs_obj.kwargs, **kwargs)
 
     def predict(
         self,
         image: Image,
@@ -119,17 +141,19 @@
         remove_out_of_bound: bool = False,
         scaling: float = 1.0,
         **kwargs,
     ):
         """Predict segmentation.
 
         Args:
-            image: ndarray of (h,w,c) format. Value of c must be 1-3
+            image: A ndarray of (h,w,c) format. Value of c must be 1-3
             min_area: Minimum area of a valid prediction. Default is 0
             remove_out_of_bound: Whether to remove out-of-bound predictions. Default is False.
+            scaling: A image scaling factor. If not 1, the input image will be resized internally before fed
+                to the model. The results will be resized back to the scale of the orginal input image.
 
         Returns:
             Raw model prediction as a dict. Most important keys are
 
             instance_output: Segmentation instances. (N, S, S) array
             instance_yc: The meshgrid y-coordinates of the instances. (N, S, S) array
             instance_xc: The meshgrid x-coordinates of the instances. (N, S, S) array
@@ -147,14 +171,19 @@
         if scaling != 1.0:
             h, w, c = image.shape
             image = jax.image.resize(
                 image, [round(h * scaling), round(w * scaling), c], "linear"
             )
 
         preds = _predict(apply_fn, params, image)
+        del preds["encoder_features"]
+        del preds["decoder_features"]
+        del preds["lpn_features"]
+        del preds["lpn_scores"]
+        del preds["lpn_regressions"]
 
         if min_area > 0:
             areas = jnp.count_nonzero(preds["instance_logit"] > 0, axis=(1, 2))
             preds["pred_scores"] = jnp.where(
                 areas > min_area,
                 preds["pred_scores"],
                 -1,
@@ -183,22 +212,45 @@
                 preds["instance_yc"],
                 preds["instance_xc"],
             ) = lacss.ops.rescale_patches(preds, 1 / scaling)
             preds["pred_locations"] = preds["pred_locations"] / scaling
 
         return preds
 
-    def predict_label(self, image, **kwargs):
+    def predict_label(self, image, *, score_threshold=0.5, **kwargs):
+        """ A convinent funciton to obtain prediction in image label format
+
+        Args:
+            image: Input image.
+            score_threshold: The minimal prediction scores. Default is 0.5
+
+        Returns:
+            label: A [H, W] array. The values indicate the id of the cells. For cells
+                with overlapping areas, the pixel is assigned for the cell with higher
+                prediction scores.
+        """
         preds = self.predict(image, **kwargs)
 
-        return patches_to_label(preds, input_size=image.shape[:2])
+        return patches_to_label(
+            preds, 
+            input_size=image.shape[:2], 
+            score_threshold=score_threshold,
+        )
 
     @property
     def module(self):
         return self.model[0]
+    
+    @property
+    def params(self):
+        return self.model[1]
+    
+    @params.setter
+    def params(self, new_params):
+        self.model = self.module, new_params
 
     @property
     def detector(self):
         return self.module.detector
 
     # FIXME Change the detector without first compile the mode will result
     # in error. This is a hidden gotcha. Need to setup warning to the user.
```

### Comparing `lacss-0.4.0/lacss/losses/__pycache__/auxiliary.cpython-38.pyc` & `lacss-0.4.1/lacss/losses/__pycache__/auxiliary.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:13 2023 UTC, .py size: 5248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c51e 9764 8014 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 99e8 9964 8014 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 6d04 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6403 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6505 a00d 6408  d.l.m.Z...e...d.
@@ -198,26 +198,26 @@
 00000c50: ff02 0704 0106 0002 0002 0002 ff06 030e  ................
 00000c60: 011a 0208 010e 0110 0272 5800 0000 6302  .........rX...c.
 00000c70: 0000 0000 0000 0000 0000 0004 0000 0004  ................
 00000c80: 0000 004b 0000 0073 3e00 0000 6401 7c01  ...K...s>...d.|.
 00000c90: 6b06 721c 7c01 6401 1900 6402 6b04 a000  k.r.|.d...d.k...
 00000ca0: 6403 a101 7d03 6e0e 7c01 6404 1900 a000  d...}.n.|.d.....
 00000cb0: 6403 a101 7d03 7401 a002 7c00 6405 1900  d...}.t...|.d...
-00000cc0: 7c03 a102 a003 a100 5300 2906 4eda 0967  |.......S.).N..g
+00000cc0: 7c03 a102 a003 a100 5300 2906 4e5a 0967  |.......S.).NZ.g
 00000cd0: 745f 6c61 6265 6c73 7201 0000 0072 0800  t_labelsr....r..
 00000ce0: 0000 5a07 6774 5f6d 6173 6b72 4100 0000  ..Z.gt_maskrA...
 00000cf0: 2904 722f 0000 0072 2200 0000 da1c 7369  ).r/...r".....si
 00000d00: 676d 6f69 645f 6269 6e61 7279 5f63 726f  gmoid_binary_cro
 00000d10: 7373 5f65 6e74 726f 7079 7224 0000 0029  ss_entropyr$...)
 00000d20: 0472 2500 0000 da06 6c61 6265 6c73 7227  .r%.....labelsr'
 00000d30: 0000 0072 5600 0000 721b 0000 0072 1b00  ...rV...r....r..
 00000d40: 0000 721c 0000 00da 1c73 7570 6572 7669  ..r......supervi
 00000d50: 7365 645f 7365 676d 656e 7461 7469 6f6e  sed_segmentation
 00000d60: 5f6c 6f73 737f 0000 0073 0800 0000 0002  _loss....s......
-00000d70: 0802 1404 0e02 725c 0000 0063 0000 0000  ......r\...c....
+00000d70: 0802 1404 0e02 725b 0000 0063 0000 0000  ......r[...c....
 00000d80: 0000 0000 0000 0000 0000 0000 0300 0000  ................
 00000d90: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
 00000da0: 0265 0365 0364 019c 0264 0264 0384 045a  .e.e.d...d.d...Z
 00000db0: 0464 0453 0029 05da 0b41 7578 4564 6765  .d.S.)...AuxEdge
 00000dc0: 4c6f 7373 2902 7226 0000 0072 2500 0000  Loss).r&...r%...
 00000dd0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
 00000de0: 0003 0000 004b 0000 0073 1600 0000 6401  .....K...s....d.
@@ -228,89 +228,89 @@
 00000e30: 656c 6672 2600 0000 7225 0000 0072 2700  elfr&...r%...r'.
 00000e40: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
 00000e50: 00da 0463 616c 6c8d 0000 0073 0600 0000  ...call....s....
 00000e60: 0006 0801 0402 7a10 4175 7845 6467 654c  ......z.AuxEdgeL
 00000e70: 6f73 732e 6361 6c6c 4e29 05da 085f 5f6e  oss.callN)...__n
 00000e80: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00000e90: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000ea0: 0464 6963 7472 6000 0000 721b 0000 0072  .dictr`...r....r
-00000eb0: 1b00 0000 721b 0000 0072 1c00 0000 725d  ....r....r....r]
+00000ea0: 0464 6963 7472 5f00 0000 721b 0000 0072  .dictr_...r....r
+00000eb0: 1b00 0000 721b 0000 0072 1c00 0000 725c  ....r....r....r\
 00000ec0: 0000 008c 0000 0073 0600 0000 0803 0201  .......s........
-00000ed0: 02fd 725d 0000 0063 0000 0000 0000 0000  ..r]...c........
+00000ed0: 02fd 725c 0000 0063 0000 0000 0000 0000  ..r\...c........
 00000ee0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
 00000ef0: 7326 0000 0065 005a 0164 005a 0264 0687  s&...e.Z.d.Z.d..
 00000f00: 0066 0164 0264 0384 095a 0364 0464 0584  .f.d.d...Z.d.d..
 00000f10: 005a 0487 0004 005a 0553 0029 07da 0b41  .Z.....Z.S.)...A
 00000f20: 7578 5369 7a65 4c6f 7373 724b 0000 0063  uxSizeLossrK...c
 00000f30: 0200 0000 0000 0000 0000 0000 0200 0000  ................
 00000f40: 0200 0000 0300 0000 7314 0000 0074 0083  ........s....t..
 00000f50: 00a0 01a1 0001 007c 017c 005f 0264 0053  .......|.|._.d.S
 00000f60: 0029 014e 2903 da05 7375 7065 72da 085f  .).N)...super.._
-00000f70: 5f69 6e69 745f 5fda 0161 2902 725f 0000  _init__..a).r_..
+00000f70: 5f69 6e69 745f 5fda 0161 2902 725e 0000  _init__..a).r^..
 00000f80: 00da 0561 6c70 6861 a901 da09 5f5f 636c  ...alpha....__cl
 00000f90: 6173 735f 5f72 1b00 0000 721c 0000 0072  ass__r....r....r
-00000fa0: 6700 0000 9a00 0000 7304 0000 0000 010a  g.......s.......
+00000fa0: 6600 0000 9a00 0000 7304 0000 0000 010a  f.......s.......
 00000fb0: 017a 1441 7578 5369 7a65 4c6f 7373 2e5f  .z.AuxSizeLoss._
 00000fc0: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
 00000fd0: 0000 0000 0400 0000 0500 0000 4b00 0000  ............K...
 00000fe0: 7310 0000 0074 007c 027c 017c 006a 0164  s....t.|.|.|.j.d
 00000ff0: 018d 0353 0029 024e 724c 0000 0029 0272  ...S.).NrL...).r
-00001000: 5800 0000 7268 0000 0072 5e00 0000 721b  X...rh...r^...r.
-00001010: 0000 0072 1b00 0000 721c 0000 0072 6000  ...r....r....r`.
+00001000: 5800 0000 7267 0000 0072 5d00 0000 721b  X...rg...r]...r.
+00001010: 0000 0072 1b00 0000 721c 0000 0072 5f00  ...r....r....r_.
 00001020: 0000 9e00 0000 7302 0000 0000 027a 1041  ......s......z.A
 00001030: 7578 5369 7a65 4c6f 7373 2e63 616c 6c29  uxSizeLoss.call)
-00001040: 0172 4b00 0000 a906 7261 0000 0072 6200  .rK.....ra...rb.
-00001050: 0000 7263 0000 0072 6700 0000 7260 0000  ..rc...rg...r`..
+00001040: 0172 4b00 0000 a906 7260 0000 0072 6100  .rK.....r`...ra.
+00001050: 0000 7262 0000 0072 6600 0000 725f 0000  ..rb...rf...r_..
 00001060: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00001070: 721b 0000 0072 1b00 0000 726a 0000 0072  r....r....rj...r
-00001080: 1c00 0000 7265 0000 0099 0000 0073 0400  ....re.......s..
-00001090: 0000 0801 0e04 7265 0000 0063 0000 0000  ......re...c....
+00001070: 721b 0000 0072 1b00 0000 7269 0000 0072  r....r....ri...r
+00001080: 1c00 0000 7264 0000 0099 0000 0073 0400  ....rd.......s..
+00001090: 0000 0801 0e04 7264 0000 0063 0000 0000  ......rd...c....
 000010a0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
 000010b0: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
 000010c0: 0264 0787 0066 0164 0364 0484 095a 0364  .d...f.d.d...Z.d
 000010d0: 0564 0684 005a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
 000010e0: 08da 0a41 7578 5365 674c 6f73 7372 2900  ...AuxSegLossr).
 000010f0: 0000 e700 0000 0000 0014 4063 0300 0000  ..........@c....
 00001100: 0000 0000 0000 0000 0400 0000 0600 0000  ................
 00001110: 0b00 0000 736a 0000 0074 0083 006a 0166  ....sj...t...j.f
 00001120: 007c 038e 0101 007a 0c7c 0164 0119 0001  .|.....z.|.d....
 00001130: 0057 006e 1201 0001 0001 007c 0166 017d  .W.n.......|.f.}
 00001140: 0159 006e 0258 007a 0c7c 0264 0119 0001  .Y.n.X.z.|.d....
 00001150: 0057 006e 1201 0001 0001 007c 0266 017d  .W.n.......|.f.}
 00001160: 0259 006e 0258 0074 02a0 037c 02a1 017c  .Y.n.X.t...|...|
 00001170: 005f 0474 02a0 037c 01a1 017c 005f 0564  ._.t...|...|._.d
-00001180: 0053 0029 024e 7201 0000 0029 0672 6600  .S.).Nr....).rf.
-00001190: 0000 7267 0000 0072 0b00 0000 da05 6172  ..rg...r......ar
+00001180: 0053 0029 024e 7201 0000 0029 0672 6500  .S.).Nr....).re.
+00001190: 0000 7266 0000 0072 0b00 0000 da05 6172  ..rf...r......ar
 000011a0: 7261 7972 2b00 0000 722a 0000 0029 0472  rayr+...r*...).r
-000011b0: 5f00 0000 722a 0000 0072 2b00 0000 7227  _...r*...r+...r'
-000011c0: 0000 0072 6a00 0000 721b 0000 0072 1c00  ...rj...r....r..
-000011d0: 0000 7267 0000 00a4 0000 0073 1600 0000  ..rg.......s....
+000011b0: 5e00 0000 722a 0000 0072 2b00 0000 7227  ^...r*...r+...r'
+000011c0: 0000 0072 6900 0000 721b 0000 0072 1c00  ...ri...r....r..
+000011d0: 0000 7266 0000 00a4 0000 0073 1600 0000  ..rf.......s....
 000011e0: 0001 0e01 0201 0c01 0601 0c02 0201 0c01  ................
 000011f0: 0601 0c02 0c01 7a13 4175 7853 6567 4c6f  ......z.AuxSegLo
 00001200: 7373 2e5f 5f69 6e69 745f 5f63 0300 0000  ss.__init__c....
 00001210: 0000 0000 0000 0000 0400 0000 0600 0000  ................
 00001220: 4b00 0000 7314 0000 0074 007c 027c 017c  K...s....t.|.|.|
 00001230: 006a 017c 006a 0264 018d 0453 0029 024e  .j.|.j.d...S.).N
 00001240: 2902 722b 0000 0072 2a00 0000 2903 724a  ).r+...r*...).rJ
-00001250: 0000 0072 2b00 0000 722a 0000 0072 5e00  ...r+...r*...r^.
+00001250: 0000 0072 2b00 0000 722a 0000 0072 5d00  ...r+...r*...r].
 00001260: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00001270: 0072 6000 0000 b300 0000 730c 0000 0000  .r`.......s.....
+00001270: 0072 5f00 0000 b300 0000 730c 0000 0000  .r_.......s.....
 00001280: 0202 0102 0102 0104 0104 fc7a 0f41 7578  ...........z.Aux
 00001290: 5365 674c 6f73 732e 6361 6c6c 2902 7229  SegLoss.call).r)
-000012a0: 0000 0072 6f00 0000 726c 0000 0072 1b00  ...ro...rl...r..
-000012b0: 0000 721b 0000 0072 6a00 0000 721c 0000  ..r....rj...r...
-000012c0: 0072 6e00 0000 a300 0000 7304 0000 0008  .rn.......s.....
-000012d0: 010e 0f72 6e00 0000 2919 da09 6675 6e63  ...rn...)...func
+000012a0: 0000 0072 6e00 0000 726b 0000 0072 1b00  ...rn...rk...r..
+000012b0: 0000 721b 0000 0072 6900 0000 721c 0000  ..r....ri...r...
+000012c0: 0072 6d00 0000 a300 0000 7304 0000 0008  .rm.......s.....
+000012d0: 010e 0f72 6d00 0000 2919 da09 6675 6e63  ...rm...)...func
 000012e0: 746f 6f6c 7372 0200 0000 721f 0000 00da  toolsr....r.....
 000012f0: 096a 6178 2e6e 756d 7079 da05 6e75 6d70  .jax.numpy..nump
 00001300: 7972 0b00 0000 7222 0000 00da 036f 7073  yr....r".....ops
 00001310: 7204 0000 005a 0a74 7261 696e 2e6c 6f73  r....Z.train.los
 00001320: 7372 0500 0000 da09 6465 7465 6374 696f  sr......detectio
 00001330: 6e72 0700 0000 da05 6669 6e66 6fda 0365  nr......finfo..e
 00001340: 7073 7252 0000 0072 1d00 0000 7228 0000  psrR...r....r(..
-00001350: 0072 7000 0000 724a 0000 0072 5800 0000  .rp...rJ...rX...
-00001360: 725c 0000 0072 5d00 0000 7265 0000 0072  r\...r]...re...r
-00001370: 6e00 0000 721b 0000 0072 1b00 0000 721b  n...r....r....r.
+00001350: 0072 6f00 0000 724a 0000 0072 5800 0000  .ro...rJ...rX...
+00001360: 725b 0000 0072 5c00 0000 7264 0000 0072  r[...r\...rd...r
+00001370: 6d00 0000 721b 0000 0072 1b00 0000 721b  m...r....r....r.
 00001380: 0000 0072 1c00 0000 da08 3c6d 6f64 756c  ...r......<modul
 00001390: 653e 0100 0000 7322 0000 000c 0208 010c  e>....s"........
 000013a0: 0108 020c 010c 010c 020c 0308 1408 130a  ................
 000013b0: 010a fb0c 350e 1908 0d10 0d10 0a         ....5........
```

### Comparing `lacss-0.4.0/lacss/losses/__pycache__/detection.cpython-38.pyc` & `lacss-0.4.1/lacss/losses/__pycache__/detection.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 15:28:24 2023 UTC, .py size: 2423 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 98ae 9964 7709 0000  U..........dw...
+00000000: 550d 0d0a 0000 0000 99e8 9964 7709 0000  U..........dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6404 6405 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6504 6a08 5a09 6509 a00a 6406 a101  ..e.j.Z.e...d...
 00000070: 6a0b 5a0c 6417 6408 6409 8401 5a0d 6418  j.Z.d.d.d...Z.d.
```

### Comparing `lacss-0.4.0/lacss/losses/__pycache__/instance.cpython-38.pyc` & `lacss-0.4.1/lacss/losses/__pycache__/instance.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 11:55:46 2023 UTC, .py size: 5493 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c27c 9964 7515 0000  U........|.du...
+00000000: 550d 0d0a 0000 0000 9c30 9b64 e115 0000  U........0.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 6d04 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6403 6405 6c09 6d0a 5a0a 0100 6505  ..d.d.l.m.Z...e.
 00000070: a00b 6406 a101 6a0c 5a0d 6407 6408 8400  ..d...j.Z.d.d...
@@ -36,274 +36,272 @@
 00000230: 6a5f 6c61 6373 732f 6c61 6373 732f 6c61  j_lacss/lacss/la
 00000240: 6373 732f 6c6f 7373 6573 2f69 6e73 7461  css/losses/insta
 00000250: 6e63 652e 7079 da17 5f6d 6561 6e5f 6f76  nce.py.._mean_ov
 00000260: 6572 5f62 6f6f 6c65 616e 5f6d 6173 6b0d  er_boolean_mask.
 00000270: 0000 0073 0c00 0000 0001 1201 0e02 1201  ...s............
 00000280: 1601 0802 7218 0000 0063 0200 0000 0000  ....r....c......
 00000290: 0000 0000 0000 1500 0000 0600 0000 4b00  ..............K.
-000002a0: 0000 73a8 0100 007c 0064 0119 007d 037c  ..s....|.d...}.|
+000002a0: 0000 73a4 0100 007c 0064 0119 007d 037c  ..s....|.d...}.|
 000002b0: 0064 0219 007d 047c 0064 0319 007d 057c  .d...}.|.d...}.|
 000002c0: 0064 0419 007d 0674 007c 0174 0183 0273  .d...}.t.|.t...s
 000002d0: 3474 017c 0164 058d 017d 0164 067c 016b  4t.|.d...}.d.|.k
 000002e0: 0672 aa7c 0164 0619 00a0 0264 07a1 017d  .r.|.d.....d...}
 000002f0: 077c 056a 035c 037d 087d 097d 0a74 04a0  .|.j.\.}.}.}.t..
 00000300: 057c 077c 0964 081a 00a1 027d 077c 077c  .|.|.d.....}.|.|
 00000310: 057c 0964 081a 0017 007c 067c 0964 081a  .|.d.....|.|.d..
 00000320: 0017 0066 0219 0074 04a0 067c 08a1 0164  ...f...t...|...d
 00000330: 0964 0985 0264 0964 0966 0319 0064 0a17  .d...d.d.f...d..
-00000340: 006b 027d 0b7c 0ba0 0274 07a1 017d 0b6e  .k.}.|...t...}.n
-00000350: e874 04a0 087c 0164 0b19 0064 0c64 0aa1  .t...|.d...d.d..
-00000360: 035c 047d 0c7d 0d7d 0e7d 0f7c 0164 0d19  .\.}.}.}.}.|.d..
-00000370: 007d 1074 097c 106a 0383 0164 0e6b 0272  .}.t.|.j...d.k.r
-00000380: e47c 10a0 0a64 0fa1 017d 107c 106a 0364  .|...d...}.|.j.d
+00000340: 006b 027d 0b7c 0ba0 0264 0ba1 017d 0b6e  .k.}.|...d...}.n
+00000350: e474 04a0 077c 0164 0c19 0064 0d64 0aa1  .t...|.d...d.d..
+00000360: 035c 047d 0c7d 0d7d 0e7d 0f7c 0164 0e19  .\.}.}.}.}.|.d..
+00000370: 007d 1074 087c 106a 0383 0164 0f6b 0272  .}.t.|.j...d.k.r
+00000380: e47c 10a0 0964 10a1 017d 107c 106a 0364  .|...d...}.|.j.d
 00000390: 0a19 007d 117c 0e7c 0c18 007c 111b 007d  ...}.|.|...|...}
 000003a0: 127c 0f7c 0d18 007c 111b 007d 137c 057c  .|.|...|...}.|.|
 000003b0: 0c64 0964 0985 0264 0964 0966 0319 0018  .d.d...d.d.f....
-000003c0: 0064 1017 007c 1264 0964 0985 0264 0964  .d...|.d.d...d.d
+000003c0: 0064 1117 007c 1264 0964 0985 0264 0964  .d...|.d.d...d.d
 000003d0: 0966 0319 001b 007d 057c 067c 0d64 0964  .f.....}.|.|.d.d
-000003e0: 0985 0264 0964 0966 0319 0018 0064 1017  ...d.d.f.....d..
+000003e0: 0985 0264 0964 0966 0319 0018 0064 1117  ...d.d.f.....d..
 000003f0: 007c 1364 0964 0985 0264 0964 0966 0319  .|.d.d...d.d.f..
-00000400: 001b 007d 0674 0ba0 0c74 0d74 0e64 1164  ...}.t...t.t.d.d
-00000410: 128d 02a1 017c 1074 046a 0f7c 057c 0667  .....|.t.j.|.|.g
-00000420: 0264 0f64 138d 0283 027d 0b7c 0b64 106b  .d.d.....}.|.d.k
-00000430: 05a0 0274 07a1 017d 0b74 10a0 117c 047c  ...t...}.t...|.|
-00000440: 0ba1 027d 1474 127c 147c 0383 0253 0029  ...}.t.|.|...S.)
-00000450: 147a 374c 4143 5353 2069 6e73 7461 6e63  .z7LACSS instanc
-00000460: 6520 6c6f 7373 2c20 7375 7065 7276 6973  e loss, supervis
-00000470: 6564 2077 6974 6820 7365 676d 656e 7461  ed with segmenta
-00000480: 7469 6f6e 206c 6162 656c da0d 696e 7374  tion label..inst
-00000490: 616e 6365 5f6d 6173 6bda 0e69 6e73 7461  ance_mask..insta
-000004a0: 6e63 655f 6c6f 6769 74da 0b69 6e73 7461  nce_logit..insta
-000004b0: 6e63 655f 7963 da0b 696e 7374 616e 6365  nce_yc..instance
-000004c0: 5f78 6329 01da 0967 745f 6c61 6265 6c73  _xc)...gt_labels
-000004d0: 721d 0000 00da 0569 6e74 3332 7203 0000  r......int32r...
-000004e0: 004e 7207 0000 00da 0967 745f 6262 6f78  .Nr......gt_bbox
-000004f0: 6573 7201 0000 00da 0867 745f 6d61 736b  esr......gt_mask
-00000500: 73e9 0400 0000 7208 0000 00e7 0000 0000  s.....r.........
-00000510: 0000 e03f 5429 01da 0d65 6467 655f 696e  ...?T)...edge_in
-00000520: 6465 7869 6e67 2901 7209 0000 0029 13da  dexing).r....)..
-00000530: 0a69 7369 6e73 7461 6e63 65da 0464 6963  .isinstance..dic
-00000540: 74da 0661 7374 7970 6572 0d00 0000 720e  t..astyper....r.
-00000550: 0000 00da 0370 6164 da06 6172 616e 6765  .....pad..arange
-00000560: da03 696e 74da 0873 7761 7061 7865 73da  ..int..swapaxes.
-00000570: 036c 656e da07 7371 7565 657a 65da 036a  .len..squeeze..j
-00000580: 6178 da04 766d 6170 7202 0000 0072 0400  ax..vmapr....r..
-00000590: 0000 da05 7374 6163 6bda 056f 7074 6178  ....stack..optax
-000005a0: da1c 7369 676d 6f69 645f 6269 6e61 7279  ..sigmoid_binary
-000005b0: 5f63 726f 7373 5f65 6e74 726f 7079 7218  _cross_entropyr.
-000005c0: 0000 0029 15da 0570 7265 6473 da06 6c61  ...)...preds..la
-000005d0: 6265 6c73 da06 6b77 6172 6773 7219 0000  bels..kwargsr...
-000005e0: 0072 1a00 0000 da02 7963 da02 7863 721d  .r......yc..xcr.
-000005f0: 0000 00da 096e 5f70 6174 6368 6573 da02  .....n_patches..
-00000600: 7073 da01 5fda 0a67 745f 7061 7463 6865  ps.._..gt_patche
-00000610: 73da 0279 30da 0278 30da 0279 31da 0278  s..y0..x0..y1..x
-00000620: 315a 0767 745f 7365 6773 5a08 7365 675f  1Z.gt_segsZ.seg_
-00000630: 7369 7a65 da02 6873 da02 7773 7213 0000  size..hs..wsr...
-00000640: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000650: da18 7375 7065 7276 6973 6564 5f69 6e73  ..supervised_ins
-00000660: 7461 6e63 655f 6c6f 7373 1800 0000 733c  tance_loss....s<
-00000670: 0000 0000 0308 0108 0108 0108 020a 010a  ................
-00000680: 0208 010e 020c 0210 011a 011a ff04 030c  ................
-00000690: 031a 0108 010e 010a 010a 030c 010c 032c  ...............,
-000006a0: 012c 0310 0102 0110 fe04 040e 020c 0272  .,.............r
-000006b0: 4100 0000 54a9 01da 0a73 6f66 745f 6c61  A...T....soft_la
-000006c0: 6265 6c63 0100 0000 0000 0000 0100 0000  belc............
-000006d0: 1100 0000 0600 0000 4300 0000 735e 0100  ........C...s^..
-000006e0: 007c 0064 0119 007d 027c 0064 0219 007d  .|.d...}.|.d...}
-000006f0: 037c 0064 0319 007d 047c 0064 0419 007d  .|.d...}.|.d...}
-00000700: 057c 0064 0519 007d 067c 036a 0064 0619  .|.d...}.|.j.d..
-00000710: 007d 077c 0764 071a 0064 0717 007d 087c  .}.|.d...d...}.|
-00000720: 057c 0837 007d 057c 067c 0837 007d 0674  .|.7.}.|.|.7.}.t
-00000730: 016a 02a0 0374 016a 04a0 057c 0064 0819  .j...t.j...|.d..
-00000740: 00a1 01a1 017d 0974 06a0 077c 097c 08a1  .....}.t...|.|..
-00000750: 027d 0a7c 0172 d67c 0a7c 057c 0666 0219  .}.|.r.|.|.|.f..
-00000760: 007d 0b64 097c 0b18 007c 0314 007c 0b64  .}.d.|...|...|.d
-00000770: 097c 0318 0014 0017 007d 0c74 06a0 087c  .|.......}.t...|
-00000780: 0aa1 017d 0d7c 0d6a 097c 057c 0666 0219  ...}.|.j.|.|.f..
-00000790: 00a0 0a7c 03a1 017d 0d7c 0d7c 057c 0666  ...|...}.|.|.|.f
-000007a0: 0219 007c 0318 007d 0e7c 0c7c 037c 0e14  ...|...}.|.|.|..
-000007b0: 0017 007d 0c6e 7e7c 0a64 0a6b 04a0 0b7c  ...}.n~|.d.k...|
-000007c0: 036a 0ca1 017d 0a7c 0a7c 057c 0666 0219  .j...}.|.|.|.f..
-000007d0: 007d 0b64 097c 0b18 007c 0314 007c 0b64  .}.d.|...|...|.d
-000007e0: 097c 0318 0014 0017 007d 0c74 06a0 087c  .|.......}.t...|
-000007f0: 0aa1 017d 0f74 016a 04a0 0d7c 040b 00a1  ...}.t.j...|....
-00000800: 010b 007d 107c 0f6a 097c 057c 0666 0219  ...}.|.j.|.|.f..
-00000810: 00a0 0a7c 10a1 017d 0f7c 0f7c 057c 0666  ...|...}.|.|.|.f
-00000820: 0219 007c 1018 007d 107c 0c7c 037c 1014  ...|...}.|.|.|..
-00000830: 0017 007d 0c74 0e7c 0c7c 0283 0253 0029  ...}.t.|.|...S.)
-00000840: 0b7a 214c 4143 5353 2069 6e73 7461 6e63  .z!LACSS instanc
-00000850: 6520 6c6f 7373 2c20 756e 7375 7065 7276  e loss, unsuperv
-00000860: 6973 6564 7219 0000 00da 0f69 6e73 7461  isedr......insta
-00000870: 6e63 655f 6f75 7470 7574 721a 0000 0072  nce_outputr....r
-00000880: 1b00 0000 721c 0000 0072 0800 0000 7203  ....r....r....r.
-00000890: 0000 00da 0766 675f 7072 6564 e700 0000  .....fg_pred....
-000008a0: 0000 00f0 3f72 2200 0000 290f 720d 0000  ....?r"...).r...
-000008b0: 0072 2d00 0000 da03 6c61 78da 0d73 746f  .r-.....lax..sto
-000008c0: 705f 6772 6164 6965 6e74 da02 6e6e da07  p_gradient..nn..
-000008d0: 7369 676d 6f69 6472 0e00 0000 7227 0000  sigmoidr....r'..
-000008e0: 00da 0a7a 6572 6f73 5f6c 696b 65da 0261  ...zeros_like..a
-000008f0: 74da 0361 6464 7226 0000 00da 0564 7479  t..addr&.....dty
-00000900: 7065 da0b 6c6f 675f 7369 676d 6f69 6472  pe..log_sigmoidr
-00000910: 1800 0000 2911 7232 0000 0072 4300 0000  ....).r2...rC...
-00000920: 7219 0000 00da 0969 6e73 7461 6e63 6573  r......instances
-00000930: 721a 0000 0072 3500 0000 7236 0000 00da  r....r5...r6....
-00000940: 0a70 6174 6368 5f73 697a 65da 0c70 6164  .patch_size..pad
-00000950: 6469 6e67 5f73 697a 65da 0b62 696e 6172  ding_size..binar
-00000960: 795f 6d61 736b da03 7365 67da 0973 6567  y_mask..seg..seg
-00000970: 5f70 6174 6368 7213 0000 005a 0c69 6e73  _patchr....Z.ins
-00000980: 7461 6e63 655f 7375 6d5a 0e69 6e73 7461  tance_sumZ.insta
-00000990: 6e63 655f 7375 6d5f 69da 0a6c 6f67 5f79  nce_sum_i..log_y
-000009a0: 695f 7375 6dda 066c 6f67 5f79 6972 1600  i_sum..log_yir..
-000009b0: 0000 7216 0000 0072 1700 0000 da1d 7365  ..r....r......se
-000009c0: 6c66 5f73 7570 6572 7669 7365 645f 696e  lf_supervised_in
-000009d0: 7374 616e 6365 5f6c 6f73 7349 0000 0073  stance_lossI...s
-000009e0: 3600 0000 0003 0801 0801 0801 0801 0802  6...............
-000009f0: 0a01 0c01 0801 0802 1801 0c02 0401 0c02  ................
-00000a00: 1802 0a01 1401 1002 0e03 1001 0c02 1802  ................
-00000a10: 0a01 1001 1401 1002 0c02 7258 0000 0046  ..........rX...F
-00000a20: a901 da0b 6967 6e6f 7265 5f6d 6173 6b63  ....ignore_maskc
-00000a30: 0300 0000 0000 0000 0100 0000 1100 0000  ................
-00000a40: 0500 0000 4b00 0000 732a 0100 007c 0064  ....K...s*...|.d
-00000a50: 0119 007d 057c 0064 0219 007d 067c 0064  ...}.|.d...}.|.d
-00000a60: 0319 007d 077c 0064 0419 007d 087c 0064  ...}.|.d...}.|.d
-00000a70: 0519 007d 097c 066a 0064 0619 007d 0a7c  ...}.|.j.d...}.|
-00000a80: 0a64 071a 0064 0717 007d 0b7c 087c 0b37  .d...d...}.|.|.7
-00000a90: 007d 087c 097c 0b37 007d 097c 0372 8274  .}.|.|.7.}.|.r.t
-00000aa0: 01a0 027c 0264 0819 006a 0064 0964 0685  ...|.d...j.d.d..
-00000ab0: 0219 00a1 017d 0c74 01a0 037c 0c7c 0ba1  .....}.t...|.|..
-00000ac0: 027d 0c74 01a0 047c 06a1 017d 0d6e 5474  .}.t...|...}.nTt
-00000ad0: 057c 0174 0683 0272 9c7c 0164 0a19 00a0  .|.t...r.|.d....
-00000ae0: 0764 0ba1 017d 0c6e 0a7c 01a0 0764 0ba1  .d...}.n.|...d..
-00000af0: 017d 0c74 01a0 037c 0c7c 0ba1 027d 0c7c  .}.t...|.|...}.|
-00000b00: 0c7c 087c 0966 0219 007d 0e64 0c7c 0e18  .|.|.f...}.d.|..
-00000b10: 007c 0614 007c 0e64 0c7c 0618 0014 0017  .|...|.d.|......
-00000b20: 007d 0d74 01a0 047c 0ca1 017d 0f74 086a  .}.t...|...}.t.j
-00000b30: 09a0 0a7c 070b 00a1 010b 007d 107c 0f6a  ...|.......}.|.j
-00000b40: 0b7c 087c 0966 0219 00a0 0c7c 10a1 017d  .|.|.f.....|...}
-00000b50: 0f7c 0f7c 087c 0966 0219 007c 1018 007d  .|.|.|.f...|...}
-00000b60: 107c 0d7c 067c 1014 0017 007d 0d74 0d7c  .|.|.|.....}.t.|
-00000b70: 0d7c 0583 0253 0029 0d7a 2f4c 6163 7373  .|...S.).z/Lacss
-00000b80: 2069 6e73 7461 6e63 6520 6c6f 7373 2c20   instance loss, 
-00000b90: 7375 7065 7276 6973 6564 2077 6974 6820  supervised with 
-00000ba0: 696d 6167 6520 6d61 736b 7219 0000 0072  image maskr....r
-00000bb0: 4400 0000 721a 0000 0072 1b00 0000 721c  D...r....r....r.
-00000bc0: 0000 0072 0800 0000 7203 0000 00da 0569  ...r....r......i
-00000bd0: 6d61 6765 4eda 0767 745f 6d61 736b 7206  mageN..gt_maskr.
-00000be0: 0000 0072 4600 0000 290e 720d 0000 0072  ...rF...).r....r
-00000bf0: 0e00 0000 da05 7a65 726f 7372 2700 0000  ......zerosr'...
-00000c00: 724b 0000 0072 2400 0000 7225 0000 0072  rK...r$...r%...r
-00000c10: 2600 0000 722d 0000 0072 4900 0000 724f  &...r-...rI...rO
-00000c20: 0000 0072 4c00 0000 724d 0000 0072 1800  ...rL...rM...r..
-00000c30: 0000 2911 7232 0000 0072 3300 0000 da06  ..).r2...r3.....
-00000c40: 696e 7075 7473 725a 0000 0072 3400 0000  inputsrZ...r4...
-00000c50: 7219 0000 0072 5000 0000 721a 0000 0072  r....rP...r....r
-00000c60: 3500 0000 7236 0000 0072 5100 0000 7252  5...r6...rQ...rR
-00000c70: 0000 0072 5400 0000 7213 0000 0072 5500  ...rT...r....rU.
-00000c80: 0000 7256 0000 0072 5700 0000 7216 0000  ..rV...rW...r...
-00000c90: 0072 1600 0000 7217 0000 00da 1f77 6561  .r....r......wea
-00000ca0: 6b6c 795f 7375 7065 7276 6973 6564 5f69  kly_supervised_i
-00000cb0: 6e73 7461 6e63 655f 6c6f 7373 7500 0000  nstance_lossu...
-00000cc0: 7332 0000 0000 0508 0108 0108 0108 0108  s2..............
-00000cd0: 020a 010c 0108 0108 0204 0118 010c 010c  ................
-00000ce0: 020a 0110 020a 010c 010c 0118 020a 0210  ................
-00000cf0: 0114 0110 020c 0272 5f00 0000 6300 0000  .......r_...c...
-00000d00: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000d10: 0040 0000 0073 1c00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000d20: 5a02 6503 6503 6401 9c02 6402 6403 8404  Z.e.e.d...d.d...
-00000d30: 5a04 6404 5300 2905 da16 5375 7065 7276  Z.d.S.)...Superv
-00000d40: 6973 6564 496e 7374 616e 6365 4c6f 7373  isedInstanceLoss
-00000d50: 2902 7232 0000 0072 3300 0000 6303 0000  ).r2...r3...c...
-00000d60: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-00000d70: 004b 0000 0073 0a00 0000 7400 7c01 7c02  .K...s....t.|.|.
-00000d80: 8302 5300 a901 4e29 0172 4100 0000 2904  ..S...N).rA...).
-00000d90: da04 7365 6c66 7232 0000 0072 3300 0000  ..selfr2...r3...
-00000da0: 7234 0000 0072 1600 0000 7216 0000 0072  r4...r....r....r
-00000db0: 1700 0000 da04 6361 6c6c 9e00 0000 7302  ......call....s.
-00000dc0: 0000 0000 017a 1b53 7570 6572 7669 7365  .....z.Supervise
-00000dd0: 6449 6e73 7461 6e63 654c 6f73 732e 6361  dInstanceLoss.ca
-00000de0: 6c6c 4e29 05da 085f 5f6e 616d 655f 5fda  llN)...__name__.
-00000df0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000e00: 7561 6c6e 616d 655f 5f72 2500 0000 7263  ualname__r%...rc
-00000e10: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-00000e20: 0000 7217 0000 0072 6000 0000 9d00 0000  ..r....r`.......
-00000e30: 7302 0000 0008 0172 6000 0000 6300 0000  s......r`...c...
-00000e40: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00000e50: 0000 0000 0073 3200 0000 6500 5a01 6400  .....s2...e.Z.d.
-00000e60: 5a02 6408 6503 6402 9c01 8700 6601 6403  Z.d.e.d.....f.d.
-00000e70: 6404 840d 5a04 6505 6405 9c01 6406 6407  d...Z.e.d...d.d.
-00000e80: 8404 5a06 8700 0400 5a07 5300 2909 da1a  ..Z.....Z.S.)...
-00000e90: 5365 6c66 5375 7065 7276 6973 6564 496e  SelfSupervisedIn
-00000ea0: 7374 616e 6365 4c6f 7373 5472 4200 0000  stanceLossTrB...
-00000eb0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00000ec0: 0003 0000 000f 0000 0073 1800 0000 7400  .........s....t.
-00000ed0: 8300 6a01 7c02 7c03 8e01 0100 7c01 7c00  ..j.|.|.....|.|.
-00000ee0: 5f02 6400 5300 7261 0000 0029 03da 0573  _.d.S.ra...)...s
-00000ef0: 7570 6572 da08 5f5f 696e 6974 5f5f 7243  uper..__init__rC
-00000f00: 0000 0029 0472 6200 0000 7243 0000 00da  ...).rb...rC....
-00000f10: 0461 7267 7372 3400 0000 a901 da09 5f5f  .argsr4.......__
-00000f20: 636c 6173 735f 5f72 1600 0000 7217 0000  class__r....r...
-00000f30: 0072 6900 0000 a300 0000 7304 0000 0000  .ri.......s.....
-00000f40: 010e 017a 2353 656c 6653 7570 6572 7669  ...z#SelfSupervi
-00000f50: 7365 6449 6e73 7461 6e63 654c 6f73 732e  sedInstanceLoss.
-00000f60: 5f5f 696e 6974 5f5f 2901 7232 0000 0063  __init__).r2...c
-00000f70: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000f80: 0400 0000 4b00 0000 730e 0000 0074 007c  ....K...s....t.|
-00000f90: 017c 006a 0164 018d 0253 0029 024e 7242  .|.j.d...S.).NrB
-00000fa0: 0000 0029 0272 5800 0000 7243 0000 0029  ...).rX...rC...)
-00000fb0: 0372 6200 0000 7232 0000 0072 3400 0000  .rb...r2...r4...
-00000fc0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000fd0: 6300 0000 a700 0000 7302 0000 0000 017a  c.......s......z
-00000fe0: 1f53 656c 6653 7570 6572 7669 7365 6449  .SelfSupervisedI
-00000ff0: 6e73 7461 6e63 654c 6f73 732e 6361 6c6c  nstanceLoss.call
-00001000: 2901 5429 0872 6400 0000 7265 0000 0072  ).T).rd...re...r
-00001010: 6600 0000 da04 626f 6f6c 7269 0000 0072  f.....boolri...r
-00001020: 2500 0000 7263 0000 00da 0d5f 5f63 6c61  %...rc.....__cla
-00001030: 7373 6365 6c6c 5f5f 7216 0000 0072 1600  sscell__r....r..
-00001040: 0000 726b 0000 0072 1700 0000 7267 0000  ..rk...r....rg..
-00001050: 00a2 0000 0073 0400 0000 0801 1404 7267  .....s........rg
-00001060: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001070: 0000 0000 0500 0000 0000 0000 732c 0000  ............s,..
-00001080: 0065 005a 0164 005a 0264 0765 0364 029c  .e.Z.d.Z.d.e.d..
-00001090: 0187 0066 0164 0364 0484 0d5a 0464 0564  ...f.d.d...Z.d.d
-000010a0: 0684 005a 0587 0004 005a 0653 0029 08da  ...Z.....Z.S.)..
-000010b0: 1c57 6561 6b6c 7953 7570 6572 7669 7365  .WeaklySupervise
-000010c0: 6449 6e73 7461 6e63 654c 6f73 7346 7259  dInstanceLossFrY
-000010d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000010e0: 0400 0000 0300 0000 0f00 0000 7318 0000  ............s...
-000010f0: 0074 0083 006a 017c 027c 038e 0101 007c  .t...j.|.|.....|
-00001100: 017c 005f 0264 0053 0072 6100 0000 2903  .|._.d.S.ra...).
-00001110: 7268 0000 0072 6900 0000 725a 0000 0029  rh...ri...rZ...)
-00001120: 0472 6200 0000 725a 0000 0072 6a00 0000  .rb...rZ...rj...
-00001130: 7234 0000 0072 6b00 0000 7216 0000 0072  r4...rk...r....r
-00001140: 1700 0000 7269 0000 00ac 0000 0073 0400  ....ri.......s..
-00001150: 0000 0001 0e01 7a25 5765 616b 6c79 5375  ......z%WeaklySu
-00001160: 7065 7276 6973 6564 496e 7374 616e 6365  pervisedInstance
-00001170: 4c6f 7373 2e5f 5f69 6e69 745f 5f63 0100  Loss.__init__c..
-00001180: 0000 0000 0000 0300 0000 0400 0000 0600  ................
-00001190: 0000 4300 0000 7312 0000 0074 007c 017c  ..C...s....t.|.|
-000011a0: 027c 037c 006a 0164 018d 0453 0029 024e  .|.|.j.d...S.).N
-000011b0: 7259 0000 0029 0272 5f00 0000 725a 0000  rY...).r_...rZ..
-000011c0: 0029 0472 6200 0000 7232 0000 0072 3300  .).rb...r2...r3.
-000011d0: 0000 725e 0000 0072 1600 0000 7216 0000  ..r^...r....r...
-000011e0: 0072 1700 0000 7263 0000 00b0 0000 0073  .r....rc.......s
-000011f0: 0c00 0000 0001 0201 0200 0200 0200 04ff  ................
-00001200: 7a21 5765 616b 6c79 5375 7065 7276 6973  z!WeaklySupervis
-00001210: 6564 496e 7374 616e 6365 4c6f 7373 2e63  edInstanceLoss.c
-00001220: 616c 6c29 0146 2907 7264 0000 0072 6500  all).F).rd...re.
-00001230: 0000 7266 0000 0072 6d00 0000 7269 0000  ..rf...rm...ri..
-00001240: 0072 6300 0000 726e 0000 0072 1600 0000  .rc...rn...r....
-00001250: 7216 0000 0072 6b00 0000 7217 0000 0072  r....rk...r....r
-00001260: 6f00 0000 ab00 0000 7304 0000 0008 0114  o.......s.......
-00001270: 0472 6f00 0000 2916 da09 6675 6e63 746f  .ro...)...functo
-00001280: 6f6c 7372 0200 0000 722d 0000 00da 096a  olsr....r-.....j
-00001290: 6178 2e6e 756d 7079 da05 6e75 6d70 7972  ax.numpy..numpyr
-000012a0: 0e00 0000 7230 0000 00da 036f 7073 7204  ....r0.....opsr.
-000012b0: 0000 00da 0a74 7261 696e 2e6c 6f73 7372  .....train.lossr
-000012c0: 0500 0000 da05 6669 6e66 6fda 0365 7073  ......finfo..eps
-000012d0: 7210 0000 0072 1800 0000 7241 0000 0072  r....r....rA...r
-000012e0: 6d00 0000 7258 0000 0072 5f00 0000 7260  m...rX...r_...r`
-000012f0: 0000 0072 6700 0000 726f 0000 0072 1600  ...rg...ro...r..
-00001300: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001310: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00001320: 2000 0000 0c02 0801 0c01 0802 0c01 0c02   ...............
-00001330: 0c03 080b 0831 142d 02ff 0401 02ff 0c28  .....1.-.......(
-00001340: 1005 1009                                ....
+00000400: 001b 007d 0674 0aa0 0b74 0ca1 017c 1074  ...}.t...t...|.t
+00000410: 046a 0d7c 057c 0667 0264 1064 128d 0264  .j.|.|.g.d.d...d
+00000420: 1118 0083 027d 0b7c 0b64 116b 05a0 0264  .....}.|.d.k...d
+00000430: 0ba1 017d 0b74 0ea0 0f7c 047c 0ba1 027d  ...}.t...|.|...}
+00000440: 1474 107c 147c 0383 0253 0029 137a 374c  .t.|.|...S.).z7L
+00000450: 4143 5353 2069 6e73 7461 6e63 6520 6c6f  ACSS instance lo
+00000460: 7373 2c20 7375 7065 7276 6973 6564 2077  ss, supervised w
+00000470: 6974 6820 7365 676d 656e 7461 7469 6f6e  ith segmentation
+00000480: 206c 6162 656c da0d 696e 7374 616e 6365   label..instance
+00000490: 5f6d 6173 6bda 0e69 6e73 7461 6e63 655f  _mask..instance_
+000004a0: 6c6f 6769 74da 0b69 6e73 7461 6e63 655f  logit..instance_
+000004b0: 7963 da0b 696e 7374 616e 6365 5f78 6329  yc..instance_xc)
+000004c0: 01da 0967 745f 6c61 6265 6c73 721d 0000  ...gt_labelsr...
+000004d0: 00da 0569 6e74 3332 7203 0000 004e 7207  ...int32r....Nr.
+000004e0: 0000 0072 0600 0000 5a09 6774 5f62 626f  ...r....Z.gt_bbo
+000004f0: 7865 7372 0100 0000 da08 6774 5f6d 6173  xesr......gt_mas
+00000500: 6b73 e904 0000 0072 0800 0000 e700 0000  ks.....r........
+00000510: 0000 00e0 3f29 0172 0900 0000 2911 da0a  ....?).r....)...
+00000520: 6973 696e 7374 616e 6365 da04 6469 6374  isinstance..dict
+00000530: da06 6173 7479 7065 720d 0000 0072 0e00  ..astyper....r..
+00000540: 0000 da03 7061 64da 0661 7261 6e67 65da  ....pad..arange.
+00000550: 0873 7761 7061 7865 73da 036c 656e da07  .swapaxes..len..
+00000560: 7371 7565 657a 65da 036a 6178 da04 766d  squeeze..jax..vm
+00000570: 6170 7204 0000 00da 0573 7461 636b da05  apr......stack..
+00000580: 6f70 7461 78da 1c73 6967 6d6f 6964 5f62  optax..sigmoid_b
+00000590: 696e 6172 795f 6372 6f73 735f 656e 7472  inary_cross_entr
+000005a0: 6f70 7972 1800 0000 2915 da05 7072 6564  opyr....)...pred
+000005b0: 73da 066c 6162 656c 73da 066b 7761 7267  s..labels..kwarg
+000005c0: 7372 1900 0000 721a 0000 00da 0279 63da  sr....r......yc.
+000005d0: 0278 6372 1d00 0000 da09 6e5f 7061 7463  .xcr......n_patc
+000005e0: 6865 73da 0270 73da 015f da0a 6774 5f70  hes..ps.._..gt_p
+000005f0: 6174 6368 6573 da02 7930 da02 7830 da02  atches..y0..x0..
+00000600: 7931 da02 7831 5a07 6774 5f73 6567 735a  y1..x1Z.gt_segsZ
+00000610: 0873 6567 5f73 697a 65da 0268 73da 0277  .seg_size..hs..w
+00000620: 7372 1300 0000 7216 0000 0072 1600 0000  sr....r....r....
+00000630: 7217 0000 00da 1873 7570 6572 7669 7365  r......supervise
+00000640: 645f 696e 7374 616e 6365 5f6c 6f73 7318  d_instance_loss.
+00000650: 0000 0073 3c00 0000 0003 0801 0801 0801  ...s<...........
+00000660: 0802 0a01 0a02 0801 0e02 0c02 1001 1a01  ................
+00000670: 1aff 0403 0c03 1a01 0801 0e01 0a01 0a03  ................
+00000680: 0c01 0c03 2c01 2c03 0801 0201 14fe 0404  ....,.,.........
+00000690: 0e02 0c02 723e 0000 0054 a901 da0a 736f  ....r>...T....so
+000006a0: 6674 5f6c 6162 656c 6301 0000 0000 0000  ft_labelc.......
+000006b0: 0001 0000 0011 0000 0006 0000 0043 0000  .............C..
+000006c0: 0073 5e01 0000 7c00 6401 1900 7d02 7c00  .s^...|.d...}.|.
+000006d0: 6402 1900 7d03 7c00 6403 1900 7d04 7c00  d...}.|.d...}.|.
+000006e0: 6404 1900 7d05 7c00 6405 1900 7d06 7c03  d...}.|.d...}.|.
+000006f0: 6a00 6406 1900 7d07 7c07 6407 1a00 6407  j.d...}.|.d...d.
+00000700: 1700 7d08 7c05 7c08 3700 7d05 7c06 7c08  ..}.|.|.7.}.|.|.
+00000710: 3700 7d06 7401 6a02 a003 7401 6a04 a005  7.}.t.j...t.j...
+00000720: 7c00 6408 1900 a101 a101 7d09 7406 a007  |.d.......}.t...
+00000730: 7c09 7c08 a102 7d0a 7c01 72d6 7c0a 7c05  |.|...}.|.r.|.|.
+00000740: 7c06 6602 1900 7d0b 6409 7c0b 1800 7c03  |.f...}.d.|...|.
+00000750: 1400 7c0b 6409 7c03 1800 1400 1700 7d0c  ..|.d.|.......}.
+00000760: 7406 a008 7c0a a101 7d0d 7c0d 6a09 7c05  t...|...}.|.j.|.
+00000770: 7c06 6602 1900 a00a 7c03 a101 7d0d 7c0d  |.f.....|...}.|.
+00000780: 7c05 7c06 6602 1900 7c03 1800 7d0e 7c0c  |.|.f...|...}.|.
+00000790: 7c03 7c0e 1400 1700 7d0c 6e7e 7c0a 640a  |.|.....}.n~|.d.
+000007a0: 6b04 a00b 7c03 6a0c a101 7d0a 7c0a 7c05  k...|.j...}.|.|.
+000007b0: 7c06 6602 1900 7d0b 6409 7c0b 1800 7c03  |.f...}.d.|...|.
+000007c0: 1400 7c0b 6409 7c03 1800 1400 1700 7d0c  ..|.d.|.......}.
+000007d0: 7406 a008 7c0a a101 7d0f 7401 6a04 a00d  t...|...}.t.j...
+000007e0: 7c04 0b00 a101 0b00 7d10 7c0f 6a09 7c05  |.......}.|.j.|.
+000007f0: 7c06 6602 1900 a00a 7c10 a101 7d0f 7c0f  |.f.....|...}.|.
+00000800: 7c05 7c06 6602 1900 7c10 1800 7d10 7c0c  |.|.f...|...}.|.
+00000810: 7c03 7c10 1400 1700 7d0c 740e 7c0c 7c02  |.|.....}.t.|.|.
+00000820: 8302 5300 290b 7a21 4c41 4353 5320 696e  ..S.).z!LACSS in
+00000830: 7374 616e 6365 206c 6f73 732c 2075 6e73  stance loss, uns
+00000840: 7570 6572 7669 7365 6472 1900 0000 da0f  upervisedr......
+00000850: 696e 7374 616e 6365 5f6f 7574 7075 7472  instance_outputr
+00000860: 1a00 0000 721b 0000 0072 1c00 0000 7208  ....r....r....r.
+00000870: 0000 0072 0300 0000 da07 6667 5f70 7265  ...r......fg_pre
+00000880: 64e7 0000 0000 0000 f03f 7221 0000 0029  d........?r!...)
+00000890: 0f72 0d00 0000 722a 0000 00da 036c 6178  .r....r*.....lax
+000008a0: da0d 7374 6f70 5f67 7261 6469 656e 74da  ..stop_gradient.
+000008b0: 026e 6eda 0773 6967 6d6f 6964 720e 0000  .nn..sigmoidr...
+000008c0: 0072 2500 0000 da0a 7a65 726f 735f 6c69  .r%.....zeros_li
+000008d0: 6b65 da02 6174 da03 6164 6472 2400 0000  ke..at..addr$...
+000008e0: da05 6474 7970 65da 0b6c 6f67 5f73 6967  ..dtype..log_sig
+000008f0: 6d6f 6964 7218 0000 0029 1172 2f00 0000  moidr....).r/...
+00000900: 7240 0000 0072 1900 0000 da09 696e 7374  r@...r......inst
+00000910: 616e 6365 7372 1a00 0000 7232 0000 0072  ancesr....r2...r
+00000920: 3300 0000 da0a 7061 7463 685f 7369 7a65  3.....patch_size
+00000930: da0c 7061 6464 696e 675f 7369 7a65 da0b  ..padding_size..
+00000940: 6269 6e61 7279 5f6d 6173 6bda 0373 6567  binary_mask..seg
+00000950: da09 7365 675f 7061 7463 6872 1300 0000  ..seg_patchr....
+00000960: 5a0c 696e 7374 616e 6365 5f73 756d 5a0e  Z.instance_sumZ.
+00000970: 696e 7374 616e 6365 5f73 756d 5f69 da0a  instance_sum_i..
+00000980: 6c6f 675f 7969 5f73 756d da06 6c6f 675f  log_yi_sum..log_
+00000990: 7969 7216 0000 0072 1600 0000 7217 0000  yir....r....r...
+000009a0: 00da 1d73 656c 665f 7375 7065 7276 6973  ...self_supervis
+000009b0: 6564 5f69 6e73 7461 6e63 655f 6c6f 7373  ed_instance_loss
+000009c0: 4900 0000 7336 0000 0000 0308 0108 0108  I...s6..........
+000009d0: 0108 0108 020a 010c 0108 0108 0218 010c  ................
+000009e0: 0204 010c 0218 020a 0114 0110 020e 0310  ................
+000009f0: 010c 0218 020a 0110 0114 0110 020c 0272  ...............r
+00000a00: 5500 0000 46a9 01da 0b69 676e 6f72 655f  U...F....ignore_
+00000a10: 6d61 736b 6303 0000 0000 0000 0001 0000  maskc...........
+00000a20: 0011 0000 0005 0000 004b 0000 0073 2a01  .........K...s*.
+00000a30: 0000 7c00 6401 1900 7d05 7c00 6402 1900  ..|.d...}.|.d...
+00000a40: 7d06 7c00 6403 1900 7d07 7c00 6404 1900  }.|.d...}.|.d...
+00000a50: 7d08 7c00 6405 1900 7d09 7c06 6a00 6406  }.|.d...}.|.j.d.
+00000a60: 1900 7d0a 7c0a 6407 1a00 6407 1700 7d0b  ..}.|.d...d...}.
+00000a70: 7c08 7c0b 3700 7d08 7c09 7c0b 3700 7d09  |.|.7.}.|.|.7.}.
+00000a80: 7c03 7282 7401 a002 7c02 6408 1900 6a00  |.r.t...|.d...j.
+00000a90: 6409 6406 8502 1900 a101 7d0c 7401 a003  d.d.......}.t...
+00000aa0: 7c0c 7c0b a102 7d0c 7401 a004 7c06 a101  |.|...}.t...|...
+00000ab0: 7d0d 6e54 7405 7c01 7406 8302 729c 7c01  }.nTt.|.t...r.|.
+00000ac0: 640a 1900 a007 640b a101 7d0c 6e0a 7c01  d.....d...}.n.|.
+00000ad0: a007 640b a101 7d0c 7401 a003 7c0c 7c0b  ..d...}.t...|.|.
+00000ae0: a102 7d0c 7c0c 7c08 7c09 6602 1900 7d0e  ..}.|.|.|.f...}.
+00000af0: 640c 7c0e 1800 7c06 1400 7c0e 640c 7c06  d.|...|...|.d.|.
+00000b00: 1800 1400 1700 7d0d 7401 a004 7c0c a101  ......}.t...|...
+00000b10: 7d0f 7408 6a09 a00a 7c07 0b00 a101 0b00  }.t.j...|.......
+00000b20: 7d10 7c0f 6a0b 7c08 7c09 6602 1900 a00c  }.|.j.|.|.f.....
+00000b30: 7c10 a101 7d0f 7c0f 7c08 7c09 6602 1900  |...}.|.|.|.f...
+00000b40: 7c10 1800 7d10 7c0d 7c06 7c10 1400 1700  |...}.|.|.|.....
+00000b50: 7d0d 740d 7c0d 7c05 8302 5300 290d 7a2f  }.t.|.|...S.).z/
+00000b60: 4c61 6373 7320 696e 7374 616e 6365 206c  Lacss instance l
+00000b70: 6f73 732c 2073 7570 6572 7669 7365 6420  oss, supervised 
+00000b80: 7769 7468 2069 6d61 6765 206d 6173 6b72  with image maskr
+00000b90: 1900 0000 7241 0000 0072 1a00 0000 721b  ....rA...r....r.
+00000ba0: 0000 0072 1c00 0000 7208 0000 0072 0300  ...r....r....r..
+00000bb0: 0000 da05 696d 6167 654e da07 6774 5f6d  ....imageN..gt_m
+00000bc0: 6173 6b72 0600 0000 7243 0000 0029 0e72  askr....rC...).r
+00000bd0: 0d00 0000 720e 0000 00da 057a 6572 6f73  ....r......zeros
+00000be0: 7225 0000 0072 4800 0000 7222 0000 0072  r%...rH...r"...r
+00000bf0: 2300 0000 7224 0000 0072 2a00 0000 7246  #...r$...r*...rF
+00000c00: 0000 0072 4c00 0000 7249 0000 0072 4a00  ...rL...rI...rJ.
+00000c10: 0000 7218 0000 0029 1172 2f00 0000 7230  ..r....).r/...r0
+00000c20: 0000 00da 0669 6e70 7574 7372 5700 0000  .....inputsrW...
+00000c30: 7231 0000 0072 1900 0000 724d 0000 0072  r1...r....rM...r
+00000c40: 1a00 0000 7232 0000 0072 3300 0000 724e  ....r2...r3...rN
+00000c50: 0000 0072 4f00 0000 7251 0000 0072 1300  ...rO...rQ...r..
+00000c60: 0000 7252 0000 0072 5300 0000 7254 0000  ..rR...rS...rT..
+00000c70: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000c80: da1f 7765 616b 6c79 5f73 7570 6572 7669  ..weakly_supervi
+00000c90: 7365 645f 696e 7374 616e 6365 5f6c 6f73  sed_instance_los
+00000ca0: 7375 0000 0073 3200 0000 0005 0801 0801  su...s2.........
+00000cb0: 0801 0801 0802 0a01 0c01 0801 0802 0401  ................
+00000cc0: 1801 0c01 0c02 0a01 1002 0a01 0c01 0c01  ................
+00000cd0: 1802 0a02 1001 1401 1002 0c02 725c 0000  ............r\..
+00000ce0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000cf0: 0000 0300 0000 4000 0000 731c 0000 0065  ......@...s....e
+00000d00: 005a 0164 005a 0265 0365 0364 019c 0264  .Z.d.Z.e.e.d...d
+00000d10: 0264 0384 045a 0464 0453 0029 05da 1653  .d...Z.d.S.)...S
+00000d20: 7570 6572 7669 7365 6449 6e73 7461 6e63  upervisedInstanc
+00000d30: 654c 6f73 7329 0272 2f00 0000 7230 0000  eLoss).r/...r0..
+00000d40: 0063 0300 0000 0000 0000 0000 0000 0400  .c..............
+00000d50: 0000 0300 0000 4b00 0000 730a 0000 0074  ......K...s....t
+00000d60: 007c 017c 0283 0253 00a9 014e 2901 723e  .|.|...S...N).r>
+00000d70: 0000 0029 04da 0473 656c 6672 2f00 0000  ...)...selfr/...
+00000d80: 7230 0000 0072 3100 0000 7216 0000 0072  r0...r1...r....r
+00000d90: 1600 0000 7217 0000 00da 0463 616c 6c9e  ....r......call.
+00000da0: 0000 0073 0200 0000 0001 7a1b 5375 7065  ...s......z.Supe
+00000db0: 7276 6973 6564 496e 7374 616e 6365 4c6f  rvisedInstanceLo
+00000dc0: 7373 2e63 616c 6c4e 2905 da08 5f5f 6e61  ss.callN)...__na
+00000dd0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000de0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7223  ..__qualname__r#
+00000df0: 0000 0072 6000 0000 7216 0000 0072 1600  ...r`...r....r..
+00000e00: 0000 7216 0000 0072 1700 0000 725d 0000  ..r....r....r]..
+00000e10: 009d 0000 0073 0200 0000 0801 725d 0000  .....s......r]..
+00000e20: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000e30: 0000 0500 0000 0000 0000 7332 0000 0065  ..........s2...e
+00000e40: 005a 0164 005a 0264 0865 0364 029c 0187  .Z.d.Z.d.e.d....
+00000e50: 0066 0164 0364 0484 0d5a 0465 0564 059c  .f.d.d...Z.e.d..
+00000e60: 0164 0664 0784 045a 0687 0004 005a 0753  .d.d...Z.....Z.S
+00000e70: 0029 09da 1a53 656c 6653 7570 6572 7669  .)...SelfSupervi
+00000e80: 7365 6449 6e73 7461 6e63 654c 6f73 7354  sedInstanceLossT
+00000e90: 723f 0000 0063 0200 0000 0000 0000 0000  r?...c..........
+00000ea0: 0000 0400 0000 0300 0000 0f00 0000 7318  ..............s.
+00000eb0: 0000 0074 0083 006a 017c 027c 038e 0101  ...t...j.|.|....
+00000ec0: 007c 017c 005f 0264 0053 0072 5e00 0000  .|.|._.d.S.r^...
+00000ed0: 2903 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
+00000ee0: 745f 5f72 4000 0000 2904 725f 0000 0072  t__r@...).r_...r
+00000ef0: 4000 0000 da04 6172 6773 7231 0000 00a9  @.....argsr1....
+00000f00: 01da 095f 5f63 6c61 7373 5f5f 7216 0000  ...__class__r...
+00000f10: 0072 1700 0000 7266 0000 00a3 0000 0073  .r....rf.......s
+00000f20: 0400 0000 0001 0e01 7a23 5365 6c66 5375  ........z#SelfSu
+00000f30: 7065 7276 6973 6564 496e 7374 616e 6365  pervisedInstance
+00000f40: 4c6f 7373 2e5f 5f69 6e69 745f 5f29 0172  Loss.__init__).r
+00000f50: 2f00 0000 6302 0000 0000 0000 0000 0000  /...c...........
+00000f60: 0003 0000 0004 0000 004b 0000 0073 0e00  .........K...s..
+00000f70: 0000 7400 7c01 7c00 6a01 6401 8d02 5300  ..t.|.|.j.d...S.
+00000f80: 2902 4e72 3f00 0000 2902 7255 0000 0072  ).Nr?...).rU...r
+00000f90: 4000 0000 2903 725f 0000 0072 2f00 0000  @...).r_...r/...
+00000fa0: 7231 0000 0072 1600 0000 7216 0000 0072  r1...r....r....r
+00000fb0: 1700 0000 7260 0000 00a7 0000 0073 0200  ....r`.......s..
+00000fc0: 0000 0001 7a1f 5365 6c66 5375 7065 7276  ....z.SelfSuperv
+00000fd0: 6973 6564 496e 7374 616e 6365 4c6f 7373  isedInstanceLoss
+00000fe0: 2e63 616c 6c29 0154 2908 7261 0000 0072  .call).T).ra...r
+00000ff0: 6200 0000 7263 0000 00da 0462 6f6f 6c72  b...rc.....boolr
+00001000: 6600 0000 7223 0000 0072 6000 0000 da0d  f...r#...r`.....
+00001010: 5f5f 636c 6173 7363 656c 6c5f 5f72 1600  __classcell__r..
+00001020: 0000 7216 0000 0072 6800 0000 7217 0000  ..r....rh...r...
+00001030: 0072 6400 0000 a200 0000 7304 0000 0008  .rd.......s.....
+00001040: 0114 0472 6400 0000 6300 0000 0000 0000  ...rd...c.......
+00001050: 0000 0000 0000 0000 0005 0000 0000 0000  ................
+00001060: 0073 2c00 0000 6500 5a01 6400 5a02 6407  .s,...e.Z.d.Z.d.
+00001070: 6503 6402 9c01 8700 6601 6403 6404 840d  e.d.....f.d.d...
+00001080: 5a04 6405 6406 8400 5a05 8700 0400 5a06  Z.d.d...Z.....Z.
+00001090: 5300 2908 da1c 5765 616b 6c79 5375 7065  S.)...WeaklySupe
+000010a0: 7276 6973 6564 496e 7374 616e 6365 4c6f  rvisedInstanceLo
+000010b0: 7373 4672 5600 0000 6302 0000 0000 0000  ssFrV...c.......
+000010c0: 0000 0000 0004 0000 0003 0000 000f 0000  ................
+000010d0: 0073 1800 0000 7400 8300 6a01 7c02 7c03  .s....t...j.|.|.
+000010e0: 8e01 0100 7c01 7c00 5f02 6400 5300 725e  ....|.|._.d.S.r^
+000010f0: 0000 0029 0372 6500 0000 7266 0000 0072  ...).re...rf...r
+00001100: 5700 0000 2904 725f 0000 0072 5700 0000  W...).r_...rW...
+00001110: 7267 0000 0072 3100 0000 7268 0000 0072  rg...r1...rh...r
+00001120: 1600 0000 7217 0000 0072 6600 0000 ac00  ....r....rf.....
+00001130: 0000 7304 0000 0000 010e 017a 2557 6561  ..s........z%Wea
+00001140: 6b6c 7953 7570 6572 7669 7365 6449 6e73  klySupervisedIns
+00001150: 7461 6e63 654c 6f73 732e 5f5f 696e 6974  tanceLoss.__init
+00001160: 5f5f 6301 0000 0000 0000 0003 0000 0004  __c.............
+00001170: 0000 0006 0000 0043 0000 0073 1200 0000  .......C...s....
+00001180: 7400 7c01 7c02 7c03 7c00 6a01 6401 8d04  t.|.|.|.|.j.d...
+00001190: 5300 2902 4e72 5600 0000 2902 725c 0000  S.).NrV...).r\..
+000011a0: 0072 5700 0000 2904 725f 0000 0072 2f00  .rW...).r_...r/.
+000011b0: 0000 7230 0000 0072 5b00 0000 7216 0000  ..r0...r[...r...
+000011c0: 0072 1600 0000 7217 0000 0072 6000 0000  .r....r....r`...
+000011d0: b000 0000 730c 0000 0000 0102 0102 0002  ....s...........
+000011e0: 0002 0004 ff7a 2157 6561 6b6c 7953 7570  .....z!WeaklySup
+000011f0: 6572 7669 7365 6449 6e73 7461 6e63 654c  ervisedInstanceL
+00001200: 6f73 732e 6361 6c6c 2901 4629 0772 6100  oss.call).F).ra.
+00001210: 0000 7262 0000 0072 6300 0000 726a 0000  ..rb...rc...rj..
+00001220: 0072 6600 0000 7260 0000 0072 6b00 0000  .rf...r`...rk...
+00001230: 7216 0000 0072 1600 0000 7268 0000 0072  r....r....rh...r
+00001240: 1700 0000 726c 0000 00ab 0000 0073 0400  ....rl.......s..
+00001250: 0000 0801 1404 726c 0000 0029 16da 0966  ......rl...)...f
+00001260: 756e 6374 6f6f 6c73 7202 0000 0072 2a00  unctoolsr....r*.
+00001270: 0000 da09 6a61 782e 6e75 6d70 79da 056e  ....jax.numpy..n
+00001280: 756d 7079 720e 0000 0072 2d00 0000 da03  umpyr....r-.....
+00001290: 6f70 7372 0400 0000 da0a 7472 6169 6e2e  opsr......train.
+000012a0: 6c6f 7373 7205 0000 00da 0566 696e 666f  lossr......finfo
+000012b0: da03 6570 7372 1000 0000 7218 0000 0072  ..epsr....r....r
+000012c0: 3e00 0000 726a 0000 0072 5500 0000 725c  >...rj...rU...r\
+000012d0: 0000 0072 5d00 0000 7264 0000 0072 6c00  ...r]...rd...rl.
+000012e0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
+000012f0: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001300: 0100 0000 7320 0000 000c 0208 010c 0108  ....s ..........
+00001310: 020c 010c 020c 0308 0b08 3114 2d02 ff04  ..........1.-...
+00001320: 0102 ff0c 2810 0510 09                   ....(....
```

### Comparing `lacss-0.4.0/lacss/losses/auxiliary.py` & `lacss-0.4.1/lacss/losses/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/losses/detection.py` & `lacss-0.4.1/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/losses/instance.py` & `lacss-0.4.1/lacss/losses/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     instance_logit = preds["instance_logit"]
     yc = preds["instance_yc"]
     xc = preds["instance_xc"]
 
     if not isinstance(labels, dict):
         labels = dict(gt_labels=labels)
 
-    if "gt_labels" in labels:
+    if "gt_labels" in labels: # labeled with image label
         gt_labels = labels["gt_labels"].astype("int32")
 
         n_patches, ps, _ = yc.shape
 
         gt_labels = jnp.pad(gt_labels, ps // 2)
         gt_patches = gt_labels[yc + ps // 2, xc + ps // 2] == (
             jnp.arange(n_patches)[:, None, None] + 1
         )
-        gt_patches = gt_patches.astype(int)
+        gt_patches = gt_patches.astype("float32")
 
-    else:
+    else: # labeled with bboxes and rescaled segmentation masks, ie, coco
         y0, x0, y1, x1 = jnp.swapaxes(labels["gt_bboxes"], 0, 1)
         gt_segs = labels["gt_masks"]
         if len(gt_segs.shape) == 4: # either NxHxWx1 or NxHxW
             gt_segs = gt_segs.squeeze(-1) 
         seg_size = gt_segs.shape[1]
 
         # pixel size of the gt mask labels
@@ -55,19 +55,19 @@
         ws = (x1 - x0) / seg_size
 
         # compute rescaled coorinats in edge indexing
         yc = (yc - y0[:, None, None] + .5) / hs[:, None, None]
         xc = (xc - x0[:, None, None] + .5) / ws[:, None, None]
 
         # resample the label to match model coordinates
-        gt_patches = jax.vmap(partial(sub_pixel_samples, edge_indexing=True))(
+        gt_patches = jax.vmap(sub_pixel_samples)(
             gt_segs,
-            jnp.stack([yc, xc], axis=-1),
+            jnp.stack([yc, xc], axis=-1) - .5, # default is center indexing
         )
-        gt_patches = (gt_patches>=.5).astype(int)
+        gt_patches = (gt_patches>=.5).astype("float32")
 
     loss = optax.sigmoid_binary_cross_entropy(instance_logit, gt_patches)
 
     return _mean_over_boolean_mask(loss, instance_mask)
 
 
 def self_supervised_instance_loss(preds, *, soft_label: bool = True):
```

### Comparing `lacss-0.4.0/lacss/metrics/__pycache__/ranked.cpython-38.pyc` & `lacss-0.4.1/lacss/metrics/__pycache__/ranked.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:04 2023 UTC, .py size: 5103 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bc1e 9764 ef13 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 99e8 9964 ef13 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 6401 6402 6c03 5a05 6403  m.Z...d.d.l.Z.d.
 00000050: 6404 6c06 5400 6403 6405 6c07 6d08 5a08  d.l.T.d.d.l.m.Z.
 00000060: 0100 6403 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 6408 8400 5a0b 6409 640a 8400 5a0c 4700  d...Z.d.d...Z.G.
```

### Comparing `lacss-0.4.0/lacss/metrics/ranked.py` & `lacss-0.4.1/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/auxiliary.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/auxiliary.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 15:28:15 2023 UTC, .py size: 2075 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 8fae 9964 1b08 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 99e8 9964 1b08 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c05 5a05 6400 6401 6c06  ..d.d.l.Z.d.d.l.
 00000050: 6d07 5a08 0100 6402 6403 6c09 5400 6402  m.Z...d.d.l.T.d.
 00000060: 6404 6c0a 6d0b 5a0b 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000070: 8400 6406 6504 6a0c 8303 5a0d 4700 6407  ..d.e.j...Z.G.d.
```

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/common.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/convnext.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/convnext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/detector.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/detector.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/lacss.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/lacss.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:13 2023 UTC, .py size: 4138 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c51e 9764 2a10 0000  U..........d*...
+00000000: 550d 0d0a 0000 0000 20ee 9964 1810 0000  U....... ..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6401 6c07 6d08 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6401 6c0a 5a0a 6400 6401 6c0b 6d0c 5a0d  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6404 6405 6c0e 5400 6406 6405 6c0f  ..d.d.l.T.d.d.l.
@@ -169,49 +169,48 @@
 00000a80: 6f72 6567 726f 756e 64da 0e5f 6175 785f  oreground.._aux_
 00000a90: 6667 5f6d 6f64 756c 6529 0172 3600 0000  fg_module).r6...
 00000aa0: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
 00000ab0: 0573 6574 7570 7600 0000 730a 0000 0000  .setupv...s.....
 00000ac0: 010e 010a 010e 010a 017a 154c 6163 7373  .........z.Lacss
 00000ad0: 5769 7468 4865 6c70 6572 2e73 6574 7570  WithHelper.setup
 00000ae0: 4672 1800 0000 6304 0000 0000 0000 0001  Fr....c.........
-00000af0: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
-00000b00: 5200 0000 7c00 6a00 7c01 7c02 7c04 6401  R...|.j.|.|.|.d.
+00000af0: 0000 0006 0000 0006 0000 0043 0000 0073  ...........C...s
+00000b00: 5000 0000 7c00 6a00 7c01 7c02 7c04 6401  P...|.j.|.|.|.d.
 00000b10: 8d03 7d05 7c00 6a01 6400 6b09 722e 7c05  ..}.|.j.d.k.r.|.
 00000b20: a002 7c00 6a03 7c01 7c03 6402 8d02 a101  ..|.j.|.|.d.....
-00000b30: 0100 7c00 6a04 6400 6b09 724e 7c05 a002  ..|.j.d.k.rN|...
-00000b40: 7c00 6a05 7c01 7c03 7c04 6403 8d03 a101  |.j.|.|.|.d.....
-00000b50: 0100 7c05 5300 2904 4e72 1800 0000 2901  ..|.S.).Nr....).
-00000b60: da08 6361 7465 676f 7279 2902 724f 0000  ..category).rO..
-00000b70: 00da 0761 7567 6d65 6e74 2906 7249 0000  ...augment).rI..
-00000b80: 0072 4700 0000 7235 0000 0072 4b00 0000  .rG...r5...rK...
-00000b90: 7248 0000 0072 4d00 0000 2906 7236 0000  rH...rM...).r6..
-00000ba0: 0072 1a00 0000 721b 0000 0072 4f00 0000  .r....r....rO...
-00000bb0: 7219 0000 00da 0570 7265 6473 7215 0000  r......predsr...
-00000bc0: 0072 1500 0000 7216 0000 0072 3a00 0000  .r....r....r:...
-00000bd0: 7d00 0000 7310 0000 0000 0210 020a 0214  }...s...........
-00000be0: 020a 0204 010e ff04 047a 184c 6163 7373  .........z.Lacss
-00000bf0: 5769 7468 4865 6c70 6572 2e5f 5f63 616c  WithHelper.__cal
-00000c00: 6c5f 5f29 024e 4e29 0d72 3b00 0000 723c  l__).NN).r;...r<
-00000c10: 0000 0072 3d00 0000 7203 0000 0072 3300  ...r=...r....r3.
-00000c20: 0000 7246 0000 0072 4000 0000 7247 0000  ..rF...r@...rG..
-00000c30: 00da 0274 70da 084f 7074 696f 6e61 6c72  ...tp..Optionalr
-00000c40: 4800 0000 724e 0000 0072 3a00 0000 7215  H...rN...r:...r.
-00000c50: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000c60: 0000 7244 0000 0071 0000 0073 0a00 0000  ..rD...q...s....
-00000c70: 0a01 1201 1201 1202 0807 7244 0000 0029  ..........rD...)
-00000c80: 1dda 0674 7970 696e 6772 5200 0000 da0b  ...typingrR.....
-00000c90: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
-00000ca0: 7203 0000 00da 0966 756e 6374 6f6f 6c73  r......functools
-00000cb0: 7204 0000 00da 0a66 6c61 782e 6c69 6e65  r......flax.line
-00000cc0: 6eda 056c 696e 656e 723e 0000 00da 036a  n..linenr>.....j
-00000cd0: 6178 da09 6a61 782e 6e75 6d70 79da 056e  ax..jax.numpy..n
-00000ce0: 756d 7079 722d 0000 00da 036f 7073 da09  umpyr-.....ops..
-00000cf0: 6175 7869 6c69 6172 79da 0863 6f6e 766e  auxiliary..convn
-00000d00: 6578 7472 0800 0000 7210 0000 0072 0900  extr....r....r..
-00000d10: 0000 720f 0000 0072 0a00 0000 da06 7265  ..r....r......re
-00000d20: 736e 6574 720b 0000 0072 1100 0000 720c  snetr....r....r.
-00000d30: 0000 0072 3f00 0000 720d 0000 0072 4400  ...r?...r....rD.
-00000d40: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00000d50: 0072 1600 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000d60: 0100 0000 731c 0000 0008 0110 010c 020c  ....s...........
-00000d70: 0108 010c 0208 0108 010c 010c 010c 010c  ................
-00000d80: 010c 0312 5f                             ...._
+00000b30: 0100 7c00 6a04 6400 6b09 724c 7c05 a002  ..|.j.d.k.rL|...
+00000b40: 7c00 6a05 7c01 7c03 6402 8d02 a101 0100  |.j.|.|.d.......
+00000b50: 7c05 5300 2903 4e72 1800 0000 2901 da08  |.S.).Nr....)...
+00000b60: 6361 7465 676f 7279 2906 7249 0000 0072  category).rI...r
+00000b70: 4700 0000 7235 0000 0072 4b00 0000 7248  G...r5...rK...rH
+00000b80: 0000 0072 4d00 0000 2906 7236 0000 0072  ...rM...).r6...r
+00000b90: 1a00 0000 721b 0000 0072 4f00 0000 7219  ....r....rO...r.
+00000ba0: 0000 00da 0570 7265 6473 7215 0000 0072  .....predsr....r
+00000bb0: 1500 0000 7216 0000 0072 3a00 0000 7d00  ....r....r:...}.
+00000bc0: 0000 7310 0000 0000 0210 020a 0214 020a  ..s.............
+00000bd0: 0204 010c ff04 047a 184c 6163 7373 5769  .......z.LacssWi
+00000be0: 7468 4865 6c70 6572 2e5f 5f63 616c 6c5f  thHelper.__call_
+00000bf0: 5f29 024e 4e29 0d72 3b00 0000 723c 0000  _).NN).r;...r<..
+00000c00: 0072 3d00 0000 7203 0000 0072 3300 0000  .r=...r....r3...
+00000c10: 7246 0000 0072 4000 0000 7247 0000 00da  rF...r@...rG....
+00000c20: 0274 70da 084f 7074 696f 6e61 6c72 4800  .tp..OptionalrH.
+00000c30: 0000 724e 0000 0072 3a00 0000 7215 0000  ..rN...r:...r...
+00000c40: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000c50: 7244 0000 0071 0000 0073 0a00 0000 0a01  rD...q...s......
+00000c60: 1201 1201 1202 0807 7244 0000 0029 1dda  ........rD...)..
+00000c70: 0674 7970 696e 6772 5100 0000 da0b 6461  .typingrQ.....da
+00000c80: 7461 636c 6173 7365 7372 0200 0000 7203  taclassesr....r.
+00000c90: 0000 00da 0966 756e 6374 6f6f 6c73 7204  .....functoolsr.
+00000ca0: 0000 00da 0a66 6c61 782e 6c69 6e65 6eda  .....flax.linen.
+00000cb0: 056c 696e 656e 723e 0000 00da 036a 6178  .linenr>.....jax
+00000cc0: da09 6a61 782e 6e75 6d70 79da 056e 756d  ..jax.numpy..num
+00000cd0: 7079 722d 0000 00da 036f 7073 da09 6175  pyr-.....ops..au
+00000ce0: 7869 6c69 6172 79da 0863 6f6e 766e 6578  xiliary..convnex
+00000cf0: 7472 0800 0000 7210 0000 0072 0900 0000  tr....r....r....
+00000d00: 720f 0000 0072 0a00 0000 da06 7265 736e  r....r......resn
+00000d10: 6574 720b 0000 0072 1100 0000 720c 0000  etr....r....r...
+00000d20: 0072 3f00 0000 720d 0000 0072 4400 0000  .r?...r....rD...
+00000d30: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00000d40: 1600 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000d50: 0000 731c 0000 0008 0110 010c 020c 0108  ..s.............
+00000d60: 010c 0208 0108 010c 010c 010c 010c 010c  ................
+00000d70: 0312 5f                                  .._
```

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/lpn.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/lpn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/resnet.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/resnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/segmentor.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/segmentor.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 5254 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 8614 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 221d 9b64 8614 0000  U......."..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6400 6401 6c08 5a08 6400  m.Z...d.d.l.Z.d.
 00000060: 6401 6c09 6d0a 5a0b 0100 6403 6404 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6405 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `lacss-0.4.0/lacss/modules/__pycache__/unet.cpython-38.pyc` & `lacss-0.4.1/lacss/modules/__pycache__/unet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/auxiliary.py` & `lacss-0.4.1/lacss/modules/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/common.py` & `lacss-0.4.1/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/convnext.py` & `lacss-0.4.1/lacss/modules/convnext.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/detector.py` & `lacss-0.4.1/lacss/modules/detector.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/lacss.py` & `lacss-0.4.1/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/lpn.py` & `lacss-0.4.1/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/resnet.py` & `lacss-0.4.1/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/segmentor.py` & `lacss-0.4.1/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/modules/unet.py` & `lacss-0.4.1/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/__pycache__/boxes.cpython-38.pyc` & `lacss-0.4.1/lacss/ops/__pycache__/boxes.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:04 2023 UTC, .py size: 2321 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bc1e 9764 1109 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 99e8 9964 1109 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 6401 6402 6c03 5a05 6403  m.Z...d.d.l.Z.d.
 00000050: 6404 8400 5a06 6405 6406 8400 5a07 6407  d...Z.d.d...Z.d.
 00000060: 6408 8400 5a08 6402 5300 2909 7a8a 204f  d...Z.d.S.).z. O
 00000070: 7073 206f 6e20 626f 756e 6469 6e67 2d62  ps on bounding-b
```

### Comparing `lacss-0.4.0/lacss/ops/__pycache__/image.cpython-38.pyc` & `lacss-0.4.1/lacss/ops/__pycache__/image.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:13 2023 UTC, .py size: 3289 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c51e 9764 d90c 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 99e8 9964 d90c 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6502  Z.d.d.l.m.Z...e.
 00000050: 6a05 5a06 6404 6405 8400 5a07 640d 6406  j.Z.d.d...Z.d.d.
 00000060: 6407 8401 5a08 640e 6409 640a 8401 5a09  d...Z.d.d.d...Z.
 00000070: 640f 640b 640c 8401 5a0a 6402 5300 2910  d.d.d...Z.d.S.).
```

### Comparing `lacss-0.4.0/lacss/ops/__pycache__/locations.cpython-38.pyc` & `lacss-0.4.1/lacss/ops/__pycache__/locations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:04 2023 UTC, .py size: 2843 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bc1e 9764 1b0b 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 99e8 9964 1b0b 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6500 6a01 5a02 6409 6403  d.l.Z.e.j.Z.d.d.
 00000040: 6404 8401 5a03 6405 6406 8400 5a04 6407  d...Z.d.d...Z.d.
 00000050: 6408 8400 5a05 6401 5300 290a e900 0000  d...Z.d.S.).....
 00000060: 004e e700 0000 0000 00f8 3f63 0300 0000  .N........?c....
 00000070: 0000 0000 0000 0000 0e00 0000 0700 0000  ................
```

### Comparing `lacss-0.4.0/lacss/ops/__pycache__/masks.cpython-38.pyc` & `lacss-0.4.1/lacss/ops/__pycache__/masks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/__pycache__/nms.cpython-38.pyc` & `lacss-0.4.1/lacss/ops/__pycache__/nms.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 16:50:04 2023 UTC, .py size: 4732 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bc1e 9764 7c12 0000  U..........d|...
+00000000: 550d 0d0a 0000 0000 99e8 9964 7c12 0000  U..........d|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 6404 6c03 6d04 5a04 0100 6403  Z.d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 6502 6a07 5a08  d.l.m.Z...e.j.Z.
 00000060: 6406 5a09 6407 6408 8400 5a0a 6409 640a  d.Z.d.d...Z.d.d.
 00000070: 8400 5a0b 640f 650c 650d 650d 640c 9c03  ..Z.d.e.e.e.d...
```

### Comparing `lacss-0.4.0/lacss/ops/__pycache__/patches.cpython-38.pyc` & `lacss-0.4.1/lacss/ops/__pycache__/patches.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 24 23:31:54 2023 UTC, .py size: 11768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 ea7c 9764 f82d 0000  U........|.d.-..
+00000000: 550d 0d0a 0000 0000 99e8 9964 f82d 0000  U..........d.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6401 6404 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a09 6401 6404 6c0a 6d0b 5a0c 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6404 6c0b 5a0d 6405 6406 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -401,30 +401,30 @@
 00001900: 7572 6e73 3a0a 2020 2020 2020 2020 6c61  urns:.        la
 00001910: 6265 6c3a 205b 6865 6967 6874 2c20 7769  bel: [height, wi
 00001920: 6474 685d 0a20 2020 2072 2800 0000 4ea9  dth].    r(...N.
 00001930: 01da 0564 7479 7065 da0d 696e 7374 616e  ...dtype..instan
 00001940: 6365 5f6d 6173 6ba9 0272 0800 0000 720f  ce_mask..r....r.
 00001950: 0000 0072 1100 0000 7201 0000 00da 1274  ...r....r......t
 00001960: 7261 696e 696e 675f 6c6f 6361 7469 6f6e  raining_location
-00001970: 73da 0b70 7265 645f 7363 6f72 6573 7208  s..pred_scoresr.
+00001970: 735a 0b70 7265 645f 7363 6f72 6573 7208  sZ.pred_scoresr.
 00001980: 0000 0072 2900 0000 722a 0000 0029 0d72  ...r)...r*...).r
 00001990: 1400 0000 725c 0000 0072 1300 0000 da04  ....r\...r......
 000019a0: 6f6e 6573 da04 626f 6f6c 722e 0000 0072  ones..boolr....r
 000019b0: 4a00 0000 7216 0000 0072 1700 0000 724c  J...r....r....rL
 000019c0: 0000 0072 3800 0000 724b 0000 0072 5d00  ...r8...rK...r].
 000019d0: 0000 290d 722f 0000 0072 4000 0000 7261  ..).r/...r@...ra
 000019e0: 0000 0072 6200 0000 7234 0000 0072 6300  ...rb...r4...rc.
 000019f0: 0000 da05 6c61 6265 6cda 0270 7272 5f00  ....label..prr_.
 00001a00: 0000 720d 0000 0072 1e00 0000 7230 0000  ..r....r....r0..
 00001a10: 0072 3100 0000 7225 0000 0072 2500 0000  .r1...r%...r%...
 00001a20: 7226 0000 00da 1070 6174 6368 6573 5f74  r&.....patches_t
 00001a30: 6f5f 6c61 6265 6cd1 0000 0073 2000 0000  o_label....s ...
 00001a40: 0015 0a01 0c01 0c02 0801 1001 1401 1001  ................
 00001a50: 1001 1602 3201 1c01 1e02 0801 0802 1402  ....2...........
-00001a60: 726e 0000 0063 0200 0000 0000 0000 0000  rn...c..........
+00001a60: 726d 0000 0063 0200 0000 0000 0000 0000  rm...c..........
 00001a70: 0000 1300 0000 0800 0000 4300 0000 73a4  ..........C...s.
 00001a80: 0100 0074 007c 0083 017d 0274 017c 027c  ...t.|...}.t.|.|
 00001a90: 0283 027d 0374 02a0 037c 0364 01a1 027d  ...}.t...|.d...}
 00001aa0: 0374 02a0 047c 0364 026b 04a1 015c 027d  .t...|.d.k...\.}
 00001ab0: 047d 057c 0064 0319 006a 0564 0419 007d  .}.|.d...j.d...}
 00001ac0: 0674 02a0 067c 0064 0319 00a1 017c 016b  .t...|.d.....|.k
 00001ad0: 057d 077c 077c 0419 007d 087c 077c 0519  .}.|.|...}.|.|..
@@ -467,32 +467,32 @@
 00001d20: 7472 6978 2e0a 2020 2020 7208 0000 0072  trix..    r....r
 00001d30: 0100 0000 7228 0000 0072 1000 0000 e903  ....r(...r......
 00001d40: 0000 0072 6400 0000 7229 0000 0072 2a00  ...rd...r)...r*.
 00001d50: 0000 4e72 0f00 0000 7267 0000 0072 1100  ..Nr....rg...r..
 00001d60: 0000 7249 0000 0029 0c72 3f00 0000 7209  ..rI...).r?...r.
 00001d70: 0000 00da 026e 70da 0474 7269 7572 3800  .....np..triur8.
 00001d80: 0000 7213 0000 00da 0761 7361 7272 6179  ..r......asarray
-00001d90: 725c 0000 00da 036c 656e 726b 0000 0072  r\.....lenrk...r
+00001d90: 725c 0000 00da 036c 656e 726a 0000 0072  r\.....lenrj...r
 00001da0: 4d00 0000 724a 0000 0029 1372 2f00 0000  M...rJ...).r/...
-00001db0: 7234 0000 0072 3e00 0000 da08 626f 785f  r4...r>.....box_
+00001db0: 7234 0000 0072 3e00 0000 5a08 626f 785f  r4...r>...Z.box_
 00001dc0: 696f 7573 da02 6379 da02 6378 da08 7061  ious..cy..cx..pa
 00001dd0: 645f 7369 7a65 7224 0000 005a 0970 6174  d_sizer$...Z.pat
 00001de0: 6368 6573 5f79 5a09 7061 7463 6865 735f  ches_yZ.patches_
 00001df0: 785a 0670 6c74 5f74 6fda 0264 79da 0264  xZ.plt_to..dy..d
 00001e00: 7872 5700 0000 da06 756e 696f 6e73 5a07  xrW.....unionsZ.
 00001e10: 6172 6561 735f 795a 0761 7265 6173 5f78  areas_yZ.areas_x
 00001e20: 7256 0000 00da 096d 6173 6b5f 696f 7573  rV.....mask_ious
 00001e30: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
 00001e40: 1f69 6f75 735f 6f66 5f70 6174 6368 6573  .ious_of_patches
 00001e50: 5f66 726f 6d5f 7361 6d65 5f69 6d61 6765  _from_same_image
 00001e60: fd00 0000 733e 0000 0000 0b08 010a 010c  ....s>..........
 00001e70: 0412 010e 0212 0108 0108 0120 0216 0116  ........... ....
 00001e80: ff02 0202 fe02 ff02 0616 0116 ff02 0202  ................
 00001e90: fe02 ff02 0610 0134 0122 0112 020e 010e  .......4."......
-00001ea0: 0214 0204 010c 0272 7c00 0000 e733 3333  .......r|....333
+00001ea0: 0214 0204 010c 0272 7a00 0000 e733 3333  .......rz....333
 00001eb0: 3333 33e3 3f29 0372 2f00 0000 da0d 696f  333.?).r/.....io
 00001ec0: 755f 7468 7265 7368 6f6c 6472 0e00 0000  u_thresholdr....
 00001ed0: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
 00001ee0: 0004 0000 0043 0000 0073 7c00 0000 7400  .....C...s|...t.
 00001ef0: 7c00 8301 7d02 7c02 7c01 6b04 7d03 6401  |...}.|.|.k.}.d.
 00001f00: 7d04 7401 a002 7c03 a101 7c04 6b03 726e  }.t...|...|.k.rn
 00001f10: 7403 a002 7c03 a101 7d04 7c03 6a04 6401  t...|...}.|.j.d.
@@ -511,24 +511,24 @@
 00001fe0: 2020 2069 6f75 735f 7468 7265 7368 6f6c     ious_threshol
 00001ff0: 643a 2064 6566 6175 6c74 2030 2e36 0a0a  d: default 0.6..
 00002000: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
 00002010: 2020 2020 206d 6173 6b3a 2062 6f6f 6c65       mask: boole
 00002020: 616e 206d 6173 6b20 6f66 2063 656c 6c73  an mask of cells
 00002030: 206e 6f74 2073 7570 7265 7373 6564 0a20   not supressed. 
 00002040: 2020 2072 0100 0000 7211 0000 004e 2905     r....r....N).
-00002050: 727c 0000 0072 7000 0000 724a 0000 0072  r|...rp...rJ...r
+00002050: 727a 0000 0072 6f00 0000 724a 0000 0072  rz...ro...rJ...r
 00002060: 1400 0000 7236 0000 0029 0772 2f00 0000  ....r6...).r/...
-00002070: 727e 0000 0072 5600 0000 7261 0000 00da  r~...rV...ra....
+00002070: 727c 0000 0072 5600 0000 7261 0000 00da  r|...rV...ra....
 00002080: 0363 6e74 da13 6361 6e5f 7375 7070 7265  .cnt..can_suppre
 00002090: 7373 5f6f 7468 6572 73da 0a73 7570 7072  ss_others..suppr
 000020a0: 6573 7365 6472 2500 0000 7225 0000 0072  essedr%...r%...r
 000020b0: 2600 0000 da1c 6e6f 6e5f 6d61 785f 7375  &.....non_max_su
 000020c0: 7070 7265 7373 5f70 7265 6469 6374 696f  ppress_predictio
 000020d0: 6e73 3001 0000 7312 0000 0000 0b08 0108  ns0...s.........
-000020e0: 0204 010e 010a 010e 011c 0118 0272 8200  .............r..
+000020e0: 0204 010e 010a 010e 011c 0118 0272 8000  .............r..
 000020f0: 0000 5429 01da 0d65 6467 655f 696e 6465  ..T)...edge_inde
 00002100: 7869 6e67 2903 722f 0000 00da 0573 6361  xing).r/.....sca
 00002110: 6c65 720e 0000 0063 0200 0000 0000 0000  ler....c........
 00002120: 0000 0000 0b00 0000 0600 0000 4300 0000  ............C...
 00002130: 732a 0100 007c 0064 0119 0064 0264 0285  s*...|.d...d.d..
 00002140: 0264 0364 0366 0319 0064 0417 007c 0114  .d.d.f...d...|..
 00002150: 007d 027c 0064 0519 0064 0264 0285 0264  .}.|.d...d.d...d
@@ -592,43 +592,43 @@
 000024f0: 7269 6420 666f 726d 6174 0a20 2020 2072  rid format.    r
 00002500: 2900 0000 4e72 0100 0000 7233 0000 0072  )...Nr....r3...r
 00002510: 2a00 0000 7228 0000 0072 1000 0000 7208  *...r(...r....r.
 00002520: 0000 0072 1100 0000 290a da05 726f 756e  ...r....)...roun
 00002530: 6472 1300 0000 7214 0000 0072 1900 0000  dr....r....r....
 00002540: da05 666c 6f6f 7272 1600 0000 7217 0000  ..floorr....r...
 00002550: 00da 0c5f 7361 6d70 6c69 6e67 5f6f 7072  ..._sampling_opr
-00002560: 7000 0000 721a 0000 0029 0b72 2f00 0000  p...r....).r/...
-00002570: 7284 0000 005a 066e 6577 5f79 305a 066e  r....Z.new_y0Z.n
+00002560: 6f00 0000 721a 0000 0029 0b72 2f00 0000  o...r....).r/...
+00002570: 7282 0000 005a 066e 6577 5f79 305a 066e  r....Z.new_y0Z.n
 00002580: 6577 5f78 30da 0570 6174 6368 da02 7073  ew_x0..patch..ps
 00002590: 721f 0000 0072 2000 0000 5a06 7265 6c5f  r....r ...Z.rel_
 000025a0: 7979 5a06 7265 6c5f 7878 5a09 6e65 775f  yyZ.rel_xxZ.new_
 000025b0: 7061 7463 6872 2500 0000 7225 0000 0072  patchr%...r%...r
 000025c0: 2600 0000 da0f 7265 7363 616c 655f 7061  &.....rescale_pa
 000025d0: 7463 6865 734b 0100 0073 3000 0000 0012  tchesK...s0.....
 000025e0: 1e01 1e01 0801 1202 1a02 20ff 0204 20ff  .......... ... .
 000025f0: 0204 1801 02ff 0401 02ff 0a03 1801 02ff  ................
-00002600: 0401 02ff 0a03 0201 0201 10fe 0405 728a  ..............r.
+00002600: 0401 02ff 0a03 0201 0201 10fe 0405 7288  ..............r.
 00002610: 0000 0029 0172 3300 0000 2902 4e72 3300  ...).r3...).Nr3.
 00002620: 0000 2902 7244 0000 0072 3300 0000 2901  ..).rD...r3...).
 00002630: 7233 0000 0029 044e 7233 0000 0072 3300  r3...).Nr3...r3.
 00002640: 0000 7201 0000 0029 0172 3300 0000 2901  ..r....).r3...).
-00002650: 727d 0000 0029 23da 075f 5f64 6f63 5f5f  r}...)#..__doc__
+00002650: 727b 0000 0029 23da 075f 5f64 6f63 5f5f  r{...)#..__doc__
 00002660: da09 6675 6e63 746f 6f6c 7372 0200 0000  ..functoolsr....
 00002670: da06 7479 7069 6e67 7203 0000 0072 0400  ..typingr....r..
 00002680: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
 00002690: 00da 036a 6178 da09 6a61 782e 6e75 6d70  ...jax..jax.nump
-000026a0: 79da 056e 756d 7079 7214 0000 0072 7000  y..numpyr....rp.
+000026a0: 79da 056e 756d 7079 7214 0000 0072 6f00  y..numpyr....ro.
 000026b0: 0000 da05 626f 7865 7372 0900 0000 da05  ....boxesr......
 000026c0: 696d 6167 6572 0a00 0000 da07 6e64 6172  imager......ndar
 000026d0: 7261 7972 1700 0000 da05 7475 706c 6572  rayr......tupler
 000026e0: 2700 0000 7232 0000 00da 0566 6c6f 6174  '...r2.....float
 000026f0: 723f 0000 0072 4300 0000 722c 0000 0072  r?...rC...r,...r
-00002700: 5b00 0000 7260 0000 0072 6e00 0000 727c  [...r`...rn...r|
-00002710: 0000 0072 8200 0000 da04 766d 6170 7287  ...r......vmapr.
-00002720: 0000 0072 8a00 0000 7225 0000 0072 2500  ...r....r%...r%.
+00002700: 5b00 0000 7260 0000 0072 6d00 0000 727a  [...r`...rm...rz
+00002710: 0000 0072 8000 0000 da04 766d 6170 7285  ...r......vmapr.
+00002720: 0000 0072 8800 0000 7225 0000 0072 2500  ...r....r%...r%.
 00002730: 0000 7225 0000 0072 2600 0000 da08 3c6d  ..r%...r&.....<m
 00002740: 6f64 756c 653e 0100 0000 737e 0000 0004  odule>....s~....
 00002750: 050c 011c 0208 010c 0108 020c 010c 0404  ................
 00002760: 0004 0002 0102 fe0c 2908 0f00 ff02 010a  ........).......
 00002770: 0002 0104 fe0c 2600 0100 fd02 010a 010a  ......&.........
 00002780: 0102 0102 fc0c 2100 0000 ff02 0102 0004  ......!.........
 00002790: 0002 0002 0104 fe0c 2c00 ff02 0102 000a  ........,.......
```

### Comparing `lacss-0.4.0/lacss/ops/__pycache__/uda.cpython-38.pyc` & `lacss-0.4.1/lacss/ops/__pycache__/uda.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/boxes.py` & `lacss-0.4.1/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/image.py` & `lacss-0.4.1/lacss/ops/image.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/locations.py` & `lacss-0.4.1/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/masks.py` & `lacss-0.4.1/lacss/ops/masks.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/nms.py` & `lacss-0.4.1/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/ops/patches.py` & `lacss-0.4.1/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/tracking/predict.py` & `lacss-0.4.1/lacss/tracking/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/tracking/smc.py` & `lacss-0.4.1/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/tracking/utils.py` & `lacss-0.4.1/lacss/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/__pycache__/loss.cpython-38.pyc` & `lacss-0.4.1/lacss/train/__pycache__/loss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/__pycache__/metric.cpython-38.pyc` & `lacss-0.4.1/lacss/train/__pycache__/metric.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/__pycache__/strategy.cpython-38.pyc` & `lacss-0.4.1/lacss/train/__pycache__/strategy.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 4018 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 b20f 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 e931 9b64 b20f 0000  U........1.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c04 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a07 0100 6400 6401 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6403 6c0b 6d0c 5a0c 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6405 6c0d 6d0e 5a0e 0100 6406 6407 6c0f  d.l.m.Z...d.d.l.
```

### Comparing `lacss-0.4.0/lacss/train/__pycache__/trainer.cpython-38.pyc` & `lacss-0.4.1/lacss/train/__pycache__/trainer.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 16:10:07 2023 UTC, .py size: 13001 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5fb8 9964 c932 0000  U......._..d.2..
+00000000: 550d 0d0a 0000 0000 8831 9b64 7732 0000  U........1.dw2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
 00000060: 6401 6c08 6d09 5a0a 0100 6400 6401 6c0b  d.l.m.Z...d.d.l.
 00000070: 5a0b 6400 6401 6c0c 6d0d 5a0e 0100 6400  Z.d.d.l.m.Z...d.
@@ -464,298 +464,296 @@
 00001cf0: 00da 0574 7261 696e bc00 0000 7336 0000  ...train....s6..
 00001d00: 0000 1708 0106 0206 0108 0208 0214 0114  ................
 00001d10: 010e 0208 010e 0112 0116 0204 0206 0206  ................
 00001d20: 010e ff06 0302 0102 0004 0002 0002 0002  ................
 00001d30: ff0c 0312 0208 027a 0d54 7261 696e 6572  .......z.Trainer
 00001d40: 2e74 7261 696e 2901 da0a 7375 625f 6d6f  .train)...sub_mo
 00001d50: 6475 6c65 6303 0000 0000 0000 0000 0000  dulec...........
-00001d60: 0007 0000 0009 0000 0043 0000 0073 a200  .........C...s..
+00001d60: 0006 0000 0009 0000 0043 0000 0073 9000  .........C...s..
 00001d70: 0000 7c00 6a00 7d03 7c00 6a01 7d04 7c02  ..|.j.}.|.j.}.|.
 00001d80: 6401 6b09 7242 7c03 a002 7403 7c04 6402  d.k.rB|...t.|.d.
 00001d90: 8d01 a101 7d03 7404 7c03 7c02 8302 7d03  ....}.t.|.|...}.
 00001da0: 7c03 a005 a100 5c02 7d03 7d04 7c04 6403  |.....\.}.}.|.d.
 00001db0: 1900 7d04 7406 7c01 7407 8302 7256 7408  ..}.t.|.t...rVt.
 00001dc0: a009 7c01 a101 7d01 7c01 6a0a 6a0b 6404  ..|...}.|.j.j.d.
 00001dd0: 6404 6405 8d02 0100 740c 7c01 6406 8302  d.d.....t.|.d...
-00001de0: 8f28 7d05 740d a00e 7c03 a101 7d06 740f  .(}.t...|...}.t.
-00001df0: 7c04 8301 7d04 7410 a011 7c06 7c04 6602  |...}.t...|.|.f.
-00001e00: 7c05 a102 0100 5700 3500 5100 5200 5800  |.....W.5.Q.R.X.
-00001e10: 6401 5300 2907 6101 0100 0020 5361 7665  d.S.).a.... Save
-00001e20: 2074 6865 206d 6f64 656c 2069 6e20 6120   the model in a 
-00001e30: 7069 636b 6c65 6420 6669 6c65 2e20 5468  pickled file. Th
-00001e40: 6520 7069 636b 6c65 2069 7320 6120 7475  e pickle is a tu
-00001e50: 706c 6520 6f66 0a20 2020 2020 2020 2020  ple of.         
-00001e60: 2020 2028 6d6f 6475 6c65 2c20 7765 6967     (module, weig
-00001e70: 6874 7329 2e0a 0a20 2020 2020 2020 2041  hts)...        A
-00001e80: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00001e90: 2070 6174 683a 2054 6865 2066 696c 6520   path: The file 
-00001ea0: 7061 7468 2e0a 2020 2020 2020 2020 2020  path..          
-00001eb0: 2020 7375 625f 6d6f 6475 6c65 3a20 4f70    sub_module: Op
-00001ec0: 7469 6f6e 616c 6c79 206f 6e6c 7920 7361  tionally only sa
-00001ed0: 7665 2061 2073 7562 5f6d 6f64 756c 6520  ve a sub_module 
-00001ee0: 6f66 2074 6865 206d 6f64 656c 0a20 2020  of the model.   
-00001ef0: 2020 2020 2020 2020 2020 2020 2062 7920               by 
-00001f00: 7370 6563 6966 7969 6e67 2074 6865 206e  specifying the n
-00001f10: 616d 650a 2020 2020 2020 2020 4ea9 0172  ame.        N..r
-00001f20: 3900 0000 7239 0000 0054 a902 da07 7061  9...r9...T....pa
-00001f30: 7265 6e74 73da 0865 7869 7374 5f6f 6bda  rents..exist_ok.
-00001f40: 0277 6229 1272 1a00 0000 7239 0000 00da  .wb).r....r9....
-00001f50: 0462 696e 64da 0464 6963 74da 0767 6574  .bind..dict..get
-00001f60: 6174 7472 7241 0000 0072 1f00 0000 da03  attrrA...r......
-00001f70: 7374 72da 0770 6174 686c 6962 da04 5061  str..pathlib..Pa
-00001f80: 7468 da06 7061 7265 6e74 da05 6d6b 6469  th..parent..mkdi
-00001f90: 72da 046f 7065 6eda 0b64 6174 6163 6c61  r..open..datacla
-00001fa0: 7373 6573 da06 6173 6469 6374 7205 0000  sses..asdictr...
-00001fb0: 00da 0b63 6c6f 7564 7069 636b 6c65 da04  ...cloudpickle..
-00001fc0: 6475 6d70 2907 7228 0000 00da 0470 6174  dump).r(.....pat
-00001fd0: 6872 6500 0000 da06 6d6f 6475 6c65 7239  hre.....moduler9
-00001fe0: 0000 00da 0166 da03 6366 6772 1500 0000  .....f..cfgr....
-00001ff0: 7215 0000 0072 1600 0000 da0a 7361 7665  r....r......save
-00002000: 5f6d 6f64 656c f400 0000 731c 0000 0000  _model....s.....
-00002010: 0906 0106 0208 0110 010a 010c 0108 020a  ................
-00002020: 010a 0210 010c 010a 0108 017a 1254 7261  ...........z.Tra
-00002030: 696e 6572 2e73 6176 655f 6d6f 6465 6c63  iner.save_modelc
-00002040: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00002050: 0900 0000 4300 0000 734a 0000 0074 007c  ....C...sJ...t.|
-00002060: 0174 0183 0272 1474 02a0 037c 01a1 017d  .t...r.t...|...}
-00002070: 017c 016a 046a 0564 0164 0164 028d 0201  .|.j.j.d.d.d....
-00002080: 0074 067c 0164 0383 028f 127d 0274 07a0  .t.|.d.....}.t..
-00002090: 087c 007c 02a1 0201 0057 0035 0051 0052  .|.|.....W.5.Q.R
-000020a0: 0058 0064 0453 0029 057a 9820 4d61 6b65  .X.d.S.).z. Make
-000020b0: 2061 2063 6865 636b 706f 696e 7420 6f66   a checkpoint of
-000020c0: 2074 6865 2074 7261 696e 6572 2e20 5468   the trainer. Th
-000020d0: 6973 2073 6176 6573 2074 6865 206d 6f64  is saves the mod
-000020e0: 656c 2061 7320 7765 6c6c 2061 730a 2020  el as well as.  
-000020f0: 2020 2020 2020 7468 6520 7472 6169 6e69        the traini
-00002100: 6e67 2073 7461 7465 732e 0a0a 2020 2020  ng states...    
-00002110: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00002120: 2020 2020 2020 7061 7468 3a20 5468 6520        path: The 
-00002130: 6669 6c65 2070 6174 682e 0a20 2020 2020  file path..     
-00002140: 2020 2054 7267 0000 0072 6a00 0000 4e29     Trg...rj...N)
-00002150: 0972 1f00 0000 726e 0000 0072 6f00 0000  .r....rn...ro...
-00002160: 7270 0000 0072 7100 0000 7272 0000 0072  rp...rq...rr...r
-00002170: 7300 0000 7276 0000 0072 7700 0000 2903  s...rv...rw...).
-00002180: 7228 0000 0072 7800 0000 727a 0000 0072  r(...rx...rz...r
-00002190: 1500 0000 7215 0000 0072 1600 0000 da0a  ....r....r......
-000021a0: 6368 6563 6b70 6f69 6e74 0f01 0000 730a  checkpoint....s.
-000021b0: 0000 0000 070a 010a 0210 020c 017a 1254  .............z.T
-000021c0: 7261 696e 6572 2e63 6865 636b 706f 696e  rainer.checkpoin
-000021d0: 7463 0100 0000 0000 0000 0000 0000 0400  tc..............
-000021e0: 0000 0a00 0000 4300 0000 7372 0000 0074  ......C...sr...t
-000021f0: 007c 0074 0183 0272 1474 02a0 037c 00a1  .|.t...r.t...|..
-00002200: 017d 007a 0c7c 00a0 04a1 007d 0157 006e  .}.z.|.....}.W.n
-00002210: 3004 0074 056b 0a72 5001 007d 0201 007a  0..t.k.rP..}...z
-00002220: 1274 0664 017c 029b 009d 0283 0182 0157  .t.d.|.........W
-00002230: 0035 0064 027d 027e 0258 0059 006e 0258  .5.d.}.~.X.Y.n.X
-00002240: 0074 07a0 087c 01a1 017d 0374 007c 0374  .t...|...}.t.|.t
-00002250: 0983 0273 6e74 0a64 0383 0182 017c 0353  ...snt.d.....|.S
-00002260: 0029 047a 9520 5265 7374 6f72 6520 6672  .).z. Restore fr
-00002270: 6f6d 2074 6865 2063 6865 636b 706f 696e  om the checkpoin
-00002280: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
-00002290: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-000022a0: 7468 3a20 5468 6520 6368 6563 6b70 6f69  th: The checkpoi
-000022b0: 6e74 2066 696c 6520 7061 7468 2e0a 0a20  nt file path... 
-000022c0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-000022d0: 2020 2020 2020 2020 2020 2020 4120 6e65              A ne
-000022e0: 7720 7472 6169 6e65 7220 6f62 6a65 6374  w trainer object
-000022f0: 2e0a 2020 2020 2020 2020 7a2e 436f 756c  ..        z.Coul
-00002300: 6420 6e6f 7420 6c6f 6164 2074 6865 2063  d not load the c
-00002310: 6865 636b 706f 696e 742e 2047 6f74 2065  heckpoint. Got e
-00002320: 7863 6570 7469 6f6e 3a20 4e7a 2954 6865  xception: Nz)The
-00002330: 2073 6176 6564 206f 626a 2069 7320 6e6f   saved obj is no
-00002340: 7420 6120 5472 6169 6e65 7220 6368 6563  t a Trainer chec
-00002350: 6b70 6f69 6e74 290b 721f 0000 0072 6e00  kpoint).r....rn.
-00002360: 0000 726f 0000 0072 7000 0000 da0a 7265  ..ro...rp.....re
-00002370: 6164 5f62 7974 6573 da0d 4261 7365 4578  ad_bytes..BaseEx
-00002380: 6365 7074 696f 6eda 074f 5345 7272 6f72  ception..OSError
-00002390: 7276 0000 00da 056c 6f61 6473 7218 0000  rv.....loadsr...
-000023a0: 00da 0954 7970 6545 7272 6f72 2904 7278  ...TypeError).rx
-000023b0: 0000 00da 065f 6279 7465 73da 0165 da07  ....._bytes..e..
-000023c0: 7472 6169 6e65 7272 1500 0000 7215 0000  trainerr....r...
-000023d0: 0072 1600 0000 da0f 6672 6f6d 5f63 6865  .r......from_che
-000023e0: 636b 706f 696e 741e 0100 0073 1400 0000  ckpoint....s....
-000023f0: 000a 0a01 0a02 0201 0c01 1001 2002 0a02  ............ ...
-00002400: 0a01 0802 7a17 5472 6169 6e65 722e 6672  ....z.Trainer.fr
-00002410: 6f6d 5f63 6865 636b 706f 696e 7463 0400  om_checkpointc..
-00002420: 0000 0000 0000 0000 0000 0c00 0000 0800  ................
-00002430: 0000 6300 0000 7398 0000 007c 0364 016b  ..c...s....|.d.k
-00002440: 0872 0e7c 006a 007d 037a 0c74 017c 0283  .r.|.j.}.z.t.|..
-00002450: 0101 0057 006e 1a04 0074 026b 0a72 3401  ...W.n...t.k.r4.
-00002460: 0001 0001 007c 0267 017d 0259 006e 0258  .....|.g.}.Y.n.X
-00002470: 0074 037c 0183 0144 005d 547d 0474 047c  .t.|...D.]T}.t.|
-00002480: 0483 015c 037d 057d 067d 077c 036a 057d  ...\.}.}.}.|.j.}
-00002490: 087c 087c 006a 067c 0583 027d 0974 0766  .|.|.j.|...}.t.f
-000024a0: 007c 057c 0964 029c 027c 0697 028e 017d  .|.|.d...|.....}
-000024b0: 0a7c 0244 005d 107d 0b7c 0b6a 0866 007c  .|.D.].}.|.j.f.|
-000024c0: 0a8e 0101 0071 7a7c 0256 0001 0071 3e64  .....qz|.V...q>d
-000024d0: 0153 0029 0361 4003 0000 2043 7265 6174  .S.).a@... Creat
-000024e0: 6520 7465 7374 2f76 616c 6964 6174 696f  e test/validatio
-000024f0: 6e20 6974 6572 6174 6f72 2e0a 0a20 2020  n iterator...   
-00002500: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00002510: 2020 2020 2020 2064 6174 6173 6574 3a20         dataset: 
-00002520: 416e 2069 7465 7261 746f 7220 6f72 2067  An iterator or g
-00002530: 656e 6572 6174 6f72 2066 756e 6374 696f  enerator functio
-00002540: 6e20 746f 2073 7570 706c 7920 7468 6520  n to supply the 
-00002550: 7465 7374 696e 6720 6461 7461 2e0a 2020  testing data..  
-00002560: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-00002570: 6520 6974 6572 6174 6f72 2073 686f 756c  e iterator shoul
-00002580: 6420 7969 656c 6420 6120 7475 7070 6c65  d yield a tupple
-00002590: 206f 6620 2869 6e70 7574 732c 206c 6162   of (inputs, lab
-000025a0: 656c 7329 2e20 5468 6520 6c61 6265 6c73  els). The labels
-000025b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000025c0: 2073 686f 756c 6420 6265 2061 2064 6963   should be a dic
-000025d0: 742e 0a20 2020 2020 2020 2020 2020 206d  t..            m
-000025e0: 6574 7269 6373 3a20 4120 6c69 7374 206f  etrics: A list o
-000025f0: 6620 4d65 7472 6963 206f 626a 6563 7473  f Metric objects
-00002600: 2e20 5468 6579 2073 686f 756c 6420 6861  . They should ha
-00002610: 7665 2074 776f 2066 756e 6374 696f 6e73  ve two functions
-00002620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002630: 2020 6d2e 7570 6461 7465 2870 7265 6473    m.update(preds
-00002640: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2070 7265 6473 2069 7320 7468 6520 6d6f   preds is the mo
-00002670: 6465 6c20 6f75 7470 7574 2e20 7468 6520  del output. the 
-00002680: 7265 6d61 696e 696e 6720 6b77 6172 6773  remaining kwargs
-00002690: 2061 7265 2063 6f6e 7465 6e74 206f 660a   are content of.
-000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026b0: 2020 2020 6c61 6265 6c73 2e0a 2020 2020      labels..    
-000026c0: 2020 2020 2020 2020 2020 2020 6d2e 636f              m.co
-000026d0: 6d70 7574 6528 293a 0a20 2020 2020 2020  mpute():.       
-000026e0: 2020 2020 2020 2020 2020 2020 2077 6869               whi
-000026f0: 6368 2073 686f 756c 6420 7265 7475 726e  ch should return
-00002700: 2074 6865 2061 6363 756d 756c 6174 6564   the accumulated
-00002710: 206d 6574 7269 6320 7661 6c75 652e 0a20   metric value.. 
-00002720: 2020 2020 2020 2020 2020 2073 7472 6174             strat
-00002730: 6567 793a 204f 7074 696f 6e61 6c6c 7920  egy: Optionally 
-00002740: 6f76 6572 7269 6465 2074 6865 2064 6566  override the def
-00002750: 6175 6c74 2073 7472 6174 6567 792e 0a20  ault strategy.. 
-00002760: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002770: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00002780: 2020 2020 2041 6e20 6974 6572 6174 6f72       An iterator
-00002790: 2e20 5374 6570 7069 6e67 2074 6872 6f75  . Stepping throu
-000027a0: 6768 2069 7420 7769 6c6c 2064 7269 7665  gh it will drive
-000027b0: 2074 6865 2075 7064 6174 696e 6720 6f66   the updating of
-000027c0: 2065 6163 6820 6d65 7472 6963 0a20 2020   each metric.   
-000027d0: 2020 2020 2020 2020 2020 2020 206f 626a               obj
-000027e0: 2e20 5468 6520 6974 6572 6174 6f72 2069  . The iterator i
-000027f0: 7473 656c 6620 7265 7475 726e 2074 6865  tself return the
-00002800: 206c 6973 7420 6f66 206d 6574 7269 6373   list of metrics
-00002810: 2e0a 2020 2020 2020 2020 4e29 0272 4700  ..        N).rG.
-00002820: 0000 7252 0000 0029 0972 2600 0000 7212  ..rR...).r&...r.
-00002830: 0000 0072 8200 0000 7217 0000 0072 3e00  ...r....r....r>.
-00002840: 0000 724d 0000 0072 4400 0000 726c 0000  ..rM...rD...rl..
-00002850: 00da 0675 7064 6174 6529 0c72 2800 0000  ...update).r(...
-00002860: 7245 0000 00da 076d 6574 7269 6373 720d  rE.....metricsr.
-00002870: 0000 0072 5e00 0000 7247 0000 0072 5f00  ...r^...rG...r_.
-00002880: 0000 7248 0000 0072 5100 0000 7252 0000  ..rH...rQ...rR..
-00002890: 0072 5000 0000 da01 6d72 1500 0000 7215  .rP.....mr....r.
-000028a0: 0000 0072 1600 0000 da04 7465 7374 3701  ...r......test7.
-000028b0: 0000 7326 0000 0000 1308 0106 0202 010c  ..s&............
-000028c0: 010e 010c 040c 010e 0106 010c 0104 0102  ................
-000028d0: 0102 fe04 0302 fd06 0508 010e 027a 0c54  .............z.T
-000028e0: 7261 696e 6572 2e74 6573 7463 0100 0000  rainer.testc....
-000028f0: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00002900: 4f00 0000 7320 0000 007c 006a 007c 017c  O...s ...|.j.|.|
-00002910: 028e 0144 005d 047d 0371 0c64 0164 0284  ...D.].}.q.d.d..
-00002920: 007c 0344 0083 0153 0029 037a b820 4120  .|.D...S.).z. A 
-00002930: 636f 6e76 6965 6e74 2066 756e 6374 696f  convient functio
-00002940: 6e20 746f 2063 6f6d 7075 7465 2061 6c6c  n to compute all
-00002950: 206d 6574 7269 6373 2e0a 0a20 2020 2020   metrics...     
-00002960: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00002970: 2020 2020 2073 616d 6520 6173 2074 6865       same as the
-00002980: 2074 6573 7428 2920 6675 636e 7469 6f6e   test() fucntion
-00002990: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000029a0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000029b0: 2020 2020 2020 2041 206d 6574 7269 6320         A metric 
-000029c0: 6469 6374 2e20 4b65 7973 2061 7265 206d  dict. Keys are m
-000029d0: 6574 7269 6320 6e61 6d65 732e 0a20 2020  etric names..   
-000029e0: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
-000029f0: 0000 0200 0000 0500 0000 5300 0000 731a  ..........S...s.
-00002a00: 0000 0069 007c 005d 127d 0174 007c 0183  ...i.|.].}.t.|..
-00002a10: 017c 01a0 01a1 0093 0271 0453 0072 1500  .|.......q.S.r..
-00002a20: 0000 2902 720a 0000 0072 5500 0000 2902  ..).r....rU...).
-00002a30: 722b 0000 0072 8900 0000 7215 0000 0072  r+...r....r....r
-00002a40: 1500 0000 7216 0000 0072 5600 0000 6d01  ....r....rV...m.
-00002a50: 0000 7306 0000 0006 0002 0006 007a 2c54  ..s..........z,T
-00002a60: 7261 696e 6572 2e74 6573 745f 616e 645f  rainer.test_and_
-00002a70: 636f 6d70 7574 652e 3c6c 6f63 616c 733e  compute.<locals>
-00002a80: 2e3c 6469 6374 636f 6d70 3e29 0172 8a00  .<dictcomp>).r..
-00002a90: 0000 2904 7228 0000 00da 0461 7267 7372  ..).r(.....argsr
-00002aa0: 5000 0000 7288 0000 0072 1500 0000 7215  P...r....r....r.
-00002ab0: 0000 0072 1600 0000 da10 7465 7374 5f61  ...r......test_a
-00002ac0: 6e64 5f63 6f6d 7075 7465 6201 0000 7306  nd_computeb...s.
-00002ad0: 0000 0000 0910 0102 017a 1854 7261 696e  .........z.Train
-00002ae0: 6572 2e74 6573 745f 616e 645f 636f 6d70  er.test_and_comp
-00002af0: 7574 6563 0100 0000 0000 0000 0000 0000  utec............
-00002b00: 0100 0000 0100 0000 4300 0000 7308 0000  ........C...s...
-00002b10: 007c 006a 006a 0153 0072 1100 0000 2902  .|.j.j.S.r....).
-00002b20: 7244 0000 0072 3900 0000 7236 0000 0072  rD...r9...r6...r
-00002b30: 1500 0000 7215 0000 0072 1600 0000 7239  ....r....r....r9
-00002b40: 0000 006f 0100 0073 0200 0000 0002 7a0e  ...o...s......z.
-00002b50: 5472 6169 6e65 722e 7061 7261 6d73 6302  Trainer.paramsc.
-00002b60: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00002b70: 0000 0043 0000 0073 1400 0000 7c00 6a00  ...C...s....|.j.
-00002b80: 6a01 7c01 6401 8d01 7c00 5f00 6400 5300  j.|.d...|._.d.S.
-00002b90: 2902 4e72 6600 0000 2902 7244 0000 0072  ).Nrf...).rD...r
-00002ba0: 4e00 0000 2902 7228 0000 00da 0a6e 6577  N...).r(.....new
-00002bb0: 5f70 6172 616d 7372 1500 0000 7215 0000  _paramsr....r...
-00002bc0: 0072 1600 0000 7239 0000 0073 0100 0073  .r....r9...s...s
-00002bd0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00002be0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00002bf0: 0600 0000 7c00 6a00 5300 7211 0000 0029  ....|.j.S.r....)
-00002c00: 0172 2500 0000 7236 0000 0072 1500 0000  .r%...r6...r....
-00002c10: 7215 0000 0072 1600 0000 721c 0000 0077  r....r....r....w
-00002c20: 0100 0073 0200 0000 0002 7a11 5472 6169  ...s......z.Trai
-00002c30: 6e65 722e 6f70 7469 6d69 7a65 7263 0200  ner.optimizerc..
-00002c40: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00002c50: 0000 4300 0000 7328 0000 007c 017c 005f  ..C...s(...|.|._
-00002c60: 007c 006a 0172 2474 026a 037c 006a 046a  .|.j.r$t.j.|.j.j
-00002c70: 057c 006a 067c 0164 018d 037c 005f 0764  .|.j.|.d...|._.d
-00002c80: 0053 0029 024e 723a 0000 0029 0872 2500  .S.).Nr:...).r%.
-00002c90: 0000 7227 0000 0072 0600 0000 7242 0000  ..r'...r....rB..
-00002ca0: 0072 1a00 0000 7243 0000 0072 3900 0000  .r....rC...r9...
-00002cb0: 7244 0000 0029 0272 2800 0000 7238 0000  rD...).r(...r8..
-00002cc0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00002cd0: 721c 0000 007b 0100 0073 0e00 0000 0002  r....{...s......
-00002ce0: 0602 0601 0401 0601 0401 02fd 2901 4e29  ............).N)
-00002cf0: 014e 2902 4e4e 2901 4e29 014e 2920 da08  .N).NN).N).N) ..
-00002d00: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00002d10: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00002d20: 5f5f da07 5f5f 646f 635f 5f72 0d00 0000  __..__doc__r....
-00002d30: da03 4a49 54da 026e 6eda 064d 6f64 756c  ..JIT..nn..Modul
-00002d40: 65da 0274 70da 084f 7074 696f 6e61 6cda  e..tp..Optional.
-00002d50: 064c 4f53 5345 5372 0700 0000 da03 696e  .LOSSESr......in
-00002d60: 74da 0474 7970 6572 2900 0000 7235 0000  t..typer)...r5..
-00002d70: 00da 0870 726f 7065 7274 7972 3700 0000  ...propertyr7...
-00002d80: 724b 0000 0072 5300 0000 7257 0000 0072  rK...rS...rW...r
-00002d90: 6400 0000 726e 0000 0072 7c00 0000 727d  d...rn...r|...r}
-00002da0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
-00002db0: 6472 8600 0000 728a 0000 0072 8c00 0000  dr....r....r....
-00002dc0: 7239 0000 00da 0673 6574 7465 7272 1c00  r9.....setterr..
-00002dd0: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00002de0: 0072 1600 0000 7218 0000 0023 0000 0073  .r....r....#...s
-00002df0: 4200 0000 0801 041d 0201 0201 0201 04fa  B...............
-00002e00: 0202 0401 0801 0201 0201 02fa 0c14 0a21  ...............!
-00002e10: 0201 0a03 1025 0e1a 0806 0a38 161b 080f  .....%.....8....
-00002e20: 0201 0a18 0a2b 080d 0201 0a03 0401 0a03  .....+..........
-00002e30: 0201 0a03 0401 7218 0000 0029 2572 7400  ......r....)%rt.
-00002e40: 0000 726f 0000 00da 0674 7970 696e 6772  ..ro.....typingr
-00002e50: 9500 0000 da09 6675 6e63 746f 6f6c 7372  ......functoolsr
-00002e60: 0200 0000 7203 0000 0072 7600 0000 da0a  ....r....rv.....
-00002e70: 666c 6178 2e6c 696e 656e da05 6c69 6e65  flax.linen..line
-00002e80: 6e72 9300 0000 7222 0000 00da 096a 6178  nr....r".....jax
-00002e90: 2e6e 756d 7079 da05 6e75 6d70 7972 2000  .numpy..numpyr .
-00002ea0: 0000 da15 666c 6178 2e63 6f72 652e 6672  ....flax.core.fr
-00002eb0: 6f7a 656e 5f64 6963 7472 0400 0000 7205  ozen_dictr....r.
-00002ec0: 0000 00da 1966 6c61 782e 7472 6169 6e69  .....flax.traini
-00002ed0: 6e67 2e74 7261 696e 5f73 7461 7465 7206  ng.train_stater.
-00002ee0: 0000 00da 056f 7074 6178 7207 0000 00da  .....optaxr.....
-00002ef0: 0575 7469 6c73 7209 0000 0072 0a00 0000  .utilsr....r....
-00002f00: da00 720d 0000 0072 5e00 0000 722c 0000  ..r....r^...r,..
-00002f10: 0072 1000 0000 724f 0000 00da 0555 6e69  .r....rO.....Uni
-00002f20: 6f6e da08 4361 6c6c 6162 6c65 da08 5365  on..Callable..Se
-00002f30: 7175 656e 6365 7297 0000 0072 1700 0000  quencer....r....
-00002f40: 7218 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00002f50: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-00002f60: 6c65 3e01 0000 0073 2400 0000 0801 0801  le>....s$.......
-00002f70: 0801 1002 0801 0c01 0801 0c01 1001 0c01  ................
-00002f80: 0c02 1001 0c01 0801 0c04 0802 1803 0809  ................
+00001de0: 8f16 7d05 740d a00e 7c03 7c04 6602 7c05  ..}.t...|.|.f.|.
+00001df0: a102 0100 5700 3500 5100 5200 5800 6401  ....W.5.Q.R.X.d.
+00001e00: 5300 2907 6101 0100 0020 5361 7665 2074  S.).a.... Save t
+00001e10: 6865 206d 6f64 656c 2069 6e20 6120 7069  he model in a pi
+00001e20: 636b 6c65 6420 6669 6c65 2e20 5468 6520  ckled file. The 
+00001e30: 7069 636b 6c65 2069 7320 6120 7475 706c  pickle is a tupl
+00001e40: 6520 6f66 0a20 2020 2020 2020 2020 2020  e of.           
+00001e50: 2028 6d6f 6475 6c65 2c20 7765 6967 6874   (module, weight
+00001e60: 7329 2e0a 0a20 2020 2020 2020 2041 7267  s)...        Arg
+00001e70: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00001e80: 6174 683a 2054 6865 2066 696c 6520 7061  ath: The file pa
+00001e90: 7468 2e0a 2020 2020 2020 2020 2020 2020  th..            
+00001ea0: 7375 625f 6d6f 6475 6c65 3a20 4f70 7469  sub_module: Opti
+00001eb0: 6f6e 616c 6c79 206f 6e6c 7920 7361 7665  onally only save
+00001ec0: 2061 2073 7562 5f6d 6f64 756c 6520 6f66   a sub_module of
+00001ed0: 2074 6865 206d 6f64 656c 0a20 2020 2020   the model.     
+00001ee0: 2020 2020 2020 2020 2020 2062 7920 7370             by sp
+00001ef0: 6563 6966 7969 6e67 2074 6865 206e 616d  ecifying the nam
+00001f00: 650a 2020 2020 2020 2020 4ea9 0172 3900  e.        N..r9.
+00001f10: 0000 7239 0000 0054 a902 da07 7061 7265  ..r9...T....pare
+00001f20: 6e74 73da 0865 7869 7374 5f6f 6bda 0277  nts..exist_ok..w
+00001f30: 6229 0f72 1a00 0000 7239 0000 00da 0462  b).r....r9.....b
+00001f40: 696e 64da 0464 6963 74da 0767 6574 6174  ind..dict..getat
+00001f50: 7472 7241 0000 0072 1f00 0000 da03 7374  trrA...r......st
+00001f60: 72da 0770 6174 686c 6962 da04 5061 7468  r..pathlib..Path
+00001f70: da06 7061 7265 6e74 da05 6d6b 6469 72da  ..parent..mkdir.
+00001f80: 046f 7065 6eda 0b63 6c6f 7564 7069 636b  .open..cloudpick
+00001f90: 6c65 da04 6475 6d70 2906 7228 0000 00da  le..dump).r(....
+00001fa0: 0470 6174 6872 6500 0000 da06 6d6f 6475  .pathre.....modu
+00001fb0: 6c65 7239 0000 00da 0166 7215 0000 0072  ler9.....fr....r
+00001fc0: 1500 0000 7216 0000 00da 0a73 6176 655f  ....r......save_
+00001fd0: 6d6f 6465 6cf4 0000 0073 1800 0000 0009  model....s......
+00001fe0: 0601 0602 0801 1001 0a01 0c01 0802 0a01  ................
+00001ff0: 0a02 1001 0c01 7a12 5472 6169 6e65 722e  ......z.Trainer.
+00002000: 7361 7665 5f6d 6f64 656c 6302 0000 0000  save_modelc.....
+00002010: 0000 0000 0000 0003 0000 0009 0000 0043  ...............C
+00002020: 0000 0073 4a00 0000 7400 7c01 7401 8302  ...sJ...t.|.t...
+00002030: 7214 7402 a003 7c01 a101 7d01 7c01 6a04  r.t...|...}.|.j.
+00002040: 6a05 6401 6401 6402 8d02 0100 7406 7c01  j.d.d.d.....t.|.
+00002050: 6403 8302 8f12 7d02 7407 a008 7c00 7c02  d.....}.t...|.|.
+00002060: a102 0100 5700 3500 5100 5200 5800 6404  ....W.5.Q.R.X.d.
+00002070: 5300 2905 7a98 204d 616b 6520 6120 6368  S.).z. Make a ch
+00002080: 6563 6b70 6f69 6e74 206f 6620 7468 6520  eckpoint of the 
+00002090: 7472 6169 6e65 722e 2054 6869 7320 7361  trainer. This sa
+000020a0: 7665 7320 7468 6520 6d6f 6465 6c20 6173  ves the model as
+000020b0: 2077 656c 6c20 6173 0a20 2020 2020 2020   well as.       
+000020c0: 2074 6865 2074 7261 696e 696e 6720 7374   the training st
+000020d0: 6174 6573 2e0a 0a20 2020 2020 2020 2041  ates...        A
+000020e0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+000020f0: 2070 6174 683a 2054 6865 2066 696c 6520   path: The file 
+00002100: 7061 7468 2e0a 2020 2020 2020 2020 5472  path..        Tr
+00002110: 6700 0000 726a 0000 004e 2909 721f 0000  g...rj...N).r...
+00002120: 0072 6e00 0000 726f 0000 0072 7000 0000  .rn...ro...rp...
+00002130: 7271 0000 0072 7200 0000 7273 0000 0072  rq...rr...rs...r
+00002140: 7400 0000 7275 0000 0029 0372 2800 0000  t...ru...).r(...
+00002150: 7276 0000 0072 7800 0000 7215 0000 0072  rv...rx...r....r
+00002160: 1500 0000 7216 0000 00da 0a63 6865 636b  ....r......check
+00002170: 706f 696e 740d 0100 0073 0a00 0000 0007  point....s......
+00002180: 0a01 0a02 1002 0c01 7a12 5472 6169 6e65  ........z.Traine
+00002190: 722e 6368 6563 6b70 6f69 6e74 6301 0000  r.checkpointc...
+000021a0: 0000 0000 0000 0000 0004 0000 000a 0000  ................
+000021b0: 0043 0000 0073 7200 0000 7400 7c00 7401  .C...sr...t.|.t.
+000021c0: 8302 7214 7402 a003 7c00 a101 7d00 7a0c  ..r.t...|...}.z.
+000021d0: 7c00 a004 a100 7d01 5700 6e30 0400 7405  |.....}.W.n0..t.
+000021e0: 6b0a 7250 0100 7d02 0100 7a12 7406 6401  k.rP..}...z.t.d.
+000021f0: 7c02 9b00 9d02 8301 8201 5700 3500 6402  |.........W.5.d.
+00002200: 7d02 7e02 5800 5900 6e02 5800 7407 a008  }.~.X.Y.n.X.t...
+00002210: 7c01 a101 7d03 7400 7c03 7409 8302 736e  |...}.t.|.t...sn
+00002220: 740a 6403 8301 8201 7c03 5300 2904 7a95  t.d.....|.S.).z.
+00002230: 2052 6573 746f 7265 2066 726f 6d20 7468   Restore from th
+00002240: 6520 6368 6563 6b70 6f69 6e74 2e0a 0a20  e checkpoint... 
+00002250: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00002260: 2020 2020 2020 2020 2070 6174 683a 2054           path: T
+00002270: 6865 2063 6865 636b 706f 696e 7420 6669  he checkpoint fi
+00002280: 6c65 2070 6174 682e 0a0a 2020 2020 2020  le path...      
+00002290: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000022a0: 2020 2020 2020 2041 206e 6577 2074 7261         A new tra
+000022b0: 696e 6572 206f 626a 6563 742e 0a20 2020  iner object..   
+000022c0: 2020 2020 207a 2e43 6f75 6c64 206e 6f74       z.Could not
+000022d0: 206c 6f61 6420 7468 6520 6368 6563 6b70   load the checkp
+000022e0: 6f69 6e74 2e20 476f 7420 6578 6365 7074  oint. Got except
+000022f0: 696f 6e3a 204e 7a29 5468 6520 7361 7665  ion: Nz)The save
+00002300: 6420 6f62 6a20 6973 206e 6f74 2061 2054  d obj is not a T
+00002310: 7261 696e 6572 2063 6865 636b 706f 696e  rainer checkpoin
+00002320: 7429 0b72 1f00 0000 726e 0000 0072 6f00  t).r....rn...ro.
+00002330: 0000 7270 0000 00da 0a72 6561 645f 6279  ..rp.....read_by
+00002340: 7465 73da 0d42 6173 6545 7863 6570 7469  tes..BaseExcepti
+00002350: 6f6e da07 4f53 4572 726f 7272 7400 0000  on..OSErrorrt...
+00002360: da05 6c6f 6164 7372 1800 0000 da09 5479  ..loadsr......Ty
+00002370: 7065 4572 726f 7229 0472 7600 0000 da06  peError).rv.....
+00002380: 5f62 7974 6573 da01 65da 0774 7261 696e  _bytes..e..train
+00002390: 6572 7215 0000 0072 1500 0000 7216 0000  err....r....r...
+000023a0: 00da 0f66 726f 6d5f 6368 6563 6b70 6f69  ...from_checkpoi
+000023b0: 6e74 1c01 0000 7314 0000 0000 0a0a 010a  nt....s.........
+000023c0: 0202 010c 0110 0120 020a 020a 0108 027a  ....... .......z
+000023d0: 1754 7261 696e 6572 2e66 726f 6d5f 6368  .Trainer.from_ch
+000023e0: 6563 6b70 6f69 6e74 6304 0000 0000 0000  eckpointc.......
+000023f0: 0000 0000 000c 0000 0008 0000 0063 0000  .............c..
+00002400: 0073 9800 0000 7c03 6401 6b08 720e 7c00  .s....|.d.k.r.|.
+00002410: 6a00 7d03 7a0c 7401 7c02 8301 0100 5700  j.}.z.t.|.....W.
+00002420: 6e1a 0400 7402 6b0a 7234 0100 0100 0100  n...t.k.r4......
+00002430: 7c02 6701 7d02 5900 6e02 5800 7403 7c01  |.g.}.Y.n.X.t.|.
+00002440: 8301 4400 5d54 7d04 7404 7c04 8301 5c03  ..D.]T}.t.|...\.
+00002450: 7d05 7d06 7d07 7c03 6a05 7d08 7c08 7c00  }.}.}.|.j.}.|.|.
+00002460: 6a06 7c05 8302 7d09 7407 6600 7c05 7c09  j.|...}.t.f.|.|.
+00002470: 6402 9c02 7c06 9702 8e01 7d0a 7c02 4400  d...|.....}.|.D.
+00002480: 5d10 7d0b 7c0b 6a08 6600 7c0a 8e01 0100  ].}.|.j.f.|.....
+00002490: 717a 7c02 5600 0100 713e 6401 5300 2903  qz|.V...q>d.S.).
+000024a0: 6140 0300 0020 4372 6561 7465 2074 6573  a@... Create tes
+000024b0: 742f 7661 6c69 6461 7469 6f6e 2069 7465  t/validation ite
+000024c0: 7261 746f 722e 0a0a 2020 2020 2020 2020  rator...        
+000024d0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000024e0: 2020 6461 7461 7365 743a 2041 6e20 6974    dataset: An it
+000024f0: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
+00002500: 746f 7220 6675 6e63 7469 6f6e 2074 6f20  tor function to 
+00002510: 7375 7070 6c79 2074 6865 2074 6573 7469  supply the testi
+00002520: 6e67 2064 6174 612e 0a20 2020 2020 2020  ng data..       
+00002530: 2020 2020 2020 2020 2054 6865 2069 7465           The ite
+00002540: 7261 746f 7220 7368 6f75 6c64 2079 6965  rator should yie
+00002550: 6c64 2061 2074 7570 706c 6520 6f66 2028  ld a tupple of (
+00002560: 696e 7075 7473 2c20 6c61 6265 6c73 292e  inputs, labels).
+00002570: 2054 6865 206c 6162 656c 730a 2020 2020   The labels.    
+00002580: 2020 2020 2020 2020 2020 2020 7368 6f75              shou
+00002590: 6c64 2062 6520 6120 6469 6374 2e0a 2020  ld be a dict..  
+000025a0: 2020 2020 2020 2020 2020 6d65 7472 6963            metric
+000025b0: 733a 2041 206c 6973 7420 6f66 204d 6574  s: A list of Met
+000025c0: 7269 6320 6f62 6a65 6374 732e 2054 6865  ric objects. The
+000025d0: 7920 7368 6f75 6c64 2068 6176 6520 7477  y should have tw
+000025e0: 6f20 6675 6e63 7469 6f6e 733a 0a20 2020  o functions:.   
+000025f0: 2020 2020 2020 2020 2020 2020 206d 2e75               m.u
+00002600: 7064 6174 6528 7072 6564 732c 202a 2a6b  pdate(preds, **k
+00002610: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00002620: 2020 2020 2020 2020 2020 2020 7072 6564              pred
+00002630: 7320 6973 2074 6865 206d 6f64 656c 206f  s is the model o
+00002640: 7574 7075 742e 2074 6865 2072 656d 6169  utput. the remai
+00002650: 6e69 6e67 206b 7761 7267 7320 6172 6520  ning kwargs are 
+00002660: 636f 6e74 656e 7420 6f66 0a20 2020 2020  content of.     
+00002670: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002680: 6162 656c 732e 0a20 2020 2020 2020 2020  abels..         
+00002690: 2020 2020 2020 206d 2e63 6f6d 7075 7465         m.compute
+000026a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000026b0: 2020 2020 2020 2020 7768 6963 6820 7368          which sh
+000026c0: 6f75 6c64 2072 6574 7572 6e20 7468 6520  ould return the 
+000026d0: 6163 6375 6d75 6c61 7465 6420 6d65 7472  accumulated metr
+000026e0: 6963 2076 616c 7565 2e0a 2020 2020 2020  ic value..      
+000026f0: 2020 2020 2020 7374 7261 7465 6779 3a20        strategy: 
+00002700: 4f70 7469 6f6e 616c 6c79 206f 7665 7272  Optionally overr
+00002710: 6964 6520 7468 6520 6465 6661 756c 7420  ide the default 
+00002720: 7374 7261 7465 6779 2e0a 2020 2020 2020  strategy..      
+00002730: 2020 0a20 2020 2020 2020 2052 6574 7572    .        Retur
+00002740: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00002750: 416e 2069 7465 7261 746f 722e 2053 7465  An iterator. Ste
+00002760: 7070 696e 6720 7468 726f 7567 6820 6974  pping through it
+00002770: 2077 696c 6c20 6472 6976 6520 7468 6520   will drive the 
+00002780: 7570 6461 7469 6e67 206f 6620 6561 6368  updating of each
+00002790: 206d 6574 7269 630a 2020 2020 2020 2020   metric.        
+000027a0: 2020 2020 2020 2020 6f62 6a2e 2054 6865          obj. The
+000027b0: 2069 7465 7261 746f 7220 6974 7365 6c66   iterator itself
+000027c0: 2072 6574 7572 6e20 7468 6520 6c69 7374   return the list
+000027d0: 206f 6620 6d65 7472 6963 732e 0a20 2020   of metrics..   
+000027e0: 2020 2020 204e 2902 7247 0000 0072 5200       N).rG...rR.
+000027f0: 0000 2909 7226 0000 0072 1200 0000 727f  ..).r&...r....r.
+00002800: 0000 0072 1700 0000 723e 0000 0072 4d00  ...r....r>...rM.
+00002810: 0000 7244 0000 0072 6c00 0000 da06 7570  ..rD...rl.....up
+00002820: 6461 7465 290c 7228 0000 0072 4500 0000  date).r(...rE...
+00002830: da07 6d65 7472 6963 7372 0d00 0000 725e  ..metricsr....r^
+00002840: 0000 0072 4700 0000 725f 0000 0072 4800  ...rG...r_...rH.
+00002850: 0000 7251 0000 0072 5200 0000 7250 0000  ..rQ...rR...rP..
+00002860: 00da 016d 7215 0000 0072 1500 0000 7216  ...mr....r....r.
+00002870: 0000 00da 0474 6573 7435 0100 0073 2600  .....test5...s&.
+00002880: 0000 0013 0801 0602 0201 0c01 0e01 0c04  ................
+00002890: 0c01 0e01 0601 0c01 0401 0201 02fe 0403  ................
+000028a0: 02fd 0605 0801 0e02 7a0c 5472 6169 6e65  ........z.Traine
+000028b0: 722e 7465 7374 6301 0000 0000 0000 0000  r.testc.........
+000028c0: 0000 0004 0000 0003 0000 004f 0000 0073  ...........O...s
+000028d0: 2000 0000 7c00 6a00 7c01 7c02 8e01 4400   ...|.j.|.|...D.
+000028e0: 5d04 7d03 710c 6401 6402 8400 7c03 4400  ].}.q.d.d...|.D.
+000028f0: 8301 5300 2903 7ab8 2041 2063 6f6e 7669  ..S.).z. A convi
+00002900: 656e 7420 6675 6e63 7469 6f6e 2074 6f20  ent function to 
+00002910: 636f 6d70 7574 6520 616c 6c20 6d65 7472  compute all metr
+00002920: 6963 732e 0a0a 2020 2020 2020 2020 4172  ics...        Ar
+00002930: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00002940: 7361 6d65 2061 7320 7468 6520 7465 7374  same as the test
+00002950: 2829 2066 7563 6e74 696f 6e0a 2020 2020  () fucntion.    
+00002960: 2020 2020 0a20 2020 2020 2020 2052 6574      .        Ret
+00002970: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00002980: 2020 4120 6d65 7472 6963 2064 6963 742e    A metric dict.
+00002990: 204b 6579 7320 6172 6520 6d65 7472 6963   Keys are metric
+000029a0: 206e 616d 6573 2e0a 2020 2020 2020 2020   names..        
+000029b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000029c0: 0005 0000 0053 0000 0073 1a00 0000 6900  .....S...s....i.
+000029d0: 7c00 5d12 7d01 7400 7c01 8301 7c01 a001  |.].}.t.|...|...
+000029e0: a100 9302 7104 5300 7215 0000 0029 0272  ....q.S.r....).r
+000029f0: 0a00 0000 7255 0000 0029 0272 2b00 0000  ....rU...).r+...
+00002a00: 7286 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00002a10: 1600 0000 7256 0000 006b 0100 0073 0600  ....rV...k...s..
+00002a20: 0000 0600 0200 0600 7a2c 5472 6169 6e65  ........z,Traine
+00002a30: 722e 7465 7374 5f61 6e64 5f63 6f6d 7075  r.test_and_compu
+00002a40: 7465 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  te.<locals>.<dic
+00002a50: 7463 6f6d 703e 2901 7287 0000 0029 0472  tcomp>).r....).r
+00002a60: 2800 0000 da04 6172 6773 7250 0000 0072  (.....argsrP...r
+00002a70: 8500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00002a80: 0000 00da 1074 6573 745f 616e 645f 636f  .....test_and_co
+00002a90: 6d70 7574 6560 0100 0073 0600 0000 0009  mpute`...s......
+00002aa0: 1001 0201 7a18 5472 6169 6e65 722e 7465  ....z.Trainer.te
+00002ab0: 7374 5f61 6e64 5f63 6f6d 7075 7465 6301  st_and_computec.
+00002ac0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00002ad0: 0000 0043 0000 0073 0800 0000 7c00 6a00  ...C...s....|.j.
+00002ae0: 6a01 5300 7211 0000 0029 0272 4400 0000  j.S.r....).rD...
+00002af0: 7239 0000 0072 3600 0000 7215 0000 0072  r9...r6...r....r
+00002b00: 1500 0000 7216 0000 0072 3900 0000 6d01  ....r....r9...m.
+00002b10: 0000 7302 0000 0000 027a 0e54 7261 696e  ..s......z.Train
+00002b20: 6572 2e70 6172 616d 7363 0200 0000 0000  er.paramsc......
+00002b30: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00002b40: 0000 7314 0000 007c 006a 006a 017c 0164  ..s....|.j.j.|.d
+00002b50: 018d 017c 005f 0064 0053 0029 024e 7266  ...|._.d.S.).Nrf
+00002b60: 0000 0029 0272 4400 0000 724e 0000 0029  ...).rD...rN...)
+00002b70: 0272 2800 0000 da0a 6e65 775f 7061 7261  .r(.....new_para
+00002b80: 6d73 7215 0000 0072 1500 0000 7216 0000  msr....r....r...
+00002b90: 0072 3900 0000 7101 0000 7302 0000 0000  .r9...q...s.....
+00002ba0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+00002bb0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00002bc0: 006a 0053 0072 1100 0000 2901 7225 0000  .j.S.r....).r%..
+00002bd0: 0072 3600 0000 7215 0000 0072 1500 0000  .r6...r....r....
+00002be0: 7216 0000 0072 1c00 0000 7501 0000 7302  r....r....u...s.
+00002bf0: 0000 0000 027a 1154 7261 696e 6572 2e6f  .....z.Trainer.o
+00002c00: 7074 696d 697a 6572 6302 0000 0000 0000  ptimizerc.......
+00002c10: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00002c20: 0073 2800 0000 7c01 7c00 5f00 7c00 6a01  .s(...|.|._.|.j.
+00002c30: 7224 7402 6a03 7c00 6a04 6a05 7c00 6a06  r$t.j.|.j.j.|.j.
+00002c40: 7c01 6401 8d03 7c00 5f07 6400 5300 2902  |.d...|._.d.S.).
+00002c50: 4e72 3a00 0000 2908 7225 0000 0072 2700  Nr:...).r%...r'.
+00002c60: 0000 7206 0000 0072 4200 0000 721a 0000  ..r....rB...r...
+00002c70: 0072 4300 0000 7239 0000 0072 4400 0000  .rC...r9...rD...
+00002c80: 2902 7228 0000 0072 3800 0000 7215 0000  ).r(...r8...r...
+00002c90: 0072 1500 0000 7216 0000 0072 1c00 0000  .r....r....r....
+00002ca0: 7901 0000 730e 0000 0000 0206 0206 0104  y...s...........
+00002cb0: 0106 0104 0102 fd29 014e 2901 4e29 024e  .......).N).N).N
+00002cc0: 4e29 014e 2901 4e29 20da 085f 5f6e 616d  N).N).N) ..__nam
+00002cd0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00002ce0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00002cf0: 5f64 6f63 5f5f 720d 0000 00da 034a 4954  _doc__r......JIT
+00002d00: da02 6e6e da06 4d6f 6475 6c65 da02 7470  ..nn..Module..tp
+00002d10: da08 4f70 7469 6f6e 616c da06 4c4f 5353  ..Optional..LOSS
+00002d20: 4553 7207 0000 00da 0369 6e74 da04 7479  ESr......int..ty
+00002d30: 7065 7229 0000 0072 3500 0000 da08 7072  per)...r5.....pr
+00002d40: 6f70 6572 7479 7237 0000 0072 4b00 0000  opertyr7...rK...
+00002d50: 7253 0000 0072 5700 0000 7264 0000 0072  rS...rW...rd...r
+00002d60: 6e00 0000 7279 0000 0072 7a00 0000 da0c  n...ry...rz.....
+00002d70: 7374 6174 6963 6d65 7468 6f64 7283 0000  staticmethodr...
+00002d80: 0072 8700 0000 7289 0000 0072 3900 0000  .r....r....r9...
+00002d90: da06 7365 7474 6572 721c 0000 0072 1500  ..setterr....r..
+00002da0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00002db0: 0072 1800 0000 2300 0000 7342 0000 0008  .r....#...sB....
+00002dc0: 0104 1d02 0102 0102 0104 fa02 0204 0108  ................
+00002dd0: 0102 0102 0102 fa0c 140a 2102 010a 0310  ..........!.....
+00002de0: 250e 1a08 060a 3816 1908 0f02 010a 180a  %.....8.........
+00002df0: 2b08 0d02 010a 0304 010a 0302 010a 0304  +...............
+00002e00: 0172 1800 0000 2925 da0b 6461 7461 636c  .r....)%..datacl
+00002e10: 6173 7365 7372 6f00 0000 da06 7479 7069  assesro.....typi
+00002e20: 6e67 7292 0000 00da 0966 756e 6374 6f6f  ngr......functoo
+00002e30: 6c73 7202 0000 0072 0300 0000 7274 0000  lsr....r....rt..
+00002e40: 00da 0a66 6c61 782e 6c69 6e65 6eda 056c  ...flax.linen..l
+00002e50: 696e 656e 7290 0000 0072 2200 0000 da09  inenr....r".....
+00002e60: 6a61 782e 6e75 6d70 79da 056e 756d 7079  jax.numpy..numpy
+00002e70: 7220 0000 00da 1566 6c61 782e 636f 7265  r .....flax.core
+00002e80: 2e66 726f 7a65 6e5f 6469 6374 7204 0000  .frozen_dictr...
+00002e90: 0072 0500 0000 da19 666c 6178 2e74 7261  .r......flax.tra
+00002ea0: 696e 696e 672e 7472 6169 6e5f 7374 6174  ining.train_stat
+00002eb0: 6572 0600 0000 da05 6f70 7461 7872 0700  er......optaxr..
+00002ec0: 0000 da05 7574 696c 7372 0900 0000 720a  ....utilsr....r.
+00002ed0: 0000 00da 0072 0d00 0000 725e 0000 0072  .....r....r^...r
+00002ee0: 2c00 0000 7210 0000 0072 4f00 0000 da05  ,...r....rO.....
+00002ef0: 556e 696f 6eda 0843 616c 6c61 626c 65da  Union..Callable.
+00002f00: 0853 6571 7565 6e63 6572 9400 0000 7217  .Sequencer....r.
+00002f10: 0000 0072 1800 0000 7215 0000 0072 1500  ...r....r....r..
+00002f20: 0000 7215 0000 0072 1600 0000 da08 3c6d  ..r....r......<m
+00002f30: 6f64 756c 653e 0100 0000 7324 0000 0008  odule>....s$....
+00002f40: 0108 0108 0110 0208 010c 0108 010c 0110  ................
+00002f50: 010c 010c 0210 010c 0108 010c 0408 0218  ................
+00002f60: 0308 09                                  ...
```

### Comparing `lacss-0.4.0/lacss/train/data/__init__.py` & `lacss-0.4.1/lacss/train/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/__init__.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/data_handler.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/data_handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/dataset.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/dataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/__pycache__/utils.cpython-38.pyc` & `lacss-0.4.1/lacss/train/data/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/array_adapter.py` & `lacss-0.4.1/lacss/train/data/array_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/data_adapter.py` & `lacss-0.4.1/lacss/train/data/data_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/data_handler.py` & `lacss-0.4.1/lacss/train/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/dataset.py` & `lacss-0.4.1/lacss/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/generator_adapter.py` & `lacss-0.4.1/lacss/train/data/generator_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/list_adapter.py` & `lacss-0.4.1/lacss/train/data/list_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/tf_dataset_adapter.py` & `lacss-0.4.1/lacss/train/data/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/torch_dataloader_adapter.py` & `lacss-0.4.1/lacss/train/data/torch_dataloader_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/data/utils.py` & `lacss-0.4.1/lacss/train/data/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/loss.py` & `lacss-0.4.1/lacss/train/loss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/strategy.py` & `lacss-0.4.1/lacss/train/strategy.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/lacss/train/trainer.py` & `lacss-0.4.1/lacss/train/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,17 +260,15 @@
             params = params["params"]
 
         if isinstance(path, str):
             path = pathlib.Path(path)
 
         path.parent.mkdir(parents=True, exist_ok=True)
         with open(path, "wb") as f:
-            cfg = dataclasses.asdict(module)
-            params = unfreeze(params)
-            cloudpickle.dump((cfg, params), f)
+            cloudpickle.dump((module, params), f)
 
     def checkpoint(self, path):
         """ Make a checkpoint of the trainer. This saves the model as well as
         the training states.
 
         Args:
             path: The file path.
```

### Comparing `lacss-0.4.0/lacss/utils.py` & `lacss-0.4.1/lacss/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.0/pyproject.toml` & `lacss-0.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacss"
-version = "0.4.0"
+version = "0.4.1"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
```

### Comparing `lacss-0.4.0/PKG-INFO` & `lacss-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacss
-Version: 0.4.0
+Version: 0.4.1
 Summary: Cell segmentation and tracking
 License: MIT
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

