# Comparing `tmp/data-repo-client-1.495.0.tar.gz` & `tmp/data-repo-client-1.64.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-t0c5evqn/data-repo-client-1.495.0.tar", last modified: Mon Jun 26 23:00:52 2023, max compression
+gzip compressed data, was "dist/data-repo-client-1.64.0.tar", last modified: Fri Apr 23 18:20:39 2021, max compression
```

## Comparing `data-repo-client-1.495.0.tar` & `data-repo-client-1.64.0.tar`

### file list

```diff
@@ -1,827 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45154 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59431 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20331 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_admin_register_drs_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_configs_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_configs_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_assets_assetid.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-26 23:00:37.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 23:00:12.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_data_table_statistics_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_deletes.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_files_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_files_bulk_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_files_bulk_load_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_files_fileid.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_filesystem_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_policies_policy_name_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_policies_policy_name_members_member_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_transactions_transaction_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_id_update_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_datasets_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_duos.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_duos_duos_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_duos_duos_id_sync_authorized_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_duos_sync_authorized_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_jobs_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_jobs_id_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 23:00:15.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_journal_resource_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_register_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_search_id_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_search_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_files_fileid.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_filesystem_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_link_duos_dataset_duos_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_policies_policy_name_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_policies_policy_name_members_member_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_id_unlink_duos_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_role_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_snapshots_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_repository_v1_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_resources_v1_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_resources_v1_profiles_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_resources_v1_profiles_id_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_resources_v1_profiles_id_policies_policy_name_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/api_resources_v1_profiles_id_policies_policy_name_members_member_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/ga4gh_drs_v1_objects_object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/ga4gh_drs_v1_objects_object_id_access_access_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/ga4gh_drs_v1_service_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/paths/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/admin_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-26 23:00:05.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/configs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-26 23:00:12.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-26 23:00:14.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/duos_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-26 23:00:15.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-26 23:00:15.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/journal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-26 23:00:17.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 23:00:17.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/register_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/repository_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-26 23:00:37.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/apis/tags/upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/model/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-26 22:59:47.000000 data-repo-client-1.495.0/data_repo_client/model/access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/data_repo_client/model/access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/data_repo_client/model/access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/data_repo_client/model/access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/data_repo_client/model/access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/data_repo_client/model/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/data_repo_client/model/asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/data_repo_client/model/billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/column_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/column_name_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/compact_id_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/data_repo_client/model/config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/consent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/data_repo_client/model/data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16386 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_snapshot_name_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/data_repo_client/model/drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/drs_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/drs_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/data_repo_client/model/drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/data_repo_client/model/duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/duos_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/data_repo_client/model/file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/data_repo_client/model/job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/load_tag_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/md5_override_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/object_name_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/phs_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/data_repo_client/model/resource_create_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/search_index_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/search_index_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/search_metadata_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/search_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/search_query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/search_query_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/short_id_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    28168 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/data_repo_client/model/snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/sql_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/tag_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/unique_id_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/data_repo_client/model/upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/data_repo_client/model/upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/data_repo_client/model/user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/data_repo_client/model/workspace_policy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_admin_register_drs_aliases/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_admin_register_drs_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-06-26 23:00:26.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_admin_register_drs_aliases/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-26 23:00:23.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-06-26 23:00:29.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs_name/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-06-26 23:00:22.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs_name/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-06-26 23:00:29.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs_name/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs_reset/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs_reset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-26 23:00:27.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_configs_reset/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-06-26 23:00:21.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-26 23:00:20.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-06-26 23:00:20.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    14258 2023-06-26 23:00:27.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    16211 2023-06-26 23:00:26.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_assets/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-06-26 23:00:18.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_assets/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_assets_assetid/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_assets_assetid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-06-26 23:00:27.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_assets_assetid/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_data_table/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-26 23:00:37.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_data_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_data_table/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_data_table_statistics_column/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-26 23:00:12.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_data_table_statistics_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-06-26 23:00:09.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_data_table_statistics_column/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_deletes/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_deletes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-26 23:00:18.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_deletes/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17019 2023-06-26 23:00:24.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-06-26 23:00:19.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk_array/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk_array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-06-26 23:00:19.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk_array/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk_load_tag/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk_load_tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-06-26 23:00:19.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk_load_tag/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-06-26 23:00:23.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_bulk_load_tag/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_fileid/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_fileid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-26 23:00:21.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_fileid/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-06-26 23:00:24.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_files_fileid/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_filesystem_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_filesystem_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-06-26 23:00:25.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_filesystem_objects/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_ingest/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17063 2023-06-26 23:00:23.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_ingest/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-26 23:00:27.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies_policy_name_members/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies_policy_name_members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-06-26 23:00:18.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies_policy_name_members/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies_policy_name_members_member_email/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies_policy_name_members_member_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-06-26 23:00:21.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_policies_policy_name_members_member_email/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_roles/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-26 23:00:29.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_roles/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-26 23:00:27.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_summary/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_tags/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15751 2023-06-26 23:00:30.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_tags/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-06-26 23:00:22.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    16801 2023-06-26 23:00:25.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions_transaction_id/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions_transaction_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-06-26 23:00:29.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions_transaction_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-06-26 23:00:19.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_transactions_transaction_id/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_update_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_update_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16801 2023-06-26 23:00:30.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_id_update_schema/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_tags/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-06-26 23:00:23.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_datasets_tags/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-26 23:00:28.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_duos_id/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_duos_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-06-26 23:00:27.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_duos_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_duos_id_sync_authorized_users/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_duos_id_sync_authorized_users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-26 23:00:30.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_duos_id_sync_authorized_users/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_sync_authorized_users/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_sync_authorized_users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-06-26 23:00:30.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_duos_sync_authorized_users/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-06-26 23:00:22.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs_id/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-06-26 23:00:28.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs_id_result/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs_id_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-06-26 23:00:28.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_jobs_id_result/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_journal_resource_key/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 23:00:15.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_journal_resource_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-06-26 23:00:15.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_journal_resource_key/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_register_user/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_register_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_register_user/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_search_id_index/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_search_id_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-06-26 23:00:37.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_search_id_index/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_search_query/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_search_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-26 23:00:40.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_search_query/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-06-26 23:00:38.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14926 2023-06-26 23:00:38.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13204 2023-06-26 23:00:38.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-06-26 23:00:40.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-06-26 23:00:40.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_data_table/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_data_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-26 23:00:40.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_data_table/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_export/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-26 23:00:39.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_export/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_files_fileid/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_files_fileid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-26 23:00:39.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_files_fileid/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_filesystem_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_filesystem_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-06-26 23:00:39.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_filesystem_objects/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_link_duos_dataset_duos_id/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_link_duos_dataset_duos_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-06-26 23:00:39.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_link_duos_dataset_duos_id/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies_policy_name_members/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies_policy_name_members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-06-26 23:00:37.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies_policy_name_members/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies_policy_name_members_member_email/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies_policy_name_members_member_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-06-26 23:00:38.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_policies_policy_name_members_member_email/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_roles/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_roles/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_summary/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_tags/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_tags/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_unlink_duos_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_unlink_duos_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_id_unlink_duos_dataset/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_role_map/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_role_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-06-26 23:00:39.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_role_map/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_tags/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-26 23:00:39.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_snapshots_tags/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/api_repository_v1_upgrade/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-26 23:00:35.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-06-26 23:00:34.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles/post.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-06-26 23:00:35.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-06-26 23:00:34.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-06-26 23:00:35.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-26 23:00:35.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies_policy_name_members/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies_policy_name_members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-06-26 23:00:34.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies_policy_name_members/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies_policy_name_members_member_email/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies_policy_name_members_member_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-06-26 23:00:35.000000 data-repo-client-1.495.0/data_repo_client/paths/api_resources_v1_profiles_id_policies_policy_name_members_member_email/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/data_repo_client/paths/configuration/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-06-26 23:00:03.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-06-26 23:00:03.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-06-26 23:00:03.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id_access_access_id/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id_access_access_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id_access_access_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    19872 2023-06-26 23:00:03.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_objects_object_id_access_access_id/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_service_info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_service_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-26 23:00:03.000000 data-repo-client-1.495.0/data_repo_client/paths/ga4gh_drs_v1_service_info/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/shutdown/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/shutdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/shutdown/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client/paths/status/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/paths/status/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    98575 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/data_repo_client/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40763 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/data_repo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-26 22:59:47.000000 data-repo-client-1.495.0/test/test_models/test_access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/test/test_models/test_access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/test/test_models/test_access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/test/test_models/test_access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/test/test_models/test_access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/test/test_models/test_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 22:59:48.000000 data-repo-client-1.495.0/test/test_models/test_asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-26 22:59:49.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_column_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_column_name_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_compact_id_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-26 22:59:50.000000 data-repo-client-1.495.0/test/test_models/test_config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_consent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/test/test_models/test_data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/test/test_models/test_dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/test/test_models/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/test/test_models/test_dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/test/test_models/test_dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:53.000000 data-repo-client-1.495.0/test/test_models/test_dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_dataset_snapshot_name_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-26 22:59:51.000000 data-repo-client-1.495.0/test/test_models/test_drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_drs_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_drs_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-26 22:59:52.000000 data-repo-client-1.495.0/test/test_models/test_drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-26 22:59:54.000000 data-repo-client-1.495.0/test/test_models/test_duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_duos_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-26 22:59:55.000000 data-repo-client-1.495.0/test/test_models/test_file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-26 22:59:56.000000 data-repo-client-1.495.0/test/test_models/test_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_load_tag_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_md5_override_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_object_name_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_phs_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 22:59:57.000000 data-repo-client-1.495.0/test/test_models/test_repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_resource_create_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_search_index_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_search_index_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_search_metadata_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_search_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_search_query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_search_query_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 22:59:58.000000 data-repo-client-1.495.0/test/test_models/test_short_id_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 22:59:59.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 23:00:00.000000 data-repo-client-1.495.0/test/test_models/test_snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_sql_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_tag_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 23:00:01.000000 data-repo-client-1.495.0/test/test_models/test_unique_id_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/test/test_models/test_upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/test/test_models/test_upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/test/test_models/test_user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-26 23:00:02.000000 data-repo-client-1.495.0/test/test_models/test_workspace_policy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_admin_register_drs_aliases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_admin_register_drs_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_admin_register_drs_aliases/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs_name/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs_name/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs_name/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs_reset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs_reset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_configs_reset/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_assets/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_assets_assetid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_assets_assetid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_assets_assetid/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_data_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:37.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_data_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-26 23:00:37.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_data_table/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_data_table_statistics_column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:12.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_data_table_statistics_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-26 23:00:12.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_data_table_statistics_column/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_deletes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_deletes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_deletes/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk_array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk_array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk_array/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk_load_tag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk_load_tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk_load_tag/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_bulk_load_tag/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_fileid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_fileid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_fileid/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_files_fileid/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_filesystem_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_filesystem_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_filesystem_objects/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_ingest/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies_policy_name_members/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies_policy_name_members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies_policy_name_members/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies_policy_name_members_member_email/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies_policy_name_members_member_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_policies_policy_name_members_member_email/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_roles/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_summary/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_tags/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions_transaction_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions_transaction_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions_transaction_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_transactions_transaction_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_update_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_update_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_id_update_schema/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_datasets_tags/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_duos_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_duos_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_duos_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_duos_id_sync_authorized_users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_duos_id_sync_authorized_users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_duos_id_sync_authorized_users/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_sync_authorized_users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_sync_authorized_users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_duos_sync_authorized_users/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs_id_result/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs_id_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_jobs_id_result/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_journal_resource_key/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:15.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_journal_resource_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 23:00:15.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_journal_resource_key/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_register_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_register_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-26 23:00:31.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_register_user/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_search_id_index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_search_id_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_search_id_index/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_search_query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_search_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_search_query/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_data_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_data_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_data_table/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_export/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_files_fileid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_files_fileid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_files_fileid/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_filesystem_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_filesystem_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_filesystem_objects/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_link_duos_dataset_duos_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_link_duos_dataset_duos_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_link_duos_dataset_duos_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies_policy_name_members/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies_policy_name_members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies_policy_name_members/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies_policy_name_members_member_email/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies_policy_name_members_member_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_policies_policy_name_members_member_email/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_roles/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_summary/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_tags/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_unlink_duos_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_unlink_duos_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-26 23:00:42.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_id_unlink_duos_dataset/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_role_map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_role_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_role_map/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 23:00:41.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_snapshots_tags/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_api_repository_v1_upgrade/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles/test_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies_policy_name_members/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies_policy_name_members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies_policy_name_members/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies_policy_name_members_member_email/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies_policy_name_members_member_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 23:00:36.000000 data-repo-client-1.495.0/test/test_paths/test_api_resources_v1_profiles_id_policies_policy_name_members_member_email/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_configuration/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id_access_access_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id_access_access_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id_access_access_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_objects_object_id_access_access_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_service_info/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_service_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-26 23:00:04.000000 data-repo-client-1.495.0/test/test_paths/test_ga4gh_drs_v1_service_info/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_shutdown/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_shutdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_shutdown/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:52.000000 data-repo-client-1.495.0/test/test_paths/test_status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 23:00:43.000000 data-repo-client-1.495.0/test/test_paths/test_status/test_get.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/
+-rw-r--r--   0 myessail   (503) staff       (20)     1545 2020-12-08 18:44:05.000000 data-repo-client-1.64.0/LICENSE
+-rw-r--r--   0 myessail   (503) staff       (20)     3077 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/PKG-INFO
+-rw-r--r--   0 myessail   (503) staff       (20)    17369 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/README.md
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client/
+-rw-r--r--   0 myessail   (503) staff       (20)     9367 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/__init__.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client/api/
+-rw-r--r--   0 myessail   (503) staff       (20)      367 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/__init__.py
+-rw-r--r--   0 myessail   (503) staff       (20)    21178 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/data_repository_service_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)   220470 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/repository_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)    48309 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/resources_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)    16523 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/unauthenticated_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)    28864 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api_client.py
+-rw-r--r--   0 myessail   (503) staff       (20)    16252 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/configuration.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6399 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/exceptions.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client/models/
+-rw-r--r--   0 myessail   (503) staff       (20)     8637 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/models/__init__.py
+-rw-r--r--   0 myessail   (503) staff       (20)    12442 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8331 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/asset_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11823 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10883 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/billing_profile_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8881 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/billing_profile_update_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10190 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_array_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7136 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_array_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9274 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9809 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5536 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_state.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11633 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_history_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10716 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10106 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9123 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/column_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6117 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_enable_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9345 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_fault_counted_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8984 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_fault_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6741 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_group_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6659 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_list_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8405 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6504 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_parameter_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7502 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/data_deletion_gcs_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8512 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/data_deletion_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7203 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/data_deletion_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    13682 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10478 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7788 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_specification_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11240 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7647 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/date_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6458 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/delete_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7546 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/directory_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9199 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_access_method.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7204 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_access_url.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7335 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_checksum.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10111 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_contents_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6787 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_error.py
+-rw-r--r--   0 myessail   (503) staff       (20)    19591 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9189 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_service_info.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6857 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6757 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6774 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5524 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_sort_by_param.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6819 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/error_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8609 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11401 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_load_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    13545 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5442 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_model_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)    17287 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/ingest_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    14206 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/ingest_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10890 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/int_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11107 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/job_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6103 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/policy_member_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6515 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/policy_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6010 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/policy_response.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7892 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/relationship_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9869 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/relationship_term_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9717 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/repository_configuration_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7087 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/repository_status_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7388 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/repository_status_model_systems.py
+-rw-r--r--   0 myessail   (503) staff       (20)    13949 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8713 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11122 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_contents_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10905 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8570 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_query_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6271 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_row_id_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9573 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_row_id_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8439 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_source_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11085 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5436 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/sql_sort_direction.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5862 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/table_data_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)    12798 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9540 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/upgrade_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7831 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/upgrade_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8182 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/user_status_info.py
+-rw-r--r--   0 myessail   (503) staff       (20)    14933 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/rest.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/
+-rw-r--r--   0 myessail   (503) staff       (20)     3077 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/PKG-INFO
+-rw-r--r--   0 myessail   (503) staff       (20)     6884 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 myessail   (503) staff       (20)        1 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 myessail   (503) staff       (20)       48 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/requires.txt
+-rw-r--r--   0 myessail   (503) staff       (20)       17 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/top_level.txt
+-rw-r--r--   0 myessail   (503) staff       (20)       69 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/setup.cfg
+-rw-r--r--   0 myessail   (503) staff       (20)     6404 2021-04-23 18:19:32.000000 data-repo-client-1.64.0/setup.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/test/
+-rw-r--r--   0 myessail   (503) staff       (20)     4761 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4219 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_asset_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4301 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4442 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_billing_profile_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4332 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/test/test_billing_profile_update_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4931 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_array_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4825 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_array_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4247 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4345 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_file_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4037 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_file_state.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4384 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_history_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4330 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4270 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4121 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_column_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4066 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_enable_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4230 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_fault_counted_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4345 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_fault_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4911 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_group_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4899 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_list_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4607 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4096 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_parameter_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4242 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_data_deletion_gcs_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4611 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_data_deletion_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4346 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_data_deletion_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3900 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_data_repository_service_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6863 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9500 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_dataset_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7567 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_dataset_specification_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4227 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_dataset_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4184 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_date_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4098 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_delete_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5201 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_directory_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4331 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_access_method.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4100 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_access_url.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4059 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_checksum.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4492 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_contents_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3995 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_error.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5989 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4195 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_service_info.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4625 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_enumerate_billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4456 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_enumerate_dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4461 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_enumerate_snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4070 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/test/test_enumerate_sort_by_param.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4098 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_error_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4148 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4269 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_load_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5957 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3991 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_model_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4558 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_ingest_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4373 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_ingest_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4342 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_int_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4239 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_job_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4114 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_policy_member_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4070 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_policy_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4259 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_policy_response.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4748 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_relationship_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4197 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_relationship_term_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7673 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4337 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_configuration_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4703 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_status_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4250 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_status_model_systems.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3899 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_resources_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6369 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4351 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5287 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_contents_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7047 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4251 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_query_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4938 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_row_id_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4553 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_row_id_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4689 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_source_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4230 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4024 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/test/test_sql_sort_direction.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3991 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/test/test_table_data_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5064 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3725 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_unauthenticated_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4248 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_upgrade_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4171 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_upgrade_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4213 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_user_status_info.py
```

### Comparing `data-repo-client-1.495.0/data_repo_client/apis/tags/duos_api.py` & `data-repo-client-1.64.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-# coding: utf-8
-
-"""
-    Data Repository API
-
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from data_repo_client.paths.api_repository_v1_duos_duos_id.get import RetrieveDuosFirecloudGroup
-from data_repo_client.paths.api_repository_v1_duos.get import RetrieveDuosFirecloudGroups
-from data_repo_client.paths.api_repository_v1_duos_duos_id_sync_authorized_users.put import SyncDuosDatasetAuthorizedUsers
-from data_repo_client.paths.api_repository_v1_duos_sync_authorized_users.put import SyncDuosDatasetsAuthorizedUsers
-
-
-class DuosApi(
-    RetrieveDuosFirecloudGroup,
-    RetrieveDuosFirecloudGroups,
-    SyncDuosDatasetAuthorizedUsers,
-    SyncDuosDatasetsAuthorizedUsers,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-    pass
+Metadata-Version: 1.0
+Name: data-repo-client
+Version: 1.64.0
+Summary: Data Repository API
+Home-page: UNKNOWN
+Author: OpenAPI Generator community
+Author-email: team@openapitools.org
+License: Apache 2.0
+Description:     This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \&quot;Model\&quot;. Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: &#x60;&#x60;&#x60; docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor &#x60;&#x60;&#x60; Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with &#39;DRS&#39; to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
+            
+Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
+Platform: UNKNOWN
```

### Comparing `data-repo-client-1.495.0/data_repo_client/configuration.py` & `data-repo-client-1.64.0/data_repo_client/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
+
+from __future__ import absolute_import
+
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
-from data_repo_client.exceptions import ApiValueError
-
+import six
+from six.moves import http_client as httplib
 
-JSON_SCHEMA_VALIDATION_KEYWORDS = {
-    'multipleOf', 'maximum', 'exclusiveMaximum',
-    'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems',
-    'uniqueItems', 'maxProperties', 'minProperties',
-}
 
 class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
@@ -49,71 +45,73 @@
          implementation.
       2. The client was generated using an older version of the OpenAPI document
          and the server has been upgraded since then.
       If a schema in the OpenAPI document defines the additionalProperties attribute,
       then all undeclared properties received by the server are injected into the
       additional properties map. In that case, there are undeclared properties, and
       nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
-    :param server_index: Index to servers configuration.
-    :param server_variables: Mapping with string values to replace variables in
-      templated server configuration. The validation of enums is performed for
-      variables with defined enum values before.
-    :param server_operation_index: Mapping from operation ID to an index to server
-      configuration.
-    :param server_operation_variables: Mapping from operation ID to a mapping with
-      string values to replace variables in templated server configuration.
-      The validation of enums is performed for variables with defined enum values before.
 
     :Example:
+
+    API Key Authentication Example.
+    Given the following security scheme in the OpenAPI specification:
+      components:
+        securitySchemes:
+          cookieAuth:         # name for the security scheme
+            type: apiKey
+            in: cookie
+            name: JSESSIONID  # cookie name
+
+    You can programmatically set the cookie:
+
+conf = data_repo_client.Configuration(
+    api_key={'cookieAuth': 'abc123'}
+    api_key_prefix={'cookieAuth': 'JSESSIONID'}
+)
+
+    The following cookie will be added to the HTTP request:
+       Cookie: JSESSIONID abc123
     """
 
     _default = None
 
-    def __init__(
-        self,
-        host=None,
-        discard_unknown_keys=False,
-        disabled_client_side_validations="",
-        server_index=None,
-        server_variables=None,
-        server_operation_index=None,
-        server_operation_variables=None,
-        access_token=None,
-    ):
+    def __init__(self, host="http://localhost",
+                 api_key=None, api_key_prefix=None,
+                 username=None, password=None,
+                 discard_unknown_keys=False,
+                 ):
         """Constructor
         """
-        self._base_path = "http://localhost" if host is None else host
+        self.host = host
         """Default Base url
         """
-        self.server_index = 0 if server_index is None and host is None else server_index
-        self.server_operation_index = server_operation_index or {}
-        """Default server index
-        """
-        self.server_variables = server_variables or {}
-        self.server_operation_variables = server_operation_variables or {}
-        """Default server variables
-        """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.api_key = {}
+        if api_key:
+            self.api_key = api_key
+        """dict to store API key(s)
+        """
+        self.api_key_prefix = {}
+        if api_key_prefix:
+            self.api_key_prefix = api_key_prefix
+        """dict to store API prefix (e.g. Bearer)
+        """
+        self.refresh_api_key_hook = None
+        """function hook to refresh API key if expired
+        """
+        self.username = username
+        """Username for HTTP basic authentication
+        """
+        self.password = password
+        """Password for HTTP basic authentication
+        """
+        self.discard_unknown_keys = discard_unknown_keys
         self.access_token = None
         """access token for OAuth/Bearer
         """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("data_repo_client")
@@ -147,18 +145,14 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
-        self.tls_server_name = None
-        """SSL/TLS Server Name Indication (SNI)
-           Set this to the SNI value expected by the server.
-        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
@@ -172,20 +166,17 @@
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
-        # Enable client side validation
+        # Disable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
-        self.socket_options = None
-
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
                 setattr(result, k, copy.deepcopy(v, memo))
@@ -194,21 +185,14 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
@@ -255,15 +239,15 @@
         """
         self.__logger_file = value
         if self.__logger_file:
             # If set logging file,
             # then add file handler and remove stream handler.
             self.logger_file_handler = logging.FileHandler(self.__logger_file)
             self.logger_file_handler.setFormatter(self.logger_formatter)
-            for _, logger in self.logger.items():
+            for _, logger in six.iteritems(self.logger):
                 logger.addHandler(self.logger_file_handler)
 
     @property
     def debug(self):
         """Debug status
 
         :param value: The debug status, True or False.
@@ -277,25 +261,25 @@
 
         :param value: The debug status, True or False.
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
-            for _, logger in self.logger.items():
+            for _, logger in six.iteritems(self.logger):
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
-            for _, logger in self.logger.items():
+            for _, logger in six.iteritems(self.logger):
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -312,24 +296,23 @@
 
         :param value: The format string.
         :type: str
         """
         self.__logger_format = value
         self.logger_formatter = logging.Formatter(self.__logger_format)
 
-    def get_api_key_with_prefix(self, identifier, alias=None):
+    def get_api_key_with_prefix(self, identifier):
         """Gets API key (with prefix if set).
 
         :param identifier: The identifier of apiKey.
-        :param alias: The alternative identifier of apiKey.
         :return: The token for api key authentication.
         """
         if self.refresh_api_key_hook is not None:
             self.refresh_api_key_hook(self)
-        key = self.api_key.get(identifier, self.api_key.get(alias) if alias is not None else None)
+        key = self.api_key.get(identifier)
         if key:
             prefix = self.api_key_prefix.get(identifier)
             if prefix:
                 return "%s %s" % (prefix, key)
             else:
                 return key
 
@@ -350,23 +333,23 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
-        if self.access_token is not None:
-            auth['googleoauth'] = {
-                'type': 'oauth2',
+        if 'Authorization' in self.api_key:
+            auth['authToken'] = {
+                'type': 'api_key',
                 'in': 'header',
                 'key': 'Authorization',
-                'value': 'Bearer ' + self.access_token
+                'value': self.get_api_key_with_prefix('Authorization')
             }
         if self.access_token is not None:
-            auth['oidc'] = {
+            auth['googleoauth'] = {
                 'type': 'oauth2',
                 'in': 'header',
                 'key': 'Authorization',
                 'value': 'Bearer ' + self.access_token
             }
         return auth
 
@@ -375,71 +358,56 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 1.495.0".\
+               "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "",
+                'url': "/",
                 'description': "No description provided",
             }
         ]
 
-    def get_host_from_settings(self, index, variables=None, servers=None):
+    def get_host_from_settings(self, index, variables=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
-        :param servers: an array of host settings or None
         :return: URL based on host settings
         """
-        if index is None:
-            return self._base_path
-
         variables = {} if variables is None else variables
-        servers = self.get_host_settings() if servers is None else servers
+        servers = self.get_host_settings()
 
         try:
             server = servers[index]
         except IndexError:
             raise ValueError(
                 "Invalid index {0} when selecting the host settings. "
                 "Must be less than {1}".format(index, len(servers)))
 
         url = server['url']
 
         # go through variables and replace placeholders
-        for variable_name, variable in server.get('variables', {}).items():
+        for variable_name, variable in server['variables'].items():
             used_value = variables.get(
                 variable_name, variable['default_value'])
 
             if 'enum_values' in variable \
                     and used_value not in variable['enum_values']:
                 raise ValueError(
                     "The variable `{0}` in the host URL has invalid value "
                     "{1}. Must be {2}.".format(
                         variable_name, variables[variable_name],
                         variable['enum_values']))
 
             url = url.replace("{" + variable_name + "}", used_value)
 
         return url
-
-    @property
-    def host(self):
-        """Return generated host."""
-        return self.get_host_from_settings(self.server_index, variables=self.server_variables)
-
-    @host.setter
-    def host(self, value):
-        """Fix base path."""
-        self._base_path = value
-        self.server_index = None
```

### Comparing `data-repo-client-1.495.0/data_repo_client/model/column_statistics_text_model.py` & `data-repo-client-1.64.0/data_repo_client/models/table_data_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,148 +1,114 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
+
+import pprint
 import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
 
-import frozendict  # noqa: F401
+import six
 
-from data_repo_client import schemas  # noqa: F401
+from data_repo_client.configuration import Configuration
 
 
-class ColumnStatisticsTextModel(
-    schemas.ComposedSchema,
-):
+class TableDataType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+    """
+    allowed enum values
+    """
+    BOOLEAN = "boolean"
+    BYTES = "bytes"
+    DATE = "date"
+    DATETIME = "datetime"
+    DIRREF = "dirref"
+    FILEREF = "fileref"
+    FLOAT = "float"
+    FLOAT64 = "float64"
+    INTEGER = "integer"
+    INT64 = "int64"
+    NUMERIC = "numeric"
+    RECORD = "record"
+    STRING = "string"
+    TEXT = "text"
+    TIME = "time"
+    TIMESTAMP = "timestamp"
+
+    allowable_values = [BOOLEAN, BYTES, DATE, DATETIME, DIRREF, FILEREF, FLOAT, FLOAT64, INTEGER, INT64, NUMERIC, RECORD, STRING, TEXT, TIME, TIMESTAMP]  # noqa: E501
+
+    """
+    Attributes:
+      openapi_types (dict): The key is attribute name
+                            and the value is attribute type.
+      attribute_map (dict): The key is attribute name
+                            and the value is json key in definition.
+    """
+    openapi_types = {
+    }
+
+    attribute_map = {
+    }
 
-    class MetaOapg:
-        
-        
-        class all_of_1(
-            schemas.DictSchema
-        ):
-        
-        
-            class MetaOapg:
-                required = {
-                    "values",
-                }
-                
-                class properties:
-                    
-                    
-                    class values(
-                        schemas.ListSchema
-                    ):
-                    
-                    
-                        class MetaOapg:
-                            
-                            @staticmethod
-                            def items() -> typing.Type['ColumnStatisticsTextValue']:
-                                return ColumnStatisticsTextValue
-                    
-                        def __new__(
-                            cls,
-                            _arg: typing.Union[typing.Tuple['ColumnStatisticsTextValue'], typing.List['ColumnStatisticsTextValue']],
-                            _configuration: typing.Optional[schemas.Configuration] = None,
-                        ) -> 'values':
-                            return super().__new__(
-                                cls,
-                                _arg,
-                                _configuration=_configuration,
-                            )
-                    
-                        def __getitem__(self, i: int) -> 'ColumnStatisticsTextValue':
-                            return super().__getitem__(i)
-                    __annotations__ = {
-                        "values": values,
-                    }
-            
-            values: MetaOapg.properties.values
-            
-            @typing.overload
-            def __getitem__(self, name: typing_extensions.Literal["values"]) -> MetaOapg.properties.values: ...
-            
-            @typing.overload
-            def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-            
-            def __getitem__(self, name: typing.Union[typing_extensions.Literal["values", ], str]):
-                # dict_instance[name] accessor
-                return super().__getitem__(name)
-            
-            
-            @typing.overload
-            def get_item_oapg(self, name: typing_extensions.Literal["values"]) -> MetaOapg.properties.values: ...
-            
-            @typing.overload
-            def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-            
-            def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["values", ], str]):
-                return super().get_item_oapg(name)
-            
-        
-            def __new__(
-                cls,
-                *_args: typing.Union[dict, frozendict.frozendict, ],
-                values: typing.Union[MetaOapg.properties.values, list, tuple, ],
-                _configuration: typing.Optional[schemas.Configuration] = None,
-                **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-            ) -> 'all_of_1':
-                return super().__new__(
-                    cls,
-                    *_args,
-                    values=values,
-                    _configuration=_configuration,
-                    **kwargs,
-                )
-        
-        @classmethod
-        @functools.lru_cache()
-        def all_of(cls):
-            # we need this here to make our import statements work
-            # we must store _composed_schemas in here so the code is only run
-            # when we invoke this method. If we kept this at the class
-            # level we would get an error because the class level
-            # code would be run when this module is imported, and these composed
-            # classes don't exist yet because their module has not finished
-            # loading
-            return [
-                ColumnStatisticsModel,
-                cls.all_of_1,
-            ]
-
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ColumnStatisticsTextModel':
-        return super().__new__(
-            cls,
-            *_args,
-            _configuration=_configuration,
-            **kwargs,
-        )
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """TableDataType - a model defined in OpenAPI"""  # noqa: E501
+        if local_vars_configuration is None:
+            local_vars_configuration = Configuration()
+        self.local_vars_configuration = local_vars_configuration
+        self.discriminator = None
+
+    def to_dict(self):
+        """Returns the model properties as a dict"""
+        result = {}
+
+        for attr, _ in six.iteritems(self.openapi_types):
+            value = getattr(self, attr)
+            if isinstance(value, list):
+                result[attr] = list(map(
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
+                    value
+                ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
+            elif isinstance(value, dict):
+                result[attr] = dict(map(
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
+                    value.items()
+                ))
+            else:
+                result[attr] = value
+
+        return result
+
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return pprint.pformat(self.to_dict())
+
+    def __repr__(self):
+        """For `print` and `pprint`"""
+        return self.to_str()
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, TableDataType):
+            return False
+
+        return self.to_dict() == other.to_dict()
+
+    def __ne__(self, other):
+        """Returns true if both objects are not equal"""
+        if not isinstance(other, TableDataType):
+            return True
 
-from data_repo_client.model.column_statistics_model import ColumnStatisticsModel
-from data_repo_client.model.column_statistics_text_value import ColumnStatisticsTextValue
+        return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.495.0/data_repo_client/model/data_deletion_json_array_model.py` & `data-repo-client-1.64.0/test/test_snapshot_request_asset_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,59 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from data_repo_client import schemas  # noqa: F401
-
-
-class DataDeletionJsonArrayModel(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    a specification of row ids to delete
-
-    """
-
-
-    class MetaOapg:
-        required = {
-            "rowIds",
-        }
-        
-        class properties:
-            
-            
-            class rowIds(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.UUIDSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, uuid.UUID, ]], typing.List[typing.Union[MetaOapg.items, str, uuid.UUID, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'rowIds':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "rowIds": rowIds,
-            }
-    
-    rowIds: MetaOapg.properties.rowIds
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["rowIds"]) -> MetaOapg.properties.rowIds: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["rowIds", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["rowIds"]) -> MetaOapg.properties.rowIds: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["rowIds", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        rowIds: typing.Union[MetaOapg.properties.rowIds, list, tuple, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataDeletionJsonArrayModel':
-        return super().__new__(
-            cls,
-            *_args,
-            rowIds=rowIds,
-            _configuration=_configuration,
-            **kwargs,
+
+from __future__ import absolute_import
+
+import unittest
+import datetime
+
+import data_repo_client
+from data_repo_client.models.snapshot_request_asset_model import SnapshotRequestAssetModel  # noqa: E501
+from data_repo_client.rest import ApiException
+
+class TestSnapshotRequestAssetModel(unittest.TestCase):
+    """SnapshotRequestAssetModel unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SnapshotRequestAssetModel
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = data_repo_client.models.snapshot_request_asset_model.SnapshotRequestAssetModel()  # noqa: E501
+        if include_optional :
+            return SnapshotRequestAssetModel(
+                asset_name = 'a', 
+                root_values = [
+                    '0'
+                    ]
+            )
+        else :
+            return SnapshotRequestAssetModel(
+                asset_name = 'a',
+                root_values = [
+                    '0'
+                    ],
         )
+
+    def testSnapshotRequestAssetModel(self):
+        """Test SnapshotRequestAssetModel"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `data-repo-client-1.495.0/data_repo_client/model/delete_response_model.py` & `data-repo-client-1.64.0/test/test_relationship_term_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,55 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from data_repo_client import schemas  # noqa: F401
-
-
-class DeleteResponseModel(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Returns the state of the object of the deletion
-
-    """
-
-
-    class MetaOapg:
-        
-        class properties:
-            
-            
-            class objectState(
-                schemas.EnumBase,
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    enum_value_to_name = {
-                        "deleted": "DELETED",
-                        "not_found": "NOT_FOUND",
-                    }
-                
-                @schemas.classproperty
-                def DELETED(cls):
-                    return cls("deleted")
-                
-                @schemas.classproperty
-                def NOT_FOUND(cls):
-                    return cls("not_found")
-            __annotations__ = {
-                "objectState": objectState,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["objectState"]) -> MetaOapg.properties.objectState: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["objectState", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["objectState"]) -> typing.Union[MetaOapg.properties.objectState, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["objectState", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        objectState: typing.Union[MetaOapg.properties.objectState, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DeleteResponseModel':
-        return super().__new__(
-            cls,
-            *_args,
-            objectState=objectState,
-            _configuration=_configuration,
-            **kwargs,
+
+from __future__ import absolute_import
+
+import unittest
+import datetime
+
+import data_repo_client
+from data_repo_client.models.relationship_term_model import RelationshipTermModel  # noqa: E501
+from data_repo_client.rest import ApiException
+
+class TestRelationshipTermModel(unittest.TestCase):
+    """RelationshipTermModel unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test RelationshipTermModel
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = data_repo_client.models.relationship_term_model.RelationshipTermModel()  # noqa: E501
+        if include_optional :
+            return RelationshipTermModel(
+                table = 'a', 
+                column = 'a'
+            )
+        else :
+            return RelationshipTermModel(
+                table = 'a',
+                column = 'a',
         )
+
+    def testRelationshipTermModel(self):
+        """Test RelationshipTermModel"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `data-repo-client-1.495.0/data_repo_client/models/__init__.py` & `data-repo-client-1.64.0/data_repo_client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,148 +1,108 @@
 # coding: utf-8
 
 # flake8: noqa
 
-# import all models into this package
-# if you have many models here with many references from one model to another this may
-# raise a RecursionError
-# to avoid this, import only the models that you directly need like:
-# from data_repo_client.model.pet import Pet
-# or import this package, but before doing it, use:
-# import sys
-# sys.setrecursionlimit(n)
-
-from data_repo_client.model.access_info_big_query_model import AccessInfoBigQueryModel
-from data_repo_client.model.access_info_big_query_model_table import AccessInfoBigQueryModelTable
-from data_repo_client.model.access_info_model import AccessInfoModel
-from data_repo_client.model.access_info_parquet_model import AccessInfoParquetModel
-from data_repo_client.model.access_info_parquet_model_table import AccessInfoParquetModelTable
-from data_repo_client.model.asset_model import AssetModel
-from data_repo_client.model.asset_table_model import AssetTableModel
-from data_repo_client.model.billing_profile_model import BillingProfileModel
-from data_repo_client.model.billing_profile_request_model import BillingProfileRequestModel
-from data_repo_client.model.billing_profile_update_model import BillingProfileUpdateModel
-from data_repo_client.model.bulk_load_array_request_model import BulkLoadArrayRequestModel
-from data_repo_client.model.bulk_load_array_result_model import BulkLoadArrayResultModel
-from data_repo_client.model.bulk_load_file_model import BulkLoadFileModel
-from data_repo_client.model.bulk_load_file_result_model import BulkLoadFileResultModel
-from data_repo_client.model.bulk_load_file_state import BulkLoadFileState
-from data_repo_client.model.bulk_load_history_model import BulkLoadHistoryModel
-from data_repo_client.model.bulk_load_history_model_list import BulkLoadHistoryModelList
-from data_repo_client.model.bulk_load_request_model import BulkLoadRequestModel
-from data_repo_client.model.bulk_load_result_model import BulkLoadResultModel
-from data_repo_client.model.cloud_platform import CloudPlatform
-from data_repo_client.model.column_model import ColumnModel
-from data_repo_client.model.column_name_property import ColumnNameProperty
-from data_repo_client.model.column_statistics_double_model import ColumnStatisticsDoubleModel
-from data_repo_client.model.column_statistics_int_model import ColumnStatisticsIntModel
-from data_repo_client.model.column_statistics_model import ColumnStatisticsModel
-from data_repo_client.model.column_statistics_text_model import ColumnStatisticsTextModel
-from data_repo_client.model.column_statistics_text_value import ColumnStatisticsTextValue
-from data_repo_client.model.compact_id_prefix import CompactIdPrefix
-from data_repo_client.model.config_enable_model import ConfigEnableModel
-from data_repo_client.model.config_fault_counted_model import ConfigFaultCountedModel
-from data_repo_client.model.config_fault_model import ConfigFaultModel
-from data_repo_client.model.config_group_model import ConfigGroupModel
-from data_repo_client.model.config_list_model import ConfigListModel
-from data_repo_client.model.config_model import ConfigModel
-from data_repo_client.model.config_parameter_model import ConfigParameterModel
-from data_repo_client.model.consent_code import ConsentCode
-from data_repo_client.model.drs_access_method import DRSAccessMethod
-from data_repo_client.model.drs_access_url import DRSAccessURL
-from data_repo_client.model.drs_authorizations import DRSAuthorizations
-from data_repo_client.model.drs_checksum import DRSChecksum
-from data_repo_client.model.drs_contents_object import DRSContentsObject
-from data_repo_client.model.drs_error import DRSError
-from data_repo_client.model.drs_object import DRSObject
-from data_repo_client.model.drs_passport_request_model import DRSPassportRequestModel
-from data_repo_client.model.drs_service_info import DRSServiceInfo
-from data_repo_client.model.data_deletion_gcs_file_model import DataDeletionGcsFileModel
-from data_repo_client.model.data_deletion_json_array_model import DataDeletionJsonArrayModel
-from data_repo_client.model.data_deletion_request import DataDeletionRequest
-from data_repo_client.model.data_deletion_table_model import DataDeletionTableModel
-from data_repo_client.model.dataset_data_model import DatasetDataModel
-from data_repo_client.model.dataset_model import DatasetModel
-from data_repo_client.model.dataset_patch_request_model import DatasetPatchRequestModel
-from data_repo_client.model.dataset_request_access_include_model import DatasetRequestAccessIncludeModel
-from data_repo_client.model.dataset_request_model import DatasetRequestModel
-from data_repo_client.model.dataset_schema_column_update_model import DatasetSchemaColumnUpdateModel
-from data_repo_client.model.dataset_schema_update_model import DatasetSchemaUpdateModel
-from data_repo_client.model.dataset_snapshot_name_property import DatasetSnapshotNameProperty
-from data_repo_client.model.dataset_specification_model import DatasetSpecificationModel
-from data_repo_client.model.dataset_summary_model import DatasetSummaryModel
-from data_repo_client.model.date_partition_options_model import DatePartitionOptionsModel
-from data_repo_client.model.delete_response_model import DeleteResponseModel
-from data_repo_client.model.directory_detail_model import DirectoryDetailModel
-from data_repo_client.model.drs_alias_model import DrsAliasModel
-from data_repo_client.model.duos_firecloud_group_model import DuosFirecloudGroupModel
-from data_repo_client.model.duos_firecloud_groups_sync_response import DuosFirecloudGroupsSyncResponse
-from data_repo_client.model.duos_id import DuosId
-from data_repo_client.model.enumerate_billing_profile_model import EnumerateBillingProfileModel
-from data_repo_client.model.enumerate_dataset_model import EnumerateDatasetModel
-from data_repo_client.model.enumerate_snapshot_model import EnumerateSnapshotModel
-from data_repo_client.model.enumerate_sort_by_param import EnumerateSortByParam
-from data_repo_client.model.error_model import ErrorModel
-from data_repo_client.model.file_detail_model import FileDetailModel
-from data_repo_client.model.file_load_model import FileLoadModel
-from data_repo_client.model.file_model import FileModel
-from data_repo_client.model.file_model_type import FileModelType
-from data_repo_client.model.iam_resource_type_enum import IamResourceTypeEnum
-from data_repo_client.model.inaccessible_workspace_policy_model import InaccessibleWorkspacePolicyModel
-from data_repo_client.model.ingest_request_model import IngestRequestModel
-from data_repo_client.model.ingest_response_model import IngestResponseModel
-from data_repo_client.model.int_partition_options_model import IntPartitionOptionsModel
-from data_repo_client.model.job_model import JobModel
-from data_repo_client.model.journal_entry_model import JournalEntryModel
-from data_repo_client.model.load_tag_model import LoadTagModel
-from data_repo_client.model.md5_override_model import Md5OverrideModel
-from data_repo_client.model.object_name_property import ObjectNameProperty
-from data_repo_client.model.phs_id import PhsId
-from data_repo_client.model.policy_member_request import PolicyMemberRequest
-from data_repo_client.model.policy_model import PolicyModel
-from data_repo_client.model.policy_response import PolicyResponse
-from data_repo_client.model.relationship_model import RelationshipModel
-from data_repo_client.model.relationship_term_model import RelationshipTermModel
-from data_repo_client.model.repository_configuration_model import RepositoryConfigurationModel
-from data_repo_client.model.repository_status_model import RepositoryStatusModel
-from data_repo_client.model.resource_create_tags import ResourceCreateTags
-from data_repo_client.model.resource_locks import ResourceLocks
-from data_repo_client.model.resource_policy_model import ResourcePolicyModel
-from data_repo_client.model.sam_policy_model import SamPolicyModel
-from data_repo_client.model.search_index_model import SearchIndexModel
-from data_repo_client.model.search_index_request import SearchIndexRequest
-from data_repo_client.model.search_metadata_model import SearchMetadataModel
-from data_repo_client.model.search_metadata_response import SearchMetadataResponse
-from data_repo_client.model.search_query_request import SearchQueryRequest
-from data_repo_client.model.search_query_result_model import SearchQueryResultModel
-from data_repo_client.model.short_id_property import ShortIdProperty
-from data_repo_client.model.snapshot_export_response_model import SnapshotExportResponseModel
-from data_repo_client.model.snapshot_ids_and_roles_model import SnapshotIdsAndRolesModel
-from data_repo_client.model.snapshot_link_duos_dataset_response import SnapshotLinkDuosDatasetResponse
-from data_repo_client.model.snapshot_model import SnapshotModel
-from data_repo_client.model.snapshot_patch_request_model import SnapshotPatchRequestModel
-from data_repo_client.model.snapshot_preview_model import SnapshotPreviewModel
-from data_repo_client.model.snapshot_request_asset_model import SnapshotRequestAssetModel
-from data_repo_client.model.snapshot_request_contents_model import SnapshotRequestContentsModel
-from data_repo_client.model.snapshot_request_model import SnapshotRequestModel
-from data_repo_client.model.snapshot_request_query_model import SnapshotRequestQueryModel
-from data_repo_client.model.snapshot_request_row_id_model import SnapshotRequestRowIdModel
-from data_repo_client.model.snapshot_request_row_id_table_model import SnapshotRequestRowIdTableModel
-from data_repo_client.model.snapshot_retrieve_include_model import SnapshotRetrieveIncludeModel
-from data_repo_client.model.snapshot_source_model import SnapshotSourceModel
-from data_repo_client.model.snapshot_summary_model import SnapshotSummaryModel
-from data_repo_client.model.sql_sort_direction import SqlSortDirection
-from data_repo_client.model.storage_resource_model import StorageResourceModel
-from data_repo_client.model.table_data_type import TableDataType
-from data_repo_client.model.table_model import TableModel
-from data_repo_client.model.tag import Tag
-from data_repo_client.model.tag_count import TagCount
-from data_repo_client.model.tag_count_result_model import TagCountResultModel
-from data_repo_client.model.tag_update_request_model import TagUpdateRequestModel
-from data_repo_client.model.transaction_close_model import TransactionCloseModel
-from data_repo_client.model.transaction_create_model import TransactionCreateModel
-from data_repo_client.model.transaction_model import TransactionModel
-from data_repo_client.model.unique_id_property import UniqueIdProperty
-from data_repo_client.model.upgrade_model import UpgradeModel
-from data_repo_client.model.upgrade_response_model import UpgradeResponseModel
-from data_repo_client.model.user_status_info import UserStatusInfo
-from data_repo_client.model.workspace_policy_model import WorkspacePolicyModel
+"""
+    Data Repository API
+
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+from __future__ import absolute_import
+
+__version__ = "1.0.0"
+
+# import apis into sdk package
+from data_repo_client.api.data_repository_service_api import DataRepositoryServiceApi
+from data_repo_client.api.repository_api import RepositoryApi
+from data_repo_client.api.resources_api import ResourcesApi
+from data_repo_client.api.unauthenticated_api import UnauthenticatedApi
+
+# import ApiClient
+from data_repo_client.api_client import ApiClient
+from data_repo_client.configuration import Configuration
+from data_repo_client.exceptions import OpenApiException
+from data_repo_client.exceptions import ApiTypeError
+from data_repo_client.exceptions import ApiValueError
+from data_repo_client.exceptions import ApiKeyError
+from data_repo_client.exceptions import ApiException
+# import models into sdk package
+from data_repo_client.models.asset_model import AssetModel
+from data_repo_client.models.asset_table_model import AssetTableModel
+from data_repo_client.models.billing_profile_model import BillingProfileModel
+from data_repo_client.models.billing_profile_request_model import BillingProfileRequestModel
+from data_repo_client.models.billing_profile_update_model import BillingProfileUpdateModel
+from data_repo_client.models.bulk_load_array_request_model import BulkLoadArrayRequestModel
+from data_repo_client.models.bulk_load_array_result_model import BulkLoadArrayResultModel
+from data_repo_client.models.bulk_load_file_model import BulkLoadFileModel
+from data_repo_client.models.bulk_load_file_result_model import BulkLoadFileResultModel
+from data_repo_client.models.bulk_load_file_state import BulkLoadFileState
+from data_repo_client.models.bulk_load_history_model import BulkLoadHistoryModel
+from data_repo_client.models.bulk_load_request_model import BulkLoadRequestModel
+from data_repo_client.models.bulk_load_result_model import BulkLoadResultModel
+from data_repo_client.models.column_model import ColumnModel
+from data_repo_client.models.config_enable_model import ConfigEnableModel
+from data_repo_client.models.config_fault_counted_model import ConfigFaultCountedModel
+from data_repo_client.models.config_fault_model import ConfigFaultModel
+from data_repo_client.models.config_group_model import ConfigGroupModel
+from data_repo_client.models.config_list_model import ConfigListModel
+from data_repo_client.models.config_model import ConfigModel
+from data_repo_client.models.config_parameter_model import ConfigParameterModel
+from data_repo_client.models.drs_access_method import DRSAccessMethod
+from data_repo_client.models.drs_access_url import DRSAccessURL
+from data_repo_client.models.drs_checksum import DRSChecksum
+from data_repo_client.models.drs_contents_object import DRSContentsObject
+from data_repo_client.models.drs_error import DRSError
+from data_repo_client.models.drs_object import DRSObject
+from data_repo_client.models.drs_service_info import DRSServiceInfo
+from data_repo_client.models.data_deletion_gcs_file_model import DataDeletionGcsFileModel
+from data_repo_client.models.data_deletion_request import DataDeletionRequest
+from data_repo_client.models.data_deletion_table_model import DataDeletionTableModel
+from data_repo_client.models.dataset_model import DatasetModel
+from data_repo_client.models.dataset_request_model import DatasetRequestModel
+from data_repo_client.models.dataset_specification_model import DatasetSpecificationModel
+from data_repo_client.models.dataset_summary_model import DatasetSummaryModel
+from data_repo_client.models.date_partition_options_model import DatePartitionOptionsModel
+from data_repo_client.models.delete_response_model import DeleteResponseModel
+from data_repo_client.models.directory_detail_model import DirectoryDetailModel
+from data_repo_client.models.enumerate_billing_profile_model import EnumerateBillingProfileModel
+from data_repo_client.models.enumerate_dataset_model import EnumerateDatasetModel
+from data_repo_client.models.enumerate_snapshot_model import EnumerateSnapshotModel
+from data_repo_client.models.enumerate_sort_by_param import EnumerateSortByParam
+from data_repo_client.models.error_model import ErrorModel
+from data_repo_client.models.file_detail_model import FileDetailModel
+from data_repo_client.models.file_load_model import FileLoadModel
+from data_repo_client.models.file_model import FileModel
+from data_repo_client.models.file_model_type import FileModelType
+from data_repo_client.models.ingest_request_model import IngestRequestModel
+from data_repo_client.models.ingest_response_model import IngestResponseModel
+from data_repo_client.models.int_partition_options_model import IntPartitionOptionsModel
+from data_repo_client.models.job_model import JobModel
+from data_repo_client.models.policy_member_request import PolicyMemberRequest
+from data_repo_client.models.policy_model import PolicyModel
+from data_repo_client.models.policy_response import PolicyResponse
+from data_repo_client.models.relationship_model import RelationshipModel
+from data_repo_client.models.relationship_term_model import RelationshipTermModel
+from data_repo_client.models.repository_configuration_model import RepositoryConfigurationModel
+from data_repo_client.models.repository_status_model import RepositoryStatusModel
+from data_repo_client.models.repository_status_model_systems import RepositoryStatusModelSystems
+from data_repo_client.models.snapshot_model import SnapshotModel
+from data_repo_client.models.snapshot_request_asset_model import SnapshotRequestAssetModel
+from data_repo_client.models.snapshot_request_contents_model import SnapshotRequestContentsModel
+from data_repo_client.models.snapshot_request_model import SnapshotRequestModel
+from data_repo_client.models.snapshot_request_query_model import SnapshotRequestQueryModel
+from data_repo_client.models.snapshot_request_row_id_model import SnapshotRequestRowIdModel
+from data_repo_client.models.snapshot_request_row_id_table_model import SnapshotRequestRowIdTableModel
+from data_repo_client.models.snapshot_source_model import SnapshotSourceModel
+from data_repo_client.models.snapshot_summary_model import SnapshotSummaryModel
+from data_repo_client.models.sql_sort_direction import SqlSortDirection
+from data_repo_client.models.table_data_type import TableDataType
+from data_repo_client.models.table_model import TableModel
+from data_repo_client.models.upgrade_model import UpgradeModel
+from data_repo_client.models.upgrade_response_model import UpgradeResponseModel
+from data_repo_client.models.user_status_info import UserStatusInfo
+
```

### Comparing `data-repo-client-1.495.0/setup.py` & `data-repo-client-1.64.0/data_repo_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,12 @@
-# coding: utf-8
-
-"""
-    Data Repository API
-
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from setuptools import setup, find_packages  # noqa: H301
-
-NAME = "data-repo-client"
-VERSION = "1.495.0"
-# To install the library, run the following
-#
-# python setup.py install
-#
-# prerequisite: setuptools
-# http://pypi.python.org/pypi/setuptools
-
-REQUIRES = [
-    "certifi >= 14.5.14",
-    "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
-    "setuptools >= 21.0.0",
-    "typing_extensions ~= 4.3.0",
-    "urllib3 ~= 1.26.7",
-]
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description="Data Repository API",
-    author="OpenAPI Generator community",
-    author_email="team@openapitools.org",
-    url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Data Repository API"],
-    python_requires=">=3.7",
-    install_requires=REQUIRES,
-    packages=find_packages(exclude=["test", "tests"]),
-    include_package_data=True,
-    license="Apache 2.0",
-    long_description="""\
-    &lt;details&gt;&lt;summary&gt;This document defines the REST API for the Terra Data Repository.&lt;/summary&gt; &lt;p&gt; **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. &lt;p&gt; **Notes on Naming** &lt;p&gt; All of the reference items are suffixed with \\\&quot;Model\\\&quot;. Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. &lt;/details&gt;   # noqa: E501
-    """
-)
+Metadata-Version: 1.0
+Name: data-repo-client
+Version: 1.64.0
+Summary: Data Repository API
+Home-page: UNKNOWN
+Author: OpenAPI Generator community
+Author-email: team@openapitools.org
+License: Apache 2.0
+Description:     This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \&quot;Model\&quot;. Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: &#x60;&#x60;&#x60; docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor &#x60;&#x60;&#x60; Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with &#39;DRS&#39; to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
+            
+Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
+Platform: UNKNOWN
```

