# Comparing `tmp/kevin-toolbox-1.1.1.tar.gz` & `tmp/kevin-toolbox-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kevin-toolbox-1.1.1.tar", last modified: Wed Jun 21 04:23:26 2023, max compression
+gzip compressed data, was "dist/kevin-toolbox-1.1.2.tar", last modified: Tue Jun 27 11:05:16 2023, max compression
```

## Comparing `kevin-toolbox-1.1.1.tar` & `kevin-toolbox-1.1.2.tar`

### file list

```diff
@@ -1,317 +1,317 @@
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5229 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4707 2023-06-21 04:22:25.000000 kevin-toolbox-1.1.1/README.md
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       23 2023-06-21 04:22:36.000000 kevin-toolbox-1.1.1/kevin_toolbox/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_dict/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      273 2023-06-14 02:14:33.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      887 2023-06-14 03:38:14.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      645 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3543 2023-06-20 10:55:20.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1303 2023-06-20 11:09:48.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_value_by_name.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1051 2023-06-20 10:25:59.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-06-20 09:49:43.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2350 2023-06-20 23:12:24.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2842 2023-06-20 11:37:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3951 2023-06-20 12:12:02.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      169 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3181 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1737 2023-06-21 04:20:39.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2155 2023-06-21 03:37:47.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_seq/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/locks/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/locks/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/pareto_front/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/registration/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/registration/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13982 2023-06-21 01:27:56.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/registration/registry.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/scheduler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11495 2023-06-21 01:55:52.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2203 2023-06-21 01:47:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/search/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/search/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/search/binary_search.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      120 2023-06-01 10:31:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-01 10:26:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3101 2023-06-01 10:35:42.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5571 2023-06-01 10:29:44.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/utils/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/data_structure/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/data_structure/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-1.1.1/kevin_toolbox/computer_science/data_structure/executor.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/dangerous/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-1.1.1/kevin_toolbox/dangerous/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/cache/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/cache/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2507 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/unified_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/converter/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      161 2023-06-01 11:21:11.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/converter/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/converter/integrate.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      237 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/read_json.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      785 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/write_json.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/converter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-06-21 01:55:22.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16285 2023-06-21 00:22:15.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/read.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6838 2023-06-21 00:15:01.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/write.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/decorator/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/decorator/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/decorator/restore_original_work_path.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/singleton/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/singleton/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/general_matrix_multiplication.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/numerical_characteristics/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/numerical_characteristics/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/numerical_characteristics/iou.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/my_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/my_iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/sequence_map_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/developing/test.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/check_validity_and_uninstall.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/check_version_and_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/test/test_version.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/compare_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/parse_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/sort_version_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/__old_version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_collision.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_overlap.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/analysis/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/dummy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/convert/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/merge_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/split_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/transpose/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/transpose/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/cache.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/test_get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/dct/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/dct/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/dct/dct_calculator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/scaling_and_shift/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2023-04-21 12:36:14.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/utils/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/utils/convert_dtype.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/utils/get_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/utils/set_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2023-05-30 12:44:28.000000 kevin-toolbox-1.1.1/kevin_toolbox/math/utils/spilt_integer_most_evenly.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/arrow3d.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-24 08:38:24.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       99 2023-04-24 08:58:58.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/linalg/normalize.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      253 2023-04-24 08:55:02.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/linalg/softmax.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_optuna/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2023-05-26 09:14:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_optuna/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4588 2023-05-26 09:40:56.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_os/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       27 2023-04-10 12:15:40.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_os/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      658 2023-04-17 12:51:37.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_os/remove.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2023-06-21 03:42:19.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_test/check_consistency.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/concat.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/tile.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/where.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/math/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/math/my_around.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox.egg-info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5229 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    14421 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/kevin_toolbox.egg-info/top_level.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-1.1.1/pyproject.toml
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-21 04:23:26.000000 kevin-toolbox-1.1.1/setup.cfg
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-1.1.1/setup.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2265 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1691 2023-06-27 11:04:31.000000 kevin-toolbox-1.1.2/README.md
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       23 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_dict/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      273 2023-06-14 02:14:33.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      887 2023-06-14 03:38:14.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      645 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3543 2023-06-20 10:55:20.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2122 2023-06-27 09:56:21.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_value_by_name.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1051 2023-06-20 10:25:59.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-06-20 09:49:43.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2350 2023-06-20 23:12:24.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2875 2023-06-27 09:41:07.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3951 2023-06-20 12:12:02.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      169 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3181 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1737 2023-06-21 04:20:39.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2155 2023-06-21 03:37:47.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_seq/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/locks/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/locks/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/pareto_front/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/registration/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/registration/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13567 2023-06-27 10:15:54.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/registration/registry.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/scheduler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11495 2023-06-21 01:55:52.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4508 2023-06-27 11:00:57.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/search/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/search/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/search/binary_search.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      120 2023-06-01 10:31:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-01 10:26:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3101 2023-06-01 10:35:42.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5571 2023-06-01 10:29:44.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/utils/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/data_structure/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/data_structure/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-1.1.2/kevin_toolbox/computer_science/data_structure/executor.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/dangerous/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-1.1.2/kevin_toolbox/dangerous/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/cache/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/cache/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2507 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/unified_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/converter/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      161 2023-06-01 11:21:11.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/converter/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/converter/integrate.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      237 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/read_json.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      785 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/write_json.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/converter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-06-21 01:55:22.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16285 2023-06-21 00:22:15.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/read.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6838 2023-06-21 00:15:01.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/write.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/decorator/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/decorator/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/decorator/restore_original_work_path.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/singleton/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/singleton/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/general_matrix_multiplication.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/numerical_characteristics/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/numerical_characteristics/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/numerical_characteristics/iou.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/my_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/my_iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/sequence_map_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/developing/test.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/check_validity_and_uninstall.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/check_version_and_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/test/test_version.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/compare_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/parse_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/sort_version_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/__old_version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_collision.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_overlap.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/analysis/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/dummy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/convert/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/merge_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/split_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/transpose/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/transpose/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/cache.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/test_get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/dct/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/dct/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/dct/dct_calculator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/scaling_and_shift/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2023-04-21 12:36:14.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/utils/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/utils/convert_dtype.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/utils/get_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/utils/set_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2023-05-30 12:44:28.000000 kevin-toolbox-1.1.2/kevin_toolbox/math/utils/spilt_integer_most_evenly.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/arrow3d.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-24 08:38:24.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       99 2023-04-24 08:58:58.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/linalg/normalize.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      253 2023-04-24 08:55:02.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/linalg/softmax.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_optuna/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2023-05-26 09:14:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_optuna/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4588 2023-05-26 09:40:56.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_os/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       27 2023-04-10 12:15:40.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_os/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      658 2023-04-17 12:51:37.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_os/remove.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3184 2023-06-26 08:43:44.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_test/check_consistency.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/concat.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/tile.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/where.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/math/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/math/my_around.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox.egg-info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2265 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    14421 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/kevin_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-1.1.2/pyproject.toml
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-27 11:05:16.000000 kevin-toolbox-1.1.2/setup.cfg
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-1.1.2/setup.py
```

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                                 名字 name 的具体介绍参见函数 name_handler.parse_name()
                                 假设 var=dict(acc=[0.66,0.78,0.99])，如果你想将 var["acc"][1] 设置为 100，那么可以将 name 写成：
                                     ":acc@1" 或者 "|acc|1" 等。
                                 注意，在 name 的开头也可以添加任意非取值方式的字符，本函数将直接忽略它们，比如下面的:
                                     "var:acc@1" 和 "xxxx|acc|1" 也能正常写入。
             value:          待赋给的值
             b_force:        <boolean> 当无法设置时，是否尝试创建或者修改节点
-                                默认为 False，
+                                默认为 False，此时若无法设置，则报错
                                 当设置为 True，可能会对 var 的结构产生不可逆的改变，请谨慎使用。
                                     - 根据取值方式的不同，新创建或者修改的节点的类型可能是 dict 或者 list，
                                         对于 list，其中缺省值填充 None。
                                     - 当需要创建节点时，| 方式将优先创建 dict
     """
     _, method_ls, node_ls = parse_name(name=name, b_de_escape_node=False)
     if len(node_ls) == 0:
```

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/registration/registry.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/registration/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,46 +53,56 @@
     __counter = 0
 
     def __new__(cls, *args, **kwargs):
         """
             __new__函数返回的实例，将作为self参数被传入到__init__函数。
                 如果__new__函数返回一个已经存在的实例（不论是哪个类的），__init__还是会被调用的，所以要特别注意__init__中对变量的赋值。
         """
-        uid = kwargs.get("uid", cls.__counter)
+        if "uid" in kwargs:
+            uid = kwargs["uid"]
+        else:
+            while cls.__counter in cls.__instances:
+                cls.__counter += 1
+            uid = cls.__counter
 
         # 获取实例
         if uid in cls.__instances:
             # 返回已存在的实例
             self = cls.__instances[uid]
         else:
             # 传入 __init__ 中新建一个实例
             self = super().__new__(cls)
         return self
 
     def __init__(self, *args, **kwargs):
         """
             参数：
                 uid:                <hashable> 实例的唯一标识符
-                                        默认置空，此时将新建一个实例，并将此时已有实例的数量作为 uid
-                                        当为非空，则根据 uid 到已有实例中寻找相同的实例，并返回（使用该特性可以构造单例模式）
+                                        - 不设置。新建一个实例，并自动分配一个整数作为 uid（一般是此时已有实例的数量-1），
+                                            并将该实例记录到类变量 instances_of_Registry 中。
+                                        - 设置为 None。新建一个实例，但不记录到类变量 instances_of_Registry 中。
+                                        - 设置为其他值。根据 uid 到类变量 instances_of_Registry 的已有实例中寻找相同的实例，
+                                            若命中则返回已有实例，若无则以该 uid 新建一个实例并添加到 instances_of_Registry 中。
+                                            （使用该特性可以构造单例模式）
+                                        默认为不设置。
         """
         try:
             getattr(self, "uid")
         except:
             pass
         else:
             return  # 如果是从 __new__ 中获取的已有的实例则不重复进行参数赋值
         self.database = dict()
         #
         self.uid = kwargs.get("uid", Registry.__counter)
         self._path_to_collect = []
         self._item_to_add = []
         # 记录到 __instances 中
-        Registry.__instances[self.uid] = self
-        Registry.__counter += 1
+        if self.uid is not None:
+            Registry.__instances[self.uid] = self
 
     def add(self, obj, name=None, b_force=False, b_execute_now=True):
         """
             注册
 
             参数：
                 obj：            待注册成员
@@ -136,82 +146,45 @@
             return True
 
         # 尝试注册
         temp = fndl.set_value_by_name(var=fndl.copy_(var=self.database, b_deepcopy=False), name=name, value=obj,
                                       b_force=True)
         # check
         if not b_force:
-            inc_node_nums = fndl.count_leaf_node_nums(var=obj) if isinstance(obj, (list, dict)) else 1  # 增加的节点数量
+            inc_node_nums = fndl.count_leaf_node_nums(var=obj) if isinstance(obj, (list, dict)) else 1  # 应该增加的节点数量
             if fndl.count_leaf_node_nums(var=temp) != fndl.count_leaf_node_nums(var=self.database) + inc_node_nums:
                 # print(f'registration failed, name {name} may be a conflict with an '
                 #       f'existing member in {[i for i, j in fndl.get_nodes(var=self.database)]}')
                 return False
 
         self.database = temp
         return True
 
-    def get(self, name, **kwargs):
+    def get(self, name, b_pop=False, **kwargs):
         """
             获取
 
             参数：
-                name：           <str> 成员名称
-                default:          默认值
+                name:           <str> 成员名称
+                b_pop:          <boolean> 取值的同时移除该成员
+                                    默认为 False
+                default:        默认值
                                     找不到时，若无默认值则报错，否则将返回默认值
         """
         # 加载待注册成员
         if len(self._item_to_add) > 0:
             for i in self._item_to_add:
                 self.add(**i)
             self._item_to_add.clear()
         if len(self._path_to_collect) > 0:
             for i in self._path_to_collect:
                 self.collect_from_paths(**i)
             self._path_to_collect.clear()
 
-        try:
-            return fndl.get_value_by_name(var=self.database, name=name)
-        except:
-            if "default" in kwargs:
-                return kwargs["default"]
-            else:
-                raise AssertionError(f'element {name} not exists')
-
-    def pop(self, name, **kwargs):
-        """
-            弹出
-
-            参数：
-                name：           <str> 成员名称
-                                    名称一定要准确，不能含有模糊的 | 字符
-                default:          默认值
-                                    找不到时，若无默认值则报错，否则将返回默认值
-        """
-        assert "|" not in name, \
-            f'to pop up a specific member needs to give the exact name, ' \
-            f'does not support the "|" character with automatic deduction, invalid name: {name}, ' \
-            f'what you probably want to pop is {name.replace("|", ":")}'
-        res, b_found = None, False
-
-        def func(_, idx, value):
-            nonlocal res, b_found
-            if res is None and idx == name:
-                res, b_found = value, True
-                return True
-            else:
-                return False
-
-        fndl.traverse(var=self.database, match_cond=func, action_mode="remove", b_use_name_as_idx=True)
-        if b_found:
-            return res
-        else:
-            if "default" in kwargs:
-                return kwargs["default"]
-            else:
-                raise AssertionError(f'element {name} not exists')
+        return fndl.get_value_by_name(var=self.database, name=name, b_pop=b_pop, **kwargs)
 
     def clear(self):
         self.database.clear()
 
     # -------------------- 装饰器 --------------------- #
 
     def register(self, name=None, b_force=False, b_execute_now=True):
@@ -232,15 +205,15 @@
         def wrapper(obj):
             nonlocal self, name, b_force, b_execute_now
             self.add(obj, name=name, b_force=b_force, b_execute_now=b_execute_now)
             return obj
 
         return wrapper
 
-    # -------------------- 其他 --------------------- #
+    # -------------------- 通过路径添加 --------------------- #
 
     def collect_from_paths(self, path_ls=None, path_ls_to_exclude=None, b_execute_now=False):
         """
             遍历 path_ls 下的所有模块，并自动导入其中主要被注册的部分
                 比如被 register() 装饰器包裹或者通过 add() 添加的部分
 
             参数：
@@ -294,9 +267,15 @@
                 for name, obj in inspect.getmembers(module):
                     if getattr(obj, "name", None) == Registry.name and getattr(obj, "uid", None) == self.uid:
                         temp = obj
                         break
         if temp is not None:
             self.database = temp.database
 
+    # -------------------- 其他 --------------------- #
+
+    @property
+    def instances_of_Registry(self):
+        return dict(Registry.__instances)
+
 
 UNIFIED_REGISTRY = Registry(uid="UNIFIED_REGISTRY")
```

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/search/binary_search.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/search/binary_search.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/computer_science/data_structure/executor.py` & `kevin-toolbox-1.1.2/kevin_toolbox/computer_science/data_structure/executor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py` & `kevin-toolbox-1.1.2/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/unified_reader.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/unified_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/core/reader/unified_reader_base.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/core/reader/unified_reader_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/json_/write_json.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/json_/write_json.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/converter.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/converter.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/data_flow/file/kevin_notation/write.py` & `kevin-toolbox-1.1.2/kevin_toolbox/data_flow/file/kevin_notation/write.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/producer_consumer/node.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/producer_consumer/node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/general_matrix_multiplication.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/general_matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/numerical_characteristics/iou.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/numerical_characteristics/iou.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/__init__.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/my_iterator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/my_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/developing/temperate/my_iterator_base.py` & `kevin-toolbox-1.1.2/kevin_toolbox/developing/temperate/my_iterator_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/env_info/check_validity_and_uninstall.py` & `kevin-toolbox-1.1.2/kevin_toolbox/env_info/check_validity_and_uninstall.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/env_info/check_version_and_update.py` & `kevin-toolbox-1.1.2/kevin_toolbox/env_info/check_version_and_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/env_info/test/test_version.py` & `kevin-toolbox-1.1.2/kevin_toolbox/env_info/test/test_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/compare_version.py` & `kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/compare_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/parse_version.py` & `kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/parse_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/env_info/version/sort_version_ls.py` & `kevin-toolbox-1.1.2/kevin_toolbox/env_info/version/sort_version_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/__init__.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_collision.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_collision.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/geometry/for_boxes/detect_overlap.py` & `kevin-toolbox-1.1.2/kevin_toolbox/geometry/for_boxes/detect_overlap.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/factory.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/factory.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py` & `kevin-toolbox-1.1.2/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/merge_blocks.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/split_blocks.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/split_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/get_primes.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/test_get_primes.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/test_get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/number_theory/test/test_prime_factorization.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/number_theory/test/test_prime_factorization.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/transform/dct/dct_calculator.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/transform/dct/dct_calculator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/transform/scaling_and_shift/scaling.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/transform/scaling_and_shift/scaling.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/utils/convert_dtype.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/utils/convert_dtype.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/utils/get_crop_by_box.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/utils/get_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/math/utils/set_crop_by_box.py` & `kevin-toolbox-1.1.2/kevin_toolbox/math/utils/set_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_matplotlib/arrow3d.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_matplotlib/arrow3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_numpy/linalg/normalize.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_numpy/linalg/normalize.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_os/remove.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_os/remove.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_test/check_consistency.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_test/check_consistency.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,17 +45,19 @@
                     f"{args[0]}, {v}, deviation: {np.max(np.abs(args[0] - v))}"
         elif issubclass(args[0].dtype.type, (np.flexible, object,)):
             # 可变长度类型
             assert issubclass(v.dtype.type, (np.flexible, object,))
             for i, j in zip(args[0].reshape(-1), v.reshape(-1)):
                 temp = i == j
                 if isinstance(temp, (bool,)):
-                    assert temp
+                    assert temp, \
+                        f"{args[0]}, {v}, diff: {temp}"
                 else:
-                    assert temp.all()
+                    assert temp.all(), \
+                        f"{args[0]}, {v}, diff: {temp}"
         else:
             raise ValueError
 
 
 if __name__ == '__main__':
     a = np.array([[1, 2, 3]])
     b = np.array([[1, 2, 3]])
```

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/tile.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/tile.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/compatible/where.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/compatible/where.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/math/get_y_at_x.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/math/get_y_at_x.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox/patches/for_torch/math/my_around.py` & `kevin-toolbox-1.1.2/kevin_toolbox/patches/for_torch/math/my_around.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/kevin_toolbox.egg-info/SOURCES.txt` & `kevin-toolbox-1.1.2/kevin_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/setup.cfg` & `kevin-toolbox-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.1/setup.py` & `kevin-toolbox-1.1.2/setup.py`

 * *Files identical despite different names*

