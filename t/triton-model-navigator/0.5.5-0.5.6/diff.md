# Comparing `tmp/triton_model_navigator-0.5.5-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,135 +1,135 @@
-Zip file size: 234334 bytes, number of entries: 133
--rw-r--r--  2.0 unx      881 b- defN 23-May-24 10:59 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-May-24 10:59 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3668 b- defN 23-May-24 10:59 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     9474 b- defN 23-May-24 10:59 model_navigator/execution_context.py
--rw-r--r--  2.0 unx     4790 b- defN 23-May-24 10:59 model_navigator/logger.py
--rw-rw-rw-  2.0 unx     1716 b- defN 23-May-24 10:59 model_navigator/api/__init__.py
--rw-rw-rw-  2.0 unx    24304 b- defN 23-May-24 10:59 model_navigator/api/config.py
--rw-rw-rw-  2.0 unx     6425 b- defN 23-May-24 10:59 model_navigator/api/jax.py
--rw-rw-rw-  2.0 unx     5423 b- defN 23-May-24 10:59 model_navigator/api/onnx.py
--rw-rw-rw-  2.0 unx    11860 b- defN 23-May-24 10:59 model_navigator/api/package.py
--rw-rw-rw-  2.0 unx     4906 b- defN 23-May-24 10:59 model_navigator/api/python.py
--rw-rw-rw-  2.0 unx     7748 b- defN 23-May-24 10:59 model_navigator/api/pytriton.py
--rw-rw-rw-  2.0 unx     6519 b- defN 23-May-24 10:59 model_navigator/api/tensorflow.py
--rw-rw-rw-  2.0 unx     6325 b- defN 23-May-24 10:59 model_navigator/api/torch.py
--rw-rw-rw-  2.0 unx     1553 b- defN 23-May-24 10:59 model_navigator/api/triton.py
--rw-rw-rw-  2.0 unx     1811 b- defN 23-May-24 10:59 model_navigator/api/utilities.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/__init__.py
--rw-rw-rw-  2.0 unx     4938 b- defN 23-May-24 10:59 model_navigator/commands/base.py
--rw-rw-rw-  2.0 unx    10065 b- defN 23-May-24 10:59 model_navigator/commands/infer_metadata.py
--rw-rw-rw-  2.0 unx     3289 b- defN 23-May-24 10:59 model_navigator/commands/load.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/convert/__init__.py
--rw-rw-rw-  2.0 unx     9863 b- defN 23-May-24 10:59 model_navigator/commands/convert/base.py
--rw-rw-rw-  2.0 unx     7838 b- defN 23-May-24 10:59 model_navigator/commands/convert/tf.py
--rw-rw-rw-  2.0 unx    10224 b- defN 23-May-24 10:59 model_navigator/commands/convert/torch.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/__init__.py
--rw-rw-rw-  2.0 unx     3418 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-rw-rw-  2.0 unx     3105 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/ts2onnx.py
--rw-rw-rw-  2.0 unx     4992 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-rw-rw-  2.0 unx      680 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/__init__.py
--rw-rw-rw-  2.0 unx     1727 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-rw-rw-  2.0 unx    10818 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-rw-rw-  2.0 unx     2235 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/copy/__init__.py
--rw-rw-rw-  2.0 unx     1729 b- defN 23-May-24 10:59 model_navigator/commands/copy/onnx.py
--rw-rw-rw-  2.0 unx      678 b- defN 23-May-24 10:59 model_navigator/commands/correctness/__init__.py
--rw-rw-rw-  2.0 unx     5594 b- defN 23-May-24 10:59 model_navigator/commands/correctness/correctness.py
--rw-rw-rw-  2.0 unx     4550 b- defN 23-May-24 10:59 model_navigator/commands/correctness/correctness_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/data_dump/__init__.py
--rw-rw-rw-  2.0 unx    11162 b- defN 23-May-24 10:59 model_navigator/commands/data_dump/samples.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/export/__init__.py
--rw-rw-rw-  2.0 unx     3531 b- defN 23-May-24 10:59 model_navigator/commands/export/jax.py
--rw-rw-rw-  2.0 unx     5485 b- defN 23-May-24 10:59 model_navigator/commands/export/tf.py
--rw-rw-rw-  2.0 unx     9043 b- defN 23-May-24 10:59 model_navigator/commands/export/torch.py
--rw-rw-rw-  2.0 unx     1056 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/__init__.py
--rw-rw-rw-  2.0 unx     3945 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-rw-rw-  2.0 unx     3171 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-rw-rw-  2.0 unx     3122 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-rw-rw-  2.0 unx     3077 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/torch2onnx.py
--rw-rw-rw-  2.0 unx     2728 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-rw-rw-  2.0 unx      715 b- defN 23-May-24 10:59 model_navigator/commands/find_max_batch_size/__init__.py
--rw-rw-rw-  2.0 unx     6396 b- defN 23-May-24 10:59 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-rw-rw-  2.0 unx     2984 b- defN 23-May-24 10:59 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-rw-rw-  2.0 unx      688 b- defN 23-May-24 10:59 model_navigator/commands/performance/__init__.py
--rw-rw-rw-  2.0 unx    15770 b- defN 23-May-24 10:59 model_navigator/commands/performance/performance.py
--rw-rw-rw-  2.0 unx     3037 b- defN 23-May-24 10:59 model_navigator/commands/performance/performance_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/verification/__init__.py
--rw-rw-rw-  2.0 unx     5441 b- defN 23-May-24 10:59 model_navigator/commands/verification/verify.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/configuration/__init__.py
--rw-rw-rw-  2.0 unx     2473 b- defN 23-May-24 10:59 model_navigator/configuration/common_config.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/configuration/model/__init__.py
--rw-rw-rw-  2.0 unx    15623 b- defN 23-May-24 10:59 model_navigator/configuration/model/model_config.py
--rw-rw-rw-  2.0 unx    13677 b- defN 23-May-24 10:59 model_navigator/configuration/model/model_config_builder.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/core/__init__.py
--rw-rw-rw-  2.0 unx     1326 b- defN 23-May-24 10:59 model_navigator/core/constants.py
--rw-rw-rw-  2.0 unx    20111 b- defN 23-May-24 10:59 model_navigator/core/package.py
--rw-rw-rw-  2.0 unx    20337 b- defN 23-May-24 10:59 model_navigator/core/status.py
--rw-rw-rw-  2.0 unx     8052 b- defN 23-May-24 10:59 model_navigator/core/tensor.py
--rw-rw-rw-  2.0 unx     2817 b- defN 23-May-24 10:59 model_navigator/frameworks/__init__.py
--rw-rw-rw-  2.0 unx      669 b- defN 23-May-24 10:59 model_navigator/frameworks/jax/__init__.py
--rw-rw-rw-  2.0 unx     1554 b- defN 23-May-24 10:59 model_navigator/frameworks/jax/model.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/frameworks/onnx/__init__.py
--rw-rw-rw-  2.0 unx     1085 b- defN 23-May-24 10:59 model_navigator/frameworks/onnx/utils.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/frameworks/tensorrt/__init__.py
--rw-rw-rw-  2.0 unx    26575 b- defN 23-May-24 10:59 model_navigator/frameworks/tensorrt/cuda.py
--rw-rw-rw-  2.0 unx     9874 b- defN 23-May-24 10:59 model_navigator/frameworks/tensorrt/utils.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/frameworks/torch/__init__.py
--rw-rw-rw-  2.0 unx     1508 b- defN 23-May-24 10:59 model_navigator/frameworks/torch/utils.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/pipelines/__init__.py
--rw-rw-rw-  2.0 unx     5685 b- defN 23-May-24 10:59 model_navigator/pipelines/pipeline.py
--rw-rw-rw-  2.0 unx     7333 b- defN 23-May-24 10:59 model_navigator/pipelines/pipeline_manager.py
--rw-rw-rw-  2.0 unx     9805 b- defN 23-May-24 10:59 model_navigator/pipelines/validation.py
--rw-rw-rw-  2.0 unx     1879 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/__init__.py
--rw-rw-rw-  2.0 unx     2036 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/correctness.py
--rw-rw-rw-  2.0 unx     5703 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-rw-rw-  2.0 unx     1647 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/jax.py
--rw-rw-rw-  2.0 unx     2483 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/onnx.py
--rw-rw-rw-  2.0 unx     2365 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/preprocessing.py
--rw-rw-rw-  2.0 unx     2685 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/profiling.py
--rw-rw-rw-  2.0 unx     2869 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/tensorflow.py
--rw-rw-rw-  2.0 unx     3261 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/torch.py
--rw-rw-rw-  2.0 unx     2042 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/verify.py
--rw-rw-rw-  2.0 unx     1584 b- defN 23-May-24 10:59 model_navigator/runners/__init__.py
--rw-rw-rw-  2.0 unx    11369 b- defN 23-May-24 10:59 model_navigator/runners/base.py
--rw-rw-rw-  2.0 unx     2620 b- defN 23-May-24 10:59 model_navigator/runners/jax.py
--rw-rw-rw-  2.0 unx     7302 b- defN 23-May-24 10:59 model_navigator/runners/onnx.py
--rw-rw-rw-  2.0 unx     2267 b- defN 23-May-24 10:59 model_navigator/runners/python.py
--rw-rw-rw-  2.0 unx     2285 b- defN 23-May-24 10:59 model_navigator/runners/registry.py
--rw-rw-rw-  2.0 unx     7976 b- defN 23-May-24 10:59 model_navigator/runners/tensorflow.py
--rw-rw-rw-  2.0 unx    25301 b- defN 23-May-24 10:59 model_navigator/runners/tensorrt.py
--rw-rw-rw-  2.0 unx     7699 b- defN 23-May-24 10:59 model_navigator/runners/torch.py
--rw-rw-rw-  2.0 unx     3554 b- defN 23-May-24 10:59 model_navigator/runners/utils.py
--rw-rw-rw-  2.0 unx      937 b- defN 23-May-24 10:59 model_navigator/runtime_analyzer/__init__.py
--rw-rw-rw-  2.0 unx    11706 b- defN 23-May-24 10:59 model_navigator/runtime_analyzer/analyzer.py
--rw-rw-rw-  2.0 unx     2304 b- defN 23-May-24 10:59 model_navigator/runtime_analyzer/strategy.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/triton/__init__.py
--rw-rw-rw-  2.0 unx     3180 b- defN 23-May-24 10:59 model_navigator/triton/model_config.py
--rw-rw-rw-  2.0 unx     5218 b- defN 23-May-24 10:59 model_navigator/triton/model_config_builder.py
--rw-rw-rw-  2.0 unx    23090 b- defN 23-May-24 10:59 model_navigator/triton/model_config_generator.py
--rw-rw-rw-  2.0 unx    15193 b- defN 23-May-24 10:59 model_navigator/triton/model_repository.py
--rw-rw-rw-  2.0 unx     2081 b- defN 23-May-24 10:59 model_navigator/triton/utils.py
--rw-rw-rw-  2.0 unx      944 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/__init__.py
--rw-rw-rw-  2.0 unx     2872 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/base_model_config.py
--rw-rw-rw-  2.0 unx    22326 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/common.py
--rw-rw-rw-  2.0 unx     2229 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/internal.py
--rw-rw-rw-  2.0 unx     2685 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-rw-rw-  2.0 unx     1785 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/python_model_config.py
--rw-rw-rw-  2.0 unx     2239 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-rw-rw-  2.0 unx     3162 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-rw-rw-  2.0 unx     3040 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/utils/__init__.py
--rw-rw-rw-  2.0 unx    14113 b- defN 23-May-24 10:59 model_navigator/utils/common.py
--rw-rw-rw-  2.0 unx     7996 b- defN 23-May-24 10:59 model_navigator/utils/dataloader.py
--rw-rw-rw-  2.0 unx     3902 b- defN 23-May-24 10:59 model_navigator/utils/devices.py
--rw-rw-rw-  2.0 unx     1308 b- defN 23-May-24 10:59 model_navigator/utils/enums.py
--rw-rw-rw-  2.0 unx     6163 b- defN 23-May-24 10:59 model_navigator/utils/environment.py
--rw-rw-rw-  2.0 unx     3528 b- defN 23-May-24 10:59 model_navigator/utils/format_helpers.py
--rw-rw-rw-  2.0 unx     2325 b- defN 23-May-24 10:59 model_navigator/utils/module.py
--rw-rw-rw-  2.0 unx     3233 b- defN 23-May-24 10:59 model_navigator/utils/package.py
--rw-rw-rw-  2.0 unx    10140 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    12074 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    13272 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/RECORD
-133 files, 705762 bytes uncompressed, 212698 bytes compressed:  69.9%
+Zip file size: 234262 bytes, number of entries: 133
+-rw-r--r--  2.0 unx      881 b- defN 23-Jun-22 17:26 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Jun-23 10:40 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3668 b- defN 23-Jun-23 01:05 model_navigator/exceptions.py
+-rw-r--r--  2.0 unx     9474 b- defN 23-Jun-23 01:05 model_navigator/execution_context.py
+-rw-r--r--  2.0 unx     4790 b- defN 23-Jun-23 01:05 model_navigator/logger.py
+-rw-rw-rw-  2.0 unx     1716 b- defN 23-Jun-23 10:40 model_navigator/api/__init__.py
+-rw-rw-rw-  2.0 unx    24304 b- defN 23-Jun-23 10:40 model_navigator/api/config.py
+-rw-rw-rw-  2.0 unx     6425 b- defN 23-Jun-23 10:40 model_navigator/api/jax.py
+-rw-rw-rw-  2.0 unx     5423 b- defN 23-Jun-23 10:40 model_navigator/api/onnx.py
+-rw-rw-rw-  2.0 unx    11860 b- defN 23-Jun-23 10:40 model_navigator/api/package.py
+-rw-rw-rw-  2.0 unx     4906 b- defN 23-Jun-23 10:40 model_navigator/api/python.py
+-rw-rw-rw-  2.0 unx     7748 b- defN 23-Jun-23 01:05 model_navigator/api/pytriton.py
+-rw-rw-rw-  2.0 unx     6519 b- defN 23-Jun-23 10:40 model_navigator/api/tensorflow.py
+-rw-rw-rw-  2.0 unx     6325 b- defN 23-Jun-23 10:40 model_navigator/api/torch.py
+-rw-r--r--  2.0 unx     1553 b- defN 23-Jun-22 17:26 model_navigator/api/triton.py
+-rw-r--r--  2.0 unx     1811 b- defN 23-Jun-22 17:26 model_navigator/api/utilities.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/__init__.py
+-rw-rw-rw-  2.0 unx     4938 b- defN 23-Jun-23 01:05 model_navigator/commands/base.py
+-rw-rw-rw-  2.0 unx    10065 b- defN 23-Jun-23 10:40 model_navigator/commands/infer_metadata.py
+-rw-rw-rw-  2.0 unx     3289 b- defN 23-Jun-23 01:05 model_navigator/commands/load.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/__init__.py
+-rw-rw-rw-  2.0 unx     9863 b- defN 23-Jun-23 01:05 model_navigator/commands/convert/base.py
+-rw-rw-rw-  2.0 unx     7489 b- defN 23-Jun-23 10:40 model_navigator/commands/convert/tf.py
+-rw-rw-rw-  2.0 unx     9879 b- defN 23-Jun-23 10:40 model_navigator/commands/convert/torch.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/__init__.py
+-rw-r--r--  2.0 unx     3418 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-r--r--  2.0 unx     4992 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-r--r--  2.0 unx      680 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/onnx/__init__.py
+-rw-r--r--  2.0 unx     1727 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    10643 b- defN 23-Jun-23 10:40 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-r--r--  2.0 unx     2235 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/copy/__init__.py
+-rw-rw-rw-  2.0 unx     1729 b- defN 23-Jun-23 01:05 model_navigator/commands/copy/onnx.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Jun-22 17:26 model_navigator/commands/correctness/__init__.py
+-rw-rw-rw-  2.0 unx     5594 b- defN 23-Jun-23 01:05 model_navigator/commands/correctness/correctness.py
+-rw-rw-rw-  2.0 unx     4550 b- defN 23-Jun-23 01:05 model_navigator/commands/correctness/correctness_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/data_dump/__init__.py
+-rw-rw-rw-  2.0 unx    11162 b- defN 23-Jun-23 10:40 model_navigator/commands/data_dump/samples.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/export/__init__.py
+-rw-rw-rw-  2.0 unx     3531 b- defN 23-Jun-23 01:05 model_navigator/commands/export/jax.py
+-rw-rw-rw-  2.0 unx     5485 b- defN 23-Jun-23 01:05 model_navigator/commands/export/tf.py
+-rw-rw-rw-  2.0 unx     9043 b- defN 23-Jun-23 01:05 model_navigator/commands/export/torch.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/__init__.py
+-rw-r--r--  2.0 unx     3945 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-r--r--  2.0 unx     3122 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-r--r--  2.0 unx     2728 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-22 17:26 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-rw-rw-  2.0 unx     6396 b- defN 23-Jun-23 10:40 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-rw-rw-  2.0 unx     2984 b- defN 23-Jun-23 10:40 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-rw-rw-  2.0 unx      688 b- defN 23-Jun-23 01:05 model_navigator/commands/performance/__init__.py
+-rw-rw-rw-  2.0 unx    15770 b- defN 23-Jun-23 10:40 model_navigator/commands/performance/performance.py
+-rw-rw-rw-  2.0 unx     3037 b- defN 23-Jun-23 10:40 model_navigator/commands/performance/performance_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/verification/__init__.py
+-rw-rw-rw-  2.0 unx     5441 b- defN 23-Jun-23 01:05 model_navigator/commands/verification/verify.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/configuration/__init__.py
+-rw-rw-rw-  2.0 unx     2473 b- defN 23-Jun-23 10:40 model_navigator/configuration/common_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/configuration/model/__init__.py
+-rw-rw-rw-  2.0 unx    15623 b- defN 23-Jun-23 01:05 model_navigator/configuration/model/model_config.py
+-rw-r--r--  2.0 unx    13677 b- defN 23-Jun-22 17:26 model_navigator/configuration/model/model_config_builder.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/core/__init__.py
+-rw-rw-rw-  2.0 unx     1326 b- defN 23-Jun-23 10:40 model_navigator/core/constants.py
+-rw-rw-rw-  2.0 unx    20111 b- defN 23-Jun-23 10:40 model_navigator/core/package.py
+-rw-rw-rw-  2.0 unx    20337 b- defN 23-Jun-23 10:40 model_navigator/core/status.py
+-rw-rw-rw-  2.0 unx     8052 b- defN 23-Jun-23 10:40 model_navigator/core/tensor.py
+-rw-r--r--  2.0 unx     2817 b- defN 23-Jun-22 17:26 model_navigator/frameworks/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Jun-22 17:26 model_navigator/frameworks/jax/__init__.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jun-22 17:26 model_navigator/frameworks/jax/model.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/frameworks/onnx/__init__.py
+-rw-r--r--  2.0 unx     1085 b- defN 23-Jun-22 17:26 model_navigator/frameworks/onnx/utils.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/frameworks/tensorrt/__init__.py
+-rw-rw-rw-  2.0 unx    26575 b- defN 23-Jun-23 10:40 model_navigator/frameworks/tensorrt/cuda.py
+-rw-rw-rw-  2.0 unx     9874 b- defN 23-Jun-23 10:40 model_navigator/frameworks/tensorrt/utils.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/frameworks/torch/__init__.py
+-rw-rw-rw-  2.0 unx     1508 b- defN 23-Jun-23 01:05 model_navigator/frameworks/torch/utils.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/pipelines/__init__.py
+-rw-rw-rw-  2.0 unx     5685 b- defN 23-Jun-23 01:05 model_navigator/pipelines/pipeline.py
+-rw-rw-rw-  2.0 unx     7333 b- defN 23-Jun-23 01:05 model_navigator/pipelines/pipeline_manager.py
+-rw-rw-rw-  2.0 unx     9805 b- defN 23-Jun-23 10:40 model_navigator/pipelines/validation.py
+-rw-rw-rw-  2.0 unx     1879 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/__init__.py
+-rw-rw-rw-  2.0 unx     2036 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/correctness.py
+-rw-rw-rw-  2.0 unx     5703 b- defN 23-Jun-23 10:40 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-rw-rw-  2.0 unx     1647 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2483 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/onnx.py
+-rw-rw-rw-  2.0 unx     2365 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/preprocessing.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/profiling.py
+-rw-rw-rw-  2.0 unx     2869 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/tensorflow.py
+-rw-rw-rw-  2.0 unx     3261 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/torch.py
+-rw-rw-rw-  2.0 unx     2042 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/verify.py
+-rw-r--r--  2.0 unx     1584 b- defN 23-Jun-22 17:26 model_navigator/runners/__init__.py
+-rw-rw-rw-  2.0 unx    11369 b- defN 23-Jun-23 10:40 model_navigator/runners/base.py
+-rw-r--r--  2.0 unx     2620 b- defN 23-Jun-22 17:26 model_navigator/runners/jax.py
+-rw-rw-rw-  2.0 unx     7302 b- defN 23-Jun-23 10:40 model_navigator/runners/onnx.py
+-rw-r--r--  2.0 unx     2267 b- defN 23-Jun-22 17:26 model_navigator/runners/python.py
+-rw-rw-rw-  2.0 unx     2285 b- defN 23-Jun-23 01:05 model_navigator/runners/registry.py
+-rw-r--r--  2.0 unx     7976 b- defN 23-Jun-22 17:26 model_navigator/runners/tensorflow.py
+-rw-rw-rw-  2.0 unx    25301 b- defN 23-Jun-23 10:40 model_navigator/runners/tensorrt.py
+-rw-rw-rw-  2.0 unx     7699 b- defN 23-Jun-23 10:40 model_navigator/runners/torch.py
+-rw-rw-rw-  2.0 unx     3554 b- defN 23-Jun-23 01:05 model_navigator/runners/utils.py
+-rw-r--r--  2.0 unx      937 b- defN 23-Jun-22 17:26 model_navigator/runtime_analyzer/__init__.py
+-rw-rw-rw-  2.0 unx    11706 b- defN 23-Jun-23 01:05 model_navigator/runtime_analyzer/analyzer.py
+-rw-r--r--  2.0 unx     2304 b- defN 23-Jun-22 17:26 model_navigator/runtime_analyzer/strategy.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/triton/__init__.py
+-rw-r--r--  2.0 unx     3180 b- defN 23-Jun-22 17:26 model_navigator/triton/model_config.py
+-rw-r--r--  2.0 unx     5218 b- defN 23-Jun-22 17:26 model_navigator/triton/model_config_builder.py
+-rw-r--r--  2.0 unx    23090 b- defN 23-Jun-22 17:26 model_navigator/triton/model_config_generator.py
+-rw-rw-rw-  2.0 unx    15245 b- defN 23-Jun-23 10:40 model_navigator/triton/model_repository.py
+-rw-r--r--  2.0 unx     2081 b- defN 23-Jun-22 17:26 model_navigator/triton/utils.py
+-rw-r--r--  2.0 unx      944 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/__init__.py
+-rw-r--r--  2.0 unx     2872 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-r--r--  2.0 unx    22326 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/common.py
+-rw-r--r--  2.0 unx     2229 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/internal.py
+-rw-r--r--  2.0 unx     2685 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-r--r--  2.0 unx     3162 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/utils/__init__.py
+-rw-rw-rw-  2.0 unx    14113 b- defN 23-Jun-23 10:40 model_navigator/utils/common.py
+-rw-rw-rw-  2.0 unx     8004 b- defN 23-Jun-23 10:40 model_navigator/utils/dataloader.py
+-rw-r--r--  2.0 unx     3902 b- defN 23-Jun-22 17:26 model_navigator/utils/devices.py
+-rw-r--r--  2.0 unx     1308 b- defN 23-Jun-22 17:26 model_navigator/utils/enums.py
+-rw-r--r--  2.0 unx     6163 b- defN 23-Jun-22 17:26 model_navigator/utils/environment.py
+-rw-rw-rw-  2.0 unx     3528 b- defN 23-Jun-23 01:05 model_navigator/utils/format_helpers.py
+-rw-rw-rw-  2.0 unx     2325 b- defN 23-Jun-23 01:05 model_navigator/utils/module.py
+-rw-rw-rw-  2.0 unx     3233 b- defN 23-Jun-23 01:05 model_navigator/utils/package.py
+-rw-r--r--  2.0 unx    10140 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12074 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    13271 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/RECORD
+133 files, 704952 bytes uncompressed, 212626 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -378,23 +378,23 @@
 
 Filename: model_navigator/utils/module.py
 Comment: 
 
 Filename: model_navigator/utils/package.py
 Comment: 
 
-Filename: triton_model_navigator-0.5.5.dist-info/LICENSE
+Filename: triton_model_navigator-0.5.6.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.5.5.dist-info/METADATA
+Filename: triton_model_navigator-0.5.6.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.5.5.dist-info/WHEEL
+Filename: triton_model_navigator-0.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.5.5.dist-info/top_level.txt
+Filename: triton_model_navigator-0.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.5.5.dist-info/RECORD
+Filename: triton_model_navigator-0.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D100
-__version__ = "0.5.5"
+__version__ = "0.5.6"
```

## model_navigator/commands/convert/tf.py

```diff
@@ -49,17 +49,15 @@
             CommandOutput: Conversion output.
         """
         LOGGER.info("SavedModel to ONNX conversion started")
 
         exported_model_path = workspace / parent_path
         converted_model_path = workspace / path
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
-        if converted_model_path.exists():
-            LOGGER.info("Model already exists. Skipping conversion.")
-            return CommandOutput(status=CommandStatus.SKIPPED)
+
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported SavedModel model not found at {exported_model_path}. Skipping conversion")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         convert_cmd = [
             "python",
             "-m",
@@ -128,17 +126,14 @@
         if not devices.get_available_gpus():
             raise RuntimeError("No GPUs available.")
 
         exported_model_path = workspace / parent_path
         converted_model_path = workspace / path
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
-        if converted_model_path.exists():
-            LOGGER.info("Model already exists. Skipping conversion.")
-            return CommandOutput(status=CommandStatus.SKIPPED)
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported SavedModel model not found at {exported_model_path}. Skipping conversion")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         custom_trt_profile = trt_profile
         trt_profile = self._get_trt_profile(
             dataloader_trt_profile=dataloader_trt_profile, custom_trt_profile=custom_trt_profile
```

## model_navigator/commands/convert/torch.py

```diff
@@ -61,18 +61,14 @@
 
         Returns:
             CommandOutput: Status OK.
         """
         LOGGER.info("TorchScript to ONNX conversion started")
         exported_model_path = workspace / parent_path
         converted_model_path = workspace / path
-        if converted_model_path.exists():
-            LOGGER.info("Model already exists. Skipping export.")
-            return CommandOutput(status=CommandStatus.SKIPPED)
-
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         with ExecutionContext(
             workspace=workspace,
             script_path=converted_model_path.parent / "reproduce_conversion.py",
             cmd_path=converted_model_path.parent / "reproduce_conversion.sh",
             verbose=verbose,
@@ -116,15 +112,15 @@
         batch_dim: Optional[int] = None,
         dataloader_max_batch_size: Optional[int] = None,
         device_max_batch_size: Optional[int] = None,
         trt_profile: Optional[TensorRTProfile] = None,
     ) -> CommandOutput:
         """Run Torchscript ot Torch-TensorRT conversion.
 
-        For detaild explenation of TensorRT parameters please refer to [documentation]
+        For detailed explanation of TensorRT parameters please refer to [documentation]
         [documentation]: https://pytorch.org/TensorRT/
 
         Args:
             workspace (Path): Model Navigator workspace path.
             path (Path): Output Torch-TensorRT model path relative to workspace path.
             parent_path (Path): TorchScript model path relative to workspace path.
             precision (TensorRTPrecision): TensorRTPrecision.
@@ -150,17 +146,15 @@
             CommandOutput: Status OK.
         """
         LOGGER.info("Conversion TorchScript to TorchTensorRT started")
         if not devices.get_available_gpus():
             raise RuntimeError("No GPUs available.")
         exported_model_path = workspace / parent_path
         converted_model_path = workspace / path
-        if converted_model_path.exists():
-            LOGGER.info("Model already exists. Skipping conversion.")
-            return CommandOutput(status=CommandStatus.SKIPPED)
+
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported TorchScript model not found at {exported_model_path}. Skipping conversion.")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         custom_trt_profile = trt_profile
         trt_profile = self._get_trt_profile(
             dataloader_trt_profile=dataloader_trt_profile, custom_trt_profile=custom_trt_profile
```

## model_navigator/commands/convert/onnx/onnx2trt.py

```diff
@@ -86,17 +86,14 @@
         """
         LOGGER.info("ONNX to TRT conversion started")
         if not devices.get_available_gpus():
             raise RuntimeError("No GPUs available.")
 
         input_model_path = workspace / parent_path
         converted_model_path = workspace / path
-        if converted_model_path.exists():
-            LOGGER.info("Model already exists. Skipping conversion.")
-            return CommandOutput(status=CommandStatus.SKIPPED)
 
         if not input_model_path.exists():
             LOGGER.warning(f"Exported ONNX model not found at {input_model_path}. Skipping conversion.")
             return CommandOutput(status=CommandStatus.SKIPPED)
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         custom_trt_profile = trt_profile
```

## model_navigator/triton/model_repository.py

```diff
@@ -101,15 +101,15 @@
     TensorFlowTensorRTRunner,
 )
 
 
 def add_model(
     model_repository_path: Union[str, pathlib.Path],
     model_name: str,
-    model_path: pathlib.Path,
+    model_path: Union[str, pathlib.Path],
     config: Union[
         ONNXModelConfig,
         TensorRTModelConfig,
         PyTorchModelConfig,
         PythonModelConfig,
         TensorFlowModelConfig,
     ],
@@ -163,23 +163,23 @@
             model_name=model_name,
             model_version=model_version,
             tensorrt_config=config,
         )
     else:
         raise ModelNavigatorWrongParameterError(f"Unsupported model config provided: {config.__class__}")
 
-    triton_model_repository = _TritonModelRepository(model_repository_path=model_repository_path)
+    triton_model_repository = _TritonModelRepository(model_repository_path=pathlib.Path(model_repository_path))
     return triton_model_repository.deploy_model(
-        model_path=model_path,
+        model_path=pathlib.Path(model_path),
         model_config=model_config,
     )
 
 
 def add_model_from_package(
-    model_repository_path: pathlib.Path,
+    model_repository_path: Union[str, pathlib.Path],
     model_name: str,
     package: Package,
     model_version: int = 1,
     strategy: Optional[RuntimeSearchStrategy] = None,
     response_cache: bool = False,
 ):
     """Create the Triton Model Store with optimized model and save it to `model_repository_path`.
```

## model_navigator/utils/dataloader.py

```diff
@@ -203,15 +203,15 @@
     """
     if isinstance(workspace, str):
         workspace = Path(workspace)
     samples_type = samples_name.split("_")[0]
     samples_dirname = "model_output" if samples_name.split("_")[-1] == "output" else "model_input"
     samples_dirpath = workspace / samples_dirname / samples_type
     samples = []
-    for sample_filepath in samples_dirpath.iterdir():
+    for sample_filepath in sorted(samples_dirpath.iterdir()):
         sample = {}
         with np.load(sample_filepath.as_posix()) as data:
             for k, v in data.items():
                 if batch_dim is not None:
                     v = np.expand_dims(v, batch_dim)
                     # v = numpy.repeat(v, max_batch_size, batch_dim)
                 sample[k] = v
```

## Comparing `triton_model_navigator-0.5.5.dist-info/LICENSE` & `triton_model_navigator-0.5.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.5.5.dist-info/METADATA` & `triton_model_navigator-0.5.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.5.5
+Version: 0.5.6
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `triton_model_navigator-0.5.5.dist-info/RECORD` & `triton_model_navigator-0.5.6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=OER3JOWyTyl2EWNM_d6KFSiH4Mg0S8OMrlQamc54JuA,649
+model_navigator/__version__.py,sha256=OAsic7CwhOApIQYmiIX1VsDMoVwieEfdphmvFQ01s-Y,649
 model_navigator/exceptions.py,sha256=6wR9REQeNkmHOklMPQ46SrGC61EJVH4jz0n2BC4e7ek,3668
 model_navigator/execution_context.py,sha256=eYV2YJU4V8X-v-dWTI6Oi5zJl3RdtK41XWtPxPRxNvU,9474
 model_navigator/logger.py,sha256=946izjz2i81kuehttGIkJ2_NhpNVCgTt6y9fL-s19-U,4790
 model_navigator/api/__init__.py,sha256=ZCychLWYCVP_Q5BWXK7-8FzldMSyFTiGgcT6c_kOnJc,1716
 model_navigator/api/config.py,sha256=MkYyt3XiD37d5ptOOJOvb9HwW-sYKCZetKgCDJfT7lk,24304
 model_navigator/api/jax.py,sha256=eLDXpJsYNhVkquv6bJaO20aXO7aBqWmCGrDd1cvkzDc,6425
 model_navigator/api/onnx.py,sha256=RI9d_-H7_3Q7hkDNSGvQ89jbbbAxS1kLv-8YKlR5Kx0,5423
@@ -16,23 +16,23 @@
 model_navigator/api/utilities.py,sha256=iDAsvY2lFZ1ri54OSmThTVokJ31vCnHoylBHiKkYUNg,1811
 model_navigator/commands/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/base.py,sha256=O75ENxJH4GtjYHru56h5XSLrR_iqnsbaQE7YHbtOnLk,4938
 model_navigator/commands/infer_metadata.py,sha256=uFDHHnadjjOFTjNVSPigBXcZYTD3h9jtPPj8-EtndWc,10065
 model_navigator/commands/load.py,sha256=7v1YqLbG0VZOf981XW-2Y6ad828d4Ynq2HNmj7_a8ys,3289
 model_navigator/commands/convert/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/convert/base.py,sha256=YlFjgaik1oqZr9m8FujYQ-gunFoHXA8dgLScgXTG__E,9863
-model_navigator/commands/convert/tf.py,sha256=tQw4DTmAqzDO0pr7ZPMjzTInmd11qmsNIKW6JsWasNM,7838
-model_navigator/commands/convert/torch.py,sha256=s7l6jNhoG4zoej3EOVbw04MGJ67HIw1XFa58OV_a4Js,10224
+model_navigator/commands/convert/tf.py,sha256=-5YBgVGglo1hLsyjmF7RRrOsEg1jRIfdtpN0Efar9EU,7489
+model_navigator/commands/convert/torch.py,sha256=rWsZDF8Wv-xdv2AyFNGKWbJtNu_-N42j2lHMdb94CE0,9879
 model_navigator/commands/convert/converters/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/convert/converters/sm2tftrt.py,sha256=AcNyKV60yCUrzJ5B501H5SHKjtkr7kaNXNIewnOFJzk,3418
 model_navigator/commands/convert/converters/ts2onnx.py,sha256=ezjlPeHHbhx2LB4HDoLkVlmaZa1dreVMQMk2PL5UMos,3105
 model_navigator/commands/convert/converters/ts2torchtrt.py,sha256=a_mpR0j4y5ClaY6Ik_oIKEAlh45zD-ycCLHigsy1C7M,4992
 model_navigator/commands/convert/onnx/__init__.py,sha256=LwvvDj4oH7rwmUJXVEyRxIOWZnUxix6n_DmkAJzEJBY,680
 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py,sha256=KQR-qrVWVVBGVr5pqcKink2dcDNCk1Lszvl8x6TwqjU,1727
-model_navigator/commands/convert/onnx/onnx2trt.py,sha256=FI-EKl4IP5wz_UTquhNz2xZFoe2BT3EQO_JbW3Klq8g,10818
+model_navigator/commands/convert/onnx/onnx2trt.py,sha256=2dCVmkRhC0jJOANzdjilzXkG3NdDxMx_xXGkRILxJnM,10643
 model_navigator/commands/convert/onnx/trt_load_script.py,sha256=D2fTNNIBELAsBSmy3ij9oxMyRDxi0RNFV29zAlPYFz8,2235
 model_navigator/commands/copy/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/copy/onnx.py,sha256=Z2dtowzXW1qVJq2L4bNNLLRRTbyeiJT7MoIxi4y42fk,1729
 model_navigator/commands/correctness/__init__.py,sha256=Xm-ikcHX6zpdmukjkSgL4JnPt2FIImoxXUPsL-334FM,678
 model_navigator/commands/correctness/correctness.py,sha256=qPBKlBE_wuJTtIJ2tt8zXWjFestp-nDvIn3Zh5T5xsc,5594
 model_navigator/commands/correctness/correctness_script.py,sha256=USxoVaa0flsEjNy-vYxjDTkF5Z-lVSY6Jl6Zv9sqNOA,4550
 model_navigator/commands/data_dump/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
@@ -102,32 +102,32 @@
 model_navigator/runtime_analyzer/__init__.py,sha256=BrhKs-NzpT0ilLmYe38kUtOS7AJ-KfzyV-Hc7ANJWEE,937
 model_navigator/runtime_analyzer/analyzer.py,sha256=Y5vBtEEKPv7Ce1Mg3GV6sxe61zDj_fz7RZD8Ge6NM8s,11706
 model_navigator/runtime_analyzer/strategy.py,sha256=L6dqnf1OS0s5mrBvxTTFgNPghKbuEFC2X_2tMm3_Hs4,2304
 model_navigator/triton/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/triton/model_config.py,sha256=Efcx0_48bmkmBwJgqm6Ejsuwh0ZPnYmyR1o6bz4Y5to,3180
 model_navigator/triton/model_config_builder.py,sha256=4uh5xArtOMnyzIKO2Duliz9SRltrP5El2xPqzE1At_0,5218
 model_navigator/triton/model_config_generator.py,sha256=i45y9ezQJ9xcQmNcGHW_5r0TZ7-Ikxvmzb9pgfBlZaY,23090
-model_navigator/triton/model_repository.py,sha256=5hxutEQg0VFP2tgdTiXqSQC-VxvaK-9Fo-5Ot1e83UY,15193
+model_navigator/triton/model_repository.py,sha256=z_9SWYHGqO7a-FP3nkP2vfQgZN6v2Lwwgvqmc-1l2eg,15245
 model_navigator/triton/utils.py,sha256=uJeGyzMSvxZj2hyUAC3bTk0cuMcKTYeCKAi7zerP3hA,2081
 model_navigator/triton/specialized_configs/__init__.py,sha256=lcQy-49A74vMSidK-avYy6xdX4p3OG3ygzSw6y9-OQw,944
 model_navigator/triton/specialized_configs/base_model_config.py,sha256=UOeuce-xT9lC3Zv3H3BbdSem7cTNyn7boKybxChzRgs,2872
 model_navigator/triton/specialized_configs/common.py,sha256=l6FPhZTU1WQHDVXG8HxEXx2c8s87EWgYUvtQrxqUH1k,22326
 model_navigator/triton/specialized_configs/internal.py,sha256=R42XlgUEOC5B-WotI_dAQs8sQyHJOnVyTvVk3CaZ6kM,2229
 model_navigator/triton/specialized_configs/onnx_model_config.py,sha256=oN76Ux7JI4eqlarlEVSSiIbbajAqdrF3bW0n6WQBPPw,2685
 model_navigator/triton/specialized_configs/python_model_config.py,sha256=NGijgogtoJnbBLL1hQqhw-n4rBo_OgFsCdn9ezw24VI,1785
 model_navigator/triton/specialized_configs/pytorch_model_config.py,sha256=GxJnFB4UpnUwB75t09d5XZ2iqeMZM1SmTbGe2aqmph8,2239
 model_navigator/triton/specialized_configs/tensorflow_model_config.py,sha256=C_qMi-5TAWTSL_wBDIoJju3gHRHX10RBbHvBE9of780,3162
 model_navigator/triton/specialized_configs/tensorrt_model_config.py,sha256=ikNi_i_cPjL2Mhea1uJHXe3KElvpHkiPH_zXK895pQU,3040
 model_navigator/utils/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/utils/common.py,sha256=AHqkU5xRTR6OFFq0T-UNWCQ9AoMkVdjxnyVGVhuecsw,14113
-model_navigator/utils/dataloader.py,sha256=_fxjq2vP4DNFxOEZA_HPX_8caQcbSwgP55gdey9rq-M,7996
+model_navigator/utils/dataloader.py,sha256=pOXC63nRpSqUMhTh-Rr7VOSE7ohwwafXbKAcY-OfMM0,8004
 model_navigator/utils/devices.py,sha256=pGjRBByJqFjG6dyJ0H2E6GJA7hIgF6rgeINLNdS27kU,3902
 model_navigator/utils/enums.py,sha256=T-G5VV5CqimxpctOqPaCvVoAwx-pp10Eeo0rKlWoVGU,1308
 model_navigator/utils/environment.py,sha256=MnpdF5eCx2DJpHtaq8fUSky0hdT03qTJrGnJDhCnFhM,6163
 model_navigator/utils/format_helpers.py,sha256=VAbRMfBw-eZljk_yDcV6Q1ojkl8ah1OnqZR6DshXNqU,3528
 model_navigator/utils/module.py,sha256=fkokQmxhWgShqrhsXDPa-g-jBA0XaUQvuVuM74WPOIM,2325
 model_navigator/utils/package.py,sha256=wp1xOwrKuB_rtVfe61y2AznmA-up320RtHNNV2UExe4,3233
-triton_model_navigator-0.5.5.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.5.5.dist-info/METADATA,sha256=-q2kbOGb5fXNXyHKmRT0vEHy3ihlW97_-UUMeApvLys,12074
-triton_model_navigator-0.5.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.5.5.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.5.5.dist-info/RECORD,,
+triton_model_navigator-0.5.6.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.5.6.dist-info/METADATA,sha256=b71-boQKxHg9IE_sQiYu47g8cYK1Wrc5OB3ZV2t3LN4,12074
+triton_model_navigator-0.5.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+triton_model_navigator-0.5.6.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.5.6.dist-info/RECORD,,
```

