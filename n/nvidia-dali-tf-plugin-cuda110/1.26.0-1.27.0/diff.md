# Comparing `tmp/nvidia-dali-tf-plugin-cuda110-1.26.0.tar.gz` & `tmp/nvidia-dali-tf-plugin-cuda110-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-cuda110-1.26.0.tar", last modified: Fri May 12 16:29:46 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-cuda110-1.27.0.tar", last modified: Tue Jun 13 09:35:47 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0.tar` & `nvidia-dali-tf-plugin-cuda110-1.27.0.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2735 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    43001 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_dataset_op.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/
--rw-r--r--   0 root         (0) root         (0)     5169 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_dataset.h
--rw-r--r--   0 root         (0) root         (0)     7079 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_helper.h
--rw-r--r--   0 root         (0) root         (0)    17344 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_install_tool.py
--rw-r--r--   0 root         (0) root         (0)     6207 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_utils.py
--rw-r--r--   0 root         (0) root         (0)    17543 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/daliop.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/
--rw-r--r--   0 root         (0) root         (0)    27259 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/c_api.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.092265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/
--rw-r--r--   0 root         (0) root         (0)     5686 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/access_order.h
--rw-r--r--   0 root         (0) root         (0)    10320 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/any.h
--rw-r--r--   0 root         (0) root         (0)     1461 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/api_helper.h
--rw-r--r--   0 root         (0) root         (0)     2207 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/backend_tags.h
--rw-r--r--   0 root         (0) root         (0)     7777 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/bitmask.h
--rw-r--r--   0 root         (0) root         (0)     7937 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/boundary.h
--rw-r--r--   0 root         (0) root         (0)     3297 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/byte_io.h
--rw-r--r--   0 root         (0) root         (0)     1281 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/call_at_exit.h
--rw-r--r--   0 root         (0) root         (0)     5354 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/common.h
--rw-r--r--   0 root         (0) root         (0)    17542 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/convert.h
--rw-r--r--   0 root         (0) root         (0)     2428 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/copy_vector_helper.h
--rw-r--r--   0 root         (0) root         (0)     5249 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_error.h
--rw-r--r--   0 root         (0) root         (0)     1895 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event.h
--rw-r--r--   0 root         (0) root         (0)     3154 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event_pool.h
--rw-r--r--   0 root         (0) root         (0)     2460 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_rt_utils.h
--rw-r--r--   0 root         (0) root         (0)     2059 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream.h
--rw-r--r--   0 root         (0) root         (0)     7050 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream_pool.h
--rw-r--r--   0 root         (0) root         (0)     2179 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_utils.h
--rw-r--r--   0 root         (0) root         (0)     5012 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_array.h
--rw-r--r--   0 root         (0) root         (0)     5315 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_buffer.h
--rw-r--r--   0 root         (0) root         (0)     6438 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_string.h
--rw-r--r--   0 root         (0) root         (0)     1381 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/device_guard.h
--rw-r--r--   0 root         (0) root         (0)      815 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cuda.h
--rw-r--r--   0 root         (0) root         (0)     5034 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cufile.h
--rw-r--r--   0 root         (0) root         (0)     6146 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/endian_util.h
--rw-r--r--   0 root         (0) root         (0)    10891 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/error_handling.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.092265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/exec/
--rw-r--r--   0 root         (0) root         (0)     2115 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/exec/engine.h
--rw-r--r--   0 root         (0) root         (0)     4648 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/expand_dims.h
--rw-r--r--   0 root         (0) root         (0)     6831 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/fast_div.h
--rw-r--r--   0 root         (0) root         (0)    14461 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/float16.h
--rw-r--r--   0 root         (0) root         (0)      977 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/force_inline.h
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/format.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.092265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/box.h
--rw-r--r--   0 root         (0) root         (0)     1706 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/geom_utils.h
--rw-r--r--   0 root         (0) root         (0)    17992 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/mat.h
--rw-r--r--   0 root         (0) root         (0)     4521 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/transform.h
--rw-r--r--   0 root         (0) root         (0)    21114 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/vec.h
--rw-r--r--   0 root         (0) root         (0)     1160 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/host_dev.h
--rw-r--r--   0 root         (0) root         (0)     2267 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/int_literals.h
--rw-r--r--   0 root         (0) root         (0)     5889 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/math_util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/
--rw-r--r--   0 root         (0) root         (0)    22047 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/async_pool.h
--rw-r--r--   0 root         (0) root         (0)     5291 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/composite_resource.h
--rw-r--r--   0 root         (0) root         (0)     9018 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cu_vm.h
--rw-r--r--   0 root         (0) root         (0)    27092 2023-05-09 19:27:36.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cuda_vm_resource.h
--rw-r--r--   0 root         (0) root         (0)     5267 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/default_resources.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/
--rw-r--r--   0 root         (0) root         (0)     3850 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/align.h
--rw-r--r--   0 root         (0) root         (0)     6541 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_alloc.h
--rw-r--r--   0 root         (0) root         (0)     1426 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_collections.h
--rw-r--r--   0 root         (0) root         (0)    25585 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/free_list.h
--rw-r--r--   0 root         (0) root         (0)     2332 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/util.h
--rw-r--r--   0 root         (0) root         (0)     2934 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/fixed_order_resource.h
--rw-r--r--   0 root         (0) root         (0)     6580 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/malloc_resource.h
--rw-r--r--   0 root         (0) root         (0)    22782 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory.h
--rw-r--r--   0 root         (0) root         (0)     2057 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_kind.h
--rw-r--r--   0 root         (0) root         (0)     2278 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_resource.h
--rw-r--r--   0 root         (0) root         (0)     9348 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/monotonic_resource.h
--rw-r--r--   0 root         (0) root         (0)    11682 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource.h
--rw-r--r--   0 root         (0) root         (0)     1084 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource_base.h
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/with_upstream.h
--rw-r--r--   0 root         (0) root         (0)     3169 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/nvtx.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/os/
--rw-r--r--   0 root         (0) root         (0)     5420 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/os/shared_mem.h
--rw-r--r--   0 root         (0) root         (0)     4677 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/partition.h
--rw-r--r--   0 root         (0) root         (0)    10461 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/per_stream_pool.h
--rw-r--r--   0 root         (0) root         (0)     3288 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/permute.h
--rw-r--r--   0 root         (0) root         (0)     2337 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/python_util.h
--rw-r--r--   0 root         (0) root         (0)     3283 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/random.h
--rw-r--r--   0 root         (0) root         (0)    19482 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/small_vector.h
--rw-r--r--   0 root         (0) root         (0)     9394 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/span.h
--rw-r--r--   0 root         (0) root         (0)     1902 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/spinlock.h
--rw-r--r--   0 root         (0) root         (0)     5372 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_map.h
--rw-r--r--   0 root         (0) root         (0)     6547 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_switch.h
--rw-r--r--   0 root         (0) root         (0)     5872 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/stream.h
--rw-r--r--   0 root         (0) root         (0)    18748 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_layout.h
--rw-r--r--   0 root         (0) root         (0)    54963 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape.h
--rw-r--r--   0 root         (0) root         (0)     1617 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape_print.h
--rw-r--r--   0 root         (0) root         (0)    33471 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_view.h
--rw-r--r--   0 root         (0) root         (0)     2403 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/traits.h
--rw-r--r--   0 root         (0) root         (0)     8062 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tuple_helpers.h
--rw-r--r--   0 root         (0) root         (0)     5479 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/unique_handle.h
--rw-r--r--   0 root         (0) root         (0)    13956 2023-04-27 19:33:13.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/util.h
--rw-r--r--   0 root         (0) root         (0)     1655 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/version_util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/
--rw-r--r--   0 root         (0) root         (0)     5734 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/decode_results.h
--rw-r--r--   0 root         (0) root         (0)     8884 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder.h
--rw-r--r--   0 root         (0) root         (0)     8845 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder_interfaces.h
--rw-r--r--   0 root         (0) root         (0)     4098 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_format.h
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_orientation.h
--rw-r--r--   0 root         (0) root         (0)     5546 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_source.h
--rw-r--r--   0 root         (0) root         (0)     1992 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/operators.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/
--rw-r--r--   0 root         (0) root         (0)   256667 2023-04-24 07:02:14.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/Acknowledgements.txt
--rw-r--r--   0 root         (0) root         (0)      621 2023-04-24 07:02:14.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/COPYRIGHT
--rw-r--r--   0 root         (0) root         (0)    10142 2023-04-24 07:02:14.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      690 2023-05-12 16:29:45.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/dali_tf_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2735 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3985 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/
--rw-r--r--   0 root         (0) root         (0)   206632 2023-05-12 16:29:42.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_11.so
--rw-r--r--   0 root         (0) root         (0)   206896 2023-05-12 16:29:42.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_12.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/stub/
--rw-r--r--   0 root         (0) root         (0)    13800 2023-05-12 16:29:42.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/stub/libdali.so
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4409 2023-05-12 16:29:45.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-04-24 07:05:38.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/stubgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    43001 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_dataset_op.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.486541 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/
+-rw-r--r--   0 root         (0) root         (0)     5169 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_dataset.h
+-rw-r--r--   0 root         (0) root         (0)     7079 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_helper.h
+-rw-r--r--   0 root         (0) root         (0)    17344 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_install_tool.py
+-rw-r--r--   0 root         (0) root         (0)     6207 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17543 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/daliop.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.482541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.486541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/
+-rw-r--r--   0 root         (0) root         (0)    27259 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/c_api.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.490541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/
+-rw-r--r--   0 root         (0) root         (0)     5686 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/access_order.h
+-rw-r--r--   0 root         (0) root         (0)    10320 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/any.h
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/api_helper.h
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/backend_tags.h
+-rw-r--r--   0 root         (0) root         (0)     7777 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/bitmask.h
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/boundary.h
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/byte_io.h
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/call_at_exit.h
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/common.h
+-rw-r--r--   0 root         (0) root         (0)    17542 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/convert.h
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/copy_vector_helper.h
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_error.h
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event.h
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event_pool.h
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_rt_utils.h
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream.h
+-rw-r--r--   0 root         (0) root         (0)     7050 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream_pool.h
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_utils.h
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_array.h
+-rw-r--r--   0 root         (0) root         (0)     5315 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_string.h
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/device_guard.h
+-rw-r--r--   0 root         (0) root         (0)      815 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cuda.h
+-rw-r--r--   0 root         (0) root         (0)     5034 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cufile.h
+-rw-r--r--   0 root         (0) root         (0)     6146 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/endian_util.h
+-rw-r--r--   0 root         (0) root         (0)    10891 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/error_handling.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.490541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/exec/
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/exec/engine.h
+-rw-r--r--   0 root         (0) root         (0)     4648 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/expand_dims.h
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/fast_div.h
+-rw-r--r--   0 root         (0) root         (0)    14461 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/float16.h
+-rw-r--r--   0 root         (0) root         (0)      977 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/force_inline.h
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/format.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/box.h
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/geom_utils.h
+-rw-r--r--   0 root         (0) root         (0)    17992 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/mat.h
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/transform.h
+-rw-r--r--   0 root         (0) root         (0)    21114 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/vec.h
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/host_dev.h
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/int_literals.h
+-rw-r--r--   0 root         (0) root         (0)     5889 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/math_util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/
+-rw-r--r--   0 root         (0) root         (0)    22129 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/async_pool.h
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/binning_resource.h
+-rw-r--r--   0 root         (0) root         (0)     5291 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/composite_resource.h
+-rw-r--r--   0 root         (0) root         (0)     9018 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cu_vm.h
+-rw-r--r--   0 root         (0) root         (0)    34893 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cuda_vm_resource.h
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/default_resources.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/align.h
+-rw-r--r--   0 root         (0) root         (0)     6541 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_alloc.h
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_collections.h
+-rw-r--r--   0 root         (0) root         (0)    25585 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/free_list.h
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/util.h
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/fixed_order_resource.h
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/malloc_resource.h
+-rw-r--r--   0 root         (0) root         (0)    22782 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory.h
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_kind.h
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_resource.h
+-rw-r--r--   0 root         (0) root         (0)     9348 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/monotonic_resource.h
+-rw-r--r--   0 root         (0) root         (0)    11682 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource.h
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource_base.h
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/with_upstream.h
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/nvtx.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/os/
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/os/shared_mem.h
+-rw-r--r--   0 root         (0) root         (0)     4677 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/partition.h
+-rw-r--r--   0 root         (0) root         (0)    10461 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/per_stream_pool.h
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/permute.h
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/python_util.h
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/random.h
+-rw-r--r--   0 root         (0) root         (0)    19482 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/small_vector.h
+-rw-r--r--   0 root         (0) root         (0)     9394 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/span.h
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/spinlock.h
+-rw-r--r--   0 root         (0) root         (0)     5372 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_map.h
+-rw-r--r--   0 root         (0) root         (0)     6547 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_switch.h
+-rw-r--r--   0 root         (0) root         (0)     5872 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/stream.h
+-rw-r--r--   0 root         (0) root         (0)    18748 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_layout.h
+-rw-r--r--   0 root         (0) root         (0)    54963 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape.h
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape_print.h
+-rw-r--r--   0 root         (0) root         (0)    33471 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_view.h
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/traits.h
+-rw-r--r--   0 root         (0) root         (0)     8062 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tuple_helpers.h
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-06-13 07:30:32.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/unique_handle.h
+-rw-r--r--   0 root         (0) root         (0)    13956 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/util.h
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/version_util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.494541 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/decode_results.h
+-rw-r--r--   0 root         (0) root         (0)     8884 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder.h
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder_interfaces.h
+-rw-r--r--   0 root         (0) root         (0)     4098 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_format.h
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_orientation.h
+-rw-r--r--   0 root         (0) root         (0)     5546 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_source.h
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/operators.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.482541 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/
+-rw-r--r--   0 root         (0) root         (0)   256667 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/Acknowledgements.txt
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/COPYRIGHT
+-rw-r--r--   0 root         (0) root         (0)    10142 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      690 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-06-12 11:00:14.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/dali_tf_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4027 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/
+-rw-r--r--   0 root         (0) root         (0)   206632 2023-06-13 09:35:40.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_11.so
+-rw-r--r--   0 root         (0) root         (0)   206896 2023-06-13 09:35:40.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_12.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/stub/
+-rw-r--r--   0 root         (0) root         (0)    13800 2023-06-13 09:35:40.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/stub/libdali.so
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 09:35:47.498541 nvidia-dali-tf-plugin-cuda110-1.27.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4409 2023-06-13 09:35:47.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-12 11:00:15.000000 nvidia-dali-tf-plugin-cuda110-1.27.0/stubgen.py
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/PKG-INFO` & `nvidia-dali-tf-plugin-cuda110-1.27.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-cuda110
-Version: 1.26.0
-Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: cdc39704b8f824f342e0e0c9163ba12518434987
+Version: 1.27.0
+Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 4cc38a6b48a74cc06fe8594b6e5c18ae090dc045
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Description: TensorFlow plugin for NVIDIA DALI
         =================================
         
         The TensorFlow plugin enables usage of DALI with TensorFlow.
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_dataset_op.cc` & `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_dataset_op.cc`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_dataset.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_dataset.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin/dali_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_install_tool.py` & `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_install_tool.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_utils.py` & `nvidia-dali-tf-plugin-cuda110-1.27.0/dali_tf_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/daliop.cc` & `nvidia-dali-tf-plugin-cuda110-1.27.0/daliop.cc`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/c_api.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/c_api.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/access_order.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/access_order.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/any.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/any.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/api_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/api_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/backend_tags.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/backend_tags.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/bitmask.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/bitmask.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/boundary.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/boundary.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/byte_io.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/byte_io.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/call_at_exit.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/call_at_exit.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/common.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/common.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/convert.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/convert.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/copy_vector_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/copy_vector_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_error.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_error.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_event_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_rt_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_rt_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_stream_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_array.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_array.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_buffer.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_buffer.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_string.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dev_string.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/device_guard.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/device_guard.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cuda.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cuda.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cufile.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/dynlink_cufile.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/endian_util.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/endian_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/error_handling.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/error_handling.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/exec/engine.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/exec/engine.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/expand_dims.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/expand_dims.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/fast_div.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/fast_div.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/float16.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/float16.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/force_inline.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/force_inline.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/format.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/format.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/box.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/box.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/geom_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/geom_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/mat.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/mat.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/transform.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/transform.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/vec.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/geom/vec.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/host_dev.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/host_dev.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/int_literals.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/int_literals.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/math_util.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/math_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/async_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/async_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -373,32 +373,33 @@
         if (!supports_splitting && block_size - bytes - front_padding > max_padding)
           return nullptr;  // no point in continuing - the map is sorted
 
         from.by_size.erase(it);
         char *block_end = base + block_size;
         char *remainder = detail::align_ptr(aligned + bytes, remainder_alignment);
         bool split = supports_splitting && remainder + min_split_remainder < block_end;
+        size_t orig_alignment = f->alignment;
         size_t split_size = block_size;
         if (split) {
           // Adjust the pending free `f` so that it contains only what remains after
           // the block was split.
           size_t remainder_size = block_end - remainder;
           f->addr = remainder;
           f->bytes = remainder_size;
           f->alignment = remainder_alignment;
           from.by_size.insert({ remainder_size, f });
           // The block taken out from the free list is now reduced
           split_size = remainder - base;
         } else {
           remove_pending_free(from, f, false);
         }
-        if (split_size != bytes) {
+        if (split_size != bytes || alignment != orig_alignment) {
           padded_[aligned] = { split_size,
                                static_cast<int>(front_padding),
-                               static_cast<int>(alignment) };
+                               static_cast<int>(orig_alignment) };
         }
         return aligned;
       }
     }
     return nullptr;
   }
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/composite_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/composite_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cu_vm.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cu_vm.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cuda_vm_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/cuda_vm_resource.h`

 * *Files 15% similar despite different names*

```diff
@@ -73,15 +73,18 @@
     }
     return ptr;
   }
 
   struct Stat {
     int allocated_blocks;
     int peak_allocated_blocks;
+    int va_ranges;
+    int peak_va_ranges;
     size_t allocated_va;
+    size_t peak_va;
     size_t curr_allocated;
     size_t peak_allocated;
     size_t curr_free;
     size_t curr_allocations;
     size_t peak_allocations;
     size_t total_allocations;
     size_t total_deallocations;
@@ -105,23 +108,27 @@
     lock_guard pool_guard(pool_lock_);
     stat_ = {};
   }
 
   void dump_stats(std::ostream &os) {
     print(os, "cuda_vm_resource stat dump:",
       "\ntotal VM size:         ", stat_.allocated_va,
+      "\npeak VM size:          ", stat_.peak_va,
+      "\n# VM ranges:           ", stat_.va_ranges,
+      "\npeak # VM ranges:      ", stat_.peak_va_ranges,
       "\ncurrently allocated:   ", stat_.curr_allocated,
       "\npeak allocated:        ", stat_.peak_allocated,
       "\nallocated_blocks:      ", stat_.allocated_blocks,
       "\nblock size:            ", block_size_,
       "\nnon-freed allocations: ", stat_.curr_allocations,
       "\ntotal allocations:     ", stat_.total_allocations,
       "\ntotal deallocations:   ", stat_.total_deallocations,
       "\ntotal unmapping:       ", stat_.total_unmaps,
-      "\nfree pool size:        ", stat_.curr_free);
+      "\nfree pool size:        ", stat_.curr_free,
+      "\n");
   }
 
   void dbg_dump(std::ostream &os) {
     dump_stats(os);
     dump_regions(os);
   }
 
@@ -147,18 +154,24 @@
 
   /**
    * @brief Releases unused physical blocks
    *
    * Releases physical blocks that are currently allocated, but fully available.
    */
   void release_unused() override {
+    do_release_unused(false);
+  }
+
+ protected:
+  std::pair<size_t, size_t> do_release_unused(bool release_va) {
+    size_t mem_freed = 0, va_freed = 0;
     std::vector<cuvm::CUMem> blocks_to_free;
     {
-      lock_guard pool_guard(pool_lock_);
-      mem_lock_guard mem_guard(mem_lock_);
+      std::unique_lock pool_guard(pool_lock_, std::try_to_lock);
+      std::unique_lock mem_guard(mem_lock_, std::try_to_lock);
 
       ptrdiff_t num_blocks_to_free = 0;
       for (auto &region : va_regions_) {
         ptrdiff_t start = 0, end = 0;
         for (;; start = end + 1) {
           start = region.available.find(true, start);
           end = region.available.find(false, start + 1);
@@ -178,30 +191,142 @@
             if (end <= start)
               break;
             auto *start_ptr = region.block_ptr<char>(start);
             auto *end_ptr = region.block_ptr<char>(end);
             for (ptrdiff_t i = start; i < end; i++) {
               blocks_to_free.push_back(region.unmap_block(i));
               stat_.total_unmaps++;
+              mem_freed += block_size_;
             }
             free_mapped_.get_specific_block(start_ptr, end_ptr);
           }
         }
       }();
       assert(static_cast<ptrdiff_t>(blocks_to_free.size()) == num_blocks_to_free);
       stat_.allocated_blocks -= blocks_to_free.size();
     }
     blocks_to_free.clear();  // free the physical memory
+    if (release_va)
+      va_freed = release_unused_va();
+    return { mem_freed, va_freed };
   }
 
  protected:
   void do_deallocate(void *ptr, size_t size, size_t alignment) override {
     deallocate_impl(ptr, size, alignment, true);
   }
 
+  int find_va_region(CUdeviceptr ptr) {
+    for (size_t i = 0; i < va_regions_.size(); i++)
+      if (va_regions_[i].address_range.contains(ptr))
+        return i;
+    return -1;
+  }
+
+  size_t release_unused_va() {
+    struct RangeDesc {
+      int range_idx, region_idx;
+      int start_block, end_block;
+    };
+    std::vector<cuvm::CUMem> blocks_to_free;
+    std::vector<cuvm::CUMemAddressRange> va_ranges_to_free;
+    std::vector<RangeDesc> ranges_to_free;
+    blocks_to_free.reserve(stat_.allocated_blocks);
+    va_ranges_to_free.reserve(va_ranges_.size());
+    ranges_to_free.reserve(va_ranges_.size());
+    size_t va_freed = 0;
+
+    {
+      std::unique_lock pool_guard(pool_lock_, std::try_to_lock);
+      std::unique_lock mem_guard(mem_lock_, std::try_to_lock);
+
+      // the whole block below musn't throw or it'll leave the resource in an inconsistent state
+      [&]() noexcept {
+        for (int i = 0, n = va_ranges_.size(); i < n; i++) {
+          auto start = va_ranges_[i].ptr();
+          auto end = va_ranges_[i].end();
+          if (free_va_.contains(reinterpret_cast<void*>(start), reinterpret_cast<void*>(end))) {
+            int region_idx = find_va_region(start);
+            assert(region_idx >= 0);
+            va_region &region = va_regions_[region_idx];
+
+            ptrdiff_t offset = start - region.address_range.ptr();
+            assert(offset % block_size_ == 0);
+            int num_blocks = (end - start) / block_size_;
+            int start_block = offset / block_size_;  // index of the first block
+            int end_block = start_block + num_blocks;  // index of the last block
+
+            int avail = region.available.find(true, start_block);
+            while (avail < end_block) {
+              int end_avail = std::min<int>(region.available.find(false, avail + 1), end_block);
+              for (int b = avail; b < end_avail; b++) {
+                blocks_to_free.push_back(region.unmap_block(b));
+                stat_.total_unmaps++;
+              }
+              auto *start_ptr = region.block_ptr<char>(avail);
+              auto *end_ptr = region.block_ptr<char>(end_avail);
+              free_mapped_.get_specific_block(start_ptr, end_ptr);
+
+              if (end_avail == end_block)
+                break;
+              avail = region.available.find(true, end_avail + 1);
+            }
+
+            ranges_to_free.push_back({ i, region_idx, start_block, end_block });
+          }
+        }
+        stat_.allocated_blocks -= blocks_to_free.size();
+      }();
+
+      for (const RangeDesc &rd : ranges_to_free) {
+        auto &region = va_regions_[rd.region_idx];
+
+        // We split the va_region as follows:
+
+        // |<--------------- old region ---------------------->|
+        // |<---region-->|<--va_range_to_remove-->|<---tail--->|
+        //               ^                        ^
+        // start_block---^                        ^---- end_block
+
+        // If start_block is 0 then `region` will become empty and we can either
+        // overwrite it with tail (if not empty) or remove it altogether
+
+        va_region tail = region.split(rd.end_block);
+        region.resize(rd.start_block);
+
+        auto *start_ptr = region.block_ptr<char>(rd.start_block);
+        auto *end_ptr = region.block_ptr<char>(rd.end_block);
+        ptrdiff_t range_size = (end_ptr - start_ptr);
+
+        if (region.empty()) {
+          if (tail.empty())
+            va_regions_.erase(va_regions_.begin() + rd.region_idx);
+          else
+            region = std::move(tail);
+        } else if (!tail.empty()) {
+          va_regions_.push_back(std::move(tail));
+        }
+
+        va_ranges_to_free.push_back(std::move(va_ranges_[rd.range_idx]));
+        va_ranges_.erase(va_ranges_.begin() + rd.range_idx);
+        stat_.allocated_va -= range_size;
+        va_freed += range_size;
+        void *p = free_va_.get_specific_block(start_ptr, end_ptr);
+        assert(p != nullptr);
+        (void)p;  // for non-debug builds
+      }
+
+      stat_.va_ranges -= va_ranges_to_free.size();
+    }
+
+    blocks_to_free.clear();
+    va_ranges_to_free.clear();
+    return va_freed;
+  }
+
   void *do_allocate(size_t size, size_t alignment) override {
     if (size == 0)
       return nullptr;
     if (size > total_mem_)
       throw CUDABadAlloc(size);  // this can't succeed - no need to even try
     adjust_params(size, alignment, true);
     std::unique_lock<pool_lock_t> pool_guard(pool_lock_);
@@ -274,14 +399,18 @@
     va_region(va_region &&) = default;
     va_region &operator=(va_region &&) = default;
 
     ~va_region() {
       purge();
     }
 
+    bool empty() const {
+      return num_blocks() == 0;
+    }
+
     int num_blocks() const {
       return mapping.size();
     }
 
     void purge() {
       CUdeviceptr ptr = address_range.ptr();
       for (size_t i = 0; i < mapping.size(); i++, ptr += block_size) {
@@ -318,22 +447,27 @@
       assert(available_blocks >= 0 && available_blocks <= num_blocks());
     }
 
     cuvm::CUMem unmap_block(int block_idx) {
       assert(available[block_idx]);
       cuvm::Unmap(block_dptr(block_idx), block_size);
       cuvm::CUMem mem({mapping[block_idx], block_size });
-      mapping[block_idx] = 0;
+      mapping[block_idx] = {};
       mapped[block_idx] = false;
       available[block_idx] = false;
       available_blocks--;
       assert(available_blocks >= 0 && available_blocks <= num_blocks());
       return mem;
     }
 
+    /**
+     * @brief Adds the contents of `other` at the end of this region.
+     *
+     * @note This function operates purely on metadata and doesn't affect the process memory map.
+     */
     void append(va_region &&other) {
       assert(address_range.end() == other.address_range.ptr());
       assert(block_size == other.block_size);
       address_range.size() += other.address_range.size();
       int other_blocks = other.num_blocks();
       int old_blocks = num_blocks();
       mapping.resize(old_blocks + other_blocks);
@@ -350,14 +484,61 @@
       other.mapped = {};
       available_blocks += other.available_blocks;
       other.available_blocks = 0;
       assert(mapping.size() == mapped.size());
       assert(mapping.size() == available.size());
     }
 
+    /**
+     * @brief Trims the current region to `tail_start` blocks and returns the rest as a new region.
+     *
+     * @note This function operates purely on metadata and doesn't affect the process memory map.
+     *
+     * @param tail_start  The index of the first block to be moved to `tail`
+     * @return va_region  The region starting at `tail_start`.
+     */
+    va_region split(int tail_start) {
+      if (tail_start == 0) {
+        va_region ret = std::move(*this);
+        available_blocks = 0;
+        address_range = {};
+        return ret;
+      } else if (tail_start == num_blocks()) {
+        return va_region({}, block_size);
+      }
+      int tail_blocks = num_blocks() - tail_start;
+      cuvm::CUAddressRange tail_range(block_dptr(tail_start), tail_blocks * block_size);
+      va_region tail(tail_range, block_size);
+      int n = num_blocks();
+      for (int src = tail_start, dst = 0; src < n; src++, dst++) {
+        tail.mapping[dst] = std::move(available[src]);
+        tail.mapped[dst] = mapped[src];
+
+        bool avail = available[src];
+        tail.available[dst] = avail;
+        if (avail) {  // update the available block count
+          tail.available_blocks++;
+          available_blocks--;
+        }
+      }
+      resize(tail_start);
+      return tail;
+    }
+
+    /**
+     * @brief Changes the size of the region.
+     *
+     * If the new size is smaller than the old one and there are any blocks mapped at indices
+     * that would become out of range, they are unmapped and deallocated.
+     *
+     * @note This function may change the process memory map.
+     *
+     * @note This function affects just the region and doesn't adjust the free_va / free_mapped
+     *       in the enclosing VM resource. These need to be adjusted by the caller.
+     */
     void resize(int new_num_blocks) {
       if (new_num_blocks < num_blocks()) {
         int no_longer_in_range = 0;
         for (int i = new_num_blocks; i < num_blocks(); i++) {
           if (mapping[i]) {
             cuvm::Unmap(block_ptr(i), block_size);
             CUDA_DTOR_CALL(cuMemRelease(mapping[i]));
@@ -453,30 +634,33 @@
   }
 
   /**
    * @brief Allocate virtual address space of at at least `min_size` bytes.
    *
    * The function hints the driver to use a distinct address space for each device in the
    * attempt to have a contiguous address spaces for each device. Currently, the spacing
-   * between device VA spaces is 1 TiB and initial VA size for each device is 4 GiB.
+   * between device VA spaces is 1 TiB and initial VA size for each device is double the physical
+   * size.
+   * On platforms that restrict VA size, if the reservation, fails there are more attempts to
+   * allocate the size that's large enough to accommodate the requested size.
    */
   void va_allocate(size_t min_size) {
     size_t va_size = std::max(next_pow2(min_size), initial_va_size_);
 
     cuvm::CUMemAddressRange va;
 
     struct Hint {
       CUdeviceptr address;
       size_t      alignment;
     };
     SmallVector<Hint, 4> hints;
 
     if (va_regions_.empty()) {
       // Calculate the alignment for the initial allocations for this device - we start from
-      // 4 TiB nad go down.
+      // 4 TiB and go down.
       // The address hint is not important.
       hints = {
         { 0_zu, 1_zu << 42 },
         { 0_zu, 1_zu << 40 },
         { 0_zu, 1_zu << 38 },
         { 0_zu, 1_zu << 36 }
       };
@@ -489,39 +673,64 @@
       va_size = std::max(va_size, 2 * va_ranges_.back().size());
       hints = {
         { last_va.address_range.end(), block_size_ },
         { first_va.address_range.ptr() - va_size, block_size_ }
       };
     }
 
-    // Try to allocate at hinted locations...
-    for (auto hint : hints) {
-      try {
-        va = cuvm::CUMemAddressRange::Reserve(va_size, hint.alignment, hint.address);
-        break;
-      } catch (const CUDAError &) {
-      } catch (const std::bad_alloc &) {}
+    while (!va) {
+      // Try to allocate at hinted locations...
+      for (auto hint : hints) {
+        try {
+          va = cuvm::CUMemAddressRange::Reserve(va_size, hint.alignment, hint.address);
+          break;
+        } catch (const CUDAError &) {
+        } catch (const std::bad_alloc &) {}
+      }
+      if (!va) {
+        // ...hint failed - allocate anywhere, just align to block_size_
+        auto on_error = [&](auto &exception) {
+          size_t next_va_size;
+          next_va_size = std::max(align_up(min_size, block_size_), va_size >> 1);
+          if (next_va_size == va_size) {  // we're already as low as we can - rethrow
+            if (!release_unused_va())
+              throw exception;
+          }
+          va_size = next_va_size;
+        };
+
+        try {
+          va = cuvm::CUMemAddressRange::Reserve(va_size, block_size_, 0);
+          break;
+        } catch (const CUDAError &e) {
+          on_error(e);
+        } catch (const std::bad_alloc &e) {
+          on_error(e);
+        }
+      }
     }
-    if (!va)  // ...hint failed - allocate anywhere, just align to block_size_
-      va = cuvm::CUMemAddressRange::Reserve(va_size, block_size_, 0);
+
+
+    if (va_size < initial_va_size_)
+        initial_va_size_ = va_size;
 
     if (!mm::detail::is_aligned(detail::u2ptr(va.ptr()), block_size_))
       throw std::logic_error("The VA region is not aligned to block size!\n"
         "This should never happen.");
 
     va_ranges_.push_back(std::move(va));
-    va_add_region(va_ranges_.back());
+    va_add_range(va_ranges_.back());
     stat_va_add(va_size);
   }
 
   /**
    * @brief Add a memory region that spans the given VA range and merge it with adjacent
    *        regions, if found.
    */
-  void va_add_region(cuvm::CUAddressRange va) {
+  void va_add_range(cuvm::CUAddressRange va) {
     // Try to merge regions
     // 1. Find preceding region
     va_region *region = nullptr;
     for (auto &r : va_regions_)
       if (r.address_range.end() == va.ptr()) {
         region = &r;
         break;
@@ -801,14 +1010,19 @@
     stat_.allocated_blocks += count;
     if (stat_.allocated_blocks > stat_.peak_allocated_blocks)
       stat_.peak_allocated_blocks = stat_.allocated_blocks;
   }
 
   void stat_va_add(size_t size) {
     stat_.allocated_va += size;
+    if (stat_.allocated_va > stat_.peak_va)
+      stat_.peak_va = stat_.allocated_va;
+    stat_.va_ranges++;
+    if (stat_.va_ranges > stat_.peak_va_ranges)
+      stat_.peak_va_ranges = stat_.va_ranges;
   }
 };
 
 }  // namespace mm
 }  // namespace dali
 
 #endif  // DALI_USE_CUDA_VM_MAP
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/default_resources.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/default_resources.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/align.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/align.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_alloc.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_alloc.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_collections.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/aux_collections.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/free_list.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/free_list.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/util.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/detail/util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/fixed_order_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/fixed_order_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/malloc_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/malloc_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_kind.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_kind.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/memory_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/monotonic_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/monotonic_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource_base.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/pool_resource_base.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/with_upstream.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/mm/with_upstream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/nvtx.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/nvtx.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/os/shared_mem.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/os/shared_mem.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/partition.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/partition.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/per_stream_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/per_stream_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/permute.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/permute.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/python_util.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/python_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/random.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/random.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/small_vector.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/small_vector.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/span.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/span.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/spinlock.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/spinlock.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_map.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_map.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_switch.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/static_switch.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/stream.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/stream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_layout.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_layout.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape_print.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_shape_print.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_view.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tensor_view.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/traits.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/traits.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tuple_helpers.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/tuple_helpers.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/unique_handle.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/unique_handle.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/util.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/version_util.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/core/version_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/decode_results.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/decode_results.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder_interfaces.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_decoder_interfaces.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_format.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_format.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_orientation.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_orientation.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_source.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/imgcodec/image_source.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/operators.h` & `nvidia-dali-tf-plugin-cuda110-1.27.0/include/dali/operators.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/Acknowledgements.txt` & `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/Acknowledgements.txt`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/COPYRIGHT` & `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/LICENSE` & `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/LICENSE`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/__init__.py` & `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.26.0'
-__git_sha__ = 'cdc39704b8f824f342e0e0c9163ba12518434987'
+__version__ = '1.27.0'
+__git_sha__ = '4cc38a6b48a74cc06fe8594b6e5c18ae090dc045'
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/dali_tf_plugin.py` & `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia/dali_tf_plugin/dali_tf_plugin.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-cuda110
-Version: 1.26.0
-Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: cdc39704b8f824f342e0e0c9163ba12518434987
+Version: 1.27.0
+Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 4cc38a6b48a74cc06fe8594b6e5c18ae090dc045
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Description: TensorFlow plugin for NVIDIA DALI
         =================================
         
         The TensorFlow plugin enables usage of DALI with TensorFlow.
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt` & `nvidia-dali-tf-plugin-cuda110-1.27.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 ./include/dali/core/exec/engine.h
 ./include/dali/core/geom/box.h
 ./include/dali/core/geom/geom_utils.h
 ./include/dali/core/geom/mat.h
 ./include/dali/core/geom/transform.h
 ./include/dali/core/geom/vec.h
 ./include/dali/core/mm/async_pool.h
+./include/dali/core/mm/binning_resource.h
 ./include/dali/core/mm/composite_resource.h
 ./include/dali/core/mm/cu_vm.h
 ./include/dali/core/mm/cuda_vm_resource.h
 ./include/dali/core/mm/default_resources.h
 ./include/dali/core/mm/fixed_order_resource.h
 ./include/dali/core/mm/malloc_resource.h
 ./include/dali/core/mm/memory.h
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_11.so` & `nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_11.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_12.so` & `nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/libdali_tf_2_12.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/stub/libdali.so` & `nvidia-dali-tf-plugin-cuda110-1.27.0/prebuilt/stub/libdali.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/setup.py` & `nvidia-dali-tf-plugin-cuda110-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         # It doesn't matter what we write here, because we are overriding the
         # build_ext step altogether.
         # By filling this ext_modules we are signaling that this package needs
         # to be built for different platforms
         self.ext_modules = [Extension('nvidia.dali_tf_plugin', [])]
 
 setup(name='nvidia-dali-tf-plugin-cuda110',
-      description='NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: cdc39704b8f824f342e0e0c9163ba12518434987',
+      description='NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 4cc38a6b48a74cc06fe8594b6e5c18ae090dc045',
       long_description='''TensorFlow plugin for NVIDIA DALI
 =================================
 
 The TensorFlow plugin enables usage of DALI with TensorFlow.
 
 The NVIDIA Data Loading Library (DALI) is a library for data loading and
 pre-processing to accelerate deep learning applications. It provides a
@@ -70,30 +70,30 @@
     :alt: DALI Diagram
 
 .. |release-doc| replace:: latest DALI Documentation
 .. _release-doc: https://docs.nvidia.com/deeplearning/dali/user-guide/docs/index.html
 ''',
       long_description_content_type="text/x-rst",
       url='https://github.com/NVIDIA/dali',
-      version='1.26.0',
+      version='1.27.0',
       author='NVIDIA Corporation',
       license='Apache License 2.0',
       packages=find_namespace_packages(include=['nvidia.*']),
       include_package_data=True,
       zip_safe=False,
       python_requires='>=3.6, <3.11',
       classifiers=[
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           ],
       install_requires = [
-          'nvidia-dali-cuda110==1.26.0'
+          'nvidia-dali-cuda110==1.27.0'
           ],
 
       cmdclass={
           'build_ext': CustomBuildExt,
       },
       distclass=CustomDistribution
      )
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.26.0/stubgen.py` & `nvidia-dali-tf-plugin-cuda110-1.27.0/stubgen.py`

 * *Files identical despite different names*

