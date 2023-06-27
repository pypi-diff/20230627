# Comparing `tmp/pyogmios-0.7.1.tar.gz` & `tmp/pyogmios-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyogmios-0.7.1.tar", max compression
+gzip compressed data, was "pyogmios-0.7.2.tar", max compression
```

## Comparing `pyogmios-0.7.1.tar` & `pyogmios-0.7.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     8987 2023-06-18 20:32:48.588485 pyogmios-0.7.1/README.md
--rw-r--r--   0        0        0       22 2023-06-19 19:16:42.601321 pyogmios-0.7.1/pyogmios_client/__init__.py
--rw-r--r--   0        0        0     6150 2023-06-19 19:02:32.153169 pyogmios-0.7.1/pyogmios_client/connection.py
--rw-r--r--   0        0        0     1767 2023-06-14 02:13:31.891113 pyogmios-0.7.1/pyogmios_client/enums/__init__.py
--rw-r--r--   0        0        0     2401 2023-06-18 20:30:32.505186 pyogmios-0.7.1/pyogmios_client/exceptions.py
--rw-r--r--   0        0        0    49367 2023-06-18 20:29:46.297072 pyogmios-0.7.1/pyogmios_client/models/__init__.py
--rw-r--r--   0        0        0      829 2023-06-02 00:12:52.975582 pyogmios-0.7.1/pyogmios_client/models/base_model.py
--rw-r--r--   0        0        0      391 2023-06-18 20:29:46.297119 pyogmios-0.7.1/pyogmios_client/models/base_request_response_model.py
--rw-r--r--   0        0        0      142 2023-05-29 12:12:30.855476 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/__init__.py
--rw-r--r--   0        0        0      768 2023-06-02 05:09:09.052857 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py
--rw-r--r--   0        0        0      481 2023-06-02 05:09:09.053018 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/txPayload__.py
--rw-r--r--   0        0        0      657 2023-06-02 05:09:09.055011 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block___.py
--rw-r--r--   0        0        0    96308 2023-06-04 20:21:45.553261 pyogmios-0.7.1/pyogmios_client/models/generated/__init__.py
--rw-r--r--   0        0        0     2247 2023-06-18 20:29:46.297175 pyogmios-0.7.1/pyogmios_client/models/request_model.py
--rw-r--r--   0        0        0     6746 2023-06-19 19:01:43.896476 pyogmios-0.7.1/pyogmios_client/models/response_model.py
--rw-r--r--   0        0        0     7881 2023-06-19 19:01:43.883277 pyogmios-0.7.1/pyogmios_client/models/result_models.py
--rw-r--r--   0        0        0     1642 2023-06-18 20:29:46.297316 pyogmios-0.7.1/pyogmios_client/models/server_health_model.py
--rw-r--r--   0        0        0        0 2023-05-26 12:54:40.062980 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:23.680249 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/__init__.py
--rw-r--r--   0        0        0     4979 2023-06-18 20:30:58.307688 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py
--rw-r--r--   0        0        0     2039 2023-06-18 20:30:58.307736 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py
--rw-r--r--   0        0        0      558 2023-06-18 20:30:58.307782 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:35.095043 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 11:49:09.937446 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/__init__.py
--rw-r--r--   0        0        0     1124 2023-06-19 13:26:03.805077 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py
--rw-r--r--   0        0        0     1058 2023-06-19 13:26:03.799723 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py
--rw-r--r--   0        0        0     1515 2023-06-19 13:26:03.787064 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py
--rw-r--r--   0        0        0     2442 2023-06-19 19:01:43.872490 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py
--rw-r--r--   0        0        0     2467 2023-06-19 19:01:43.889843 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py
--rw-r--r--   0        0        0     1417 2023-06-19 19:01:43.873064 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py
--rw-r--r--   0        0        0     1513 2023-06-19 12:51:57.285087 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py
--rw-r--r--   0        0        0     2330 2023-06-19 19:01:43.881035 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py
--rw-r--r--   0        0        0     2027 2023-06-19 13:26:03.775214 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py
--rw-r--r--   0        0        0     2374 2023-06-19 13:05:31.395379 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py
--rw-r--r--   0        0        0     1918 2023-06-19 13:26:03.802451 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py
--rw-r--r--   0        0        0     2201 2023-06-19 13:26:03.782424 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py
--rw-r--r--   0        0        0     1905 2023-06-19 13:26:03.776935 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py
--rw-r--r--   0        0        0     1720 2023-06-19 13:26:03.779645 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py
--rw-r--r--   0        0        0     1914 2023-06-19 19:01:44.042282 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py
--rw-r--r--   0        0        0     1958 2023-06-19 13:29:43.173810 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py
--rw-r--r--   0        0        0     1902 2023-06-19 19:01:44.042429 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py
--rw-r--r--   0        0        0     1093 2023-06-19 13:29:43.176699 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py
--rw-r--r--   0        0        0     2106 2023-06-19 13:39:50.892528 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py
--rw-r--r--   0        0        0     2297 2023-06-18 20:31:30.892685 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/query.py
--rw-r--r--   0        0        0    14518 2023-06-19 19:01:52.850535 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:49.879933 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-18 12:37:04.955397 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py
--rw-r--r--   0        0        0     1384 2023-06-18 20:20:34.012346 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py
--rw-r--r--   0        0        0     1703 2023-06-18 20:20:34.021771 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py
--rw-r--r--   0        0        0     1359 2023-06-18 20:20:34.030230 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py
--rw-r--r--   0        0        0     1507 2023-06-18 12:56:13.502657 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py
--rw-r--r--   0        0        0     3221 2023-06-18 20:20:34.074501 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py
--rw-r--r--   0        0        0        0 2023-05-26 12:33:01.699483 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/__init__.py
--rw-r--r--   0        0        0     4986 2023-06-18 20:20:34.090809 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py
--rw-r--r--   0        0        0     4171 2023-06-18 20:20:34.117964 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py
--rw-r--r--   0        0        0    22305 2023-06-18 20:20:34.306218 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py
--rw-r--r--   0        0        0    16290 2023-06-18 20:20:34.294212 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py
--rw-r--r--   0        0        0     3338 2023-06-18 20:20:34.059117 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py
--rw-r--r--   0        0        0      707 2023-06-18 20:30:32.505453 pyogmios-0.7.1/pyogmios_client/request.py
--rw-r--r--   0        0        0     1130 2023-06-18 20:30:32.505497 pyogmios-0.7.1/pyogmios_client/server_health.py
--rw-r--r--   0        0        0        0 2023-05-27 19:33:04.693841 pyogmios-0.7.1/pyogmios_client/utils/__init__.py
--rw-r--r--   0        0        0     2683 2023-06-18 20:20:34.070550 pyogmios-0.7.1/pyogmios_client/utils/event_emitter.py
--rw-r--r--   0        0        0     2538 2023-06-18 20:30:11.984569 pyogmios-0.7.1/pyogmios_client/utils/queue.py
--rw-r--r--   0        0        0      337 2023-06-19 19:02:32.153256 pyogmios-0.7.1/pyogmios_client/utils/socket_utils.py
--rw-r--r--   0        0        0     1532 2023-06-19 19:15:58.350847 pyogmios-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     9719 1970-01-01 00:00:00.000000 pyogmios-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 00:54:20.205293 pyogmios-0.7.2/LICENSE
+-rw-r--r--   0        0        0     8987 2023-06-18 20:32:48.588485 pyogmios-0.7.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 03:12:53.465216 pyogmios-0.7.2/pyogmios_client/__init__.py
+-rw-r--r--   0        0        0     6360 2023-06-27 02:56:56.199704 pyogmios-0.7.2/pyogmios_client/connection.py
+-rw-r--r--   0        0        0     1767 2023-06-14 02:13:31.891113 pyogmios-0.7.2/pyogmios_client/enums/__init__.py
+-rw-r--r--   0        0        0     3120 2023-06-27 02:56:56.187607 pyogmios-0.7.2/pyogmios_client/exceptions.py
+-rw-r--r--   0        0        0    49367 2023-06-18 20:29:46.297072 pyogmios-0.7.2/pyogmios_client/models/__init__.py
+-rw-r--r--   0        0        0      829 2023-06-02 00:12:52.975582 pyogmios-0.7.2/pyogmios_client/models/base_model.py
+-rw-r--r--   0        0        0      391 2023-06-18 20:29:46.297119 pyogmios-0.7.2/pyogmios_client/models/base_request_response_model.py
+-rw-r--r--   0        0        0      142 2023-05-29 12:12:30.855476 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/__init__.py
+-rw-r--r--   0        0        0      768 2023-06-02 05:09:09.052857 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-02 05:09:09.053018 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/txPayload__.py
+-rw-r--r--   0        0        0      657 2023-06-02 05:09:09.055011 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block___.py
+-rw-r--r--   0        0        0    96308 2023-06-04 20:21:45.553261 pyogmios-0.7.2/pyogmios_client/models/generated/__init__.py
+-rw-r--r--   0        0        0     2247 2023-06-18 20:29:46.297175 pyogmios-0.7.2/pyogmios_client/models/request_model.py
+-rw-r--r--   0        0        0     6746 2023-06-19 19:01:43.896476 pyogmios-0.7.2/pyogmios_client/models/response_model.py
+-rw-r--r--   0        0        0     7881 2023-06-19 19:01:43.883277 pyogmios-0.7.2/pyogmios_client/models/result_models.py
+-rw-r--r--   0        0        0     1642 2023-06-18 20:29:46.297316 pyogmios-0.7.2/pyogmios_client/models/server_health_model.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:54:40.062980 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:23.680249 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/__init__.py
+-rw-r--r--   0        0        0     4979 2023-06-18 20:30:58.307688 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py
+-rw-r--r--   0        0        0     2039 2023-06-18 20:30:58.307736 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py
+-rw-r--r--   0        0        0      558 2023-06-18 20:30:58.307782 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:35.095043 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:49:09.937446 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/__init__.py
+-rw-r--r--   0        0        0     1124 2023-06-19 13:26:03.805077 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py
+-rw-r--r--   0        0        0     1058 2023-06-19 13:26:03.799723 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py
+-rw-r--r--   0        0        0     1515 2023-06-19 13:26:03.787064 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py
+-rw-r--r--   0        0        0     2442 2023-06-19 19:01:43.872490 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py
+-rw-r--r--   0        0        0     2467 2023-06-19 19:01:43.889843 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py
+-rw-r--r--   0        0        0     1417 2023-06-19 19:01:43.873064 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py
+-rw-r--r--   0        0        0     1513 2023-06-19 12:51:57.285087 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py
+-rw-r--r--   0        0        0     2330 2023-06-19 19:01:43.881035 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py
+-rw-r--r--   0        0        0     2027 2023-06-19 13:26:03.775214 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py
+-rw-r--r--   0        0        0     2374 2023-06-19 13:05:31.395379 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py
+-rw-r--r--   0        0        0     1918 2023-06-19 13:26:03.802451 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py
+-rw-r--r--   0        0        0     2201 2023-06-19 13:26:03.782424 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py
+-rw-r--r--   0        0        0     1905 2023-06-19 13:26:03.776935 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py
+-rw-r--r--   0        0        0     1720 2023-06-19 13:26:03.779645 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py
+-rw-r--r--   0        0        0     1914 2023-06-19 19:01:44.042282 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py
+-rw-r--r--   0        0        0     1958 2023-06-19 13:29:43.173810 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py
+-rw-r--r--   0        0        0     1902 2023-06-19 19:01:44.042429 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py
+-rw-r--r--   0        0        0     1093 2023-06-19 13:29:43.176699 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py
+-rw-r--r--   0        0        0     2106 2023-06-19 13:39:50.892528 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py
+-rw-r--r--   0        0        0     2297 2023-06-18 20:31:30.892685 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/query.py
+-rw-r--r--   0        0        0    14518 2023-06-19 19:01:52.850535 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:49.879933 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-18 12:37:04.955397 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py
+-rw-r--r--   0        0        0     1384 2023-06-18 20:20:34.012346 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py
+-rw-r--r--   0        0        0     1703 2023-06-18 20:20:34.021771 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py
+-rw-r--r--   0        0        0     1359 2023-06-18 20:20:34.030230 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py
+-rw-r--r--   0        0        0     1507 2023-06-18 12:56:13.502657 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py
+-rw-r--r--   0        0        0     3221 2023-06-18 20:20:34.074501 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:33:01.699483 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/__init__.py
+-rw-r--r--   0        0        0     5139 2023-06-27 03:11:32.548129 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py
+-rw-r--r--   0        0        0     4669 2023-06-27 03:08:43.040389 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py
+-rw-r--r--   0        0        0    22331 2023-06-27 03:12:17.329092 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py
+-rw-r--r--   0        0        0    16290 2023-06-18 20:20:34.294212 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py
+-rw-r--r--   0        0        0     3338 2023-06-18 20:20:34.059117 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py
+-rw-r--r--   0        0        0      833 2023-06-27 02:55:56.143439 pyogmios-0.7.2/pyogmios_client/request.py
+-rw-r--r--   0        0        0     1407 2023-06-27 02:56:56.179854 pyogmios-0.7.2/pyogmios_client/server_health.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:33:04.693841 pyogmios-0.7.2/pyogmios_client/utils/__init__.py
+-rw-r--r--   0        0        0     2807 2023-06-27 02:55:56.143555 pyogmios-0.7.2/pyogmios_client/utils/event_emitter.py
+-rw-r--r--   0        0        0     3100 2023-06-27 02:55:56.143602 pyogmios-0.7.2/pyogmios_client/utils/queue.py
+-rw-r--r--   0        0        0      421 2023-06-27 02:55:56.143664 pyogmios-0.7.2/pyogmios_client/utils/socket_utils.py
+-rw-r--r--   0        0        0     1870 2023-06-27 03:17:39.383985 pyogmios-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 pyogmios-0.7.2/PKG-INFO
```

### Comparing `pyogmios-0.7.1/README.md` & `pyogmios-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/connection.py` & `pyogmios-0.7.2/pyogmios_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Create a connection to the server.
+
+This module contains the classes and default functions to create a connection to the server.
+"""
 import logging
 import threading
 from typing import Optional, Callable
 
 import websocket
 from websocket import WebSocketApp, enableTrace
 
@@ -13,26 +18,34 @@
     ConnectionConfig,
     Connection,
     Options as ServerHealthOptions,
 )
 
 
 class InteractionContext(BaseModel):
+    """
+    Interaction context model class
+    """
+
     connection: Connection
     socket: WebSocketApp
     after_each: Callable[[WebSocketApp, Callable[[], None]], None]
     log_level: str
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         logging.basicConfig(format="%(levelname)s - %(message)s")
         logging.getLogger().setLevel(logging.getLevelName(self.log_level.upper()))
 
 
 class InteractionContextOptions(BaseModel):
+    """
+    Interaction context options model class
+    """
+
     connection_config: Optional[ConnectionConfig]
     interaction_type: Optional[InteractionType]
     log_level: str = "DEBUG"
 
 
 def default_error_handler(_: WebSocketApp, error: Exception):
     """
@@ -147,15 +160,14 @@
 
         def on_message_handler(ws_app, message):
             """
             On message.
             :param ws_app: The websocket app
             :param message: The message
             """
-            print(f"Message: {message}")
             if message == "error":
                 on_initial_error(ws_app, Exception(message))
             elif message == "close":
                 raise WebSocketClosedError()
 
         def on_open_handler(_: WebSocketApp):
             """
```

### Comparing `pyogmios-0.7.1/pyogmios_client/enums/__init__.py` & `pyogmios-0.7.2/pyogmios_client/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/__init__.py` & `pyogmios-0.7.2/pyogmios_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/base_model.py` & `pyogmios-0.7.2/pyogmios_client/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py` & `pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block___.py` & `pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block___.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/generated/__init__.py` & `pyogmios-0.7.2/pyogmios_client/models/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/request_model.py` & `pyogmios-0.7.2/pyogmios_client/models/request_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/response_model.py` & `pyogmios-0.7.2/pyogmios_client/models/response_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/result_models.py` & `pyogmios-0.7.2/pyogmios_client/models/result_models.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/models/server_health_model.py` & `pyogmios-0.7.2/pyogmios_client/models/server_health_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/query.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/query.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module contains the evaluate_tx function.
+
+The evaluate_tx function is used to evaluate a transaction.
+"""
 import json
 from typing import Optional, List
 
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import UnknownResultError
 from pyogmios_client.models import (
@@ -32,14 +37,15 @@
     NonScriptInputReferencedByRedeemerError,
     UnknownInputReferencedByRedeemerError,
     ValidatorFailedError,
     IncompatibleEraError,
     AdditionalUtxoOverlapError,
     NotEnoughSyncedError,
     CannotCreateEvaluationContextError,
+    MissingRequiredDatumsError,
 )
 
 
 async def evaluate_tx(
     context: InteractionContext, bytes_: str, additional_utxo_set: Optional[Utxo] = None
 ) -> EvaluationResult | List[Exception]:
     """
@@ -90,15 +96,15 @@
                 for k in script_failures.keys():
                     failure = script_failures[k]
                     if isinstance(failure, ExtraRedeemers):
                         errors += ExtraRedeemersError(failure)
                     elif isinstance(failure, IllFormedExecutionBudget):
                         errors += IllFormedExecutionBudgetError(failure)
                     elif isinstance(failure, MissingRequiredDatums):
-                        errors += MissingRequiredDatums(failure)
+                        errors += MissingRequiredDatumsError(failure)
                     elif isinstance(failure, MissingRequiredScripts):
                         errors += MissingRequiredScriptsError(failure)
                     elif isinstance(failure, NoCostModelForLanguage):
                         errors += NoCostModelForLanguageError(failure)
                     elif isinstance(failure, NonScriptInputReferencedByRedeemer):
                         errors += NonScriptInputReferencedByRedeemerError(failure)
                     elif isinstance(failure, UnknownInputReferencedByRedeemer):
```

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+This module contains the error types that can be returned by the evaluation endpoint.
+
+The error types are:
+
+- AdditionalUtxoOverlapError
+- CannotCreateEvaluationContextError
+- ExtraRedeemersError
+- IllFormedExecutionBudgetError
+- IncompatibleEraError
+- MissingRequiredDatumsError
+- MissingRequiredScriptsError
+- NoCostModelForLanguageError
+- NonScriptInputReferencedByRedeemerError
+- NotEnoughSyncedError
+- UnknownInputReferencedByRedeemerError
+- UnknownResultError
+- ValidatorFailedError
+"""
 import json
 from typing import Union
 
 from pyogmios_client.models import (
     EvaluationFailureAdditionalUtxoOverlap,
     EvaluationFailureCannotCreateEvaluationContext,
     EvaluationFailureIncompatibleEra,
```

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     SubmitTxErrorMirNegativeTransferNotCurrentlyAllowed,
     SubmitTxErrorMirProducesNegativeUpdate,
     SubmitTxErrorMirTransferNotCurrentlyAllowed,
     SubmitTxErrorMissingAtLeastOneInputUtxo,
     SubmitTxErrorMissingCollateralInputs,
     SubmitTxErrorMissingDatumHashesForInputs,
     MissingRequiredDatums,
-    MissingRequiredRedeemers,
     SubmitTxErrorMissingRequiredSignatures,
     SubmitTxErrorMissingScriptWitnesses,
     SubmitTxErrorMissingTxMetadata,
     SubmitTxErrorMissingTxMetadataHash,
     SubmitTxErrorMissingVkWitnesses,
     SubmitTxErrorNetworkMismatch,
     SubmitTxErrorNonGenesisVoters,
@@ -64,14 +63,15 @@
     SubmitTxErrorUnspendableScriptInputs,
     SubmitTxErrorUpdateWrongEpoch,
     SubmitTxErrorValidationTagMismatch,
     SubmitTxErrorValueNotConserved,
     SubmitTxErrorWrongCertificateType,
     SubmitTxErrorWrongPoolCertificate,
     SubmitTxErrorWrongRetirementEpoch,
+    SubmitTxErrorMissingRequiredRedeemers,
 )
 from pyogmios_client.models.generated import SubmitTxErrorAddressAttributesTooLarge
 
 
 class AddressAttributesTooLargeError(Exception):
     """
     Address attributes too large error.
@@ -373,15 +373,15 @@
 
 
 class MissingRequiredRedeemersError(Exception):
     """
     Missing input witnesses error.
     """
 
-    def __init__(self, raw_error: MissingRequiredRedeemers):
+    def __init__(self, raw_error: SubmitTxErrorMissingRequiredRedeemers):
         super().__init__()
         self.message = json.dumps(raw_error.missingRequiredRedeemers)
 
 
 class MissingRequiredSignaturesError(Exception):
     """
     Missing input witnesses error.
```

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py` & `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.1/pyogmios_client/server_health.py` & `pyogmios-0.7.2/pyogmios_client/server_health.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,55 @@
+"""
+Server health module
+
+This module contains the functions to check the server health.
+"""
 from typing import Optional
 
 import aiohttp
 from pyogmios_client.models.base_model import BaseModel
 
 from pyogmios_client.exceptions import RequestError
 from pyogmios_client.models.server_health_model import ServerHealth
 
 
 class ConnectionConfig(BaseModel):
+    """
+    Connection configuration model class
+    """
+
     host: Optional[str]
     port: Optional[int]
     tls: Optional[bool]
     max_payload: Optional[int]
 
 
 class Address(BaseModel):
+    """
+    Address model class
+    """
+
     http: Optional[str]
     webSocket: Optional[str]
 
 
 class Connection(ConnectionConfig):
+    """
+    Connection model class
+    """
+
     max_payload: int
     address: Address
 
 
 class Options(BaseModel):
+    """
+    Options model class
+    """
+
     connection: Connection
 
 
 async def get_server_health(options: Options) -> ServerHealth | RequestError:
     """
     Checks the server health.
     :param options: The options
```

### Comparing `pyogmios-0.7.1/pyogmios_client/utils/event_emitter.py` & `pyogmios-0.7.2/pyogmios_client/utils/event_emitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module contains the EventEmitter class.
+
+The EventEmitter class can be used to emit events and listen to them.
+"""
 from typing import Dict
 
 from typing import TypeVar, Callable
 from queue import Queue
 
 T = TypeVar("T")
```

### Comparing `pyogmios-0.7.1/pyogmios_client/utils/queue.py` & `pyogmios-0.7.2/pyogmios_client/utils/queue.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+A queue that can be used to store tasks.
+
+This module contains the Queue class.
+"""
 from collections import deque
 from typing import Callable, Any
 
 from promise import Promise
 
 
 class Queue:
@@ -41,14 +46,20 @@
         :param element: The task to be added to the queue.
         :return:
         """
 
         def executor(
             resolve: Callable[[Any], None], reject: Callable[[Exception], None]
         ) -> None:
+            """
+            The executor function for the Promise.
+            :param resolve: The resolve function of the Promise.
+            :param reject: The reject function of the Promise.
+            :return: None
+            """
             try:
                 resolve(self.unshift(element))
             except Exception as error:
                 reject(error)
             return None
 
         return Promise(executor)
@@ -69,14 +80,20 @@
         :param element: The task to be added to the queue.
         :return: A Promise that will be fulfilled (rejected) when the task is completed successfully (unsuccessfully).
         """
 
         def executor(
             resolve: Callable[[Any], None], reject: Callable[[Exception], None]
         ) -> None:
+            """
+            The executor function for the Promise.
+            :param resolve: The resolve function of the Promise.
+            :param reject: The reject function of the Promise.
+            :return: None
+            """
             try:
                 resolve(self.push(element))
             except Exception as error:
                 reject(error)
             return None
 
         return Promise(executor)
```

### Comparing `pyogmios-0.7.1/PKG-INFO` & `pyogmios-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: pyogmios
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python client for Ogmios
 Author: Hareem Adderley
 Author-email: hadderley@kingpinapps.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.10,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: nanoid (>=2.0.0,<3.0.0)
 Requires-Dist: promise (>=2.3,<3.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Requires-Dist: pyee (>=9.1.0,<10.0.0)
+Requires-Dist: pyee (>=11.0.0,<12.0.0)
 Requires-Dist: rel (>=0.4.9,<0.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websocket-client (>=1.5.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PyOgmios
```

