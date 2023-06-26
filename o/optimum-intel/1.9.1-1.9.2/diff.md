# Comparing `tmp/optimum-intel-1.9.1.tar.gz` & `tmp/optimum-intel-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-intel-1.9.1.tar", last modified: Thu Jun 15 15:43:12 2023, max compression
+gzip compressed data, was "optimum-intel-1.9.2.tar", last modified: Mon Jun 26 22:28:05 2023, max compression
```

## Comparing `optimum-intel-1.9.1.tar` & `optimum-intel-1.9.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/commands/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/commands/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/commands/neural_compressor/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/commands/neural_compressor/quantize.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/commands/register/register_inc.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/intel/
--rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/intel/generation/
--rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/generation/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/generation/modeling.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/intel/ipex/
--rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/ipex/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/ipex/inference.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.485665 optimum-intel-1.9.1/optimum/intel/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3730 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/launcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/neural_coder_adaptor.py
--rw-r--r--   0 ella      (1000) ella      (1000)    27858 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38957 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.485665 optimum-intel-1.9.1/optimum/intel/openvino/
--rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15434 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18258 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_base_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17577 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    28970 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18032 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    14161 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/optimum/intel/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_ipex_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/modeling_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-15 15:40:31.000000 optimum-intel-1.9.1/optimum/intel/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/optimum_intel.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-15 15:43:11.000000 optimum-intel-1.9.1/optimum_intel.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-15 15:43:11.000000 optimum-intel-1.9.1/optimum_intel.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-15 15:43:11.000000 optimum-intel-1.9.1/optimum_intel.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)      441 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     2671 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.756608 optimum-intel-1.9.2/optimum/commands/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/commands/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/commands/neural_compressor/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/commands/neural_compressor/quantize.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/commands/register/register_inc.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/intel/
+-rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.776608 optimum-intel-1.9.2/optimum/intel/generation/
+-rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/generation/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/generation/modeling.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.776608 optimum-intel-1.9.2/optimum/intel/ipex/
+-rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/ipex/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/ipex/inference.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.776608 optimum-intel-1.9.2/optimum/intel/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3801 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/launcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/neural_coder_adaptor.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28880 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    39154 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/optimum/intel/openvino/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15434 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18258 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_base_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17577 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28970 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18032 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    14161 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/optimum/intel/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_ipex_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9057 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/modeling_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-26 22:25:58.000000 optimum-intel-1.9.2/optimum/intel/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/optimum_intel.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-26 22:28:04.000000 optimum-intel-1.9.2/optimum_intel.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-26 22:28:04.000000 optimum-intel-1.9.2/optimum_intel.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)      441 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     2671 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/setup.py
```

### Comparing `optimum-intel-1.9.1/LICENSE` & `optimum-intel-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/MANIFEST.in` & `optimum-intel-1.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/PKG-INFO` & `optimum-intel-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.1
+Version: 1.9.2
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.1/README.md` & `optimum-intel-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/commands/neural_compressor/base.py` & `optimum-intel-1.9.2/optimum/commands/neural_compressor/base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/commands/neural_compressor/quantize.py` & `optimum-intel-1.9.2/optimum/commands/neural_compressor/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/commands/register/register_inc.py` & `optimum-intel-1.9.2/optimum/commands/register/register_inc.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/__init__.py` & `optimum-intel-1.9.2/optimum/intel/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/generation/__init__.py` & `optimum-intel-1.9.2/optimum/intel/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/generation/modeling.py` & `optimum-intel-1.9.2/optimum/intel/generation/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/ipex/inference.py` & `optimum-intel-1.9.2/optimum/intel/ipex/inference.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/__init__.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/configuration.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,16 @@
                 # "frequency": weight_compression.pruning_frequency,
             }
         return config
 
     @staticmethod
     def _create_distillation_config(config: Union[Dict, DistillationConfig]):
         if isinstance(config, DistillationConfig):
-            criterion = next(iter(config.criterion.values()))
+            criterion = getattr(config.criterion, "config", config.criterion)
+            criterion = next(iter(criterion.values()))
             config = {
                 "teacher_model_name_or_path": config.teacher_model.config._name_or_path,
                 "temperature": criterion.temperature,
                 # "loss_types": criterion.loss_types,
                 # "loss_weights": criterion.loss_weights,
             }
         return config
```

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/modeling_diffusion.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/neural_coder_adaptor.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/neural_coder_adaptor.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/quantization.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/quantization.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from enum import Enum
 from itertools import chain
 from pathlib import Path
 from typing import Callable, ClassVar, Dict, Optional, Union
 
 import torch
 from datasets import Dataset, load_dataset
-from huggingface_hub import HfApi, hf_hub_download
+from huggingface_hub import hf_hub_download
 from neural_compressor.adaptor.pytorch import PyTorch_FXAdaptor, _cfg_to_qconfig, _propagate_qconfig
 from neural_compressor.config import PostTrainingQuantConfig
 from neural_compressor.experimental.export import torch_to_int8_onnx
 from neural_compressor.model.torch_model import IPEXModel, PyTorchModel
 from neural_compressor.quantization import fit
 from neural_compressor.utils.pytorch import load
 from torch.utils.data import DataLoader, RandomSampler
@@ -56,26 +56,29 @@
 
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
 from optimum.quantization_base import OptimumQuantizer
 
 from ..utils.constant import _TASK_ALIASES, MIN_QDQ_ONNX_OPSET, ONNX_WEIGHTS_NAME, WEIGHTS_NAME
 from ..utils.import_utils import (
+    _ipex_version,
     _neural_compressor_version,
     _torch_version,
+    is_ipex_version,
     is_neural_compressor_version,
     is_torch_version,
 )
 from .configuration import INCConfig
 from .utils import INCDataLoader, _cfgs_to_fx_cfgs
 
 
 logger = logging.getLogger(__name__)
 
 NEURAL_COMPRESSOR_MINIMUM_VERSION = "2.1.0"
+IPEX_MINIMUM_VERSION = "2.1.0"
 
 if is_neural_compressor_version("<", NEURAL_COMPRESSOR_MINIMUM_VERSION):
     raise ImportError(
         f"Found an incompatible version of neural-compressor. Found version {_neural_compressor_version}, "
         f"but only version {NEURAL_COMPRESSOR_MINIMUM_VERSION} or higher is supported."
     )
 
@@ -159,14 +162,15 @@
                 Whether or not to remove the columns unused by the model forward method.
         """
         save_directory = Path(save_directory)
         save_directory.mkdir(parents=True, exist_ok=True)
         save_onnx_model = kwargs.pop("save_onnx_model", False)
         output_path = save_directory.joinpath(file_name or WEIGHTS_NAME)
         calibration_dataloader = None
+        self._set_task()
 
         if INCQuantizationMode(quantization_config.approach) == INCQuantizationMode.STATIC:
             # Since PyTorch fx trace does not really require an example_inputs, only need calibration_dataset or calibration_fn here.
             if calibration_dataset is None and self.calibration_fn is None:
                 raise ValueError(
                     "Post-training static quantization needs a calibration dataset or a calibration_function."
                 )
@@ -177,14 +181,32 @@
                 calibration_dataloader = self._get_calibration_dataloader(
                     calibration_dataset=calibration_dataset,
                     batch_size=batch_size,
                     remove_unused_columns=remove_unused_columns,
                     data_collator=data_collator,
                 )
 
+        # Disable ONNX export for post-training quantized model as deprecated in neural-compressor>=2.2.0
+        if save_onnx_model:
+            logger.warning(
+                "ONNX export for post-training quantized model is no longer supported by neural-compressor>=2.2.0. "
+                "To apply quantization on an ONNX model, check out optimum.onnxruntime.ORTQuantizer"
+            )
+            save_onnx_model = False
+
+        if (
+            quantization_config.backend == "ipex"
+            and is_ipex_version("<", IPEX_MINIMUM_VERSION)
+            and "generation" in self.task
+        ):
+            raise ImportError(
+                f"Found an incompatible version of intel-extension-for-pytorch. Found version {_ipex_version}, "
+                f"but only version {IPEX_MINIMUM_VERSION} or higher is supported."
+            )
+
         if isinstance(self._original_model.config, PretrainedConfig):
             self._original_model.config.backend = quantization_config.backend
 
         compressed_model = fit(
             self._original_model,
             conf=quantization_config,
             calib_dataloader=calibration_dataloader,
@@ -202,15 +224,14 @@
             self._original_model.config.torch_dtype = "int8"
             self._original_model.config.save_pretrained(save_directory)
             self._original_model.config.torch_dtype = original_dtype
 
         self._quantized_model = compressed_model._model
 
         if save_onnx_model:
-            self._set_task()
             model_type = self._original_model.config.model_type.replace("_", "-")
             model_name = getattr(self._original_model, "name", None)
             onnx_config_class = TasksManager.get_exporter_config_constructor(
                 exporter="onnx",
                 model=self._original_model,
                 task=self.task,
                 model_type=model_type,
@@ -242,37 +263,40 @@
 
     def _onnx_export(
         self,
         model: PyTorchModel,
         config: OnnxConfig,
         output_path: Union[str, Path],
     ):
-        opset = min(config.DEFAULT_ONNX_OPSET, MIN_QDQ_ONNX_OPSET)
+        opset = max(config.DEFAULT_ONNX_OPSET, MIN_QDQ_ONNX_OPSET)
         dynamic_axes = dict(chain(config.inputs.items(), config.outputs.items()))
         inputs = config.generate_dummy_inputs(framework="pt")
         device = model.model.device
         inputs = {k: v.to(device) for k, v in inputs.items()}
+
         torch_to_int8_onnx(
-            fp32_model=self._original_model.to(device),
-            int8_model=model.model,
+            model.model,
             q_config=model.q_config,
             save_path=str(output_path),
             example_inputs=inputs,
             opset_version=opset,
             dynamic_axes=dynamic_axes,
             input_names=list(config.inputs.keys()),
             output_names=list(config.outputs.keys()),
         )
 
     def _set_task(self):
         if self.task is None:
-            self.task = HfApi().model_info(self._original_model.config._name_or_path).pipeline_tag
-            if self.task is None:
-                raise ValueError(
-                    "The task defining the model topology could not be extracted and needs to be specified for the ONNX export."
+            try:
+                self.task = TasksManager.infer_task_from_model(self._original_model.config._name_or_path)
+            except Exception as e:
+                self.task = "default"
+                logger.warning(
+                    f"The task could not be automatically inferred and will be set to {self.task}. "
+                    f"Please provide the task argument with the relevant task from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
                 )
 
         self.task = _TASK_ALIASES.get(self.task, self.task)
 
         if self.task == "text2text-generation":
             raise ValueError("Seq2Seq models are currently not supported for post-training static quantization.")
```

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,14 +592,19 @@
         # Save the model
         if state_dict is None:
             state_dict = self.model.state_dict()
             if self._compression_manager is not None and hasattr(self._compression_manager.model, "q_config"):
                 state_dict["best_configure"] = self._compression_manager.model.q_config
         torch.save(state_dict, output_model_file)
 
+        # Disable ONNX export for quantized model as deprecated in neural-compressor>=2.2.0
+        if save_onnx_model and self.dtype == "int8":
+            logger.warning("ONNX export for quantized model is no longer supported by neural-compressor>=2.2.0. ")
+            save_onnx_model = False
+
         # Export the compressed model to the ONNX format
         if save_onnx_model:
             self._set_task()
             model_type = self.model.config.model_type.replace("_", "-")
             model_name = getattr(self.model, "name", None)
             onnx_config_class = TasksManager.get_exporter_config_constructor(
                 exporter="onnx", model=self.model, task=self.task, model_type=model_type, model_name=model_name
@@ -633,27 +638,26 @@
         dynamic_axes = dict(chain(config.inputs.items(), config.outputs.items()))
         inputs = config.generate_dummy_inputs(framework="pt")
         device = model.device
         inputs = {k: v.to(device) for k, v in inputs.items()}
 
         if self.dtype == "int8":
             torch_to_int8_onnx(
-                fp32_model=self._compression_manager.model.fp32_model.to(device),
-                int8_model=model,
+                model,
                 q_config=self._compression_manager.model.q_config,
                 save_path=output_path,
                 example_inputs=inputs,
                 opset_version=opset,
                 dynamic_axes=dynamic_axes,
                 input_names=list(config.inputs.keys()),
                 output_names=list(config.outputs.keys()),
             )
         else:
             torch_to_fp32_onnx(
-                fp32_model=model,
+                model,
                 save_path=output_path,
                 example_inputs=inputs,
                 opset_version=opset,
                 dynamic_axes=dynamic_axes,
                 input_names=list(config.inputs.keys()),
                 output_names=list(config.outputs.keys()),
                 do_constant_folding=True,
```

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer_seq2seq.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/neural_compressor/utils.py` & `optimum-intel-1.9.2/optimum/intel/neural_compressor/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/__init__.py` & `optimum-intel-1.9.2/optimum/intel/openvino/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/configuration.py` & `optimum-intel-1.9.2/optimum/intel/openvino/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/modeling.py` & `optimum-intel-1.9.2/optimum/intel/openvino/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/modeling_base.py` & `optimum-intel-1.9.2/optimum/intel/openvino/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/modeling_base_seq2seq.py` & `optimum-intel-1.9.2/optimum/intel/openvino/modeling_base_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/modeling_decoder.py` & `optimum-intel-1.9.2/optimum/intel/openvino/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/modeling_diffusion.py` & `optimum-intel-1.9.2/optimum/intel/openvino/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/modeling_seq2seq.py` & `optimum-intel-1.9.2/optimum/intel/openvino/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/quantization.py` & `optimum-intel-1.9.2/optimum/intel/openvino/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/trainer.py` & `optimum-intel-1.9.2/optimum/intel/openvino/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/training_args.py` & `optimum-intel-1.9.2/optimum/intel/openvino/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/openvino/utils.py` & `optimum-intel-1.9.2/optimum/intel/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/__init__.py` & `optimum-intel-1.9.2/optimum/intel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/constant.py` & `optimum-intel-1.9.2/optimum/intel/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/dummy_ipex_objects.py` & `optimum-intel-1.9.2/optimum/intel/utils/dummy_ipex_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py` & `optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_objects.py` & `optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py` & `optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py` & `optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_nncf_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_objects.py` & `optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/import_utils.py` & `optimum-intel-1.9.2/optimum/intel/utils/import_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,23 @@
     Compare the current torch version to a given reference with an operation.
     """
     if not _torch_available:
         return False
     return compare_versions(parse(_torch_version), operation, version)
 
 
+def is_ipex_version(operation: str, version: str):
+    """
+    Compare the current ipex version to a given reference with an operation.
+    """
+    if not _ipex_available:
+        return False
+    return compare_versions(parse(_ipex_version), operation, version)
+
+
 DIFFUSERS_IMPORT_ERROR = """
 {0} requires the diffusers library but it was not found in your environment. You can install it with pip:
 `pip install diffusers`. Please note that you may need to restart your runtime after installation.
 """
 
 IPEX_IMPORT_ERROR = """
 {0} requires the ipex library but it was not found in your environment. You can install it with pip:
```

### Comparing `optimum-intel-1.9.1/optimum/intel/utils/modeling_utils.py` & `optimum-intel-1.9.2/optimum/intel/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/optimum/intel/version.py` & `optimum-intel-1.9.2/optimum/intel/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.9.1"
+__version__ = "1.9.2"
```

### Comparing `optimum-intel-1.9.1/optimum_intel.egg-info/PKG-INFO` & `optimum-intel-1.9.2/optimum_intel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.1
+Version: 1.9.2
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.1/optimum_intel.egg-info/SOURCES.txt` & `optimum-intel-1.9.2/optimum_intel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/pyproject.toml` & `optimum-intel-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/setup.cfg` & `optimum-intel-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.1/setup.py` & `optimum-intel-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "torchaudio",
     "rjieba",
 ]
 
 QUALITY_REQUIRE = ["black~=23.1", "ruff>=0.0.241"]
 
 EXTRAS_REQUIRE = {
-    "neural-compressor": ["neural-compressor>=2.1.1", "onnx", "onnxruntime<1.15.0"],
+    "neural-compressor": ["neural-compressor>=2.2.0", "onnx", "onnxruntime<1.15.0"],
     "openvino": ["openvino>=2023.0.0", "onnx", "onnxruntime"],
     "nncf": ["nncf>=2.5.0", "openvino-dev>=2023.0.0"],
     "ipex": ["intel-extension-for-pytorch", "onnx"],
     "diffusers": ["diffusers"],
     "quality": QUALITY_REQUIRE,
     "tests": TESTS_REQUIRE,
 }
```

