# Comparing `tmp/alchemite_apiclient-0.55.0.tar.gz` & `tmp/alchemite_apiclient-0.56.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemite_apiclient-0.55.0.tar", last modified: Wed Jun  7 09:52:41 2023, max compression
+gzip compressed data, was "alchemite_apiclient-0.56.0.tar", last modified: Tue Jun 27 15:47:49 2023, max compression
```

## Comparing `alchemite_apiclient-0.55.0.tar` & `alchemite_apiclient-0.56.0.tar`

### file list

```diff
@@ -1,584 +1,580 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.447537 alchemite_apiclient-0.55.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-06-07 09:52:41.447537 alchemite_apiclient-0.55.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4232 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.339536 alchemite_apiclient-0.55.0/alchemite_apiclient/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22601 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.343536 alchemite_apiclient-0.55.0/alchemite_apiclient/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112942 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/api/datasets_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35604 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/api/default_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5200 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/api/metrics_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    58820 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/api/model_dataset_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   239467 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/api/models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37770 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/api_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.343536 alchemite_apiclient-0.55.0/alchemite_apiclient/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17318 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5079 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13896 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/extensions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.383536 alchemite_apiclient-0.55.0/alchemite_apiclient/model/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14502 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/additive_sensitivity_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15940 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12717 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24816 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18046 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12124 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15273 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11771 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14958 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column_info_stats.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17661 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13506 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11411 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11432 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11554 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_batch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11605 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13897 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11120 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_response_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11587 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11749 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_value_nullable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15595 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11760 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_column_info_stats.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16839 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12255 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11280 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27957 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11519 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset1.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14079 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_or_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11454 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14432 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12022 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11619 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_request_sort.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11888 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11530 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_response_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14166 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14730 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14585 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14493 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14338 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15173 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14716 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14627 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14486 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12802 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12505 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dimensionality_reduction_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12947 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dimensionality_reduction_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12516 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13100 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13072 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11829 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12971 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_model_reduction_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11523 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_one_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12103 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_three_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11810 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_two_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11759 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/drpca_reduction_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13502 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/drumap_reduction_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12701 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/empty_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12903 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/empty_continuous_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12586 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/error.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11685 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_all_opt_jobs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15543 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11951 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15300 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11638 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15422 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_optimizing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11784 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15176 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11437 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16376 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11926 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16185 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16061 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11464 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16265 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11778 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16322 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11906 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16031 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16235 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16295 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11896 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16215 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11746 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16016 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16220 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11435 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_categorical_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12150 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_scalar_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10976 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_target_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11839 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_vector_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12403 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_vector_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12954 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/importance_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13832 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/impute_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11377 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/int_cat_arr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/job_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11133 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/load_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34713 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18541 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/model_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11754 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/model_permitted_column_relationships.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10999 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/models_dataset_put_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11775 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12259 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14076 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11795 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14640 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12340 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11409 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14495 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12142 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11451 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14403 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_product.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12061 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11607 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14248 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15083 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12869 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11581 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14626 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12265 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11958 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14537 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12178 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11981 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14354 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12440 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/non_empty_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12381 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/non_empty_continuous_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17508 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/optimize_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12405 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12087 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_sample_def_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10877 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_set_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13043 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/outliers_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13158 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12571 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11980 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11919 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11857 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11129 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_univariate_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11449 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_dependent_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12668 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11837 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13493 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13473 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13463 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_new_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13513 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11670 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14407 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13421 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13415 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/predict_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12027 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16555 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/query_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14001 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/query_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12844 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10940 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16961 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_composition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15367 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_composition_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12213 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14847 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12546 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_discrete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_integer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11515 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_start_prop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12389 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10958 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/scalar_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11456 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/scalar_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13086 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/sensitivity_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10871 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/set_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11163 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/share_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12266 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11045 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_def_categorical_column_values.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12135 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_def_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11386 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/string_cat_arr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23791 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24667 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11828 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11688 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13065 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15809 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13828 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_result_samples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12045 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15023 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11821 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17283 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11679 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13582 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19333 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11439 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19913 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12068 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21491 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13609 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23011 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14071 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_specific.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17421 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11507 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17938 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11673 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_include_categories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16619 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11624 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16767 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10952 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/target_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23224 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/train_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11148 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/training_dataset_outliers_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/validate_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12755 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/validation_split.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12070 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/vector_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12058 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/vector_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12055 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/vector_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model/version_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    82086 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/model_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.383536 alchemite_apiclient-0.55.0/alchemite_apiclient/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21772 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14208 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/alchemite_apiclient/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.339536 alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-06-07 09:52:41.000000 alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23621 2023-06-07 09:52:41.000000 alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-07 09:52:41.000000 alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-07 09:52:41.000000 alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-06-07 09:52:41.000000 alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.435536 alchemite_apiclient-0.55.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/AdditiveSensitivityRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1477 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/AnalyseValidateRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1123 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/AnalyseValidateRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5720 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/AnalyseValidateResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2764 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/AnalyseValidateResponseColumnAnalytics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      990 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalColumnInfoStats.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2073 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1557 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/CategoricalResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnGroupBatchRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      720 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnGroupPatchRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      600 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnGroupRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnGroupResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      545 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnGroupResponseAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      624 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ColumnValueNullable.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ContinuousColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      582 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ContinuousColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ContinuousColumnInfoStats.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1676 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ContinuousModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ContinuousModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      802 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRDatasetReductionData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRDatasetReductionMetadata.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRDatasetReductionMetadataSources.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRJobReductionMetadata.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRJobReductionMetadataSources.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1016 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRModelReductionData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DROneDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRPCAReductionType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRThreeDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRTwoDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DRUMAPReductionType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      578 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/Data.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7250 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/Dataset.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/Dataset1.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetChunk.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetOrData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetQueryRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetQueryRequestRowIDs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetQueryRequestSort.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetQueryResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetQueryResponseResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61432 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DatasetsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18436 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DefaultApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgCol.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgColWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgConstantSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      731 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgProduct.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      737 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      772 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      661 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DependentColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DimensionalityReductionRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/DimensionalityReductionResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      881 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/EmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/EmptyContinuousColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/Error.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetAllOptJobs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizeDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizeDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizeFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizeFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizeOptimizing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizeOptimizingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizePending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetOptimizePendingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalPendingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalRunningAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestHistoricDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestHistoricDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestHistoricFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1144 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestHistoricPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1186 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestHistoricRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestInitialDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestInitialDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1210 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestInitialFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestInitialFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestInitialPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/GetSuggestInitialRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/HistoricCategoricalPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/HistoricPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/HistoricScalarPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/HistoricTargetFunction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/HistoricValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/HistoricVectorPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/HistoricVectorValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ImportanceRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1583 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ImputeRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/IntCatArr.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/JobPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/LoadRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/MetricsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7976 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/Model.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34815 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelDatasetApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)   143019 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelsDatasetPutRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelsIdAdditiveSensitivityOrigin.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ModelsIdTrainPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgCol.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgColAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgColWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgColWeightsAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgColWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgConstantSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgConstantSumAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgConstantSumAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgProduct.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgProductAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgProductAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      719 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgRatioAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgSummandsWeightsAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      754 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedConstSumAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedRatioAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NewColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      770 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NonEmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      843 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NonEmptyContinuousColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/NonEmptyIntegerCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1254 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OTSampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OTSampleDefContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OTSampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      494 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OTSetInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2953 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OptimizeRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutliersRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutputToleranceRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutputToleranceResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutputToleranceResponseFixedInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutputToleranceResponsePredictedOutputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutputToleranceResponsePredictions.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      741 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutputToleranceResponseSampledInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/OutputToleranceUnivariateResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartDependentColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartGetOptimize.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartGetOptimizeDoneResultArray.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1099 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartGetSuggestAdditional.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartGetSuggestHistoric.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartGetSuggestInitial.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartNewColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartTarFnAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartTarFnBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartTarFnBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartTarFnCategoricals.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1968 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartTarFnSingleTar.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartTarFnSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PartTarFnWeightedSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/PredictRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/Prediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/QueryRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/QueryResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      771 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SISampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      538 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SISampleDefCategoricalColumnValues.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SISampleDefContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SISampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefCategoricalColumnValues.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2029 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefComposition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefCompositionAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefContinuousWithStart.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefDiscrete.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefInteger.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefStartProp.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefWeightedCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ScalarPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ScalarResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SensitivityRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SetInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ShareGroup.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/StringCatArr.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4837 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestAdditionalParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3870 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestAdditionalParametersAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestAdditionalRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestAdditionalRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestAdditionalResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestHistoricParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestHistoricRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestHistoricResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1358 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestHistoricResultSamples.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestInitialParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestInitialRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      740 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestInitialRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestInitialResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      393 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestInitialResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingCommon.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2955 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingDataAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3155 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingDatasetID.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      848 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingDatasetIDAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4011 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingImputedData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingImputedDataAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4589 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/SuggestMissingSpecific.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2226 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnExcludeCategories.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnExcludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnIncludeCategories.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnIncludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnSumAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnSumAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnSumBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnSumBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1828 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnSumBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnSumBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnWeightedSumAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnWeightedSumAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnWeightedSumBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnWeightedSumBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnWeightedSumBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TarFnWeightedSumBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1218 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TargetFunction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5666 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TrainRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/TrainingDatasetOutliersRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ValidateRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1096 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/ValidationSplit.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/Value.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/VectorPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/VectorResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/VectorValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/docs/VersionResponse.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.443537 alchemite_apiclient-0.55.0/example/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   701201 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/adrenergic.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)   243835 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/adrenergic_holdout.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/adrenergic_row.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/categorical.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/credentials_auth_code_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/credentials_client_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/credentials_pass_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/credentials_pass_prompted_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4566 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_additive_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3944 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2775 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4120 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_column_groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_connect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5769 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_custom_validation_splits.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5634 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_dimensionality_reduction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_download.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_export_import.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_hyperopt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3833 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_importance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5574 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4774 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_output_tolerance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4511 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_preload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4053 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4504 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5511 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5547 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1980 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4598 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_suggest_missing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3419 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_training_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_validate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5496 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/example_vector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/optimize_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/optimize_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1290 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/optimize_dependentColumns_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/steels.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/steels_impute.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/suggest_additional_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/suggest_additional_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/suggest_historic_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/suggest_historic_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/suggest_initial_args.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/example/vector.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-07 09:52:41.447537 alchemite_apiclient-0.55.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1178 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 09:52:41.447537 alchemite_apiclient-0.55.0/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/test/test_cornercases.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-06-07 09:52:34.000000 alchemite_apiclient-0.55.0/test/test_examples.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.283194 alchemite_apiclient-0.56.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-06-27 15:47:49.283194 alchemite_apiclient-0.56.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4232 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.211194 alchemite_apiclient-0.56.0/alchemite_apiclient/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22403 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.211194 alchemite_apiclient-0.56.0/alchemite_apiclient/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   111028 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/api/datasets_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34995 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/api/default_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5113 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/api/metrics_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57863 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/api/model_dataset_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   235552 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/api/models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37770 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/api_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.211194 alchemite_apiclient-0.56.0/alchemite_apiclient/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17318 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5079 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15773 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/extensions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.247194 alchemite_apiclient-0.56.0/alchemite_apiclient/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14502 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/additive_sensitivity_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15940 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12717 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24816 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18046 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12124 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15273 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11771 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14958 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column_info_stats.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17661 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13506 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11411 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11432 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11554 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_batch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11605 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13897 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11120 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_response_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11587 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11749 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_value_nullable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15595 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11760 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_column_info_stats.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16839 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12255 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11280 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27957 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11519 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset1.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14079 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_or_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11454 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14432 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12022 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11619 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_request_sort.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11888 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11530 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_response_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14166 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14730 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14585 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14493 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14338 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15173 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14716 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14627 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14486 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12802 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12505 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dimensionality_reduction_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12947 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dimensionality_reduction_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12516 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13100 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13072 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11829 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12971 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_model_reduction_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11523 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_one_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12103 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_three_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11810 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_two_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11759 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/drpca_reduction_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13502 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/drumap_reduction_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12701 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/empty_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12903 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/empty_continuous_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12586 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/error.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11685 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_all_opt_jobs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15543 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11951 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15300 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11638 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15422 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_optimizing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11784 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15176 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11437 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16376 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11926 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16185 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16061 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11464 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16265 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11778 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16322 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11906 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16031 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16235 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16295 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11896 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16215 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11746 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16016 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16220 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11435 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_categorical_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12150 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_scalar_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10976 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_target_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11839 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_vector_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12403 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_vector_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12954 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/importance_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13832 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/impute_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11377 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/int_cat_arr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/job_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11133 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/load_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34713 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18541 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/model_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11754 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/model_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10999 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/models_dataset_put_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11775 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12259 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14076 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11795 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14640 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12340 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11409 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14495 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12142 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11451 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14403 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12061 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11607 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14248 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15083 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12869 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11581 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14626 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12265 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11958 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14537 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12178 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11981 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14354 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12440 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/non_empty_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12381 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/non_empty_continuous_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17508 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/optimize_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12405 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12087 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_sample_def_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10877 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_set_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13043 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/outliers_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13158 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12571 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11980 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11919 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11857 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11129 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_univariate_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11449 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_dependent_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12668 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11837 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13493 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13473 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13463 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_new_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13513 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11670 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14407 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13421 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13415 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/predict_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12027 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16555 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/query_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14001 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/query_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12844 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10940 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16961 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_composition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15367 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_composition_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12213 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14847 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12546 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_discrete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_integer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11515 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_start_prop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12389 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10958 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/scalar_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11456 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/scalar_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13086 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/sensitivity_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10871 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/set_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11163 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/share_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12251 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/si_sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/si_sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11386 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/string_cat_arr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23791 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24667 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11828 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11688 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13065 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15809 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13828 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_result_samples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12045 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15023 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11821 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17283 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11679 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13582 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19333 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11439 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19913 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12068 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21491 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13609 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23011 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14071 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_specific.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17421 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11507 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17938 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11673 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_include_categories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16619 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11624 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16767 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10952 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/target_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23224 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/train_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11148 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/training_dataset_outliers_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/validate_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12755 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/validation_split.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12070 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/vector_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12058 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/vector_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12055 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/vector_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model/version_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    82086 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/model_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.247194 alchemite_apiclient-0.56.0/alchemite_apiclient/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21574 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14208 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/alchemite_apiclient/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.211194 alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-06-27 15:47:49.000000 alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23425 2023-06-27 15:47:49.000000 alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 15:47:49.000000 alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-27 15:47:49.000000 alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-06-27 15:47:49.000000 alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.275194 alchemite_apiclient-0.56.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/AdditiveSensitivityRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1477 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/AnalyseValidateRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1123 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/AnalyseValidateRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5720 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/AnalyseValidateResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2764 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/AnalyseValidateResponseColumnAnalytics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      990 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalColumnInfoStats.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2073 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1557 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/CategoricalResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnGroupBatchRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      720 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnGroupPatchRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      600 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnGroupRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnGroupResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      545 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnGroupResponseAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      624 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ColumnValueNullable.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ContinuousColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      582 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ContinuousColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ContinuousColumnInfoStats.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1676 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ContinuousModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ContinuousModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      802 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRDatasetReductionData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRDatasetReductionMetadata.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRDatasetReductionMetadataSources.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRJobReductionMetadata.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRJobReductionMetadataSources.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1016 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRModelReductionData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DROneDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRPCAReductionType.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRThreeDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRTwoDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DRUMAPReductionType.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      578 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/Data.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7250 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/Dataset.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/Dataset1.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetChunk.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetOrData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetQueryRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetQueryRequestRowIDs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetQueryRequestSort.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetQueryResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetQueryResponseResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61432 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DatasetsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18436 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DefaultApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgCol.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgColWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      731 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgProduct.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      737 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      772 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      661 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DependentColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DimensionalityReductionRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/DimensionalityReductionResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      881 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/EmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/EmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/Error.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetAllOptJobs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizeDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizeDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizeFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizeFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizeOptimizing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizeOptimizingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizePending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetOptimizePendingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalPendingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalRunningAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestHistoricDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestHistoricDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestHistoricFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1144 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestHistoricPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1186 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestHistoricRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestInitialDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestInitialDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1210 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestInitialFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestInitialFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestInitialPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/GetSuggestInitialRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/HistoricCategoricalPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/HistoricPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/HistoricScalarPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/HistoricTargetFunction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/HistoricValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/HistoricVectorPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/HistoricVectorValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ImportanceRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1583 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ImputeRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/IntCatArr.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/JobPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/LoadRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/MetricsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7976 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/Model.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34815 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelDatasetApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   143019 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelsDatasetPutRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelsIdAdditiveSensitivityOrigin.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ModelsIdTrainPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgCol.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgColAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgColWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgColWeightsAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgColWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgConstantSumAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgConstantSumAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgProduct.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgProductAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgProductAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      719 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgRatioAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgSummandsWeightsAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      754 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedConstSumAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedRatioAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NewColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      770 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NonEmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      843 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NonEmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/NonEmptyIntegerCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1254 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OTSampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OTSampleDefContinuous.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OTSampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      494 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OTSetInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2953 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OptimizeRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutliersRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutputToleranceRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutputToleranceResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutputToleranceResponseFixedInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutputToleranceResponsePredictedOutputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutputToleranceResponsePredictions.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      741 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutputToleranceResponseSampledInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/OutputToleranceUnivariateResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartDependentColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartGetOptimize.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartGetOptimizeDoneResultArray.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1099 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartGetSuggestAdditional.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartGetSuggestHistoric.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartGetSuggestInitial.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartNewColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartTarFnAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartTarFnBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartTarFnBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartTarFnCategoricals.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1968 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartTarFnSingleTar.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartTarFnSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PartTarFnWeightedSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/PredictRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/Prediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/QueryRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/QueryResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SISampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SISampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefCategoricalColumnValues.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2029 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefComposition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefCompositionAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefContinuous.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefContinuousWithStart.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefDiscrete.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefInteger.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefStartProp.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefWeightedCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ScalarPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ScalarResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SensitivityRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SetInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ShareGroup.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/StringCatArr.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4837 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestAdditionalParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3870 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestAdditionalParametersAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestAdditionalRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestAdditionalRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestAdditionalResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestHistoricParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestHistoricRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestHistoricResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1358 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestHistoricResultSamples.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestInitialParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestInitialRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      740 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestInitialRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestInitialResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      393 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestInitialResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingCommon.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2955 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingDataAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3155 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingDatasetID.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      848 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingDatasetIDAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4011 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingImputedData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingImputedDataAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4589 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/SuggestMissingSpecific.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2226 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnExcludeCategories.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnExcludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnIncludeCategories.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnIncludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnSumAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnSumAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnSumBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnSumBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1828 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnSumBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnWeightedSumAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnWeightedSumAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1218 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TargetFunction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5666 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TrainRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/TrainingDatasetOutliersRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ValidateRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1096 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/ValidationSplit.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/Value.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/VectorPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/VectorResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/VectorValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/docs/VersionResponse.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.283194 alchemite_apiclient-0.56.0/example/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   701201 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/adrenergic.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   243835 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/adrenergic_holdout.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/adrenergic_row.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/categorical.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/credentials_auth_code_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/credentials_client_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/credentials_pass_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/credentials_pass_prompted_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4566 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_additive_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3944 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2775 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4120 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_column_groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_connect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5769 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_custom_validation_splits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5634 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_dimensionality_reduction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_download.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_export_import.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_hyperopt.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3833 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_importance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5574 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4774 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_output_tolerance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4511 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_preload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4053 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4504 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5511 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5547 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1980 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4598 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_suggest_missing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3419 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_training_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_validate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5496 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/example_vector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/optimize_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/optimize_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1290 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/optimize_dependentColumns_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/steels.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/steels_impute.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/suggest_additional_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/suggest_additional_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/suggest_historic_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/suggest_historic_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/suggest_initial_args.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/example/vector.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-27 15:47:49.283194 alchemite_apiclient-0.56.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1178 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 15:47:49.283194 alchemite_apiclient-0.56.0/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/test/test_cornercases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-06-27 15:47:43.000000 alchemite_apiclient-0.56.0/test/test_examples.py
```

### Comparing `alchemite_apiclient-0.55.0/PKG-INFO` & `alchemite_apiclient-0.56.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite_apiclient
-Version: 0.55.0
+Version: 0.56.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -19,15 +19,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.55.0
+API version: 0.56.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.55.0/README.md` & `alchemite_apiclient-0.56.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.55.0
+API version: 0.56.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/__init__.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
     Contact: support@intellegens.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.55.0"
+__version__ = "0.56.0"
 
 # import ApiClient
 from alchemite_apiclient.api_client import ApiClient
 
 # import Configuration
 from alchemite_apiclient.configuration import Configuration
 
@@ -203,16 +203,14 @@
 from alchemite_apiclient.model.part_tar_fn_sum import PartTarFnSum
 from alchemite_apiclient.model.part_tar_fn_weighted_sum import PartTarFnWeightedSum
 from alchemite_apiclient.model.predict_request import PredictRequest
 from alchemite_apiclient.model.prediction import Prediction
 from alchemite_apiclient.model.query_request import QueryRequest
 from alchemite_apiclient.model.query_response import QueryResponse
 from alchemite_apiclient.model.si_sample_def_categorical import SISampleDefCategorical
-from alchemite_apiclient.model.si_sample_def_categorical_column_values import SISampleDefCategoricalColumnValues
-from alchemite_apiclient.model.si_sample_def_continuous import SISampleDefContinuous
 from alchemite_apiclient.model.si_sample_definition import SISampleDefinition
 from alchemite_apiclient.model.sample_def_categorical import SampleDefCategorical
 from alchemite_apiclient.model.sample_def_categorical_column_values import SampleDefCategoricalColumnValues
 from alchemite_apiclient.model.sample_def_composition import SampleDefComposition
 from alchemite_apiclient.model.sample_def_composition_all_of import SampleDefCompositionAllOf
 from alchemite_apiclient.model.sample_def_continuous import SampleDefContinuous
 from alchemite_apiclient.model.sample_def_continuous_with_start import SampleDefContinuousWithStart
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/api/datasets_api.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/api/datasets_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,14 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.datasets_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([Dataset],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets',
                 'operation_id': 'datasets_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -91,17 +88,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_chunks_chunk_number_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/chunks/{chunk_number}',
                 'operation_id': 'datasets_id_chunks_chunk_number_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -151,17 +145,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_chunks_chunk_number_get_endpoint = _Endpoint(
             settings={
                 'response_type': (DatasetChunk,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/chunks/{chunk_number}',
                 'operation_id': 'datasets_id_chunks_chunk_number_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -211,17 +202,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_chunks_chunk_number_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/chunks/{chunk_number}',
                 'operation_id': 'datasets_id_chunks_chunk_number_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -277,17 +265,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_chunks_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/chunks',
                 'operation_id': 'datasets_id_chunks_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -331,17 +316,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_chunks_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([DatasetChunk],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/chunks',
                 'operation_id': 'datasets_id_chunks_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -385,17 +367,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_column_groups_batch_post_endpoint = _Endpoint(
             settings={
                 'response_type': ([str],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/column-groups/batch',
                 'operation_id': 'datasets_id_column_groups_batch_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -447,17 +426,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_column_groups_column_group_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/column-groups/{column_group_id}',
                 'operation_id': 'datasets_id_column_groups_column_group_id_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -507,17 +483,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_column_groups_column_group_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (ColumnGroupResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/column-groups/{column_group_id}',
                 'operation_id': 'datasets_id_column_groups_column_group_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -567,17 +540,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_column_groups_column_group_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/column-groups/{column_group_id}',
                 'operation_id': 'datasets_id_column_groups_column_group_id_patch',
                 'http_method': 'PATCH',
                 'servers': None,
             },
@@ -633,17 +603,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_column_groups_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([ColumnGroupResponse],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/column-groups',
                 'operation_id': 'datasets_id_column_groups_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -687,17 +654,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_column_groups_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/column-groups',
                 'operation_id': 'datasets_id_column_groups_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -749,17 +713,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}',
                 'operation_id': 'datasets_id_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -803,17 +764,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_dimensionality_reduction_put_endpoint = _Endpoint(
             settings={
                 'response_type': (DimensionalityReductionResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/dimensionality-reduction',
                 'operation_id': 'datasets_id_dimensionality_reduction_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -863,17 +821,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_download_get_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/download',
                 'operation_id': 'datasets_id_download_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -918,17 +873,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (Dataset,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}',
                 'operation_id': 'datasets_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -972,17 +924,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}',
                 'operation_id': 'datasets_id_patch',
                 'http_method': 'PATCH',
                 'servers': None,
             },
@@ -1032,17 +981,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_share_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/share',
                 'operation_id': 'datasets_id_share_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -1093,17 +1039,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_share_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([str],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/share',
                 'operation_id': 'datasets_id_share_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -1147,17 +1090,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_share_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/share',
                 'operation_id': 'datasets_id_share_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -1208,17 +1148,14 @@
             },
             api_client=api_client
         )
         self.datasets_id_uploaded_post_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets/{id}/uploaded',
                 'operation_id': 'datasets_id_uploaded_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -1262,17 +1199,14 @@
             },
             api_client=api_client
         )
         self.datasets_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/datasets',
                 'operation_id': 'datasets_post',
                 'http_method': 'POST',
                 'servers': None,
             },
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/api/default_api.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/api/default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,14 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.query_v1_put_endpoint = _Endpoint(
             settings={
                 'response_type': (QueryResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/query/v1',
                 'operation_id': 'query_v1_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -116,17 +113,14 @@
             },
             api_client=api_client
         )
         self.suggest_initial_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([SuggestInitialResponse],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/suggest-initial',
                 'operation_id': 'suggest_initial_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -163,17 +157,14 @@
             },
             api_client=api_client
         )
         self.suggest_initial_job_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/suggest-initial/{job_id}',
                 'operation_id': 'suggest_initial_job_id_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -217,17 +208,14 @@
             },
             api_client=api_client
         )
         self.suggest_initial_job_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (SuggestInitialResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/suggest-initial/{job_id}',
                 'operation_id': 'suggest_initial_job_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -271,17 +259,14 @@
             },
             api_client=api_client
         )
         self.suggest_initial_job_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/suggest-initial/{job_id}',
                 'operation_id': 'suggest_initial_job_id_patch',
                 'http_method': 'PATCH',
                 'servers': None,
             },
@@ -331,17 +316,14 @@
             },
             api_client=api_client
         )
         self.suggest_initial_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/suggest-initial',
                 'operation_id': 'suggest_initial_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -387,17 +369,14 @@
             },
             api_client=api_client
         )
         self.version_get_endpoint = _Endpoint(
             settings={
                 'response_type': (VersionResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/version',
                 'operation_id': 'version_get',
                 'http_method': 'GET',
                 'servers': None,
             },
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/api/metrics_api.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/api/metrics_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,14 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.metrics_get_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/metrics',
                 'operation_id': 'metrics_get',
                 'http_method': 'GET',
                 'servers': None,
             },
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/api/model_dataset_api.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/api/model_dataset_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,14 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.models_id_dataset_chunks_chunk_number_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset/chunks/{chunk_number}',
                 'operation_id': 'models_id_dataset_chunks_chunk_number_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -97,17 +94,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_chunks_chunk_number_get_endpoint = _Endpoint(
             settings={
                 'response_type': (DatasetChunk,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset/chunks/{chunk_number}',
                 'operation_id': 'models_id_dataset_chunks_chunk_number_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -157,17 +151,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_chunks_chunk_number_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset/chunks/{chunk_number}',
                 'operation_id': 'models_id_dataset_chunks_chunk_number_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -223,17 +214,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_chunks_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset/chunks',
                 'operation_id': 'models_id_dataset_chunks_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -277,17 +265,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_chunks_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([DatasetChunk],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset/chunks',
                 'operation_id': 'models_id_dataset_chunks_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -331,17 +316,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset',
                 'operation_id': 'models_id_dataset_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -385,17 +367,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_download_get_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset/download',
                 'operation_id': 'models_id_dataset_download_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -440,17 +419,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_get_endpoint = _Endpoint(
             settings={
                 'response_type': (Dataset,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset',
                 'operation_id': 'models_id_dataset_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -494,17 +470,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset',
                 'operation_id': 'models_id_dataset_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -555,17 +528,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset',
                 'operation_id': 'models_id_dataset_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -615,17 +585,14 @@
             },
             api_client=api_client
         )
         self.models_id_dataset_uploaded_post_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/dataset/uploaded',
                 'operation_id': 'models_id_dataset_uploaded_post',
                 'http_method': 'POST',
                 'servers': None,
             },
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/api/models_api.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/api/models_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,17 +71,14 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.models_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([Model],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models',
                 'operation_id': 'models_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -118,17 +115,14 @@
             },
             api_client=api_client
         )
         self.models_id_additive_sensitivity_put_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/additive-sensitivity',
                 'operation_id': 'models_id_additive_sensitivity_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -179,17 +173,14 @@
             },
             api_client=api_client
         )
         self.models_id_analyse_validate_put_endpoint = _Endpoint(
             settings={
                 'response_type': (AnalyseValidateResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/analyse-validate',
                 'operation_id': 'models_id_analyse_validate_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -239,17 +230,14 @@
             },
             api_client=api_client
         )
         self.models_id_copy_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/copy',
                 'operation_id': 'models_id_copy_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -294,17 +282,14 @@
             },
             api_client=api_client
         )
         self.models_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}',
                 'operation_id': 'models_id_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -348,17 +333,14 @@
             },
             api_client=api_client
         )
         self.models_id_export_get_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/export',
                 'operation_id': 'models_id_export_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -403,17 +385,14 @@
             },
             api_client=api_client
         )
         self.models_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (Model,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}',
                 'operation_id': 'models_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -457,17 +436,14 @@
             },
             api_client=api_client
         )
         self.models_id_importance_put_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/importance',
                 'operation_id': 'models_id_importance_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -519,17 +495,14 @@
             },
             api_client=api_client
         )
         self.models_id_impute_put_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/impute',
                 'operation_id': 'models_id_impute_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -580,17 +553,14 @@
             },
             api_client=api_client
         )
         self.models_id_load_post_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/load',
                 'operation_id': 'models_id_load_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -640,17 +610,14 @@
             },
             api_client=api_client
         )
         self.models_id_log_get_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/log',
                 'operation_id': 'models_id_log_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -695,17 +662,14 @@
             },
             api_client=api_client
         )
         self.models_id_optimize_get_endpoint = _Endpoint(
             settings={
                 'response_type': (GetAllOptJobs,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/optimize',
                 'operation_id': 'models_id_optimize_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -760,17 +724,14 @@
             },
             api_client=api_client
         )
         self.models_id_optimize_job_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/optimize/{job_id}',
                 'operation_id': 'models_id_optimize_job_id_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -820,17 +781,14 @@
             },
             api_client=api_client
         )
         self.models_id_optimize_job_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/optimize/{job_id}',
                 'operation_id': 'models_id_optimize_job_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -891,17 +849,14 @@
             },
             api_client=api_client
         )
         self.models_id_optimize_job_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/optimize/{job_id}',
                 'operation_id': 'models_id_optimize_job_id_patch',
                 'http_method': 'PATCH',
                 'servers': None,
             },
@@ -957,17 +912,14 @@
             },
             api_client=api_client
         )
         self.models_id_optimize_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/optimize',
                 'operation_id': 'models_id_optimize_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -1019,17 +971,14 @@
             },
             api_client=api_client
         )
         self.models_id_outliers_put_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/outliers',
                 'operation_id': 'models_id_outliers_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -1080,17 +1029,14 @@
             },
             api_client=api_client
         )
         self.models_id_output_tolerance_put_endpoint = _Endpoint(
             settings={
                 'response_type': (OutputToleranceResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/output-tolerance',
                 'operation_id': 'models_id_output_tolerance_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -1140,17 +1086,14 @@
             },
             api_client=api_client
         )
         self.models_id_output_tolerance_univariate_put_endpoint = _Endpoint(
             settings={
                 'response_type': (OutputToleranceUnivariateResponse,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/output-tolerance-univariate',
                 'operation_id': 'models_id_output_tolerance_univariate_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -1200,17 +1143,14 @@
             },
             api_client=api_client
         )
         self.models_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}',
                 'operation_id': 'models_id_patch',
                 'http_method': 'PATCH',
                 'servers': None,
             },
@@ -1260,17 +1200,14 @@
             },
             api_client=api_client
         )
         self.models_id_predict_put_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/predict',
                 'operation_id': 'models_id_predict_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -1321,17 +1258,14 @@
             },
             api_client=api_client
         )
         self.models_id_sensitivity_put_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/sensitivity',
                 'operation_id': 'models_id_sensitivity_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -1382,17 +1316,14 @@
             },
             api_client=api_client
         )
         self.models_id_share_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/share',
                 'operation_id': 'models_id_share_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -1443,17 +1374,14 @@
             },
             api_client=api_client
         )
         self.models_id_share_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([str],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/share',
                 'operation_id': 'models_id_share_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -1497,17 +1425,14 @@
             },
             api_client=api_client
         )
         self.models_id_share_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/share',
                 'operation_id': 'models_id_share_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -1558,17 +1483,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_additional_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([bool, date, datetime, dict, float, int, list, str, none_type],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-additional',
                 'operation_id': 'models_id_suggest_additional_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -1612,17 +1534,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_additional_job_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-additional/{job_id}',
                 'operation_id': 'models_id_suggest_additional_job_id_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -1672,17 +1591,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_additional_job_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-additional/{job_id}',
                 'operation_id': 'models_id_suggest_additional_job_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -1732,17 +1648,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_additional_job_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-additional/{job_id}',
                 'operation_id': 'models_id_suggest_additional_job_id_patch',
                 'http_method': 'PATCH',
                 'servers': None,
             },
@@ -1798,17 +1711,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_additional_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-additional',
                 'operation_id': 'models_id_suggest_additional_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -1860,17 +1770,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_historic_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([bool, date, datetime, dict, float, int, list, str, none_type],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-historic',
                 'operation_id': 'models_id_suggest_historic_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -1914,17 +1821,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_historic_job_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-historic/{job_id}',
                 'operation_id': 'models_id_suggest_historic_job_id_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
@@ -1974,17 +1878,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_historic_job_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-historic/{job_id}',
                 'operation_id': 'models_id_suggest_historic_job_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -2034,17 +1935,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_historic_job_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-historic/{job_id}',
                 'operation_id': 'models_id_suggest_historic_job_id_patch',
                 'http_method': 'PATCH',
                 'servers': None,
             },
@@ -2100,17 +1998,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_historic_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-historic',
                 'operation_id': 'models_id_suggest_historic_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -2162,17 +2057,14 @@
             },
             api_client=api_client
         )
         self.models_id_suggest_missing_put_endpoint = _Endpoint(
             settings={
                 'response_type': ([SuggestMissingResponse],),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/suggest-missing',
                 'operation_id': 'models_id_suggest_missing_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -2223,17 +2115,14 @@
             },
             api_client=api_client
         )
         self.models_id_train_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/train',
                 'operation_id': 'models_id_train_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -2284,17 +2173,14 @@
             },
             api_client=api_client
         )
         self.models_id_training_dataset_outliers_get_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/training-dataset-outliers',
                 'operation_id': 'models_id_training_dataset_outliers_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -2339,17 +2225,14 @@
             },
             api_client=api_client
         )
         self.models_id_training_dataset_outliers_put_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/training-dataset-outliers',
                 'operation_id': 'models_id_training_dataset_outliers_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -2400,17 +2283,14 @@
             },
             api_client=api_client
         )
         self.models_id_unload_put_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/unload',
                 'operation_id': 'models_id_unload_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -2454,17 +2334,14 @@
             },
             api_client=api_client
         )
         self.models_id_validate_put_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/validate',
                 'operation_id': 'models_id_validate_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
@@ -2515,17 +2392,14 @@
             },
             api_client=api_client
         )
         self.models_id_validation_predictions_get_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/validation-predictions',
                 'operation_id': 'models_id_validation_predictions_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -2570,17 +2444,14 @@
             },
             api_client=api_client
         )
         self.models_id_validation_splits_get_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/validation-splits',
                 'operation_id': 'models_id_validation_splits_get',
                 'http_method': 'GET',
                 'servers': None,
             },
@@ -2624,17 +2495,14 @@
             },
             api_client=api_client
         )
         self.models_import_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models/import',
                 'operation_id': 'models_import_post',
                 'http_method': 'POST',
                 'servers': None,
             },
@@ -2678,17 +2546,14 @@
             },
             api_client=api_client
         )
         self.models_post_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
-                    'oauth',
-                    'oauth',
-                    'oauth',
                     'oauth'
                 ],
                 'endpoint_path': '/models',
                 'operation_id': 'models_post',
                 'http_method': 'POST',
                 'servers': None,
             },
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/api_client.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.55.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.56.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/apis/__init__.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/configuration.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,16 +403,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.55.0\n"\
-               "SDK Package Version: 0.55.0".\
+               "Version of the API: 0.56.0\n"\
+               "SDK Package Version: 0.56.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/exceptions.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/extensions.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/extensions.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 import warnings
 import webbrowser
 from getpass import getpass
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
 import tqdm
 from oauthlib.oauth2 import BackendApplicationClient, LegacyApplicationClient, \
-    OAuth2Error, WebApplicationClient
+    OAuth2Error, WebApplicationClient, InvalidGrantError
 from oauthlib.oauth2.rfc6749.errors import CustomOAuth2Error
 from requests_oauthlib import OAuth2Session
 from requests.adapters import HTTPAdapter
 
 import alchemite_apiclient as client
+from alchemite_apiclient.exceptions import ServiceException
 
 TOKEN_FILE = ".alchemite_token"
 
 try:
     from urllib3.contrib import pyopenssl
 
     # Requests v2.23.0 calls pyopenssl.inject_into_urllib3() to "Monkey-patch
@@ -66,37 +67,39 @@
 </script>
 </body>
 </html>
 """
 
 
 class Configuration(client.Configuration):
-    def __init__(self):
-        self.grant_type = ""
-        self.client_id = ""
+    def __init__(self, *, grant_type="authorization_code", client_id="PythonClient", username="", offline=False):
+        self.grant_type = grant_type
+        self.client_id = client_id
         self.client_secret = ""
-        self.username = ""
+        self.username = username
         self.password = ""
         self.token = {}
         self._session = None
         self._offline_token = None
-        self.offline = False
+        self.offline = offline
+        self._proxy = None
+        self._auth_backoff = False
 
         super(Configuration, self).__init__()
 
     @property
     def token_endpoint(self):
         return self.host + "/auth/realms/master/protocol/openid-connect/token"
 
     @property
     def auth_endpoint(self):
         return self.host + "/auth/realms/master/protocol/openid-connect/auth"
 
-    def token_expired(self):
-        return self.token["expires_at"] - time.time() < 10
+    def token_expired(self, soft=True):
+        return self.token["expires_at"] - time.time() < (10 if soft else 0)
 
     @property
     def session(self):
         if self._session is None:
             if self.grant_type == "client_credentials":
                 client = BackendApplicationClient(client_id=self.client_id)
             elif self.grant_type == "password":
@@ -198,15 +201,14 @@
 
         token = self.session.fetch_token(
             token_url=self.token_endpoint,
             authorization_response=authorization_response.pop(),
             client_id=self.client_id,
             verify=self.verify_ssl,
         )
-
         return token
 
     def try_offline(self):
         if not self.offline:
             return False
         if os.path.exists(TOKEN_FILE):
             with open(TOKEN_FILE, 'r') as file:
@@ -222,15 +224,15 @@
     def save_offline(self, token):
         if not self.offline:
             return
         if token['refresh_token'] == self._offline_token:
             # Nothing to update
             return
         if ('offline_access' in token['scope']
-                and token['refresh_expires_in'] == 0):
+            and token['refresh_expires_in'] == 0):
             self._offline_token = token['refresh_token']
             with open(TOKEN_FILE, 'w') as file:
                 file.write(token['refresh_token'])
 
     def refresh_token(self):
         # Make request with 'grant_type'='refresh_token'
         self.token = self.session.refresh_token(
@@ -241,21 +243,27 @@
         )
         self.save_offline(self.token)
 
     @property
     def access_token(self):
         if not self.token:
             self.token = self.get_token()
-        elif self.token_expired():
-            # try:
-            #     self.refresh_token()
-            # except oauthlib.oauth2.rfc6749.errors.InvalidGrantError:
-            #     # The refresh token has expired or been revoked
-            #     self.token = self.get_token()
-            self.token = self.get_token()
+        elif (self.token_expired() and not self._auth_backoff) or self.token_expired(soft=False):
+            try:
+                self.refresh_token()
+                if self.token["expires_in"] <= 10 and not self._auth_backoff:
+                    # Refresh token expiring, causing auth flooding
+                    self.token = self.get_token()
+                    if self.token['expires_in'] <= 10:
+                        # Fresh token didn't help, so backoff until token fully expires
+                        self._auth_backoff = True
+            except InvalidGrantError:
+                # The refresh token has expired or been revoked
+                self.token = self.get_token()
+                self._auth_backoff = False
 
         return self.token["access_token"]
 
     @access_token.setter
     def access_token(self, val):
         self._access_token = val
 
@@ -278,14 +286,43 @@
                 "If you are not Intellegens staff, please remove 'insecure' from your credentials file to avoid potential security risks"
             )
             # Debug shim
             import os
             os.environ["OAUTHLIB_INSECURE_TRANSPORT"] = "1"
             self.verify_ssl = False
 
+    @property
+    def proxy(self):
+        return self._proxy
+
+    @proxy.setter
+    def proxy(self, val):
+        self._proxy = val
+        if val is not None:
+            os.environ['http_proxy'] = val
+            os.environ['https_proxy'] = val
+
+    def auth_settings(self):
+        """Gets Auth Settings dict for api client.
+
+        Overridden to only do this once (the generator makes 4 of these)
+
+        :return: The Auth Settings information dict.
+        """
+        auth = {}
+        access_token = self.access_token
+        if access_token is not None:
+            auth['oauth'] = {
+                'type': 'oauth2',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + access_token
+            }
+        return auth
+
 
 def await_trained(get_model):
     """
     Block until the model is 'trained' and a print progress bar with updates
 
     Parameters
     ----------
@@ -295,16 +332,25 @@
     Returns
     -------
     Model
         The model metadata after training is completed
     """
 
     with tqdm.tqdm(total=100, unit="%") as pbar:
+        err_count = 0
         while True:
-            model = get_model()
+            try:
+                model = get_model()
+            except ServiceException:
+                err_count += 1
+                if err_count > 60:
+                    raise
+                time.sleep(1)
+                continue
+            err_count = 0
             training_progress = model.training_progress
             hyperopt_progress = model.hyperparameter_optimization_progress
             validation_method = model.validation_method
 
             if training_progress is None:
                 training_progress = 0
 
@@ -314,27 +360,27 @@
             else:
                 progress = (60 * hyperopt_progress + training_progress) / 61
 
             pbar.update(progress - pbar.n)
 
             pbar.set_description(model.status)
             if (
-                    (
-                            model.status == "trained"
-                            and (
-                                    validation_method == "none"
-                                    or model.validation_r_squared is not None
-                            )
-                            and (
-                                    model.training_dataset_outliers_job_id is None
-                                    or model.training_dataset_outliers_job_status == "done"
-                            )
+                (
+                    model.status == "trained"
+                    and (
+                        validation_method == "none"
+                        or model.validation_r_squared is not None
                     )
-                    or model.status == "failed"
-                    or model.training_dataset_outliers_job_status == "failed"
+                    and (
+                        model.training_dataset_outliers_job_id is None
+                        or model.training_dataset_outliers_job_status == "done"
+                    )
+                )
+                or model.status == "failed"
+                or model.training_dataset_outliers_job_status == "failed"
             ):
                 break
             time.sleep(1)
 
     if model.status != "trained":
         raise RuntimeError(f"Model is not trained, status: {model.status}")
 
@@ -364,16 +410,25 @@
     Returns
     -------
     dict
         The optimize job result with metadata
     """
     status = None
     with tqdm.tqdm(total=100, unit="%") as pbar:
+        err_count = 0
         while True:
-            job = get_job()
+            try:
+                job = get_job()
+            except ServiceException:
+                err_count += 1
+                if err_count > 60:
+                    raise
+                time.sleep(1)
+                continue
+            err_count = 0
             status = job["status"]
 
             if "progress" in job:
                 progress = job["progress"]
             elif status == "done":
                 progress = 100
             else:
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/additive_sensitivity_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/additive_sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_request_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column_info.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column_info_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_column_info_stats.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_model_column_info.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/categorical_result.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/categorical_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_batch_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_batch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_patch_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_patch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_group_response_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_group_response_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_info.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_value.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/column_value_nullable.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/column_value_nullable.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_column_info.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_column_info_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_column_info_stats.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_model_column_info.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/data.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset1.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset1.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_chunk.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_or_data.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_or_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_patch.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_request_row_ids.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_request_row_ids.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_request_sort.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_request_sort.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dataset_query_response_result.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dataset_query_response_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dependent_columns.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dimensionality_reduction_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dimensionality_reduction_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dimensionality_reduction_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dimensionality_reduction_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_dataset_reduction_data.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_dataset_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_job_reduction_metadata.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_job_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_model_reduction_data.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_model_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_one_dimension_point.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_one_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_three_dimension_point.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_three_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/dr_two_dimension_point.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/dr_two_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/drpca_reduction_type.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/drpca_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/drumap_reduction_type.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/drumap_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/empty_categorical_column.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/empty_continuous_column.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/error.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/error.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_all_opt_jobs.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_all_opt_jobs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_done.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_done_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_failed.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_failed_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_optimizing.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_optimizing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_pending.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_optimize_pending_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_optimize_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_done.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_failed.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_pending.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_running.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_done.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_failed.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_pending.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_historic_running.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_historic_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_done.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_failed.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_pending.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/get_suggest_initial_running.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/get_suggest_initial_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_categorical_prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_scalar_prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_target_function.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_target_function.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_value.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_vector_prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/historic_vector_value.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/historic_vector_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/importance_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/importance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/impute_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/impute_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/int_cat_arr.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/int_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/job_patch.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/job_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/load_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/load_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/model.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/model.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/model_column_info.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/model_patch.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/model_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/model_permitted_column_relationships.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/model_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/models_dataset_put_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/models_dataset_put_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_product.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/new_columns.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/non_empty_categorical_column.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/non_empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/non_empty_continuous_column.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/non_empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/optimize_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/optimize_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_sample_def_categorical.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_sample_def_continuous.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_sample_definition.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/ot_set_inputs.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/ot_set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/outliers_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/outliers_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_predictions.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_predictions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/output_tolerance_univariate_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/output_tolerance_univariate_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_dependent_columns.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_optimize.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_suggest_additional.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_suggest_historic.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_get_suggest_initial.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_get_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_new_columns.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_above.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_below.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_between.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_categoricals.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_categoricals.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_single_tar.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_single_tar.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_sum.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/predict_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/predict_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/query_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/query_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_categorical.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_categorical_column_values.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_categorical_column_values.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_composition.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_composition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_composition_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_composition_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_continuous.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_continuous_with_start.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_continuous_with_start.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_discrete.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_discrete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_integer.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_integer.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_start_prop.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_start_prop.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_def_weighted_categorical.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_def_weighted_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sample_definition.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/scalar_prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/scalar_result.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/scalar_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/sensitivity_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/set_inputs.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/share_group.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/share_group.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_def_categorical.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/si_sample_def_categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.si_sample_def_categorical_column_values import SISampleDefCategoricalColumnValues
-    globals()['SISampleDefCategoricalColumnValues'] = SISampleDefCategoricalColumnValues
+    from alchemite_apiclient.model.sample_def_categorical_column_values import SampleDefCategoricalColumnValues
+    globals()['SampleDefCategoricalColumnValues'] = SampleDefCategoricalColumnValues
 
 
 class SISampleDefCategorical(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -90,15 +90,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (str,),  # noqa: E501
-            'values': ({str: (SISampleDefCategoricalColumnValues,)},),  # noqa: E501
+            'values': ({str: (SampleDefCategoricalColumnValues,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
@@ -114,15 +114,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, values, *args, **kwargs):  # noqa: E501
         """SISampleDefCategorical - a model defined in OpenAPI
 
         Args:
-            values ({str: (SISampleDefCategoricalColumnValues,)}): Describe the options and accompanying values to choose between.
+            values ({str: (SampleDefCategoricalColumnValues,)}): Describe the options and accompanying values to choose between.
 
         Keyword Args:
             type (str): defaults to "categorical", must be one of ["categorical", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -202,15 +202,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, values, *args, **kwargs):  # noqa: E501
         """SISampleDefCategorical - a model defined in OpenAPI
 
         Args:
-            values ({str: (SISampleDefCategoricalColumnValues,)}): Describe the options and accompanying values to choose between.
+            values ({str: (SampleDefCategoricalColumnValues,)}): Describe the options and accompanying values to choose between.
 
         Keyword Args:
             type (str): defaults to "categorical", must be one of ["categorical", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_def_categorical_column_values.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/si_sample_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 
-class SISampleDefCategoricalColumnValues(ModelNormal):
+class SISampleDefinition(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,15 +55,14 @@
 
     allowed_values = {
     }
 
     validations = {
         ('value',): {
             'min_properties': 1,
-            'max_properties': 1,
         },
     }
 
     @cached_property
     def additional_properties_type():  # noqa
         """
         This must be a method because a model may have properties that are
@@ -98,15 +97,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SISampleDefCategoricalColumnValues - a model defined in OpenAPI
+        """SISampleDefinition - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -179,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SISampleDefCategoricalColumnValues - a model defined in OpenAPI
+        """SISampleDefinition - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_def_continuous.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/value.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from alchemite_apiclient.model.float_none_type import FloatNoneType
+    from alchemite_apiclient.model.vector_value import VectorValue
+    globals()['VectorValue'] = VectorValue
+    globals()['float, none_type'] = float, none_type
 
-class SISampleDefContinuous(ModelNormal):
+
+class Value(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -50,76 +56,71 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'CONTINUOUS': "continuous",
-        },
     }
 
     validations = {
-        ('range',): {
-            'max_items': 2,
-            'min_items': 2,
-        },
     }
 
     @cached_property
     def additional_properties_type():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'range': ([float],),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'range': 'range',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, range, *args, **kwargs):  # noqa: E501
-        """SISampleDefContinuous - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, value, *args, **kwargs):  # noqa: E501
+        """Value - a model defined in OpenAPI
 
         Args:
-            range ([float]): Range is an array consisting of a lower and upper bound where the lower bound is strictly smaller than the upper bound. 
+            name (str): Property's name
+            value (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
-            type (str): Search a continuous domain within the `\"range\"` specified with uniform prior. . defaults to "continuous", must be one of ["continuous", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -144,15 +145,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        type = kwargs.get('type', "continuous")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -170,16 +170,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.range = range
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,22 +192,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, range, *args, **kwargs):  # noqa: E501
-        """SISampleDefContinuous - a model defined in OpenAPI
+    def __init__(self, name, value, *args, **kwargs):  # noqa: E501
+        """Value - a model defined in OpenAPI
 
         Args:
-            range ([float]): Range is an array consisting of a lower and upper bound where the lower bound is strictly smaller than the upper bound. 
+            name (str): Property's name
+            value (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
-            type (str): Search a continuous domain within the `\"range\"` specified with uniform prior. . defaults to "continuous", must be one of ["continuous", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -232,15 +232,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        type = kwargs.get('type', "continuous")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -256,16 +255,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.range = range
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/si_sample_definition.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/target_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 
-class SISampleDefinition(ModelNormal):
+class TargetFunction(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -97,15 +97,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SISampleDefinition - a model defined in OpenAPI
+        """TargetFunction - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -178,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SISampleDefinition - a model defined in OpenAPI
+        """TargetFunction - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/string_cat_arr.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/string_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_parameters.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_request_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_additional_result.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_additional_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_parameters.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_result.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_historic_result_samples.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_historic_result_samples.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_parameters.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_request_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_initial_result.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_initial_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_common.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_common.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_data.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_data_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_dataset_id.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_dataset_id.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_imputed_data.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_imputed_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_response.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/suggest_missing_specific.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/suggest_missing_specific.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_above.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_above_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_below.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_below_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_between.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_between_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_exclude_categories.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_exclude_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_include_categories.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_include_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_above.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_below.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_between.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/target_function.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/training_dataset_outliers_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 
-class TargetFunction(ModelNormal):
+class TrainingDatasetOutliersRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -53,59 +53,55 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('value',): {
-            'min_properties': 1,
+        ('row_ids',): {
+            'min_items': 1,
         },
     }
 
-    @cached_property
-    def additional_properties_type():  # noqa
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'row_ids': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
+        'row_ids': 'rowIDs',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TargetFunction - a model defined in OpenAPI
+        """TrainingDatasetOutliersRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,14 +126,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            row_ids ([str]): The IDs of the rows to return outliers for. If not given then outliers for all rows in the dataset will be returned.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +175,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TargetFunction - a model defined in OpenAPI
+        """TrainingDatasetOutliersRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -211,14 +208,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            row_ids ([str]): The IDs of the rows to return outliers for. If not given then outliers for all rows in the dataset will be returned.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/train_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/train_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/training_dataset_outliers_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/version_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 
-class TrainingDatasetOutliersRequest(ModelNormal):
+class VersionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -53,55 +53,62 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('row_ids',): {
-            'min_items': 1,
-        },
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():  # noqa
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'row_ids': ([str],),  # noqa: E501
+            'api_definition_version': (str,),  # noqa: E501
+            'api_application_version': (str,),  # noqa: E501
+            'alchemite_version': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'row_ids': 'rowIDs',  # noqa: E501
+        'api_definition_version': 'APIDefinitionVersion',  # noqa: E501
+        'api_application_version': 'APIApplicationVersion',  # noqa: E501
+        'alchemite_version': 'AlchemiteVersion',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TrainingDatasetOutliersRequest - a model defined in OpenAPI
+        """VersionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,15 +133,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            row_ids ([str]): The IDs of the rows to return outliers for. If not given then outliers for all rows in the dataset will be returned.. [optional]  # noqa: E501
+            api_definition_version (str): The version of the API definition in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            api_application_version (str): The version of the running API application in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            alchemite_version (str): The current version of Alchemite.  Note that existing models trained on older versions will have to be retrained to take advantage of the latest version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -175,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TrainingDatasetOutliersRequest - a model defined in OpenAPI
+        """VersionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -208,15 +217,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            row_ids ([str]): The IDs of the rows to return outliers for. If not given then outliers for all rows in the dataset will be returned.. [optional]  # noqa: E501
+            api_definition_version (str): The version of the API definition in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            api_application_version (str): The version of the running API application in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            alchemite_version (str): The current version of Alchemite.  Note that existing models trained on older versions will have to be retrained to take advantage of the latest version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/validate_request.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/validate_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/validation_split.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/validation_split.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/value.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/vector_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,36 +24,26 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from alchemite_apiclient.model.float_none_type import FloatNoneType
-    from alchemite_apiclient.model.vector_value import VectorValue
-    globals()['VectorValue'] = VectorValue
-    globals()['float, none_type'] = float, none_type
 
-
-class Value(ModelNormal):
+class VectorValue(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
@@ -61,66 +51,63 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():  # noqa
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'value': ([bool, date, datetime, dict, float, int, list, str, none_type],),
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
-    attribute_map = {
-        'name': 'name',  # noqa: E501
-        'value': 'value',  # noqa: E501
-    }
+    attribute_map = {}
 
-    read_only_vars = {
-    }
+    read_only_vars = set()
 
-    _composed_schemas = {}
+    _composed_schemas = None
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-    @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, value, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
+    def __init__(self, *args, **kwargs):
+        """VectorValue - a model defined in OpenAPI
+
+        Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            name (str): Property's name
-            value (bool, date, datetime, dict, float, int, list, str, none_type):
+            args[0] ([bool, date, datetime, dict, float, int, list, str, none_type]): Deprecated, it is recommended that series-based data is split out over separate columns for each series point..  # noqa: E501
 
         Keyword Args:
+            value ([bool, date, datetime, dict, float, int, list, str, none_type]): Deprecated, it is recommended that series-based data is split out over separate columns for each series point..  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -144,23 +131,34 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
-        self = super(OpenApiModel, cls).__new__(cls)
-
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
                     self.__class__.__name__,
                 ),
                 path_to_item=_path_to_item,
@@ -169,45 +167,37 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.name = name
         self.value = value
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, name, value, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
+    def _from_openapi_data(cls, *args, **kwargs):
+        """VectorValue - a model defined in OpenAPI
+
+        Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            name (str): Property's name
-            value (bool, date, datetime, dict, float, int, list, str, none_type):
+            args[0] ([bool, date, datetime, dict, float, int, list, str, none_type]): Deprecated, it is recommended that series-based data is split out over separate columns for each series point..  # noqa: E501
 
         Keyword Args:
+            value ([bool, date, datetime, dict, float, int, list, str, none_type]): Deprecated, it is recommended that series-based data is split out over separate columns for each series point..  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -231,18 +221,33 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
@@ -254,21 +259,19 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.name = name
         self.value = value
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
+
+        return self
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/vector_prediction.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model/vector_result.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model/vector_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/model_utils.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/model_utils.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/models/__init__.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,16 +176,14 @@
 from alchemite_apiclient.model.part_tar_fn_sum import PartTarFnSum
 from alchemite_apiclient.model.part_tar_fn_weighted_sum import PartTarFnWeightedSum
 from alchemite_apiclient.model.predict_request import PredictRequest
 from alchemite_apiclient.model.prediction import Prediction
 from alchemite_apiclient.model.query_request import QueryRequest
 from alchemite_apiclient.model.query_response import QueryResponse
 from alchemite_apiclient.model.si_sample_def_categorical import SISampleDefCategorical
-from alchemite_apiclient.model.si_sample_def_categorical_column_values import SISampleDefCategoricalColumnValues
-from alchemite_apiclient.model.si_sample_def_continuous import SISampleDefContinuous
 from alchemite_apiclient.model.si_sample_definition import SISampleDefinition
 from alchemite_apiclient.model.sample_def_categorical import SampleDefCategorical
 from alchemite_apiclient.model.sample_def_categorical_column_values import SampleDefCategoricalColumnValues
 from alchemite_apiclient.model.sample_def_composition import SampleDefComposition
 from alchemite_apiclient.model.sample_def_composition_all_of import SampleDefCompositionAllOf
 from alchemite_apiclient.model.sample_def_continuous import SampleDefContinuous
 from alchemite_apiclient.model.sample_def_continuous_with_start import SampleDefContinuousWithStart
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient/rest.py` & `alchemite_apiclient-0.56.0/alchemite_apiclient/rest.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/PKG-INFO` & `alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite-apiclient
-Version: 0.55.0
+Version: 0.56.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -19,15 +19,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.55.0
+API version: 0.56.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.55.0/alchemite_apiclient.egg-info/SOURCES.txt` & `alchemite_apiclient-0.56.0/alchemite_apiclient.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -206,16 +206,14 @@
 alchemite_apiclient/model/sample_definition.py
 alchemite_apiclient/model/scalar_prediction.py
 alchemite_apiclient/model/scalar_result.py
 alchemite_apiclient/model/sensitivity_request.py
 alchemite_apiclient/model/set_inputs.py
 alchemite_apiclient/model/share_group.py
 alchemite_apiclient/model/si_sample_def_categorical.py
-alchemite_apiclient/model/si_sample_def_categorical_column_values.py
-alchemite_apiclient/model/si_sample_def_continuous.py
 alchemite_apiclient/model/si_sample_definition.py
 alchemite_apiclient/model/string_cat_arr.py
 alchemite_apiclient/model/suggest_additional_parameters.py
 alchemite_apiclient/model/suggest_additional_parameters_all_of.py
 alchemite_apiclient/model/suggest_additional_request.py
 alchemite_apiclient/model/suggest_additional_request_all_of.py
 alchemite_apiclient/model/suggest_additional_result.py
@@ -443,16 +441,14 @@
 docs/PartTarFnSum.md
 docs/PartTarFnWeightedSum.md
 docs/PredictRequest.md
 docs/Prediction.md
 docs/QueryRequest.md
 docs/QueryResponse.md
 docs/SISampleDefCategorical.md
-docs/SISampleDefCategoricalColumnValues.md
-docs/SISampleDefContinuous.md
 docs/SISampleDefinition.md
 docs/SampleDefCategorical.md
 docs/SampleDefCategoricalColumnValues.md
 docs/SampleDefComposition.md
 docs/SampleDefCompositionAllOf.md
 docs/SampleDefContinuous.md
 docs/SampleDefContinuousWithStart.md
```

### Comparing `alchemite_apiclient-0.55.0/docs/AdditiveSensitivityRequest.md` & `alchemite_apiclient-0.56.0/docs/AdditiveSensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/AnalyseValidateRequest.md` & `alchemite_apiclient-0.56.0/docs/AnalyseValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/AnalyseValidateRequestAllOf.md` & `alchemite_apiclient-0.56.0/docs/AnalyseValidateRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/AnalyseValidateResponse.md` & `alchemite_apiclient-0.56.0/docs/AnalyseValidateResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/AnalyseValidateResponseColumnAnalytics.md` & `alchemite_apiclient-0.56.0/docs/AnalyseValidateResponseColumnAnalytics.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalColumn.md` & `alchemite_apiclient-0.56.0/docs/CategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalColumnInfo.md` & `alchemite_apiclient-0.56.0/docs/CategoricalColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalColumnInfoAllOf.md` & `alchemite_apiclient-0.56.0/docs/CategoricalColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalColumnInfoStats.md` & `alchemite_apiclient-0.56.0/docs/CategoricalColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalModelColumnInfo.md` & `alchemite_apiclient-0.56.0/docs/CategoricalModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalModelColumnInfoAllOf.md` & `alchemite_apiclient-0.56.0/docs/CategoricalModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalPrediction.md` & `alchemite_apiclient-0.56.0/docs/CategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/CategoricalResult.md` & `alchemite_apiclient-0.56.0/docs/CategoricalResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnGroupBatchRequest.md` & `alchemite_apiclient-0.56.0/docs/ColumnGroupBatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnGroupPatchRequest.md` & `alchemite_apiclient-0.56.0/docs/ColumnGroupPatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnGroupRequest.md` & `alchemite_apiclient-0.56.0/docs/ColumnGroupRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnGroupResponse.md` & `alchemite_apiclient-0.56.0/docs/ColumnGroupResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnGroupResponseAllOf.md` & `alchemite_apiclient-0.56.0/docs/ColumnGroupResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnInfo.md` & `alchemite_apiclient-0.56.0/docs/ColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnValue.md` & `alchemite_apiclient-0.56.0/docs/ColumnValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ColumnValueNullable.md` & `alchemite_apiclient-0.56.0/docs/ColumnValueNullable.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ContinuousColumnInfo.md` & `alchemite_apiclient-0.56.0/docs/ContinuousColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ContinuousColumnInfoAllOf.md` & `alchemite_apiclient-0.56.0/docs/ContinuousColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ContinuousColumnInfoStats.md` & `alchemite_apiclient-0.56.0/docs/ContinuousColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ContinuousModelColumnInfo.md` & `alchemite_apiclient-0.56.0/docs/ContinuousModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ContinuousModelColumnInfoAllOf.md` & `alchemite_apiclient-0.56.0/docs/ContinuousModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRDatasetReductionData.md` & `alchemite_apiclient-0.56.0/docs/DRDatasetReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRDatasetReductionMetadata.md` & `alchemite_apiclient-0.56.0/docs/DRDatasetReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRDatasetReductionMetadataSources.md` & `alchemite_apiclient-0.56.0/docs/DRDatasetReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRJobReductionMetadata.md` & `alchemite_apiclient-0.56.0/docs/DRJobReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRJobReductionMetadataSources.md` & `alchemite_apiclient-0.56.0/docs/DRJobReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRModelReductionData.md` & `alchemite_apiclient-0.56.0/docs/DRModelReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRPCAReductionType.md` & `alchemite_apiclient-0.56.0/docs/DRPCAReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRThreeDimensionPoint.md` & `alchemite_apiclient-0.56.0/docs/DRThreeDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRTwoDimensionPoint.md` & `alchemite_apiclient-0.56.0/docs/DRTwoDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DRUMAPReductionType.md` & `alchemite_apiclient-0.56.0/docs/DRUMAPReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/Data.md` & `alchemite_apiclient-0.56.0/docs/Data.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/Dataset.md` & `alchemite_apiclient-0.56.0/docs/Dataset.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/Dataset1.md` & `alchemite_apiclient-0.56.0/docs/Dataset1.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetChunk.md` & `alchemite_apiclient-0.56.0/docs/DatasetChunk.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetOrData.md` & `alchemite_apiclient-0.56.0/docs/DatasetOrData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetPatch.md` & `alchemite_apiclient-0.56.0/docs/DatasetPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetQueryRequest.md` & `alchemite_apiclient-0.56.0/docs/DatasetQueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetQueryRequestRowIDs.md` & `alchemite_apiclient-0.56.0/docs/DatasetQueryRequestRowIDs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetQueryRequestSort.md` & `alchemite_apiclient-0.56.0/docs/DatasetQueryRequestSort.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetQueryResponseResult.md` & `alchemite_apiclient-0.56.0/docs/DatasetQueryResponseResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DatasetsApi.md` & `alchemite_apiclient-0.56.0/docs/DatasetsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DefaultApi.md` & `alchemite_apiclient-0.56.0/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgCol.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgColWeights.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgConstantSum.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgProduct.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgRatio.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgSummandsWeights.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgWeightedRatio.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgZeroIfZero.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.56.0/docs/DependentColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DependentColumns.md` & `alchemite_apiclient-0.56.0/docs/DependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DimensionalityReductionRequest.md` & `alchemite_apiclient-0.56.0/docs/DimensionalityReductionRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/DimensionalityReductionResponse.md` & `alchemite_apiclient-0.56.0/docs/DimensionalityReductionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/EmptyCategoricalColumn.md` & `alchemite_apiclient-0.56.0/docs/EmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/EmptyContinuousColumn.md` & `alchemite_apiclient-0.56.0/docs/EmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/Error.md` & `alchemite_apiclient-0.56.0/docs/Error.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizeDone.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizeDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizeDoneAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizeDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizeFailed.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizeFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizeFailedAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizeFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizeOptimizing.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizeOptimizing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizeOptimizingAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizeOptimizingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizePending.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizePending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetOptimizePendingAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetOptimizePendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalDone.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalDoneAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalFailed.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalFailedAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalPending.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalPendingAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalPendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalRunning.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestAdditionalRunningAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestAdditionalRunningAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestHistoricDone.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestHistoricDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestHistoricDoneAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestHistoricDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestHistoricFailed.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestHistoricFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestHistoricPending.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestHistoricPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestHistoricRunning.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestHistoricRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestInitialDone.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestInitialDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestInitialDoneAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestInitialDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestInitialFailed.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestInitialFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestInitialFailedAllOf.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestInitialFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestInitialPending.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestInitialPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/GetSuggestInitialRunning.md` & `alchemite_apiclient-0.56.0/docs/GetSuggestInitialRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/HistoricCategoricalPrediction.md` & `alchemite_apiclient-0.56.0/docs/HistoricCategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/HistoricPrediction.md` & `alchemite_apiclient-0.56.0/docs/HistoricPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/HistoricScalarPrediction.md` & `alchemite_apiclient-0.56.0/docs/HistoricScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/HistoricTargetFunction.md` & `alchemite_apiclient-0.56.0/docs/HistoricTargetFunction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/HistoricValue.md` & `alchemite_apiclient-0.56.0/docs/HistoricValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/HistoricVectorPrediction.md` & `alchemite_apiclient-0.56.0/docs/HistoricVectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/HistoricVectorValue.md` & `alchemite_apiclient-0.56.0/docs/HistoricVectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ImportanceRequest.md` & `alchemite_apiclient-0.56.0/docs/ImportanceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ImputeRequest.md` & `alchemite_apiclient-0.56.0/docs/ImputeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/JobPatch.md` & `alchemite_apiclient-0.56.0/docs/JobPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/MetricsApi.md` & `alchemite_apiclient-0.56.0/docs/MetricsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/Model.md` & `alchemite_apiclient-0.56.0/docs/Model.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ModelColumnInfo.md` & `alchemite_apiclient-0.56.0/docs/ModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ModelDatasetApi.md` & `alchemite_apiclient-0.56.0/docs/ModelDatasetApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ModelPatch.md` & `alchemite_apiclient-0.56.0/docs/ModelPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ModelPermittedColumnRelationships.md` & `alchemite_apiclient-0.56.0/docs/ModelPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ModelsApi.md` & `alchemite_apiclient-0.56.0/docs/ModelsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ModelsIdAdditiveSensitivityOrigin.md` & `alchemite_apiclient-0.56.0/docs/ModelsIdAdditiveSensitivityOrigin.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ModelsIdTrainPermittedColumnRelationships.md` & `alchemite_apiclient-0.56.0/docs/ModelsIdTrainPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgCol.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgColAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgColAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgColWeights.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgColWeightsAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgColWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgColWeightsAllOfArguments.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgColWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgConstantSum.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgConstantSumAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgConstantSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgConstantSumAllOfArguments.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgConstantSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgProduct.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgProductAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgProductAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgProductAllOfArguments.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgProductAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgRatio.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgRatioAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgSummandsWeights.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgSummandsWeightsAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgSummandsWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedConstSumAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedConstSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedRatio.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedRatioAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgWeightedRatioAllOfArguments.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgWeightedRatioAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgZeroIfZero.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.56.0/docs/NewColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NewColumns.md` & `alchemite_apiclient-0.56.0/docs/NewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NonEmptyCategoricalColumn.md` & `alchemite_apiclient-0.56.0/docs/NonEmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NonEmptyContinuousColumn.md` & `alchemite_apiclient-0.56.0/docs/NonEmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/NonEmptyIntegerCategoricalColumn.md` & `alchemite_apiclient-0.56.0/docs/NonEmptyIntegerCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OTSampleDefCategorical.md` & `alchemite_apiclient-0.56.0/docs/OTSampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OTSampleDefContinuous.md` & `alchemite_apiclient-0.56.0/docs/OTSampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OTSampleDefinition.md` & `alchemite_apiclient-0.56.0/docs/OTSampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OptimizeRequest.md` & `alchemite_apiclient-0.56.0/docs/OptimizeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OutliersRequest.md` & `alchemite_apiclient-0.56.0/docs/OutliersRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OutputToleranceRequest.md` & `alchemite_apiclient-0.56.0/docs/OutputToleranceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OutputToleranceResponse.md` & `alchemite_apiclient-0.56.0/docs/OutputToleranceResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OutputToleranceResponseFixedInputs.md` & `alchemite_apiclient-0.56.0/docs/OutputToleranceResponseFixedInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OutputToleranceResponsePredictedOutputs.md` & `alchemite_apiclient-0.56.0/docs/OutputToleranceResponsePredictedOutputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OutputToleranceResponsePredictions.md` & `alchemite_apiclient-0.56.0/docs/OutputToleranceResponsePredictions.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/OutputToleranceResponseSampledInputs.md` & `alchemite_apiclient-0.56.0/docs/OutputToleranceResponseSampledInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartDependentColumns.md` & `alchemite_apiclient-0.56.0/docs/PartDependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartGetOptimize.md` & `alchemite_apiclient-0.56.0/docs/PartGetOptimize.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartGetSuggestAdditional.md` & `alchemite_apiclient-0.56.0/docs/PartGetSuggestAdditional.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartGetSuggestHistoric.md` & `alchemite_apiclient-0.56.0/docs/PartGetSuggestHistoric.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartGetSuggestInitial.md` & `alchemite_apiclient-0.56.0/docs/PartGetSuggestInitial.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartNewColumns.md` & `alchemite_apiclient-0.56.0/docs/PartNewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartTarFnBetween.md` & `alchemite_apiclient-0.56.0/docs/PartTarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartTarFnCategoricals.md` & `alchemite_apiclient-0.56.0/docs/PartTarFnCategoricals.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartTarFnSingleTar.md` & `alchemite_apiclient-0.56.0/docs/PartTarFnSingleTar.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartTarFnSum.md` & `alchemite_apiclient-0.56.0/docs/PartTarFnSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PartTarFnWeightedSum.md` & `alchemite_apiclient-0.56.0/docs/PartTarFnWeightedSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/PredictRequest.md` & `alchemite_apiclient-0.56.0/docs/PredictRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/Prediction.md` & `alchemite_apiclient-0.56.0/docs/Prediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/QueryRequest.md` & `alchemite_apiclient-0.56.0/docs/QueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/QueryResponse.md` & `alchemite_apiclient-0.56.0/docs/QueryResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SISampleDefCategorical.md` & `alchemite_apiclient-0.56.0/docs/SISampleDefCategorical.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SISampleDefCategorical
 
 The key value is a made up variable name by which to identify the constraint. 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**values** | [**{str: (SISampleDefCategoricalColumnValues,)}**](SISampleDefCategoricalColumnValues.md) | Describe the options and accompanying values to choose between. | 
+**values** | [**{str: (SampleDefCategoricalColumnValues,)}**](SampleDefCategoricalColumnValues.md) | Describe the options and accompanying values to choose between. | 
 **type** | **str** |  | defaults to "categorical"
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/SISampleDefCategoricalColumnValues.md` & `alchemite_apiclient-0.56.0/docs/SampleDefCategoricalColumnValues.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SISampleDefCategoricalColumnValues
+# SampleDefCategoricalColumnValues
 
 The key value is a made up name for the option defined.
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
```

### Comparing `alchemite_apiclient-0.55.0/docs/SISampleDefContinuous.md` & `alchemite_apiclient-0.56.0/docs/SampleDefContinuousWithStart.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# SISampleDefContinuous
+# SampleDefContinuousWithStart
 
 The key value must be a valid column name. The constraint will be applied to this column. 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
+**type** | **str** | * &#x60;\&quot;continuous\&quot;&#x60;: Search a continuous domain within the &#x60;\&quot;range\&quot;&#x60; specified with uniform prior. * &#x60;\&quot;continuous or zero\&quot;&#x60;: Either search a continuous domain within the &#x60;\&quot;range\&quot;&#x60; specified, or return 0.  | 
 **range** | **[float]** | Range is an array consisting of a lower and upper bound where the lower bound is strictly smaller than the upper bound.  | 
-**type** | **str** | Search a continuous domain within the &#x60;\&quot;range\&quot;&#x60; specified with uniform prior.  | defaults to "continuous"
+**start** | **float** | &#x60;\&quot;start\&quot;&#x60; is used for local optimization only. * &#x60;\&quot;start\&quot;&#x60; specifies the start point of the local optimisation. * If it is not specified the mean value of the &#x60;\&quot;range\&quot;&#x60; will be taken as the starting point.  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/SISampleDefinition.md` & `alchemite_apiclient-0.56.0/docs/SISampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefCategorical.md` & `alchemite_apiclient-0.56.0/docs/SampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefCategoricalColumnValues.md` & `alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBelowAllOf.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# SampleDefCategoricalColumnValues
+# TarFnWeightedSumBelowAllOf
 
-The key value is a made up name for the option defined.
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
+**type** | **str** | Find a solution where the weighted sum of the given columns is below &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "weighted sum below"
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefComposition.md` & `alchemite_apiclient-0.56.0/docs/SampleDefComposition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefCompositionAllOf.md` & `alchemite_apiclient-0.56.0/docs/SampleDefCompositionAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefContinuous.md` & `alchemite_apiclient-0.56.0/docs/SampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefContinuousWithStart.md` & `alchemite_apiclient-0.56.0/docs/TarFnSumBetween.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# SampleDefContinuousWithStart
+# TarFnSumBetween
 
-The key value must be a valid column name. The constraint will be applied to this column. 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | **str** | * &#x60;\&quot;continuous\&quot;&#x60;: Search a continuous domain within the &#x60;\&quot;range\&quot;&#x60; specified with uniform prior. * &#x60;\&quot;continuous or zero\&quot;&#x60;: Either search a continuous domain within the &#x60;\&quot;range\&quot;&#x60; specified, or return 0.  | 
-**range** | **[float]** | Range is an array consisting of a lower and upper bound where the lower bound is strictly smaller than the upper bound.  | 
-**start** | **float** | &#x60;\&quot;start\&quot;&#x60; is used for local optimization only. * &#x60;\&quot;start\&quot;&#x60; specifies the start point of the local optimisation. * If it is not specified the mean value of the &#x60;\&quot;range\&quot;&#x60; will be taken as the starting point.  | [optional] 
+**maximum** | **float** |  | 
+**minimum** | **float** |  | 
+**targets** | **[str]** | Array of columns names to sum | 
+**type** | **str** | Find a solution where the sum of the given columns is between &#x60;\&quot;minimum\&quot;&#x60; and &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "sum between"
+**importance** | **float** | The higher the value the higher the importance of this target.  If the importance values all equal 1 then the &#x60;probabilityOfSuccess&#x60; is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers &gt; 1 can make the &#x60;probabilityOfSuccess&#x60; very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the &#x60;probabilityOfSuccess&#x60; scale with the number of columns so that it becomes a more natural-looking \&quot;score\&quot; of how likely the targets are to be met. For example, the reported &#x60;probabilityOfSuccess&#x60; of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5.  | [optional]  if omitted the server will use the default value of 1
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefDiscrete.md` & `alchemite_apiclient-0.56.0/docs/SampleDefDiscrete.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefInteger.md` & `alchemite_apiclient-0.56.0/docs/SampleDefInteger.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefStartProp.md` & `alchemite_apiclient-0.56.0/docs/SampleDefStartProp.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefWeightedCategorical.md` & `alchemite_apiclient-0.56.0/docs/SampleDefWeightedCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SampleDefinition.md` & `alchemite_apiclient-0.56.0/docs/SampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ScalarPrediction.md` & `alchemite_apiclient-0.56.0/docs/ScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ScalarResult.md` & `alchemite_apiclient-0.56.0/docs/ScalarResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SensitivityRequest.md` & `alchemite_apiclient-0.56.0/docs/SensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ShareGroup.md` & `alchemite_apiclient-0.56.0/docs/ShareGroup.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestAdditionalParameters.md` & `alchemite_apiclient-0.56.0/docs/SuggestAdditionalParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestAdditionalParametersAllOf.md` & `alchemite_apiclient-0.56.0/docs/SuggestAdditionalParametersAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestAdditionalRequest.md` & `alchemite_apiclient-0.56.0/docs/SuggestAdditionalRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestAdditionalRequestAllOf.md` & `alchemite_apiclient-0.56.0/docs/SuggestAdditionalRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestHistoricParameters.md` & `alchemite_apiclient-0.56.0/docs/SuggestHistoricParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestHistoricRequest.md` & `alchemite_apiclient-0.56.0/docs/SuggestHistoricRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestHistoricResult.md` & `alchemite_apiclient-0.56.0/docs/SuggestHistoricResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestHistoricResultSamples.md` & `alchemite_apiclient-0.56.0/docs/SuggestHistoricResultSamples.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestInitialParameters.md` & `alchemite_apiclient-0.56.0/docs/SuggestInitialParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestInitialRequest.md` & `alchemite_apiclient-0.56.0/docs/SuggestInitialRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestInitialRequestAllOf.md` & `alchemite_apiclient-0.56.0/docs/SuggestInitialRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestInitialResponse.md` & `alchemite_apiclient-0.56.0/docs/SuggestInitialResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingCommon.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingCommon.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingData.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingDataAllOf.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingDatasetID.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingDatasetID.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingDatasetIDAllOf.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingDatasetIDAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingImputedData.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingImputedData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingImputedDataAllOf.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingImputedDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingRequest.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingResponse.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/SuggestMissingSpecific.md` & `alchemite_apiclient-0.56.0/docs/SuggestMissingSpecific.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnAbove.md` & `alchemite_apiclient-0.56.0/docs/TarFnAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnAboveAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnBelow.md` & `alchemite_apiclient-0.56.0/docs/TarFnBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnBelowAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnBetween.md` & `alchemite_apiclient-0.56.0/docs/TarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnBetweenAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnExcludeCategories.md` & `alchemite_apiclient-0.56.0/docs/TarFnExcludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnExcludeCategoriesAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnExcludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnIncludeCategories.md` & `alchemite_apiclient-0.56.0/docs/TarFnIncludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnIncludeCategoriesAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnIncludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnSumAbove.md` & `alchemite_apiclient-0.56.0/docs/TarFnSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnSumAboveAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnSumBelow.md` & `alchemite_apiclient-0.56.0/docs/TarFnSumBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnSumBelowAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnSumBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnSumBetween.md` & `alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBelow.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# TarFnSumBetween
+# TarFnWeightedSumBelow
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **maximum** | **float** |  | 
-**minimum** | **float** |  | 
-**targets** | **[str]** | Array of columns names to sum | 
-**type** | **str** | Find a solution where the sum of the given columns is between &#x60;\&quot;minimum\&quot;&#x60; and &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "sum between"
+**targets** | **{str: (float,)}** |  | 
+**type** | **str** | Find a solution where the weighted sum of the given columns is below &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "weighted sum below"
 **importance** | **float** | The higher the value the higher the importance of this target.  If the importance values all equal 1 then the &#x60;probabilityOfSuccess&#x60; is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers &gt; 1 can make the &#x60;probabilityOfSuccess&#x60; very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the &#x60;probabilityOfSuccess&#x60; scale with the number of columns so that it becomes a more natural-looking \&quot;score\&quot; of how likely the targets are to be met. For example, the reported &#x60;probabilityOfSuccess&#x60; of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5.  | [optional]  if omitted the server will use the default value of 1
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnSumBetweenAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnSumBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnWeightedSumAbove.md` & `alchemite_apiclient-0.56.0/docs/TarFnWeightedSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnWeightedSumAboveAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnWeightedSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnWeightedSumBelow.md` & `alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBetween.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# TarFnWeightedSumBelow
+# TarFnWeightedSumBetween
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **maximum** | **float** |  | 
+**minimum** | **float** |  | 
 **targets** | **{str: (float,)}** |  | 
-**type** | **str** | Find a solution where the weighted sum of the given columns is below &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "weighted sum below"
+**type** | **str** | Find a solution where the weighted sum of the given columns is between &#x60;\&quot;minimum\&quot;&#x60; and &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "weighted sum between"
 **importance** | **float** | The higher the value the higher the importance of this target.  If the importance values all equal 1 then the &#x60;probabilityOfSuccess&#x60; is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers &gt; 1 can make the &#x60;probabilityOfSuccess&#x60; very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the &#x60;probabilityOfSuccess&#x60; scale with the number of columns so that it becomes a more natural-looking \&quot;score\&quot; of how likely the targets are to be met. For example, the reported &#x60;probabilityOfSuccess&#x60; of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5.  | [optional]  if omitted the server will use the default value of 1
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnWeightedSumBelowAllOf.md` & `alchemite_apiclient-0.56.0/docs/TarFnWeightedSumBetweenAllOf.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TarFnWeightedSumBelowAllOf
+# TarFnWeightedSumBetweenAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | **str** | Find a solution where the weighted sum of the given columns is below &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "weighted sum below"
+**type** | **str** | Find a solution where the weighted sum of the given columns is between &#x60;\&quot;minimum\&quot;&#x60; and &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "weighted sum between"
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/TarFnWeightedSumBetween.md` & `alchemite_apiclient-0.56.0/docs/TargetFunction.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-# TarFnWeightedSumBetween
+# TargetFunction
 
+Dictionary of (potentially multiple) targets to optimize against. The cost function for optimization can be considered to be 1 minus the probability of the given sample to achieve the targets.  The probability function, for each target, accounts for the prediction and the uncertainty in that prediction. Using multiple targets, the overall cost function is 1 minus the probability that all targets are achieved; this is the product of the individual target probabilities. The key value should be a made up name to give the defined target. When importance is specified, the importance factors are included as linear weights on the probabilities in log-probability space. The target column cannot be empty in the training dataset used to create the model. 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**maximum** | **float** |  | 
-**minimum** | **float** |  | 
-**targets** | **{str: (float,)}** |  | 
-**type** | **str** | Find a solution where the weighted sum of the given columns is between &#x60;\&quot;minimum\&quot;&#x60; and &#x60;\&quot;maximum\&quot;&#x60;. | defaults to "weighted sum between"
-**importance** | **float** | The higher the value the higher the importance of this target.  If the importance values all equal 1 then the &#x60;probabilityOfSuccess&#x60; is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers &gt; 1 can make the &#x60;probabilityOfSuccess&#x60; very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the &#x60;probabilityOfSuccess&#x60; scale with the number of columns so that it becomes a more natural-looking \&quot;score\&quot; of how likely the targets are to be met. For example, the reported &#x60;probabilityOfSuccess&#x60; of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5.  | [optional]  if omitted the server will use the default value of 1
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.55.0/docs/TrainRequest.md` & `alchemite_apiclient-0.56.0/docs/TrainRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ValidateRequest.md` & `alchemite_apiclient-0.56.0/docs/ValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/ValidationSplit.md` & `alchemite_apiclient-0.56.0/docs/ValidationSplit.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/Value.md` & `alchemite_apiclient-0.56.0/docs/Value.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/VectorPrediction.md` & `alchemite_apiclient-0.56.0/docs/VectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/VectorResult.md` & `alchemite_apiclient-0.56.0/docs/VectorResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/VectorValue.md` & `alchemite_apiclient-0.56.0/docs/VectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/docs/VersionResponse.md` & `alchemite_apiclient-0.56.0/docs/VersionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/adrenergic.csv` & `alchemite_apiclient-0.56.0/example/adrenergic.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/adrenergic_holdout.csv` & `alchemite_apiclient-0.56.0/example/adrenergic_holdout.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/adrenergic_row.csv` & `alchemite_apiclient-0.56.0/example/adrenergic_row.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/categorical.csv` & `alchemite_apiclient-0.56.0/example/categorical.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_additive_sensitivity.py` & `alchemite_apiclient-0.56.0/example/example_additive_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_basic.py` & `alchemite_apiclient-0.56.0/example/example_basic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_categorical.py` & `alchemite_apiclient-0.56.0/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_chunk.py` & `alchemite_apiclient-0.56.0/example/example_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_column_groups.py` & `alchemite_apiclient-0.56.0/example/example_column_groups.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_custom_validation_splits.py` & `alchemite_apiclient-0.56.0/example/example_custom_validation_splits.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_delete.py` & `alchemite_apiclient-0.56.0/example/example_delete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_dimensionality_reduction.py` & `alchemite_apiclient-0.56.0/example/example_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_download.py` & `alchemite_apiclient-0.56.0/example/example_download.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_export_import.py` & `alchemite_apiclient-0.56.0/example/example_export_import.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_hyperopt.py` & `alchemite_apiclient-0.56.0/example/example_hyperopt.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_importance.py` & `alchemite_apiclient-0.56.0/example/example_importance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_optimize.py` & `alchemite_apiclient-0.56.0/example/example_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_outliers.py` & `alchemite_apiclient-0.56.0/example/example_outliers.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_output_tolerance.py` & `alchemite_apiclient-0.56.0/example/example_output_tolerance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_preload.py` & `alchemite_apiclient-0.56.0/example/example_preload.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_query.py` & `alchemite_apiclient-0.56.0/example/example_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_sensitivity.py` & `alchemite_apiclient-0.56.0/example/example_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_suggest_additional.py` & `alchemite_apiclient-0.56.0/example/example_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_suggest_historic.py` & `alchemite_apiclient-0.56.0/example/example_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_suggest_initial.py` & `alchemite_apiclient-0.56.0/example/example_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_suggest_missing.py` & `alchemite_apiclient-0.56.0/example/example_suggest_missing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_training_outliers.py` & `alchemite_apiclient-0.56.0/example/example_training_outliers.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_validate.py` & `alchemite_apiclient-0.56.0/example/example_validate.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/example_vector.py` & `alchemite_apiclient-0.56.0/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/optimize_args_steel.json` & `alchemite_apiclient-0.56.0/example/optimize_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/optimize_dependentColumns_args_steel.json` & `alchemite_apiclient-0.56.0/example/optimize_dependentColumns_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/steels.csv` & `alchemite_apiclient-0.56.0/example/steels.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/example/suggest_additional_args_steel.json` & `alchemite_apiclient-0.56.0/example/suggest_additional_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/pyproject.toml` & `alchemite_apiclient-0.56.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alchemite_apiclient"
-version = "0.55.0"
+version = "0.56.0"
 authors = [
   { name="Intellegens", email="support@intellegens.com" },
 ]
 description = "A python API client for using Alchemite Analytics"
 keywords = ["Alchemite", "Alchemite API", "Machine Learning", "Artificial Intelligence"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `alchemite_apiclient-0.55.0/setup.py` & `alchemite_apiclient-0.56.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "alchemite-apiclient"
-VERSION = "0.55.0"
+VERSION = "0.56.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `alchemite_apiclient-0.55.0/test/test_cornercases.py` & `alchemite_apiclient-0.56.0/test/test_cornercases.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.55.0/test/test_examples.py` & `alchemite_apiclient-0.56.0/test/test_examples.py`

 * *Files identical despite different names*

