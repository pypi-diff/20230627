# Comparing `tmp/jammy-0.1.6.tar.gz` & `tmp/jammy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jammy-0.1.6.tar", max compression
+gzip compressed data, was "jammy-0.1.7.tar", max compression
```

## Comparing `jammy-0.1.6.tar` & `jammy-0.1.7.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0     2479 2023-05-30 04:24:29.738662 jammy-0.1.6/README.md
--rw-r--r--   0        0        0     1259 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/__init__.py
--rw-r--r--   0        0        0       70 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli/__init__.py
--rw-r--r--   0        0        0     5682 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli/argument.py
--rw-r--r--   0        0        0     1329 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli/cmd_utils.py
--rw-r--r--   0        0        0     2047 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli/cmdline_viz.py
--rw-r--r--   0        0        0     2403 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli/colors.py
--rw-r--r--   0        0        0     1743 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli/device.py
--rw-r--r--   0        0        0     2754 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli/keyboard.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.793661 jammy-0.1.6/jammy/cli_scripts/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.793661 jammy-0.1.6/jammy/cli_scripts/conf/__init__.py
--rw-r--r--   0        0        0      302 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli_scripts/conf/jamdk.yaml
--rw-r--r--   0        0        0      408 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli_scripts/conf/ngc.yaml
--rw-r--r--   0        0        0     4256 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli_scripts/dk.py
--rw-r--r--   0        0        0     3716 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli_scripts/gpu_sc.py
--rw-r--r--   0        0        0      304 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli_scripts/inspect_file.py
--rw-r--r--   0        0        0     6524 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli_scripts/ngc_debug.py
--rw-r--r--   0        0        0    17767 2023-05-30 04:24:29.742662 jammy-0.1.6/jammy/cli_scripts/shell_executor.py
--rw-r--r--   0        0        0    15458 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/cli_scripts/sys_info.py
--rw-r--r--   0        0        0       31 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/collections/__init__.py
--rw-r--r--   0        0        0      312 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/collections/lazy_dict.py
--rw-r--r--   0        0        0       39 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/comm/__init__.py
--rw-r--r--   0        0        0     6007 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/comm/cs.py
--rw-r--r--   0        0        0     1295 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/comm/utils.py
--rw-r--r--   0        0        0     2521 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/concurrency/__init__.py
--rw-r--r--   0        0        0     3757 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/concurrency/packing.py
--rw-r--r--   0        0        0     2533 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/concurrency/zmq_utils.py
--rw-r--r--   0        0        0       24 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/event/__init__.py
--rw-r--r--   0        0        0     2990 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/event/registry.py
--rw-r--r--   0        0        0       66 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/image/__init__.py
--rw-r--r--   0        0        0     3191 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/image/backend.py
--rw-r--r--   0        0        0     2139 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/image/codecs.py
--rw-r--r--   0        0        0     1554 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/image/imgio.py
--rw-r--r--   0        0        0     5101 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/image/imgproc.py
--rw-r--r--   0        0        0       84 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/io/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-30 04:24:29.743661 jammy-0.1.6/jammy/io/common.py
--rw-r--r--   0        0        0    12085 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/io/fs.py
--rw-r--r--   0        0        0     1342 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/io/path.py
--rw-r--r--   0        0        0      302 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/io/tempfile.py
--rw-r--r--   0        0        0       95 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/logging/__init__.py
--rw-r--r--   0        0        0      489 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/logging/fake_logger.py
--rw-r--r--   0        0        0     1167 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/logging/logger.py
--rw-r--r--   0        0        0     5341 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/logging/wandb_utils.py
--rw-r--r--   0        0        0       44 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/random/__init__.py
--rw-r--r--   0        0        0     6177 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/random/_lazy_bind.py
--rw-r--r--   0        0        0     2952 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/random/rng.py
--rw-r--r--   0        0        0       26 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/storage/__init__.py
--rw-r--r--   0        0        0     1045 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/storage/attr_saver.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.793661 jammy-0.1.6/jammy/storage/kv/__init__.py
--rw-r--r--   0        0        0     2437 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/storage/kv/kv.py
--rw-r--r--   0        0        0     2860 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/storage/kv/lmdb.py
--rw-r--r--   0        0        0      834 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/storage/kv/mem.py
--rw-r--r--   0        0        0     2141 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/storage/kv/memcached.py
--rw-r--r--   0        0        0      188 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/__init__.py
--rw-r--r--   0        0        0     3739 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/argument.py
--rw-r--r--   0        0        0     2306 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/cache.py
--rw-r--r--   0        0        0     1039 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/cfg.py
--rw-r--r--   0        0        0     1773 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/cnt.py
--rw-r--r--   0        0        0     1968 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/colored_tqdm.py
--rw-r--r--   0        0        0     3271 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/container.py
--rw-r--r--   0        0        0      358 2023-05-30 04:24:29.744661 jammy-0.1.6/jammy/utils/context.py
--rw-r--r--   0        0        0     1994 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/debug.py
--rw-r--r--   0        0        0     5725 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/defaults.py
--rw-r--r--   0        0        0      630 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/deprecated.py
--rw-r--r--   0        0        0     1483 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/enum.py
--rw-r--r--   0        0        0     1229 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/env.py
--rw-r--r--   0        0        0     2061 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/filelock.py
--rw-r--r--   0        0        0     1201 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/git.py
--rw-r--r--   0        0        0     1581 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/gpu.py
--rw-r--r--   0        0        0      430 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/hash.py
--rw-r--r--   0        0        0     3515 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/hyd.py
--rw-r--r--   0        0        0     2334 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/imp.py
--rw-r--r--   0        0        0      975 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/init.py
--rw-r--r--   0        0        0     1930 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/inspect.py
--rw-r--r--   0        0        0     4034 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/matching.py
--rw-r--r--   0        0        0     7222 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/meta.py
--rw-r--r--   0        0        0     2986 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/meter.py
--rw-r--r--   0        0        0       38 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/mock.py
--rw-r--r--   0        0        0      797 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/naming.py
--rw-r--r--   0        0        0     2118 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/notifier.py
--rw-r--r--   0        0        0      442 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/num_check.py
--rw-r--r--   0        0        0     8895 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/printing.py
--rw-r--r--   0        0        0     6380 2023-05-30 04:24:29.745662 jammy-0.1.6/jammy/utils/process.py
--rw-r--r--   0        0        0    17173 2023-05-30 04:24:29.746662 jammy-0.1.6/jammy/utils/profiler.py
--rw-r--r--   0        0        0     4520 2023-05-30 04:24:29.746662 jammy-0.1.6/jammy/utils/registry.py
--rw-r--r--   0        0        0     4694 2023-05-30 04:24:29.746662 jammy-0.1.6/jammy/utils/retry.py
--rw-r--r--   0        0        0     1281 2023-05-30 04:24:29.746662 jammy-0.1.6/jammy/utils/sizeof.py
--rw-r--r--   0        0        0       81 2023-05-30 04:24:29.746662 jammy-0.1.6/jamnp/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-30 04:24:29.746662 jammy-0.1.6/jamnp/buffer_storage.py
--rw-r--r--   0        0        0     1075 2023-05-30 04:24:29.746662 jammy-0.1.6/jamnp/container.py
--rw-r--r--   0        0        0      522 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/__init__.py
--rw-r--r--   0        0        0       22 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/cuda/__init__.py
--rw-r--r--   0        0        0      695 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/cuda/device.py
--rw-r--r--   0        0        0      172 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/cuda/readme.md
--rw-r--r--   0        0        0       64 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/data/__init__.py
--rw-r--r--   0        0        0     1291 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/data/buffer_storage.py
--rw-r--r--   0        0        0      554 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/data/dataset.py
--rw-r--r--   0        0        0     1532 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/data/meta.py
--rw-r--r--   0        0        0      116 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/ddp/__init__.py
--rw-r--r--   0        0        0      471 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/ddp/ddp_template.yaml
--rw-r--r--   0        0        0     2761 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/ddp/ddp_trainer.py
--rw-r--r--   0        0        0     4327 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/ddp/ddp_utils.py
--rw-r--r--   0        0        0      571 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/ddp/ema_trainer.py
--rw-r--r--   0        0        0      543 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/ddp/fns.py
--rw-r--r--   0        0        0      309 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/ddp/readme.md
--rw-r--r--   0        0        0       55 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/distributed/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-30 04:24:29.746662 jammy-0.1.6/jamtorch/distributed/basic.py
--rw-r--r--   0        0        0     2866 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/distributed/filelock.py
--rw-r--r--   0        0        0      255 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/distributions/__init__.py
--rw-r--r--   0        0        0     4576 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/distributions/base.py
--rw-r--r--   0        0        0     2513 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/distributions/discrete.py
--rw-r--r--   0        0        0      403 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/distributions/fns.py
--rw-r--r--   0        0        0     6912 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/distributions/normal.py
--rw-r--r--   0        0        0     3416 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/distributions/uniform.py
--rw-r--r--   0        0        0      108 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/io/__init__.py
--rw-r--r--   0        0        0     5084 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/io/ckpt.py
--rw-r--r--   0        0        0     2798 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/io/ema.py
--rw-r--r--   0        0        0      475 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/io/ema_helper.py
--rw-r--r--   0        0        0      207 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/io/io.py
--rw-r--r--   0        0        0     2391 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/io/param_ema.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.795661 jammy-0.1.6/jamtorch/learn/__init__.py
--rw-r--r--   0        0        0     4248 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/learn/gan/sn_discriminator.py
--rw-r--r--   0        0        0       22 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/logging/__init__.py
--rw-r--r--   0        0        0      451 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/logging/logger.py
--rw-r--r--   0        0        0       76 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/nn/__init__.py
--rw-r--r--   0        0        0     7517 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/nn/base_modules.py
--rw-r--r--   0        0        0     2588 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/nn/fouriermlp.py
--rw-r--r--   0        0        0      186 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/nn/readme.md
--rw-r--r--   0        0        0     4461 2023-05-30 04:24:29.747661 jammy-0.1.6/jamtorch/nn/seq.py
--rw-r--r--   0        0        0      572 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/nn/simple_network.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.795661 jammy-0.1.6/jamtorch/nn/utils/__init__.py
--rw-r--r--   0        0        0    14986 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/nn/utils/spectral_norm.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.795661 jammy-0.1.6/jamtorch/pl_callbacks/__init__.py
--rw-r--r--   0        0        0     1438 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/pl_callbacks/cuda_cb.py
--rw-r--r--   0        0        0      575 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/pl_callbacks/every_n.py
--rw-r--r--   0        0        0      552 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/prototype/__init__.py
--rw-r--r--   0        0        0      185 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/prototype/optim.py
--rw-r--r--   0        0        0     3560 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/prototype/pytorch_util.py
--rw-r--r--   0        0        0      177 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/readme.md
--rw-r--r--   0        0        0      106 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/__init__.py
--rw-r--r--   0        0        0     3228 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/amp.py
--rw-r--r--   0        0        0     2956 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/cfg_trainer.py
--rw-r--r--   0        0        0      413 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/design_trainer.md
--rw-r--r--   0        0        0      738 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/ema_trainer.py
--rw-r--r--   0        0        0    10807 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/genetic_trainer.py
--rw-r--r--   0        0        0      400 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/hydra_utils.py
--rw-r--r--   0        0        0     2940 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/monitor.py
--rw-r--r--   0        0        0     3632 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/progress_fn.py
--rw-r--r--   0        0        0     1070 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/simple_trainer.py
--rw-r--r--   0        0        0     2489 2023-05-30 04:24:29.748661 jammy-0.1.6/jamtorch/trainer/tb.py
--rw-r--r--   0        0        0     5312 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/trainer/test_trainer.py
--rw-r--r--   0        0        0    10617 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/trainer/trainer.py
--rw-r--r--   0        0        0     2161 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/trainer/trainer_fn.py
--rw-r--r--   0        0        0     1474 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/trainer/trainer_monitor.py
--rw-r--r--   0        0        0     2242 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/trainer/utils.py
--rw-r--r--   0        0        0       69 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/utils/__init__.py
--rw-r--r--   0        0        0      907 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/utils/deep_to.py
--rw-r--r--   0        0        0      239 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/utils/grad.py
--rw-r--r--   0        0        0      523 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/utils/init.py
--rw-r--r--   0        0        0     2324 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/utils/meta.py
--rw-r--r--   0        0        0     2325 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/utils/pytree.py
--rw-r--r--   0        0        0     3217 2023-05-30 04:24:29.749662 jammy-0.1.6/jamtorch/utils/ts_ops.py
--rw-r--r--   0        0        0      129 2023-05-30 04:24:29.749662 jammy-0.1.6/jamviz/README.md
--rw-r--r--   0        0        0       19 2023-05-30 04:24:29.749662 jammy-0.1.6/jamviz/__init__.py
--rw-r--r--   0        0        0     2482 2023-05-30 04:24:29.749662 jammy-0.1.6/jamviz/img.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.795661 jammy-0.1.6/jamviz/jupyter/__init__.py
--rw-r--r--   0        0        0       64 2023-05-30 04:24:29.749662 jammy-0.1.6/jamviz/plt/__init__.py
--rw-r--r--   0        0        0     2297 2023-05-30 04:24:29.749662 jammy-0.1.6/jamviz/plt/color_list.py
--rw-r--r--   0        0        0      613 2023-05-30 04:24:29.749662 jammy-0.1.6/jamviz/plt/img.py
--rw-r--r--   0        0        0     4405 2023-05-30 04:24:29.749662 jammy-0.1.6/jamviz/plt/mstd.py
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.795661 jammy-0.1.6/jamweb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-30 04:24:29.749662 jammy-0.1.6/jamweb/readme.md
--rw-r--r--   0        0        0        0 2023-05-30 04:24:29.795661 jammy-0.1.6/jamweb/session/__init__.py
--rw-r--r--   0        0        0     2649 2023-05-30 04:24:29.749662 jammy-0.1.6/jamweb/session/memcached.py
--rw-r--r--   0        0        0     1662 2023-05-30 04:24:29.749662 jammy-0.1.6/jamweb/session/session.py
--rw-r--r--   0        0        0       27 2023-05-30 04:24:29.750661 jammy-0.1.6/jamweb/web/__init__.py
--rw-r--r--   0        0        0     5935 2023-05-30 04:24:29.750661 jammy-0.1.6/jamweb/web/application.py
--rw-r--r--   0        0        0     2883 2023-05-30 04:24:30.890650 jammy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 jammy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-06-27 00:21:24.963913 jammy-0.1.7/README.md
+-rw-r--r--   0        0        0     1259 2023-06-27 00:21:24.966913 jammy-0.1.7/jammy/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli/__init__.py
+-rw-r--r--   0        0        0     5682 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli/argument.py
+-rw-r--r--   0        0        0     1329 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli/cmd_utils.py
+-rw-r--r--   0        0        0     2047 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli/cmdline_viz.py
+-rw-r--r--   0        0        0     2403 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli/colors.py
+-rw-r--r--   0        0        0     1743 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli/device.py
+-rw-r--r--   0        0        0     2754 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli/keyboard.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.017911 jammy-0.1.7/jammy/cli_scripts/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.017911 jammy-0.1.7/jammy/cli_scripts/conf/__init__.py
+-rw-r--r--   0        0        0      302 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/conf/jamdk.yaml
+-rw-r--r--   0        0        0      452 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/conf/ngc.yaml
+-rw-r--r--   0        0        0     4256 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/dk.py
+-rw-r--r--   0        0        0     3716 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/gpu_sc.py
+-rw-r--r--   0        0        0      304 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/inspect_file.py
+-rw-r--r--   0        0        0     6839 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/ngc_debug.py
+-rw-r--r--   0        0        0    17767 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/shell_executor.py
+-rw-r--r--   0        0        0    15458 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/cli_scripts/sys_info.py
+-rw-r--r--   0        0        0       31 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/collections/__init__.py
+-rw-r--r--   0        0        0      312 2023-06-27 00:21:24.967913 jammy-0.1.7/jammy/collections/lazy_dict.py
+-rw-r--r--   0        0        0       39 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/comm/__init__.py
+-rw-r--r--   0        0        0     6007 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/comm/cs.py
+-rw-r--r--   0        0        0     1295 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/comm/utils.py
+-rw-r--r--   0        0        0     2521 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/concurrency/__init__.py
+-rw-r--r--   0        0        0     3757 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/concurrency/packing.py
+-rw-r--r--   0        0        0     2533 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/concurrency/zmq_utils.py
+-rw-r--r--   0        0        0       24 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/event/__init__.py
+-rw-r--r--   0        0        0     2990 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/event/registry.py
+-rw-r--r--   0        0        0       66 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/image/__init__.py
+-rw-r--r--   0        0        0     3191 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/image/backend.py
+-rw-r--r--   0        0        0     2139 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/image/codecs.py
+-rw-r--r--   0        0        0     1554 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/image/imgio.py
+-rw-r--r--   0        0        0     5101 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/image/imgproc.py
+-rw-r--r--   0        0        0       84 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/io/__init__.py
+-rw-r--r--   0        0        0     1088 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/io/common.py
+-rw-r--r--   0        0        0    12085 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/io/fs.py
+-rw-r--r--   0        0        0     1342 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/io/path.py
+-rw-r--r--   0        0        0      302 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/io/tempfile.py
+-rw-r--r--   0        0        0       95 2023-06-27 00:21:24.968912 jammy-0.1.7/jammy/logging/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/logging/fake_logger.py
+-rw-r--r--   0        0        0     1167 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/logging/logger.py
+-rw-r--r--   0        0        0     5341 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/logging/wandb_utils.py
+-rw-r--r--   0        0        0       44 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/random/__init__.py
+-rw-r--r--   0        0        0     6177 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/random/_lazy_bind.py
+-rw-r--r--   0        0        0     2952 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/random/rng.py
+-rw-r--r--   0        0        0       26 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/storage/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/storage/attr_saver.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.017911 jammy-0.1.7/jammy/storage/kv/__init__.py
+-rw-r--r--   0        0        0     2437 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/storage/kv/kv.py
+-rw-r--r--   0        0        0     2860 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/storage/kv/lmdb.py
+-rw-r--r--   0        0        0      834 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/storage/kv/mem.py
+-rw-r--r--   0        0        0     2141 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/storage/kv/memcached.py
+-rw-r--r--   0        0        0      188 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/__init__.py
+-rw-r--r--   0        0        0     3739 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/argument.py
+-rw-r--r--   0        0        0     2306 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/cache.py
+-rw-r--r--   0        0        0     1039 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/cfg.py
+-rw-r--r--   0        0        0     1773 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/cnt.py
+-rw-r--r--   0        0        0     1968 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/colored_tqdm.py
+-rw-r--r--   0        0        0     3271 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/container.py
+-rw-r--r--   0        0        0      358 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/context.py
+-rw-r--r--   0        0        0     1994 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/debug.py
+-rw-r--r--   0        0        0     5725 2023-06-27 00:21:24.969912 jammy-0.1.7/jammy/utils/defaults.py
+-rw-r--r--   0        0        0      630 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/deprecated.py
+-rw-r--r--   0        0        0     1483 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/enum.py
+-rw-r--r--   0        0        0     1229 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/env.py
+-rw-r--r--   0        0        0     2061 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/filelock.py
+-rw-r--r--   0        0        0     1201 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/git.py
+-rw-r--r--   0        0        0     1581 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/gpu.py
+-rw-r--r--   0        0        0      430 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/hash.py
+-rw-r--r--   0        0        0     3515 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/hyd.py
+-rw-r--r--   0        0        0     2334 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/imp.py
+-rw-r--r--   0        0        0      975 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/init.py
+-rw-r--r--   0        0        0     1930 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/inspect.py
+-rw-r--r--   0        0        0     4034 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/matching.py
+-rw-r--r--   0        0        0     7222 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/meta.py
+-rw-r--r--   0        0        0     2986 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/meter.py
+-rw-r--r--   0        0        0       38 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/mock.py
+-rw-r--r--   0        0        0      797 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/naming.py
+-rw-r--r--   0        0        0     2118 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/notifier.py
+-rw-r--r--   0        0        0      442 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/num_check.py
+-rw-r--r--   0        0        0     8895 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/printing.py
+-rw-r--r--   0        0        0     6380 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/process.py
+-rw-r--r--   0        0        0    17173 2023-06-27 00:21:24.970912 jammy-0.1.7/jammy/utils/profiler.py
+-rw-r--r--   0        0        0     4520 2023-06-27 00:21:24.971912 jammy-0.1.7/jammy/utils/registry.py
+-rw-r--r--   0        0        0     4694 2023-06-27 00:21:24.971912 jammy-0.1.7/jammy/utils/retry.py
+-rw-r--r--   0        0        0     1281 2023-06-27 00:21:24.971912 jammy-0.1.7/jammy/utils/sizeof.py
+-rw-r--r--   0        0        0       81 2023-06-27 00:21:24.971912 jammy-0.1.7/jamnp/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-27 00:21:24.971912 jammy-0.1.7/jamnp/buffer_storage.py
+-rw-r--r--   0        0        0     1075 2023-06-27 00:21:24.971912 jammy-0.1.7/jamnp/container.py
+-rw-r--r--   0        0        0      522 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/cuda/__init__.py
+-rw-r--r--   0        0        0      695 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/cuda/device.py
+-rw-r--r--   0        0        0      172 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/cuda/readme.md
+-rw-r--r--   0        0        0       64 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/data/__init__.py
+-rw-r--r--   0        0        0     1291 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/data/buffer_storage.py
+-rw-r--r--   0        0        0      554 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/data/dataset.py
+-rw-r--r--   0        0        0     1532 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/data/meta.py
+-rw-r--r--   0        0        0      116 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/ddp/__init__.py
+-rw-r--r--   0        0        0      471 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/ddp/ddp_template.yaml
+-rw-r--r--   0        0        0     2761 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/ddp/ddp_trainer.py
+-rw-r--r--   0        0        0     4327 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/ddp/ddp_utils.py
+-rw-r--r--   0        0        0      571 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/ddp/ema_trainer.py
+-rw-r--r--   0        0        0      543 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/ddp/fns.py
+-rw-r--r--   0        0        0      309 2023-06-27 00:21:24.971912 jammy-0.1.7/jamtorch/ddp/readme.md
+-rw-r--r--   0        0        0       55 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributed/__init__.py
+-rw-r--r--   0        0        0     1183 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributed/basic.py
+-rw-r--r--   0        0        0     2866 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributed/filelock.py
+-rw-r--r--   0        0        0      255 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributions/__init__.py
+-rw-r--r--   0        0        0     4576 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributions/base.py
+-rw-r--r--   0        0        0     2513 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributions/discrete.py
+-rw-r--r--   0        0        0      403 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributions/fns.py
+-rw-r--r--   0        0        0     6912 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributions/normal.py
+-rw-r--r--   0        0        0     3416 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/distributions/uniform.py
+-rw-r--r--   0        0        0      108 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/io/__init__.py
+-rw-r--r--   0        0        0     5084 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/io/ckpt.py
+-rw-r--r--   0        0        0     2798 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/io/ema.py
+-rw-r--r--   0        0        0      475 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/io/ema_helper.py
+-rw-r--r--   0        0        0      207 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/io/io.py
+-rw-r--r--   0        0        0     2391 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/io/param_ema.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.017911 jammy-0.1.7/jamtorch/learn/__init__.py
+-rw-r--r--   0        0        0     4248 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/learn/gan/sn_discriminator.py
+-rw-r--r--   0        0        0       22 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/logging/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/logging/logger.py
+-rw-r--r--   0        0        0       76 2023-06-27 00:21:24.972912 jammy-0.1.7/jamtorch/nn/__init__.py
+-rw-r--r--   0        0        0     7517 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/nn/base_modules.py
+-rw-r--r--   0        0        0     2588 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/nn/fouriermlp.py
+-rw-r--r--   0        0        0      186 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/nn/readme.md
+-rw-r--r--   0        0        0     4461 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/nn/seq.py
+-rw-r--r--   0        0        0      572 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/nn/simple_network.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.025911 jammy-0.1.7/jamtorch/nn/utils/__init__.py
+-rw-r--r--   0        0        0    14986 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/nn/utils/spectral_norm.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.025911 jammy-0.1.7/jamtorch/pl_callbacks/__init__.py
+-rw-r--r--   0        0        0     1438 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/pl_callbacks/cuda_cb.py
+-rw-r--r--   0        0        0      575 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/pl_callbacks/every_n.py
+-rw-r--r--   0        0        0      552 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/prototype/__init__.py
+-rw-r--r--   0        0        0      185 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/prototype/optim.py
+-rw-r--r--   0        0        0     3560 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/prototype/pytorch_util.py
+-rw-r--r--   0        0        0      177 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/readme.md
+-rw-r--r--   0        0        0      106 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/trainer/__init__.py
+-rw-r--r--   0        0        0     3228 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/trainer/amp.py
+-rw-r--r--   0        0        0     2956 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/trainer/cfg_trainer.py
+-rw-r--r--   0        0        0      413 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/trainer/design_trainer.md
+-rw-r--r--   0        0        0      738 2023-06-27 00:21:24.973912 jammy-0.1.7/jamtorch/trainer/ema_trainer.py
+-rw-r--r--   0        0        0    10807 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/genetic_trainer.py
+-rw-r--r--   0        0        0      400 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/hydra_utils.py
+-rw-r--r--   0        0        0     2940 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/monitor.py
+-rw-r--r--   0        0        0     3632 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/progress_fn.py
+-rw-r--r--   0        0        0     1070 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/simple_trainer.py
+-rw-r--r--   0        0        0     2489 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/tb.py
+-rw-r--r--   0        0        0     5312 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/test_trainer.py
+-rw-r--r--   0        0        0    10617 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/trainer.py
+-rw-r--r--   0        0        0     2161 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/trainer_fn.py
+-rw-r--r--   0        0        0     1474 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/trainer_monitor.py
+-rw-r--r--   0        0        0     2242 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/trainer/utils.py
+-rw-r--r--   0        0        0       69 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/utils/__init__.py
+-rw-r--r--   0        0        0      907 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/utils/deep_to.py
+-rw-r--r--   0        0        0      239 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/utils/grad.py
+-rw-r--r--   0        0        0      523 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/utils/init.py
+-rw-r--r--   0        0        0     2324 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/utils/meta.py
+-rw-r--r--   0        0        0     2325 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/utils/pytree.py
+-rw-r--r--   0        0        0     3217 2023-06-27 00:21:24.974912 jammy-0.1.7/jamtorch/utils/ts_ops.py
+-rw-r--r--   0        0        0      129 2023-06-27 00:21:24.974912 jammy-0.1.7/jamviz/README.md
+-rw-r--r--   0        0        0       19 2023-06-27 00:21:24.974912 jammy-0.1.7/jamviz/__init__.py
+-rw-r--r--   0        0        0     2482 2023-06-27 00:21:24.974912 jammy-0.1.7/jamviz/img.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.026911 jammy-0.1.7/jamviz/jupyter/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-27 00:21:24.974912 jammy-0.1.7/jamviz/plt/__init__.py
+-rw-r--r--   0        0        0     2297 2023-06-27 00:21:24.975912 jammy-0.1.7/jamviz/plt/color_list.py
+-rw-r--r--   0        0        0      613 2023-06-27 00:21:24.975912 jammy-0.1.7/jamviz/plt/img.py
+-rw-r--r--   0        0        0     4405 2023-06-27 00:21:24.975912 jammy-0.1.7/jamviz/plt/mstd.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.026911 jammy-0.1.7/jamweb/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-27 00:21:24.975912 jammy-0.1.7/jamweb/readme.md
+-rw-r--r--   0        0        0        0 2023-06-27 00:21:25.026911 jammy-0.1.7/jamweb/session/__init__.py
+-rw-r--r--   0        0        0     2649 2023-06-27 00:21:24.975912 jammy-0.1.7/jamweb/session/memcached.py
+-rw-r--r--   0        0        0     1662 2023-06-27 00:21:24.975912 jammy-0.1.7/jamweb/session/session.py
+-rw-r--r--   0        0        0       27 2023-06-27 00:21:24.975912 jammy-0.1.7/jamweb/web/__init__.py
+-rw-r--r--   0        0        0     5935 2023-06-27 00:21:24.975912 jammy-0.1.7/jamweb/web/application.py
+-rw-r--r--   0        0        0     2883 2023-06-27 00:21:26.196878 jammy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 jammy-0.1.7/PKG-INFO
```

### Comparing `jammy-0.1.6/README.md` & `jammy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/__init__.py` & `jammy-0.1.7/jammy/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli/argument.py` & `jammy-0.1.7/jammy/cli/argument.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli/cmd_utils.py` & `jammy-0.1.7/jammy/cli/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli/cmdline_viz.py` & `jammy-0.1.7/jammy/cli/cmdline_viz.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli/colors.py` & `jammy-0.1.7/jammy/cli/colors.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli/device.py` & `jammy-0.1.7/jammy/cli/device.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli/keyboard.py` & `jammy-0.1.7/jammy/cli/keyboard.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli_scripts/dk.py` & `jammy-0.1.7/jammy/cli_scripts/dk.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli_scripts/gpu_sc.py` & `jammy-0.1.7/jammy/cli_scripts/gpu_sc.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli_scripts/ngc_debug.py` & `jammy-0.1.7/jammy/cli_scripts/ngc_debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,30 @@
     'minAvailability': 1,
     'replicaCount': 1,
     'arrayType': 'PYTORCH',
     'runPolicy': {'totalRuntimeSeconds': 604800, 'preemptClass': 'RUNONCE'},
     'resultContainerMountPoint': '/result',
     'workspaceMounts': [
     ],
+    'datasetMounts': [
+    ],
 }
 
 def parse_all(cfg):
     if cfg.img is not None:
         job_cfg['dockerImageName'] = cfg.img
     if cfg.name is not None:
         job_cfg['name'] = "ml-model.qsh_debug."+cfg.name
     else:
         job_cfg['name'] = f"ml-model.qsh_debug.{cfg.device}"
     parse_device(cfg)
     parse_cmd(cfg)
     parse_ws_qsh(cfg)
     parse_extra_ws(cfg)
+    parse_dataset(cfg)
 
 def parse_device(cfg):
     if cfg.device is not None:
         cfg.device = str(cfg.device)
         if "x" in cfg.device:
             if cfg.device.count("x") == 1:
                 num_node = 1
@@ -147,14 +150,22 @@
         for ws, target_loc in cfg.extra_ws.items():
             job_cfg['workspaceMounts'].append({
                 "containerMountPoint": target_loc,
                 "id": ws,
                 "mountMode": "RW"
             })
 
+def parse_dataset(cfg):
+    if cfg.dataset is not None:
+        for dataset_id, target_loc in cfg.dataset.items():
+            job_cfg['datasetMounts'].append({
+                "containerMountPoint": target_loc,
+                "id": dataset_id,
+            })
+
 def read_local_cfg(cfg):
     cfg_path = hydra.utils.to_absolute_path(cfg.file)
     if not osp.exists(cfg_path):
         return cfg
     logger.info("readding config from: " + cfg_path)
     local_cfg = OmegaConf.load(cfg_path)
     cli_cfg = OmegaConf.from_cli()
```

### Comparing `jammy-0.1.6/jammy/cli_scripts/shell_executor.py` & `jammy-0.1.7/jammy/cli_scripts/shell_executor.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/cli_scripts/sys_info.py` & `jammy-0.1.7/jammy/cli_scripts/sys_info.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/comm/cs.py` & `jammy-0.1.7/jammy/comm/cs.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/comm/utils.py` & `jammy-0.1.7/jammy/comm/utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/concurrency/__init__.py` & `jammy-0.1.7/jammy/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/concurrency/packing.py` & `jammy-0.1.7/jammy/concurrency/packing.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/concurrency/zmq_utils.py` & `jammy-0.1.7/jammy/concurrency/zmq_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/event/registry.py` & `jammy-0.1.7/jammy/event/registry.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/image/backend.py` & `jammy-0.1.7/jammy/image/backend.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/image/codecs.py` & `jammy-0.1.7/jammy/image/codecs.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/image/imgio.py` & `jammy-0.1.7/jammy/image/imgio.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/image/imgproc.py` & `jammy-0.1.7/jammy/image/imgproc.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/io/common.py` & `jammy-0.1.7/jammy/io/common.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/io/fs.py` & `jammy-0.1.7/jammy/io/fs.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/io/path.py` & `jammy-0.1.7/jammy/io/path.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/logging/logger.py` & `jammy-0.1.7/jammy/logging/logger.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/logging/wandb_utils.py` & `jammy-0.1.7/jammy/logging/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/random/_lazy_bind.py` & `jammy-0.1.7/jammy/random/_lazy_bind.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/random/rng.py` & `jammy-0.1.7/jammy/random/rng.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/storage/attr_saver.py` & `jammy-0.1.7/jammy/storage/attr_saver.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/storage/kv/kv.py` & `jammy-0.1.7/jammy/storage/kv/kv.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/storage/kv/lmdb.py` & `jammy-0.1.7/jammy/storage/kv/lmdb.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/storage/kv/mem.py` & `jammy-0.1.7/jammy/storage/kv/mem.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/storage/kv/memcached.py` & `jammy-0.1.7/jammy/storage/kv/memcached.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/argument.py` & `jammy-0.1.7/jammy/utils/argument.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/cache.py` & `jammy-0.1.7/jammy/utils/cache.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/cfg.py` & `jammy-0.1.7/jammy/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/cnt.py` & `jammy-0.1.7/jammy/utils/cnt.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/colored_tqdm.py` & `jammy-0.1.7/jammy/utils/colored_tqdm.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/container.py` & `jammy-0.1.7/jammy/utils/container.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/debug.py` & `jammy-0.1.7/jammy/utils/debug.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/defaults.py` & `jammy-0.1.7/jammy/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/deprecated.py` & `jammy-0.1.7/jammy/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/enum.py` & `jammy-0.1.7/jammy/utils/enum.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/env.py` & `jammy-0.1.7/jammy/utils/env.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/filelock.py` & `jammy-0.1.7/jammy/utils/filelock.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/git.py` & `jammy-0.1.7/jammy/utils/git.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/gpu.py` & `jammy-0.1.7/jammy/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/hyd.py` & `jammy-0.1.7/jammy/utils/hyd.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/imp.py` & `jammy-0.1.7/jammy/utils/imp.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/init.py` & `jammy-0.1.7/jammy/utils/init.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/inspect.py` & `jammy-0.1.7/jammy/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/matching.py` & `jammy-0.1.7/jammy/utils/matching.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/meta.py` & `jammy-0.1.7/jammy/utils/meta.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/meter.py` & `jammy-0.1.7/jammy/utils/meter.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/naming.py` & `jammy-0.1.7/jammy/utils/naming.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/notifier.py` & `jammy-0.1.7/jammy/utils/notifier.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/printing.py` & `jammy-0.1.7/jammy/utils/printing.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/process.py` & `jammy-0.1.7/jammy/utils/process.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/profiler.py` & `jammy-0.1.7/jammy/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/registry.py` & `jammy-0.1.7/jammy/utils/registry.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/retry.py` & `jammy-0.1.7/jammy/utils/retry.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jammy/utils/sizeof.py` & `jammy-0.1.7/jammy/utils/sizeof.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamnp/buffer_storage.py` & `jammy-0.1.7/jamnp/buffer_storage.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamnp/container.py` & `jammy-0.1.7/jamnp/container.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/__init__.py` & `jammy-0.1.7/jamtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/cuda/device.py` & `jammy-0.1.7/jamtorch/cuda/device.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/data/buffer_storage.py` & `jammy-0.1.7/jamtorch/data/buffer_storage.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/data/dataset.py` & `jammy-0.1.7/jamtorch/data/dataset.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/data/meta.py` & `jammy-0.1.7/jamtorch/data/meta.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/ddp/ddp_trainer.py` & `jammy-0.1.7/jamtorch/ddp/ddp_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/ddp/ddp_utils.py` & `jammy-0.1.7/jamtorch/ddp/ddp_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/ddp/ema_trainer.py` & `jammy-0.1.7/jamtorch/ddp/ema_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/ddp/fns.py` & `jammy-0.1.7/jamtorch/ddp/fns.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/distributed/basic.py` & `jammy-0.1.7/jamtorch/distributed/basic.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/distributed/filelock.py` & `jammy-0.1.7/jamtorch/distributed/filelock.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/distributions/base.py` & `jammy-0.1.7/jamtorch/distributions/base.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/distributions/discrete.py` & `jammy-0.1.7/jamtorch/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/distributions/normal.py` & `jammy-0.1.7/jamtorch/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/distributions/uniform.py` & `jammy-0.1.7/jamtorch/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/io/ckpt.py` & `jammy-0.1.7/jamtorch/io/ckpt.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/io/ema.py` & `jammy-0.1.7/jamtorch/io/ema.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/io/param_ema.py` & `jammy-0.1.7/jamtorch/io/param_ema.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/learn/gan/sn_discriminator.py` & `jammy-0.1.7/jamtorch/learn/gan/sn_discriminator.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/nn/base_modules.py` & `jammy-0.1.7/jamtorch/nn/base_modules.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/nn/fouriermlp.py` & `jammy-0.1.7/jamtorch/nn/fouriermlp.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/nn/seq.py` & `jammy-0.1.7/jamtorch/nn/seq.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/nn/simple_network.py` & `jammy-0.1.7/jamtorch/nn/simple_network.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/nn/utils/spectral_norm.py` & `jammy-0.1.7/jamtorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/pl_callbacks/cuda_cb.py` & `jammy-0.1.7/jamtorch/pl_callbacks/cuda_cb.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/pl_callbacks/every_n.py` & `jammy-0.1.7/jamtorch/pl_callbacks/every_n.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/prototype/__init__.py` & `jammy-0.1.7/jamtorch/prototype/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/prototype/pytorch_util.py` & `jammy-0.1.7/jamtorch/prototype/pytorch_util.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/amp.py` & `jammy-0.1.7/jamtorch/trainer/amp.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/cfg_trainer.py` & `jammy-0.1.7/jamtorch/trainer/cfg_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/ema_trainer.py` & `jammy-0.1.7/jamtorch/trainer/ema_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/genetic_trainer.py` & `jammy-0.1.7/jamtorch/trainer/genetic_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/monitor.py` & `jammy-0.1.7/jamtorch/trainer/monitor.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/progress_fn.py` & `jammy-0.1.7/jamtorch/trainer/progress_fn.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/simple_trainer.py` & `jammy-0.1.7/jamtorch/trainer/simple_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/tb.py` & `jammy-0.1.7/jamtorch/trainer/tb.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/test_trainer.py` & `jammy-0.1.7/jamtorch/trainer/test_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/trainer.py` & `jammy-0.1.7/jamtorch/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/trainer_fn.py` & `jammy-0.1.7/jamtorch/trainer/trainer_fn.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/trainer_monitor.py` & `jammy-0.1.7/jamtorch/trainer/trainer_monitor.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/trainer/utils.py` & `jammy-0.1.7/jamtorch/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/utils/deep_to.py` & `jammy-0.1.7/jamtorch/utils/deep_to.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/utils/init.py` & `jammy-0.1.7/jamtorch/utils/init.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/utils/meta.py` & `jammy-0.1.7/jamtorch/utils/meta.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/utils/pytree.py` & `jammy-0.1.7/jamtorch/utils/pytree.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamtorch/utils/ts_ops.py` & `jammy-0.1.7/jamtorch/utils/ts_ops.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamviz/img.py` & `jammy-0.1.7/jamviz/img.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamviz/plt/color_list.py` & `jammy-0.1.7/jamviz/plt/color_list.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamviz/plt/img.py` & `jammy-0.1.7/jamviz/plt/img.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamviz/plt/mstd.py` & `jammy-0.1.7/jamviz/plt/mstd.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamweb/session/memcached.py` & `jammy-0.1.7/jamweb/session/memcached.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamweb/session/session.py` & `jammy-0.1.7/jamweb/session/session.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/jamweb/web/application.py` & `jammy-0.1.7/jamweb/web/application.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.6/pyproject.toml` & `jammy-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jammy"
-version = "0.1.6"
+version = "0.1.7"
 description = "A Versatile ToolBox"
 authors = ["Qin <qsh.zh27@gmail.com>"]
 license = "MIT"
 packages = [
     { include="jammy" },
     { include="jamtorch" },
     { include="jamnp" },
```

### Comparing `jammy-0.1.6/PKG-INFO` & `jammy-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jammy
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Versatile ToolBox
 License: MIT
 Author: Qin
 Author-email: qsh.zh27@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jammy Version: 0.1.6 Summary: A Versatile ToolBox
+Metadata-Version: 2.1 Name: jammy Version: 0.1.7 Summary: A Versatile ToolBox
 License: MIT Author: Qin Author-email: qsh.zh27@gmail.com Requires-Python:
 >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Provides-Extra: all Provides-Extra: pro Provides-Extra: storage
 Provides-Extra: torch Provides-Extra: web Requires-Dist: GitPython
```

