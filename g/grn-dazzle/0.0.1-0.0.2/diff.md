# Comparing `tmp/grn_dazzle-0.0.1.tar.gz` & `tmp/grn_dazzle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grn_dazzle-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "grn_dazzle-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `grn_dazzle-0.0.1.tar` & `grn_dazzle-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2023-06-11 04:44:56.760608 grn_dazzle-0.0.1/LICENSE
--rw-r--r--   0        0        0     1219 2023-06-26 23:59:32.409908 grn_dazzle-0.0.1/README.md
--rw-r--r--   0        0        0      254 2023-06-26 22:10:00.178325 grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     3843 2023-06-26 22:09:04.246444 grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/data-checkpoint.py
--rw-r--r--   0        0        0     4461 2023-05-07 03:27:10.715981 grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/evaluate-checkpoint.py
--rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/logger-checkpoint.py
--rw-r--r--   0        0        0     7007 2023-06-26 22:07:34.526475 grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/models-checkpoint.py
--rw-r--r--   0        0        0    13251 2023-06-26 22:08:41.516436 grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/runner-checkpoint.py
--rw-r--r--   0        0        0      254 2023-06-26 22:10:00.178325 grn_dazzle-0.0.1/grn_dazzle/__init__.py
--rw-r--r--   0        0        0     3843 2023-06-26 22:09:04.246444 grn_dazzle-0.0.1/grn_dazzle/data.py
--rw-r--r--   0        0        0     2942 2023-06-11 00:24:31.884393 grn_dazzle-0.0.1/grn_dazzle/evaluate.py
--rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grn_dazzle-0.0.1/grn_dazzle/logger.py
--rw-r--r--   0        0        0     7007 2023-06-26 22:07:34.526475 grn_dazzle-0.0.1/grn_dazzle/models.py
--rw-r--r--   0        0        0    13251 2023-06-26 22:08:41.516436 grn_dazzle-0.0.1/grn_dazzle/runner.py
--rw-r--r--   0        0        0      745 2023-06-27 00:00:46.577135 grn_dazzle-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 grn_dazzle-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-11 04:44:56.760608 grn_dazzle-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1216 2023-06-27 00:24:41.215346 grn_dazzle-0.0.2/README.md
+-rw-r--r--   0        0        0      254 2023-06-26 22:10:00.178325 grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     3843 2023-06-26 22:09:04.246444 grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/data-checkpoint.py
+-rw-r--r--   0        0        0     4461 2023-05-07 03:27:10.715981 grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/evaluate-checkpoint.py
+-rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/logger-checkpoint.py
+-rw-r--r--   0        0        0     7007 2023-06-26 22:07:34.526475 grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/models-checkpoint.py
+-rw-r--r--   0        0        0    13251 2023-06-26 22:08:41.516436 grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/runner-checkpoint.py
+-rw-r--r--   0        0        0      254 2023-06-26 22:10:00.178325 grn_dazzle-0.0.2/dazzle/__init__.py
+-rw-r--r--   0        0        0     3843 2023-06-26 22:09:04.246444 grn_dazzle-0.0.2/dazzle/data.py
+-rw-r--r--   0        0        0     2942 2023-06-11 00:24:31.884393 grn_dazzle-0.0.2/dazzle/evaluate.py
+-rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grn_dazzle-0.0.2/dazzle/logger.py
+-rw-r--r--   0        0        0     7007 2023-06-26 22:07:34.526475 grn_dazzle-0.0.2/dazzle/models.py
+-rw-r--r--   0        0        0    13251 2023-06-26 22:08:41.516436 grn_dazzle-0.0.2/dazzle/runner.py
+-rw-r--r--   0        0        0      781 2023-06-27 00:24:49.070597 grn_dazzle-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 grn_dazzle-0.0.2/PKG-INFO
```

### Comparing `grn_dazzle-0.0.1/LICENSE` & `grn_dazzle-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/README.md` & `grn_dazzle-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # DAZZLE
 
 This repository include code and documentation for our manuscript "Improving Gene Regulatory Network Inference using Dropout Augmentation". 
 
 ## Install
 
-This package is available on pip
+This package is available on pip 
 
 ```
 pip install grn-dazzle
 ```
 
 ## Basic Usage
 
@@ -18,15 +18,15 @@
 - **Experiment Configs**. We also provide two sets of default configs with this package, namely `DEFAULT_DAZZLE_CONFIGS` and `DEFAULT_DEEPSEM_CONFIGS`. They are just two python dictionaries. If you need to make modifications, just save them to a variable and adjust the values. 
 
 ## Quick Example
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kwRG0dsqJAHxsOXF9zFeyNxpuh_TWSGg?usp=sharing)
 
 ```
-from grn-dazzle import load_beeline, runDAZZLE, get_metrics, DEFAULT_DAZZLE_CONFIGS
+from dazzle import load_beeline, runDAZZLE, get_metrics, DEFAULT_DAZZLE_CONFIGS
 
 
 bl_data, bl_ground_truth = load_beeline(
     data_dir='data', 
     benchmark_data="hESC", 
     benchmark_setting="500_STRING"
 )
```

### Comparing `grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/data-checkpoint.py` & `grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/data-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/evaluate-checkpoint.py` & `grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/evaluate-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/logger-checkpoint.py` & `grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/logger-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/models-checkpoint.py` & `grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/models-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/.ipynb_checkpoints/runner-checkpoint.py` & `grn_dazzle-0.0.2/dazzle/.ipynb_checkpoints/runner-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/data.py` & `grn_dazzle-0.0.2/dazzle/data.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/evaluate.py` & `grn_dazzle-0.0.2/dazzle/evaluate.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/logger.py` & `grn_dazzle-0.0.2/dazzle/logger.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/models.py` & `grn_dazzle-0.0.2/dazzle/models.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/grn_dazzle/runner.py` & `grn_dazzle-0.0.2/dazzle/runner.py`

 * *Files identical despite different names*

### Comparing `grn_dazzle-0.0.1/pyproject.toml` & `grn_dazzle-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,26 @@
     { name = "Donna Slonim", email="donna.slonim@tufts.edu"}
 ]
 maintainers = [
     { name = "Hao Zhu", email = "haozhu233@gmail.com" }
 ]
 license = {file = "LICENSE"}
 description = "Improving single-cell GRN Inference using Dropout Augmentation"
-version = "0.0.1"
+version = "0.0.2"
 requires-python = ">=3.7"
 classifiers = ["License :: OSI Approved :: MIT License"]
 readme = "README.md"
 
 dependencies = [
     "numpy>=1.16.5",
     "pandas>=1.1.1",
     "torch",
     "tqdm",
     "scanpy",
     "scikit-learn"
 ]
 
 [project.urls]
-Home = "https://bcb.cs.tufts.edu/DAZZLE/"
+Home = "https://bcb.cs.tufts.edu/DAZZLE/"
+
+[tool.flit.module]
+name = "dazzle"
```

### Comparing `grn_dazzle-0.0.1/PKG-INFO` & `grn_dazzle-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grn-dazzle
-Version: 0.0.1
+Version: 0.0.2
 Summary: Improving single-cell GRN Inference using Dropout Augmentation
 Author-email: Hao Zhu <haozhu233@gmail.com>, Donna Slonim <donna.slonim@tufts.edu>
 Maintainer-email: Hao Zhu <haozhu233@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy>=1.16.5
@@ -17,15 +17,15 @@
 
 # DAZZLE
 
 This repository include code and documentation for our manuscript "Improving Gene Regulatory Network Inference using Dropout Augmentation". 
 
 ## Install
 
-This package is available on pip
+This package is available on pip 
 
 ```
 pip install grn-dazzle
 ```
 
 ## Basic Usage
 
@@ -35,15 +35,15 @@
 - **Experiment Configs**. We also provide two sets of default configs with this package, namely `DEFAULT_DAZZLE_CONFIGS` and `DEFAULT_DEEPSEM_CONFIGS`. They are just two python dictionaries. If you need to make modifications, just save them to a variable and adjust the values. 
 
 ## Quick Example
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kwRG0dsqJAHxsOXF9zFeyNxpuh_TWSGg?usp=sharing)
 
 ```
-from grn-dazzle import load_beeline, runDAZZLE, get_metrics, DEFAULT_DAZZLE_CONFIGS
+from dazzle import load_beeline, runDAZZLE, get_metrics, DEFAULT_DAZZLE_CONFIGS
 
 
 bl_data, bl_ground_truth = load_beeline(
     data_dir='data', 
     benchmark_data="hESC", 
     benchmark_setting="500_STRING"
 )
```

