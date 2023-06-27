# Comparing `tmp/summa_embed-0.17.3.tar.gz` & `tmp/summa_embed-0.17.4.tar.gz`

## Comparing `summa_embed-0.17.3.tar` & `summa_embed-0.17.4.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.3/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20   370551 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/dictionaries/drugs.csv
--rw-r--r--   0      501       20       92 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7233 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5492 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20    13820 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    31266 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13903 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    20309 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5962 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     6539 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      250 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20     1193 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
--rw-r--r--   0      501       20      693 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
--rw-r--r--   0      501       20     2092 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
--rw-r--r--   0      501       20    13740 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1899 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    67734 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     5812 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-r--r--   0      501       20     2498 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/utils.rs
--rw-r--r--   0      501       20     2216 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11998 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7462 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     4680 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8015 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5474 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      559 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.3/local_dependencies/summa-server/Cargo.toml
--rw-r--r--   0      501       20       43 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/.cargo/config.toml
--rw-r--r--   0      501       20     1050 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/LICENSE
--rw-r--r--   0      501       20     2832 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/consumer.rs
--rw-r--r--   0      501       20    13268 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/index.rs
--rw-r--r--   0      501       20      105 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/mod.rs
--rw-r--r--   0      501       20     2909 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/reflection.rs
--rw-r--r--   0      501       20     1278 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/apis/search.rs
--rw-r--r--   0      501       20      783 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/bin/main.rs
--rw-r--r--   0      501       20     5305 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumer_manager.rs
--rw-r--r--   0      501       20      813 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
--rw-r--r--   0      501       20     1082 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/dummy.rs
--rw-r--r--   0      501       20    11633 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
--rw-r--r--   0      501       20      270 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
--rw-r--r--   0      501       20      532 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
--rw-r--r--   0      501       20      155 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/mod.rs
--rw-r--r--   0      501       20     3811 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/index_meter.rs
--rw-r--r--   0      501       20      258 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/components/mod.rs
--rw-r--r--   0      501       20      943 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/api.rs
--rw-r--r--   0      501       20      919 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/consumer.rs
--rw-r--r--   0      501       20      434 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/metrics.rs
--rw-r--r--   0      501       20      116 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/mod.rs
--rw-r--r--   0      501       20     3994 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/server.rs
--rw-r--r--   0      501       20      991 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/configs/store.rs
--rw-r--r--   0      501       20     3459 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/errors.rs
--rw-r--r--   0      501       20     1427 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/lib.rs
--rw-r--r--   0      501       20     3681 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/logging.rs
--rw-r--r--   0      501       20    15704 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/server.rs
--rw-r--r--   0      501       20     8110 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/api.rs
--rw-r--r--   0      501       20    40378 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/index.rs
--rw-r--r--   0      501       20     5174 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/metrics.rs
--rw-r--r--   0      501       20      287 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/services/mod.rs
--rw-r--r--   0      501       20     2108 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/utils/mod.rs
--rw-r--r--   0      501       20      923 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-server/src/utils/thread_handler.rs
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.3/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2381 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10641 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7871 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2523 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      394 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-06-26 09:16:47.000000 summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.3/Cargo.toml
--rw-r--r--   0      501       20      685 2023-06-26 09:16:47.000000 summa_embed-0.17.3/.gitignore
--rw-r--r--   0      501       20      400 2023-06-26 09:16:47.000000 summa_embed-0.17.3/pyproject.toml
--rw-r--r--   0      501       20     2199 2023-06-26 09:16:47.000000 summa_embed-0.17.3/src/lib.rs
--rw-r--r--   0      501       20   104388 2023-06-26 09:16:57.000000 summa_embed-0.17.3/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.3/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.4/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2381 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10598 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7789 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.4/local_dependencies/summa-server/Cargo.toml
+-rw-r--r--   0      501       20       43 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/.cargo/config.toml
+-rw-r--r--   0      501       20     1050 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/LICENSE
+-rw-r--r--   0      501       20     2832 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/consumer.rs
+-rw-r--r--   0      501       20    13268 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/index.rs
+-rw-r--r--   0      501       20      105 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/mod.rs
+-rw-r--r--   0      501       20     2909 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/reflection.rs
+-rw-r--r--   0      501       20     1278 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/apis/search.rs
+-rw-r--r--   0      501       20      783 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/bin/main.rs
+-rw-r--r--   0      501       20     5305 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumer_manager.rs
+-rw-r--r--   0      501       20      813 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
+-rw-r--r--   0      501       20     1082 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/dummy.rs
+-rw-r--r--   0      501       20    11633 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
+-rw-r--r--   0      501       20      270 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
+-rw-r--r--   0      501       20      532 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
+-rw-r--r--   0      501       20      155 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/mod.rs
+-rw-r--r--   0      501       20     3811 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/index_meter.rs
+-rw-r--r--   0      501       20      258 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/components/mod.rs
+-rw-r--r--   0      501       20      943 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/api.rs
+-rw-r--r--   0      501       20      919 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/consumer.rs
+-rw-r--r--   0      501       20      434 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/metrics.rs
+-rw-r--r--   0      501       20      116 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/mod.rs
+-rw-r--r--   0      501       20     4268 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/server.rs
+-rw-r--r--   0      501       20      991 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/configs/store.rs
+-rw-r--r--   0      501       20     3459 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/errors.rs
+-rw-r--r--   0      501       20     1427 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/lib.rs
+-rw-r--r--   0      501       20     3681 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/logging.rs
+-rw-r--r--   0      501       20    15704 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/server.rs
+-rw-r--r--   0      501       20     8110 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/api.rs
+-rw-r--r--   0      501       20    40154 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/index.rs
+-rw-r--r--   0      501       20     5174 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/metrics.rs
+-rw-r--r--   0      501       20      287 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/services/mod.rs
+-rw-r--r--   0      501       20     2108 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/utils/mod.rs
+-rw-r--r--   0      501       20      923 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-server/src/utils/thread_handler.rs
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.4/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20   370551 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-r--r--   0      501       20       92 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7233 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5492 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20    13820 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    31266 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13903 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    20309 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5962 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     6539 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      250 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20     1193 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-r--r--   0      501       20      693 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-r--r--   0      501       20     2092 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-r--r--   0      501       20    13740 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1899 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    67578 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     5812 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     2498 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-r--r--   0      501       20     2216 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11998 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7462 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     4680 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8015 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      559 2023-06-27 09:06:44.000000 summa_embed-0.17.4/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.4/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-06-27 09:06:44.000000 summa_embed-0.17.4/.gitignore
+-rw-r--r--   0      501       20      400 2023-06-27 09:06:44.000000 summa_embed-0.17.4/pyproject.toml
+-rw-r--r--   0      501       20     2199 2023-06-27 09:06:44.000000 summa_embed-0.17.4/src/lib.rs
+-rw-r--r--   0      501       20   102250 2023-06-27 09:08:59.000000 summa_embed-0.17.4/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.4/PKG-INFO
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.4/local_dependencies/summa-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.17.3"
+version = "0.17.4"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.4/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/dictionaries/drugs.csv` & `summa_embed-0.17.4/local_dependencies/summa-core/dictionaries/drugs.csv`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 2% similar despite different names*

```diff
@@ -602,51 +602,54 @@
                 let field_name = search_group.next().expect("grammar failure");
                 let grouping_or_term = search_group.next().expect("grammar failure");
                 match grouping_or_term.as_rule() {
                     Rule::grouping => {
                         let grouping = grouping_or_term.into_inner().next().expect("grammar failure");
                         let occur = self.parse_occur(&grouping);
                         let mut intermediate_results = vec![];
-                        match self.schema.find_field(self.resolve_field_name(field_name.as_str())) {
+                        let resolved_field_name = self.resolve_field_name(field_name.as_str());
+                        match self.schema.find_field(resolved_field_name) {
                             Some((field, full_path)) => {
                                 for term in grouping.into_inner() {
                                     intermediate_results.push(self.parse_term(term, &field, full_path, statement_boost)?);
                                 }
                             }
-                            None => match proto::MissingFieldPolicy::from_i32(self.query_parser_config.0.missing_field_policy) {
-                                Some(proto::MissingFieldPolicy::AsUsualTerms) => {
-                                    intermediate_results.push(self.default_field_queries(field_name, statement_boost)?);
-                                    for term in grouping.into_inner() {
-                                        intermediate_results.push(self.default_field_queries(term, statement_boost)?)
-                                    }
+                            None => {
+                                if self.query_parser_config.0.removed_fields.iter().any(|x| x == resolved_field_name) {
+                                    return Ok(Box::new(EmptyQuery {}));
+                                }
+                                intermediate_results.push(self.default_field_queries(field_name, statement_boost)?);
+                                for term in grouping.into_inner() {
+                                    intermediate_results.push(self.default_field_queries(term, statement_boost)?)
                                 }
-                                Some(proto::MissingFieldPolicy::Remove) => return Ok(Box::new(EmptyQuery {})),
-                                Some(proto::MissingFieldPolicy::Fail) => return Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
-                                _ => unreachable!(),
-                            },
+                            }
                         }
                         let group_query = Box::new(BooleanQuery::new(intermediate_results.into_iter().map(|q| (Occur::Should, q)).collect())) as Box<dyn Query>;
                         match occur {
                             Occur::Should => Ok(group_query),
                             Occur::Must => Ok(Box::new(BooleanQuery::new(vec![(Occur::Must, group_query)])) as Box<dyn Query>),
                             Occur::MustNot => Ok(Box::new(BooleanQuery::new(vec![(Occur::MustNot, group_query)])) as Box<dyn Query>),
                         }
                     }
-                    Rule::term => match self.schema.find_field(self.resolve_field_name(field_name.as_str())) {
-                        Some((field, full_path)) => self.parse_term(grouping_or_term, &field, full_path, statement_boost),
-                        None => match proto::MissingFieldPolicy::from_i32(self.query_parser_config.0.missing_field_policy) {
-                            Some(proto::MissingFieldPolicy::AsUsualTerms) => Ok(Box::new(BooleanQuery::new(vec![
-                                (Occur::Should, self.default_field_queries(field_name, statement_boost)?),
-                                (Occur::Should, self.default_field_queries(grouping_or_term, statement_boost)?),
-                            ])) as Box<dyn Query>),
-                            Some(proto::MissingFieldPolicy::Remove) => Ok(Box::new(EmptyQuery {}) as Box<dyn Query>),
-                            Some(proto::MissingFieldPolicy::Fail) => Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
-                            _ => unreachable!(),
-                        },
-                    },
+                    Rule::term => {
+                        let resolved_field_name = self.resolve_field_name(field_name.as_str());
+                        match self.schema.find_field(resolved_field_name) {
+                            Some((field, full_path)) => self.parse_term(grouping_or_term, &field, full_path, statement_boost),
+                            None => {
+                                if self.query_parser_config.0.removed_fields.iter().any(|x| x == resolved_field_name) {
+                                    Ok(Box::new(EmptyQuery {}) as Box<dyn Query>)
+                                } else {
+                                    Ok(Box::new(BooleanQuery::new(vec![
+                                        (Occur::Should, self.default_field_queries(field_name, statement_boost)?),
+                                        (Occur::Should, self.default_field_queries(grouping_or_term, statement_boost)?),
+                                    ])) as Box<dyn Query>)
+                                }
+                            }
+                        }
+                    }
                     _ => unreachable!(),
                 }
             }
             Rule::doi => {
                 let mut queries = vec![];
 
                 for term_field_mapper_name in ["doi", "doi_isbn"] {
@@ -1182,15 +1185,15 @@
             },
         );
         query_parser.query_parser_config.0.morphology_configs = morphology_configs;
         query_parser.query_parser_config.0.query_language = Some("en".to_string());
         let query = query_parser.parse_query("red1 search engine going");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"red1\"))), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"search\")), TermQuery(Term(field=0, type=Str, \"searches\"))], tie_breaker: 0.3 }), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.3 }), (Should, TermQuery(Term(field=0, type=Str, \"going\")))] })");
         let query = query_parser.parse_query("iso 34-1:2022");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"iso\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"1\")))] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"iso\")), TermQuery(Term(field=0, type=Str, \"isos\"))], tie_breaker: 0.3 }), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"1\")))] })");
     }
 
     #[test]
     pub fn test_ner() {
         let mut query_parser = create_query_parser();
         let mut morphology_configs = HashMap::new();
         morphology_configs.insert(
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/query_parser/utils.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/query_parser/utils.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-core/src/validators.rs` & `summa_embed-0.17.4/local_dependencies/summa-core/src/validators.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/Cargo.toml` & `summa_embed-0.17.4/local_dependencies/summa-server/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "summa-server"
-version = "0.17.3"
+version = "0.17.4"
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
-summa-core = { version = "0.17.3", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.4", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { features = ["grpc"] , path = "../summa-proto" }
 take_mut = "0.2"
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tantivy-fst = "0.4.0"
 time = { version = "0.3", features = ["serde-well-known", "wasm-bindgen"] }
 thiserror = "1.0"
 tokio = { version = "1.25", default_features = false , features = ["full", "time"] }
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/LICENSE` & `summa_embed-0.17.4/local_dependencies/summa-server/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/consumer.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/index.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/reflection.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/reflection.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/apis/search.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/apis/search.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/bin/main.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/bin/main.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumer_manager.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumer_manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/dummy.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/dummy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/components/consumers/kafka/status.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/components/consumers/kafka/status.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/components/index_meter.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/components/index_meter.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/api.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/consumer.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/server.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/server.rs`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,20 @@
             .data_path(data_path)
             .api(
                 crate::configs::api::ConfigBuilder::default()
                     .grpc_endpoint(format!("127.0.0.1:{}", acquire_free_port()))
                     .build()
                     .expect("cannot create api config"),
             )
+            .metrics(Some(
+                crate::configs::metrics::ConfigBuilder::default()
+                    .endpoint(format!("127.0.0.1:{}", acquire_free_port()))
+                    .build()
+                    .expect("cannot create metrics config"),
+            ))
             .build()
             .expect("cannot create server config")
     }
 
     pub fn create_test_server_config_holder(data_path: &Path) -> Arc<dyn ConfigProxy<Config>> {
         ConfigHolder::from_config(create_test_server_config(data_path))
     }
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/configs/store.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/configs/store.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/errors.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/lib.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/logging.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/logging.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/server.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/services/api.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/services/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/services/index.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/services/index.rs`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,14 @@
                     path: index_path.to_string_lossy().to_string(),
                 };
                 let index = IndexHolder::open_file_index(&file_engine_config).await?;
                 let index_engine_config = proto::IndexEngineConfig {
                     config: Some(proto::index_engine_config::Config::File(file_engine_config)),
                     merge_policy: attach_index_request.merge_policy,
                     query_parser_config: query_parser_config.clone(),
-                    field_triggers: Default::default(),
                 };
                 (index, index_engine_config)
             }
             Some(proto::attach_index_request::IndexEngine::Remote(proto::AttachRemoteEngineRequest {
                 config: Some(remote_engine_config),
             })) => {
                 let index = IndexHolder::open_remote_index::<HyperExternalRequest, DefaultExternalRequestGenerator<HyperExternalRequest>>(
@@ -240,15 +239,14 @@
                     true,
                 )
                 .await?;
                 let index_engine_config = proto::IndexEngineConfig {
                     config: Some(proto::index_engine_config::Config::Remote(remote_engine_config)),
                     merge_policy: attach_index_request.merge_policy,
                     query_parser_config: query_parser_config.clone(),
-                    field_triggers: Default::default(),
                 };
                 (index, index_engine_config)
             }
             _ => unimplemented!(),
         };
         let index_holder = self.insert_index(&attach_index_request.index_name, index, &index_engine_config).await?;
         index_holder
@@ -317,27 +315,25 @@
                 let index = IndexHolder::create_file_index(&index_path, index_builder).await?;
                 let index_engine_config = proto::IndexEngineConfig {
                     config: Some(proto::index_engine_config::Config::File(proto::FileEngineConfig {
                         path: index_path.to_string_lossy().to_string(),
                     })),
                     merge_policy: create_index_request.merge_policy,
                     query_parser_config,
-                    field_triggers: Default::default(),
                 };
                 (index, index_engine_config)
             }
             Some(proto::create_index_request::IndexEngine::Memory(proto::CreateMemoryEngineRequest {})) => {
                 let index = IndexHolder::create_memory_index(index_builder)?;
                 let index_engine_config = proto::IndexEngineConfig {
                     config: Some(proto::index_engine_config::Config::Memory(proto::MemoryEngineConfig {
                         schema: serde_yaml::to_string(&index.schema()).expect("cannot serialize"),
                     })),
                     merge_policy: create_index_request.merge_policy,
                     query_parser_config,
-                    field_triggers: Default::default(),
                 };
                 (index, index_engine_config)
             }
         };
         let index_holder = self.insert_index(&create_index_request.index_name, index, &index_engine_config).await?;
         index_holder.partial_warmup(false, &default_fields).await?;
         Ok(index_holder)
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/services/metrics.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/services/metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/utils/mod.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-server/src/utils/thread_handler.rs` & `summa_embed-0.17.4/local_dependencies/summa-server/src/utils/thread_handler.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.4/local_dependencies/summa-proto/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-proto"
-version = "0.28.2"
+version = "0.29.0"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa search server proto files"
 
 [lib]
 name = "summa_proto"
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.4/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.4/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.4/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.4/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.4/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,14 @@
     FileEngineConfig file = 1;
     MemoryEngineConfig memory = 2;
     RemoteEngineConfig remote = 3;
   }
   // Merge policy
   MergePolicy merge_policy = 10;
   QueryParserConfig query_parser_config = 11;
-  map<string, string> field_triggers = 12;
 }
 
 // Description containing `Index` metadata fields
 message IndexDescription {
   string index_name = 1;
   // All index aliases
   repeated string index_aliases = 2;
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.4/local_dependencies/summa-proto/proto/query.proto`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,19 @@
   float tie_breaker = 1;
 };
 message ExactMatchesPromoter {
   uint32 slop = 1;
   optional float boost = 2;
   repeated string fields = 3;
 }
+
 message NerMatchesPromoter {
   optional float boost = 1;
   repeated string fields = 2;
 }
-enum MissingFieldPolicy {
-  AsUsualTerms = 0;
-  Remove = 1;
-  Fail = 2;
-}
 
 message MorphologyConfig {
   optional float derive_tenses_coefficient = 1;
 }
 
 message QueryParserConfig {
   map<string, string> field_aliases = 1;
@@ -37,15 +33,15 @@
   uint32 term_limit = 4;
   repeated string default_fields = 5;
   oneof default_mode {
     MatchQueryBooleanShouldMode boolean_should_mode = 6;
     MatchQueryDisjuctionMaxMode disjuction_max_mode = 7;
   }
   ExactMatchesPromoter exact_matches_promoter = 8;
-  MissingFieldPolicy missing_field_policy = 9;
+  repeated string removed_fields = 9;
   map<string, MorphologyConfig> morphology_configs = 10;
   optional string query_language = 11;
   NerMatchesPromoter ner_matches_promoter = 12;
 }
 
 message SearchResponse {
   // Time spent inside of `search` handler
```

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.4/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.4/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.4/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/Cargo.toml` & `summa_embed-0.17.4/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-embed-py"
-version = "0.17.3"
+version = "0.17.4"
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
-summa-core = { version = "0.17.3", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
-summa-server = { version = "0.17.3", path = "local_dependencies/summa-server", default_features = false }
+summa-core = { version = "0.17.4", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-server = { version = "0.17.4", path = "local_dependencies/summa-server", default_features = false }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.17.3/.gitignore` & `summa_embed-0.17.4/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/src/lib.rs` & `summa_embed-0.17.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.3/Cargo.lock` & `summa_embed-0.17.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -134,36 +134,14 @@
 checksum = "7c48ccdbf6ca6b121e0f586cbc0e73ae440e56c67c30fa0873b4e110d9c26d2b"
 dependencies = [
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
-name = "async-stream"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
-dependencies = [
- "async-stream-impl",
- "futures-core",
- "pin-project-lite",
-]
-
-[[package]]
-name = "async-stream-impl"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.22",
-]
-
-[[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -252,17 +230,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6dbe3c979c178231552ecba20214a8272df4e09f232a87aef4320cf06539aded"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
 
 [[package]]
 name = "bitpacking"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8c7d2ac73c167c06af4a5f37e6e59d84148d57ccbe4480b76f0273eefea82d7"
 dependencies = [
@@ -747,17 +725,17 @@
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "examples"
 version = "0.0.0"
 dependencies = [
  "serde_json",
- "summa-proto 0.28.2",
+ "summa-proto",
  "tokio",
- "tonic 0.9.2",
+ "tonic",
 ]
 
 [[package]]
 name = "fail"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe5e43d0f78a42ad591453aedb1d7ae631ce7ee445c7643691055a9ed8d3b01c"
@@ -1027,17 +1005,17 @@
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -1162,17 +1140,17 @@
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
 [[package]]
 name = "hyper"
-version = "0.14.26"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -1294,15 +1272,15 @@
  "minicbor",
  "multihash 0.18.1",
  "prost",
  "rayon",
  "rust-unixfs",
  "serde_json",
  "sled",
- "summa-proto 0.26.0",
+ "summa-proto",
  "unsigned-varint",
 ]
 
 [[package]]
 name = "ipfs-hamt-directory-py"
 version = "0.1.1"
 dependencies = [
@@ -2982,15 +2960,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.17.3"
+version = "0.17.4"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "chrono",
  "config",
@@ -3017,78 +2995,62 @@
  "rustc-hash",
  "serde",
  "serde_bytes",
  "serde_cbor",
  "serde_json",
  "serde_yaml",
  "strfmt",
- "summa-proto 0.28.2",
+ "summa-proto",
  "take_mut",
  "tantivy",
  "tantivy-common",
  "tantivy-query-grammar",
  "thiserror",
  "time 0.3.22",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.17.3"
+version = "0.17.4"
 dependencies = [
  "async-broadcast",
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "pythonize",
  "serde_json",
  "summa-core",
- "summa-proto 0.28.2",
+ "summa-proto",
  "summa-server",
  "tantivy",
  "tokio",
 ]
 
 [[package]]
 name = "summa-proto"
-version = "0.26.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11800e4c382bb5e8b6756e4fcaeb37a966e75f9c9796912e5066799587d81d00"
-dependencies = [
- "prost",
- "prost-build",
- "prost-types",
- "protoc-bin-vendored",
- "serde",
- "tonic 0.8.3",
- "tonic-build 0.8.4",
- "tonic-reflection 0.6.0",
-]
-
-[[package]]
-name = "summa-proto"
-version = "0.28.2"
+version = "0.29.0"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
  "tokio",
- "tonic 0.9.2",
- "tonic-build 0.9.2",
- "tonic-reflection 0.9.2",
+ "tonic",
+ "tonic-build",
+ "tonic-reflection",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.17.3"
+version = "0.17.4"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3108,54 +3070,54 @@
  "rdkafka",
  "rlimit",
  "serde",
  "serde_derive",
  "serde_json",
  "serde_yaml",
  "summa-core",
- "summa-proto 0.28.2",
+ "summa-proto",
  "take_mut",
  "tantivy",
  "tantivy-fst",
  "tempdir",
  "thiserror",
  "tikv-jemallocator",
  "time 0.3.22",
  "tokio",
  "tokio-stream",
  "tokio-util",
- "tonic 0.9.2",
- "tonic-build 0.9.2",
- "tonic-reflection 0.9.2",
+ "tonic",
+ "tonic-build",
+ "tonic-reflection",
  "tonic-web",
  "tower",
  "tower-http",
  "tracing",
  "tracing-appender",
  "tracing-futures",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "summa-wasm"
-version = "0.124.0"
+version = "0.124.4"
 dependencies = [
  "async-trait",
  "console_error_panic_hook",
  "futures",
  "getrandom",
  "instant",
  "js-sys",
  "parking_lot 0.12.1",
  "prost",
  "serde",
  "serde-wasm-bindgen",
  "strfmt",
  "summa-core",
- "summa-proto 0.28.2",
+ "summa-proto",
  "tantivy",
  "thiserror",
  "tokio",
  "tracing",
  "tracing-wasm",
  "wasm-bindgen",
  "wasm-bindgen-futures",
@@ -3556,47 +3518,14 @@
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tonic"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f219fad3b929bef19b1f86fbc0358d35daed8f2cac972037ac0dc10bbb8d5fb"
-dependencies = [
- "async-stream",
- "async-trait",
- "axum",
- "base64 0.13.1",
- "bytes",
- "flate2",
- "futures-core",
- "futures-util",
- "h2",
- "http",
- "http-body",
- "hyper",
- "hyper-timeout",
- "percent-encoding",
- "pin-project",
- "prost",
- "prost-derive",
- "tokio",
- "tokio-stream",
- "tokio-util",
- "tower",
- "tower-layer",
- "tower-service",
- "tracing",
- "tracing-futures",
-]
-
-[[package]]
-name = "tonic"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3082666a3a6433f7f511c7192923fa1fe07c69332d3c6a2e6bb040b569199d5a"
 dependencies = [
  "async-trait",
  "axum",
  "base64 0.21.2",
@@ -3618,63 +3547,36 @@
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "tonic-build"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bf5e9b9c0f7e0a7c027dcfaba7b2c60816c7049171f679d99ee2ff65d0de8c4"
-dependencies = [
- "prettyplease",
- "proc-macro2",
- "prost-build",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "tonic-build"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6fdaae4c2c638bb70fe42803a26fbd6fc6ac8c72f5c59f67ecc2a2dcabf4b07"
 dependencies = [
  "prettyplease",
  "proc-macro2",
  "prost-build",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "tonic-reflection"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67494bad4dda4c9bffae901dfe14e2b2c0f760adb4706dc10beeb81799f7f7b2"
-dependencies = [
- "bytes",
- "prost",
- "prost-types",
- "tokio",
- "tokio-stream",
- "tonic 0.8.3",
-]
-
-[[package]]
-name = "tonic-reflection"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0543d7092032041fbeac1f2c84304537553421a11a623c2301b12ef0264862c7"
 dependencies = [
  "prost",
  "prost-types",
  "tokio",
  "tokio-stream",
- "tonic 0.9.2",
+ "tonic",
 ]
 
 [[package]]
 name = "tonic-web"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21b00ec4842256d1fe0a46176e2ef5bc357664c66e7d91aff5a7d43d83a65f47"
@@ -3682,15 +3584,15 @@
  "base64 0.21.2",
  "bytes",
  "futures-core",
  "http",
  "http-body",
  "hyper",
  "pin-project",
- "tonic 0.9.2",
+ "tonic",
  "tower-http",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
@@ -3715,15 +3617,15 @@
 
 [[package]]
 name = "tower-http"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8bd22a874a2d0b70452d5597b12c537331d49060824a95f49f108994f94aa4c"
 dependencies = [
- "bitflags 2.3.2",
+ "bitflags 2.3.3",
  "bytes",
  "futures-core",
  "futures-util",
  "http",
  "http-body",
  "http-range-header",
  "pin-project-lite",
@@ -3916,17 +3818,17 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.3.4"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
+checksum = "d023da39d1fde5a8a3fe1f3e01ca9632ada0a63e9797de55a879d6e2236277be"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "valuable"
```

