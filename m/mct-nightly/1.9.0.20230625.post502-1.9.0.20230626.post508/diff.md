# Comparing `tmp/mct-nightly-1.9.0.20230625.post502.tar.gz` & `tmp/mct-nightly-1.9.0.20230626.post508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-1.9.0.20230625.post502.tar", last modified: Sun Jun 25 00:05:03 2023, max compression
+gzip compressed data, was "mct-nightly-1.9.0.20230626.post508.tar", last modified: Mon Jun 26 00:05:09 2023, max compression
```

## Comparing `mct-nightly-1.9.0.20230625.post502.tar` & `mct-nightly-1.9.0.20230626.post508.tar`

### file list

```diff
@@ -1,529 +1,529 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.023582 mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-25 00:05:02.000000 mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32808 2023-06-25 00:05:02.000000 mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:05:02.000000 mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-25 00:05:02.000000 mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-25 00:05:02.000000 mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.027583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.027583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.027583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.027583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.027583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.027583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.031583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.031583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.031583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.031583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.031583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.031583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.035583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.035583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.035583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.035583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.035583 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.039584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.039584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.039584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.039584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.039584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.043584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/keras_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.043584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.043584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.043584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.043584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.047584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.047584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.047584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.047584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.047584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.047584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.047584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.051584 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.055585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/legacy/keras_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/legacy/pytorch_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.059585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.063585 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.067586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-25 00:04:14.000000 mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 00:05:03.071586 mct-nightly-1.9.0.20230625.post502/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-25 00:05:02.000000 mct-nightly-1.9.0.20230625.post502/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.784938 mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-26 00:05:09.000000 mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32808 2023-06-26 00:05:09.000000 mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:05:09.000000 mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 00:05:09.000000 mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 00:05:09.000000 mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.784938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.784938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.788938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.788938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.788938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.788938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.792938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.792938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.792938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.792938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.792938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.792938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.792938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.796938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.796938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.796938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.796938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.800938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.800938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.800938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.800938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.800938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27295 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/keras_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.804938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.808938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.808938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.808938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.808938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.808938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.808938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25800 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.808938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.812938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.816938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.816938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.816938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.816938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.816938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.820938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.820938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.820938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.820938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.820938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/legacy/keras_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/legacy/pytorch_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.820938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.824938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.824938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.824938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.824938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.824938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.824938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.828938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.828938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.828938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.828938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.828938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.832938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.832938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.832938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.836938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.836938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.836938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.836938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.840938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.840938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.840938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.844938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.844938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.844938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.844938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.844938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:05:09.848938 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-26 00:04:22.000000 mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 00:05:09.852938 mct-nightly-1.9.0.20230626.post508/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-26 00:05:08.000000 mct-nightly-1.9.0.20230626.post508/setup.py
```

### Comparing `mct-nightly-1.9.0.20230625.post502/LICENSE.md` & `mct-nightly-1.9.0.20230626.post508/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/PKG-INFO` & `mct-nightly-1.9.0.20230626.post508/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230625.post502
+Version: 1.9.0.20230626.post508
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-1.9.0.20230625.post502/README.md` & `mct-nightly-1.9.0.20230626.post508/README.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.9.0.20230625.post502
+Version: 1.9.0.20230626.post508
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-1.9.0.20230625.post502/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-1.9.0.20230626.post508/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/constants.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/analyzer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/data_loader.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/data_loader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/defaultdict.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 from typing import List
 
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.constants import FLOAT_BITWIDTH
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
 
 
 def filter_nodes_candidates(graph: Graph):
@@ -34,52 +36,86 @@
     nodes = list(graph.nodes)
     for n in nodes:
         n.candidates_quantization_cfg = filter_node_candidates(node=n)
 
     return graph
 
 
+def _filter_bit_method_dups(candidates: List[CandidateNodeQuantizationConfig]) -> List[CandidateNodeQuantizationConfig]:
+    """
+    Filters out duplications in candidates configuration list, based on similarity in
+    (weights_n_bits, weights_quantization_method, activation_n_bits, activation_quantization_method).
+
+    Args:
+        candidates: A list of quantization configuration candidates.
+
+    Returns: A filtered list of quantization configuration candidates.
+
+    """
+    seen_bits_method_combinations = set()
+    final_candidates = []
+    for c in candidates:
+        comb = (c.weights_quantization_cfg.weights_n_bits,
+                c.weights_quantization_cfg.weights_quantization_method,
+                c.activation_quantization_cfg.activation_n_bits,
+                c.activation_quantization_cfg.activation_quantization_method)
+        if comb not in seen_bits_method_combinations:
+            final_candidates.append(c)
+            seen_bits_method_combinations.add(comb)
+
+    return final_candidates
+
+
 def filter_node_candidates(node: BaseNode) -> List[CandidateNodeQuantizationConfig]:
     """
     Updates a node's candidates configuration list.
     If the node's weights quantization is disabled (or it only has activations to quantize), then the updated list
     will have a candidate with any of the different original activation bitwidths candidates and a default value
     for its weights bitwidth (that doesn't have any impact on the quantization or the mixed-precision search.
     If the node's activation quantization is disabled, the same filtering applied for the weights bitwidth candidates.
 
     Args:
         node: Node to set its quantization configurations.
     """
 
     filtered_candidates = copy.deepcopy(node.candidates_quantization_cfg)
+    final_candidates = copy.deepcopy(node.candidates_quantization_cfg)
 
     if not node.is_weights_quantization_enabled() and not node.is_activation_quantization_enabled():
         # If both weights and activation quantization are disabled, but for some reason the node has multiple candidates
         # then replace it with a single dummy candidate with default bit-width values.
         single_dummy_candidate = filtered_candidates[0]
         single_dummy_candidate.activation_quantization_cfg.activation_n_bits = FLOAT_BITWIDTH
         single_dummy_candidate.weights_quantization_cfg.weights_n_bits = FLOAT_BITWIDTH
-        filtered_candidates = [single_dummy_candidate]
+        single_dummy_candidate.weights_quantization_cfg.weights_quantization_method = QuantizationMethod.POWER_OF_TWO
+        single_dummy_candidate.activation_quantization_cfg.activation_quantization_method = QuantizationMethod.POWER_OF_TWO
+        final_candidates = [single_dummy_candidate]
 
     elif not node.is_activation_quantization_enabled():
         # Remove candidates that have duplicated weights candidates for node with disabled activation quantization.
         # Replacing the activation n_bits in the remained configurations with default value to prevent confusion.
         seen_candidates = set()
         filtered_candidates = [candidate for candidate in filtered_candidates if
                                candidate.weights_quantization_cfg not in seen_candidates
                                and not seen_candidates.add(candidate.weights_quantization_cfg)]
 
         for c in filtered_candidates:
             c.activation_quantization_cfg.activation_n_bits = FLOAT_BITWIDTH
+            c.activation_quantization_cfg.activation_quantization_method = QuantizationMethod.POWER_OF_TWO
+
+        final_candidates = _filter_bit_method_dups(filtered_candidates)
 
     elif not node.is_weights_quantization_enabled():
         # Remove candidates that have duplicated activation candidates for node with disabled weights quantization.
         # Replacing the weights n_bits in the remained configurations with default value to prevent confusion.
         seen_candidates = set()
         filtered_candidates = [candidate for candidate in filtered_candidates if
                                candidate.activation_quantization_cfg not in seen_candidates
                                and not seen_candidates.add(candidate.activation_quantization_cfg)]
 
         for c in filtered_candidates:
             c.weights_quantization_cfg.weights_n_bits = FLOAT_BITWIDTH
+            c.weights_quantization_cfg.weights_quantization_method = QuantizationMethod.POWER_OF_TWO
+
+        final_candidates = _filter_bit_method_dups(filtered_candidates)
 
-    return filtered_candidates
+    return final_candidates
```

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_analyzer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         Logger.critical(f'Look-Up-Table bit configuration has {n_bits} bits, but must be less or equal to '
                         f'{MULTIPLIER_N_BITS}')  # pragma: no cover
     # TODO: need to set this externally
     if len(np.unique(tensor_data.flatten())) < 2 ** n_bits:
         n_clusters = len(np.unique(tensor_data.flatten()))
     else:
         n_clusters = 2 ** n_bits
-    kmeans = KMeans(n_clusters=n_clusters)
+    kmeans = KMeans(n_clusters=n_clusters, n_init=10)
 
     threshold_selection_tensor = symmetric_selection_tensor if is_symmetric else power_of_two_selection_tensor
     thresholds_per_channel = threshold_selection_tensor(tensor_data, p, n_bits, per_channel,
                                                         channel_axis, n_iter, min_threshold,
                                                         qc.QuantizationErrorMethod.NOCLIPPING)[THRESHOLD]
 
     tensor_for_kmeans = int_quantization_with_threshold(tensor_data, thresholds_per_channel, MULTIPLIER_N_BITS)
@@ -121,15 +121,15 @@
 
     bins_with_values = np.abs(bins)[1:][counts > 0]
     if len(np.unique(bins_with_values.flatten())) < 2 ** n_bits:
         n_clusters = len(np.unique(bins_with_values.flatten()))
     else:
         n_clusters = 2 ** n_bits
 
-    kmeans = KMeans(n_clusters=n_clusters)
+    kmeans = KMeans(n_clusters=n_clusters, n_init=10)
     tensor_max = np.max(bins_with_values)
     threshold = max_power_of_two(tensor_max, min_threshold)
 
     signed = np.any(bins[:-1][counts != 0] < 0)  # Whether histogram contains negative values or not.
     tensor_for_kmeans = int_quantization_with_threshold(data=bins, threshold=threshold, n_bits=MULTIPLIER_N_BITS, signed=signed)
     kmeans.fit(tensor_for_kmeans.reshape(-1, 1), sample_weight=np.insert(counts, 0, 0))
```

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,142 +11,122 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
 import copy
+from typing import Callable
+
 import numpy as np
-from typing import Tuple, Callable
 
 from model_compression_toolkit.core import common
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.base_graph import Graph
-from model_compression_toolkit.core.common.graph.graph_matchers import EdgeMatcher, NodeOperationMatcher
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
+from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 
-class BatchNormalizationFolding(common.BaseSubstitution):
+class BatchNormalizationReconstruction(common.BaseSubstitution):
     """
-    Fold BatchNormalization into preceding linear layers.
+    Reconstruct BatchNormalization after linear layers.
     """
-
     def __init__(self,
                  source_node: NodeOperationMatcher,
-                 bn_node: NodeOperationMatcher,
-                 update_kernel_for_bn_folding_fn: Callable,
-                 kernel_str: str,
-                 bias_str: str,
+                 create_bn_node: Callable,
                  gamma_str: str,
                  beta_str: str,
                  moving_mean_str: str,
-                 moving__variance_str: str,
-                 epsilon_str: str,
-                 use_bias: str,
-                 layer_name_str: str):
+                 moving_variance_str: str,
+                 epsilon_val: float):
         """
-        Matches: Conv node (source node) to Batch Normalization (bn node).
+        Matches: Source (linear) nodes.
 
         Args:
-            source_node: Node matcher for convolution type nodes.
-            bn_node: Node matcher for batch normalization nodes.
-            update_kernel_for_bn_folding_fn: Function for updating the convolution kernel
-            with the batch normalization weights
-            kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
-            bias_str: The framework specific attribute name of the convolution layer's bias.
+            source_node: Node matcher for linear type nodes.
+            create_bn_node: Function for creating BN nodes.
             gamma_str: The framework specific attribute name of the batch norm layer's gamma parameter.
             beta_str: The framework specific attribute name of the batch norm layer's beta parameter.
             moving_mean_str: The framework specific attribute name of the batch norm layer's moving mean parameter.
-            moving__variance_str: The framework specific attribute name of the batch norm layer's moving variance parameter.
-            epsilon_str: The framework specific attribute name of the batch norm layer's epsilon parameter.
-            use_bias: The framework specific attribute name of the convolution layer's bias flag.
-            layer_name_str: The framework specific attribute name of layer's name.
+            moving_variance_str: The framework specific attribute name of the batch norm layer's moving
+            variance parameter.
+            epsilon_val: The framework specific attribute value of the batch norm layer's epsilon parameter.
         """
-        super().__init__(matcher_instance=EdgeMatcher(source_node, bn_node))
-        self.update_kernel_for_bn_folding_fn = update_kernel_for_bn_folding_fn
-        self.kernel_str = kernel_str
-        self.bias_str = bias_str
+        super().__init__(matcher_instance=source_node)
+        self.create_bn_node = create_bn_node
         self.gamma_str = gamma_str
         self.beta_str = beta_str
         self.moving_mean_str = moving_mean_str
-        self.moving__variance_str = moving__variance_str
-        self.epsilon_str = epsilon_str
-        self.use_bias = use_bias
-        self.layer_name_str = layer_name_str
+        self.moving_variance_str = moving_variance_str
+        self.epsilon_val = epsilon_val
 
     def substitute(self,
                    graph: Graph,
-                   edge_nodes: Tuple[BaseNode, BaseNode]) -> Graph:
+                   source_node: BaseNode) -> Graph:
         """
-        Fold BatchNormalization into preceding linear layers.
+        Reconstruct BatchNormalization after linear layers.
 
         Args:
             graph: Graph we apply the substitution on.
-            edge_nodes: Tuple of tow nodes (linear op and batchnorm node).
+            source_node: linear type node.
 
         Returns:
             Graph after applying the substitution.
         """
 
-        num_nodes_before_substition = len(graph.nodes)
-        num_edges_before_substition = len(graph.edges)
-
-        conv_node = edge_nodes[0]
+        num_nodes_before_substitution = len(graph.nodes)
+        num_edges_before_substitution = len(graph.edges)
 
         # If the linear operator is part of a reused group (it is the "base" node, or a reused node),
         # we should skip the substitution.
-        if conv_node.reuse or conv_node.reuse_group is not None:
+        if source_node.reuse or source_node.reuse_group is not None:
+            for qc in source_node.candidates_quantization_cfg:
+                qc.weights_quantization_cfg.weights_second_moment_correction = False
             return graph
 
-        bn_node = edge_nodes[1]
-
-        if len(graph.get_next_nodes(conv_node)) > 1 or len(graph.get_prev_nodes(bn_node)) > 1:
+        # We apply only on nodes with folded BatchNormalization.
+        if source_node.prior_info.std_output is None or source_node.prior_info.mean_output is None:
+            for qc in source_node.candidates_quantization_cfg:
+                qc.weights_quantization_cfg.weights_second_moment_correction = False
             return graph
 
-        kernel = conv_node.get_weights_by_keys(self.kernel_str)
-        bias = conv_node.get_weights_by_keys(self.bias_str)
-        gamma = bn_node.get_weights_by_keys(self.gamma_str)
-        beta = bn_node.get_weights_by_keys(self.beta_str)
-        moving_mean = bn_node.get_weights_by_keys(self.moving_mean_str)
-        moving_variance = bn_node.get_weights_by_keys(self.moving__variance_str)
-        eps = bn_node.framework_attr[self.epsilon_str]
-
-        if gamma is None:
-            gamma = 1.0
-        if beta is None:
-            beta = 0.0
-        if bias is None:
-            bias = 0.0
-
-        weights_scale = gamma / np.sqrt(moving_variance + eps)
-        bias = beta + (bias - moving_mean) * weights_scale
-
-        kernel, kernel_name = self.update_kernel_for_bn_folding_fn(conv_node, kernel, weights_scale)
-
-        framework_attr = copy.copy(conv_node.framework_attr)
-        framework_attr[self.use_bias] = True
-        if self.layer_name_str is not None:
-            framework_attr[self.layer_name_str] = conv_node.name + '_bn'
-
-        weights_dict = {kernel_name: kernel,
-                        self.bias_str: bias}
-
-        conv_bn = copy.deepcopy(conv_node)
-        conv_bn_name = conv_node.name + '_bn'
-        conv_bn.name = conv_bn_name
-        conv_bn.framework_attr = framework_attr
-        conv_bn.weights = weights_dict
-
-        graph.add_node(conv_bn)
-        graph.reconnect_out_edges(current_node=bn_node, new_node=conv_bn)
-        graph.reconnect_in_edges(current_node=conv_node, new_node=conv_bn)
-
-        graph.replace_output_node(current_node=bn_node, new_node=conv_bn)
-
-        conv_bn.prior_info = bn_node.prior_info
-
-        graph.remove_edge(conv_node, bn_node)
-        graph.remove_node(bn_node)
-        graph.remove_node(conv_node)
+        # This feature disabled for models with weights quantization method of Power of 2
+        for qc in source_node.candidates_quantization_cfg:
+            if qc.weights_quantization_cfg.weights_quantization_method == QuantizationMethod.POWER_OF_TWO:
+                Logger.warning("Second moment statistics correction feature disabled for models with weights "
+                               "quantization method of Power of 2")
+                for qc_inner in source_node.candidates_quantization_cfg:
+                    qc_inner.weights_quantization_cfg.weights_second_moment_correction = False
+                return graph
+
+        eps = self.epsilon_val
+
+        original_gamma = source_node.prior_info.std_output
+        beta = source_node.prior_info.mean_output
+        moving_mean = beta
+        moving_var = np.power(original_gamma, 2)
+        gamma = np.sqrt(moving_var + eps)
+
+        bn_node_weights = {self.gamma_str: gamma,
+                           self.beta_str: beta,
+                           self.moving_mean_str: moving_mean,
+                           self.moving_variance_str: moving_var}
+
+        bn_node = self.create_bn_node(source_node, bn_node_weights)
+
+        bn_node.prior_info = copy.deepcopy(source_node.prior_info)
+
+        bn_node.candidates_quantization_cfg = copy.deepcopy(source_node.candidates_quantization_cfg)
+
+        for qc in bn_node.candidates_quantization_cfg:
+            qc.weights_quantization_cfg.enable_weights_quantization = False
+            qc.activation_quantization_cfg.enable_activation_quantization = False
+
+        graph.reconnect_out_edges(current_node=source_node, new_node=bn_node)
+        graph.replace_output_node(current_node=source_node, new_node=bn_node)
+        graph.add_node_with_in_edges(bn_node, [source_node])
+
+        assert len(graph.nodes) - num_nodes_before_substitution == 1
+        assert len(graph.edges) - num_edges_before_substitution == 1
 
-        assert num_nodes_before_substition - len(graph.nodes) == 1
-        assert num_edges_before_substition - len(graph.edges) == 1
         return graph
```

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.activation_decomposition import \
     ActivationDecomposition
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.softmax_shift import \
     keras_softmax_shift
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.batchnorm_folding import \
-    keras_batchnorm_folding
+    keras_batchnorm_folding, keras_batchnorm_forward_folding
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.batchnorm_refusing import \
     keras_batchnorm_refusing
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.linear_collapsing import \
     keras_linear_collapsing
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.residual_collapsing import \
     keras_residual_collapsing
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.input_scaling import InputScaling, \
@@ -256,15 +256,16 @@
         Args:
             quant_config: QuantizationConfig to determine which substitutions to return.
 
         Returns:
             A list of the framework substitutions used before we collect statistics.
 
         """
-        substitutions_list = [keras_batchnorm_folding()]
+        substitutions_list = [keras_batchnorm_folding(),
+                              keras_batchnorm_forward_folding()]
         if quant_config.relu_bound_to_power_of_2:
             substitutions_list.append(ReLUBoundToPowerOfTwo())
         return substitutions_list
 
     def get_substitutions_statistics_correction(self, quant_config: QuantizationConfig) -> \
             List[common.BaseSubstitution]:
         """
```

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/kpi_data_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,66 +8,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-import numpy as np
 from torch.nn import BatchNorm2d, Conv2d, ConvTranspose2d
 
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
-from model_compression_toolkit.core.common import BaseNode
-from model_compression_toolkit.core.common.substitutions.batchnorm_folding import BatchNormalizationFolding
+from model_compression_toolkit.core.common.substitutions.batchnorm_refusing import BatchNormalizationRefusing
 from model_compression_toolkit.core.pytorch.constants import KERNEL, BIAS, GAMMA, BETA, MOVING_MEAN, MOVING_VARIANCE, \
     EPSILON, USE_BIAS
+from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.batchnorm_folding import \
+    update_kernel_for_bn_folding_fn
 
 
-def batchnorm_folding_node_matchers():
+def batchnorm_refusing_node_matchers():
     """
     Function generates matchers for matching:
     (Conv2d, ConvTranspose2d)-> BatchNorm2d.
 
     Returns:
         Matcher for batch norm nodes, and source nodes.
     """
     bn_node = NodeOperationMatcher(BatchNorm2d)
     source_node = NodeOperationMatcher(Conv2d) | \
                   NodeOperationMatcher(ConvTranspose2d)
     return bn_node, source_node
 
 
-def update_kernel_for_bn_folding_fn(conv_node: BaseNode,
-                                    kernel: np.ndarray,
-                                    weights_scale: np.ndarray):
+def pytorch_batchnorm_refusing() -> BatchNormalizationRefusing:
     """
-    Args:
-        conv_node: Convolution node to update the weight/kernel.
-        kernel: The Convolution node's weight
-        weights_scale: Weight scale factor in which to multiply the conv node's weight.
-
-    Returns:
-        The modified convolution node's weight/kernel/
-    """
-    return kernel * weights_scale[:, None, None, None], KERNEL
-
-
-def pytorch_batchnorm_folding() -> BatchNormalizationFolding:
-    """
-
+    Re-fuse BatchNormalization into preceding linear layers.
     Returns:
-        A BatchNormalizationFolding initialized for Pytorch models.
+        A BatchNormalizationRefusing initialized for Pytorch models.
     """
-    bn_node, source_node = batchnorm_folding_node_matchers()
-    return BatchNormalizationFolding(source_node,
-                                      bn_node,
-                                      update_kernel_for_bn_folding_fn,
-                                      KERNEL,
-                                      BIAS,
-                                      GAMMA,
-                                      BETA,
-                                      MOVING_MEAN,
-                                      MOVING_VARIANCE,
-                                      EPSILON,
-                                      USE_BIAS,
-                                      layer_name_str=None,  # torch.nn.Modules don't have an attribute 'name'
-                                      )
+    bn_node, source_node = batchnorm_refusing_node_matchers()
+    return BatchNormalizationRefusing(source_node, bn_node, update_kernel_for_bn_folding_fn, KERNEL, BIAS, GAMMA, BETA,
+                                      MOVING_MEAN, MOVING_VARIANCE, EPSILON, USE_BIAS, layer_name_str=None)
```

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/kpi_data_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from model_compression_toolkit.core.common.similarity_analyzer import compute_mse, compute_kl_divergence, compute_cs
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework import get_pytorch_model_builder
 from model_compression_toolkit.core.pytorch.back2framework.model_gradients import \
     pytorch_iterative_approx_jacobian_trace
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.batchnorm_folding import \
-    pytorch_batchnorm_folding
+    pytorch_batchnorm_folding, pytorch_batchnorm_forward_folding
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.batchnorm_reconstruction import \
     pytorch_batchnorm_reconstruction
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.batchnorm_refusing import \
     pytorch_batchnorm_refusing
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.linear_collapsing import \
     pytorch_linear_collapsing
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.multi_head_attention_decomposition \
@@ -239,15 +239,16 @@
                                                     ) -> List[common.BaseSubstitution]:
         """
         Args:
             quant_config: QuantizationConfig to determine which substitutions to return.
 
         Returns: A list of the framework substitutions used before we build a quantized module.
         """
-        substitutions_list = [pytorch_batchnorm_folding()]
+        substitutions_list = [pytorch_batchnorm_folding(),
+                              pytorch_batchnorm_forward_folding()]
         if quant_config.relu_bound_to_power_of_2:
             substitutions_list.append(ReLUBoundToPowerOfTwo())
         return substitutions_list
 
     def get_substitutions_statistics_correction(self, quant_config: QuantizationConfig
                                                 ) -> List[common.BaseSubstitution]:
         """
```

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/core/runner.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/gptq/runner.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/legacy/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/legacy/keras_quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/legacy/keras_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/legacy/pytorch_quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/legacy/pytorch_quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/logger.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/ptq/runner.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-1.9.0.20230626.post508/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.9.0.20230625.post502/setup.py` & `mct-nightly-1.9.0.20230626.post508/setup.py`

 * *Files identical despite different names*

