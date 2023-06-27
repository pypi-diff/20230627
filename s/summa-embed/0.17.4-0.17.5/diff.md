# Comparing `tmp/summa_embed-0.17.4.tar.gz` & `tmp/summa_embed-0.17.5.tar.gz`

## Comparing `summa_embed-0.17.4.tar` & `summa_embed-0.17.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.4/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2381 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10598 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7789 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2523 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      394 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.4/local_dependencies/summa-server/Cargo.toml
--rw-r--r--   0      501       20       43 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/.cargo/config.toml
--rw-r--r--   0      501       20     1050 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/LICENSE
--rw-r--r--   0      501       20     2832 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/consumer.rs
--rw-r--r--   0      501       20    13268 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/index.rs
--rw-r--r--   0      501       20      105 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/mod.rs
--rw-r--r--   0      501       20     2909 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/reflection.rs
--rw-r--r--   0      501       20     1278 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/search.rs
--rw-r--r--   0      501       20      783 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/bin/main.rs
--rw-r--r--   0      501       20     5305 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumer_manager.rs
--rw-r--r--   0      501       20      813 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
--rw-r--r--   0      501       20     1082 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/dummy.rs
--rw-r--r--   0      501       20    11633 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
--rw-r--r--   0      501       20      270 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
--rw-r--r--   0      501       20      532 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
--rw-r--r--   0      501       20      155 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/mod.rs
--rw-r--r--   0      501       20     3811 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/index_meter.rs
--rw-r--r--   0      501       20      258 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/mod.rs
--rw-r--r--   0      501       20      943 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/api.rs
--rw-r--r--   0      501       20      919 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/consumer.rs
--rw-r--r--   0      501       20      434 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/metrics.rs
--rw-r--r--   0      501       20      116 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/mod.rs
--rw-r--r--   0      501       20     4268 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/server.rs
--rw-r--r--   0      501       20      991 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/store.rs
--rw-r--r--   0      501       20     3459 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/errors.rs
--rw-r--r--   0      501       20     1427 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/lib.rs
--rw-r--r--   0      501       20     3681 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/logging.rs
--rw-r--r--   0      501       20    15704 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/server.rs
--rw-r--r--   0      501       20     8110 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/api.rs
--rw-r--r--   0      501       20    40154 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/index.rs
--rw-r--r--   0      501       20     5174 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/metrics.rs
--rw-r--r--   0      501       20      287 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/mod.rs
--rw-r--r--   0      501       20     2108 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/utils/mod.rs
--rw-r--r--   0      501       20      923 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/utils/thread_handler.rs
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.4/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20   370551 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/dictionaries/drugs.csv
--rw-r--r--   0      501       20       92 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7233 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5492 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20    13820 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    31266 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13903 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    20309 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5962 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     6539 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      250 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20     1193 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
--rw-r--r--   0      501       20      693 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
--rw-r--r--   0      501       20     2092 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
--rw-r--r--   0      501       20    13740 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1899 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    67578 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     5812 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-r--r--   0      501       20     2498 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/utils.rs
--rw-r--r--   0      501       20     2216 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11998 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7462 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     4680 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8015 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5474 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      559 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.4/Cargo.toml
--rw-r--r--   0      501       20      685 2023-06-27 09:06:44.000000 summa_embed-0.17.4/.gitignore
--rw-r--r--   0      501       20      400 2023-06-27 09:06:44.000000 summa_embed-0.17.4/pyproject.toml
--rw-r--r--   0      501       20     2199 2023-06-27 09:06:44.000000 summa_embed-0.17.4/src/lib.rs
--rw-r--r--   0      501       20   102250 2023-06-27 09:08:59.000000 summa_embed-0.17.4/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.4/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.5/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2381 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10598 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7789 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.5/local_dependencies/summa-server/Cargo.toml
+-rw-r--r--   0      501       20       43 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/.cargo/config.toml
+-rw-r--r--   0      501       20     1050 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/LICENSE
+-rw-r--r--   0      501       20     2832 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/consumer.rs
+-rw-r--r--   0      501       20    13268 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/index.rs
+-rw-r--r--   0      501       20      105 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/mod.rs
+-rw-r--r--   0      501       20     2909 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/reflection.rs
+-rw-r--r--   0      501       20     1278 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/search.rs
+-rw-r--r--   0      501       20      783 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/bin/main.rs
+-rw-r--r--   0      501       20     5305 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumer_manager.rs
+-rw-r--r--   0      501       20      813 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
+-rw-r--r--   0      501       20     1082 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/dummy.rs
+-rw-r--r--   0      501       20    11633 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
+-rw-r--r--   0      501       20      270 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
+-rw-r--r--   0      501       20      532 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
+-rw-r--r--   0      501       20      155 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/mod.rs
+-rw-r--r--   0      501       20     3811 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/index_meter.rs
+-rw-r--r--   0      501       20      258 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/mod.rs
+-rw-r--r--   0      501       20      943 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/api.rs
+-rw-r--r--   0      501       20      919 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/consumer.rs
+-rw-r--r--   0      501       20      434 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/metrics.rs
+-rw-r--r--   0      501       20      116 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/mod.rs
+-rw-r--r--   0      501       20     4268 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/server.rs
+-rw-r--r--   0      501       20      991 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/store.rs
+-rw-r--r--   0      501       20     3459 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/errors.rs
+-rw-r--r--   0      501       20     1427 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/lib.rs
+-rw-r--r--   0      501       20     3681 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/logging.rs
+-rw-r--r--   0      501       20    15704 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/server.rs
+-rw-r--r--   0      501       20     8110 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/api.rs
+-rw-r--r--   0      501       20    40154 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/index.rs
+-rw-r--r--   0      501       20     5174 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/metrics.rs
+-rw-r--r--   0      501       20      287 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/mod.rs
+-rw-r--r--   0      501       20     2108 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/utils/mod.rs
+-rw-r--r--   0      501       20      923 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/utils/thread_handler.rs
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.5/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20   370551 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-r--r--   0      501       20       92 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7233 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5492 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20    13820 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    31266 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13903 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    20309 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5962 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     6539 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      250 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20     1193 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-r--r--   0      501       20      693 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-r--r--   0      501       20     2092 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-r--r--   0      501       20    13740 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1899 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    67578 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     5812 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     2498 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-r--r--   0      501       20     2216 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11998 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7462 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     4680 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8015 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      559 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.5/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-06-27 09:46:43.000000 summa_embed-0.17.5/.gitignore
+-rw-r--r--   0      501       20      400 2023-06-27 09:46:43.000000 summa_embed-0.17.5/pyproject.toml
+-rw-r--r--   0      501       20     2199 2023-06-27 09:46:43.000000 summa_embed-0.17.5/src/lib.rs
+-rw-r--r--   0      501       20   102250 2023-06-27 09:47:05.000000 summa_embed-0.17.5/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.5/PKG-INFO
```

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.5/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.5/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.5/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.5/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.5/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.5/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.5/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.5/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.5/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/Cargo.toml` & `summa_embed-0.17.5/local_dependencies/summa-server/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "summa-server"
-version = "0.17.4"
+version = "0.17.5"
 license-file = "LICENSE"
 description = "Fast full-text search server"
 homepage = "https://github.com/izihawa/summa"
 repository = "https://github.com/izihawa/summa"
 keywords = ["async", "search", "server", "grpc"]
 
 [lib]
@@ -51,15 +51,15 @@
 rand = { version = "0.8", features = ["small_rng"] }
 rdkafka = { version = "0.29", optional = true }
 rlimit = "0.9"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_derive = "1.0"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
-summa-core = { version = "0.17.4", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.5", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { features = ["grpc"] , path = "../summa-proto" }
 take_mut = "0.2"
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tantivy-fst = "0.4.0"
 time = { version = "0.3", features = ["serde-well-known", "wasm-bindgen"] }
 thiserror = "1.0"
 tokio = { version = "1.25", default_features = false , features = ["full", "time"] }
```

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/LICENSE` & `summa_embed-0.17.5/local_dependencies/summa-server/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/consumer.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/index.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/reflection.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/reflection.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/search.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/search.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/bin/main.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/bin/main.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumer_manager.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumer_manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/dummy.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/dummy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/status.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/status.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/components/index_meter.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/components/index_meter.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/api.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/consumer.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/server.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/store.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/store.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/errors.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/lib.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/logging.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/logging.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/server.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/services/api.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/services/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/services/index.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/services/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/services/metrics.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/services/metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/utils/mod.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-server/src/utils/thread_handler.rs` & `summa_embed-0.17.5/local_dependencies/summa-server/src/utils/thread_handler.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.5/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.17.4"
+version = "0.17.5"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.5/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/dictionaries/drugs.csv` & `summa_embed-0.17.5/local_dependencies/summa-core/dictionaries/drugs.csv`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
                         match self.schema.find_field(resolved_field_name) {
                             Some((field, full_path)) => {
                                 for term in grouping.into_inner() {
                                     intermediate_results.push(self.parse_term(term, &field, full_path, statement_boost)?);
                                 }
                             }
                             None => {
-                                if self.query_parser_config.0.removed_fields.iter().any(|x| x == resolved_field_name) {
+                                if self.query_parser_config.0.removed_fields.iter().any(|x| x == field_name.as_str()) {
                                     return Ok(Box::new(EmptyQuery {}));
                                 }
                                 intermediate_results.push(self.default_field_queries(field_name, statement_boost)?);
                                 for term in grouping.into_inner() {
                                     intermediate_results.push(self.default_field_queries(term, statement_boost)?)
                                 }
                             }
@@ -631,15 +631,15 @@
                         }
                     }
                     Rule::term => {
                         let resolved_field_name = self.resolve_field_name(field_name.as_str());
                         match self.schema.find_field(resolved_field_name) {
                             Some((field, full_path)) => self.parse_term(grouping_or_term, &field, full_path, statement_boost),
                             None => {
-                                if self.query_parser_config.0.removed_fields.iter().any(|x| x == resolved_field_name) {
+                                if self.query_parser_config.0.removed_fields.iter().any(|x| x == field_name.as_str()) {
                                     Ok(Box::new(EmptyQuery {}) as Box<dyn Query>)
                                 } else {
                                     Ok(Box::new(BooleanQuery::new(vec![
                                         (Occur::Should, self.default_field_queries(field_name, statement_boost)?),
                                         (Occur::Should, self.default_field_queries(grouping_or_term, statement_boost)?),
                                     ])) as Box<dyn Query>)
                                 }
```

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/utils.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/utils.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/local_dependencies/summa-core/src/validators.rs` & `summa_embed-0.17.5/local_dependencies/summa-core/src/validators.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/Cargo.toml` & `summa_embed-0.17.5/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-embed-py"
-version = "0.17.4"
+version = "0.17.5"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
@@ -13,12 +13,12 @@
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.8"
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.17.4", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
-summa-server = { version = "0.17.4", path = "local_dependencies/summa-server", default_features = false }
+summa-core = { version = "0.17.5", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-server = { version = "0.17.5", path = "local_dependencies/summa-server", default_features = false }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.17.4/.gitignore` & `summa_embed-0.17.5/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/src/lib.rs` & `summa_embed-0.17.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.4/Cargo.lock` & `summa_embed-0.17.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2960,15 +2960,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.17.4"
+version = "0.17.5"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "chrono",
  "config",
@@ -3008,15 +3008,15 @@
  "time 0.3.22",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.17.4"
+version = "0.17.5"
 dependencies = [
  "async-broadcast",
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
@@ -3042,15 +3042,15 @@
  "tonic",
  "tonic-build",
  "tonic-reflection",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.17.4"
+version = "0.17.5"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3095,15 +3095,15 @@
  "tracing-appender",
  "tracing-futures",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "summa-wasm"
-version = "0.124.4"
+version = "0.125.0"
 dependencies = [
  "async-trait",
  "console_error_panic_hook",
  "futures",
  "getrandom",
  "instant",
  "js-sys",
```

