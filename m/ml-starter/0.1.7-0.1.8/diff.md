# Comparing `tmp/ml-starter-0.1.7.tar.gz` & `tmp/ml-starter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.7.tar", last modified: Mon Jun 26 06:22:45 2023, max compression
+gzip compressed data, was "ml-starter-0.1.8.tar", last modified: Tue Jun 27 05:21:27 2023, max compression
```

## Comparing `ml-starter-0.1.7.tar` & `ml-starter-0.1.8.tar`

### file list

```diff
@@ -1,167 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.886608 ml-starter-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 06:22:30.000000 ml-starter-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 06:22:30.000000 ml-starter-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 06:22:45.886608 ml-starter-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 06:22:30.000000 ml-starter-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.850607 ml-starter-0.1.7/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.850607 ml-starter-0.1.7/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.854608 ml-starter-0.1.7/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.854608 ml-starter-0.1.7/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.858608 ml-starter-0.1.7/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.858608 ml-starter-0.1.7/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.858608 ml-starter-0.1.7/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.862608 ml-starter-0.1.7/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.862608 ml-starter-0.1.7/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.862608 ml-starter-0.1.7/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.866608 ml-starter-0.1.7/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.866608 ml-starter-0.1.7/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.870608 ml-starter-0.1.7/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.870608 ml-starter-0.1.7/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.870608 ml-starter-0.1.7/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.870608 ml-starter-0.1.7/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.874608 ml-starter-0.1.7/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.882608 ml-starter-0.1.7/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.882608 ml-starter-0.1.7/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.882608 ml-starter-0.1.7/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-26 06:22:30.000000 ml-starter-0.1.7/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:22:45.886608 ml-starter-0.1.7/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 06:22:45.000000 ml-starter-0.1.7/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-26 06:22:45.000000 ml-starter-0.1.7/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:22:45.000000 ml-starter-0.1.7/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 06:22:45.000000 ml-starter-0.1.7/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 06:22:45.000000 ml-starter-0.1.7/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 06:22:30.000000 ml-starter-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 06:22:30.000000 ml-starter-0.1.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 06:22:30.000000 ml-starter-0.1.7/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 06:22:30.000000 ml-starter-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 06:22:45.886608 ml-starter-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-26 06:22:30.000000 ml-starter-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 05:21:15.000000 ml-starter-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 05:21:15.000000 ml-starter-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 05:21:27.611322 ml-starter-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-27 05:21:15.000000 ml-starter-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44768 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.595322 ml-starter-0.1.8/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.599322 ml-starter-0.1.8/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.603322 ml-starter-0.1.8/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.607322 ml-starter-0.1.8/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.607322 ml-starter-0.1.8/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-27 05:21:15.000000 ml-starter-0.1.8/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:21:27.611322 ml-starter-0.1.8/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 05:21:27.000000 ml-starter-0.1.8/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-27 05:21:15.000000 ml-starter-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 05:21:15.000000 ml-starter-0.1.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 05:21:15.000000 ml-starter-0.1.8/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 05:21:15.000000 ml-starter-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 05:21:27.611322 ml-starter-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-27 05:21:15.000000 ml-starter-0.1.8/setup.py
```

### Comparing `ml-starter-0.1.7/LICENSE` & `ml-starter-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/PKG-INFO` & `ml-starter-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.7
+Version: 0.1.8
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.7/README.md` & `ml-starter-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/api.py` & `ml-starter-0.1.8/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
     "LoraConv2d",
     "LoraConvTranspose1d",
     "LoraConvTranspose2d",
     "LoraEmbedding",
     "LoraGRU",
     "LoraLinear",
     "LoraLSTM",
+    "loss_fn",
     "Loss",
     "maybe_lora",
     "meta_to_empty_func",
     "MultiIterDataset",
     "MultiprocessConfig",
     "MultiProcessLauncher",
     "MultiProcessLauncherConfig",
@@ -248,14 +249,15 @@
     AsyncEnvironmentWorker,
     AsyncWorkerPool,
     BaseEnvironmentWorker,
     SyncEnvironmentWorker,
     SyncWorkerPool,
     WorkerPool,
 )
+from ml.tasks.losses.loss import loss_fn
 from ml.tasks.losses.reduce import cast_reduce_type, reduce
 from ml.tasks.rl.base import ReinforcementLearningTask, ReinforcementLearningTaskConfig
 from ml.tasks.sl.base import SupervisedLearningTask, SupervisedLearningTaskConfig
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig
 from ml.trainers.learning import BaseLearningTrainer, BaseLearningTrainerConfig
 from ml.trainers.rl import ReinforcementLearningTrainer, ReinforcementLearningTrainerConfig
 from ml.trainers.sl import SupervisedLearningTrainer, SupervisedLearningTrainerConfig
```

### Comparing `ml-starter-0.1.7/ml/core/common_types.py` & `ml-starter-0.1.8/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/core/config.py` & `ml-starter-0.1.8/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/core/env.py` & `ml-starter-0.1.8/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/core/registry.py` & `ml-starter-0.1.8/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/core/state.py` & `ml-starter-0.1.8/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/launchers/base.py` & `ml-starter-0.1.8/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/launchers/mp.py` & `ml-starter-0.1.8/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/launchers/slurm.py` & `ml-starter-0.1.8/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/launchers/torchrun.py` & `ml-starter-0.1.8/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/loggers/base.py` & `ml-starter-0.1.8/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/loggers/meter.py` & `ml-starter-0.1.8/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/loggers/multi.py` & `ml-starter-0.1.8/ml/loggers/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -948,14 +948,15 @@
             audio = get_audio_channel(audio, channel_select_mode)
 
             def to_frames(ms: float) -> int:
                 return 2 ** round(math.log2(ms * sample_rate / 1000))
 
             n_fft = to_frames(n_fft_ms)
             hop_length = None if hop_length_ms is None else to_frames(hop_length_ms)
+            audio = audio.to(torch.float32)
             audio_spec = torch.stft(audio, n_fft, hop_length=hop_length, normalized=True, return_complex=True)
             audio_spec = torch.log10(torch.abs(audio_spec) + 1e-6)
             return standardize_image(
                 audio_spec,
                 log_key=f"{namespace}/{key}",
                 keep_resolution=keep_resolution,
             )
@@ -1005,14 +1006,15 @@
             audio = get_audio_channel(audio, channel_select_mode)
 
             def to_frames(ms: float) -> int:
                 return 2 ** round(math.log2(ms * sample_rate / 1000))
 
             n_fft = to_frames(n_fft_ms)
             hop_length = None if hop_length_ms is None else to_frames(hop_length_ms)
+            audio = audio.to(torch.float32)
             audio_spec = torch.stft(audio, n_fft, hop_length=hop_length, normalized=True, return_complex=True)
             audio_spec = torch.log10(torch.abs(audio_spec) + 1e-6)
             audio_spec = standardize_images(
                 audio_spec,
                 log_key=f"{namespace}/{key}",
                 keep_resolution=keep_resolution,
             )
```

### Comparing `ml-starter-0.1.7/ml/loggers/stdout.py` & `ml-starter-0.1.8/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/loggers/tensorboard.py` & `ml-starter-0.1.8/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/lr_schedulers/base.py` & `ml-starter-0.1.8/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/lr_schedulers/constant.py` & `ml-starter-0.1.8/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.8/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.8/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/lr_schedulers/linear.py` & `ml-starter-0.1.8/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.8/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.8/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/activations.py` & `ml-starter-0.1.8/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/base.py` & `ml-starter-0.1.8/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/embeddings.py` & `ml-starter-0.1.8/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/init.py` & `ml-starter-0.1.8/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/kmeans.py` & `ml-starter-0.1.8/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/lora.py` & `ml-starter-0.1.8/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/norms.py` & `ml-starter-0.1.8/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/models/parallel.py` & `ml-starter-0.1.8/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/optimizers/adam.py` & `ml-starter-0.1.8/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/optimizers/adamw.py` & `ml-starter-0.1.8/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/optimizers/adan.py` & `ml-starter-0.1.8/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/optimizers/base.py` & `ml-starter-0.1.8/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/optimizers/common.py` & `ml-starter-0.1.8/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/optimizers/lion.py` & `ml-starter-0.1.8/ml/optimizers/lion.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         update = update + weight * weight_deacy
         update = update * lr
         return update, momentum
 """
 
 import logging
 from dataclasses import dataclass
-from typing import Callable
+from typing import Callable, cast
 
 import torch
 from torch import Tensor, nn
 from torch.optim.optimizer import Optimizer
 
 from ml.core.config import conf_field
 from ml.core.registry import register_optimizer
@@ -106,38 +106,41 @@
             "lr": lr,
             "betas": betas,
             "weight_decay": weight_decay,
         }
 
         super().__init__(params, defaults)
 
-        self.update_fn = get_update_fn(use_triton)
+        self.update_fn = get_update_fn(use_triton=False)
+        self.update_fn_cuda = get_update_fn(use_triton=use_triton)
 
     @torch.no_grad()
     def step(self, closure: OptLossClosure = None) -> OptFloat:
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
             for p in group["params"]:
+                p = cast(Tensor, p)
                 if p.grad is None:
                     continue
 
                 grad = p.grad.data
                 lr: float = group["lr"]
                 wd: float = group["weight_decay"]
                 beta1, beta2 = group["betas"]
                 state = self.state[p]
 
                 if len(state) == 0:
                     state["exp_avg"] = torch.zeros_like(p)
 
-                self.update_fn(p, grad, state["exp_avg"], lr, wd, beta1, beta2)
+                update_fn = self.update_fn_cuda if grad.is_cuda else self.update_fn
+                update_fn(p, grad, state["exp_avg"], lr, wd, beta1, beta2)
 
         return loss
 
 
 @dataclass
 class LionOptimizerConfig(BaseOptimizerConfig):
     lr: float = conf_field(1e-4, help="Learning rate.")
```

### Comparing `ml-starter-0.1.7/ml/optimizers/sgd.py` & `ml-starter-0.1.8/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/optimizers/shampoo.py` & `ml-starter-0.1.8/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/scripts/cli.py` & `ml-starter-0.1.8/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/scripts/stage.py` & `ml-starter-0.1.8/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/scripts/train.py` & `ml-starter-0.1.8/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/base.py` & `ml-starter-0.1.8/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.8/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.8/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/collate.py` & `ml-starter-0.1.8/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.8/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.8/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.8/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.8/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.8/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.8/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/environments/base.py` & `ml-starter-0.1.8/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/environments/utils.py` & `ml-starter-0.1.8/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/environments/worker.py` & `ml-starter-0.1.8/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/losses/reduce.py` & `ml-starter-0.1.8/ml/tasks/losses/reduce.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,21 +21,23 @@
 def cast_reduce_type(s: str | None) -> ReduceType:
     args = get_args(ReduceType)
     assert s in args, f"Invalid reduce type: '{s}' Valid options are {args}"
     return cast(ReduceType, s)
 
 
 def reduce(t: Tensor, reduce_type: ReduceType, dim: int | None = None) -> Tensor:
-    if reduce_type is None:
-        return t
-    if reduce_type == "mean":
-        return t.mean(dim)
-    if reduce_type == "sum":
-        return t.sum(dim)
-    raise NotImplementedError(f"Unexpected sample reduction type: {reduce_type}")
+    match reduce_type:
+        case None:
+            return t
+        case "mean":
+            return t.mean(dim)
+        case "sum":
+            return t.sum(dim)
+        case _:
+            raise NotImplementedError(f"Unexpected sample reduction type: {reduce_type}")
 
 
 class SampleReduce(nn.Module):
     def __init__(self, reduce_type: ReduceType) -> None:
         super().__init__()
 
         self.reduce_type = reduce_type
```

### Comparing `ml-starter-0.1.7/ml/tasks/rl/base.py` & `ml-starter-0.1.8/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/rl/replay.py` & `ml-starter-0.1.8/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/tasks/sl/base.py` & `ml-starter-0.1.8/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/base.py` & `ml-starter-0.1.8/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/learning.py` & `ml-starter-0.1.8/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/compile.py` & `ml-starter-0.1.8/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.8/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.8/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.8/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.1.8/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.8/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.8/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.8/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.8/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.8/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/rl.py` & `ml-starter-0.1.8/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/trainers/sl.py` & `ml-starter-0.1.8/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/argparse.py` & `ml-starter-0.1.8/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/atomic.py` & `ml-starter-0.1.8/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/audio.py` & `ml-starter-0.1.8/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/augmentation.py` & `ml-starter-0.1.8/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/caching.py` & `ml-starter-0.1.8/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/checkpoint.py` & `ml-starter-0.1.8/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/cli.py` & `ml-starter-0.1.8/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/colors.py` & `ml-starter-0.1.8/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/data.py` & `ml-starter-0.1.8/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/datetime.py` & `ml-starter-0.1.8/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/device/auto.py` & `ml-starter-0.1.8/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/device/base.py` & `ml-starter-0.1.8/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/device/cpu.py` & `ml-starter-0.1.8/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/device/gpu.py` & `ml-starter-0.1.8/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/device/metal.py` & `ml-starter-0.1.8/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/distributed.py` & `ml-starter-0.1.8/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/image.py` & `ml-starter-0.1.8/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/io.py` & `ml-starter-0.1.8/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/large_models.py` & `ml-starter-0.1.8/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/logging.py` & `ml-starter-0.1.8/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/meter.py` & `ml-starter-0.1.8/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/parallel.py` & `ml-starter-0.1.8/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/staging.py` & `ml-starter-0.1.8/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/testing.py` & `ml-starter-0.1.8/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/timer.py` & `ml-starter-0.1.8/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/tokens.py` & `ml-starter-0.1.8/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/torch_distributed.py` & `ml-starter-0.1.8/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/triton/kmeans.py` & `ml-starter-0.1.8/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/triton/lion.py` & `ml-starter-0.1.8/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml/utils/video.py` & `ml-starter-0.1.8/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.8/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.7
+Version: 0.1.8
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.7/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.8/ml_starter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 ml/lr_schedulers/linear.py
 ml/lr_schedulers/linear_no_decay.py
 ml/lr_schedulers/scripts/__init__.py
 ml/lr_schedulers/scripts/plot.py
 ml/models/__init__.py
 ml/models/activations.py
 ml/models/base.py
+ml/models/codebook.py
 ml/models/embeddings.py
 ml/models/init.py
 ml/models/kmeans.py
 ml/models/lora.py
 ml/models/norms.py
 ml/models/parallel.py
 ml/optimizers/__init__.py
@@ -74,14 +75,17 @@
 ml/tasks/datasets/transforms.py
 ml/tasks/datasets/video_file.py
 ml/tasks/environments/__init__.py
 ml/tasks/environments/base.py
 ml/tasks/environments/utils.py
 ml/tasks/environments/worker.py
 ml/tasks/losses/__init__.py
+ml/tasks/losses/audio.py
+ml/tasks/losses/image.py
+ml/tasks/losses/loss.py
 ml/tasks/losses/reduce.py
 ml/tasks/rl/__init__.py
 ml/tasks/rl/base.py
 ml/tasks/rl/replay.py
 ml/tasks/sl/__init__.py
 ml/tasks/sl/base.py
 ml/trainers/__init__.py
```

### Comparing `ml-starter-0.1.7/pyproject.toml` & `ml-starter-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.7/setup.py` & `ml-starter-0.1.8/setup.py`

 * *Files identical despite different names*

