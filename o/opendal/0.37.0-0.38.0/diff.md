# Comparing `tmp/opendal-0.37.0.tar.gz` & `tmp/opendal-0.38.0.tar.gz`

## Comparing `opendal-0.37.0.tar` & `opendal-0.38.0.tar`

### file list

```diff
@@ -1,322 +1,340 @@
--rw-r--r--   0        0        0     6291 1970-01-01 00:00:00.000000 opendal-0.37.0/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    79781 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1114 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6804 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2792 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1827 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1290 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     6142 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10879 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     3172 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
--rw-r--r--   0     1001      123     2687 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
--rw-r--r--   0     1001      123     2576 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md
--rw-r--r--   0     1001      123     4658 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    26044 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6622 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    22150 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9829 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    17421 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    14214 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    52907 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13282 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    29688 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12370 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2250 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    13102 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    23050 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    38366 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    13680 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/timeout.rs
--rw-r--r--   0     1001      123    11978 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3644 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3570 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    18865 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123    10363 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1020 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1566 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     5407 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
--rw-r--r--   0     1001      123    10349 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
--rw-r--r--   0     1001      123     1067 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
--rw-r--r--   0     1001      123     1934 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     5973 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5282 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3415 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    11165 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2159 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123    22541 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/multipart.rs
--rw-r--r--   0     1001      123     2962 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11712 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1976 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     3018 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/append.rs
--rw-r--r--   0     1001      123     9434 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15408 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4150 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4579 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2097 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3516 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10670 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9158 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6894 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5206 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     3953 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    12115 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/ops.rs
--rw-r--r--   0     1001      123    11671 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6507 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123     4514 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/appender.rs
--rw-r--r--   0     1001      123    31443 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123     5544 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    16950 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     2304 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/docs.md
--rw-r--r--   0     1001      123     5870 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      927 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2054 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    14348 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123    10123 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     1960 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/docs.md
--rw-r--r--   0     1001      123     3519 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2711 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     5727 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/appender.rs
--rw-r--r--   0     1001      123    13653 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/backend.rs
--rw-r--r--   0     1001      123     9184 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/core.rs
--rw-r--r--   0     1001      123     1314 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/docs.md
--rw-r--r--   0     1001      123     3492 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/error.rs
--rw-r--r--   0     1001      123      910 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/mod.rs
--rw-r--r--   0     1001      123     5963 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/pager.rs
--rw-r--r--   0     1001      123     2032 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/cos/writer.rs
--rw-r--r--   0     1001      123     3972 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      186 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/dashmap/docs.md
--rw-r--r--   0     1001      123      859 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123     1409 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/fs/appender.rs
--rw-r--r--   0     1001      123    23158 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123      869 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/fs/docs.md
--rw-r--r--   0     1001      123     1424 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      898 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3092 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    15925 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123      737 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ftp/docs.md
--rw-r--r--   0     1001      123     1808 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4208 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     1900 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    21320 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    16245 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3512 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10592 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6315 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123     3361 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/backend.rs
--rw-r--r--   0     1001      123     4276 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/builder.rs
--rw-r--r--   0     1001      123     7046 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/core.rs
--rw-r--r--   0     1001      123     1743 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/error.rs
--rw-r--r--   0     1001      123      904 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/mod.rs
--rw-r--r--   0     1001      123     1956 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/writer.rs
--rw-r--r--   0     1001      123    20868 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2375 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    13212 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     2419 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/docs.md
--rw-r--r--   0     1001      123     1497 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2461 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    16276 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1875 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    15935 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123      867 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/docs.md
--rw-r--r--   0     1001      123     1871 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     9060 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123      186 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/docs.md
--rw-r--r--   0     1001      123     2790 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1753 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     5712 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9177 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4224 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      511 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/memory/docs.md
--rw-r--r--   0     1001      123      857 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     4157 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     8174 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123     4710 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/obs/appender.rs
--rw-r--r--   0     1001      123    15615 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     9401 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3492 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      910 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2032 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    12487 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/backend.rs
--rw-r--r--   0     1001      123     4177 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/builder.rs
--rw-r--r--   0     1001      123     1743 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/error.rs
--rw-r--r--   0     1001      123     9228 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs
--rw-r--r--   0     1001      123      926 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/mod.rs
--rw-r--r--   0     1001      123     4874 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/pager.rs
--rw-r--r--   0     1001      123     6228 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/writer.rs
--rw-r--r--   0     1001      123     4869 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/appender.rs
--rw-r--r--   0     1001      123    21977 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    25318 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     1842 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/docs.md
--rw-r--r--   0     1001      123     3407 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      910 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6651 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123     9662 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      856 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/redis/docs.md
--rw-r--r--   0     1001      123      855 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     4245 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123     1263 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/rocksdb/docs.md
--rw-r--r--   0     1001      123      859 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    36101 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     4183 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28669 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     7050 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/docs.md
--rw-r--r--   0     1001      123     4749 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7387 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7234 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123    16103 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sftp/backend.rs
--rw-r--r--   0     1001      123     1029 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sftp/docs.md
--rw-r--r--   0     1001      123     2587 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sftp/error.rs
--rw-r--r--   0     1001      123      899 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sftp/mod.rs
--rw-r--r--   0     1001      123     2420 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sftp/pager.rs
--rw-r--r--   0     1001      123     3641 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sftp/utils.rs
--rw-r--r--   0     1001      123     1760 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sftp/writer.rs
--rw-r--r--   0     1001      123     4846 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      642 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sled/docs.md
--rw-r--r--   0     1001      123      854 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123     9779 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/supabase/backend.rs
--rw-r--r--   0     1001      123     8021 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/supabase/core.rs
--rw-r--r--   0     1001      123     2761 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/supabase/error.rs
--rw-r--r--   0     1001      123      894 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/supabase/mod.rs
--rw-r--r--   0     1001      123     2357 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/supabase/writer.rs
--rw-r--r--   0     1001      123     4558 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
--rw-r--r--   0     1001      123     3636 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
--rw-r--r--   0     1001      123     1743 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
--rw-r--r--   0     1001      123      912 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
--rw-r--r--   0     1001      123     2030 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
--rw-r--r--   0     1001      123    39341 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29752 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     3761 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2025 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20966 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      990 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2560 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2041 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    16176 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     1864 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/docs.md
--rw-r--r--   0     1001      123     4085 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2452 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2051 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     8596 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/appender.rs
--rw-r--r--   0     1001      123     2649 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6870 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    12002 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     7417 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    16556 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1614 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    24401 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123    13497 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3073 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1153 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    49497 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123     2863 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/operator/operator_functions.rs
--rw-r--r--   0     1001      123    17237 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/operator/operator_futures.rs
--rw-r--r--   0     1001      123     9547 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     6741 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    10770 2023-06-06 09:17:40.000000 opendal-0.37.0/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 opendal-0.37.0/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-06-06 09:17:40.000000 opendal-0.37.0/.gitignore
--rw-r--r--   0     1001      123     2212 2023-06-06 09:17:40.000000 opendal-0.37.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123      982 2023-06-06 09:17:40.000000 opendal-0.37.0/README.md
--rw-r--r--   0     1001      123      765 2023-06-06 09:17:40.000000 opendal-0.37.0/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-06-06 09:17:40.000000 opendal-0.37.0/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-06-06 09:17:40.000000 opendal-0.37.0/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-06-06 09:17:40.000000 opendal-0.37.0/examples/object.ipynb
--rw-r--r--   0     1001      123     1660 2023-06-06 09:17:40.000000 opendal-0.37.0/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-06-06 09:17:40.000000 opendal-0.37.0/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-06-06 09:17:40.000000 opendal-0.37.0/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123      405 2023-06-06 09:17:40.000000 opendal-0.37.0/python/opendal/layers.pyi
--rw-r--r--   0     1001      123    11963 2023-06-06 09:17:40.000000 opendal-0.37.0/src/asyncio.rs
--rw-r--r--   0     1001      123     3074 2023-06-06 09:17:40.000000 opendal-0.37.0/src/layers.rs
--rw-r--r--   0     1001      123    12218 2023-06-06 09:17:40.000000 opendal-0.37.0/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-06-06 09:17:40.000000 opendal-0.37.0/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-06-06 09:17:40.000000 opendal-0.37.0/tests/steps/binding.py
--rw-r--r--   0     1001      123   132202 2023-06-06 09:17:40.000000 opendal-0.37.0/Cargo.lock
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 opendal-0.37.0/PKG-INFO
+-rw-r--r--   0        0        0     6825 1970-01-01 00:00:00.000000 opendal-0.38.0/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    89540 2023-06-27 15:43:19.000000 opendal-0.38.0/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1114 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6290 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5554 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2987 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1290 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123     1040 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10880 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     2687 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
+-rw-r--r--   0     1001      123     2576 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md
+-rw-r--r--   0     1001      123     4658 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    26469 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6622 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    32922 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9949 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17725 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    14214 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    53997 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13488 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    30012 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12657 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2376 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13222 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    23560 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    38577 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    11611 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/throttle.rs
+-rw-r--r--   0     1001      123    14179 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/timeout.rs
+-rw-r--r--   0     1001      123    12198 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3644 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3571 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    18865 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123    12928 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1020 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1566 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     5407 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
+-rw-r--r--   0     1001      123    12938 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
+-rw-r--r--   0     1001      123     1067 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     5928 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5735 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3415 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    11165 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2159 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123    35575 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/multipart.rs
+-rw-r--r--   0     1001      123     2962 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11712 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1976 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     3018 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/append.rs
+-rw-r--r--   0     1001      123     9434 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15408 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4150 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     2842 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_reader.rs
+-rw-r--r--   0     1001      123     1473 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_stream.rs
+-rw-r--r--   0     1001      123     1070 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/mod.rs
+-rw-r--r--   0     1001      123     4579 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2181 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10670 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     2132 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/stream.rs
+-rw-r--r--   0     1001      123     9158 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5739 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     3953 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    12115 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/ops.rs
+-rw-r--r--   0     1001      123    11671 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6507 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123     4514 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/appender.rs
+-rw-r--r--   0     1001      123    31973 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123     5544 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    16987 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     2304 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/docs.md
+-rw-r--r--   0     1001      123     5870 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      927 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2252 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    14348 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123    10123 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     1960 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/docs.md
+-rw-r--r--   0     1001      123     3519 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2909 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     4216 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cacache/backend.rs
+-rw-r--r--   0     1001      123      657 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cacache/docs.md
+-rw-r--r--   0     1001      123      860 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cacache/mod.rs
+-rw-r--r--   0     1001      123     5727 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/appender.rs
+-rw-r--r--   0     1001      123    13653 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/backend.rs
+-rw-r--r--   0     1001      123     9184 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/core.rs
+-rw-r--r--   0     1001      123     1314 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/docs.md
+-rw-r--r--   0     1001      123     3492 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/error.rs
+-rw-r--r--   0     1001      123      910 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/mod.rs
+-rw-r--r--   0     1001      123     5963 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/pager.rs
+-rw-r--r--   0     1001      123     2230 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/writer.rs
+-rw-r--r--   0     1001      123     3972 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      186 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/docs.md
+-rw-r--r--   0     1001      123      859 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123     2935 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/backend.rs
+-rw-r--r--   0     1001      123     4144 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/builder.rs
+-rw-r--r--   0     1001      123     4854 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/core.rs
+-rw-r--r--   0     1001      123     2573 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/error.rs
+-rw-r--r--   0     1001      123      906 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/mod.rs
+-rw-r--r--   0     1001      123     2160 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/writer.rs
+-rw-r--r--   0     1001      123     1409 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/appender.rs
+-rw-r--r--   0     1001      123    23158 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123      869 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/docs.md
+-rw-r--r--   0     1001      123     1424 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      898 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3290 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    15921 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123      737 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/docs.md
+-rw-r--r--   0     1001      123     1808 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4208 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     2098 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    23912 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    17063 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3512 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10592 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6513 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123     3361 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/backend.rs
+-rw-r--r--   0     1001      123     4276 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/builder.rs
+-rw-r--r--   0     1001      123     7046 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/core.rs
+-rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/error.rs
+-rw-r--r--   0     1001      123      904 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/mod.rs
+-rw-r--r--   0     1001      123     2154 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/writer.rs
+-rw-r--r--   0     1001      123    20868 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2573 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    13208 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     2419 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/docs.md
+-rw-r--r--   0     1001      123     1497 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2659 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    16276 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1875 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    15931 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123      867 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/docs.md
+-rw-r--r--   0     1001      123     1871 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     9056 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123      186 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/docs.md
+-rw-r--r--   0     1001      123     2790 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1951 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     5712 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9177 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4405 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      511 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memory/docs.md
+-rw-r--r--   0     1001      123      857 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     6599 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/mini_moka/backend.rs
+-rw-r--r--   0     1001      123      861 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/mini_moka/mod.rs
+-rw-r--r--   0     1001      123     4625 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     8174 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123     4710 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/appender.rs
+-rw-r--r--   0     1001      123    15624 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     9417 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3492 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      910 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2230 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    12480 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/backend.rs
+-rw-r--r--   0     1001      123     4177 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/error.rs
+-rw-r--r--   0     1001      123     9228 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs
+-rw-r--r--   0     1001      123      926 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/mod.rs
+-rw-r--r--   0     1001      123     4874 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/pager.rs
+-rw-r--r--   0     1001      123     6426 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/writer.rs
+-rw-r--r--   0     1001      123     4869 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/appender.rs
+-rw-r--r--   0     1001      123    21977 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    25318 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     1842 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/docs.md
+-rw-r--r--   0     1001      123     3407 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      910 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6849 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123     6613 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redb/backend.rs
+-rw-r--r--   0     1001      123      677 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redb/docs.md
+-rw-r--r--   0     1001      123      854 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redb/mod.rs
+-rw-r--r--   0     1001      123     9658 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      856 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redis/docs.md
+-rw-r--r--   0     1001      123      855 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     4241 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123     1263 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/docs.md
+-rw-r--r--   0     1001      123      859 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    36080 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     4183 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28667 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     7050 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/docs.md
+-rw-r--r--   0     1001      123     4805 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7387 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7720 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123    16132 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/backend.rs
+-rw-r--r--   0     1001      123     1076 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/docs.md
+-rw-r--r--   0     1001      123     2587 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/error.rs
+-rw-r--r--   0     1001      123      899 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/mod.rs
+-rw-r--r--   0     1001      123     2420 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/pager.rs
+-rw-r--r--   0     1001      123     3641 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/utils.rs
+-rw-r--r--   0     1001      123     1958 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/writer.rs
+-rw-r--r--   0     1001      123     5813 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      642 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sled/docs.md
+-rw-r--r--   0     1001      123      854 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123     9779 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/backend.rs
+-rw-r--r--   0     1001      123     8021 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/core.rs
+-rw-r--r--   0     1001      123     2952 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/error.rs
+-rw-r--r--   0     1001      123      894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/mod.rs
+-rw-r--r--   0     1001      123     2555 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/writer.rs
+-rw-r--r--   0     1001      123     4551 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
+-rw-r--r--   0     1001      123     3636 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
+-rw-r--r--   0     1001      123      912 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
+-rw-r--r--   0     1001      123     2228 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
+-rw-r--r--   0     1001      123    39653 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29752 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     4779 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2223 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20966 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      990 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2560 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2239 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19002 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     1864 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/docs.md
+-rw-r--r--   0     1001      123     4224 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     7373 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     4859 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2249 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     8596 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/appender.rs
+-rw-r--r--   0     1001      123     2649 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6975 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12002 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     7417 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    16556 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1614 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    26806 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123    13888 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3073 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1153 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    49498 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123     2863 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_functions.rs
+-rw-r--r--   0     1001      123    17237 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_futures.rs
+-rw-r--r--   0     1001      123     9547 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     7375 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    13822 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 opendal-0.38.0/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-06-27 15:43:20.000000 opendal-0.38.0/.gitignore
+-rw-r--r--   0     1001      123     2213 2023-06-27 15:43:20.000000 opendal-0.38.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1084 2023-06-27 15:43:20.000000 opendal-0.38.0/README.md
+-rw-r--r--   0     1001      123      765 2023-06-27 15:43:20.000000 opendal-0.38.0/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-06-27 15:43:20.000000 opendal-0.38.0/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-06-27 15:43:20.000000 opendal-0.38.0/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-06-27 15:43:20.000000 opendal-0.38.0/examples/object.ipynb
+-rw-r--r--   0     1001      123     1660 2023-06-27 15:43:20.000000 opendal-0.38.0/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-06-27 15:43:20.000000 opendal-0.38.0/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-06-27 15:43:20.000000 opendal-0.38.0/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123      405 2023-06-27 15:43:20.000000 opendal-0.38.0/python/opendal/layers.pyi
+-rw-r--r--   0     1001      123    11963 2023-06-27 15:43:20.000000 opendal-0.38.0/src/asyncio.rs
+-rw-r--r--   0     1001      123     3074 2023-06-27 15:43:20.000000 opendal-0.38.0/src/layers.rs
+-rw-r--r--   0     1001      123    12218 2023-06-27 15:43:20.000000 opendal-0.38.0/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-06-27 15:43:20.000000 opendal-0.38.0/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-06-27 15:43:20.000000 opendal-0.38.0/tests/steps/binding.py
+-rw-r--r--   0     1001      123   138739 2023-06-27 15:43:19.000000 opendal-0.38.0/Cargo.lock
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 opendal-0.38.0/PKG-INFO
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/Cargo.toml` & `opendal-0.38.0/local_dependencies/opendal/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.37.0"
+version= "0.38.0"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -71,14 +71,15 @@
 # Enable all layers.
 layers-all = [
   "layers-chaos",
   "layers-metrics",
   "layers-prometheus",
   "layers-tracing",
   "layers-minitrace",
+  "layers-throttle",
 ]
 # Enable layers chaos support
 layers-chaos = ["dep:rand"]
 # Enable layers metrics support
 layers-metrics = ["dep:metrics"]
 # Enable layers prometheus support
 layers-prometheus = ["dep:prometheus"]
@@ -86,32 +87,36 @@
 layers-madsim = ["dep:madsim"]
 # Enable layers minitrace support.
 layers-minitrace = ["dep:minitrace"]
 # Enable layers tracing support.
 layers-tracing = ["dep:tracing"]
 # Enable layers oteltrace support.
 layers-otel-trace = ["dep:opentelemetry"]
+# Enable layers throttle support.
+layers-throttle = ["dep:governor"]
 
 services-azblob = [
   "dep:sha2",
   "dep:reqsign",
   "reqsign?/services-azblob",
   "reqsign?/reqwest_request",
 ]
 services-azdfs = [
   "dep:reqsign",
   "reqsign?/services-azblob",
   "reqsign?/reqwest_request",
 ]
+services-cacache = ["dep:cacache"]
 services-cos = [
   "dep:reqsign",
   "reqsign?/services-tencent",
   "reqsign?/reqwest_request",
 ]
 services-dashmap = ["dep:dashmap"]
+services-dropbox = []
 services-fs = ["tokio/fs"]
 services-ftp = ["dep:suppaftp", "dep:lazy-regex", "dep:bb8", "dep:async-tls"]
 services-gcs = [
   "dep:reqsign",
   "reqsign?/services-google",
   "reqsign?/reqwest_request",
 ]
@@ -119,14 +124,15 @@
 services-ghac = []
 services-hdfs = ["dep:hdrs"]
 services-http = []
 services-ipfs = ["dep:prost"]
 services-ipmfs = []
 services-memcached = ["dep:bb8"]
 services-memory = []
+services-mini-moka = ["dep:mini-moka"]
 services-moka = ["dep:moka"]
 services-obs = [
   "dep:reqsign",
   "reqsign?/services-huaweicloud",
   "reqsign?/reqwest_request",
 ]
 services-onedrive = []
@@ -149,45 +155,53 @@
 services-wasabi = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-webdav = []
 services-webhdfs = []
+services-redb = ["dep:redb"]
 
 [lib]
 bench = false
 
 [[bench]]
 harness = false
 name = "ops"
 
+[[test]]
+harness = false
+name = "behavior"
+
 [dependencies]
 anyhow = { version = "1.0.30", features = ["std"] }
 async-compat = "0.2"
 async-tls = { version = "0.11", optional = true }
 async-trait = "0.1.68"
 backon = "0.4.0"
 base64 = "0.21"
 bb8 = { version = "0.8", optional = true }
 bytes = "1.2"
+cacache =  { version = "11.6", default-features = false, features = ["tokio-runtime", "mmap"], optional = true }
 chrono = "0.4.24"
 dashmap = { version = "5.4", optional = true }
 dirs = { version = "5.0.1", optional = true }
 flagset = "0.4"
-futures = { version = "0.3", default-features = false, features = ["alloc"] }
+futures = { version = "0.3", default-features = false, features = ["std"] }
+governor = { version = "0.5", optional = true, features = ["std"] }
 hdrs = { version = "0.2", optional = true, features = ["async_file"] }
 http = "0.2.5"
 hyper = "0.14"
 lazy-regex = { version = "2.5.0", optional = true }
 log = "0.4"
 madsim = { version = "0.2.21", optional = true }
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
 minitrace = { version = "0.4.0", optional = true }
+mini-moka = { version = "0.10", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
 openssh = { version = "0.9.9", optional = true }
 openssh-sftp-client = { version = "0.13.5", optional = true, features = [
   "openssh",
   "tracing",
 ] }
@@ -208,14 +222,15 @@
   "stream",
 ], default-features = false }
 rocksdb = { version = "0.21.0", default-features = false, optional = true }
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
 sha2 = { version = "0.10", optional = true }
 sled = { version = "0.34.7", optional = true }
+redb = { version = "1.0.0", optional = true }
 suppaftp = { version = "4.5", default-features = false, features = [
   "async-secure",
   "async-rustls",
 ], optional = true }
 tokio = "1.27"
 tracing = { version = "0.1", optional = true }
 uuid = { version = "1", features = ["serde", "v4"] }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.38.0/local_dependencies/opendal/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,104 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.38.0] - 2023-06-27
+
+### Added
+* feat(raw/http_util): Implement mixed multipart parser by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2430
+* feat(services/gcs): Add batch delete support by @wcy-fdu in https://github.com/apache/incubator-opendal/pull/2142
+* feat(core): Add Write::sink API by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2440
+* feat(services/s3): Allow retry for unexpected 499 error by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2453
+* feat(layer): add throttle layer by @morristai in https://github.com/apache/incubator-opendal/pull/2444
+* feat(bindings/haskell): init haskell binding by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2463
+* feat(core): add capability check by @unixzii in https://github.com/apache/incubator-opendal/pull/2461
+* feat(bindings/haskell): add CONTRIBUTING.md by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2466
+* feat(bindings/haskell): add CI test for haskell binding by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2468
+* feat(binding/lua): introduce opendal lua binding by @oowl in https://github.com/apache/incubator-opendal/pull/2469
+* feat(bindings/swift): add Swift binding by @unixzii in https://github.com/apache/incubator-opendal/pull/2470
+* feat(bindings/haskell): support `is_exist` `create_dir` `copy` `rename` `delete` by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2475
+* feat(bindings/haskell): add `Monad` wrapper by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2482
+* feat(bindings/dotnet): basic structure by @tisonkun in https://github.com/apache/incubator-opendal/pull/2485
+* feat(services/dropbox): Support create/read/delete for Dropbox by @Zheaoli in https://github.com/apache/incubator-opendal/pull/2264
+* feat(bindings/java): support load system lib by @tisonkun in https://github.com/apache/incubator-opendal/pull/2502
+* feat(blocking operator): add remove_all api by @infdahai in https://github.com/apache/incubator-opendal/pull/2449
+* feat(core): adopt WebHDFS LISTSTATUS_BATCH for better performance by @morristai in https://github.com/apache/incubator-opendal/pull/2499
+* feat(bindings/haskell): support stat by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2504
+* feat(adapters-kv): add rename and copy support to kv adapters by @oowl in https://github.com/apache/incubator-opendal/pull/2513
+* feat: Implement sink for services s3 by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2508
+* feat(adapters-kv): add rename and copy support to non typed kv adapters by @oowl in https://github.com/apache/incubator-opendal/pull/2515
+* feat: Implement test harness via libtest-mimic instead by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2517
+* feat(service/sled): introduce tree support by @oowl in https://github.com/apache/incubator-opendal/pull/2516
+* feat(bindings/haskell): support list and scan by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2527
+* feat(services/redb): support redb service by @oowl in https://github.com/apache/incubator-opendal/pull/2526
+* feat(core): implement service for Mini Moka by @morristai in https://github.com/apache/incubator-opendal/pull/2537
+* feat(core): add Mini Moka GitHub Action workflow job by @morristai in https://github.com/apache/incubator-opendal/pull/2539
+* feat(services): add cacache backend by @PsiACE in https://github.com/apache/incubator-opendal/pull/2548
+* feat: Implement Writer::copy so user can copy from AsyncRead by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2552
+### Changed
+* refactor(bindings/C): refactor c bindings to call all APIs using pointer by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2489
+### Fixed
+* fix(services/azblob): Fix azblob batch max operations by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2434
+* fix(services/sftp): change default root config to remote server setting by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2431
+* fix: Enable `std` feature for futures to allow `futures::AsyncRead` by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2450
+* fix(services/gcs): GCS should support create dir by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2467
+* fix(bindings/C): use copy_from_slice instead of from_static in opendal_bytes by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2473
+* fix(bindings/swift): reorg the package to correct its name by @unixzii in https://github.com/apache/incubator-opendal/pull/2479
+* fix: Fix the build for zig binding by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2493
+* fix(service/webhdfs): fix webhdfs config builder for disable_list_batch by @morristai in https://github.com/apache/incubator-opendal/pull/2509
+* fix(core/types): add missing `vercel artifacts` for `FromStr` by @cijiugechu in https://github.com/apache/incubator-opendal/pull/2519
+* fix(types/operator): fix operation limit error default size by @oowl in https://github.com/apache/incubator-opendal/pull/2536
+### Docs
+* docs: Replace `create` with `new` by @NiwakaDev in https://github.com/apache/incubator-opendal/pull/2427
+* docs(services/redis): fix redis via config example by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2443
+* docs: add rust usage example by @Young-Flash in https://github.com/apache/incubator-opendal/pull/2447
+* docs: Polish rust examples by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2456
+* docs: polish docs and fix typos by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2458
+* docs: fix a typo on the landing page by @unixzii in https://github.com/apache/incubator-opendal/pull/2460
+* docs(examples/rust): Add 01-init-operator by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2464
+* docs: update readme.md to match the output by @rrain7 in https://github.com/apache/incubator-opendal/pull/2486
+* docs: Update components for Libraries and Services by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2487
+* docs: Add OctoBase into our users list by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2506
+* docs: Fix scan not checked for sled services by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2507
+* doc(binding/lua): Improve readme doc for contribute and usage by @oowl in https://github.com/apache/incubator-opendal/pull/2511
+* doc(services/redb): add doc for redb service backend by @oowl in https://github.com/apache/incubator-opendal/pull/2538
+* doc(bindings/swift): add CONTRIBUTING.md by @unixzii in https://github.com/apache/incubator-opendal/pull/2540
+* docs: Add new rust example 02-async-io by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2541
+* docs: Fix link for CONTRIBUTING.md  by @HuSharp in https://github.com/apache/incubator-opendal/pull/2544
+* doc: polish release doc by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2531
+* docs: Move verify to upper folder by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2546
+* doc(binding/lua): add ldoc generactor for lua binding by @oowl in https://github.com/apache/incubator-opendal/pull/2549
+* docs: Add new architectural image for OpenDAL by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2553
+* docs: Polish README for core and bindings by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2554
+### CI
+* ci: Fix append test should use copy_buf to avoid call times by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2436
+* build(bindings/ruby): fix compile rb-sys on Apple M1 by @tisonkun in https://github.com/apache/incubator-opendal/pull/2451
+* ci: Use summary for zig test to fix build by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2480
+* ci(workflow): add lua binding test workflow by @oowl in https://github.com/apache/incubator-opendal/pull/2478
+* build(deps): bump actions/setup-python from 3 to 4 by @dependabot in https://github.com/apache/incubator-opendal/pull/2481
+* ci(bindings/swift): add CI for Swift binding by @unixzii in https://github.com/apache/incubator-opendal/pull/2492
+* ci: Try to make webhdfs tests more stable by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2503
+* ci(bindings/java): auto release snapshot  by @tisonkun in https://github.com/apache/incubator-opendal/pull/2521
+* ci: Disable the stage snapshot CI by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2528
+* ci: fix opendal-java snapshot releases by @tisonkun in https://github.com/apache/incubator-opendal/pull/2532
+* ci: Fix typo in binding java CI by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2534
+* ci(bindings/swift): optimize time consumption of CI pipeline by @unixzii in https://github.com/apache/incubator-opendal/pull/2545
+* ci: Fix PR label not updated while edited by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2547
+### Chore
+* chore: Add redis bench support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2438
+* chore(bindings/nodejs): update index.d.ts by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2459
+* chore: Add release 0.37.0 to download by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2472
+* chore: Fix Cargo.lock not updated by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2490
+* chore: Polish some code details by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2505
+* chore(bindings/nodejs): provide more precise type for scheme by @cijiugechu in https://github.com/apache/incubator-opendal/pull/2520
+
 ## [v0.37.0] - 2023-06-06
 
 ### Added
 * feat(services/webdav): support redirection when get 302/307 response during read operation by @Yansongsongsong in https://github.com/apache/incubator-opendal/pull/2256
 * feat: Add Zig Bindings Module by @kassane in https://github.com/apache/incubator-opendal/pull/2374
 * feat: Implement Timeout Layer by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2395
 * feat(bindings/c): add  opendal_operator_blocking_delete method by @jiaoew1991 in https://github.com/apache/incubator-opendal/pull/2416
@@ -2276,14 +2366,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.38.0]: https://github.com/apache/incubator-opendal/compare/v0.37.0...v0.38.0
 [v0.37.0]: https://github.com/apache/incubator-opendal/compare/v0.36.0...v0.37.0
 [v0.36.0]: https://github.com/apache/incubator-opendal/compare/v0.35.0...v0.36.0
 [v0.35.0]: https://github.com/apache/incubator-opendal/compare/v0.34.0...v0.35.0
 [v0.34.0]: https://github.com/apache/incubator-opendal/compare/v0.33.3...v0.34.0
 [v0.33.3]: https://github.com/apache/incubator-opendal/compare/v0.33.2...v0.33.3
 [v0.33.2]: https://github.com/apache/incubator-opendal/compare/v0.33.1...v0.33.2
 [v0.33.1]: https://github.com/apache/incubator-opendal/compare/v0.33.0...v0.33.1
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.38.0/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.38.0/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.38.0/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.38.0/local_dependencies/opendal/benches/ops/read.rs`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                     .range_reader(path, 0..=size.bytes() as u64)
                     .await
                     .unwrap();
                 io::copy(r, &mut io::sink()).await.unwrap();
             })
         });
 
-        std::mem::drop(temp_data);
+        drop(temp_data);
     }
 
     group.finish()
 }
 
 /// Read from 1/4 to 3/4 and than drop the reader without consuming all data;
 fn bench_read_part(c: &mut Criterion, name: &str, op: Operator) {
@@ -145,12 +145,12 @@
                             .collect::<Vec<_>>();
                         futures::future::join_all(futures).await
                     })
                 },
             );
         }
 
-        std::mem::drop(temp_data);
+        drop(temp_data);
     }
 
     group.finish()
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.38.0/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,20 @@
 pub fn services() -> Vec<(&'static str, Option<Operator>)> {
     let _ = dotenvy::dotenv();
 
     vec![
         ("fs", service::<services::Fs>()),
         ("s3", service::<services::S3>()),
         ("memory", service::<services::Memory>()),
+        #[cfg(feature = "services-mini-moka")]
+        ("mini-moka", service::<services::MiniMoka>()),
         #[cfg(feature = "services-moka")]
         ("moka", service::<services::Moka>()),
+        #[cfg(feature = "services-redis")]
+        ("redis", service::<services::Redis>()),
     ]
 }
 
 pub fn gen_bytes(rng: &mut ThreadRng, size: usize) -> Bytes {
     let mut content = vec![0; size];
     rng.fill_bytes(&mut content);
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.38.0/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.38.0/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/features.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/features.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ## Service Features
 
 - `services-dashmap`: Enable dashmap service support.
 - `services-ftp`: Enable ftp service support.
 - `services-hdfs`: Enable hdfs service support.
 - `services-memcached`: Enable memcached service support.
+- `services-mini-moka`: Enable mini-moka service support.
 - `services-moka`: Enable moka service support.
 - `services-ipfs`: Enable ipfs service support.
 - `services-redis`: Enable redis service support.
 - `services-rocksdb`: Enable rocksdb service support.
 - `services-sled`: Enable sled service support.
 
 ## Dependencies Features
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.38.0/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 //! use its formal name.
 //!
 //! For example, we will use `s3` for AWS S3 Compatible Storage Service
 //! instead of `aws` or `awss3`. This is because there are many storage
 //! vendors that provide s3-like RESTful APIs, and our s3 service is
 //! implemented to support all of them, not just AWS S3.
 //!
-//! Obviously, we can use `duck` as scheme, let's add a new variant in [`Scheme`], and implement all reqired functions like `Scheme::from_str` and `Scheme::into_static`:
+//! Obviously, we can use `duck` as scheme, let's add a new variant in [`Scheme`], and implement all required functions like `Scheme::from_str` and `Scheme::into_static`:
 //!
 //! ```ignore
 //! pub enum Scheme {
 //!     Duck,
 //! }
 //! ```
 //!
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.38.0/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# Upgrade to v0.38
+
+There are no public API changes.
+
+## Raw API
+
+OpenDAL add the `Write::sink` API to enable streaming writing. This is a breaking change for users who depend on the raw API.
+
+For a quick fix, users who have implemented `opendal::raw::oio::Write` can return an `Unsupported` error for `Write::sink()`. 
+
+More detailes could be found at [RFC: Writer `sink` API][crate::docs::rfcs::rfc_2083_writer_sink_api].
+
 # Upgrade to v0.37
 
 In v0.37.0, OpenDAL bump the version of `reqsign` to v0.13.0.
 
 There are no public API and raw API changes.
 
 # Upgrade to v0.36
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,18 @@
         self.inner.write(bs).await
     }
 
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner.sink(size, s).await
+    }
+
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await
     }
 }
 
 impl<R: oio::BlockingWrite> oio::BlockingWrite for ConcurrentLimitWrapper<R> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,22 @@
         self.inner.abort().await.map_err(|err| {
             err.with_operation(WriteOperation::Abort)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner.sink(size, s).await.map_err(|err| {
+            err.with_operation(WriteOperation::Sink)
+                .with_context("service", self.scheme)
+                .with_context("path", &self.path)
+        })
+    }
+
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await.map_err(|err| {
             err.with_operation(WriteOperation::Close)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1339,14 +1339,46 @@
                     )
                 }
                 Err(err)
             }
         }
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        match self.inner.sink(size, s).await {
+            Ok(_) => {
+                self.written += size;
+                trace!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} path={} written={} -> data sink {}B",
+                    self.scheme,
+                    WriteOperation::Sink,
+                    self.path,
+                    self.written,
+                    size
+                );
+                Ok(())
+            }
+            Err(err) => {
+                if let Some(lvl) = self.failure_level {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} path={} written={} -> data sink failed: {err:?}",
+                        self.scheme,
+                        WriteOperation::Sink,
+                        self.path,
+                        self.written,
+                    )
+                }
+                Err(err)
+            }
+        }
+    }
+
     async fn abort(&mut self) -> Result<()> {
         match self.inner.abort().await {
             Ok(_) => {
                 trace!(
                     target: LOGGING_TARGET,
                     "service={} operation={} path={} written={} -> abort writer",
                     self.scheme,
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,21 @@
         }
         #[cfg(not(madsim))]
         {
             unreachable!("madsim is not enabled")
         }
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> crate::Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "will be supported in the future",
+        ))
+    }
+
     async fn abort(&mut self) -> crate::Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "will be supported in the future",
         ))
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files 1% similar despite different names*

```diff
@@ -860,14 +860,25 @@
             .map(|_| self.bytes += size as u64)
             .map_err(|err| {
                 self.handle.increment_errors_total(self.op, err.kind());
                 err
             })
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner
+            .sink(size, s)
+            .await
+            .map(|_| self.bytes += size)
+            .map_err(|err| {
+                self.handle.increment_errors_total(self.op, err.kind());
+                err
+            })
+    }
+
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await.map_err(|err| {
             self.handle.increment_errors_total(self.op, err.kind());
             err
         })
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,24 @@
             .in_span(Span::enter_with_parent(
                 WriteOperation::Write.into_static(),
                 &self.span,
             ))
             .await
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner
+            .sink(size, s)
+            .in_span(Span::enter_with_parent(
+                WriteOperation::Sink.into_static(),
+                &self.span,
+            ))
+            .await
+    }
+
     async fn abort(&mut self) -> Result<()> {
         self.inner
             .abort()
             .in_span(Span::enter_with_parent(
                 WriteOperation::Abort.into_static(),
                 &self.span,
             ))
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -72,9 +72,14 @@
 #[cfg(feature = "layers-madsim")]
 pub use self::madsim::MadsimLayer;
 #[cfg(feature = "layers-madsim")]
 pub use self::madsim::MadsimServer;
 
 #[cfg(feature = "layers-otel-trace")]
 mod oteltrace;
+
+#[cfg(feature = "layers-throttle")]
+mod throttle;
 #[cfg(feature = "layers-otel-trace")]
 pub use self::oteltrace::OtelTraceLayer;
+#[cfg(feature = "layers-throttle")]
+pub use self::throttle::ThrottleLayer;
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files 2% similar despite different names*

```diff
@@ -318,14 +318,18 @@
 
 #[async_trait]
 impl<R: oio::Write> oio::Write for OtelTraceWrapper<R> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.inner.write(bs).await
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner.sink(size, s).await
+    }
+
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await
     }
 
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files 1% similar despite different names*

```diff
@@ -680,14 +680,30 @@
             })
             .map_err(|err| {
                 self.stats.increment_errors_total(self.op, err.kind());
                 err
             })
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner
+            .sink(size, s)
+            .await
+            .map(|_| {
+                self.stats
+                    .bytes_total
+                    .with_label_values(&[&self.scheme, Operation::Write.into_static()])
+                    .observe(size as f64)
+            })
+            .map_err(|err| {
+                self.stats.increment_errors_total(self.op, err.kind());
+                err
+            })
+    }
+
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await.map_err(|err| {
             self.stats.increment_errors_total(self.op, err.kind());
             err
         })
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 0% similar despite different names*

```diff
@@ -644,14 +644,19 @@
                         continue;
                     }
                 },
             }
         }
     }
 
+    /// Sink will move the input stream, so we can't retry it.
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner.sink(size, s).await
+    }
+
     async fn abort(&mut self) -> Result<()> {
         let mut backoff = self.builder.build();
 
         loop {
             match self.inner.abort().await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
@@ -856,14 +861,15 @@
         type Appender = ();
         type Pager = MockPager;
         type BlockingPager = ();
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
             am.set_capability(Capability {
+                read: true,
                 list: true,
                 list_with_delimiter_slash: true,
                 list_without_delimiter: true,
                 batch: true,
                 ..Default::default()
             });
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/timeout.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/timeout.rs`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,27 @@
                 Error::new(ErrorKind::Unexpected, "operation timeout")
                     .with_operation(WriteOperation::Write)
                     .with_context("timeout", timeout.as_secs_f64().to_string())
                     .set_temporary()
             })?
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        let timeout = self.io_timeout(size);
+
+        tokio::time::timeout(timeout, self.inner.sink(size, s))
+            .await
+            .map_err(|_| {
+                Error::new(ErrorKind::Unexpected, "operation timeout")
+                    .with_operation(WriteOperation::Sink)
+                    .with_context("timeout", timeout.as_secs_f64().to_string())
+                    .set_temporary()
+            })?
+    }
+
     async fn abort(&mut self) -> Result<()> {
         tokio::time::timeout(self.timeout, self.inner.abort())
             .await
             .map_err(|_| {
                 Error::new(ErrorKind::Unexpected, "operation timeout")
                     .with_operation(WriteOperation::Abort)
                     .with_context("timeout", self.timeout.as_secs_f64().to_string())
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,22 @@
         self.inner.write(bs).await
     }
 
     #[tracing::instrument(
         parent = &self.span,
         level = "trace",
         skip_all)]
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.inner.sink(size, s).await
+    }
+
+    #[tracing::instrument(
+        parent = &self.span,
+        level = "trace",
+        skip_all)]
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await
     }
 
     #[tracing::instrument(
         parent = &self.span,
         level = "trace",
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.38.0/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/lib.rs` & `opendal-0.38.0/local_dependencies/opendal/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 //! OpenDAL is the Open Data Access Layer to **freely** access data.
 //!
-//! - Documentation: All docs are carried byself, visit [`docs`] for more.
+//! - Documentation: All docs are carried by self, visit [`docs`] for more.
 //! - Services: All supported services could be found at [`services`].
 //! - Layers: All builtin layer could be found at [`layers`].
 //! - Features: All features could be found at [`features`][docs::features].
 //!
 //! # Quick Start
 //!
 //! ```no_run
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 15% similar despite different names*

```diff
@@ -79,14 +79,22 @@
         }
 
         if cap.write {
             cap.create_dir = true;
             cap.delete = true;
         }
 
+        if cap.read && cap.write {
+            cap.copy = true;
+        }
+
+        if cap.read && cap.write && cap.delete {
+            cap.rename = true;
+        }
+
         if cap.list {
             cap.list_without_delimiter = true;
         }
 
         am
     }
 
@@ -226,14 +234,76 @@
 
         let p = build_abs_path(&self.root, path);
         let res = self.kv.blocking_scan(&p)?;
         let pager = KvPager::new(&self.root, res);
 
         Ok((RpList::default(), pager))
     }
+
+    async fn rename(&self, from: &str, to: &str, _: OpRename) -> Result<RpRename> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.get(&from).await? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.set(&to, &bs).await?;
+
+        self.kv.delete(&from).await?;
+        Ok(RpRename::default())
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, _: OpRename) -> Result<RpRename> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.blocking_get(&from)? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.blocking_set(&to, &bs)?;
+
+        self.kv.blocking_delete(&from)?;
+        Ok(RpRename::default())
+    }
+
+    async fn copy(&self, from: &str, to: &str, _: OpCopy) -> Result<RpCopy> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.get(&from).await? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.set(&to, &bs).await?;
+
+        Ok(RpCopy::default())
+    }
+
+    fn blocking_copy(&self, from: &str, to: &str, _: OpCopy) -> Result<RpCopy> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.blocking_get(&from)? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.blocking_set(&to, &bs)?;
+
+        Ok(RpCopy::default())
+    }
 }
 
 impl<S> Backend<S>
 where
     S: Adapter,
 {
     fn apply_range(&self, mut bs: Vec<u8>, br: BytesRange) -> Vec<u8> {
@@ -321,14 +391,21 @@
     // TODO: we need to support append in the future.
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.buf = Some(bs.into());
 
         Ok(())
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs`

 * *Files 21% similar despite different names*

```diff
@@ -88,14 +88,24 @@
         }
 
         if kv_cap.scan {
             cap.list = true;
             cap.list_without_delimiter = true;
         }
 
+        if cap.read && cap.write {
+            cap.copy = true;
+        }
+
+        if cap.read && cap.write && cap.delete {
+            cap.rename = true;
+        }
+
+        cap.blocking = true;
+
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
         let p = build_abs_path(&self.root, path);
         self.kv.set(&p, Value::new_dir()).await?;
         Ok(RpCreateDir::default())
@@ -215,14 +225,74 @@
 
         let p = build_abs_path(&self.root, path);
         let res = self.kv.blocking_scan(&p)?;
         let pager = KvPager::new(&self.root, res);
 
         Ok((RpList::default(), pager))
     }
+
+    async fn rename(&self, from: &str, to: &str, _: OpRename) -> Result<RpRename> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.get(&from).await? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.set(&to, bs).await?;
+        self.kv.delete(&from).await?;
+        Ok(RpRename::default())
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, _: OpRename) -> Result<RpRename> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.blocking_get(&from)? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.blocking_set(&to, bs)?;
+        self.kv.blocking_delete(&from)?;
+        Ok(RpRename::default())
+    }
+
+    async fn copy(&self, from: &str, to: &str, _: OpCopy) -> Result<RpCopy> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.get(&from).await? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.set(&to, bs).await?;
+
+        Ok(RpCopy::default())
+    }
+
+    fn blocking_copy(&self, from: &str, to: &str, _: OpCopy) -> Result<RpCopy> {
+        let from = build_abs_path(&self.root, from);
+        let to = build_abs_path(&self.root, to);
+
+        let bs = match self.kv.blocking_get(&from)? {
+            // TODO: we can reuse the metadata in value to build content range.
+            Some(bs) => bs,
+            None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
+        };
+
+        self.kv.blocking_set(&to, bs)?;
+
+        Ok(RpCopy::default())
+    }
 }
 
 impl<S> Backend<S>
 where
     S: Adapter,
 {
     fn apply_range(&self, mut bs: Bytes, br: BytesRange) -> Bytes {
@@ -334,14 +404,21 @@
     // TODO: we need to support append in the future.
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.buf.push(bs);
 
         Ok(())
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         self.buf.clear();
 
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 use std::task::ready;
 use std::task::Context;
 use std::task::Poll;
 
 use bytes::Buf;
 use bytes::BufMut;
 use bytes::Bytes;
-use futures::Stream;
 use futures::StreamExt;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
@@ -37,40 +36,40 @@
 #[derive(Default)]
 pub enum AsyncBody {
     /// An empty body.
     #[default]
     Empty,
     /// Body with bytes.
     Bytes(Bytes),
+    /// Body with stream.
+    Stream(oio::Streamer),
 }
 
-type BytesStream = Box<dyn Stream<Item = Result<Bytes>> + Send + Sync + Unpin>;
-
 /// IncomingAsyncBody carries the content returned by remote servers.
 ///
 /// # Notes
 ///
 /// Client SHOULD NEVER construct this body.
 pub struct IncomingAsyncBody {
     /// # TODO
     ///
     /// hyper returns `impl Stream<Item = crate::Result<Bytes>>` but we can't
     /// write the types in stable. So we will box here.
     ///
     /// After [TAIT](https://rust-lang.github.io/rfcs/2515-type_alias_impl_trait.html)
     /// has been stable, we can change `IncomingAsyncBody` into `IncomingAsyncBody<S>`.
-    inner: BytesStream,
+    inner: oio::Streamer,
     size: Option<u64>,
     consumed: u64,
     chunk: Option<Bytes>,
 }
 
 impl IncomingAsyncBody {
     /// Construct a new incoming async body
-    pub fn new(s: BytesStream, size: Option<u64>) -> Self {
+    pub fn new(s: oio::Streamer, size: Option<u64>) -> Self {
         Self {
             inner: s,
             size,
             consumed: 0,
             chunk: None,
         }
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 use futures::TryStreamExt;
 use http::Request;
 use http::Response;
 
 use super::body::IncomingAsyncBody;
 use super::parse_content_length;
 use super::AsyncBody;
+use crate::raw::oio::into_stream;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
 /// HttpClient that used across opendal.
 #[derive(Clone)]
 pub struct HttpClient {
@@ -72,31 +73,34 @@
     /// Get the async client from http client.
     pub fn client(&self) -> reqwest::Client {
         self.client.clone()
     }
 
     /// Send a request in async way.
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
-        let url = req.uri().to_string();
+        // Uri stores all string alike data in `Bytes` which means
+        // the clone here is cheap.
+        let uri = req.uri().clone();
         let is_head = req.method() == http::Method::HEAD;
 
         let (parts, body) = req.into_parts();
 
         let mut req_builder = self
             .client
             .request(
                 parts.method,
-                reqwest::Url::from_str(&url).expect("input request url must be valid"),
+                reqwest::Url::from_str(&uri.to_string()).expect("input request url must be valid"),
             )
             .version(parts.version)
             .headers(parts.headers);
 
         req_builder = match body {
             AsyncBody::Empty => req_builder.body(reqwest::Body::from("")),
             AsyncBody::Bytes(bs) => req_builder.body(reqwest::Body::from(bs)),
+            AsyncBody::Stream(s) => req_builder.body(reqwest::Body::wrap_stream(s)),
         };
 
         let mut resp = req_builder.send().await.map_err(|err| {
             let is_temporary = !(
                 // Builder related error should not be retried.
                 err.is_builder() ||
                 // Error returned by RedirectPolicy.
@@ -107,15 +111,15 @@
                 //
                 // Status should be checked by our services.
                 err.is_status()
             );
 
             let mut oerr = Error::new(ErrorKind::Unexpected, "send async request")
                 .with_operation("http_util::Client::send_async")
-                .with_context("url", &url)
+                .with_context("url", uri.to_string())
                 .set_source(err);
             if is_temporary {
                 oerr = oerr.set_temporary();
             }
 
             oerr
         })?;
@@ -126,27 +130,33 @@
             None
         } else {
             parse_content_length(resp.headers()).expect("response content length must be valid")
         };
 
         let mut hr = Response::builder()
             .version(resp.version())
-            .status(resp.status());
+            .status(resp.status())
+            // Insert uri into response extension so that we can fetch
+            // it later.
+            .extension(uri.clone());
         // Swap headers directly instead of copy the entire map.
         mem::swap(hr.headers_mut().unwrap(), resp.headers_mut());
 
         let stream = resp.bytes_stream().map_err(move |err| {
             // If stream returns a body related error, we can convert
             // it to interrupt so we can retry it.
             Error::new(ErrorKind::Unexpected, "read data from http stream")
                 .map(|v| if err.is_body() { v.set_temporary() } else { v })
-                .with_context("url", &url)
+                .with_context("url", uri.to_string())
                 .set_source(err)
         });
 
-        let body = IncomingAsyncBody::new(Box::new(stream), content_length);
+        let body = IncomingAsyncBody::new(
+            Box::new(into_stream::from_futures_stream(stream)),
+            content_length,
+        );
 
         let resp = hr.body(body).expect("response must build succeed");
 
         Ok(resp)
     }
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         .set_source(err)
 }
 
 /// Create a new error happened during signing request.
 pub fn new_request_credential_error(err: anyhow::Error) -> Error {
     Error::new(
         ErrorKind::Unexpected,
-        "loading credentail to sign http request",
+        "loading credential to sign http request",
     )
     .set_temporary()
     .with_operation("reqsign::LoadCredential")
     .set_source(err)
 }
 
 /// Create a new error happened during signing request.
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/multipart.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/multipart.rs`

 * *Files 22% similar despite different names*

```diff
@@ -11,32 +11,38 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::mem;
 use std::str::FromStr;
 
 use bytes::Bytes;
 use bytes::BytesMut;
+use futures::stream;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::uri::PathAndQuery;
 use http::HeaderMap;
 use http::HeaderName;
 use http::HeaderValue;
 use http::Method;
 use http::Request;
+use http::Response;
+use http::StatusCode;
 use http::Uri;
 use http::Version;
 
 use super::new_request_build_error;
 use super::AsyncBody;
+use super::IncomingAsyncBody;
+use crate::raw::oio::into_stream;
 use crate::*;
 
 /// Multipart is a builder for multipart/form-data.
 #[derive(Debug)]
 pub struct Multipart<T: Part> {
     boundary: String,
     parts: Vec<T>,
@@ -54,37 +60,66 @@
         Multipart {
             boundary: format!("opendal-{}", uuid::Uuid::new_v4()),
             parts: Vec::default(),
         }
     }
 
     /// Set the boundary with given string.
-    #[cfg(test)]
-    fn with_boundary(mut self, boundary: &str) -> Self {
+    pub fn with_boundary(mut self, boundary: &str) -> Self {
         self.boundary = boundary.to_string();
         self
     }
 
     /// Insert a part into multipart.
     pub fn part(mut self, part: T) -> Self {
         self.parts.push(part);
         self
     }
 
+    /// Into parts.
+    pub fn into_parts(self) -> Vec<T> {
+        self.parts
+    }
+
+    /// Parse a response with multipart body into Multipart.
+    pub fn parse(mut self, bs: Bytes) -> Result<Self> {
+        let s = String::from_utf8(bs.to_vec()).map_err(|err| {
+            Error::new(
+                ErrorKind::Unexpected,
+                "multipart response contains invalid utf-8 chars",
+            )
+            .set_source(err)
+        })?;
+
+        let parts = s
+            .split(format!("--{}", self.boundary).as_str())
+            .collect::<Vec<&str>>();
+
+        for part in parts {
+            if part.is_empty() || part.starts_with("--") {
+                continue;
+            }
+
+            self.parts.push(T::parse(part)?);
+        }
+
+        Ok(self)
+    }
+
     pub(crate) fn build(&self) -> Bytes {
         let mut bs = BytesMut::new();
 
         // Write headers.
         for v in self.parts.iter() {
             // Write the first boundary
             bs.extend_from_slice(b"--");
             bs.extend_from_slice(self.boundary.as_bytes());
             bs.extend_from_slice(b"\r\n");
 
-            bs.extend_from_slice(v.build().as_ref());
+            bs.extend_from_slice(v.format().as_ref());
         }
 
         // Write the last boundary
         bs.extend_from_slice(b"--");
         bs.extend_from_slice(self.boundary.as_bytes());
         bs.extend_from_slice(b"--");
         bs.extend_from_slice(b"\r\n");
@@ -109,22 +144,25 @@
         builder
             .body(AsyncBody::Bytes(bs))
             .map_err(new_request_build_error)
     }
 }
 
 /// Part is a trait for multipart part.
-pub trait Part {
+pub trait Part: Sized {
     /// TYPE is the type of multipart.
     ///
     /// Current available types are: `form-data` and `mixed`
     const TYPE: &'static str;
 
-    /// Build will consume this part and generates the bytes.
-    fn build(&self) -> Bytes;
+    /// format will generates the bytes.
+    fn format(&self) -> Bytes;
+
+    /// parse will parse the bytes into a part.
+    fn parse(s: &str) -> Result<Self>;
 }
 
 /// FormDataPart is a builder for multipart/form-data part.
 #[derive(Debug)]
 pub struct FormDataPart {
     headers: HeaderMap,
     content: Bytes,
@@ -162,15 +200,15 @@
         self
     }
 }
 
 impl Part for FormDataPart {
     const TYPE: &'static str = "form-data";
 
-    fn build(&self) -> Bytes {
+    fn format(&self) -> Bytes {
         let mut bs = BytesMut::new();
 
         // Write headers.
         for (k, v) in self.headers.iter() {
             bs.extend_from_slice(k.as_str().as_bytes());
             bs.extend_from_slice(b": ");
             bs.extend_from_slice(v.as_bytes());
@@ -180,90 +218,130 @@
         // Write content.
         bs.extend_from_slice(b"\r\n");
         bs.extend_from_slice(&self.content);
         bs.extend_from_slice(b"\r\n");
 
         bs.freeze()
     }
+
+    fn parse(_: &str) -> Result<Self> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "parse of form-data is not supported",
+        ))
+    }
 }
 
 /// MixedPart is a builder for multipart/mixed part.
 #[derive(Debug)]
+#[cfg_attr(test, derive(Eq, PartialEq))]
 pub struct MixedPart {
     part_headers: HeaderMap,
 
-    method: Method,
-    uri: Uri,
+    /// Common
     version: Version,
     headers: HeaderMap,
     content: Bytes,
+
+    /// Request only
+    method: Option<Method>,
+    uri: Option<Uri>,
+
+    /// Response only
+    status_code: Option<StatusCode>,
 }
 
 impl MixedPart {
-    /// Create a new mixed part with gien uri.
+    /// Create a new mixed part with given uri.
     pub fn new(uri: &str) -> Self {
         let mut part_headers = HeaderMap::new();
         part_headers.insert(CONTENT_TYPE, "application/http".parse().unwrap());
         part_headers.insert("content-transfer-encoding", "binary".parse().unwrap());
 
         let uri = Uri::from_str(uri).expect("the uri used to build a mixed part must be valid");
 
         Self {
             part_headers,
-            method: Method::GET,
-            uri,
+
             version: Version::HTTP_11,
             headers: HeaderMap::new(),
             content: Bytes::new(),
+
+            uri: Some(uri),
+            method: None,
+
+            status_code: None,
         }
     }
 
     /// Build a mixed part from a request.
-    ///
-    /// # Notes
-    ///
-    /// Mixed parts only takes the path from the request uri.
     pub fn from_request(req: Request<AsyncBody>) -> Self {
         let mut part_headers = HeaderMap::new();
         part_headers.insert(CONTENT_TYPE, "application/http".parse().unwrap());
         part_headers.insert("content-transfer-encoding", "binary".parse().unwrap());
 
         let (parts, body) = req.into_parts();
 
         let content = match body {
             AsyncBody::Empty => Bytes::new(),
             AsyncBody::Bytes(bs) => bs,
+            AsyncBody::Stream(_) => panic!("multipart request can't contain stream body"),
         };
 
         Self {
             part_headers,
-            method: parts.method,
-            uri: Uri::from_str(
-                parts
-                    .uri
-                    .path_and_query()
-                    .unwrap_or(&PathAndQuery::from_static("/"))
-                    .as_str(),
-            )
-            .expect("the uri used to build a mixed part must be valid"),
+            uri: Some(
+                Uri::from_str(
+                    parts
+                        .uri
+                        .path_and_query()
+                        .unwrap_or(&PathAndQuery::from_static("/"))
+                        .as_str(),
+                )
+                .expect("the uri used to build a mixed part must be valid"),
+            ),
             version: parts.version,
             headers: parts.headers,
             content,
+
+            method: Some(parts.method),
+            status_code: None,
         }
     }
 
+    /// Consume a mixed part to build a response.
+    pub fn into_response(mut self) -> Response<IncomingAsyncBody> {
+        let mut builder = Response::builder();
+
+        builder = builder.status(self.status_code.unwrap_or(StatusCode::OK));
+        builder = builder.version(self.version);
+        // Swap headers directly instead of copy the entire map.
+        mem::swap(builder.headers_mut().unwrap(), &mut self.headers);
+
+        let bs: Bytes = self.content;
+        let length = bs.len();
+        let body = IncomingAsyncBody::new(
+            Box::new(into_stream::from_futures_stream(stream::iter(vec![Ok(bs)]))),
+            Some(length as u64),
+        );
+
+        builder
+            .body(body)
+            .expect("mixed part must be valid response")
+    }
+
     /// Insert a part header into part.
     pub fn part_header(mut self, key: HeaderName, value: HeaderValue) -> Self {
         self.part_headers.insert(key, value);
         self
     }
 
     /// Set the method for request in this part.
     pub fn method(mut self, method: Method) -> Self {
-        self.method = method;
+        self.method = Some(method);
         self
     }
 
     /// Set the version for request in this part.
     pub fn version(mut self, version: Version) -> Self {
         self.version = version;
         self
@@ -281,15 +359,15 @@
         self
     }
 }
 
 impl Part for MixedPart {
     const TYPE: &'static str = "mixed";
 
-    fn build(&self) -> Bytes {
+    fn format(&self) -> Bytes {
         let mut bs = BytesMut::new();
 
         // Write parts headers.
         for (k, v) in self.part_headers.iter() {
             // Trick!
             //
             // Azblob could not recognize header names like `content-type`
@@ -312,17 +390,29 @@
             bs.extend_from_slice(b": ");
             bs.extend_from_slice(v.as_bytes());
             bs.extend_from_slice(b"\r\n");
         }
 
         // Write request line: `DELETE /container0/blob0 HTTP/1.1`
         bs.extend_from_slice(b"\r\n");
-        bs.extend_from_slice(self.method.as_str().as_bytes());
+        bs.extend_from_slice(
+            self.method
+                .as_ref()
+                .expect("mixed part must be a valid request that contains method")
+                .as_str()
+                .as_bytes(),
+        );
         bs.extend_from_slice(b" ");
-        bs.extend_from_slice(self.uri.path().as_bytes());
+        bs.extend_from_slice(
+            self.uri
+                .as_ref()
+                .expect("mixed part must be a valid request that contains uri")
+                .path()
+                .as_bytes(),
+        );
         bs.extend_from_slice(b" ");
         bs.extend_from_slice(format!("{:?}", self.version).as_bytes());
         bs.extend_from_slice(b"\r\n");
 
         // Write request headers.
         for (k, v) in self.headers.iter() {
             bs.extend_from_slice(k.as_str().as_bytes());
@@ -336,14 +426,99 @@
         if !self.content.is_empty() {
             bs.extend_from_slice(&self.content);
             bs.extend_from_slice(b"\r\n");
         }
 
         bs.freeze()
     }
+
+    /// TODO
+    ///
+    /// This is a simple implementation and have a lot of space to improve.
+    fn parse(s: &str) -> Result<Self> {
+        let parts = s.splitn(2, "\r\n\r\n").collect::<Vec<&str>>();
+        let part_headers_content = parts[0];
+        let http_response = parts.get(1).unwrap_or(&"");
+
+        let mut part_headers = HeaderMap::new();
+        for line in part_headers_content.lines() {
+            let parts = line.splitn(2, ": ").collect::<Vec<&str>>();
+            if parts.len() == 2 {
+                let header_name = HeaderName::from_str(parts[0]).map_err(|err| {
+                    Error::new(
+                        ErrorKind::Unexpected,
+                        "multipart response contains invalid part header name",
+                    )
+                    .set_source(err)
+                })?;
+                let header_value = parts[1].parse().map_err(|err| {
+                    Error::new(
+                        ErrorKind::Unexpected,
+                        "multipart response contains invalid part header value",
+                    )
+                    .set_source(err)
+                })?;
+
+                part_headers.insert(header_name, header_value);
+            }
+        }
+
+        let parts = http_response.split("\r\n\r\n").collect::<Vec<&str>>();
+        let headers_content = parts[0];
+        let body_content = parts.get(1).unwrap_or(&"");
+
+        let status_line = headers_content.lines().next().unwrap_or("");
+        let status_code = status_line
+            .split_whitespace()
+            .nth(1)
+            .unwrap_or("")
+            .parse::<u16>()
+            .unwrap_or(200);
+
+        let mut headers = HeaderMap::new();
+        for line in headers_content.lines().skip(1) {
+            let parts = line.splitn(2, ": ").collect::<Vec<&str>>();
+            if parts.len() == 2 {
+                let header_name = HeaderName::from_str(parts[0]).map_err(|err| {
+                    Error::new(
+                        ErrorKind::Unexpected,
+                        "multipart response contains invalid part header name",
+                    )
+                    .set_source(err)
+                })?;
+                let header_value = parts[1].parse().map_err(|err| {
+                    Error::new(
+                        ErrorKind::Unexpected,
+                        "multipart response contains invalid part header value",
+                    )
+                    .set_source(err)
+                })?;
+
+                headers.insert(header_name, header_value);
+            }
+        }
+
+        Ok(Self {
+            part_headers,
+            version: Version::HTTP_11,
+            headers,
+            content: Bytes::from(body_content.to_string()),
+
+            method: None,
+            uri: None,
+
+            status_code: Some(StatusCode::from_u16(status_code).map_err(|err| {
+                Error::new(
+                    ErrorKind::Unexpected,
+                    "multipart response contains invalid status code",
+                )
+                .set_source(err)
+            })?),
+        })
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use http::header::CONTENT_TYPE;
     use pretty_assertions::assert_eq;
 
@@ -651,8 +826,194 @@
             // Rust can't represent `\r` in a string literal, so we
             // replace `\r\n` with `\n` for comparison
             String::from_utf8(body.to_vec())
                 .unwrap()
                 .replace("\r\n", "\n")
         );
     }
+
+    /// This test is inspired by <https://cloud.google.com/storage/docs/batch>
+    #[test]
+    fn test_multipart_mixed_gcs_batch_metadata_response() {
+        let response = r#"--batch_pK7JBAk73-E=_AA5eFwv4m2Q=
+Content-Type: application/http
+Content-ID: <response-b29c5de2-0db4-490b-b421-6a51b598bd22+1>
+
+HTTP/1.1 200 OK
+ETag: "lGaP-E0memYDumK16YuUDM_6Gf0/V43j6azD55CPRGb9b6uytDYl61Y"
+Content-Type: application/json; charset=UTF-8
+Date: Mon, 22 Jan 2018 18:56:00 GMT
+Expires: Mon, 22 Jan 2018 18:56:00 GMT
+Cache-Control: private, max-age=0
+Content-Length: 846
+
+{"kind": "storage#object","id": "example-bucket/obj1/1495822576643790","metadata": {"type": "tabby"}}
+
+--batch_pK7JBAk73-E=_AA5eFwv4m2Q=
+Content-Type: application/http
+Content-ID: <response-b29c5de2-0db4-490b-b421-6a51b598bd22+2>
+
+HTTP/1.1 200 OK
+ETag: "lGaP-E0memYDumK16YuUDM_6Gf0/91POdd-sxSAkJnS8Dm7wMxBSDKk"
+Content-Type: application/json; charset=UTF-8
+Date: Mon, 22 Jan 2018 18:56:00 GMT
+Expires: Mon, 22 Jan 2018 18:56:00 GMT
+Cache-Control: private, max-age=0
+Content-Length: 846
+
+{"kind": "storage#object","id": "example-bucket/obj2/1495822576643790","metadata": {"type": "tuxedo"}}
+
+--batch_pK7JBAk73-E=_AA5eFwv4m2Q=
+Content-Type: application/http
+Content-ID: <response-b29c5de2-0db4-490b-b421-6a51b598bd22+3>
+
+HTTP/1.1 200 OK
+ETag: "lGaP-E0memYDumK16YuUDM_6Gf0/d2Z1F1_ZVbB1dC0YKM9rX5VAgIQ"
+Content-Type: application/json; charset=UTF-8
+Date: Mon, 22 Jan 2018 18:56:00 GMT
+Expires: Mon, 22 Jan 2018 18:56:00 GMT
+Cache-Control: private, max-age=0
+Content-Length: 846
+
+{"kind": "storage#object","id": "example-bucket/obj3/1495822576643790","metadata": {"type": "calico"}}
+
+--batch_pK7JBAk73-E=_AA5eFwv4m2Q=--"#.replace('\n', "\r\n");
+
+        let multipart: Multipart<MixedPart> = Multipart::new()
+            .with_boundary("batch_pK7JBAk73-E=_AA5eFwv4m2Q=")
+            .parse(Bytes::from(response))
+            .unwrap();
+
+        assert_eq!(multipart.parts.len(), 3);
+        assert_eq!(
+            multipart.parts[0],
+            MixedPart {
+                part_headers: {
+                    let mut h = HeaderMap::new();
+                    h.insert("Content-Type", "application/http".parse().unwrap());
+                    h.insert(
+                        "Content-ID",
+                        "<response-b29c5de2-0db4-490b-b421-6a51b598bd22+1>"
+                            .parse()
+                            .unwrap(),
+                    );
+
+                    h
+                },
+                version: Version::HTTP_11,
+                headers: {
+                    let mut h = HeaderMap::new();
+                    h.insert(
+                        "ETag",
+                        "\"lGaP-E0memYDumK16YuUDM_6Gf0/V43j6azD55CPRGb9b6uytDYl61Y\""
+                            .parse()
+                            .unwrap(),
+                    );
+                    h.insert(
+                        "Content-Type",
+                        "application/json; charset=UTF-8".parse().unwrap(),
+                    );
+                    h.insert("Date", "Mon, 22 Jan 2018 18:56:00 GMT".parse().unwrap());
+                    h.insert("Expires", "Mon, 22 Jan 2018 18:56:00 GMT".parse().unwrap());
+                    h.insert("Cache-Control", "private, max-age=0".parse().unwrap());
+                    h.insert("Content-Length", "846".parse().unwrap());
+
+                    h
+                },
+                content: Bytes::from_static(
+                    r#"{"kind": "storage#object","id": "example-bucket/obj1/1495822576643790","metadata": {"type": "tabby"}}"#
+                    .as_bytes()
+                ),
+                uri: None,
+                method: None,
+                status_code: Some(StatusCode::from_u16(200).unwrap())
+            }
+        );
+        assert_eq!(
+            multipart.parts[1],
+            MixedPart {
+                part_headers: {
+                    let mut h = HeaderMap::new();
+                    h.insert("Content-Type", "application/http".parse().unwrap());
+                    h.insert(
+                        "Content-ID",
+                        "<response-b29c5de2-0db4-490b-b421-6a51b598bd22+2>"
+                            .parse()
+                            .unwrap(),
+                    );
+
+                    h
+                },
+                version: Version::HTTP_11,
+                headers: {
+                    let mut h = HeaderMap::new();
+                    h.insert(
+                        "ETag",
+                        "\"lGaP-E0memYDumK16YuUDM_6Gf0/91POdd-sxSAkJnS8Dm7wMxBSDKk\""
+                            .parse()
+                            .unwrap(),
+                    );
+                    h.insert(
+                        "Content-Type",
+                        "application/json; charset=UTF-8".parse().unwrap(),
+                    );
+                    h.insert("Date", "Mon, 22 Jan 2018 18:56:00 GMT".parse().unwrap());
+                    h.insert("Expires", "Mon, 22 Jan 2018 18:56:00 GMT".parse().unwrap());
+                    h.insert("Cache-Control", "private, max-age=0".parse().unwrap());
+                    h.insert("Content-Length", "846".parse().unwrap());
+
+                    h
+                },
+                content: Bytes::from_static(
+                    r#"{"kind": "storage#object","id": "example-bucket/obj2/1495822576643790","metadata": {"type": "tuxedo"}}"#
+                    .as_bytes()
+                ),
+                uri: None,
+                method: None,
+                status_code: Some(StatusCode::from_u16(200).unwrap())
+            }
+         );
+        assert_eq!(
+            multipart.parts[2],
+            MixedPart {
+                part_headers: {
+                    let mut h = HeaderMap::new();
+                    h.insert("Content-Type", "application/http".parse().unwrap());
+                    h.insert(
+                        "Content-ID",
+                        "<response-b29c5de2-0db4-490b-b421-6a51b598bd22+3>"
+                            .parse()
+                            .unwrap(),
+                    );
+
+                    h
+                },
+                version: Version::HTTP_11,
+                headers: {
+                    let mut h = HeaderMap::new();
+                    h.insert(
+                        "ETag",
+                        "\"lGaP-E0memYDumK16YuUDM_6Gf0/d2Z1F1_ZVbB1dC0YKM9rX5VAgIQ\""
+                            .parse()
+                            .unwrap(),
+                    );
+                    h.insert(
+                        "Content-Type",
+                        "application/json; charset=UTF-8".parse().unwrap(),
+                    );
+                    h.insert("Date", "Mon, 22 Jan 2018 18:56:00 GMT".parse().unwrap());
+                    h.insert("Expires", "Mon, 22 Jan 2018 18:56:00 GMT".parse().unwrap());
+                    h.insert("Cache-Control", "private, max-age=0".parse().unwrap());
+                    h.insert("Content-Length", "846".parse().unwrap());
+
+                    h
+                },
+                content: Bytes::from_static(
+                    r#"{"kind": "storage#object","id": "example-bucket/obj3/1495822576643790","metadata": {"type": "calico"}}"#
+                    .as_bytes()
+                ),
+                uri: None,
+                method: None,
+                status_code: Some(StatusCode::from_u16(200).unwrap())
+            });
+    }
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/append.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/append.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files 26% similar despite different names*

```diff
@@ -26,30 +26,35 @@
 pub use read::BlockingRead;
 pub use read::BlockingReader;
 pub use read::Read;
 pub use read::ReadExt;
 pub use read::ReadOperation;
 pub use read::Reader;
 
-pub mod into_reader;
-
 pub mod into_blocking_reader;
+pub mod into_reader;
 
 mod write;
 pub use write::BlockingWrite;
 pub use write::BlockingWriter;
 pub use write::Write;
 pub use write::WriteOperation;
 pub use write::Writer;
 
 mod append;
 pub use append::Append;
 pub use append::AppendOperation;
 pub use append::Appender;
 
+mod stream;
+pub use stream::Stream;
+pub use stream::Streamer;
+
+pub mod into_stream;
+
 mod cursor;
 pub use cursor::Cursor;
 pub use cursor::VectorCursor;
 
 mod into_streamable;
 pub use into_streamable::into_streamable_reader;
 pub use into_streamable::IntoStreamableReader;
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         match v {
             Next => "Pager::next",
             BlockingNext => "BlockingPager::next",
         }
     }
 }
 
-/// Page trait is used by [`crate::raw::Accessor`] to implement `list`
+/// Page trait is used by [`raw::Accessor`] to implement `list`
 /// or `scan` operation.
 #[async_trait]
 pub trait Page: Send + Sync + 'static {
     /// Fetch a new page of [`Entry`]
     ///
     /// `Ok(None)` means all pages have been returned. Any following call
     /// to `next` will always get the same result.
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 
 use std::fmt::Display;
 use std::fmt::Formatter;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 
+use crate::raw::*;
 use crate::*;
 
 /// WriteOperation is the name for APIs of Writer.
 #[derive(Debug, Copy, Clone, Hash, Eq, PartialEq)]
 #[non_exhaustive]
 pub enum WriteOperation {
     /// Operation for [`Write::write`]
     Write,
+    /// Operation for [`Write::sink`]
+    Sink,
     /// Operation for [`Write::abort`]
     Abort,
     /// Operation for [`Write::close`]
     Close,
     /// Operation for [`BlockingWrite::write`]
     BlockingWrite,
     /// Operation for [`BlockingWrite::close`]
@@ -54,14 +57,15 @@
 
 impl From<WriteOperation> for &'static str {
     fn from(v: WriteOperation) -> &'static str {
         use WriteOperation::*;
 
         match v {
             Write => "Writer::write",
+            Sink => "Writer::sink",
             Abort => "Writer::abort",
             Close => "Writer::close",
             BlockingWrite => "BlockingWriter::write",
             BlockingClose => "BlockingWriter::close",
         }
     }
 }
@@ -79,24 +83,27 @@
 /// - Unsized: The total size of the object is unknown in advance.
 ///
 /// And it's possible that the given bs length is less than the total
 /// content length. Users will call write multiple times to write
 /// the whole data.
 #[async_trait]
 pub trait Write: Unpin + Send + Sync {
-    /// Write given into writer.
+    /// Write given bytes into writer.
     ///
     /// # Notes
     ///
     /// It's possible that the given bs length is less than the total
     /// content length. And users will call write multiple times.
     ///
     /// Please make sure `write` is safe to re-enter.
     async fn write(&mut self, bs: Bytes) -> Result<()>;
 
+    /// Sink given stream into writer.
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()>;
+
     /// Abort the pending writer.
     async fn abort(&mut self) -> Result<()>;
 
     /// Close the writer and make sure all data has been flushed.
     async fn close(&mut self) -> Result<()>;
 }
 
@@ -104,14 +111,21 @@
 impl Write for () {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let _ = bs;
 
         unimplemented!("write is required to be implemented for oio::Write")
     }
 
+    async fn sink(&mut self, _: u64, _: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "output writer doesn't support sink",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
     }
 
@@ -128,14 +142,18 @@
 /// To make Writer work as expected, we must add this impl.
 #[async_trait]
 impl<T: Write + ?Sized> Write for Box<T> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         (**self).write(bs).await
     }
 
+    async fn sink(&mut self, n: u64, s: oio::Streamer) -> Result<()> {
+        (**self).sink(n, s).await
+    }
+
     async fn abort(&mut self) -> Result<()> {
         (**self).abort().await
     }
 
     async fn close(&mut self) -> Result<()> {
         (**self).close().await
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/ops.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/ops.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.38.0/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/appender.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 const KNOWN_AZBLOB_ENDPOINT_SUFFIX: &[&str] = &[
     "blob.core.windows.net",
     "blob.core.usgovcloudapi.net",
     "blob.core.chinacloudapi.cn",
 ];
 
 const AZBLOB_BATCH_LIMIT: usize = 256;
-
 /// Azure Storage Blob services support.
 #[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct AzblobBuilder {
     root: Option<String>,
     container: String,
     endpoint: Option<String>,
     account_name: Option<String>,
     account_key: Option<String>,
     encryption_key: Option<String>,
     encryption_key_sha256: Option<String>,
     encryption_algorithm: Option<String>,
     sas_token: Option<String>,
     http_client: Option<HttpClient>,
+    batch_max_operations: Option<usize>,
 }
 
 impl Debug for AzblobBuilder {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut ds = f.debug_struct("Builder");
 
         ds.field("root", &self.root);
@@ -253,14 +253,21 @@
     /// This API is part of OpenDAL's Raw API. `HttpClient` could be changed
     /// during minor updates.
     pub fn http_client(&mut self, client: HttpClient) -> &mut Self {
         self.http_client = Some(client);
         self
     }
 
+    /// Set maximum batch operations of this backend.
+    pub fn batch_max_operations(&mut self, batch_max_operations: usize) -> &mut Self {
+        self.batch_max_operations = Some(batch_max_operations);
+
+        self
+    }
+
     /// from_connection_string will make a builder from connection string
     ///
     /// connection string looks like:
     ///
     /// ```txt
     /// DefaultEndpointsProtocol=http;AccountName=devstoreaccount1;
     /// AccountKey=Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==;
@@ -356,14 +363,16 @@
         map.get("account_key").map(|v| builder.account_key(v));
         map.get("encryption_key").map(|v| builder.encryption_key(v));
         map.get("encryption_key_sha256")
             .map(|v| builder.encryption_key_sha256(v));
         map.get("encryption_algorithm")
             .map(|v| builder.encryption_algorithm(v));
         map.get("sas_token").map(|v| builder.sas_token(v));
+        map.get("batch_max_operations")
+            .map(|v| builder.batch_max_operations(v.parse::<usize>().unwrap()));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", &self);
 
@@ -437,27 +446,30 @@
             }
         };
 
         let cred_loader = AzureStorageLoader::new(config_loader);
 
         let signer = AzureStorageSigner::new();
 
+        let batch_max_operations = self.batch_max_operations.unwrap_or(AZBLOB_BATCH_LIMIT);
+
         debug!("backend build finished: {:?}", &self);
         Ok(AzblobBackend {
             core: Arc::new(AzblobCore {
                 root,
                 endpoint,
                 encryption_key,
                 encryption_key_sha256,
                 encryption_algorithm,
                 container: self.container.clone(),
 
                 client,
                 loader: cred_loader,
                 signer,
+                batch_max_operations,
             }),
             has_sas_token: self.sas_token.is_some(),
         })
     }
 }
 
 fn infer_storage_name_from_endpoint(endpoint: &str) -> Option<String> {
@@ -537,15 +549,15 @@
                 presign: self.has_sas_token,
                 presign_stat: self.has_sas_token,
                 presign_read: self.has_sas_token,
                 presign_write: self.has_sas_token,
 
                 batch: true,
                 batch_delete: true,
-                batch_max_operations: Some(AZBLOB_BATCH_LIMIT),
+                batch_max_operations: Some(self.core.batch_max_operations),
 
                 ..Default::default()
             });
 
         am
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     pub endpoint: String,
     pub encryption_key: Option<HeaderValue>,
     pub encryption_key_sha256: Option<HeaderValue>,
     pub encryption_algorithm: Option<HeaderValue>,
     pub client: HttpClient,
     pub loader: AzureStorageLoader,
     pub signer: AzureStorageSigner,
+    pub batch_max_operations: usize,
 }
 
 impl Debug for AzblobCore {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
         f.debug_struct("AzblobCore")
             .field("container", &self.container)
             .field("root", &self.root)
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,21 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/writer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -17,79 +17,60 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::AzdfsCore;
+use super::core::DropboxCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct AzdfsWriter {
-    core: Arc<AzdfsCore>,
-
+pub struct DropboxWriter {
+    core: Arc<DropboxCore>,
     op: OpWrite,
     path: String,
 }
 
-impl AzdfsWriter {
-    pub fn new(core: Arc<AzdfsCore>, op: OpWrite, path: String) -> Self {
-        AzdfsWriter { core, op, path }
+impl DropboxWriter {
+    pub fn new(core: Arc<DropboxCore>, op: OpWrite, path: String) -> Self {
+        DropboxWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for AzdfsWriter {
+impl oio::Write for DropboxWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.azdfs_create_request(
-            &self.path,
-            "file",
-            self.op.content_type(),
-            self.op.content_disposition(),
-            AsyncBody::Empty,
-        )?;
-
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
-
-        let status = resp.status();
-        match status {
-            StatusCode::CREATED | StatusCode::OK => {
-                resp.into_body().consume().await?;
-            }
-            _ => {
-                return Err(parse_error(resp)
-                    .await?
-                    .with_operation("Backend::azdfs_create_request"));
-            }
-        }
-
-        let mut req =
-            self.core
-                .azdfs_update_request(&self.path, Some(bs.len()), AsyncBody::Bytes(bs))?;
-
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
-
+        let resp = self
+            .core
+            .dropbox_update(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
         let status = resp.status();
         match status {
-            StatusCode::OK | StatusCode::ACCEPTED => {
+            StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
-            _ => Err(parse_error(resp)
-                .await?
-                .with_operation("Backend::azdfs_update_request")),
+            _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/appender.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/cos/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 13% similar despite different names*

```diff
@@ -11,64 +11,68 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::CosCore;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct CosWriter {
-    core: Arc<CosCore>,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl CosWriter {
-    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
-        CosWriter { core, op, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for CosWriter {
+impl oio::Write for WebhdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.cos_put_object_request(
-            &self.path,
-            Some(bs.len()),
-            self.op.content_type(),
-            self.op.cache_control(),
-            AsyncBody::Bytes(bs),
-        )?;
-
-        self.core.sign(&mut req).await?;
+        let req = self
+            .backend
+            .webhdfs_create_object_request(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
-        let resp = self.core.send(req).await?;
+        let resp = self.backend.client.send(req).await?;
 
         let status = resp.status();
-
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/fs/appender.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/fs/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/fs/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/fs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,21 @@
             .map_err(parse_io_error)?;
         self.f.write_all(&bs).await.map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
         Ok(())
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 use super::pager::FtpPager;
 use super::util::FtpReader;
 use super::writer::FtpWriter;
 use crate::raw::*;
 use crate::*;
 
 /// FTP and FTPS services support.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct FtpBuilder {
     endpoint: Option<String>,
     root: Option<String>,
     user: Option<String>,
     password: Option<String>,
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ftp/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,21 @@
         })?;
 
         ftp_stream.finalize_put_stream(data_stream).await?;
 
         Ok(())
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -401,14 +401,16 @@
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Gcs)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
+                create_dir: true,
+
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
@@ -423,14 +425,16 @@
 
                 list: true,
                 list_with_limit: true,
                 list_with_start_after: true,
                 list_with_delimiter_slash: true,
                 list_without_delimiter: true,
 
+                batch: true,
+                batch_max_operations: Some(100),
                 presign: true,
                 presign_stat: true,
                 presign_read: true,
                 presign_write: true,
 
                 ..Default::default()
             });
@@ -553,14 +557,73 @@
                 args.delimiter(),
                 args.limit(),
                 args.start_after(),
             ),
         ))
     }
 
+    async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
+        let ops = args.into_operation();
+        if ops.len() > 100 {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "gcs services only allow delete less than 100 keys at once",
+            )
+            .with_context("length", ops.len().to_string()));
+        }
+
+        let paths: Vec<String> = ops.into_iter().map(|(p, _)| p).collect();
+        let resp = self.core.gcs_delete_objects(paths.clone()).await?;
+
+        let status = resp.status();
+
+        if let StatusCode::OK = status {
+            let content_type = parse_content_type(resp.headers())?.ok_or_else(|| {
+                Error::new(
+                    ErrorKind::Unexpected,
+                    "gcs batch delete response content type is empty",
+                )
+            })?;
+            let boundary = content_type
+                .strip_prefix("multipart/mixed; boundary=")
+                .ok_or_else(|| {
+                    Error::new(
+                        ErrorKind::Unexpected,
+                        "gcs batch delete response content type is not multipart/mixed",
+                    )
+                })?
+                .trim_matches('"');
+            let multipart: Multipart<MixedPart> = Multipart::new()
+                .with_boundary(boundary)
+                .parse(resp.into_body().bytes().await?)?;
+            let parts = multipart.into_parts();
+
+            let mut batched_result = Vec::with_capacity(parts.len());
+
+            for (i, part) in parts.into_iter().enumerate() {
+                let resp = part.into_response();
+                // TODO: maybe we can take it directly?
+                let path = paths[i].clone();
+
+                // deleting not existing objects is ok
+                if resp.status().is_success() || resp.status() == StatusCode::NOT_FOUND {
+                    batched_result.push((path, Ok(RpDelete::default().into())));
+                } else {
+                    batched_result.push((path, Err(parse_error(resp).await?)));
+                }
+            }
+
+            Ok(RpBatch::new(batched_result))
+        } else {
+            // If the overall request isn't formatted correctly and Cloud Storage is unable to parse it into sub-requests, you receive a 400 error.
+            // Otherwise, Cloud Storage returns a 200 status code, even if some or all of the sub-requests fail.
+            Err(parse_error(resp).await?)
+        }
+    }
+
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
                 self.core
                     .gcs_head_object_xml_request(path, v.if_match(), v.if_none_match())?
             }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -367,29 +367,55 @@
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     pub async fn gcs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.gcs_delete_object_request(path)?;
+
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
+
+    pub fn gcs_delete_object_request(&self, path: &str) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/storage/v1/b/{}/o/{}",
             self.endpoint,
             self.bucket,
             percent_encode_path(&p)
         );
 
-        let mut req = Request::delete(&url)
+        Request::delete(&url)
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+            .map_err(new_request_build_error)
+    }
 
-        self.sign(&mut req).await?;
+    pub async fn gcs_delete_objects(
+        &self,
+        paths: Vec<String>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let uri = format!("{}/batch/storage/v1", self.endpoint);
+
+        let mut multipart = Multipart::new();
+
+        for (idx, path) in paths.iter().enumerate() {
+            let req = self.gcs_delete_object_request(path)?;
+
+            multipart = multipart.part(
+                MixedPart::from_request(req).part_header("content-id".parse().unwrap(), idx.into()),
+            );
+        }
 
+        let req = Request::post(uri);
+        let mut req = multipart.apply(req)?;
+
+        self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn gcs_copy_object(
         &self,
         from: &str,
         to: &str,
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,21 @@
                 // write is re-enter safe.
                 self.buffer.pop();
                 Err(e)
             }
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         let location = if let Some(location) = &self.location {
             location
         } else {
             return Ok(());
         };
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/builder.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/gdrive/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,21 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,21 @@
         } else {
             Err(parse_error(resp)
                 .await
                 .map(|err| err.with_operation("Backend::ghac_upload"))?)
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         let req = self.backend.ghac_commit(self.cache_id, self.size).await?;
         let resp = self.backend.client.send(req).await?;
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 use super::error::parse_io_error;
 use super::pager::HdfsPager;
 use super::writer::HdfsWriter;
 use crate::raw::*;
 use crate::*;
 
 /// [Hadoop Distributed File System (HDFS™)](https://hadoop.apache.org/) support.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Debug, Default)]
 pub struct HdfsBuilder {
     root: Option<String>,
     name_node: Option<String>,
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,21 @@
         }
         // Reset pos to 0 for next write.
         self.pos = 0;
 
         Ok(())
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 use super::error::parse_error;
 use super::ipld::PBNode;
 use crate::raw::*;
 use crate::*;
 
 /// IPFS file system support based on [IPFS HTTP Gateway](https://docs.ipfs.tech/concepts/ipfs-gateway/).
-///
 #[doc = include_str!("docs.md")]
 #[derive(Default, Clone, Debug)]
 pub struct IpfsBuilder {
     endpoint: Option<String>,
     root: Option<String>,
     http_client: Option<HttpClient>,
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 use super::error::parse_error;
 use super::pager::IpmfsPager;
 use super::writer::IpmfsWriter;
 use crate::raw::*;
 use crate::*;
 
 /// IPFS Mutable File System (IPMFS) backend.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Clone)]
 pub struct IpmfsBackend {
     root: String,
     endpoint: String,
     client: HttpClient,
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -15,47 +15,62 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::IpmfsBackend;
+use super::backend::VercelArtifactsBackend;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct IpmfsWriter {
-    backend: IpmfsBackend,
+pub struct VercelArtifactsWriter {
+    backend: VercelArtifactsBackend,
+    op: OpWrite,
 
     path: String,
 }
 
-impl IpmfsWriter {
-    pub fn new(backend: IpmfsBackend, path: String) -> Self {
-        IpmfsWriter { backend, path }
+impl VercelArtifactsWriter {
+    pub fn new(backend: VercelArtifactsBackend, op: OpWrite, path: String) -> Self {
+        VercelArtifactsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for IpmfsWriter {
+impl oio::Write for VercelArtifactsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self.backend.ipmfs_write(&self.path, bs).await?;
+        let resp = self
+            .backend
+            .vercel_artifacts_put(
+                self.path.as_str(),
+                self.op.content_length().unwrap(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
         let status = resp.status();
 
         match status {
-            StatusCode::CREATED | StatusCode::OK => {
+            StatusCode::OK | StatusCode::ACCEPTED => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::BTreeMap;
 use std::collections::HashMap;
+use std::fmt::Debug;
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use parking_lot::Mutex;
 
 use crate::raw::adapters::typed_kv;
 use crate::*;
 
 /// In memory service support. (BTreeMap Based)
-///
 #[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct MemoryBuilder {
     root: Option<String>,
 }
 
 impl MemoryBuilder {
@@ -61,19 +61,25 @@
         Ok(MemoryBackend::new(adapter).with_root(self.root.as_deref().unwrap_or_default()))
     }
 }
 
 /// Backend is used to serve `Accessor` support in memory.
 pub type MemoryBackend = typed_kv::Backend<Adapter>;
 
-#[derive(Debug, Clone)]
+#[derive(Clone)]
 pub struct Adapter {
     inner: Arc<Mutex<BTreeMap<String, typed_kv::Value>>>,
 }
 
+impl Debug for Adapter {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        f.debug_struct("MemoryBackend").finish_non_exhaustive()
+    }
+}
+
 #[async_trait]
 impl typed_kv::Adapter for Adapter {
     fn info(&self) -> typed_kv::Info {
         typed_kv::Info::new(
             Scheme::Memory,
             &format!("{:?}", &self.inner as *const _),
             typed_kv::Capability {
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,19 @@
 pub use memcached::Memcached;
 
 #[cfg(feature = "services-memory")]
 mod memory;
 #[cfg(feature = "services-memory")]
 pub use memory::Memory;
 
+#[cfg(feature = "services-mini-moka")]
+mod mini_moka;
+#[cfg(feature = "services-mini-moka")]
+pub use self::mini_moka::MiniMoka;
+
 #[cfg(feature = "services-moka")]
 mod moka;
 #[cfg(feature = "services-moka")]
 pub use self::moka::Moka;
 
 #[cfg(feature = "services-obs")]
 mod obs;
@@ -100,14 +105,19 @@
 pub use obs::Obs;
 
 #[cfg(feature = "services-oss")]
 mod oss;
 #[cfg(feature = "services-oss")]
 pub use oss::Oss;
 
+#[cfg(feature = "services-cacache")]
+mod cacache;
+#[cfg(feature = "services-cacache")]
+pub use self::cacache::Cacache;
+
 #[cfg(feature = "services-redis")]
 mod redis;
 #[cfg(feature = "services-redis")]
 pub use self::redis::Redis;
 
 #[cfg(feature = "services-rocksdb")]
 mod rocksdb;
@@ -152,14 +162,24 @@
 #[cfg(feature = "services-onedrive")]
 pub use onedrive::Onedrive;
 
 #[cfg(feature = "services-gdrive")]
 mod gdrive;
 #[cfg(feature = "services-gdrive")]
 pub use gdrive::Gdrive;
+
+#[cfg(feature = "services-dropbox")]
+mod dropbox;
+#[cfg(feature = "services-dropbox")]
+pub use dropbox::Dropbox;
 #[cfg(feature = "services-webhdfs")]
 pub use webhdfs::Webhdfs;
 
 #[cfg(feature = "services-vercel-artifacts")]
 mod vercel_artifacts;
 #[cfg(feature = "services-vercel-artifacts")]
 pub use vercel_artifacts::VercelArtifacts;
+
+#[cfg(feature = "services-redb")]
+mod redb;
+#[cfg(feature = "services-redb")]
+pub use self::redb::Redb;
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/obs/appender.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/obs/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 use http::StatusCode;
 use http::Uri;
 use log::debug;
 use reqsign::HuaweicloudObsConfig;
 use reqsign::HuaweicloudObsCredentialLoader;
 use reqsign::HuaweicloudObsSigner;
 
+use super::appender::ObsAppender;
+use super::core::ObsCore;
 use super::error::parse_error;
 use super::pager::ObsPager;
 use super::writer::ObsWriter;
-use super::{appender::ObsAppender, core::ObsCore};
 use crate::raw::*;
 use crate::*;
 
 /// Huawei Cloud OBS services support.
 ///
 /// # Capabilities
 ///
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::time::Duration;
 
+use http::header::CACHE_CONTROL;
+use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
-use http::header::{CACHE_CONTROL, CONTENT_DISPOSITION};
 use http::Request;
 use http::Response;
 use reqsign::HuaweicloudObsCredential;
 use reqsign::HuaweicloudObsCredentialLoader;
 use reqsign::HuaweicloudObsSigner;
 
 use crate::raw::*;
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,21 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     type BlockingWriter = ();
     type Appender = ();
     type Pager = OnedrivePager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
-        ma.set_scheme(crate::Scheme::Onedrive)
+        ma.set_scheme(Scheme::Onedrive)
             .set_root(&self.root)
             .set_capability(Capability {
                 read: true,
                 write: true,
                 stat: true,
                 delete: true,
                 create_dir: true,
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/builder.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/onedrive/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,21 @@
         if size <= Self::MAX_SIMPLE_SIZE {
             self.write_simple(bs).await
         } else {
             self.write_chunked(bs).await
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/appender.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -170,14 +170,21 @@
                 // write is re-enter safe.
                 self.buffer.pop();
                 Err(e)
             }
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     // TODO: we can cancel the upload by sending an abort request.
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 use crate::raw::*;
 use crate::*;
 
 const DEFAULT_REDIS_ENDPOINT: &str = "tcp://127.0.0.1:6379";
 const DEFAULT_REDIS_PORT: u16 = 6379;
 
 /// [Redis](https://redis.io/) services support.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Clone, Default)]
 pub struct RedisBuilder {
     /// network address of the Redis service. Can be "tcp://127.0.0.1:6379", e.g.
     ///
     /// default is "tcp://127.0.0.1:6379"
     endpoint: Option<String>,
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/redis/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/redis/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 This service can be used to:
 
 - [x] stat
 - [x] read
 - [x] write
 - [x] create_dir
 - [x] delete
-- [ ] copy
-- [ ] rename
+- [x] copy
+- [x] rename
 - [ ] ~~list~~
 - [ ] scan
 - [ ] ~~presign~~
 - [ ] blocking
 
 ## Configuration
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 use rocksdb::DB;
 
 use crate::raw::adapters::kv;
 use crate::Result;
 use crate::*;
 
 /// RocksDB service support.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Clone, Default, Debug)]
 pub struct RocksdbBuilder {
     /// The path to the rocksdb data directory.
     datadir: Option<String>,
     /// the working directory of the service. Can be "/path/to/dir"
     ///
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/rocksdb/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/docs.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 This service can be used to:
 
 - [x] stat
 - [x] read
 - [x] write
 - [x] create_dir
 - [x] delete
-- [ ] copy
-- [ ] rename
+- [x] copy
+- [x] rename
 - [ ] ~~list~~
 - [x] scan
 - [ ] ~~presign~~
 - [x] blocking
 
 ## Note
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     m
 });
 
 const DEFAULT_WRITE_MIN_SIZE: usize = 8 * 1024 * 1024;
 const DEFAULT_BATCH_MAX_OPERATIONS: usize = 1000;
 /// Aws S3 and compatible services (including minio, digitalocean space, Tencent Cloud Object Storage(COS) and so on) support.
 /// For more information about s3-compatible services, refer to [Compatible Services](#compatible-services).
-///
 #[doc = include_str!("docs.md")]
 #[doc = include_str!("compatible_services.md")]
 #[derive(Default)]
 pub struct S3Builder {
     root: Option<String>,
 
     bucket: String,
@@ -410,15 +409,15 @@
     /// to load credential from ec2 metadata, a.k.a, IMDSv2
     pub fn disable_ec2_metadata(&mut self) -> &mut Self {
         self.disable_ec2_metadata = true;
         self
     }
 
     /// Allow anonymous will allow opendal to send request without signing
-    /// when credentail is not loaded.
+    /// when credential is not loaded.
     pub fn allow_anonymous(&mut self) -> &mut Self {
         self.allow_anonymous = true;
         self
     }
 
     /// Enable virtual host style so that opendal will send API requests
     /// in virtual host style instead of path style.
@@ -765,14 +764,15 @@
                 read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
                 read_with_override_cache_control: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
+                write_can_sink: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
                 create_dir: true,
                 delete: true,
                 copy: true,
 
@@ -965,22 +965,21 @@
                 quick_xml::de::from_reader(bs.reader()).map_err(new_xml_deserialize_error)?;
 
             let mut batched_result = Vec::with_capacity(result.deleted.len() + result.error.len());
             for i in result.deleted {
                 let path = build_rel_path(&self.core.root, &i.key);
                 batched_result.push((path, Ok(RpDelete::default().into())));
             }
-            // TODO: we should handle those errors with code.
             for i in result.error {
                 let path = build_rel_path(&self.core.root, &i.key);
 
                 // set the error kind and mark temporary if retryable
                 let (kind, retryable) =
                     parse_s3_error_code(i.code.as_str()).unwrap_or((ErrorKind::Unexpected, false));
-                let mut err = Error::new(kind, &format!("{i:?}"));
+                let mut err: Error = Error::new(kind, &format!("{i:?}"));
                 if retryable {
                     err = err.set_temporary();
                 }
 
                 batched_result.push((path, Err(err)));
             }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
 
         self.send(req).await
     }
 
     pub fn s3_put_object_request(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 use serde::Deserialize;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
-/// S3Error is the error returned by s3 service.
+/// WasabiError is the error returned by wasabi service.
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
-struct S3Error {
+struct WasabiError {
     code: String,
     message: String,
     resource: String,
     request_id: String,
 }
 
 /// Parse error response into Error.
@@ -50,34 +50,34 @@
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let (message, s3_err) = de::from_reader::<_, S3Error>(bs.clone().reader())
-        .map(|s3_err| (format!("{s3_err:?}"), Some(s3_err)))
+    let (message, wasabi_err) = de::from_reader::<_, WasabiError>(bs.clone().reader())
+        .map(|err| (format!("{err:?}"), Some(err)))
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
-    if let Some(s3_err) = s3_err {
-        (kind, retryable) = parse_s3_error_code(s3_err.code.as_str()).unwrap_or((kind, retryable));
+    if let Some(wasabi_err) = wasabi_err {
+        (kind, retryable) = parse_wasabi_error_code(&wasabi_err.code).unwrap_or((kind, retryable));
     }
 
     let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
 
-/// Returns the Errorkind of this code and whether the error is retryable.
+/// Returns the `Error kind` of this code and whether the error is retryable.
 /// All possible error code: <https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#ErrorCodeList>
-pub fn parse_s3_error_code(code: &str) -> Option<(ErrorKind, bool)> {
+pub fn parse_wasabi_error_code(code: &str) -> Option<(ErrorKind, bool)> {
     match code {
         // > Your socket connection to the server was not read from
         // > or written to within the timeout period."
         //
         // It's Ok for us to retry it again.
         "RequestTimeout" => Some((ErrorKind::Unexpected, true)),
         // > An internal error occurred. Try again.
@@ -114,15 +114,15 @@
   <Message>The resource you requested does not exist</Message>
   <Resource>/mybucket/myfoto.jpg</Resource>
   <RequestId>4442587FB7D0A2F9</RequestId>
 </Error>
 "#,
         );
 
-        let out: S3Error = de::from_reader(bs.reader()).expect("must success");
+        let out: WasabiError = de::from_reader(bs.reader()).expect("must success");
         println!("{out:?}");
 
         assert_eq!(out.code, "NoSuchKey");
         assert_eq!(out.message, "The resource you requested does not exist");
         assert_eq!(out.resource, "/mybucket/myfoto.jpg");
         assert_eq!(out.request_id, "4442587FB7D0A2F9");
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -50,22 +50,22 @@
             upload_id: None,
             parts: vec![],
             buffer: oio::VectorCursor::new(),
             buffer_size,
         }
     }
 
-    async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
+    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
         let mut req = self.core.s3_put_object_request(
             &self.path,
-            Some(bs.len()),
+            Some(size),
             self.op.content_type(),
             self.op.content_disposition(),
             self.op.cache_control(),
-            AsyncBody::Bytes(bs),
+            body,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
@@ -150,15 +150,17 @@
 #[async_trait]
 impl oio::Write for S3Writer {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let upload_id = match &self.upload_id {
             Some(upload_id) => upload_id,
             None => {
                 if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
-                    return self.write_oneshot(bs).await;
+                    return self
+                        .write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+                        .await;
                 } else {
                     let upload_id = self.initiate_upload().await?;
                     self.upload_id = Some(upload_id);
                     self.upload_id.as_deref().unwrap()
                 }
             }
         };
@@ -188,14 +190,25 @@
                 // write is re-enter safe.
                 self.buffer.pop();
                 Err(e)
             }
         }
     }
 
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        if self.op.content_length().unwrap_or_default() == size {
+            return self.write_oneshot(size, AsyncBody::Stream(s)).await;
+        } else {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "S3 does not support streaming multipart upload",
+            ));
+        }
+    }
+
     async fn abort(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
             return Ok(());
         };
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sftp/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 use std::cmp::min;
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::path::Path;
 use std::path::PathBuf;
-use std::time::Duration;
 
 use async_trait::async_trait;
 use futures::StreamExt;
 use log::debug;
 use openssh::KnownHosts;
 use openssh::SessionBuilder;
 use openssh_sftp_client::Sftp;
@@ -41,15 +40,14 @@
 
 /// SFTP services support. (only works on unix)
 ///
 /// Warning: Maximum number of file holdings is depending on the remote system configuration.
 ///
 /// For example, the default value is 255 in macOS, and 1024 in linux. If you want to open
 /// lots of files, you should pay attention to close the file after using it.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct SftpBuilder {
     endpoint: Option<String>,
     root: Option<String>,
     user: Option<String>,
     key: Option<String>,
@@ -75,14 +73,15 @@
             Some(endpoint.to_string())
         };
 
         self
     }
 
     /// set root path for sftp backend.
+    /// It uses the default directory set by the remote `sftp-server` as default.
     pub fn root(&mut self, root: &str) -> &mut Self {
         self.root = if root.is_empty() {
             None
         } else {
             Some(root.to_string())
         };
 
@@ -151,15 +150,15 @@
             None => return Err(Error::new(ErrorKind::ConfigInvalid, "user is empty")),
         };
 
         let root = self
             .root
             .clone()
             .map(|r| normalize_root(r.as_str()))
-            .unwrap_or(format!("/home/{}/", user));
+            .unwrap_or_default();
 
         let known_hosts_strategy = match &self.known_hosts_strategy {
             Some(v) => {
                 let v = v.to_lowercase();
                 if v == "strict" {
                     KnownHosts::Strict
                 } else if v == "accept" {
@@ -523,36 +522,36 @@
 
     #[cfg(target_os = "macos")]
     {
         let _ = std::fs::create_dir("/private/tmp/.opendal/");
         session.control_directory("/private/tmp/.opendal/");
     }
 
-    session.server_alive_interval(Duration::from_secs(5));
     session.known_hosts_check(known_hosts_strategy);
 
     let session = session.connect(&endpoint).await?;
 
     let sftp = Sftp::from_session(session, SftpOptions::default()).await?;
 
-    let mut fs = sftp.fs();
-    fs.set_cwd("/");
+    if !root.is_empty() {
+        let mut fs = sftp.fs();
 
-    let paths = Path::new(&root).components();
-    let mut current = PathBuf::from("/");
-    for p in paths {
-        current = current.join(p);
-        let res = fs.create_dir(p).await;
-
-        if let Err(e) = res {
-            // ignore error if dir already exists
-            if !is_sftp_protocol_error(&e) {
-                return Err(e.into());
+        let paths = Path::new(&root).components();
+        let mut current = PathBuf::new();
+        for p in paths {
+            current.push(p);
+            let res = fs.create_dir(p).await;
+
+            if let Err(e) = res {
+                // ignore error if dir already exists
+                if !is_sftp_protocol_error(&e) {
+                    return Err(e.into());
+                }
             }
+            fs.set_cwd(&current);
         }
-        fs.set_cwd(&current);
     }
 
     debug!("sftp connection created at {}", root);
 
     Ok(sftp)
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sftp/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/docs.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - [ ] ~~scan~~
 - [ ] ~~presign~~
 - [ ] blocking
 
 ## Configuration
 
 - `endpoint`: Set the endpoint for connection
-- `root`: Set the work directory for backend, default to `/home/$USER/`
+- `root`: Set the work directory for backend. It uses the default directory set by the remote `sftp-server` as default
 - `user`: Set the login user
 - `key`: Set the public key for login
 - `known_hosts_strategy`: Set the strategy for known hosts, default to `Strict`
 - `enable_copy`: Set whether the remote server has copy-file extension
 
 It doesn't support password login, you can use public key instead.
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sftp/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sftp/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sftp/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sftp/utils.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sftp/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,21 @@
 impl oio::Write for SftpWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.file.write_all(&bs).await?;
 
         Ok(())
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "SFTP does not support aborting writes",
         ))
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files 19% similar despite different names*

```diff
@@ -14,57 +14,68 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
+use std::str;
 
 use async_trait::async_trait;
 
 use crate::raw::adapters::kv;
 use crate::Builder;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Scheme;
 use crate::*;
 
+// https://github.com/spacejam/sled/blob/69294e59c718289ab3cb6bd03ac3b9e1e072a1e7/src/db.rs#L5
+const DEFAULT_TREE_ID: &str = r#"__sled__default"#;
+
 /// Sled service support.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct SledBuilder {
     /// That path to the sled data directory.
     datadir: Option<String>,
     root: Option<String>,
+    tree: Option<String>,
 }
 
 impl SledBuilder {
     /// Set the path to the sled data directory. Will create if not exists.
     pub fn datadir(&mut self, path: &str) -> &mut Self {
         self.datadir = Some(path.into());
         self
     }
 
     /// Set the root for sled.
     pub fn root(&mut self, path: &str) -> &mut Self {
         self.root = Some(path.into());
         self
     }
+
+    /// Set the tree for sled.
+    pub fn tree(&mut self, tree: &str) -> &mut Self {
+        self.tree = Some(tree.into());
+        self
+    }
 }
 
 impl Builder for SledBuilder {
     const SCHEME: Scheme = Scheme::Sled;
     type Accessor = SledBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
         let mut builder = SledBuilder::default();
 
         map.get("datadir").map(|v| builder.datadir(v));
         map.get("root").map(|v| builder.root(v));
+        map.get("tree").map(|v| builder.tree(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         let datadir_path = self.datadir.take().ok_or_else(|| {
             Error::new(ErrorKind::ConfigInvalid, "datadir is required but not set")
@@ -74,29 +85,43 @@
         let db = sled::open(&datadir_path).map_err(|e| {
             Error::new(ErrorKind::ConfigInvalid, "open db")
                 .with_context("service", Scheme::Sled)
                 .with_context("datadir", datadir_path.clone())
                 .set_source(e)
         })?;
 
+        // use "default" tree if not set
+        let tree_name = match self.tree.take() {
+            Some(tree) => tree,
+            None => DEFAULT_TREE_ID.to_string(),
+        };
+
+        let tree = db.open_tree(&tree_name).map_err(|e| {
+            Error::new(ErrorKind::ConfigInvalid, "open tree")
+                .with_context("service", Scheme::Sled)
+                .with_context("datadir", datadir_path.clone())
+                .with_context("tree", tree_name.clone())
+                .set_source(e)
+        })?;
+
         Ok(SledBackend::new(Adapter {
             datadir: datadir_path,
-            db,
+            tree,
         })
         .with_root(self.root.as_deref().unwrap_or_default()))
     }
 }
 
 /// Backend for sled services.
 pub type SledBackend = kv::Backend<Adapter>;
 
 #[derive(Clone)]
 pub struct Adapter {
     datadir: String,
-    db: sled::Db,
+    tree: sled::Tree,
 }
 
 impl Debug for Adapter {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut ds = f.debug_struct("Adapter");
         ds.field("path", &self.datadir);
         ds.finish()
@@ -120,43 +145,47 @@
     }
 
     async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
         self.blocking_get(path)
     }
 
     fn blocking_get(&self, path: &str) -> Result<Option<Vec<u8>>> {
-        Ok(self.db.get(path).map_err(parse_error)?.map(|v| v.to_vec()))
+        Ok(self
+            .tree
+            .get(path)
+            .map_err(parse_error)?
+            .map(|v| v.to_vec()))
     }
 
     async fn set(&self, path: &str, value: &[u8]) -> Result<()> {
         self.blocking_set(path, value)
     }
 
     fn blocking_set(&self, path: &str, value: &[u8]) -> Result<()> {
-        self.db.insert(path, value).map_err(parse_error)?;
+        self.tree.insert(path, value).map_err(parse_error)?;
 
         Ok(())
     }
 
     async fn delete(&self, path: &str) -> Result<()> {
         self.blocking_delete(path)
     }
 
     fn blocking_delete(&self, path: &str) -> Result<()> {
-        self.db.remove(path).map_err(parse_error)?;
+        self.tree.remove(path).map_err(parse_error)?;
 
         Ok(())
     }
 
     async fn scan(&self, path: &str) -> Result<Vec<String>> {
         self.blocking_scan(path)
     }
 
     fn blocking_scan(&self, path: &str) -> Result<Vec<String>> {
-        let it = self.db.scan_prefix(path).keys();
+        let it = self.tree.scan_prefix(path).keys();
         let mut res = Vec::default();
 
         for i in it {
             let bs = i.map_err(parse_error)?.to_vec();
 
             res.push(String::from_utf8(bs).map_err(|err| {
                 Error::new(ErrorKind::Unexpected, "store key is not valid utf-8 string")
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sled/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/sled/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 This service can be used to:
 
 - [x] stat
 - [x] read
 - [x] write
 - [x] create_dir
 - [x] delete
-- [ ] copy
-- [ ] rename
+- [x] copy
+- [x] rename
 - [ ] ~~list~~
-- [ ] scan
+- [x] scan
 - [ ] ~~presign~~
 - [x] blocking
 
 ## Configuration
 
 - `datadir`: Set the path to the sled data directory
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/supabase/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/supabase/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/supabase/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/error.rs`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,21 @@
 }
 
 /// Parse the supabase error type to the OpenDAL error type
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
-    let (mut kind, mut retryable) = (ErrorKind::Unexpected, false);
+    // Check HTTP status code first/
+    let (mut kind, mut retryable) = match parts.status.as_u16() {
+        500 | 502 | 503 | 504 => (ErrorKind::Unexpected, true),
+        _ => (ErrorKind::Unexpected, false),
+    };
+
+    // Than extrace the error message.
     let (message, _) = from_slice::<SupabaseError>(&bs)
         .map(|sb_err| {
             (kind, retryable) = parse_supabase_error(&sb_err);
             (format!("{sb_err:?}"), Some(sb_err))
         })
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/supabase/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/supabase/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,21 @@
         if bs.is_empty() {
             return Ok(());
         }
 
         self.upload(bs).await
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "The abort operation is not yet supported for Supabase backend",
         ))
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     type BlockingWriter = ();
     type Appender = ();
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
-        ma.set_scheme(crate::Scheme::VercelArtifacts)
+        ma.set_scheme(Scheme::VercelArtifacts)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
 
                 write: true,
 
                 ..Default::default()
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -15,55 +15,54 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::VercelArtifactsBackend;
+use super::backend::IpmfsBackend;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct VercelArtifactsWriter {
-    backend: VercelArtifactsBackend,
-    op: OpWrite,
+pub struct IpmfsWriter {
+    backend: IpmfsBackend,
 
     path: String,
 }
 
-impl VercelArtifactsWriter {
-    pub fn new(backend: VercelArtifactsBackend, op: OpWrite, path: String) -> Self {
-        VercelArtifactsWriter { backend, op, path }
+impl IpmfsWriter {
+    pub fn new(backend: IpmfsBackend, path: String) -> Self {
+        IpmfsWriter { backend, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for VercelArtifactsWriter {
+impl oio::Write for IpmfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self
-            .backend
-            .vercel_artifacts_put(
-                self.path.as_str(),
-                self.op.content_length().unwrap(),
-                AsyncBody::Bytes(bs),
-            )
-            .await?;
+        let resp = self.backend.ipmfs_write(&self.path, bs).await?;
 
         let status = resp.status();
 
         match status {
-            StatusCode::OK | StatusCode::ACCEPTED => {
+            StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 use reqsign::AwsConfig;
 use reqsign::AwsCredentialLoad;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
 
 use super::core::*;
 use super::error::parse_error;
+use super::error::parse_wasabi_error_code;
 use super::pager::WasabiPager;
 use super::writer::WasabiWriter;
 use crate::raw::*;
 use crate::*;
 
 /// Allow constructing correct region endpoint if user gives a global endpoint.
 static ENDPOINT_TEMPLATES: Lazy<HashMap<&'static str, &'static str>> = Lazy::new(|| {
@@ -1097,18 +1098,23 @@
                 let path = build_rel_path(&self.core.root, &i.key);
                 batched_result.push((path, Ok(RpDelete::default().into())));
             }
             // TODO: we should handle those errors with code.
             for i in result.error {
                 let path = build_rel_path(&self.core.root, &i.key);
 
-                batched_result.push((
-                    path,
-                    Err(Error::new(ErrorKind::Unexpected, &format!("{i:?}"))),
-                ));
+                // set the error kind and mark temporary if retryable
+                let (kind, retryable) =
+                    parse_wasabi_error_code(&i.code).unwrap_or((ErrorKind::Unexpected, false));
+                let mut err: Error = Error::new(kind, &format!("{i:?}"));
+                if retryable {
+                    err = err.set_temporary();
+                }
+
+                batched_result.push((path, Err(err)));
             }
 
             Ok(RpBatch::new(batched_result))
         } else {
             Err(parse_error(resp).await?)
         }
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files 27% similar despite different names*

```diff
@@ -13,76 +13,98 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use bytes::Buf;
 use http::Response;
-use http::StatusCode;
+use http::Uri;
 use quick_xml::de;
 use serde::Deserialize;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
-/// WasabiError is the error returned by wasabi service.
+/// S3Error is the error returned by s3 service.
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
-struct WasabiError {
+struct S3Error {
     code: String,
     message: String,
     resource: String,
     request_id: String,
 }
 
 /// Parse error response into Error.
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
-    let (mut kind, mut retryable) = match parts.status {
-        StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
-        StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
-            (ErrorKind::ConditionNotMatch, false)
-        }
-        StatusCode::INTERNAL_SERVER_ERROR
-        | StatusCode::BAD_GATEWAY
-        | StatusCode::SERVICE_UNAVAILABLE
-        | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
+    let (mut kind, mut retryable) = match parts.status.as_u16() {
+        403 => (ErrorKind::PermissionDenied, false),
+        404 => (ErrorKind::NotFound, false),
+        304 | 412 => (ErrorKind::ConditionNotMatch, false),
+        // Service like R2 could return 499 error with a message like:
+        // Client Disconnect, we should retry it.
+        499 => (ErrorKind::Unexpected, true),
+        500 | 502 | 503 | 504 => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let (message, wasabi_err) = de::from_reader::<_, WasabiError>(bs.clone().reader())
-        .map(|err| (format!("{err:?}"), Some(err)))
+    let (message, s3_err) = de::from_reader::<_, S3Error>(bs.clone().reader())
+        .map(|s3_err| (format!("{s3_err:?}"), Some(s3_err)))
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
-    // All possible error code: <https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#ErrorCodeList>
-    if let Some(wasabi_err) = wasabi_err {
-        (kind, retryable) = match wasabi_err.code.as_str() {
-            // > Your socket connection to the server was not read from
-            // > or written to within the timeout period."
-            //
-            // It's Ok for us to retry it again.
-            "RequestTimeout" => (ErrorKind::Unexpected, true),
-            _ => (kind, retryable),
-        }
+    if let Some(s3_err) = s3_err {
+        (kind, retryable) = parse_s3_error_code(s3_err.code.as_str()).unwrap_or((kind, retryable));
     }
 
     let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
 
     if retryable {
         err = err.set_temporary();
     }
 
+    if let Some(uri) = parts.extensions.get::<Uri>() {
+        err = err.with_context("uri", uri.to_string());
+    }
+
     Ok(err)
 }
 
+/// Returns the `Error kind` of this code and whether the error is retryable.
+/// All possible error code: <https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#ErrorCodeList>
+pub fn parse_s3_error_code(code: &str) -> Option<(ErrorKind, bool)> {
+    match code {
+        // > Your socket connection to the server was not read from
+        // > or written to within the timeout period."
+        //
+        // It's Ok for us to retry it again.
+        "RequestTimeout" => Some((ErrorKind::Unexpected, true)),
+        // > An internal error occurred. Try again.
+        "InternalError" => Some((ErrorKind::Unexpected, true)),
+        // > A conflicting conditional operation is currently in progress
+        // > against this resource. Try again.
+        "OperationAborted" => Some((ErrorKind::Unexpected, true)),
+        // > Please reduce your request rate.
+        //
+        // It's Ok to retry since later on the request rate may get reduced.
+        "SlowDown" => Some((ErrorKind::RateLimited, true)),
+        // > Service is unable to handle request.
+        //
+        // ServiceUnavailable is considered a retryable error because it typically
+        // indicates a temporary issue with the service or server, such as high load,
+        // maintenance, or an internal problem.
+        "ServiceUnavailable" => Some((ErrorKind::Unexpected, true)),
+        _ => None,
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
     /// Error response example is from https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html
     #[test]
     fn test_parse_error() {
@@ -94,15 +116,15 @@
   <Message>The resource you requested does not exist</Message>
   <Resource>/mybucket/myfoto.jpg</Resource>
   <RequestId>4442587FB7D0A2F9</RequestId>
 </Error>
 "#,
         );
 
-        let out: WasabiError = de::from_reader(bs.reader()).expect("must success");
+        let out: S3Error = de::from_reader(bs.reader()).expect("must success");
         println!("{out:?}");
 
         assert_eq!(out.code, "NoSuchKey");
         assert_eq!(out.message, "The resource you requested does not exist");
         assert_eq!(out.resource, "/mybucket/myfoto.jpg");
         assert_eq!(out.request_id, "4442587FB7D0A2F9");
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,21 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,21 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 5% similar despite different names*

```diff
@@ -25,32 +25,33 @@
 use http::Response;
 use http::StatusCode;
 use log::debug;
 use tokio::sync::OnceCell;
 
 use super::error::parse_error;
 use super::message::BooleanResp;
+use super::message::DirectoryListingWrapper;
 use super::message::FileStatusType;
 use super::message::FileStatusWrapper;
 use super::message::FileStatusesWrapper;
 use super::pager::WebhdfsPager;
 use super::writer::WebhdfsWriter;
 use crate::raw::*;
 use crate::*;
 
 const WEBHDFS_DEFAULT_ENDPOINT: &str = "http://127.0.0.1:9870";
 
 /// [WebHDFS](https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-hdfs/WebHDFS.html)'s REST API support.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct WebhdfsBuilder {
     root: Option<String>,
     endpoint: Option<String>,
     delegation: Option<String>,
+    disable_list_batch: bool,
 }
 
 impl Debug for WebhdfsBuilder {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Builder")
             .field("root", &self.root)
             .field("endpoint", &self.endpoint)
@@ -100,26 +101,40 @@
     /// If both are set, delegation token will be used.
     pub fn delegation(&mut self, delegation: &str) -> &mut Self {
         if !delegation.is_empty() {
             self.delegation = Some(delegation.to_string());
         }
         self
     }
+
+    /// Disable batch listing
+    ///
+    /// # Note
+    ///
+    /// When listing a directory, the backend will default to use batch listing.
+    /// If disable, the backend will list all files/directories in one request.
+    pub fn disable_list_batch(&mut self) -> &mut Self {
+        self.disable_list_batch = true;
+        self
+    }
 }
 
 impl Builder for WebhdfsBuilder {
     const SCHEME: Scheme = Scheme::Webhdfs;
     type Accessor = WebhdfsBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
         let mut builder = WebhdfsBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("delegation").map(|v| builder.delegation(v));
+        map.get("disable_list_batch")
+            .filter(|v| v == &"true")
+            .map(|_| builder.disable_list_batch());
 
         builder
     }
 
     /// build the backend
     ///
     /// # Note
@@ -155,28 +170,30 @@
 
         let backend = WebhdfsBackend {
             root,
             endpoint,
             auth,
             client,
             root_checker: OnceCell::new(),
+            disable_list_batch: self.disable_list_batch,
         };
 
         Ok(backend)
     }
 }
 
 /// Backend for WebHDFS service
 #[derive(Debug, Clone)]
 pub struct WebhdfsBackend {
     root: String,
     endpoint: String,
     auth: Option<String>,
     root_checker: OnceCell<()>,
 
+    pub disable_list_batch: bool,
     pub client: HttpClient,
 }
 
 impl WebhdfsBackend {
     /// create object or make a directory
     ///
     /// TODO: we should split it into mkdir and create
@@ -272,14 +289,44 @@
 
         let req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
         Ok(req)
     }
 
+    pub(super) fn webhdfs_list_status_batch_request(
+        &self,
+        path: &str,
+        start_after: &Option<String>,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        // if it's not the first time to call LISTSTATUS_BATCH, we will add &startAfter=<CHILD>
+        let start_after_param = match start_after {
+            Some(sa) if sa.is_empty() => String::new(),
+            Some(sa) => format!("&startAfter={}", sa),
+            None => String::new(),
+        };
+
+        let mut url = format!(
+            "{}/webhdfs/v1/{}?op=LISTSTATUS_BATCH{}",
+            self.endpoint,
+            percent_encode_path(&p),
+            start_after_param
+        );
+        if let Some(auth) = &self.auth {
+            url += format!("&{auth}").as_str();
+        }
+
+        let req = Request::get(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+        Ok(req)
+    }
+
     async fn webhdfs_read_file(
         &self,
         path: &str,
         range: BytesRange,
     ) -> Result<Response<IncomingAsyncBody>> {
         let req = self.webhdfs_open_request(path, &range).await?;
         self.client.send(req).await
@@ -485,34 +532,55 @@
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         if args.delimiter() != "/" {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "webhdfs only support delimiter `/`",
+                "WebHDFS only support delimiter `/`",
             ));
         }
 
         let path = path.trim_end_matches('/');
-        let req = self.webhdfs_list_status_request(path)?;
-
-        let resp = self.client.send(req).await?;
-        match resp.status() {
-            StatusCode::OK => {
-                let bs = resp.into_body().bytes().await?;
-                let file_statuses = serde_json::from_slice::<FileStatusesWrapper>(&bs)
-                    .map_err(new_json_deserialize_error)?
-                    .file_statuses
-                    .file_status;
 
-                let objects = WebhdfsPager::new(path, file_statuses);
-                Ok((RpList::default(), objects))
+        if !self.disable_list_batch {
+            let req = self.webhdfs_list_status_batch_request(path, &None)?;
+            let resp = self.client.send(req).await?;
+            match resp.status() {
+                StatusCode::OK => {
+                    let bs = resp.into_body().bytes().await?;
+                    let directory_listing = serde_json::from_slice::<DirectoryListingWrapper>(&bs)
+                        .map_err(new_json_deserialize_error)?
+                        .directory_listing;
+                    let file_statuses = directory_listing.partial_listing.file_statuses.file_status;
+                    let mut objects = WebhdfsPager::new(self.clone(), path, file_statuses);
+                    objects.set_remaining_entries(directory_listing.remaining_entries);
+                    Ok((RpList::default(), objects))
+                }
+                StatusCode::NOT_FOUND => {
+                    let objects = WebhdfsPager::new(self.clone(), path, vec![]);
+                    Ok((RpList::default(), objects))
+                }
+                _ => Err(parse_error(resp).await?),
             }
-            StatusCode::NOT_FOUND => {
-                let objects = WebhdfsPager::new(path, vec![]);
-                Ok((RpList::default(), objects))
+        } else {
+            let req = self.webhdfs_list_status_request(path)?;
+            let resp = self.client.send(req).await?;
+            match resp.status() {
+                StatusCode::OK => {
+                    let bs = resp.into_body().bytes().await?;
+                    let file_statuses = serde_json::from_slice::<FileStatusesWrapper>(&bs)
+                        .map_err(new_json_deserialize_error)?
+                        .file_statuses
+                        .file_status;
+                    let objects = WebhdfsPager::new(self.clone(), path, file_statuses);
+                    Ok((RpList::default(), objects))
+                }
+                StatusCode::NOT_FOUND => {
+                    let objects = WebhdfsPager::new(self.clone(), path, vec![]);
+                    Ok((RpList::default(), objects))
+                }
+                _ => Err(parse_error(resp).await?),
             }
-            _ => Err(parse_error(resp).await?),
         }
     }
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/docs.md` & `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 }
 
 fn parse_error_msg(parts: Parts, body: &str) -> Result<Error> {
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::UNAUTHORIZED | StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
         // passing invalid arguments will return BAD_REQUEST
-        // should be unretryable
+        // should be un-retryable
         StatusCode::BAD_REQUEST => (ErrorKind::Unexpected, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
@@ -77,14 +77,15 @@
 #[cfg(test)]
 mod tests {
     use bytes::Buf;
     use futures::stream;
     use serde_json::from_reader;
 
     use super::*;
+    use crate::raw::oio::into_stream;
 
     /// Error response example from https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Error%20Responses
     #[tokio::test]
     async fn test_parse_error() -> Result<()> {
         let ill_args = bytes::Bytes::from(
             r#"
 {
@@ -93,15 +94,20 @@
     "exception"    : "IllegalArgumentException",
     "javaClassName": "java.lang.IllegalArgumentException",
     "message"      : "Invalid value for webhdfs parameter \"permission\": ..."
   }
 }
     "#,
         );
-        let body = IncomingAsyncBody::new(Box::new(stream::iter(vec![Ok(ill_args.clone())])), None);
+        let body = IncomingAsyncBody::new(
+            Box::new(into_stream::from_futures_stream(stream::iter(vec![Ok(
+                ill_args.clone(),
+            )]))),
+            None,
+        );
         let resp = Response::builder()
             .status(StatusCode::BAD_REQUEST)
             .body(body)
             .unwrap();
 
         let err = parse_error(resp).await?;
         assert_eq!(err.kind(), ErrorKind::Unexpected);
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files 22% similar despite different names*

```diff
@@ -34,42 +34,59 @@
 #[serde(rename_all = "PascalCase")]
 pub(super) struct FileStatusesWrapper {
     pub file_statuses: FileStatuses,
 }
 
 #[derive(Debug, Deserialize)]
 #[serde(rename_all = "PascalCase")]
+pub(super) struct DirectoryListingWrapper {
+    pub directory_listing: DirectoryListing,
+}
+
+#[derive(Debug, Default, Deserialize)]
+#[serde(rename_all = "camelCase")]
+pub(super) struct DirectoryListing {
+    pub partial_listing: PartialListing,
+    pub remaining_entries: u32,
+}
+
+#[derive(Debug, Default, Deserialize)]
+#[serde(rename_all = "PascalCase")]
+pub(super) struct PartialListing {
+    pub file_statuses: FileStatuses,
+}
+
+#[derive(Debug, Default, Deserialize)]
+#[serde(rename_all = "PascalCase")]
 pub(super) struct FileStatuses {
     pub file_status: Vec<FileStatus>,
 }
 
-#[derive(Debug, Deserialize)]
+#[derive(Debug, Default, Deserialize)]
 #[serde(rename_all = "camelCase")]
 pub struct FileStatus {
     pub length: u64,
     pub modification_time: i64,
 
     pub path_suffix: String,
     #[serde(rename = "type")]
     pub ty: FileStatusType,
 }
 
-#[derive(Debug, Deserialize, PartialEq, Eq)]
+#[derive(Debug, Default, Deserialize, PartialEq, Eq)]
 #[serde(rename_all = "UPPERCASE")]
 pub enum FileStatusType {
     Directory,
+    #[default]
     File,
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
-    use crate::raw::oio::Page;
-    use crate::services::webhdfs::pager::WebhdfsPager;
-    use crate::EntryMode;
 
     #[test]
     fn test_file_status() {
         let json = r#"
 {
   "FileStatus":
   {
@@ -145,21 +162,88 @@
             "#;
 
         let file_statuses = serde_json::from_str::<FileStatusesWrapper>(json)
             .expect("must success")
             .file_statuses
             .file_status;
 
-        let mut pager = WebhdfsPager::new("listing/directory", file_statuses);
-        let mut entries = vec![];
-        while let Some(oes) = pager.next().await.expect("must success") {
-            entries.extend(oes);
-        }
-
-        entries.sort_by(|a, b| a.path().cmp(b.path()));
-        assert_eq!(entries.len(), 2);
-        assert_eq!(entries[0].path(), "listing/directory/a.patch");
-        assert_eq!(entries[0].mode(), EntryMode::FILE);
-        assert_eq!(entries[1].path(), "listing/directory/bar/");
-        assert_eq!(entries[1].mode(), EntryMode::DIR);
+        // we should check the value of FileStatusWrapper directly.
+        assert_eq!(file_statuses.len(), 2);
+        assert_eq!(file_statuses[0].length, 24930);
+        assert_eq!(file_statuses[0].modification_time, 1320171722771);
+        assert_eq!(file_statuses[0].path_suffix, "a.patch");
+        assert_eq!(file_statuses[0].ty, FileStatusType::File);
+        assert_eq!(file_statuses[1].length, 0);
+        assert_eq!(file_statuses[1].modification_time, 1320895981256);
+        assert_eq!(file_statuses[1].path_suffix, "bar");
+        assert_eq!(file_statuses[1].ty, FileStatusType::Directory);
+    }
+
+    #[tokio::test]
+    async fn test_list_status_batch() {
+        let json = r#"
+{
+    "DirectoryListing": {
+        "partialListing": {
+            "FileStatuses": {
+                "FileStatus": [
+                    {
+                        "accessTime": 0,
+                        "blockSize": 0,
+                        "childrenNum": 0,
+                        "fileId": 16387,
+                        "group": "supergroup",
+                        "length": 0,
+                        "modificationTime": 1473305882563,
+                        "owner": "andrew",
+                        "pathSuffix": "bardir",
+                        "permission": "755",
+                        "replication": 0,
+                        "storagePolicy": 0,
+                        "type": "DIRECTORY"
+                    },
+                    {
+                        "accessTime": 1473305896945,
+                        "blockSize": 1024,
+                        "childrenNum": 0,
+                        "fileId": 16388,
+                        "group": "supergroup",
+                        "length": 0,
+                        "modificationTime": 1473305896965,
+                        "owner": "andrew",
+                        "pathSuffix": "bazfile",
+                        "permission": "644",
+                        "replication": 3,
+                        "storagePolicy": 0,
+                        "type": "FILE"
+                    }
+                ]
+            }
+        },
+        "remainingEntries": 2
+    }
+}
+        "#;
+
+        let directory_listing = serde_json::from_str::<DirectoryListingWrapper>(json)
+            .expect("must success")
+            .directory_listing;
+
+        assert_eq!(directory_listing.remaining_entries, 2);
+        assert_eq!(
+            directory_listing
+                .partial_listing
+                .file_statuses
+                .file_status
+                .len(),
+            2
+        );
+        assert_eq!(
+            directory_listing.partial_listing.file_statuses.file_status[0].path_suffix,
+            "bardir"
+        );
+        assert_eq!(
+            directory_listing.partial_listing.file_statuses.file_status[1].path_suffix,
+            "bazfile"
+        );
     }
 }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.38.0/local_dependencies/opendal/src/services/cos/writer.rs`

 * *Files 13% similar despite different names*

```diff
@@ -11,61 +11,71 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::WebhdfsBackend;
+use super::core::CosCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct WebhdfsWriter {
-    backend: WebhdfsBackend,
+pub struct CosWriter {
+    core: Arc<CosCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl WebhdfsWriter {
-    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
-        WebhdfsWriter { backend, op, path }
+impl CosWriter {
+    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
+        CosWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WebhdfsWriter {
+impl oio::Write for CosWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let req = self
-            .backend
-            .webhdfs_create_object_request(
-                &self.path,
-                Some(bs.len()),
-                self.op.content_type(),
-                AsyncBody::Bytes(bs),
-            )
-            .await?;
+        let mut req = self.core.cos_put_object_request(
+            &self.path,
+            Some(bs.len()),
+            self.op.content_type(),
+            self.op.cache_control(),
+            AsyncBody::Bytes(bs),
+        )?;
+
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
+
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
+    }
+
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/appender.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/capability.rs`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,16 @@
     /// if operator supports read with override cache control natively, it will be true.
     pub read_with_override_cache_control: bool,
     /// if operator supports read with override content disposition natively, it will be true.
     pub read_with_override_content_disposition: bool,
 
     /// If operator supports write natively, it will be true.
     pub write: bool,
+    /// If operator supports write by sink a stream into, it will be true.
+    pub write_can_sink: bool,
     /// If operator supports write with without content length, it will
     /// be true.
     ///
     /// This feature also be called as `Unsized` write or streaming write.
     pub write_without_content_length: bool,
     /// If operator supports write with content type natively, it will be true.
     pub write_with_content_type: bool,
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/error.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/list.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 4% similar despite different names*

```diff
@@ -676,14 +676,110 @@
         let path = normalize_path(path);
 
         let _ = self.inner().blocking_delete(&path, OpDelete::new())?;
 
         Ok(())
     }
 
+    /// remove will remove files via the given paths.
+    ///
+    /// remove_via will remove files via the given vector iterators.
+    ///
+    /// # Notes
+    ///
+    /// We don't support batch delete now.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use anyhow::Result;
+    /// # use futures::io;
+    /// # use opendal::BlockingOperator;
+    /// # fn test(op: BlockingOperator) -> Result<()> {
+    /// let stream = vec!["abc".to_string(), "def".to_string()].into_iter();
+    /// op.remove_via(stream)?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub fn remove_via(&self, input: impl Iterator<Item = String>) -> Result<()> {
+        for path in input {
+            self.delete(&path)?;
+        }
+        Ok(())
+    }
+
+    /// # Notes
+    ///
+    /// We don't support batch delete now.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use anyhow::Result;
+    /// # use futures::io;
+    /// # use opendal::BlockingOperator;
+    /// # fn test(op: BlockingOperator) -> Result<()> {
+    /// op.remove(vec!["abc".to_string(), "def".to_string()])?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub fn remove(&self, paths: Vec<String>) -> Result<()> {
+        self.remove_via(paths.into_iter())?;
+
+        Ok(())
+    }
+
+    /// Remove the path and all nested dirs and files recursively.
+    ///
+    /// # Notes
+    ///
+    /// We don't support batch delete now.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use anyhow::Result;
+    /// # use futures::io;
+    /// # use opendal::BlockingOperator;
+    /// # fn test(op: BlockingOperator) -> Result<()> {
+    /// op.remove_all("path/to/dir")?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub fn remove_all(&self, path: &str) -> Result<()> {
+        let meta = match self.stat(path) {
+            Ok(metadata) => metadata,
+
+            Err(e) if e.kind() == ErrorKind::NotFound => return Ok(()),
+
+            Err(e) => return Err(e),
+        };
+
+        if meta.mode() != EntryMode::DIR {
+            return self.delete(path);
+        }
+
+        let obs = self.scan(path)?;
+
+        for v in obs {
+            match v {
+                Ok(entry) => {
+                    self.inner()
+                        .blocking_delete(entry.path(), OpDelete::new())?;
+                }
+                Err(e) => return Err(e),
+            }
+        }
+
+        // Remove the directory itself.
+        self.delete(path)?;
+
+        Ok(())
+    }
+
     /// List current dir path.
     ///
     /// This function will create a new handle to list entries.
     ///
     /// An error will be returned if path doesn't end with `/`.
     ///
     /// # Examples
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     /// ```
     pub fn via_map(scheme: Scheme, map: HashMap<String, String>) -> Result<Operator> {
         let op = match scheme {
             #[cfg(feature = "services-azblob")]
             Scheme::Azblob => Self::from_map::<services::Azblob>(map)?.finish(),
             #[cfg(feature = "services-azdfs")]
             Scheme::Azdfs => Self::from_map::<services::Azdfs>(map)?.finish(),
+            #[cfg(feature = "services-cacache")]
+            Scheme::Cacache => Self::from_map::<services::Cacache>(map)?.finish(),
             #[cfg(feature = "services-cos")]
             Scheme::Cos => Self::from_map::<services::Cos>(map)?.finish(),
             #[cfg(feature = "services-dashmap")]
             Scheme::Dashmap => Self::from_map::<services::Dashmap>(map)?.finish(),
             #[cfg(feature = "services-fs")]
             Scheme::Fs => Self::from_map::<services::Fs>(map)?.finish(),
             #[cfg(feature = "services-ftp")]
@@ -177,14 +179,16 @@
             Scheme::Ipfs => Self::from_map::<services::Ipfs>(map)?.finish(),
             #[cfg(feature = "services-ipmfs")]
             Scheme::Ipmfs => Self::from_map::<services::Ipmfs>(map)?.finish(),
             #[cfg(feature = "services-memcached")]
             Scheme::Memcached => Self::from_map::<services::Memcached>(map)?.finish(),
             #[cfg(feature = "services-memory")]
             Scheme::Memory => Self::from_map::<services::Memory>(map)?.finish(),
+            #[cfg(feature = "services-mini-moka")]
+            Scheme::MiniMoka => Self::from_map::<services::MiniMoka>(map)?.finish(),
             #[cfg(feature = "services-moka")]
             Scheme::Moka => Self::from_map::<services::Moka>(map)?.finish(),
             #[cfg(feature = "services-obs")]
             Scheme::Obs => Self::from_map::<services::Obs>(map)?.finish(),
             #[cfg(feature = "services-onedrive")]
             Scheme::Onedrive => Self::from_map::<services::Onedrive>(map)?.finish(),
             #[cfg(feature = "services-gdrive")]
@@ -207,14 +211,16 @@
             Scheme::VercelArtifacts => Self::from_map::<services::VercelArtifacts>(map)?.finish(),
             #[cfg(feature = "services-wasabi")]
             Scheme::Wasabi => Self::from_map::<services::Wasabi>(map)?.finish(),
             #[cfg(feature = "services-webdav")]
             Scheme::Webdav => Self::from_map::<services::Webdav>(map)?.finish(),
             #[cfg(feature = "services-webhdfs")]
             Scheme::Webhdfs => Self::from_map::<services::Webhdfs>(map)?.finish(),
+            #[cfg(feature = "services-redb")]
+            Scheme::Redb => Self::from_map::<services::Redb>(map)?.finish(),
             v => {
                 return Err(Error::new(
                     ErrorKind::Unsupported,
                     "scheme is not enabled or supported",
                 )
                 .with_context("scheme", v))
             }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     }
 
     pub(crate) fn from_inner(accessor: FusedAccessor) -> Self {
         let limit = accessor
             .info()
             .capability()
             .batch_max_operations
-            .unwrap_or(100);
+            .unwrap_or(1000);
         Self { accessor, limit }
     }
 
     pub(super) fn into_inner(self) -> FusedAccessor {
         self.accessor
     }
```

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/operator/operator_functions.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_functions.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/operator/operator_futures.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_futures.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.38.0/local_dependencies/opendal/src/types/scheme.rs`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 #[derive(Copy, Clone, Debug, PartialEq, Eq, Hash)]
 #[non_exhaustive]
 pub enum Scheme {
     /// [azblob][crate::services::Azblob]: Azure Storage Blob services.
     Azblob,
     /// [azdfs][crate::services::Azdfs]: Azure Data Lake Storage Gen2.
     Azdfs,
+    /// [cacache][crate::services::Cacache]: cacache backend support.
+    Cacache,
     /// [cos][crate::services::Cos]: Tencent Cloud Object Storage services.
     Cos,
     /// [dashmap][crate::services::Dashmap]: dashmap backend support.
     Dashmap,
     /// [fs][crate::services::Fs]: POSIX alike file system.
     Fs,
     /// [ftp][crate::services::Ftp]: FTP backend.
@@ -56,22 +58,26 @@
     Ipfs,
     /// [ipmfs][crate::services::Ipmfs]: IPFS mutable file system
     Ipmfs,
     /// [memcached][crate::services::Memcached]: Memcached service support.
     Memcached,
     /// [memory][crate::services::Memory]: In memory backend support.
     Memory,
+    /// [mini-moka][crate::services::MiniMoka]: Mini Moka backend support.
+    MiniMoka,
     /// [moka][crate::services::Moka]: moka backend support.
     Moka,
     /// [obs][crate::services::Obs]: Huawei Cloud OBS services.
     Obs,
     /// [onedrive][crate::services::Onedrive]: Microsoft OneDrive services.
     Onedrive,
     /// [gdrive][crate::services::Gdrive]: GoogleDrive services.
     Gdrive,
+    /// [dropbox][crate::services::Dropbox]: Dropbox services.
+    Dropbox,
     /// [oss][crate::services::Oss]: Aliyun Object Storage Services
     Oss,
     /// [redis][crate::services::Redis]: Redis services
     Redis,
     /// [rocksdb][crate::services::Rocksdb]: RocksDB services
     Rocksdb,
     /// [s3][crate::services::S3]: AWS S3 alike services.
@@ -86,14 +92,16 @@
     VercelArtifacts,
     /// [wasabi][crate::services::Wasabi]: Wasabi service
     Wasabi,
     /// [webdav][crate::services::Webdav]: WebDAV support.
     Webdav,
     /// [webhdfs][crate::services::Webhdfs]: WebHDFS RESTful API Services
     Webhdfs,
+    /// [redb][crate::services::Redb]: Redb Services
+    Redb,
     /// Custom that allow users to implement services outside of OpenDAL.
     ///
     /// # NOTE
     ///
     /// - Custom must not overwrite any existing services name.
     /// - Custom must be lowed cases.
     Custom(&'static str),
@@ -122,74 +130,81 @@
     type Err = Error;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         let s = s.to_lowercase();
         match s.as_str() {
             "azblob" => Ok(Scheme::Azblob),
             "azdfs" => Ok(Scheme::Azdfs),
+            "cacache" => Ok(Scheme::Cacache),
             "cos" => Ok(Scheme::Cos),
             "dashmap" => Ok(Scheme::Dashmap),
             "fs" => Ok(Scheme::Fs),
             "gcs" => Ok(Scheme::Gcs),
             "ghac" => Ok(Scheme::Ghac),
             "hdfs" => Ok(Scheme::Hdfs),
             "http" | "https" => Ok(Scheme::Http),
             "ftp" | "ftps" => Ok(Scheme::Ftp),
             "ipfs" | "ipns" => Ok(Scheme::Ipfs),
             "ipmfs" => Ok(Scheme::Ipmfs),
             "memcached" => Ok(Scheme::Memcached),
             "memory" => Ok(Scheme::Memory),
+            "mini_moka" => Ok(Scheme::MiniMoka),
             "moka" => Ok(Scheme::Moka),
             "obs" => Ok(Scheme::Obs),
             "redis" => Ok(Scheme::Redis),
             "rocksdb" => Ok(Scheme::Rocksdb),
             "s3" => Ok(Scheme::S3),
             "sled" => Ok(Scheme::Sled),
             "supabase" => Ok(Scheme::Supabase),
             "oss" => Ok(Scheme::Oss),
+            "vercel_artifacts" => Ok(Scheme::VercelArtifacts),
             "wasabi" => Ok(Scheme::Wasabi),
             "webdav" => Ok(Scheme::Webdav),
             "webhdfs" => Ok(Scheme::Webhdfs),
             _ => Ok(Scheme::Custom(Box::leak(s.into_boxed_str()))),
         }
     }
 }
 
 impl From<Scheme> for &'static str {
     fn from(v: Scheme) -> Self {
         match v {
             Scheme::Azblob => "azblob",
             Scheme::Azdfs => "azdfs",
+            Scheme::Cacache => "cacache",
             Scheme::Cos => "cos",
             Scheme::Dashmap => "dashmap",
             Scheme::Fs => "fs",
             Scheme::Gcs => "gcs",
             Scheme::Ghac => "ghac",
             Scheme::Hdfs => "hdfs",
             Scheme::Http => "http",
             Scheme::Ftp => "ftp",
             Scheme::Ipfs => "ipfs",
             Scheme::Ipmfs => "ipmfs",
             Scheme::Memcached => "memcached",
             Scheme::Memory => "memory",
+            Scheme::MiniMoka => "mini_moka",
             Scheme::Moka => "moka",
             Scheme::Obs => "obs",
             Scheme::Onedrive => "onedrive",
             Scheme::Gdrive => "gdrive",
+            Scheme::Dropbox => "dropbox",
             Scheme::Redis => "redis",
             Scheme::Rocksdb => "rocksdb",
             Scheme::S3 => "s3",
             Scheme::Sftp => "sftp",
             Scheme::Sled => "sled",
             Scheme::Supabase => "supabase",
             Scheme::VercelArtifacts => "vercel_artifacts",
             Scheme::Oss => "oss",
             Scheme::Wasabi => "wasabi",
             Scheme::Webdav => "webdav",
             Scheme::Webhdfs => "webhdfs",
+            Scheme::Redb => "redb",
             Scheme::Custom(v) => v,
         }
     }
 }
 
 impl From<Scheme> for String {
     fn from(v: Scheme) -> Self {
```

### Comparing `opendal-0.37.0/Cargo.toml` & `opendal-0.38.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.37.0"
+version= "0.38.0"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 futures = "0.3.28"
```

### Comparing `opendal-0.37.0/.gitignore` & `opendal-0.38.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/CONTRIBUTING.md` & `opendal-0.38.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Contributing
 
 - [Setup](#setup)
-  - [Using a devcontainer environment](#using-a-devcontainer-environment)
+  - [Using a dev container environment](#using-a-devcontainer-environment)
   - [Bring your own toolbox](#bring-your-own-toolbox)
 - [Prepare](#prepare)
 - [Build](#build)
 - [Test](#test)
 - [Docs](#docs)
 
 ## Setup
```

### Comparing `opendal-0.37.0/README.md` & `opendal-0.38.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # OpenDAL Python Binding
 
 Documentation: [main](https://opendal.apache.org/docs/python/)
 
 This crate intends to build a native python binding.
 
+![](https://github.com/apache/incubator-opendal/assets/5351546/87bbf6e5-f19e-449a-b368-3e283016c887)
+
 ## Installation
 
 ```bash
 pip install opendal
 ```
 
 ## Usage
```

### Comparing `opendal-0.37.0/benchmark/README.md` & `opendal-0.38.0/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/benchmark/async_opendal_benchmark.py` & `opendal-0.38.0/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.38.0/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/examples/object.ipynb` & `opendal-0.38.0/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/pyproject.toml` & `opendal-0.38.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/python/opendal/__init__.py` & `opendal-0.38.0/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/python/opendal/__init__.pyi` & `opendal-0.38.0/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/src/asyncio.rs` & `opendal-0.38.0/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/src/layers.rs` & `opendal-0.38.0/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/src/lib.rs` & `opendal-0.38.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/tests/binding.feature` & `opendal-0.38.0/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/tests/steps/binding.py` & `opendal-0.38.0/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.37.0/Cargo.lock` & `opendal-0.38.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 [[package]]
 name = "assert_cmd"
 version = "2.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86d6b683edf8d1119fe420a94f8a7e389239666aa72e65495d91c00462510151"
 dependencies = [
  "anstyle 1.0.0",
- "bstr",
+ "bstr 1.4.0",
  "doc-comment",
  "predicates 3.0.1",
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
@@ -433,29 +433,30 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bindgen"
-version = "0.60.1"
+version = "0.62.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "062dddbc1ba4aca46de6338e2bf87771414c335f7b2f2036e8f3e9befebf88e6"
+checksum = "c6720a8b7b2d39dd533285ed438d458f65b31b5c257e6ac7bb3d7e82844dd722"
 dependencies = [
  "bitflags 1.3.2",
  "cexpr",
  "clang-sys",
  "lazy_static",
  "lazycell",
  "peeking_take_while",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "bindgen"
 version = "0.65.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfdf7b466f9a4903edc73f95d6d2bcd5baf8ae620638762244d3f60143643cc5"
@@ -508,14 +509,23 @@
  "atomic-waker",
  "fastrand",
  "futures-lite",
 ]
 
 [[package]]
 name = "bstr"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "bstr"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
 dependencies = [
  "memchr",
  "once_cell",
  "regex-automata",
@@ -554,14 +564,41 @@
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
+name = "cacache"
+version = "11.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "11e3f7fcc57143528b55ff07ce71b4608d674d2929c2365f768c6c5bcaaa7a17"
+dependencies = [
+ "digest",
+ "either",
+ "futures",
+ "hex",
+ "libc",
+ "memmap2",
+ "miette",
+ "reflink",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "sha1",
+ "sha2",
+ "ssri",
+ "tempfile",
+ "thiserror",
+ "tokio",
+ "tokio-stream",
+ "walkdir",
+]
+
+[[package]]
 name = "camino"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c530edf18f37068ac2d977409ed5cd50d53d73bc653c7647b48eb78976ac9ae2"
 dependencies = [
  "serde",
 ]
@@ -714,14 +751,16 @@
 [[package]]
 name = "clap"
 version = "4.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a1f23fa97e1d1641371b51f35535cb26959b8e27ab50d167a8b996b5bada819"
 dependencies = [
  "clap_builder",
+ "clap_derive",
+ "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
 version = "4.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fdc5d93c358224b4d6867ef1356d740de2303e9892edc06c5340daeccd96bab"
@@ -731,14 +770,26 @@
  "bitflags 1.3.2",
  "clap_lex 0.4.1",
  "once_cell",
  "strsim",
 ]
 
 [[package]]
+name = "clap_derive"
+version = "4.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.16",
+]
+
+[[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
@@ -1522,14 +1573,32 @@
  "futures-channel",
  "futures-core",
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "governor"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c390a940a5d157878dd057c78680a33ce3415bcd05b4799509ea44210914b4d5"
+dependencies = [
+ "cfg-if",
+ "dashmap",
+ "futures",
+ "futures-timer",
+ "no-std-compat",
+ "nonzero_ext",
+ "parking_lot 0.12.1",
+ "quanta 0.9.3",
+ "rand 0.8.5",
+ "smallvec",
+]
+
+[[package]]
 name = "h2"
 version = "0.3.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5be7b54589b581f624f566bf5d8eb2bab1db736c51528720b6bd36b96b55924d"
 dependencies = [
  "bytes",
  "fnv",
@@ -2011,17 +2080,17 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -2046,14 +2115,25 @@
  "cc",
  "glob",
  "libc",
  "libz-sys",
 ]
 
 [[package]]
+name = "libtest-mimic"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d8de370f98a6cb8a4606618e53e802f93b094ddec0f96988eaec2c27e6e9ce7"
+dependencies = [
+ "clap 4.2.5",
+ "termcolor",
+ "threadpool",
+]
+
+[[package]]
 name = "libz-sys"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
 dependencies = [
  "cc",
  "pkg-config",
@@ -2107,14 +2187,32 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e24f1ad8321ca0e8a1e0ac13f23cb668e6f5466c2c57319f6a5cf1cc8e3b1c"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
+name = "lua-src"
+version = "546.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8cb00c1380f1b4b4928dd211c07301ffa34872a239e590bd3219d9e5b213face"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "luajit-src"
+version = "210.4.5+resty2cf5186"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "27b7992a40e602786272d84c6f2beca44a588ededcfd57b48ec6f82008a7cb97"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "mach"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b823e83b2affd8f40a9ee8c29dbc56404c1e34cd2710921f2801e2cf29527afa"
 dependencies = [
  "libc",
 ]
@@ -2223,14 +2321,23 @@
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
+name = "memmap2"
+version = "0.5.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
@@ -2254,20 +2361,58 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "miette"
+version = "5.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a236ff270093b0b67451bc50a509bd1bad302cb1d3c7d37d5efe931238581fa9"
+dependencies = [
+ "miette-derive",
+ "once_cell",
+ "thiserror",
+ "unicode-width",
+]
+
+[[package]]
+name = "miette-derive"
+version = "5.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4901771e1d44ddb37964565c654a3223ba41a594d02b8da471cc4464912b5cfa"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.16",
+]
+
+[[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
+name = "mini-moka"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5cafc5ec7807288595f9c20c86e6ce6d262b722f61e0547fe7e6e6e6451b58d5"
+dependencies = [
+ "crossbeam-channel",
+ "crossbeam-utils",
+ "dashmap",
+ "skeptic",
+ "smallvec",
+ "tagptr",
+ "triomphe",
+]
+
+[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "minitrace"
@@ -2315,29 +2460,57 @@
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "mlua"
+version = "0.8.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07366ed2cd22a3b000aed076e2b68896fb46f06f1f5786c5962da73c0af01577"
+dependencies = [
+ "bstr 0.2.17",
+ "cc",
+ "lua-src",
+ "luajit-src",
+ "mlua_derive",
+ "num-traits",
+ "once_cell",
+ "pkg-config",
+ "rustc-hash",
+]
+
+[[package]]
+name = "mlua_derive"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9214e60d3cf1643013b107330fcd374ccec1e4ba1eef76e7e5da5e8202e71c0"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "moka"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b6446f16d504e3d575df79cabb11bfbe9f24b17e9562d964a815db7b28ae3ec"
 dependencies = [
  "async-io",
  "async-lock",
  "crossbeam-channel",
  "crossbeam-epoch",
  "crossbeam-utils",
  "futures-util",
  "num_cpus",
  "once_cell",
  "parking_lot 0.12.1",
- "quanta",
+ "quanta 0.10.1",
  "rustc_version",
  "scheduled-thread-pool",
  "skeptic",
  "smallvec",
  "tagptr",
  "thiserror",
  "triomphe",
@@ -2422,24 +2595,36 @@
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
+name = "no-std-compat"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b93853da6d84c2e3c7d730d6473e8817692dd89be387eb01b94d7f108ecb5b8c"
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
+name = "nonzero_ext"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38bf9645c8b145698bb0b18a4637dcacbc421ea49bef2317e4fd8065a387cf21"
+
+[[package]]
 name = "normalize-line-endings"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61807f77802ff30975e01f4f071c8ba10c022052f98b3294119f3e615d13e5be"
 
 [[package]]
 name = "nu-ansi-term"
@@ -2529,15 +2714,15 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "anyhow",
  "axum",
  "chrono",
  "clap 4.2.5",
  "dirs 5.0.1",
  "futures",
@@ -2572,27 +2757,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.2.5",
  "dirs 5.0.1",
  "env_logger",
  "futures",
@@ -2615,39 +2800,43 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
  "bb8",
  "bytes",
+ "cacache",
  "chrono",
  "criterion",
  "dashmap",
  "dirs 5.0.1",
  "dotenvy",
  "flagset",
  "futures",
+ "governor",
  "hdrs",
  "http",
  "hyper",
  "lazy-regex",
+ "libtest-mimic",
  "log",
  "madsim",
  "md-5",
  "metrics",
+ "mini-moka",
  "minitrace",
  "moka",
  "once_cell",
  "openssh",
  "openssh-sftp-client",
  "opentelemetry 0.19.0",
  "opentelemetry-jaeger",
@@ -2656,14 +2845,15 @@
  "percent-encoding",
  "pin-project",
  "pretty_assertions",
  "prometheus",
  "prost",
  "quick-xml 0.27.1",
  "rand 0.8.5",
+ "redb",
  "redis",
  "reqsign",
  "reqwest",
  "rocksdb",
  "serde",
  "serde_json",
  "sha2",
@@ -2676,47 +2866,70 @@
  "tracing-subscriber",
  "uuid",
  "wiremock",
 ]
 
 [[package]]
 name = "opendal-c"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "bytes",
  "cbindgen",
  "opendal",
 ]
 
 [[package]]
+name = "opendal-dotnet"
+version = "0.1.0"
+dependencies = [
+ "opendal",
+]
+
+[[package]]
+name = "opendal-hs"
+version = "0.1.0"
+dependencies = [
+ "chrono",
+ "opendal",
+]
+
+[[package]]
 name = "opendal-java"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "anyhow",
  "jni",
  "num_cpus",
  "once_cell",
  "opendal",
  "tokio",
 ]
 
 [[package]]
+name = "opendal-lua"
+version = "0.1.0"
+dependencies = [
+ "mlua",
+ "opendal",
+]
+
+[[package]]
 name = "opendal-nodejs"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.37.0"
+version = "0.38.0"
 dependencies = [
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
 ]
@@ -3398,15 +3611,15 @@
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot 0.12.1",
- "pyo3-build-config",
+ "pyo3-build-config 0.18.3",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-asyncio"
@@ -3428,21 +3641,31 @@
 checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
+name = "pyo3-build-config"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
 name = "pyo3-ffi"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
- "pyo3-build-config",
+ "pyo3-build-config 0.18.3",
 ]
 
 [[package]]
 name = "pyo3-macros"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
@@ -3462,14 +3685,30 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quanta"
+version = "0.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "20afe714292d5e879d8b12740aa223c6a88f118af41870e8b6196e39a02238a8"
+dependencies = [
+ "crossbeam-utils",
+ "libc",
+ "mach",
+ "once_cell",
+ "raw-cpuid",
+ "wasi 0.10.0+wasi-snapshot-preview1",
+ "web-sys",
+ "winapi",
+]
+
+[[package]]
+name = "quanta"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e31331286705f455e56cca62e0e717158474ff02b7936c1fa596d983f4ae27"
 dependencies = [
  "crossbeam-utils",
  "libc",
  "mach",
@@ -3624,28 +3863,28 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "rb-sys"
-version = "0.9.72"
+version = "0.9.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e36bdb8be5f395264fb4345a5f6c13dac307ed3be3bccf6305b57835981c605"
+checksum = "91447d8cbb45afb5c915bad4dd44bd4b4e9be37648122409ceca75302cb81683"
 dependencies = [
  "rb-sys-build",
 ]
 
 [[package]]
 name = "rb-sys-build"
-version = "0.9.72"
+version = "0.9.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b56f8993adac385ed6208f0dc62f99181eb0676dea50bac7bc3d36a86bb9429b"
+checksum = "20673c1cfbd57b2db6c066b796352f07d241c45b210fd15b269dec54fa240380"
 dependencies = [
- "bindgen 0.60.1",
+ "bindgen 0.62.0",
  "lazy_static",
  "proc-macro2",
  "quote",
  "regex",
  "shell-words",
  "syn 1.0.109",
 ]
@@ -3653,14 +3892,24 @@
 [[package]]
 name = "rb-sys-env"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a35802679f07360454b418a5d1735c89716bde01d35b1560fc953c1415a0b3bb"
 
 [[package]]
+name = "redb"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89ccfb694235b9b5214d32756192abe324083e49363f29bc7c91a69854effe4c"
+dependencies = [
+ "libc",
+ "pyo3-build-config 0.19.0",
+]
+
+[[package]]
 name = "redis"
 version = "0.22.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa8455fa3621f6b41c514946de66ea0531f57ca017b2e6c7cc368035ea5b46df"
 dependencies = [
  "arc-swap",
  "async-trait",
@@ -3695,14 +3944,24 @@
 dependencies = [
  "getrandom 0.2.8",
  "redox_syscall",
  "thiserror",
 ]
 
 [[package]]
+name = "reflink"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc585ec28b565b4c28977ce8363a6636cedc280351ba25a7915f6c9f37f68cbe"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "regex"
 version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
 dependencies = [
  "aho-corasick",
  "memchr",
@@ -4130,14 +4389,25 @@
  "form_urlencoded",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "sha-1"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f5058ada175748e33390e40e872bd0fe59a19f265d0158daa551c5a88a76009c"
+dependencies = [
+ "cfg-if",
+ "cpufeatures",
+ "digest",
+]
+
+[[package]]
 name = "sha1"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f04293dc80c3993519f2d7f6f511707ee7094fe0c6d3406feb330cdb3540eba3"
 dependencies = [
  "cfg-if",
  "cpufeatures",
@@ -4345,14 +4615,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be3c6519de7ca611f71ef7e8a56eb57aa1c818fecb5242d0a0f39c83776c210c"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "ssri"
+version = "9.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b5327a6eb28e137e180380169adeae3ac6128438ca1e8a8dc80118f3d1812cbd"
+dependencies = [
+ "base64 0.21.0",
+ "digest",
+ "hex",
+ "miette",
+ "serde",
+ "sha-1",
+ "sha2",
+ "thiserror",
+ "xxhash-rust",
+]
+
+[[package]]
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
 name = "strsim"
@@ -4652,14 +4939,25 @@
 checksum = "e0d409377ff5b1e3ca6437aa86c1eb7d40c134bfec254e44c830defa92669db5"
 dependencies = [
  "rustls 0.21.1",
  "tokio",
 ]
 
 [[package]]
+name = "tokio-stream"
+version = "0.1.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
+dependencies = [
+ "futures-core",
+ "pin-project-lite",
+ "tokio",
+]
+
+[[package]]
 name = "tokio-util"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
@@ -5428,14 +5726,20 @@
  "regex",
  "serde",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
+name = "xxhash-rust"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "735a71d46c4d68d71d4b24d03fdc2b98e38cea81730595801db779c04fe80d70"
+
+[[package]]
 name = "yansi"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
 [[package]]
 name = "zeroize"
```

### Comparing `opendal-0.37.0/PKG-INFO` & `opendal-0.38.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.37.0
+Version: 0.38.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: gevent ; extra == 'benchmark'
 Requires-Dist: greenify ; extra == 'benchmark'
 Requires-Dist: greenlet ; extra == 'benchmark'
 Requires-Dist: boto3 ; extra == 'benchmark'
@@ -28,14 +28,16 @@
 
 # OpenDAL Python Binding
 
 Documentation: [main](https://opendal.apache.org/docs/python/)
 
 This crate intends to build a native python binding.
 
+![](https://github.com/apache/incubator-opendal/assets/5351546/87bbf6e5-f19e-449a-b368-3e283016c887)
+
 ## Installation
 
 ```bash
 pip install opendal
 ```
 
 ## Usage
```

