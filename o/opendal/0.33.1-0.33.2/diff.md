# Comparing `tmp/opendal-0.33.1.tar.gz` & `tmp/opendal-0.33.2.tar.gz`

## Comparing `opendal-0.33.1.tar` & `opendal-0.33.2.tar`

### file list

```diff
@@ -1,253 +1,258 @@
--rw-r--r--   0        0        0     5737 1970-01-01 00:00:00.000000 opendal-0.33.1/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    65426 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1256 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6635 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2438 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1832 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1290 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     6142 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10879 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     3172 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
--rw-r--r--   0     1001      123     4478 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    23435 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6746 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    20940 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9888 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    17355 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13556 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    51478 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13497 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    31779 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12877 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2205 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    13882 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    24230 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    37745 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    12402 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3844 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3001 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    19037 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123     9830 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1181 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1548 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     1934 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     6512 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5578 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3394 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    10427 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2025 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11983 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1950 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     8881 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15397 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4148 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4577 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2001 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9182 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6861 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5198 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     4081 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6387 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    27973 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123    10124 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    10574 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     5820 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2079 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    16278 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     9557 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3519 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2736 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     4046 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    23347 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3092 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    16606 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4206 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     1900 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    17843 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    11763 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3462 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10014 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6224 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123    20642 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2375 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    15656 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2461 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    15962 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1825 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    16861 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     8716 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1834 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     1074 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
--rw-r--r--   0     1001      123     4713 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123    10057 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4337 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     3459 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     7999 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    13617 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     7436 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3442 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2057 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    21480 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    24192 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3357 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      896 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6946 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10637 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5664 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    39561 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28456 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     3734 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7324 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7529 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123     5518 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123    38885 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29663 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     3711 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2666 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20511 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2560 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2066 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19374 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2452 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2076 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     3368 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6381 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    12002 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     6197 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    15166 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1511 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    24145 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3067 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    42718 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123    10788 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9569 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     5852 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    10696 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.33.1/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-04-25 15:52:38.000000 opendal-0.33.1/.gitignore
--rw-r--r--   0     1001      123      982 2023-04-25 15:52:38.000000 opendal-0.33.1/README.md
--rw-r--r--   0     1001      123      765 2023-04-25 15:52:38.000000 opendal-0.33.1/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-04-25 15:52:38.000000 opendal-0.33.1/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-04-25 15:52:38.000000 opendal-0.33.1/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-04-25 15:52:38.000000 opendal-0.33.1/examples/object.ipynb
--rw-r--r--   0     1001      123     1665 2023-04-25 15:52:38.000000 opendal-0.33.1/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-04-25 15:52:38.000000 opendal-0.33.1/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-04-25 15:52:38.000000 opendal-0.33.1/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11963 2023-04-25 15:52:38.000000 opendal-0.33.1/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-04-25 15:52:38.000000 opendal-0.33.1/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-04-25 15:52:38.000000 opendal-0.33.1/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-04-25 15:52:38.000000 opendal-0.33.1/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-04-25 15:52:38.000000 opendal-0.33.1/tests/steps/binding.py
--rw-r--r--   0     1001      123   117424 2023-04-25 15:52:38.000000 opendal-0.33.1/Cargo.lock
--rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.33.1/PKG-INFO
+-rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 opendal-0.33.2/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    66617 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1256 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6635 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2438 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1832 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1290 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10879 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     4478 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    23435 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6746 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    20940 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9888 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17355 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    13556 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    51478 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13497 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    31779 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12877 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2205 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13882 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    24230 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    37745 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    12402 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3844 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3001 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    19037 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123     9830 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1181 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1548 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     6512 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5578 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3394 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    11165 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2025 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11983 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1950 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     8881 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15397 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4148 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4577 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2001 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10680 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9182 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6861 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5198 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     4081 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6387 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    29068 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123    10124 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    11623 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     5870 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2079 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    16278 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     9557 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3519 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2736 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     4046 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    23347 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3092 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    16606 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4206 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     1900 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    19847 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    15836 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3512 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10592 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6187 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123    20642 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2375 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    15803 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2461 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    16169 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1875 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    16861 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     8716 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1834 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     1074 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
+-rw-r--r--   0     1001      123     4713 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123    10057 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4337 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     3584 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     7999 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    13922 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     7436 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3492 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2057 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    21785 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    24192 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3407 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6946 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10637 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5664 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    39656 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28367 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     3734 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7387 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7530 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123     5518 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123     8024 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/backend.rs
+-rw-r--r--   0     1001      123     5963 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/core.rs
+-rw-r--r--   0     1001      123     2365 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/error.rs
+-rw-r--r--   0     1001      123      894 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/mod.rs
+-rw-r--r--   0     1001      123     2382 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/writer.rs
+-rw-r--r--   0     1001      123    39009 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29663 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     3711 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2666 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20511 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2560 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2066 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19374 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2076 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     3368 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6381 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12002 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     6197 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    16557 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1511 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    24145 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123     8731 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3067 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    42718 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123    10788 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9569 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     6030 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    10696 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.33.2/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-04-27 13:47:39.000000 opendal-0.33.2/.gitignore
+-rw-r--r--   0     1001      123      982 2023-04-27 13:47:39.000000 opendal-0.33.2/README.md
+-rw-r--r--   0     1001      123      765 2023-04-27 13:47:39.000000 opendal-0.33.2/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-04-27 13:47:39.000000 opendal-0.33.2/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-04-27 13:47:39.000000 opendal-0.33.2/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-04-27 13:47:39.000000 opendal-0.33.2/examples/object.ipynb
+-rw-r--r--   0     1001      123     1665 2023-04-27 13:47:39.000000 opendal-0.33.2/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-04-27 13:47:39.000000 opendal-0.33.2/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-04-27 13:47:39.000000 opendal-0.33.2/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123    11963 2023-04-27 13:47:39.000000 opendal-0.33.2/src/asyncio.rs
+-rw-r--r--   0     1001      123     3311 2023-04-27 13:47:39.000000 opendal-0.33.2/src/layers.rs
+-rw-r--r--   0     1001      123    13929 2023-04-27 13:47:39.000000 opendal-0.33.2/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-04-27 13:47:39.000000 opendal-0.33.2/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-04-27 13:47:39.000000 opendal-0.33.2/tests/steps/binding.py
+-rw-r--r--   0     1001      123   117461 2023-04-27 13:47:39.000000 opendal-0.33.2/Cargo.lock
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.33.2/PKG-INFO
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/Cargo.toml` & `opendal-0.33.2/local_dependencies/opendal/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.33.1"
+version= "0.33.2"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -130,14 +130,15 @@
 services-rocksdb = ["dep:rocksdb"]
 services-s3 = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-sled = ["dep:sled"]
+services-supabase = []
 services-wasabi = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-webdav = []
 services-webhdfs = []
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.33.2/local_dependencies/opendal/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,41 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.33.2] - 2023-04-27
+
+### Added
+
+- feat(core): add test for `stat_with_if_none_match` (#2122)
+- feat(services/gcs): Add start-after support for list (#2107)
+- feat(services/azblob): Add supporting presign (#2120)
+- feat(services/gcs): Add supporting presign support (#2126)
+- feat(java): connect rust async/await with java future (#2112)
+- docs: add hdfs classpath related troubleshoot (#2130)
+- fix(clippy): suppress dead_code check (#2135)
+- feat(core): Add `cache-control` to Metadata (#2136)
+- fix(services/gcs): Remove HOST header to avoid gcs RESET connection (#2139)
+- test(core): test for `write_with_cache_control` (#2131)
+- test(core): test for `write_with_content_type` (#2140)
+- test(core): test for `read_with_if_none_match` (#2141)
+- feat(services/supabase): Add read/write/stat support for supabase (#2119)
+
+### Docs
+
+- docs: add hdfs classpath related troubleshoot (#2130)
+
+### CI
+
+-  ci: Mark job as skipped if owner is not apache (#2128)
+- ci: Enable native-tls to test gcs presign for workaround (#2138)
+
 ## [v0.33.1] - 2023-04-25
 
 ### Added
 
 - feat: Add behavior test for read_with_if_match & stat_with_if_match (#2088)
 - feat(tests): Add fuzz test for writer without content length (#2100)
 - feat: add if_none_match support for obs (#2103)
@@ -1981,14 +2008,16 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.33.2]: https://github.com/apache/incubator-opendal/compare/v0.33.1...v0.33.2
+[v0.33.1]: https://github.com/apache/incubator-opendal/compare/v0.33.0...v0.33.1
 [v0.33.0]: https://github.com/apache/incubator-opendal/compare/v0.32.0...v0.33.0
 [v0.32.0]: https://github.com/apache/incubator-opendal/compare/v0.31.1...v0.32.0
 [v0.31.1]: https://github.com/apache/incubator-opendal/compare/v0.31.0...v0.31.1
 [v0.31.0]: https://github.com/apache/incubator-opendal/compare/v0.30.5...v0.31.0
 [v0.30.5]: https://github.com/apache/incubator-opendal/compare/v0.30.4...v0.30.5
 [v0.30.4]: https://github.com/apache/incubator-opendal/compare/v0.30.3...v0.30.4
 [v0.30.3]: https://github.com/apache/incubator-opendal/compare/v0.30.2...v0.30.3
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.33.2/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/README.md` & `opendal-0.33.2/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.33.2/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.33.2/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.33.2/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.33.2/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.33.2/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/examples/object.rs` & `opendal-0.33.2/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.33.2/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/features.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.33.2/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.33.2/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/complete.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/logging.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/retry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.33.2/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/lib.rs` & `opendal-0.33.2/local_dependencies/opendal/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -85,13 +85,13 @@
     /// This is not a real test case.
     ///
     /// We assert our public structs here to make sure we don't introduce
     /// unexpected struct/enum size change.
     #[test]
     fn assert_size() {
         assert_eq!(24, size_of::<Operator>());
-        assert_eq!(216, size_of::<Entry>());
-        assert_eq!(192, size_of::<Metadata>());
+        assert_eq!(240, size_of::<Entry>());
+        assert_eq!(216, size_of::<Metadata>());
         assert_eq!(1, size_of::<EntryMode>());
         assert_eq!(24, size_of::<Scheme>());
     }
 }
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 // under the License.
 
 use base64::engine::general_purpose;
 use base64::Engine;
 use chrono::DateTime;
 use chrono::Utc;
 use http::header::HeaderName;
+use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
 use http::header::ETAG;
 use http::header::LAST_MODIFIED;
 use http::header::LOCATION;
@@ -52,14 +53,34 @@
             )
             .with_operation("http_util::parse_location")
             .set_source(e)
         })?)),
     }
 }
 
+/// Parse cache control from header map.
+///
+/// # Note
+///
+/// The returned value is the raw string of `cache-control` header,
+/// maybe `no-cache`, `max-age=3600`, etc.
+pub fn parse_cache_control(headers: &HeaderMap) -> Result<Option<&str>> {
+    match headers.get(CACHE_CONTROL) {
+        None => Ok(None),
+        Some(v) => Ok(Some(v.to_str().map_err(|e| {
+            Error::new(
+                ErrorKind::Unexpected,
+                "header value has to be valid utf-8 string",
+            )
+            .with_operation("http_util::parse_cache_control")
+            .set_source(e)
+        })?)),
+    }
+}
+
 /// Parse content length from header map.
 pub fn parse_content_length(headers: &HeaderMap) -> Result<Option<u64>> {
     match headers.get(CONTENT_LENGTH) {
         None => Ok(None),
         Some(v) => Ok(Some(
             v.to_str()
                 .map_err(|e| {
@@ -189,14 +210,18 @@
     let mode = if path.ends_with('/') {
         EntryMode::DIR
     } else {
         EntryMode::FILE
     };
     let mut m = Metadata::new(mode);
 
+    if let Some(v) = parse_cache_control(headers)? {
+        m.set_cache_control(v);
+    }
+
     if let Some(v) = parse_content_length(headers)? {
         m.set_content_length(v);
     }
 
     if let Some(v) = parse_content_type(headers)? {
         m.set_content_type(v);
     }
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.33.2/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
 /// - [x] copy
 /// - [x] list
 /// - [x] scan
-/// - [ ] presign
+/// - [x] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
 /// - `root`: Set the work dir for backend.
 /// - `container`: Set the container name for backend.
 /// - `endpoint`: Set the endpoint for backend.
@@ -399,14 +399,15 @@
                 container: self.container.clone(),
 
                 client,
                 loader: cred_loader,
                 signer,
                 batch_signer,
             }),
+            has_sas_token: self.sas_token.is_some(),
         })
     }
 }
 
 fn infer_storage_name_from_endpoint(endpoint: &str) -> Option<String> {
     let endpoint: &str = endpoint
         .strip_prefix("http://")
@@ -431,14 +432,15 @@
     }
 }
 
 /// Backend for azblob services.
 #[derive(Debug, Clone)]
 pub struct AzblobBackend {
     core: Arc<AzblobCore>,
+    has_sas_token: bool,
 }
 
 #[async_trait]
 impl Accessor for AzblobBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = AzblobWriter;
@@ -459,22 +461,23 @@
                 read: true,
                 read_can_next: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
-                write_with_content_type: true,
                 write_with_cache_control: true,
+                write_with_content_type: true,
 
                 delete: true,
                 create_dir: true,
                 list: true,
                 scan: true,
                 copy: true,
+                presign: self.has_sas_token,
                 batch: true,
                 batch_max_operations: Some(AZBLOB_BATCH_LIMIT),
                 ..Default::default()
             });
 
         am
     }
@@ -602,14 +605,44 @@
             "".to_string(),
             args.limit(),
         );
 
         Ok((RpScan::default(), op))
     }
 
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        let mut req = match args.operation() {
+            PresignOperation::Stat(v) => {
+                self.core
+                    .azblob_head_blob_request(path, v.if_none_match(), v.if_match())?
+            }
+            PresignOperation::Read(v) => self.core.azblob_get_blob_request(
+                path,
+                v.range(),
+                v.if_none_match(),
+                v.if_match(),
+                v.override_content_disposition(),
+            )?,
+            PresignOperation::Write(_) => {
+                self.core
+                    .azblob_put_blob_request(path, None, None, None, AsyncBody::Empty)?
+            }
+        };
+
+        self.core.sign_query(&mut req).await?;
+
+        let (parts, _) = req.into_parts();
+
+        Ok(RpPresign::new(PresignedRequest::new(
+            parts.method,
+            parts.uri,
+            parts.headers,
+        )))
+    }
+
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         let ops = args.into_operation();
         let paths = ops.into_iter().map(|(p, _)| p).collect::<Vec<_>>();
         if paths.len() > AZBLOB_BATCH_LIMIT {
             return Err(Error::new(
                 ErrorKind::Unsupported,
                 "batch delete limit exceeded",
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 use std::fmt;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 use std::str::FromStr;
 
 use http::header::HeaderName;
-use http::header::CACHE_CONTROL;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use http::Uri;
@@ -37,14 +36,15 @@
 use super::batch::BatchDeleteRequestBuilder;
 use crate::raw::*;
 use crate::*;
 
 mod constants {
     pub const X_MS_BLOB_TYPE: &str = "x-ms-blob-type";
     pub const X_MS_COPY_SOURCE: &str = "x-ms-copy-source";
+    pub const X_MS_BLOB_CACHE_CONTROL: &str = "x-ms-blob-cache-control";
 }
 
 pub struct AzblobCore {
     pub container: String,
     pub root: String,
     pub endpoint: String,
 
@@ -78,14 +78,22 @@
             Err(Error::new(
                 ErrorKind::ConfigInvalid,
                 "no valid credential found",
             ))
         }
     }
 
+    pub async fn sign_query<T>(&self, req: &mut Request<T>) -> Result<()> {
+        let cred = self.load_credential().await?;
+
+        self.signer
+            .sign_query(req, &cred)
+            .map_err(new_request_sign_error)
+    }
+
     pub async fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
         let cred = self.load_credential().await?;
         self.signer.sign(req, &cred).map_err(new_request_sign_error)
     }
 
     async fn batch_sign<T>(&self, req: &mut Request<T>) -> Result<()> {
         let cred = self.load_credential().await?;
@@ -97,22 +105,22 @@
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 }
 
 impl AzblobCore {
-    pub async fn azblob_get_blob(
+    pub fn azblob_get_blob_request(
         &self,
         path: &str,
         range: BytesRange,
         if_none_match: Option<&str>,
         if_match: Option<&str>,
         override_content_disposition: Option<&str>,
-    ) -> Result<Response<IncomingAsyncBody>> {
+    ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
             "{}/{}/{}",
             self.endpoint,
             self.container,
             percent_encode_path(&p)
@@ -150,18 +158,37 @@
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         if let Some(if_match) = if_match {
             req = req.header(IF_MATCH, if_match);
         }
 
-        let mut req = req
+        let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
+        Ok(req)
+    }
+
+    pub async fn azblob_get_blob(
+        &self,
+        path: &str,
+        range: BytesRange,
+        if_none_match: Option<&str>,
+        if_match: Option<&str>,
+        override_content_disposition: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.azblob_get_blob_request(
+            path,
+            range,
+            if_none_match,
+            if_match,
+            override_content_disposition,
+        )?;
+
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     pub fn azblob_put_blob_request(
         &self,
@@ -178,15 +205,15 @@
             self.endpoint,
             self.container,
             percent_encode_path(&p)
         );
 
         let mut req = Request::put(&url);
         if let Some(cache_control) = cache_control {
-            req = req.header(CACHE_CONTROL, cache_control);
+            req = req.header(constants::X_MS_BLOB_CACHE_CONTROL, cache_control);
         }
         if let Some(size) = size {
             req = req.header(CONTENT_LENGTH, size)
         }
 
         if let Some(ty) = content_type {
             req = req.header(CONTENT_TYPE, ty)
@@ -199,20 +226,20 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn azblob_get_blob_properties(
+    pub fn azblob_head_blob_request(
         &self,
         path: &str,
         if_none_match: Option<&str>,
         if_match: Option<&str>,
-    ) -> Result<Response<IncomingAsyncBody>> {
+    ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/{}/{}",
             self.endpoint,
             self.container,
             percent_encode_path(&p)
@@ -224,18 +251,29 @@
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         if let Some(if_match) = if_match {
             req = req.header(IF_MATCH, if_match);
         }
 
-        let mut req = req
+        let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
+        Ok(req)
+    }
+
+    pub async fn azblob_get_blob_properties(
+        &self,
+        path: &str,
+        if_none_match: Option<&str>,
+        if_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.azblob_head_blob_request(path, if_none_match, if_match)?;
+
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn azblob_delete_blob(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,17 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::sync::Arc;
 
 use async_trait::async_trait;
+use http::header::HOST;
 use http::StatusCode;
 use log::debug;
 use reqsign::GoogleCredentialLoader;
 use reqsign::GoogleSigner;
 use reqsign::GoogleTokenLoad;
 use reqsign::GoogleTokenLoader;
 use serde::Deserialize;
@@ -48,15 +49,15 @@
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
 /// - [x] list
 /// - [x] scan
 /// - [x] copy
-/// - [ ] presign
+/// - [x] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
 /// - `root`: Set the work directory for backend
 /// - `bucket`: Set the container name for backend
 /// - `endpoint`: Customizable endpoint setting
@@ -370,30 +371,43 @@
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Gcs)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
+                stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
+
                 read: true,
                 read_can_next: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
+
                 write: true,
+                write_with_content_type: true,
                 write_without_content_length: true,
+
                 list: true,
+                list_with_limit: true,
+                list_with_start_after: true,
                 scan: true,
                 copy: true,
+                presign: true,
+
                 ..Default::default()
             });
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut req =
-            self.core
-                .gcs_insert_object_request(path, Some(0), None, None, AsyncBody::Empty)?;
+        let mut req = self
+            .core
+            .gcs_insert_object_request(path, Some(0), None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         if resp.status().is_success() {
             resp.into_body().consume().await?;
@@ -431,25 +445,29 @@
             resp.into_body().consume().await?;
             Ok(RpCopy::default())
         } else {
             Err(parse_error(resp).await?)
         }
     }
 
-    async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
+    async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.gcs_get_object_metadata(path).await?;
+        let resp = self
+            .core
+            .gcs_get_object_metadata(path, args.if_match(), args.if_none_match())
+            .await?;
 
         if resp.status().is_success() {
             // read http response body
             let slc = resp.into_body().bytes().await?;
+
             let meta: GetObjectJsonResponse =
                 serde_json::from_slice(&slc).map_err(new_json_deserialize_error)?;
 
             let mode = if path.ends_with('/') {
                 EntryMode::DIR
             } else {
                 EntryMode::FILE
@@ -488,24 +506,68 @@
             Err(parse_error(resp).await?)
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            GcsPager::new(self.core.clone(), path, "/", args.limit()),
+            GcsPager::new(
+                self.core.clone(),
+                path,
+                "/",
+                args.limit(),
+                args.start_after(),
+            ),
         ))
     }
 
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
         Ok((
             RpScan::default(),
-            GcsPager::new(self.core.clone(), path, "", args.limit()),
+            GcsPager::new(self.core.clone(), path, "", args.limit(), None),
         ))
     }
+
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        // We will not send this request out, just for signing.
+        let mut req = match args.operation() {
+            PresignOperation::Stat(v) => {
+                self.core
+                    .gcs_head_object_xml_request(path, v.if_match(), v.if_none_match())?
+            }
+            PresignOperation::Read(v) => self.core.gcs_get_object_xml_request(
+                path,
+                v.range(),
+                v.if_match(),
+                v.if_none_match(),
+            )?,
+            PresignOperation::Write(_) => {
+                self.core
+                    .gcs_insert_object_xml_request(path, None, AsyncBody::Empty)?
+            }
+        };
+
+        self.core.sign_query(&mut req, args.expire()).await?;
+
+        // We don't need this request anymore, consume it directly.
+        let (mut parts, _) = req.into_parts();
+        // Always remove host header, let users' client to set it based on HTTP
+        // version.
+        //
+        // As discussed in <https://github.com/seanmonstar/reqwest/issues/1809>,
+        // google server could send RST_STREAM of PROTOCOL_ERROR if our request
+        // contains host header.
+        parts.headers.remove(HOST);
+
+        Ok(RpPresign::new(PresignedRequest::new(
+            parts.method,
+            parts.uri,
+            parts.headers,
+        )))
+    }
 }
 
 /// The raw json response returned by [`get`](https://cloud.google.com/storage/docs/json_api/v1/objects/get)
 #[derive(Debug, Default, Deserialize)]
 #[serde(default, rename_all = "camelCase")]
 struct GetObjectJsonResponse {
     /// GCS will return size in string.
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 25% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
+use std::time::Duration;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
 use bytes::Bytes;
 use bytes::BytesMut;
-use http::header::CACHE_CONTROL;
+
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
+use reqsign::GoogleCredential;
 use reqsign::GoogleCredentialLoader;
 use reqsign::GoogleSigner;
 use reqsign::GoogleToken;
 use reqsign::GoogleTokenLoader;
 
 use super::uri::percent_encode_path;
 use crate::raw::*;
@@ -81,20 +83,44 @@
             Err(Error::new(
                 ErrorKind::ConfigInvalid,
                 "no valid credential found",
             ))
         }
     }
 
+    fn load_credential(&self) -> Result<GoogleCredential> {
+        let cred = self
+            .credential_loader
+            .load()
+            .map_err(new_request_credential_error)?;
+
+        if let Some(cred) = cred {
+            Ok(cred)
+        } else {
+            Err(Error::new(
+                ErrorKind::ConfigInvalid,
+                "no valid credential found",
+            ))
+        }
+    }
+
     pub async fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
         let cred = self.load_token().await?;
 
         self.signer.sign(req, &cred).map_err(new_request_sign_error)
     }
 
+    pub async fn sign_query<T>(&self, req: &mut Request<T>, duration: Duration) -> Result<()> {
+        let cred = self.load_credential()?;
+
+        self.signer
+            .sign_query(req, duration, &cred)
+            .map_err(new_request_sign_error)
+    }
+
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 }
 
 impl GcsCore {
@@ -129,14 +155,45 @@
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
+    // It's for presign operation. Gcs only supports query sign over XML API.
+    pub fn gcs_get_object_xml_request(
+        &self,
+        path: &str,
+        range: BytesRange,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+
+        let mut req = Request::get(&url);
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+        if !range.is_full() {
+            req = req.header(http::header::RANGE, range.to_header());
+        }
+
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        Ok(req)
+    }
+
     pub async fn gcs_get_object(
         &self,
         path: &str,
         range: BytesRange,
         if_match: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
@@ -147,15 +204,14 @@
     }
 
     pub fn gcs_insert_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
-        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
             "{}/upload/storage/v1/b/{}/o?uploadType={}&name={}",
             self.endpoint,
@@ -172,18 +228,14 @@
             write!(&mut url, "&predefinedAcl={}", acl).unwrap();
         }
 
         let mut req = Request::post(&url);
 
         req = req.header(CONTENT_LENGTH, size.unwrap_or_default());
 
-        if let Some(cache_control) = cache_control {
-            req = req.header(CACHE_CONTROL, cache_control)
-        }
-
         if let Some(storage_class) = &self.default_storage_class {
             req = req.header(CONTENT_TYPE, "multipart/related; boundary=my-boundary");
 
             let mut req_body = BytesMut::with_capacity(100);
             write!(
                 &mut req_body,
                 "--my-boundary\nContent-Type: application/json; charset=UTF-8\n\n{{\"storageClass\": \"{}\"}}\n\n--my-boundary\n",
@@ -210,30 +262,112 @@
             }
 
             let req = req.body(body).map_err(new_request_build_error)?;
             Ok(req)
         }
     }
 
-    pub async fn gcs_get_object_metadata(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    // It's for presign operation. Gcs only supports query sign over XML API.
+    pub fn gcs_insert_object_xml_request(
+        &self,
+        path: &str,
+        content_type: Option<&str>,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+
+        let mut req = Request::put(&url);
+
+        if let Some(content_type) = content_type {
+            req = req.header(CONTENT_TYPE, content_type);
+        }
+
+        if let Some(acl) = &self.predefined_acl {
+            req = req.header("x-goog-acl", acl);
+        }
+
+        if let Some(storage_class) = &self.default_storage_class {
+            req = req.header("x-goog-storage-class", storage_class);
+        }
+
+        let req = req.body(body).map_err(new_request_build_error)?;
+
+        Ok(req)
+    }
+
+    pub fn gcs_head_object_request(
+        &self,
+        path: &str,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/storage/v1/b/{}/o/{}",
             self.endpoint,
             self.bucket,
             percent_encode_path(&p)
         );
 
-        let req = Request::get(&url);
+        let mut req = Request::get(&url);
+
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        Ok(req)
+    }
+
+    // It's for presign operation. Gcs only supports query sign over XML API.
+    pub fn gcs_head_object_xml_request(
+        &self,
+        path: &str,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
 
-        let mut req = req
+        let mut req = Request::head(&url);
+
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
+        let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
+        Ok(req)
+    }
+
+    pub async fn gcs_get_object_metadata(
+        &self,
+        path: &str,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.gcs_head_object_request(path, if_match, if_none_match)?;
+
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     pub async fn gcs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
@@ -268,27 +402,29 @@
             self.bucket,
             percent_encode_path(&source),
             self.bucket,
             percent_encode_path(&dest)
         );
 
         let mut req = Request::post(req_uri)
+            .header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn gcs_list_objects(
         &self,
         path: &str,
         page_token: &str,
         delimiter: &str,
         limit: Option<usize>,
+        start_after: Option<String>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
             "{}/storage/v1/b/{}/o?prefix={}",
             self.endpoint,
             self.bucket,
@@ -296,14 +432,20 @@
         );
         if !delimiter.is_empty() {
             write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
         }
         if let Some(limit) = limit {
             write!(url, "&maxResults={limit}").expect("write into string must succeed");
         }
+        if let Some(start_after) = start_after {
+            let start_after = build_abs_path(&self.root, &start_after);
+            write!(url, "&startOffset={}", percent_encode_path(&start_after))
+                .expect("write into string must succeed");
+        }
+
         if !page_token.is_empty() {
             // NOTE:
             //
             // GCS uses pageToken in request and nextPageToken in response
             //
             // Don't know how will those tokens be like so this part are copied
             // directly from AWS S3 service.
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,38 @@
 pub struct GcsPager {
     core: Arc<GcsCore>,
 
     path: String,
     delimiter: String,
     limit: Option<usize>,
 
+    /// Filter results to objects whose names are lexicographically
+    /// **equal to or after** startOffset
+    start_after: Option<String>,
+
     page_token: String,
     done: bool,
 }
 
 impl GcsPager {
     /// Generate a new directory walker
-    pub fn new(core: Arc<GcsCore>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
+    pub fn new(
+        core: Arc<GcsCore>,
+        path: &str,
+        delimiter: &str,
+        limit: Option<usize>,
+        start_after: Option<&str>,
+    ) -> Self {
         Self {
             core,
 
             path: path.to_string(),
             delimiter: delimiter.to_string(),
             limit,
+            start_after: start_after.map(String::from),
 
             page_token: "".to_string(),
             done: false,
         }
     }
 }
 
@@ -60,15 +71,21 @@
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
             .core
-            .gcs_list_objects(&self.path, &self.page_token, &self.delimiter, self.limit)
+            .gcs_list_objects(
+                &self.path,
+                &self.page_token,
+                &self.delimiter,
+                self.limit,
+                self.start_after.clone(),
+            )
             .await?;
 
         if !resp.status().is_success() {
             return Err(parse_error(resp).await?);
         }
         let bytes = resp.into_body().bytes().await?;
 
@@ -93,14 +110,20 @@
         }
 
         for object in output.items {
             if object.name.ends_with('/') {
                 continue;
             }
 
+            // exclude the inclusive start_after itself
+            let path = &build_rel_path(&self.core.root, &object.name);
+            if self.start_after.as_ref() == Some(path) {
+                continue;
+            }
+
             let mut meta = Metadata::new(EntryMode::FILE);
 
             // set metadata fields
             meta.set_content_md5(object.md5_hash.as_str());
             meta.set_etag(object.etag.as_str());
 
             let size = object.size.parse().map_err(|e| {
@@ -109,15 +132,15 @@
             meta.set_content_length(size);
             if !object.content_type.is_empty() {
                 meta.set_content_type(&object.content_type);
             }
 
             meta.set_last_modified(parse_datetime_from_rfc3339(object.updated.as_str())?);
 
-            let de = oio::Entry::new(&build_rel_path(&self.core.root, &object.name), meta);
+            let de = oio::Entry::new(path, meta);
 
             entries.push(de);
         }
 
         Ok(Some(entries))
     }
 }
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     }
 
     async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
         let mut req = self.core.gcs_insert_object_request(
             &percent_encode_path(&self.path),
             Some(bs.len()),
             self.op.content_type(),
-            self.op.cache_control(),
             AsyncBody::Bytes(bs),
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,19 @@
 /// - If meeting errors like the following:
 ///
 /// ```shell
 /// (unable to get stack trace for java.lang.NoClassDefFoundError exception: ExceptionUtils::getStackTrace error.)
 /// ```
 ///
 /// `CLASSPATH` is not set correctly or your hadoop installation is incorrect.
+///  
+/// To set `CLASSPATH`:
+/// ```shell
+/// export CLASSPATH=$(find $HADOOP_HOME -iname "*.jar" | xargs echo | tr ' ' ':'):${CLASSPATH}
+/// ```
 ///
 /// # Example
 ///
 /// ### Via Builder
 ///
 /// ```no_run
 /// use std::sync::Arc;
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -255,16 +255,22 @@
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Http)
             .set_root(&self.root)
             .set_capability(Capability {
+                stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
+
                 read: true,
                 read_can_next: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
 
                 ..Default::default()
             });
 
         ma
     }
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/http/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt` & `opendal-0.33.2/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -115,14 +115,19 @@
 pub use s3::S3;
 
 #[cfg(feature = "services-sled")]
 mod sled;
 #[cfg(feature = "services-sled")]
 pub use self::sled::Sled;
 
+// #[cfg(feature = "services-supabase")]
+mod supabase;
+// #[cfg(feature = "services-supabase")]
+pub use supabase::Supabase;
+
 #[cfg(feature = "services-wasabi")]
 mod wasabi;
 #[cfg(feature = "services-wasabi")]
 pub use wasabi::Wasabi;
 
 #[cfg(feature = "services-webdav")]
 mod webdav;
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -302,20 +302,31 @@
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Obs)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
+                stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
+
                 read: true,
                 read_can_next: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
+
                 write: true,
+                write_with_content_type: true,
+                write_with_cache_control: true,
+
                 list: true,
                 scan: true,
                 copy: true,
+
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         // OBS could return `520 Origin Error` errors which should be retried.
         v if v.as_u16() == 520 => (ErrorKind::Unexpected, true),
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -420,24 +420,35 @@
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Oss)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
+                stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
+
                 read: true,
                 read_can_next: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
+
                 write: true,
+                write_with_cache_control: true,
+                write_with_content_type: true,
                 write_without_content_length: true,
+
                 list: true,
                 scan: true,
                 copy: true,
                 presign: true,
                 batch: true,
                 batch_max_operations: Some(1000),
+
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -920,14 +920,16 @@
                 read: true,
                 read_can_next: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
+                write_with_cache_control: true,
+                write_with_content_type: true,
                 write_without_content_length: true,
 
                 list: true,
                 list_with_limit: true,
                 list_with_start_after: true,
 
                 scan: true,
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.33.2/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -442,16 +442,14 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    /// Make this functions as `pub(suber)` because `DirStream` depends
-    /// on this.
     pub async fn s3_list_objects(
         &self,
         path: &str,
         continuation_token: &str,
         delimiter: &str,
         limit: Option<usize>,
         start_after: Option<String>,
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 pub struct S3Pager {
     core: Arc<S3Core>,
 
     path: String,
     delimiter: String,
     limit: Option<usize>,
+
+    /// Amazon S3 starts listing **after** this specified key
     start_after: Option<String>,
 
     token: String,
     done: bool,
 }
 
 impl S3Pager {
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
             upload_id: None,
             parts: vec![],
             buffer: oio::VectorCursor::new(),
             // The part size must be 5 MiB to 5 GiB. There is no minimum
             // size limit on the last part of your multipart upload.
             //
-            // We pick the default value as 8 MiB for better thoughput.
+            // We pick the default value as 8 MiB for better throughput.
             //
             // TODO: allow this value to be configured.
             buffer_size: 8 * 1024 * 1024,
         }
     }
 
     async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -898,23 +898,29 @@
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Wasabi)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
+                stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
+
                 read: true,
                 read_can_next: true,
+
                 write: true,
                 list: true,
                 scan: true,
                 copy: true,
                 presign: true,
                 batch: true,
                 rename: true,
+
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -1052,15 +1058,15 @@
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         let ops = args.into_operation();
         if ops.len() > 1000 {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "s3 services only allow delete up to 1000 keys at once",
+                "wasabi services only allow delete up to 1000 keys at once",
             )
             .with_context("length", ops.len().to_string()));
         }
 
         let paths = ops.into_iter().map(|(p, _)| p).collect();
 
         let resp = self.core.delete_objects(paths).await?;
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/capability.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/error.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/list.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/metadata.rs`

 * *Files 4% similar despite different names*

```diff
@@ -32,37 +32,40 @@
 #[derive(Debug, Clone, Eq, PartialEq)]
 pub struct Metadata {
     /// bit stores current key store.
     bit: FlagSet<Metakey>,
 
     mode: EntryMode,
 
+    cache_control: Option<String>,
     content_disposition: Option<String>,
     content_length: Option<u64>,
     content_md5: Option<String>,
     content_range: Option<BytesContentRange>,
     content_type: Option<String>,
     etag: Option<String>,
     last_modified: Option<DateTime<Utc>>,
 }
 
 impl Metadata {
     /// Create a new metadata
     pub fn new(mode: EntryMode) -> Self {
         // Mode is required to be set for metadata.
-        let mut bit = Metakey::Mode.into();
+        let mut bit: FlagSet<Metakey> = Metakey::Mode.into();
         // If mode is dir, we should always mark it as complete.
         if mode.is_dir() {
             bit |= Metakey::Complete
         }
 
         Self {
             bit,
+
             mode,
 
+            cache_control: None,
             content_length: None,
             content_md5: None,
             content_type: None,
             content_range: None,
             last_modified: None,
             etag: None,
             content_disposition: None,
@@ -97,27 +100,59 @@
 
     /// Returns `true` if this metadata is for a directory.
     pub fn is_dir(&self) -> bool {
         matches!(self.mode, EntryMode::DIR)
     }
 
     /// Set mode for entry.
-    pub fn set_mode(&mut self, mode: EntryMode) -> &mut Self {
-        self.mode = mode;
+    pub fn set_mode(&mut self, v: EntryMode) -> &mut Self {
+        self.mode = v;
         self.bit |= Metakey::Mode;
         self
     }
 
     /// Set mode for entry.
-    pub fn with_mode(mut self, mode: EntryMode) -> Self {
-        self.mode = mode;
+    pub fn with_mode(mut self, v: EntryMode) -> Self {
+        self.mode = v;
         self.bit |= Metakey::Mode;
         self
     }
 
+    /// Cache control of this entry.
+    /// Cache-Control is defined by [RFC 7234](https://httpwg.org/specs/rfc7234.html#header.cache-control)
+    /// Refer to [MDN Cache-Control](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) for more information.
+    pub fn cache_control(&self) -> Option<&str> {
+        debug_assert!(
+            self.bit.contains(Metakey::CacheControl) || self.bit.contains(Metakey::Complete),
+            "visiting not set metadata: cache_control, maybe a bug"
+        );
+
+        self.cache_control.as_deref()
+    }
+
+    /// Set cache control of this entry.
+    ///
+    /// Cache-Control is defined by [RFC 7234](https://httpwg.org/specs/rfc7234.html#header.cache-control)
+    /// Refer to [MDN Cache-Control](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) for more information.
+    pub fn set_cache_control(&mut self, v: &str) -> &mut Self {
+        self.cache_control = Some(v.to_string());
+        self.bit |= Metakey::CacheControl;
+        self
+    }
+
+    /// Set cache control of this entry.
+    ///
+    /// Cache-Control is defined by [RFC 7234](https://httpwg.org/specs/rfc7234.html#header.cache-control)
+    /// Refer to [MDN Cache-Control](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) for more information.
+    pub fn with_cache_control(mut self, v: String) -> Self {
+        self.cache_control = Some(v);
+        self.bit |= Metakey::CacheControl;
+        self
+    }
+
     /// Content length of this entry.
     ///
     /// `Content-Length` is defined by [RFC 7230](https://httpwg.org/specs/rfc7230.html#header.content-length)
     /// Refer to [MDN Content-Length](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Length) for more information.
     pub fn content_length(&self) -> u64 {
         debug_assert!(
             self.bit.contains(Metakey::ContentLength) || self.bit.contains(Metakey::Complete),
@@ -129,23 +164,23 @@
 
     /// Fetch the raw content length.
     pub(crate) fn content_length_raw(&self) -> Option<u64> {
         self.content_length
     }
 
     /// Set content length of this entry.
-    pub fn set_content_length(&mut self, content_length: u64) -> &mut Self {
-        self.content_length = Some(content_length);
+    pub fn set_content_length(&mut self, v: u64) -> &mut Self {
+        self.content_length = Some(v);
         self.bit |= Metakey::ContentLength;
         self
     }
 
     /// Set content length of this entry.
-    pub fn with_content_length(mut self, content_length: u64) -> Self {
-        self.content_length = Some(content_length);
+    pub fn with_content_length(mut self, v: u64) -> Self {
+        self.content_length = Some(v);
         self.bit |= Metakey::ContentLength;
         self
     }
 
     /// Content MD5 of this entry.
     ///
     /// Content MD5 is defined by [RFC 2616](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html).
@@ -161,26 +196,26 @@
         self.content_md5.as_deref()
     }
 
     /// Set content MD5 of this entry.
     ///
     /// Content MD5 is defined by [RFC 2616](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html).
     /// And removed by [RFC 7231](https://www.rfc-editor.org/rfc/rfc7231).
-    pub fn set_content_md5(&mut self, content_md5: &str) -> &mut Self {
-        self.content_md5 = Some(content_md5.to_string());
+    pub fn set_content_md5(&mut self, v: &str) -> &mut Self {
+        self.content_md5 = Some(v.to_string());
         self.bit |= Metakey::ContentMd5;
         self
     }
 
     /// Set content MD5 of this entry.
     ///
     /// Content MD5 is defined by [RFC 2616](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html).
     /// And removed by [RFC 7231](https://www.rfc-editor.org/rfc/rfc7231).
-    pub fn with_content_md5(mut self, content_md5: String) -> Self {
-        self.content_md5 = Some(content_md5);
+    pub fn with_content_md5(mut self, v: String) -> Self {
+        self.content_md5 = Some(v);
         self.bit |= Metakey::ContentMd5;
         self
     }
 
     /// Content Type of this entry.
     ///
     /// Content Type is defined by [RFC 9110](https://httpwg.org/specs/rfc9110.html#field.content-type).
@@ -256,26 +291,26 @@
         self.last_modified
     }
 
     /// Set Last modified of this entry.
     ///
     /// `Last-Modified` is defined by [RFC 7232](https://httpwg.org/specs/rfc7232.html#header.last-modified)
     /// Refer to [MDN Last-Modified](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Last-Modified) for more information.
-    pub fn set_last_modified(&mut self, last_modified: DateTime<Utc>) -> &mut Self {
-        self.last_modified = Some(last_modified);
+    pub fn set_last_modified(&mut self, v: DateTime<Utc>) -> &mut Self {
+        self.last_modified = Some(v);
         self.bit |= Metakey::LastModified;
         self
     }
 
     /// Set Last modified of this entry.
     ///
     /// `Last-Modified` is defined by [RFC 7232](https://httpwg.org/specs/rfc7232.html#header.last-modified)
     /// Refer to [MDN Last-Modified](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Last-Modified) for more information.
-    pub fn with_last_modified(mut self, last_modified: DateTime<Utc>) -> Self {
-        self.last_modified = Some(last_modified);
+    pub fn with_last_modified(mut self, v: DateTime<Utc>) -> Self {
+        self.last_modified = Some(v);
         self.bit |= Metakey::LastModified;
         self
     }
 
     /// ETag of this entry.
     ///
     /// `ETag` is defined by [RFC 7232](https://httpwg.org/specs/rfc7232.html#header.etag)
@@ -303,16 +338,16 @@
     ///
     /// OpenDAL will return this value AS-IS like the following:
     ///
     /// - `"33a64df551425fcc55e4d42a148795d9f25f89d4"`
     /// - `W/"0815"`
     ///
     /// `"` is part of etag, don't trim it before setting.
-    pub fn set_etag(&mut self, etag: &str) -> &mut Self {
-        self.etag = Some(etag.to_string());
+    pub fn set_etag(&mut self, v: &str) -> &mut Self {
+        self.etag = Some(v.to_string());
         self.bit |= Metakey::Etag;
         self
     }
 
     /// Set ETag of this entry.
     ///
     /// `ETag` is defined by [RFC 7232](https://httpwg.org/specs/rfc7232.html#header.etag)
@@ -320,16 +355,16 @@
     ///
     /// OpenDAL will return this value AS-IS like the following:
     ///
     /// - `"33a64df551425fcc55e4d42a148795d9f25f89d4"`
     /// - `W/"0815"`
     ///
     /// `"` is part of etag, don't trim it before setting.
-    pub fn with_etag(mut self, etag: String) -> Self {
-        self.etag = Some(etag);
+    pub fn with_etag(mut self, v: String) -> Self {
+        self.etag = Some(v);
         self.bit |= Metakey::Etag;
         self
     }
 
     /// Content-Disposition of this entry
     ///
     /// `Content-Disposition` is defined by [RFC 2616](https://www.rfc-editor/rfcs/2616) and
@@ -357,16 +392,16 @@
     /// Refer to [MDN Content-Disposition](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Disposition) for more information.
     ///
     /// OpenDAL will return this value AS-IS like the following:
     ///
     /// - "inline"
     /// - "attachment"
     /// - "attachment; filename=\"filename.jpg\""
-    pub fn with_content_disposition(mut self, content_disposition: String) -> Self {
-        self.content_disposition = Some(content_disposition);
+    pub fn with_content_disposition(mut self, v: String) -> Self {
+        self.content_disposition = Some(v);
         self.bit |= Metakey::ContentDisposition;
         self
     }
 
     /// Set Content-Disposition of this entry
     ///
     /// `Content-Disposition` is defined by [RFC 2616](https://www.rfc-editor/rfcs/2616) and
@@ -374,16 +409,16 @@
     /// Refer to [MDN Content-Disposition](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Disposition) for more information.
     ///
     /// OpenDAL will return this value AS-IS like the following:
     ///
     /// - "inline"
     /// - "attachment"
     /// - "attachment; filename=\"filename.jpg\""
-    pub fn set_content_disposition(&mut self, content_disposition: &str) -> &mut Self {
-        self.content_disposition = Some(content_disposition.to_string());
+    pub fn set_content_disposition(&mut self, v: &str) -> &mut Self {
+        self.content_disposition = Some(v.to_string());
         self.bit |= Metakey::ContentDisposition;
         self
     }
 }
 
 flags! {
     /// Metakey describes the metadata keys that can be stored
@@ -402,14 +437,16 @@
     pub enum Metakey: u64 {
         /// The special metadata key that used to mark this entry
         /// already contains all metadata.
         Complete,
 
         /// Key for mode.
         Mode,
+        /// Key for cache control.
+        CacheControl,
         /// Key for content disposition.
         ContentDisposition,
         /// Key for content length.
         ContentLength,
         /// Key for content md5.
         ContentMd5,
         /// Key for content range.
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/ops.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/scheme.rs`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     Redis,
     /// [rocksdb][crate::services::Rocksdb]: RocksDB services
     Rocksdb,
     /// [s3][crate::services::S3]: AWS S3 alike services.
     S3,
     /// [sled][crate::services::Sled]: Sled services
     Sled,
+    /// [Supabase][crate::services::Supabase]: Supabase storage service
+    Supabase,
     /// [wasabi][crate::services::Wasabi]: Wasabi service
     Wasabi,
     /// [webdav][crate::services::Webdav]: WebDAV support.
     Webdav,
     /// [webhdfs][crate::services::Webhdfs]: WebHDFS RESTful API Services
     Webhdfs,
     /// Custom that allow users to implement services outside of OpenDAL.
@@ -126,14 +128,15 @@
             "memory" => Ok(Scheme::Memory),
             "moka" => Ok(Scheme::Moka),
             "obs" => Ok(Scheme::Obs),
             "redis" => Ok(Scheme::Redis),
             "rocksdb" => Ok(Scheme::Rocksdb),
             "s3" => Ok(Scheme::S3),
             "sled" => Ok(Scheme::Sled),
+            "supabase" => Ok(Scheme::Supabase),
             "oss" => Ok(Scheme::Oss),
             "wasabi" => Ok(Scheme::Wasabi),
             "webdav" => Ok(Scheme::Webdav),
             "webhdfs" => Ok(Scheme::Webhdfs),
             _ => Ok(Scheme::Custom(Box::leak(s.into_boxed_str()))),
         }
     }
@@ -157,14 +160,15 @@
             Scheme::Memory => "memory",
             Scheme::Moka => "moka",
             Scheme::Obs => "obs",
             Scheme::Redis => "redis",
             Scheme::Rocksdb => "rocksdb",
             Scheme::S3 => "s3",
             Scheme::Sled => "sled",
+            Scheme::Supabase => "supabase",
             Scheme::Oss => "oss",
             Scheme::Wasabi => "wasabi",
             Scheme::Webdav => "webdav",
             Scheme::Webhdfs => "webhdfs",
             Scheme::Custom(v) => v,
         }
     }
```

### Comparing `opendal-0.33.1/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.33.2/local_dependencies/opendal/src/types/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/Cargo.toml` & `opendal-0.33.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.33.1"
+version= "0.33.2"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 chrono = { version = "0.4.24", default-features = false, features = ["std"] }
```

### Comparing `opendal-0.33.1/.gitignore` & `opendal-0.33.2/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/README.md` & `opendal-0.33.2/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/benchmark/README.md` & `opendal-0.33.2/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/benchmark/async_opendal_benchmark.py` & `opendal-0.33.2/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.33.2/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/examples/object.ipynb` & `opendal-0.33.2/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/pyproject.toml` & `opendal-0.33.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/python/opendal/__init__.py` & `opendal-0.33.2/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/python/opendal/__init__.pyi` & `opendal-0.33.2/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/src/asyncio.rs` & `opendal-0.33.2/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/src/layers.rs` & `opendal-0.33.2/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/src/lib.rs` & `opendal-0.33.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/tests/binding.feature` & `opendal-0.33.2/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/tests/steps/binding.py` & `opendal-0.33.2/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.1/Cargo.lock` & `opendal-0.33.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2289,15 +2289,15 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.33.1"
+version = "0.33.2"
 dependencies = [
  "anyhow",
  "clap 4.1.11",
  "dirs",
  "env_logger",
  "futures",
  "log",
@@ -2326,27 +2326,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.33.1"
+version = "0.33.2"
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
-version = "0.33.1"
+version = "0.33.2"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.1.11",
  "dirs",
  "env_logger",
  "futures",
@@ -2369,15 +2369,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.33.1"
+version = "0.33.2"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
@@ -2441,31 +2441,34 @@
 ]
 
 [[package]]
 name = "opendal-java"
 version = "0.1.0"
 dependencies = [
  "jni",
+ "num_cpus",
+ "once_cell",
  "opendal",
+ "tokio",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.33.1"
+version = "0.33.2"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.33.1"
+version = "0.33.2"
 dependencies = [
  "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
```

### Comparing `opendal-0.33.1/PKG-INFO` & `opendal-0.33.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.33.1
+Version: 0.33.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pdoc; extra == 'docs'
 Requires-Dist: behave; extra == 'test'
 Requires-Dist: gevent; extra == 'benchmark'
 Requires-Dist: greenify; extra == 'benchmark'
@@ -18,17 +18,17 @@
 Summary: OpenDAL Python Binding
 Home-Page: https://opendal.apache.org/
 Author: OpenDAL Contributors <dev@opendal.apache.org>
 Author-email: OpenDAL Contributors <dev@opendal.apache.org>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://opendal.apache.org/docs/python/opendal.html
 Project-URL: Homepage, https://opendal.apache.org/
 Project-URL: Repository, https://github.com/apache/incubator-opendal
+Project-URL: Documentation, https://opendal.apache.org/docs/python/opendal.html
 
 # OpenDAL Python Binding
 
 Documentation: [main](https://opendal.apache.org/docs/python/)
 
 This crate intends to build a native python binding.
```

