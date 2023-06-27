# Comparing `tmp/intercode-bench-0.1.6.tar.gz` & `tmp/intercode-bench-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intercode-bench-0.1.6.tar", last modified: Mon Jun 26 14:46:45 2023, max compression
+gzip compressed data, was "intercode-bench-0.1.7.tar", last modified: Tue Jun 27 20:37:28 2023, max compression
```

## Comparing `intercode-bench-0.1.6.tar` & `intercode-bench-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.592644 intercode-bench-0.1.6/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.6/LICENSE
--rw-r--r--   0 johnbyang   (502) staff       (20)     3071 2023-06-26 14:46:45.592834 intercode-bench-0.1.6/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)     2073 2023-06-26 14:45:26.000000 intercode-bench-0.1.6/README.md
--rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.6/pyproject.toml
--rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-26 14:46:45.593695 intercode-bench-0.1.6/setup.cfg
--rw-r--r--   0 johnbyang   (502) staff       (20)     1451 2023-06-23 21:38:26.000000 intercode-bench-0.1.6/setup.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.573613 intercode-bench-0.1.6/src/
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.577816 intercode-bench-0.1.6/src/intercode/
--rw-r--r--   0 johnbyang   (502) staff       (20)      137 2023-06-26 14:44:17.000000 intercode-bench-0.1.6/src/intercode/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.579116 intercode-bench-0.1.6/src/intercode/envs/
--rw-r--r--   0 johnbyang   (502) staff       (20)      141 2023-06-23 21:20:36.000000 intercode-bench-0.1.6/src/intercode/envs/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.580330 intercode-bench-0.1.6/src/intercode/envs/bash/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.6/src/intercode/envs/bash/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/src/intercode/envs/bash/bash_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.581606 intercode-bench-0.1.6/src/intercode/envs/game/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.6/src/intercode/envs/game/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/src/intercode/envs/game/ctf_env.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/src/intercode/envs/ic_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.582961 intercode-bench-0.1.6/src/intercode/envs/sql/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.6/src/intercode/envs/sql/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.6/src/intercode/envs/sql/sql_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.585237 intercode-bench-0.1.6/src/intercode/utils/
--rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.6/src/intercode/utils/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.6/src/intercode/utils/data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.6/src/intercode/utils/utils.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.588972 intercode-bench-0.1.6/src/intercode_bench.egg-info/
--rw-r--r--   0 johnbyang   (502) staff       (20)     3071 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       72 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/top_level.txt
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.592106 intercode-bench-0.1.6/tests/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_env_bash.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_env_ic.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_env_sql.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.746348 intercode-bench-0.1.7/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.7/LICENSE
+-rw-r--r--   0 johnbyang   (502) staff       (20)     3126 2023-06-27 20:37:28.746549 intercode-bench-0.1.7/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2128 2023-06-27 20:37:05.000000 intercode-bench-0.1.7/README.md
+-rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.7/pyproject.toml
+-rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-27 20:37:28.747341 intercode-bench-0.1.7/setup.cfg
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1451 2023-06-23 21:38:26.000000 intercode-bench-0.1.7/setup.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.727046 intercode-bench-0.1.7/src/
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.732834 intercode-bench-0.1.7/src/intercode/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      137 2023-06-27 20:37:14.000000 intercode-bench-0.1.7/src/intercode/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.733984 intercode-bench-0.1.7/src/intercode/envs/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      141 2023-06-23 21:20:36.000000 intercode-bench-0.1.7/src/intercode/envs/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.735227 intercode-bench-0.1.7/src/intercode/envs/bash/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.7/src/intercode/envs/bash/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.7/src/intercode/envs/bash/bash_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.736229 intercode-bench-0.1.7/src/intercode/envs/game/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.7/src/intercode/envs/game/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.7/src/intercode/envs/game/ctf_env.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.7/src/intercode/envs/ic_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.737244 intercode-bench-0.1.7/src/intercode/envs/sql/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.7/src/intercode/envs/sql/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.7/src/intercode/envs/sql/sql_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.739882 intercode-bench-0.1.7/src/intercode/utils/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.7/src/intercode/utils/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.7/src/intercode/utils/data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.7/src/intercode/utils/utils.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.743141 intercode-bench-0.1.7/src/intercode_bench.egg-info/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     3126 2023-06-27 20:37:28.000000 intercode-bench-0.1.7/src/intercode_bench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-27 20:37:28.000000 intercode-bench-0.1.7/src/intercode_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-27 20:37:28.000000 intercode-bench-0.1.7/src/intercode_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       72 2023-06-27 20:37:28.000000 intercode-bench-0.1.7/src/intercode_bench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-27 20:37:28.000000 intercode-bench-0.1.7/src/intercode_bench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-27 20:37:28.745921 intercode-bench-0.1.7/tests/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.7/tests/test_data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.7/tests/test_env_bash.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.7/tests/test_env_ic.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.7/tests/test_env_sql.py
```

### Comparing `intercode-bench-0.1.6/LICENSE` & `intercode-bench-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/PKG-INFO` & `intercode-bench-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.6
+Version: 0.1.7
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
@@ -33,32 +33,31 @@
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
 </p>
 
 ## 👋 Overview
 InterCode is a **lightweight, flexible, and easy-to-use framework** for designing interactive code environments. Following the popular [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it easy to quickly define a code environment and deploy an agent to operate in code within the context of the environment.
 
-For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](TO DO) and the original paper:
+For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](https://github.com/princeton-nlp/intercode/wiki), [website](https://intercode-benchmark.github.io/) and the original paper:
 
-**[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://intercode-benchmark.github.io/)**  
+**[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://arxiv.org/abs/2306.14898)**  
 
 ## 🛠️ Installation
 > **Note**
 > InterCode requires `python` >= 3.8 a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
 
 ```
 pip install intercode-bench
 ```
 
 ## 🚀 Quick Start
-* Clone the [InterCode repository](https://github.com/intercode-benchmark/intercode-benchmark)
+* Clone the [InterCode repository](https://github.com/princeton-nlp/intercode)
 * Run `./setup.sh`
 * Run `python run_sql.py` 
 
-If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands
-to interact with the task setting.
+If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands to interact with the task setting.
 
 ## 🔎 Learn More
-To learn more about the InterCode framework, please check out the [website](https://intercode-benchmark.github.io/) and GitHub [repository](https://github.com/intercode-benchmark/intercode-benchmark)
+To learn more about the InterCode framework, please check out the [website](https://intercode-benchmark.github.io/) and GitHub [repository](https://github.com/princeton-nlp/intercode)
 
 ## 🪪 License
 Check `LICENSE.md`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.6 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.7 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
@@ -16,21 +16,22 @@
 [https://badge.fury.io/py/intercode-bench.svg] [Build] [License]
 ## ð Overview InterCode is a **lightweight, flexible, and easy-to-use
 framework** for designing interactive code environments. Following the popular
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
-InterCode environments, please check out our [wiki](TO DO) and the original
-paper: **[InterCode: Standardizing and Benchmarking Interactive Coding with
-Execution Feedback](https://intercode-benchmark.github.io/)** ## ð ï¸
-Installation > **Note** > InterCode requires `python` >= 3.8 a local `docker`
-installation to run. Learn more [here](https://docs.docker.com/get-docker/) to
-install. ``` pip install intercode-bench ``` ## ð Quick Start * Clone the
-[InterCode repository](https://github.com/intercode-benchmark/intercode-
-benchmark) * Run `./setup.sh` * Run `python run_sql.py` If InterCode was
-installed successfully, the InterCode SQL environment should be started
-successfully and a CLI interpreter should appear, allowing you to enter `SQL`
-commands to interact with the task setting. ## ð Learn More To learn more
-about the InterCode framework, please check out the [website](https://
-intercode-benchmark.github.io/) and GitHub [repository](https://github.com/
-intercode-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
+InterCode environments, please check out our [wiki](https://github.com/
+princeton-nlp/intercode/wiki), [website](https://intercode-benchmark.github.io/
+) and the original paper: **[InterCode: Standardizing and Benchmarking
+Interactive Coding with Execution Feedback](https://arxiv.org/abs/2306.14898)**
+## ð ï¸ Installation > **Note** > InterCode requires `python` >= 3.8 a local
+`docker` installation to run. Learn more [here](https://docs.docker.com/get-
+docker/) to install. ``` pip install intercode-bench ``` ## ð Quick Start *
+Clone the [InterCode repository](https://github.com/princeton-nlp/intercode) *
+Run `./setup.sh` * Run `python run_sql.py` If InterCode was installed
+successfully, the InterCode SQL environment should be started successfully and
+a CLI interpreter should appear, allowing you to enter `SQL` commands to
+interact with the task setting. ## ð Learn More To learn more about the
+InterCode framework, please check out the [website](https://intercode-
+benchmark.github.io/) and GitHub [repository](https://github.com/princeton-nlp/
+intercode) ## ðªª License Check `LICENSE.md`
```

### Comparing `intercode-bench-0.1.6/README.md` & `intercode-bench-0.1.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,32 +12,31 @@
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
 </p>
 
 ## 👋 Overview
 InterCode is a **lightweight, flexible, and easy-to-use framework** for designing interactive code environments. Following the popular [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it easy to quickly define a code environment and deploy an agent to operate in code within the context of the environment.
 
-For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](TO DO) and the original paper:
+For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](https://github.com/princeton-nlp/intercode/wiki), [website](https://intercode-benchmark.github.io/) and the original paper:
 
-**[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://intercode-benchmark.github.io/)**  
+**[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://arxiv.org/abs/2306.14898)**  
 
 ## 🛠️ Installation
 > **Note**
 > InterCode requires `python` >= 3.8 a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
 
 ```
 pip install intercode-bench
 ```
 
 ## 🚀 Quick Start
-* Clone the [InterCode repository](https://github.com/intercode-benchmark/intercode-benchmark)
+* Clone the [InterCode repository](https://github.com/princeton-nlp/intercode)
 * Run `./setup.sh`
 * Run `python run_sql.py` 
 
-If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands
-to interact with the task setting.
+If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands to interact with the task setting.
 
 ## 🔎 Learn More
-To learn more about the InterCode framework, please check out the [website](https://intercode-benchmark.github.io/) and GitHub [repository](https://github.com/intercode-benchmark/intercode-benchmark)
+To learn more about the InterCode framework, please check out the [website](https://intercode-benchmark.github.io/) and GitHub [repository](https://github.com/princeton-nlp/intercode)
 
 ## 🪪 License
 Check `LICENSE.md`
```

#### html2text {}

```diff
@@ -3,21 +3,22 @@
 [https://badge.fury.io/py/intercode-bench.svg] [Build] [License]
 ## ð Overview InterCode is a **lightweight, flexible, and easy-to-use
 framework** for designing interactive code environments. Following the popular
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
-InterCode environments, please check out our [wiki](TO DO) and the original
-paper: **[InterCode: Standardizing and Benchmarking Interactive Coding with
-Execution Feedback](https://intercode-benchmark.github.io/)** ## ð ï¸
-Installation > **Note** > InterCode requires `python` >= 3.8 a local `docker`
-installation to run. Learn more [here](https://docs.docker.com/get-docker/) to
-install. ``` pip install intercode-bench ``` ## ð Quick Start * Clone the
-[InterCode repository](https://github.com/intercode-benchmark/intercode-
-benchmark) * Run `./setup.sh` * Run `python run_sql.py` If InterCode was
-installed successfully, the InterCode SQL environment should be started
-successfully and a CLI interpreter should appear, allowing you to enter `SQL`
-commands to interact with the task setting. ## ð Learn More To learn more
-about the InterCode framework, please check out the [website](https://
-intercode-benchmark.github.io/) and GitHub [repository](https://github.com/
-intercode-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
+InterCode environments, please check out our [wiki](https://github.com/
+princeton-nlp/intercode/wiki), [website](https://intercode-benchmark.github.io/
+) and the original paper: **[InterCode: Standardizing and Benchmarking
+Interactive Coding with Execution Feedback](https://arxiv.org/abs/2306.14898)**
+## ð ï¸ Installation > **Note** > InterCode requires `python` >= 3.8 a local
+`docker` installation to run. Learn more [here](https://docs.docker.com/get-
+docker/) to install. ``` pip install intercode-bench ``` ## ð Quick Start *
+Clone the [InterCode repository](https://github.com/princeton-nlp/intercode) *
+Run `./setup.sh` * Run `python run_sql.py` If InterCode was installed
+successfully, the InterCode SQL environment should be started successfully and
+a CLI interpreter should appear, allowing you to enter `SQL` commands to
+interact with the task setting. ## ð Learn More To learn more about the
+InterCode framework, please check out the [website](https://intercode-
+benchmark.github.io/) and GitHub [repository](https://github.com/princeton-nlp/
+intercode) ## ðªª License Check `LICENSE.md`
```

### Comparing `intercode-bench-0.1.6/setup.py` & `intercode-bench-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/src/intercode/envs/bash/bash_env.py` & `intercode-bench-0.1.7/src/intercode/envs/bash/bash_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/src/intercode/envs/game/ctf_env.py` & `intercode-bench-0.1.7/src/intercode/envs/game/ctf_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/src/intercode/envs/ic_env.py` & `intercode-bench-0.1.7/src/intercode/envs/ic_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/src/intercode/envs/sql/sql_env.py` & `intercode-bench-0.1.7/src/intercode/envs/sql/sql_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/src/intercode/utils/data_loader.py` & `intercode-bench-0.1.7/src/intercode/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/src/intercode/utils/utils.py` & `intercode-bench-0.1.7/src/intercode/utils/utils.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/src/intercode_bench.egg-info/PKG-INFO` & `intercode-bench-0.1.7/src/intercode_bench.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.6
+Version: 0.1.7
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
@@ -33,32 +33,31 @@
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
 </p>
 
 ## 👋 Overview
 InterCode is a **lightweight, flexible, and easy-to-use framework** for designing interactive code environments. Following the popular [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it easy to quickly define a code environment and deploy an agent to operate in code within the context of the environment.
 
-For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](TO DO) and the original paper:
+For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](https://github.com/princeton-nlp/intercode/wiki), [website](https://intercode-benchmark.github.io/) and the original paper:
 
-**[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://intercode-benchmark.github.io/)**  
+**[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://arxiv.org/abs/2306.14898)**  
 
 ## 🛠️ Installation
 > **Note**
 > InterCode requires `python` >= 3.8 a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
 
 ```
 pip install intercode-bench
 ```
 
 ## 🚀 Quick Start
-* Clone the [InterCode repository](https://github.com/intercode-benchmark/intercode-benchmark)
+* Clone the [InterCode repository](https://github.com/princeton-nlp/intercode)
 * Run `./setup.sh`
 * Run `python run_sql.py` 
 
-If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands
-to interact with the task setting.
+If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands to interact with the task setting.
 
 ## 🔎 Learn More
-To learn more about the InterCode framework, please check out the [website](https://intercode-benchmark.github.io/) and GitHub [repository](https://github.com/intercode-benchmark/intercode-benchmark)
+To learn more about the InterCode framework, please check out the [website](https://intercode-benchmark.github.io/) and GitHub [repository](https://github.com/princeton-nlp/intercode)
 
 ## 🪪 License
 Check `LICENSE.md`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.6 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.7 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
@@ -16,21 +16,22 @@
 [https://badge.fury.io/py/intercode-bench.svg] [Build] [License]
 ## ð Overview InterCode is a **lightweight, flexible, and easy-to-use
 framework** for designing interactive code environments. Following the popular
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
-InterCode environments, please check out our [wiki](TO DO) and the original
-paper: **[InterCode: Standardizing and Benchmarking Interactive Coding with
-Execution Feedback](https://intercode-benchmark.github.io/)** ## ð ï¸
-Installation > **Note** > InterCode requires `python` >= 3.8 a local `docker`
-installation to run. Learn more [here](https://docs.docker.com/get-docker/) to
-install. ``` pip install intercode-bench ``` ## ð Quick Start * Clone the
-[InterCode repository](https://github.com/intercode-benchmark/intercode-
-benchmark) * Run `./setup.sh` * Run `python run_sql.py` If InterCode was
-installed successfully, the InterCode SQL environment should be started
-successfully and a CLI interpreter should appear, allowing you to enter `SQL`
-commands to interact with the task setting. ## ð Learn More To learn more
-about the InterCode framework, please check out the [website](https://
-intercode-benchmark.github.io/) and GitHub [repository](https://github.com/
-intercode-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
+InterCode environments, please check out our [wiki](https://github.com/
+princeton-nlp/intercode/wiki), [website](https://intercode-benchmark.github.io/
+) and the original paper: **[InterCode: Standardizing and Benchmarking
+Interactive Coding with Execution Feedback](https://arxiv.org/abs/2306.14898)**
+## ð ï¸ Installation > **Note** > InterCode requires `python` >= 3.8 a local
+`docker` installation to run. Learn more [here](https://docs.docker.com/get-
+docker/) to install. ``` pip install intercode-bench ``` ## ð Quick Start *
+Clone the [InterCode repository](https://github.com/princeton-nlp/intercode) *
+Run `./setup.sh` * Run `python run_sql.py` If InterCode was installed
+successfully, the InterCode SQL environment should be started successfully and
+a CLI interpreter should appear, allowing you to enter `SQL` commands to
+interact with the task setting. ## ð Learn More To learn more about the
+InterCode framework, please check out the [website](https://intercode-
+benchmark.github.io/) and GitHub [repository](https://github.com/princeton-nlp/
+intercode) ## ðªª License Check `LICENSE.md`
```

### Comparing `intercode-bench-0.1.6/src/intercode_bench.egg-info/SOURCES.txt` & `intercode-bench-0.1.7/src/intercode_bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/tests/test_data_loader.py` & `intercode-bench-0.1.7/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/tests/test_env_bash.py` & `intercode-bench-0.1.7/tests/test_env_bash.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/tests/test_env_ic.py` & `intercode-bench-0.1.7/tests/test_env_ic.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.6/tests/test_env_sql.py` & `intercode-bench-0.1.7/tests/test_env_sql.py`

 * *Files identical despite different names*

