# Comparing `tmp/offlinerllib-0.0.7.tar.gz` & `tmp/offlinerllib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinerllib-0.0.7.tar", last modified: Wed May 17 07:14:54 2023, max compression
+gzip compressed data, was "offlinerllib-0.0.8.tar", last modified: Tue Jun 27 12:35:35 2023, max compression
```

## Comparing `offlinerllib-0.0.7.tar` & `offlinerllib-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.025917 offlinerllib-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-17 07:14:54.025917 offlinerllib-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.017917 offlinerllib-0.0.7/offlinerllib/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/buffer/d4rl_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/env/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/env/d4rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/env/mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32225 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/module/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/net/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/policy/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/policy/model_free/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/awac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/edac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/inac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/iql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/sacn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/td3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/td3bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/xql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/xsac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:14:54.025917 offlinerllib-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.514042 offlinerllib-0.0.8/offlinerllib/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/d4rl_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/lap_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/env/d4rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/env/mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32225 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/module/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/net/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/td7_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/policy/model_free/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/awac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/edac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/inac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/iql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/sacn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/td3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/td3bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/td7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/xql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/xsac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/setup.py
```

### Comparing `offlinerllib-0.0.7/LICENSE` & `offlinerllib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/PKG-INFO` & `offlinerllib-0.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OfflineRL-Lib
-> 🚧 This repo is not ready for release, benchmarking is ongoing. 🚧
-
+<!-- > 🚧 This repo is not ready for release, benchmarking is ongoing. 🚧 -->
 OfflineRL-Lib provides unofficial and benchmarked PyTorch implementations for selected OfflineRL algorithms, including: 
 - [In-Sample Actor Critic (InAC)](https://arxiv.org/abs/2302.14372)
 - [Extreme Q-Learning (XQL)](https://arxiv.org/abs/2301.02328)
 - [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169)
 - [Decision Transformer (DT)](https://arxiv.org/abs/2106.01345)
 - [Advantage-Weighted Actor Critic (AWAC)](https://arxiv.org/abs/2006.09359)
 - [TD3-BC](https://arxiv.org/pdf/2106.06860.pdf)
+- [TD7](https://arxiv.org/abs/2306.02451)
 
-still benchmarking ... 
-- [EDAC](https://arxiv.org/abs/2110.01548)
-- [SAC-N](https://arxiv.org/abs/2110.01548)
-
-under developing (model based algorithms) ...
-- [MOPO](https://arxiv.org/abs/2005.13239)
-- [MAPLE](https://proceedings.neurips.cc/paper/2021/file/470e7a4f017a5476afb7eeb3f8b96f9b-Paper.pdf)
-- [RAMBO](https://arxiv.org/abs/2204.12581)
+For Model-Based algorithms, please check [OfflineRL-Kit](https://github.com/yihaosun1124/OfflineRL-Kit)!
 
 
 ## Benchmark Results
-See [reproduce/benchmark_result.md](https://github.com/typoverflow/OfflineRL-Lib/blob/master/reproduce/benchmark_result.md) for details. 
+<!-- See [reproduce/benchmark_result.md](https://github.com/typoverflow/OfflineRL-Lib/blob/master/reproduce/benchmark_result.md) for details.  -->
+
++ We benchmark and visualize the result via WandB. Click the following WandB links, and group the runs via the entry `task` (for offline experiments) or `env` (for online experiments). 
++ Available Runs
+  + Offline: 
+    + TD7 [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD7-D4RL)
+    + XQL [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/XQL-D4RL)
+    + InAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/InAC-D4RL)
+    + AWAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/AWAC-D4RL)
+    + IQL [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/IQL-D4RL)
+    + TD3BC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD3BC-Offline)
+    + Decision Transformer [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/DecisionTransformer-Offline)
+  + Online Runs
+    + SAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/SAC-Online)
+    + TD3 [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD3-Online)
+    + TD7 [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD7-Online)
+    + XSAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/XSAC-Online)
 
 ## Citing OfflineRL-Lib
 If you use OfflineRL-Lib in your work, please use the following bibtex
 ```tex
 @misc{offinerllib,
   author = {Chenxiao Gao},
   title = {OfflineRL-Lib: Benchmarked Implementations of Offline RL Algorithms},
```

### Comparing `offlinerllib-0.0.7/offlinerllib/buffer/d4rl_buffer.py` & `offlinerllib-0.0.8/offlinerllib/buffer/d4rl_buffer.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/env/__init__.py` & `offlinerllib-0.0.8/offlinerllib/env/__init__.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/env/d4rl.py` & `offlinerllib-0.0.8/offlinerllib/env/d4rl.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/env/mixed.py` & `offlinerllib-0.0.8/offlinerllib/env/mixed.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/module/actor.py` & `offlinerllib-0.0.8/offlinerllib/module/actor.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/module/critic.py` & `offlinerllib-0.0.8/offlinerllib/module/critic.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/module/net/basic.py` & `offlinerllib-0.0.8/offlinerllib/module/net/basic.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/module/net/mlp.py` & `offlinerllib-0.0.8/offlinerllib/module/net/mlp.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/awac.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/awac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/dt.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/dt.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/edac.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/edac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/inac.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/inac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/iql.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/iql.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/sac.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/sac.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def select_action(
         self,
         obs: np.ndarray,
         deterministic: bool = False
     ) -> np.ndarray:
         obs = torch.from_numpy(obs).float().unsqueeze(0).to(self.device)
         action, _, _ = self.actor.sample(obs, deterministic)
-        return action.squeeze().cpu().numpy()
+        return action.squeeze(0).cpu().numpy()
 
     def _actor_loss(
         self,
         batch: Dict[str, torch.Tensor]
     ) -> Tuple[torch.Tensor, Dict[str, float]]:
         obss, actions, next_obss, rewards, terminals = \
             itemgetter("observations", "actions", "next_observations", "rewards","terminals")(batch)
```

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/sacn.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/sacn.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/td3.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/td3.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     @torch.no_grad()
     def select_action(
         self, 
         obs: np.ndarray, 
         deterministic: bool=False
     ) -> np.ndarray:
         obs = torch.from_numpy(obs).float().unsqueeze(0).to(self.device)
-        action, *_ = self.actor.sample(obs, deterministic)
+        action = self.actor.sample(obs, deterministic)[0].squeeze(0).cpu().numpy()
         if not deterministic and self._exploration_noise is not None:
             action = np.clip(action + self._exploration_noise(action.shape), -self._max_action, self._max_action)
-        return action.squeeze().cpu().numpy()
+        return action
     
     def critic_loss(self, batch: Dict[str, Any]) -> Tuple[torch.Tensor, Dict[str, Any]]:
         obss, actions, next_obss, rewards, terminals = \
             itemgetter("observations", "actions", "next_observations", "rewards", "terminals")(batch)
         q_both = self.critic(obss, actions)
         with torch.no_grad():
             noise = (torch.randn_like(actions) * self._policy_noise).clamp(-self._noise_clip, self._noise_clip)
```

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/td3bc.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/td3bc.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/xql.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/xql.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.7/offlinerllib/policy/model_free/xsac.py` & `offlinerllib-0.0.8/offlinerllib/policy/model_free/xsac.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def select_action(
         self,
         obs: np.ndarray,
         deterministic: bool = False
     ) -> np.ndarray:
         obs = torch.from_numpy(obs).float().unsqueeze(0).to(self.device)
         action, _, _ = self.actor.sample(obs, deterministic)
-        return action.squeeze().cpu().numpy()
+        return action.squeeze(0).cpu().numpy()
     
     def _critic_q_loss(self, obss, actions, next_obss, rewards, terminals) -> Tuple[torch.Tensor, Dict[str, float]]:
         with torch.no_grad():
             q_target = self.critic_v_target(next_obss)
             q_target = rewards + self._discount * (1-terminals) * q_target
         q_pred = self.critic_q(obss, actions)
         q_loss = (q_pred - q_target).pow(2).sum(0).mean()
```

### Comparing `offlinerllib-0.0.7/offlinerllib.egg-info/PKG-INFO` & `offlinerllib-0.0.8/offlinerllib.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OfflineRL-Lib
-> 🚧 This repo is not ready for release, benchmarking is ongoing. 🚧
-
+<!-- > 🚧 This repo is not ready for release, benchmarking is ongoing. 🚧 -->
 OfflineRL-Lib provides unofficial and benchmarked PyTorch implementations for selected OfflineRL algorithms, including: 
 - [In-Sample Actor Critic (InAC)](https://arxiv.org/abs/2302.14372)
 - [Extreme Q-Learning (XQL)](https://arxiv.org/abs/2301.02328)
 - [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169)
 - [Decision Transformer (DT)](https://arxiv.org/abs/2106.01345)
 - [Advantage-Weighted Actor Critic (AWAC)](https://arxiv.org/abs/2006.09359)
 - [TD3-BC](https://arxiv.org/pdf/2106.06860.pdf)
+- [TD7](https://arxiv.org/abs/2306.02451)
 
-still benchmarking ... 
-- [EDAC](https://arxiv.org/abs/2110.01548)
-- [SAC-N](https://arxiv.org/abs/2110.01548)
-
-under developing (model based algorithms) ...
-- [MOPO](https://arxiv.org/abs/2005.13239)
-- [MAPLE](https://proceedings.neurips.cc/paper/2021/file/470e7a4f017a5476afb7eeb3f8b96f9b-Paper.pdf)
-- [RAMBO](https://arxiv.org/abs/2204.12581)
+For Model-Based algorithms, please check [OfflineRL-Kit](https://github.com/yihaosun1124/OfflineRL-Kit)!
 
 
 ## Benchmark Results
-See [reproduce/benchmark_result.md](https://github.com/typoverflow/OfflineRL-Lib/blob/master/reproduce/benchmark_result.md) for details. 
+<!-- See [reproduce/benchmark_result.md](https://github.com/typoverflow/OfflineRL-Lib/blob/master/reproduce/benchmark_result.md) for details.  -->
+
++ We benchmark and visualize the result via WandB. Click the following WandB links, and group the runs via the entry `task` (for offline experiments) or `env` (for online experiments). 
++ Available Runs
+  + Offline: 
+    + TD7 [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD7-D4RL)
+    + XQL [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/XQL-D4RL)
+    + InAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/InAC-D4RL)
+    + AWAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/AWAC-D4RL)
+    + IQL [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/IQL-D4RL)
+    + TD3BC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD3BC-Offline)
+    + Decision Transformer [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/DecisionTransformer-Offline)
+  + Online Runs
+    + SAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/SAC-Online)
+    + TD3 [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD3-Online)
+    + TD7 [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/TD7-Online)
+    + XSAC [:chart_with_upwards_trend:](https://wandb.ai/lamda-rl/XSAC-Online)
 
 ## Citing OfflineRL-Lib
 If you use OfflineRL-Lib in your work, please use the following bibtex
 ```tex
 @misc{offinerllib,
   author = {Chenxiao Gao},
   title = {OfflineRL-Lib: Benchmarked Implementations of Offline RL Algorithms},
```

### Comparing `offlinerllib-0.0.7/offlinerllib.egg-info/SOURCES.txt` & `offlinerllib-0.0.8/offlinerllib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 offlinerllib.egg-info/SOURCES.txt
 offlinerllib.egg-info/dependency_links.txt
 offlinerllib.egg-info/requires.txt
 offlinerllib.egg-info/top_level.txt
 offlinerllib/buffer/__init__.py
 offlinerllib/buffer/base.py
 offlinerllib/buffer/d4rl_buffer.py
+offlinerllib/buffer/lap_buffer.py
 offlinerllib/env/__init__.py
 offlinerllib/env/d4rl.py
 offlinerllib/env/mixed.py
 offlinerllib/module/__init__.py
 offlinerllib/module/actor.py
 offlinerllib/module/critic.py
+offlinerllib/module/td7_net.py
 offlinerllib/module/net/__init__.py
 offlinerllib/module/net/basic.py
 offlinerllib/module/net/mlp.py
 offlinerllib/policy/__init__.py
 offlinerllib/policy/base.py
 offlinerllib/policy/model_free/__init__.py
 offlinerllib/policy/model_free/awac.py
@@ -27,9 +29,10 @@
 offlinerllib/policy/model_free/edac.py
 offlinerllib/policy/model_free/inac.py
 offlinerllib/policy/model_free/iql.py
 offlinerllib/policy/model_free/sac.py
 offlinerllib/policy/model_free/sacn.py
 offlinerllib/policy/model_free/td3.py
 offlinerllib/policy/model_free/td3bc.py
+offlinerllib/policy/model_free/td7.py
 offlinerllib/policy/model_free/xql.py
 offlinerllib/policy/model_free/xsac.py
```

### Comparing `offlinerllib-0.0.7/setup.py` & `offlinerllib-0.0.8/setup.py`

 * *Files identical despite different names*

