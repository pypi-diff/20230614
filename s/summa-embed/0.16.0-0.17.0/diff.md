# Comparing `tmp/summa_embed-0.16.0.tar.gz` & `tmp/summa_embed-0.17.0.tar.gz`

## Comparing `summa_embed-0.16.0.tar` & `summa_embed-0.17.0.tar`

### file list

```diff
@@ -1,107 +1,113 @@
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 summa_embed-0.16.0/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-08 13:34:47.000000 summa_embed-0.16.0/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7181 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24071 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14323 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      167 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    15532 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1687 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    59733 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     4400 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-r--r--   0      501       20     2216 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11274 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3568 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5474 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.16.0/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2262 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10469 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7638 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2523 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      394 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 summa_embed-0.16.0/Cargo.toml
--rw-r--r--   0      501       20      685 2023-06-08 13:34:51.000000 summa_embed-0.16.0/.gitignore
--rwxr-xr-x   0      501       20      347 2023-06-08 13:34:51.000000 summa_embed-0.16.0/build.sh
--rw-r--r--   0      501       20      515 2023-06-08 13:34:51.000000 summa_embed-0.16.0/pyproject.toml
--rw-r--r--   0      501       20       14 2023-06-08 13:34:51.000000 summa_embed-0.16.0/requirements.txt
--rw-r--r--   0      501       20     4617 2023-06-08 13:34:52.000000 summa_embed-0.16.0/src/lib.rs
--rw-r--r--   0      501       20     1559 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/__init__.py
--rw-r--r--   0      501       20        0 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/__init__.py
--rw-r--r--   0      501       20     3124 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.py
--rw-r--r--   0      501       20     3153 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.pyi
--rw-r--r--   0      501       20     1336 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.py
--rw-r--r--   0      501       20     1115 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.pyi
--rw-r--r--   0      501       20    16903 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/index_service_pb2.py
--rw-r--r--   0      501       20    20493 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/index_service_pb2.pyi
--rw-r--r--   0      501       20    23885 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/query_pb2.py
--rw-r--r--   0      501       20    32310 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/query_pb2.pyi
--rw-r--r--   0      501       20     2214 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.py
--rw-r--r--   0      501       20     1996 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.pyi
--rw-r--r--   0      501       20     2012 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/search_service_pb2.py
--rw-r--r--   0      501       20     1903 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/search_service_pb2.pyi
--rw-r--r--   0      501       20     1742 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.py
--rw-r--r--   0      501       20     1653 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.pyi
--rw-r--r--   0      501       20     1041 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/utils_pb2.py
--rw-r--r--   0      501       20      455 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/utils_pb2.pyi
--rw-r--r--   0      501       20   101494 2023-06-08 13:37:40.000000 summa_embed-0.16.0/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.16.0/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.0/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2381 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10274 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7871 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 summa_embed-0.17.0/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20   370551 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-r--r--   0      501       20       92 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7233 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5297 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24321 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13903 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14323 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5057 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      239 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20      615 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-r--r--   0      501       20     1376 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/morphology/english_nn.rs
+-rw-r--r--   0      501       20      847 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-r--r--   0      501       20     2131 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-r--r--   0      501       20    15903 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1695 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    64149 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     6095 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     1039 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-r--r--   0      501       20     2216 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11274 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7462 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     4680 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-06-14 12:59:28.000000 summa_embed-0.17.0/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 summa_embed-0.17.0/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-06-14 12:59:28.000000 summa_embed-0.17.0/.gitignore
+-rwxr-xr-x   0      501       20      347 2023-06-14 12:59:28.000000 summa_embed-0.17.0/build.sh
+-rw-r--r--   0      501       20      515 2023-06-14 12:59:28.000000 summa_embed-0.17.0/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-06-14 12:59:28.000000 summa_embed-0.17.0/requirements.txt
+-rw-r--r--   0      501       20     4646 2023-06-14 12:59:28.000000 summa_embed-0.17.0/src/lib.rs
+-rw-r--r--   0      501       20     1542 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/__init__.py
+-rw-r--r--   0      501       20     3124 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/consumer_service_pb2.py
+-rw-r--r--   0      501       20     3153 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/consumer_service_pb2.pyi
+-rw-r--r--   0      501       20     1336 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/dag_pb_pb2.py
+-rw-r--r--   0      501       20     1115 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/dag_pb_pb2.pyi
+-rw-r--r--   0      501       20    16738 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/index_service_pb2.py
+-rw-r--r--   0      501       20    20160 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/index_service_pb2.pyi
+-rw-r--r--   0      501       20    24455 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/query_pb2.py
+-rw-r--r--   0      501       20    33178 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/query_pb2.pyi
+-rw-r--r--   0      501       20     2214 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/reflection_service_pb2.py
+-rw-r--r--   0      501       20     1996 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/reflection_service_pb2.pyi
+-rw-r--r--   0      501       20     2012 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/search_service_pb2.py
+-rw-r--r--   0      501       20     1903 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/search_service_pb2.pyi
+-rw-r--r--   0      501       20     1742 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/unixfs_pb2.py
+-rw-r--r--   0      501       20     1653 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/unixfs_pb2.pyi
+-rw-r--r--   0      501       20     1041 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/utils_pb2.py
+-rw-r--r--   0      501       20      455 2023-06-14 12:59:28.000000 summa_embed-0.17.0/summa_embed/proto/utils_pb2.pyi
+-rw-r--r--   0      501       20   115919 2023-06-14 12:59:52.000000 summa_embed-0.17.0/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.0/PKG-INFO
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.0/local_dependencies/summa-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [package]
 name = "summa-core"
-version = "0.16.0"
+version = "0.17.0"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
 path = "src/lib.rs"
 doc = true
 
 [features]
 fs = ["tantivy/mmap", "tokio/fs"]
 hyper-external-request = ["hyper", "hyper-tls"]
 metrics = ["opentelemetry"]
+nn = ["rust-bert"]
 tokio-rt = ["tokio/rt"]
 
 [dependencies]
 anyhow = "1.0"
 async-trait = "0.1"
 base64 = "0.21"
 bytes = "1.3"
@@ -38,14 +39,15 @@
 pest = "2.5"
 pest_derive = "2.5"
 pluralize-rs = "0.1"
 prost = "0.11"
 rand = { version = "0.8", features = ["small_rng"] }
 rayon = "1.6.1"
 regex = "1.8"
+rust-bert = { version = "0.21", optional = true }
 rustc-hash = "1.1.0"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_bytes = "0.11"
 serde_cbor = "0.11"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
 strfmt = "0.2"
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.0/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 use tantivy::{DocAddress, DocId, Score, SegmentOrdinal, SegmentReader};
 
 /// `ReservoirSampling` collector collects `k` random documents using `O(k)` memory
 ///
 /// ```rust
 /// use summa_core::collectors::ReservoirSampling;
 /// use summa_core::configs::core::QueryParserConfig;
+/// use summa_core::components::{MorphologyManager, QueryParser};
 /// use tantivy::collector::Count;
-/// use summa_core::components::QueryParser;
 /// use tantivy::schema::{Schema, TEXT};
 /// use tantivy::{doc, Index};
 ///
 /// let mut schema_builder = Schema::builder();
 /// let title = schema_builder.add_text_field("title", TEXT);
 /// let schema = schema_builder.build();
 /// let index = Index::create_in_ram(schema);
@@ -26,15 +26,15 @@
 /// index_writer.add_document(doc!(title => "The Diary of a Young Girl")).unwrap();
 /// assert!(index_writer.commit().is_ok());
 ///
 /// let reader = index.reader().unwrap();
 /// let searcher = reader.searcher();
 ///
 /// // Here comes the important part
-/// let query_parser = QueryParser::for_index(&index, QueryParserConfig::from_default_fields(vec!["title".to_string()])).unwrap();
+/// let query_parser = QueryParser::for_index(&index, QueryParserConfig::from_default_fields(vec!["title".to_string()]), &MorphologyManager::default()).unwrap();
 /// let query = query_parser.parse_query("diary").unwrap();
 /// let documents = searcher.search(&query, &ReservoirSampling::with_limit(2)).unwrap();
 ///
 /// assert_eq!(documents.len(), 2);
 /// ```
 pub struct ReservoirSampling {
     limit: usize,
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files 4% similar despite different names*

```diff
@@ -321,25 +321,30 @@
     "ya",
     "o",
     "este",
     "sí",
 ];
 
 /// Instantiate default tokenizers
-pub fn default_tokenizers() -> [(String, TextAnalyzer); 3] {
+pub fn default_tokenizers() -> [(String, TextAnalyzer); 4] {
     let summa_tokenizer = TextAnalyzer::builder(SummaTokenizer)
         .filter(RemoveLongFilter::limit(100))
         .filter(LowerCaser)
         .filter(StopWordFilter::remove(STOP_WORDS.map(String::from).to_vec()))
         .build();
-    let default_tokenizer = TextAnalyzer::builder(SimpleTokenizer)
+    let summa_without_stop_words_tokenizer = TextAnalyzer::builder(SummaTokenizer)
+        .filter(RemoveLongFilter::limit(100))
+        .filter(LowerCaser)
+        .build();
+    let default_tokenizer = TextAnalyzer::builder(SimpleTokenizer::default())
         .filter(RemoveLongFilter::limit(100))
         .filter(LowerCaser)
         .filter(StopWordFilter::remove(STOP_WORDS.map(String::from).to_vec()))
         .build();
-    let raw_tokenizer = TextAnalyzer::builder(RawTokenizer).filter(LowerCaser).build();
+    let raw_tokenizer = TextAnalyzer::builder(RawTokenizer::default()).filter(LowerCaser).build();
     [
         ("summa".to_owned(), summa_tokenizer),
+        ("summa_without_stop_words".to_owned(), summa_without_stop_words_tokenizer),
         ("default".to_owned(), default_tokenizer),
         ("raw".to_owned(), raw_tokenizer),
     ]
 }
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files 4% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 }
 
 impl IndexHolder {
     /// Sets up `IndexHolder`
     pub fn create_holder(
         core_config: &crate::configs::core::Config,
         mut index: Index,
-        index_name: Option<&str>,
+        index_name: &str,
         index_engine_config: Arc<dyn ConfigProxy<proto::IndexEngineConfig>>,
         merge_policy: Option<proto::MergePolicy>,
         query_parser_config: proto::QueryParserConfig,
         driver: Driver,
     ) -> SummaResult<IndexHolder> {
         register_default_tokenizers(&index);
 
@@ -179,24 +179,15 @@
                     .iter()
                     .map(|field_name| Ok::<_, Error>(cached_schema.get_field(field_name)?))
                     .collect()
             })
             .transpose()?
             .unwrap_or_default();
 
-        let index_name = index_name.map(|x| x.to_string()).unwrap_or_else(|| {
-            cached_index_attributes
-                .as_ref()
-                .expect("no attributes")
-                .default_index_name
-                .clone()
-                .expect("no index name")
-        });
-
-        let query_parser = ProtoQueryParser::for_index(&index_name, &index, query_parser_config)?;
+        let query_parser = ProtoQueryParser::for_index(index_name, &index, query_parser_config)?;
         let index_reader = index
             .reader_builder()
             .doc_store_cache_num_blocks(core_config.doc_store_cache_num_blocks)
             .reload_policy(ReloadPolicy::OnCommit)
             .try_into()?;
         index_reader.reload()?;
 
@@ -211,15 +202,15 @@
             )?)))
         } else {
             None
         };
 
         Ok(IndexHolder {
             index_engine_config,
-            index_name,
+            index_name: index_name.to_string(),
             index: index.clone(),
             query_parser,
             cached_schema,
             cached_index_attributes,
             cached_multi_fields,
             index_reader,
             index_writer_holder,
@@ -428,14 +419,20 @@
         index_alias: &str,
         query: proto::query::Query,
         collectors: Vec<proto::Collector>,
         is_fieldnorms_scoring_enabled: Option<bool>,
     ) -> SummaResult<Vec<IntermediateExtractionResult>> {
         let searcher = self.index_reader().searcher();
         trace!(action = "parse_query", index_name = ?self.index_name, query = ?query);
+        #[cfg(feature = "tokio-rt")]
+        let parsed_query = {
+            let query_parser = self.query_parser.clone();
+            tokio::task::spawn_blocking(move || query_parser.parse_query(query)).await??
+        };
+        #[cfg(not(feature = "tokio-rt"))]
         let parsed_query = self.query_parser.parse_query(query)?;
         let mut multi_collector = MultiCollector::new();
         trace!(action = "build_extractors", index_name = ?self.index_name);
         let extractors: Vec<Box<dyn FruitExtractor>> = collectors
             .into_iter()
             .map(|collector_proto| build_fruit_extractor(self, index_alias, searcher.clone(), collector_proto, &parsed_query, &mut multi_collector))
             .collect::<SummaResult<_>>()?;
@@ -463,14 +460,20 @@
         }
         trace!(action = "extracted");
         Ok(collector_outputs)
     }
 
     /// Delete `SummaDocument` by `unq`
     pub async fn delete_documents(&self, query: proto::query::Query) -> SummaResult<u64> {
+        #[cfg(feature = "tokio-rt")]
+        let parsed_query = {
+            let query_parser = self.query_parser.clone();
+            tokio::task::spawn_blocking(move || query_parser.parse_query(query)).await??
+        };
+        #[cfg(not(feature = "tokio-rt"))]
         let parsed_query = self.query_parser.parse_query(query)?;
         self.index_writer_holder()?.read().await.delete_by_query(parsed_query)
     }
 
     /// Index generic `SummaDocument`
     ///
     /// `IndexUpdater` bounds unbounded `SummaDocument` inside
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files 0% similar despite different names*

```diff
@@ -207,14 +207,15 @@
                             has_next |= doc_references.has_next;
                             total_documents += doc_references.scored_doc_addresses.len();
                             extraction_toolings.insert(doc_references.index_alias.as_str(), &doc_references.extraction_tooling);
                             if let Some(sg_config) = &doc_references.snippet_generator_config {
                                 snippet_generators_futures.push(async move { (doc_references.index_alias.as_str(), sg_config.as_tantivy_async().await) });
                             }
                         }
+                        has_next |= total_documents > limit + offset;
 
                         trace!(action = "generate_snippets");
                         let snippet_generators: HashMap<&str, Vec<(String, SnippetGenerator)>> =
                             join_all(snippet_generators_futures).await.into_iter().collect();
 
                         info!(
                             action = "retrieving_documents",
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pub use custom_serializer::NamedFieldDocument;
 pub use default_tokenizers::default_tokenizers;
 pub use driver::Driver;
 pub use fruit_extractors::{build_fruit_extractor, FruitExtractor, IntermediateExtractionResult};
 pub use index_holder::{cleanup_index, IndexHolder};
 pub use index_registry::IndexRegistry;
 pub use index_writer_holder::IndexWriterHolder;
-pub use query_parser::{ProtoQueryParser, QueryParser, QueryParserError};
+pub use query_parser::{MorphologyManager, ProtoQueryParser, QueryParser, QueryParserError};
 pub use segment_attributes::SummaSegmentAttributes;
 pub use summa_document::{DocumentParsingError, SummaDocument};
 pub use summa_tokenizer::SummaTokenizer;
 
 pub mod test_utils {
     use std::default::Default;
     use std::sync::atomic::{AtomicI64, Ordering};
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,34 @@
     AllQuery, BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, MoreLikeThisQuery, Occur, PhraseQuery, Query, RangeQuery, RegexQuery, TermQuery,
 };
 use tantivy::schema::{Field, FieldEntry, FieldType, IndexRecordOption, Schema};
 use tantivy::{DateTime, Index, Score, Term};
 use tracing::info;
 
 use crate::components::queries::ExistsQuery;
+use crate::components::query_parser::morphology::MorphologyManager;
 use crate::components::query_parser::{QueryParser, QueryParserError};
 use crate::configs::core::QueryParserConfig;
 use crate::errors::{Error, SummaResult, ValidationError};
 #[cfg(feature = "metrics")]
 use crate::metrics::ToLabel;
 
 /// Responsible for casting `crate::proto::Query` message to `tantivy::query::Query`
+#[derive(Clone)]
 pub struct ProtoQueryParser {
     index: Index,
     index_name: String,
     cached_schema: Schema,
     // Counters
     #[cfg(feature = "metrics")]
     query_counter: Counter<u64>,
     #[cfg(feature = "metrics")]
     subquery_counter: Counter<u64>,
     query_parser_config: QueryParserConfig,
+    morphology_manager: MorphologyManager,
 }
 
 pub enum QueryParserDefaultMode {
     Boolean,
     DisjuctionMax { tie_breaker: Score },
 }
 
@@ -120,14 +123,15 @@
             index_name: index_name.to_string(),
             cached_schema: index.schema(),
             #[cfg(feature = "metrics")]
             query_counter,
             #[cfg(feature = "metrics")]
             subquery_counter,
             query_parser_config: QueryParserConfig(query_parser_config),
+            morphology_manager: MorphologyManager::default(),
         })
     }
 
     pub fn resolve_field_name<'a>(&'a self, field_name: &'a str) -> &str {
         self.query_parser_config
             .0
             .field_aliases
@@ -182,24 +186,22 @@
                     .collect::<SummaResult<Vec<_>>>()?,
                 match disjunction_max_proto.tie_breaker.as_str() {
                     "" => 0.0,
                     s => f32::from_str(s).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {} as f32", disjunction_max_proto.tie_breaker)))?,
                 },
             )),
             proto::query::Query::Match(match_query_proto) => {
-                let nested_query_parser = QueryParser::for_index(
-                    &self.index,
-                    match_query_proto
-                        .query_parser_config
-                        .map(QueryParserConfig)
-                        .unwrap_or_else(|| self.query_parser_config.clone()),
-                )?;
+                let mut new_query_parser_config = self.query_parser_config.clone();
+                if let Some(query_parser_config) = match_query_proto.query_parser_config {
+                    new_query_parser_config.merge(QueryParserConfig(query_parser_config));
+                }
+                let nested_query_parser = QueryParser::for_index(&self.index, new_query_parser_config.clone(), &self.morphology_manager)?;
                 match nested_query_parser.parse_query(&match_query_proto.value) {
                     Ok(parsed_query) => {
-                        info!(parsed_match_query = ?parsed_query);
+                        info!(query = ?match_query_proto.value, parsed_match_query = ?parsed_query, query_parser_config = ?new_query_parser_config);
                         Ok(parsed_query)
                     }
                     Err(QueryParserError::FieldDoesNotExist(field)) => Err(ValidationError::MissingField(field).into()),
                     Err(e) => Err(Error::InvalidQuerySyntax(Box::new(e), match_query_proto.value.to_owned())),
                 }?
             }
             proto::query::Query::Range(range_query_proto) => {
@@ -220,15 +222,15 @@
             )),
             proto::query::Query::Regex(regex_query_proto) => {
                 let (field, _, _) = self.field_and_field_entry(&regex_query_proto.field)?;
                 Box::new(RegexQuery::from_pattern(&regex_query_proto.value, field)?)
             }
             proto::query::Query::Phrase(phrase_query_proto) => {
                 let (field, full_path, field_entry) = self.field_and_field_entry(&phrase_query_proto.field)?;
-                let tokenizer = self.index.tokenizer_for_field(field)?;
+                let mut tokenizer = self.index.tokenizer_for_field(field)?;
 
                 let mut token_stream = tokenizer.token_stream(&phrase_query_proto.value);
                 let mut terms: Vec<(usize, Term)> = vec![];
                 while let Some(token) = token_stream.next() {
                     terms.push((token.position, cast_value_to_term(field, full_path, field_entry.field_type(), &token.text)?))
                 }
                 if terms.is_empty() {
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 star = { "*" }
 statement_sep = _{ WHITE_SPACE | "," | "." | ";" | "!" | "?" | (":" ~ WHITE_SPACE) | "(" | ")" | "/" }
 allowed_chars = _{"_" | "+" | "#" | "-"}
 url_end = _{ WHITE_SPACE | "," }
 
 isbn = @{ "978" ~ ("-"? ~ ASCII_DIGIT){7,10} ~ EOI }
 doi = @{ "10." ~ ASCII_DIGIT{4,9} ~ WHITE_SPACE? ~ "/" ~ WHITE_SPACE? ~ (!WHITE_SPACE ~ ANY)+ }
-wrapped_doi = _{ ("http" ~ "s"? ~ "://")? ~ "doi.org/"? ~ doi }
+wrapped_doi = _{ ("http" ~ "s"? ~ "://")? ~ "dx."? ~"doi.org/"? ~ doi }
 // url = _{ ("http" ~ "s"? ~ "://")? ~ (!url_end ~ ANY)+ }
 
 slop = @{ DECIMAL_NUMBER+ }
 boost = { (DECIMAL_NUMBER | ".")+ }
 range = ${ "[" ~ WHITE_SPACE* ~ boundary_word ~ WHITE_SPACE+ ~ ^"to" ~ WHITE_SPACE+ ~ boundary_word ~ WHITE_SPACE* ~ "]" }
 
 field_name = @{ ASCII_ALPHA ~ (ASCII_ALPHANUMERIC | "_" | ".")* }
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 use std::ops::Deref;
 use std::str::FromStr;
 
 use pest::iterators::{Pair, Pairs};
 use pest::Parser;
 use pest_derive::Parser;
 use summa_proto::proto;
-use tantivy::json_utils::{convert_to_fast_value_and_get_term, JsonTermWriter};
 use tantivy::query::{BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, PhraseQuery, Query, QueryClone, RangeQuery, RegexQuery, TermQuery};
 use tantivy::schema::{FacetParseError, Field, FieldEntry, FieldType, IndexRecordOption, Schema, TextFieldIndexing, Type};
 use tantivy::tokenizer::{TextAnalyzer, TokenizerManager};
 use tantivy::{Index, Term};
 use tantivy_query_grammar::Occur;
 
+use crate::components::query_parser::morphology::MorphologyManager;
 use crate::components::query_parser::proto_query_parser::QueryParserDefaultMode;
-use crate::components::query_parser::term_field_mappers::{DoiIsbnMapper, DoiMapper, IsbnMapper, TermFieldMapper};
+use crate::components::query_parser::term_field_mappers::TermFieldMappersManager;
+use crate::components::query_parser::utils::cast_field_to_term;
 use crate::configs::core::QueryParserConfig;
 use crate::errors::SummaResult;
 use crate::utils::transpose;
 use crate::validators;
 
 #[derive(Parser)]
 #[grammar = "src/components/query_parser/summa_ql.pest"] // relative to src
 struct SummaQlParser;
 
 pub struct QueryParser {
     schema: Schema,
     tokenizer_manager: TokenizerManager,
+    morphology_manager: MorphologyManager,
+    term_field_mappers_manager: TermFieldMappersManager,
     query_parser_config: QueryParserConfig,
 }
 
 /// Possible error that may happen when parsing a query.
 #[derive(thiserror::Error, Debug, PartialEq)]
 pub enum QueryParserError {
     /// Error in the query syntax
@@ -172,48 +175,35 @@
             return Box::new(EmptyQuery {}) as Box<dyn Query>;
         }
         return Box::new(BooleanQuery::new(subqueries)) as Box<dyn Query>;
     }
     query
 }
 
-pub fn cast_field_to_term(field: &Field, full_path: &str, field_type: &FieldType, value: &str, force_str: bool) -> Term {
-    match field_type {
-        FieldType::Str(_) => Term::from_field_text(*field, value),
-        FieldType::JsonObject(ref json_options) => {
-            let mut term = Term::with_capacity(128);
-            let mut json_term_writer = JsonTermWriter::from_field_and_json_path(*field, full_path, json_options.is_expand_dots_enabled(), &mut term);
-            if force_str {
-                json_term_writer.set_str(value);
-                json_term_writer.term().clone()
-            } else {
-                convert_to_fast_value_and_get_term(&mut json_term_writer, value).unwrap_or_else(|| {
-                    json_term_writer.set_str(value);
-                    json_term_writer.term().clone()
-                })
-            }
-        }
-        _ => unreachable!(),
-    }
-}
-
 type Subqueries = Vec<(Occur, Box<dyn Query>)>;
 
 impl QueryParser {
-    pub fn new(schema: Schema, query_parser_config: QueryParserConfig, tokenizer_manager: &TokenizerManager) -> SummaResult<QueryParser> {
+    pub fn new(
+        schema: Schema,
+        query_parser_config: QueryParserConfig,
+        morphology_manager: &MorphologyManager,
+        tokenizer_manager: &TokenizerManager,
+    ) -> SummaResult<QueryParser> {
         validators::parse_fields(&schema, &query_parser_config.0.default_fields)?;
         Ok(QueryParser {
-            schema,
+            term_field_mappers_manager: TermFieldMappersManager::new(&schema, tokenizer_manager),
+            morphology_manager: morphology_manager.clone(),
             tokenizer_manager: tokenizer_manager.clone(),
             query_parser_config,
+            schema,
         })
     }
 
-    pub fn for_index(index: &Index, query_parser_config: QueryParserConfig) -> SummaResult<QueryParser> {
-        QueryParser::new(index.schema(), query_parser_config, index.tokenizers())
+    pub fn for_index(index: &Index, query_parser_config: QueryParserConfig, morphology_manager: &MorphologyManager) -> SummaResult<QueryParser> {
+        QueryParser::new(index.schema(), query_parser_config, morphology_manager, index.tokenizers())
     }
 
     pub fn resolve_field_name<'a>(&'a self, field_name: &'a str) -> &str {
         self.query_parser_config
             .0
             .field_aliases
             .get(field_name)
@@ -301,15 +291,15 @@
             &left,
             &right,
         ))
     }
 
     fn parse_words(&self, field: Field, option: &TextFieldIndexing, words: &str) -> Result<Vec<(usize, Term)>, QueryParserError> {
         let field_entry = self.schema.get_field_entry(field);
-        let text_analyzer = self.get_text_analyzer(field_entry, option)?;
+        let mut text_analyzer = self.get_text_analyzer(field_entry, option)?;
         let mut token_stream = text_analyzer.token_stream(words);
         let mut terms = Vec::new();
         token_stream.process(&mut |token| {
             let term = Term::from_field_text(field, &token.text);
             terms.push((token.position, term));
         });
         Ok(terms)
@@ -388,60 +378,46 @@
                     json_options.get_text_indexing_options().expect("unreachable")
                 } else {
                     unreachable!()
                 };
 
                 match pre_term.as_rule() {
                     Rule::word | Rule::field_name => {
-                        let mut token_stream = self.get_text_analyzer(field_entry, indexing)?.token_stream(pre_term.as_str());
+                        let mut text_analyzer = self.get_text_analyzer(field_entry, indexing)?;
+                        let mut token_stream = text_analyzer.token_stream(pre_term.as_str());
                         let mut queries = Vec::new();
                         token_stream.process(&mut |token| {
-                            let term = cast_field_to_term(field, full_path, field_type, &token.text, false);
-                            let inflection_config = self
+                            let morphology_config = self
                                 .query_parser_config
                                 .0
-                                .inflection_configs
+                                .morphology_configs
                                 .get(field_entry.name())
                                 .cloned()
                                 .unwrap_or_default();
-                            if inflection_config.derive_plural {
-                                let is_singular = pluralize_rs::is_singular(&token.text);
-                                let is_plural = pluralize_rs::is_plural(&token.text);
-                                let other_token = if is_singular {
-                                    Some(pluralize_rs::to_plural(&token.text))
-                                } else if is_plural {
-                                    Some(pluralize_rs::to_singular(&token.text))
-                                } else {
-                                    None
-                                };
-                                if let Some(other_token) = other_token {
-                                    let other_term = cast_field_to_term(field, full_path, field_type, &other_token, false);
-                                    let disjunction_query = DisjunctionMaxQuery::new(vec![
-                                        Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>,
-                                        Box::new(TermQuery::new(other_term, IndexRecordOption::WithFreqs)) as Box<dyn Query>,
-                                    ]);
-                                    queries.push(boost_query(Box::new(disjunction_query) as Box<dyn Query>, boost))
-                                }
+                            let query = if let Some(morphology) = self.morphology_manager.get(self.query_parser_config.0.query_language()) {
+                                morphology.derive_query(morphology_config, field, full_path, field_type, &token.text)
                             } else {
-                                let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
-                                queries.push(boost_query(query, boost));
-                            }
+                                let term = cast_field_to_term(field, full_path, field_type, &token.text, false);
+                                Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>
+                            };
+                            queries.push(boost_query(query, boost))
                         });
                         Ok(queries)
                     }
                     Rule::phrase => {
                         let mut phrase_pairs = pre_term.into_inner();
                         let words = match phrase_pairs.next() {
                             None => return Ok(vec![]),
                             Some(words) => words,
                         };
 
                         match field_type {
                             FieldType::JsonObject(_) => {
-                                let mut token_stream = self.get_text_analyzer(field_entry, indexing)?.token_stream(words.as_str());
+                                let mut text_analyzer = self.get_text_analyzer(field_entry, indexing)?;
+                                let mut token_stream = text_analyzer.token_stream(words.as_str());
                                 let mut queries = Vec::new();
 
                                 token_stream.process(&mut |token| {
                                     let term = cast_field_to_term(field, full_path, field_type, &token.text, true);
                                     let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                                     queries.push(boost_query(query, boost));
                                 });
@@ -537,22 +513,22 @@
                 Ok(Term::from_field_bool(field, val))
             }
             FieldType::Str(ref str_options) => {
                 let option = str_options.get_indexing_options().ok_or_else(|| {
                     // This should have been seen earlier really.
                     QueryParserError::FieldNotIndexed(field_entry.name().to_string())
                 })?;
-                let text_analyzer = self
+                let mut terms: Vec<Term> = Vec::new();
+                let mut text_analyzer = self
                     .tokenizer_manager
                     .get(option.tokenizer())
                     .ok_or_else(|| QueryParserError::UnknownTokenizer {
                         field: field_entry.name().to_string(),
                         tokenizer: option.tokenizer().to_string(),
                     })?;
-                let mut terms: Vec<Term> = Vec::new();
                 let mut token_stream = text_analyzer.token_stream(phrase);
                 token_stream.process(&mut |token| {
                     let term = Term::from_field_text(field, &token.text);
                     terms.push(term);
                 });
                 if terms.len() != 1 {
                     return Err(QueryParserError::UnsupportedQuery(format!(
@@ -639,33 +615,40 @@
                         },
                     },
                     _ => unreachable!(),
                 }
             }
             Rule::doi => {
                 let mut queries = vec![];
-                let doi_mapper = Box::new(DoiMapper::new(self.schema.clone(), vec!["doi".to_string()])) as Box<dyn TermFieldMapper>;
-                let doi_isbn_mapper = Box::new(DoiIsbnMapper::new(self.schema.clone(), vec!["metadata.isbns".to_string()])) as Box<dyn TermFieldMapper>;
 
-                for mapper in &[doi_mapper, doi_isbn_mapper] {
-                    if let Some(query) = mapper.map(isbn_doi_or_search_group_or_term.as_str()) {
-                        queries.push((Occur::Should, query));
+                for term_field_mapper_name in ["doi", "doi_isbn"] {
+                    if let Some(term_field_mapper_config) = self.query_parser_config.0.term_field_mapper_configs.get(term_field_mapper_name) {
+                        if let Some(term_field_mapper) = self.term_field_mappers_manager.get(term_field_mapper_name) {
+                            if let Some(query) = term_field_mapper.map(isbn_doi_or_search_group_or_term.as_str(), &term_field_mapper_config.fields) {
+                                queries.push((Occur::Should, query));
+                            }
+                        }
                     }
                 }
+
                 Ok(Box::new(BooleanQuery::new(queries)) as Box<dyn Query>)
             }
             Rule::isbn => {
                 let mut queries = vec![];
-                let isbn_mapper = Box::new(IsbnMapper::new(self.schema.clone(), vec!["metadata.isbns".to_string()])) as Box<dyn TermFieldMapper>;
 
-                for mapper in &[isbn_mapper] {
-                    if let Some(query) = mapper.map(isbn_doi_or_search_group_or_term.as_str()) {
-                        queries.push((Occur::Should, query));
+                for term_field_mapper_name in ["isbn"] {
+                    if let Some(term_field_mapper_config) = self.query_parser_config.0.term_field_mapper_configs.get(term_field_mapper_name) {
+                        if let Some(term_field_mapper) = self.term_field_mappers_manager.get(term_field_mapper_name) {
+                            if let Some(query) = term_field_mapper.map(isbn_doi_or_search_group_or_term.as_str(), &term_field_mapper_config.fields) {
+                                queries.push((Occur::Should, query));
+                            }
+                        }
                     }
                 }
+
                 Ok(Box::new(BooleanQuery::new(queries)) as Box<dyn Query>)
             }
             Rule::term => self.default_field_queries(isbn_doi_or_search_group_or_term, statement_boost),
             e => panic!("{e:?}"),
         }?;
         Ok(statement_result)
     }
@@ -674,21 +657,62 @@
         let mut subqueries = Subqueries::new();
 
         for pair in pairs.clone() {
             let parsed_queries = self.parse_statement(pair)?;
             subqueries.push((Occur::Should, parsed_queries));
         }
 
-        if let Some(exact_matches_promoter) = &self.query_parser_config.0.exact_matches_promoter {
-            if let Some(top_level_phrase) = self.extract_top_level_phrase(pairs) {
+        if let Some(top_level_phrase) = self.extract_top_level_phrase(pairs) {
+            if let Some(ner_matches_promoter) = &self.query_parser_config.0.ner_matches_promoter {
+                if let Some(morphology) = self.morphology_manager.get(self.query_parser_config.0.query_language()) {
+                    let fields = if ner_matches_promoter.fields.is_empty() {
+                        self.query_parser_config.0.default_fields.iter()
+                    } else {
+                        ner_matches_promoter.fields.iter()
+                    };
+                    let entities = morphology.detect_ners(&top_level_phrase);
+                    subqueries.extend(
+                        fields
+                            .map(|field| {
+                                let mut subsubqueries = vec![];
+                                for entity in &entities {
+                                    let field = self.schema.get_field(field).expect("no field");
+                                    let field_entry = self.schema.get_field_entry(field);
+                                    let field_boost = self.query_parser_config.0.field_boosts.get(field_entry.name()).copied();
+                                    if let FieldType::Str(ref str_option) = field_entry.field_type() {
+                                        let Some(option) = str_option.get_indexing_options() else {
+                                        continue
+                                    };
+                                        let terms = match self.parse_words(field, option, entity) {
+                                            Ok(terms) => terms,
+                                            Err(err) => return Err(err),
+                                        };
+                                        if terms.len() > 1 && option.index_option().has_positions() {
+                                            let query = Box::new(PhraseQuery::new_with_offset(terms)) as Box<dyn Query>;
+                                            subsubqueries.push(boost_query(query, multiply_boosts(ner_matches_promoter.boost, field_boost)))
+                                        }
+                                    }
+                                }
+                                Ok(subsubqueries)
+                            })
+                            .collect::<Result<Vec<Vec<_>>, _>>()?
+                            .into_iter()
+                            .flatten()
+                            .map(|q| (Occur::Should, q)),
+                    )
+                }
+            }
+            if let Some(exact_matches_promoter) = &self.query_parser_config.0.exact_matches_promoter {
+                let fields = if exact_matches_promoter.fields.is_empty() {
+                    self.query_parser_config.0.default_fields.iter()
+                } else {
+                    exact_matches_promoter.fields.iter()
+                };
                 subqueries.extend(
-                    self.query_parser_config
-                        .0
-                        .default_fields
-                        .iter()
+                    fields
                         .filter_map(|field| {
                             let field = self.schema.get_field(field).expect("no field");
                             let field_entry = self.schema.get_field_entry(field);
                             let field_boost = self.query_parser_config.0.field_boosts.get(field_entry.name()).copied();
                             if let FieldType::Str(ref str_option) = field_entry.field_type() {
                                 let Some(option) = str_option.get_indexing_options() else {
                                     return None
@@ -728,38 +752,40 @@
     use tantivy::tokenizer::{LowerCaser, RemoveLongFilter};
 
     use super::*;
     use crate::components::SummaTokenizer;
 
     fn create_query_parser() -> QueryParser {
         let tokenizer_manager = TokenizerManager::default();
+        let morphology_manager = MorphologyManager::default();
         let mut schema_builder = Schema::builder();
         schema_builder.add_text_field("title", TEXT);
         schema_builder.add_text_field("body", TEXT);
         schema_builder.add_i64_field("timestamp", INDEXED);
         schema_builder.add_text_field("doi", STRING);
         schema_builder.add_text_field("isbns", STRING);
         schema_builder.add_json_field("metadata", TEXT);
         let schema = schema_builder.build();
         let query_parser_config = QueryParserConfig(proto::QueryParserConfig {
             default_fields: vec!["title".to_string()],
             ..Default::default()
         });
-        QueryParser::new(schema, query_parser_config, &tokenizer_manager).expect("cannot create parser")
+        QueryParser::new(schema, query_parser_config, &morphology_manager, &tokenizer_manager).expect("cannot create parser")
     }
 
     fn create_complex_query_parser() -> QueryParser {
         let tokenizer_manager = TokenizerManager::default();
         tokenizer_manager.register(
             "summa",
             TextAnalyzer::builder(SummaTokenizer)
                 .filter(RemoveLongFilter::limit(100))
                 .filter(LowerCaser)
                 .build(),
         );
+        let morphology_manager = MorphologyManager::default();
         let mut schema_builder = Schema::builder();
         let text_options = TextOptions::default().set_indexing_options(
             TextFieldIndexing::default()
                 .set_tokenizer("summa")
                 .set_index_option(IndexRecordOption::WithFreqsAndPositions),
         );
         schema_builder.add_text_field("title", text_options);
@@ -771,15 +797,15 @@
         schema_builder.add_text_field("isbns", STRING);
         schema_builder.add_json_field("metadata", TEXT);
         let schema = schema_builder.build();
         let query_parser_config = QueryParserConfig(proto::QueryParserConfig {
             default_fields: vec!["title".to_string(), "body".to_string()],
             ..Default::default()
         });
-        QueryParser::new(schema, query_parser_config, &tokenizer_manager).expect("cannot create parser")
+        QueryParser::new(schema, query_parser_config, &morphology_manager, &tokenizer_manager).expect("cannot create parser")
     }
 
     #[test]
     pub fn test_parser_base() {
         let query_parser = create_query_parser();
         let query = query_parser.parse_query("search engine");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })");
@@ -798,15 +824,33 @@
             format!("{:?}", query),
             "Ok(PhraseQuery { field: Field(1), phrase_terms: [(0, Term(field=1, type=Str, \"search\")), (1, Term(field=1, type=Str, \"engine\"))], slop: 4 })"
         );
     }
 
     #[test]
     pub fn test_parser_fields() {
-        let query_parser = create_query_parser();
+        let mut query_parser = create_query_parser();
+        query_parser.query_parser_config.0.term_field_mapper_configs.insert(
+            "doi".to_string(),
+            proto::TermFieldMapperConfig {
+                fields: vec!["doi".to_string()],
+            },
+        );
+        query_parser.query_parser_config.0.term_field_mapper_configs.insert(
+            "doi_isbn".to_string(),
+            proto::TermFieldMapperConfig {
+                fields: vec!["metadata.isbns".to_string()],
+            },
+        );
+        query_parser.query_parser_config.0.term_field_mapper_configs.insert(
+            "isbn".to_string(),
+            proto::TermFieldMapperConfig {
+                fields: vec!["metadata.isbns".to_string()],
+            },
+        );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:'search engine'")),
             "Ok(PhraseQuery { field: Field(1), phrase_terms: [(0, Term(field=1, type=Str, \"search\")), (1, Term(field=1, type=Str, \"engine\"))], slop: 0 })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("timestamp:10")),
             "Ok(TermQuery(Term(field=2, type=I64, 10)))"
@@ -846,15 +890,15 @@
         assert_eq!(
             format!("{:?}", query_parser.parse_query("9781234567890")),
             "Ok(TermQuery(Term(field=5, type=Json, path=isbns, type=Str, \"9781234567890\")))"
         );
         assert_eq!(format!("{:?}", query_parser.parse_query("97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"97812\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"5678\"))), (Should, TermQuery(Term(field=0, type=Str, \"909\")))] })");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("metadata.isbns:97812-34-5678-90")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 97812))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 34))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 5678))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 90)))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=5, type=Json, path=isbns, type=I64, 97812))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=I64, 34))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=I64, 5678))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=I64, 90)))] })"
         );
         assert_eq!(format!("{:?}", query_parser.parse_query("123 97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"123\"))), (Should, TermQuery(Term(field=0, type=Str, \"97812\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"5678\"))), (Should, TermQuery(Term(field=0, type=Str, \"909\")))] })");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("10.0000/cbo123")),
             "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/cbo123\")))"
         );
         assert_eq!(
@@ -968,15 +1012,15 @@
     }
 
     #[test]
     pub fn test_json() {
         let query_parser = create_query_parser();
         assert_eq!(
             format!("{:?}", query_parser.parse_query("metadata.a:1")),
-            "Ok(TermQuery(Term(field=5, type=Json, path=a, type=U64, 1)))"
+            "Ok(TermQuery(Term(field=5, type=Json, path=a, type=I64, 1)))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("metadata.a:\"1\"")),
             "Ok(TermQuery(Term(field=5, type=Json, path=a, type=Str, \"1\")))"
         );
     }
 
@@ -1049,27 +1093,58 @@
         let query = query_parser.parse_query("timestamp:(-[1100 to 1200] [ 1000 to 2000 ] -1500 +3000)");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(MustNot, RangeQuery { field: \"timestamp\", value_type: I64, lower_bound: Included([128, 0, 0, 0, 0, 0, 4, 76]), upper_bound: Included([128, 0, 0, 0, 0, 0, 4, 176]), limit: None }), (Should, RangeQuery { field: \"timestamp\", value_type: I64, lower_bound: Included([128, 0, 0, 0, 0, 0, 3, 232]), upper_bound: Included([128, 0, 0, 0, 0, 0, 7, 208]), limit: None }), (MustNot, TermQuery(Term(field=2, type=I64, 1500))), (Must, TermQuery(Term(field=2, type=I64, 3000)))] })");
     }
 
     #[test]
     pub fn test_exact_phrase_promoter() {
         let mut query_parser = create_query_parser();
-        query_parser.query_parser_config.0.exact_matches_promoter = Some(proto::ExactMatchesPromoter { slop: 3, boost: Some(2.0) });
+        query_parser.query_parser_config.0.exact_matches_promoter = Some(proto::ExactMatchesPromoter {
+            slop: 3,
+            boost: Some(2.0),
+            fields: vec![],
+        });
         let query = query_parser.parse_query("old school holy-wood");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"old\"))), (Should, TermQuery(Term(field=0, type=Str, \"school\"))), (Should, TermQuery(Term(field=0, type=Str, \"holy\"))), (Should, TermQuery(Term(field=0, type=Str, \"wood\"))), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"old\")), (1, Term(field=0, type=Str, \"school\")), (2, Term(field=0, type=Str, \"holy\")), (3, Term(field=0, type=Str, \"wood\"))], slop: 3 }, boost=2))] })");
         let query = query_parser.parse_query("old^2.0 school");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(field=0, type=Str, \"old\")), boost=2)), (Should, TermQuery(Term(field=0, type=Str, \"school\")))] })");
         query_parser.query_parser_config.0.field_boosts = HashMap::from_iter(vec![("title".to_string(), 3.0)]);
         let query = query_parser.parse_query("old school");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(field=0, type=Str, \"old\")), boost=3)), (Should, Boost(query=TermQuery(Term(field=0, type=Str, \"school\")), boost=3)), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"old\")), (1, Term(field=0, type=Str, \"school\"))], slop: 3 }, boost=6))] })");
     }
 
     #[test]
     pub fn test_inflection() {
         let mut query_parser = create_query_parser();
-        let mut inflection_configs = HashMap::new();
-        inflection_configs.insert("title".to_string(), proto::InflectionConfig { derive_plural: true });
-        query_parser.query_parser_config.0.inflection_configs = inflection_configs;
+        let mut morphology_configs = HashMap::new();
+        morphology_configs.insert(
+            "title".to_string(),
+            proto::MorphologyConfig {
+                derive_tenses_coefficient: Some(0.3),
+            },
+        );
+        query_parser.query_parser_config.0.morphology_configs = morphology_configs;
+        query_parser.query_parser_config.0.query_language = Some("en".to_string());
         let query = query_parser.parse_query("search engine");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"search\")), TermQuery(Term(field=0, type=Str, \"searches\"))], tie_breaker: 0.0 }), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.0 })] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.3 })] })");
+    }
+
+    #[test]
+    pub fn test_ner() {
+        let mut query_parser = create_query_parser();
+        let mut morphology_configs = HashMap::new();
+        morphology_configs.insert(
+            "en".to_string(),
+            proto::MorphologyConfig {
+                derive_tenses_coefficient: Some(0.3),
+            },
+        );
+        query_parser.query_parser_config.0.morphology_configs = morphology_configs;
+        query_parser.query_parser_config.0.ner_matches_promoter = Some(proto::NerMatchesPromoter {
+            boost: Some(1.3),
+            fields: vec!["title".to_string()],
+        });
+        query_parser.query_parser_config.0.query_language = Some("en".to_string());
+        let query = query_parser.parse_query("london is the capital of Great Britain");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"london\"))), (Should, TermQuery(Term(field=0, type=Str, \"is\"))), (Should, TermQuery(Term(field=0, type=Str, \"the\"))), (Should, TermQuery(Term(field=0, type=Str, \"capital\"))), (Should, TermQuery(Term(field=0, type=Str, \"of\"))), (Should, TermQuery(Term(field=0, type=Str, \"great\"))), (Should, TermQuery(Term(field=0, type=Str, \"britain\")))] })");
+        // assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"london\"))), (Should, TermQuery(Term(field=0, type=Str, \"is\"))), (Should, TermQuery(Term(field=0, type=Str, \"the\"))), (Should, TermQuery(Term(field=0, type=Str, \"capital\"))), (Should, TermQuery(Term(field=0, type=Str, \"of\"))), (Should, TermQuery(Term(field=0, type=Str, \"great\"))), (Should, TermQuery(Term(field=0, type=Str, \"britain\"))), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"great\")), (1, Term(field=0, type=Str, \"britain\"))], slop: 0 }, boost=1.3))] })");
     }
 }
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     chars: CharIndices<'a>,
     token: Token,
 }
 
 impl Tokenizer for SummaTokenizer {
     type TokenStream<'a> = SummaTokenStream<'a>;
 
-    fn token_stream<'a>(&self, text: &'a str) -> SummaTokenStream<'a> {
+    fn token_stream<'a>(&'a mut self, text: &'a str) -> SummaTokenStream<'a> {
         let mut chars = text.char_indices();
         SummaTokenStream {
             text,
             current_char_index: chars.next(),
             chars,
             token: Token::default(),
         }
@@ -105,15 +105,15 @@
         tokenizer_manager.register(
             "tokenizer",
             TextAnalyzer::builder(SummaTokenizer)
                 .filter(RemoveLongFilter::limit(40))
                 .filter(LowerCaser)
                 .build(),
         );
-        let tokenizer = tokenizer_manager.get("tokenizer").unwrap();
+        let mut tokenizer = tokenizer_manager.get("tokenizer").unwrap();
         let mut tokens: Vec<Token> = vec![];
         {
             let mut add_token = |token: &Token| {
                 tokens.push(token.clone());
             };
             tokenizer.token_stream("Hello, world!").process(&mut add_token);
         }
@@ -129,15 +129,15 @@
         tokenizer_manager.register(
             "tokenizer",
             TextAnalyzer::builder(SummaTokenizer)
                 .filter(RemoveLongFilter::limit(40))
                 .filter(LowerCaser)
                 .build(),
         );
-        let tokenizer = tokenizer_manager.get("tokenizer").unwrap();
+        let mut tokenizer = tokenizer_manager.get("tokenizer").unwrap();
         let mut tokens: Vec<Token> = vec![];
         {
             let mut add_token = |token: &Token| {
                 tokens.push(token.clone());
             };
             tokenizer.token_stream("在查hello, worl土d动!").process(&mut add_token);
         }
@@ -157,15 +157,15 @@
         tokenizer_manager.register(
             "tokenizer",
             TextAnalyzer::builder(SummaTokenizer)
                 .filter(RemoveLongFilter::limit(40))
                 .filter(LowerCaser)
                 .build(),
         );
-        let tokenizer = tokenizer_manager.get("tokenizer").unwrap();
+        let mut tokenizer = tokenizer_manager.get("tokenizer").unwrap();
         let mut tokens: Vec<Token> = vec![];
         {
             let mut add_token = |token: &Token| {
                 tokens.push(token.clone());
             };
             tokenizer.token_stream("Veri 在查hello, c查m p查 查lex  worl土d动!").process(&mut add_token);
         }
@@ -192,15 +192,15 @@
         tokenizer_manager.register(
             "tokenizer",
             TextAnalyzer::builder(SummaTokenizer)
                 .filter(RemoveLongFilter::limit(40))
                 .filter(LowerCaser)
                 .build(),
         );
-        let tokenizer = tokenizer_manager.get("tokenizer").unwrap();
+        let mut tokenizer = tokenizer_manager.get("tokenizer").unwrap();
         let mut tokens: Vec<Token> = vec![];
         {
             let mut add_token = |token: &Token| {
                 tokens.push(token.clone());
             };
             tokenizer.token_stream("。").process(&mut add_token);
         }
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.0/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.0/local_dependencies/summa-proto/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-proto"
-version = "0.27.0"
+version = "0.28.0"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa search server proto files"
 
 [lib]
 name = "summa_proto"
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.0/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.0/local_dependencies/summa-proto/build.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,19 @@
         "proto/utils.proto",
     ];
     let serde_default_structs = &[
         "dag_pb.PBNode",
         "dag_pb.PBLink",
         "summa.proto.HistogramAggregation",
         "summa.proto.IndexAttributes",
+        "summa.proto.InflectionConfig",
         "summa.proto.MoreLikeThisQuery",
+        "summa.proto.NerMatchConfig",
         "summa.proto.PhraseQuery",
+        "summa.proto.QueryParserConfig",
         "summa.proto.ReservoirSamplingCollector",
         "summa.proto.TermsAggregation",
         "summa.proto.TopDocsCollector",
         "unixfs.Data",
     ];
     #[cfg(feature = "grpc")]
     build_tonic(files, serde_default_structs)?;
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.0/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.0/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.0/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files 2% similar despite different names*

```diff
@@ -146,20 +146,16 @@
 message IndexAttributes {
   // Timestamp when index has been created
   uint64 created_at = 1;
   // Unique fields of the index. Summa maintains unique constraint on them and uses for deduplicating data
   repeated string unique_fields = 2;
   // Multi fields is ones that may have multiple values and processed as lists. All other fields will be forcefully converted to singular value
   repeated string multi_fields = 4;
-  // Descriptive field that may be used as name for index when indices are replicating over wire
-  optional string default_index_name = 5;
   // Text index description
   optional string description = 6;
-  // (Not-used)
-  repeated string default_snippets = 7;
   ConflictStrategy conflict_strategy = 8;
 }
 
 // Request for index creation
 message CreateIndexRequest {
   // Index name
   string index_name = 1;
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.0/local_dependencies/summa-proto/proto/query.proto`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 syntax = "proto3";
 package summa.proto;
 
 import "utils.proto";
 
-message FieldMapper {
-  string mapper_name = 1;
-  repeated string fields = 2;
+message TermFieldMapperConfig {
+  repeated string fields = 1;
 }
 
 message MatchQueryBooleanShouldMode {};
 message MatchQueryDisjuctionMaxMode {
   float tie_breaker = 1;
 };
 message ExactMatchesPromoter {
   uint32 slop = 1;
   optional float boost = 2;
+  repeated string fields = 3;
+}
+message NerMatchesPromoter {
+  optional float boost = 1;
+  repeated string fields = 2;
 }
 enum MissingFieldPolicy {
   AsUsualTerms = 0;
   Remove = 1;
   Fail = 2;
 }
 
-message InflectionConfig {
-  bool derive_plural = 1;
+message MorphologyConfig {
+  optional float derive_tenses_coefficient = 1;
 }
 
 message QueryParserConfig {
   map<string, string> field_aliases = 1;
   map<string, float> field_boosts = 2;
-  map<string, FieldMapper> field_mappings = 3;
+  map<string, TermFieldMapperConfig> term_field_mapper_configs = 3;
   uint32 term_limit = 4;
   repeated string default_fields = 5;
   oneof default_mode {
     MatchQueryBooleanShouldMode boolean_should_mode = 6;
     MatchQueryDisjuctionMaxMode disjuction_max_mode = 7;
   }
   ExactMatchesPromoter exact_matches_promoter = 8;
   MissingFieldPolicy missing_field_policy = 9;
-  map<string, InflectionConfig> inflection_configs = 10;
+  map<string, MorphologyConfig> morphology_configs = 10;
+  optional string query_language = 11;
+  NerMatchesPromoter ner_matches_promoter = 12;
 }
 
 message SearchResponse {
   // Time spent inside of `search` handler
   double elapsed_secs = 1;
   // An array of collector outputs
   repeated CollectorOutput collector_outputs = 2;
```

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.0/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.0/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.0/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.0/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/Cargo.toml` & `summa_embed-0.17.0/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "summa-embed-py"
-version = "0.16.0"
+version = "0.17.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
 [dependencies]
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.8"
 serde_json = "1.0"
-summa-core = { version = "0.16.0", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.0", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.16.0/.gitignore` & `summa_embed-0.17.0/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/pyproject.toml` & `summa_embed-0.17.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/src/lib.rs` & `summa_embed-0.17.0/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -53,17 +53,18 @@
         let core_config = Arc::new(DirectProxy::new(core_config)) as Arc<dyn ConfigProxy<_>>;
         IndexRegistry {
             index_registry: summa_core::components::IndexRegistry::new(&core_config),
             core_config,
         }
     }
 
-    fn add<'a>(&'a self, py: Python<'a>, index_engine_config: &PyBytes, index_name: Option<String>) -> PyResult<&'a PyAny> {
+    fn add<'a>(&'a self, py: Python<'a>, index_engine_config: &PyBytes, index_name: &str) -> PyResult<&'a PyAny> {
         let index_engine_config = proto::IndexEngineConfig::decode(index_engine_config.as_bytes()).unwrap();
         let this = self.clone();
+        let index_name = index_name.to_string();
         pyo3_asyncio::tokio::future_into_py(py, async move {
             let index = match &index_engine_config.config {
                 Some(proto::index_engine_config::Config::Memory(memory_engine_config)) => {
                     let schema = serde_json::from_str(&memory_engine_config.schema).unwrap();
                     let index_builder = IndexBuilder::new().schema(schema);
                     IndexHolder::create_memory_index(index_builder).unwrap()
                 }
@@ -76,15 +77,15 @@
                 _ => unimplemented!(),
             };
             let core_config = this.core_config.read().await.get().clone();
             let query_parser_config = index_engine_config.query_parser_config.as_ref().cloned().unwrap_or_default();
             let index_holder = IndexHolder::create_holder(
                 &core_config,
                 index,
-                index_name.as_deref(),
+                &index_name,
                 Arc::new(DirectProxy::new(index_engine_config)),
                 None,
                 query_parser_config,
                 Driver::current_tokio(),
             )
             .unwrap();
             let index_attributes = index_holder.index_attributes().cloned().unwrap();
```

### Comparing `summa_embed-0.16.0/summa_embed/__init__.py` & `summa_embed-0.17.0/summa_embed/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .summa_embed_bin import IndexRegistry as IndexRegistryBin
 
 
 class IndexRegistry:
     def __init__(self):
         self.index_registry = IndexRegistryBin()
 
-    async def add(self, index_config, index_name: Optional[str] = None) -> index_service_pb2.IndexAttributes:
+    async def add(self, index_config, index_name: str) -> index_service_pb2.IndexAttributes:
         parsed_index_config = index_service_pb2.IndexEngineConfig()
         ParseDict(index_config, parsed_index_config)
         index_attributes_bytes = await self.index_registry.add(
             parsed_index_config.SerializeToString(),
             index_name=index_name,
         )
         index_attributes = index_service_pb2.IndexAttributes()
```

### Comparing `summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/consumer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.pyi` & `summa_embed-0.17.0/summa_embed/proto/consumer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/dag_pb_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.pyi` & `summa_embed-0.17.0/summa_embed/proto/dag_pb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/index_service_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/index_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import query_pb2 as query__pb2
 from . import utils_pb2 as utils__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13index_service.proto\x12\x0bsumma.proto\x1a\x0bquery.proto\x1a\x0butils.proto\"3\n\nPrimaryKey\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03i64\x18\x02 \x01(\x03H\x00\x42\x07\n\x05value\"\x7f\n\x0bMergePolicy\x12*\n\x03log\x18\x0b \x01(\x0b\x32\x1b.summa.proto.LogMergePolicyH\x00\x12\x34\n\x08temporal\x18\x0c \x01(\x0b\x32 .summa.proto.TemporalMergePolicyH\x00\x42\x0e\n\x0cmerge_policy\"\x19\n\x17\x41ttachFileEngineRequest\"L\n\x19\x41ttachRemoteEngineRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfig\"\x95\x02\n\x12\x41ttachIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x02 \x01(\x0b\x32$.summa.proto.AttachFileEngineRequestH\x00\x12\x38\n\x06remote\x18\x03 \x01(\x0b\x32&.summa.proto.AttachRemoteEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x0b \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigB\x0e\n\x0cindex_engine\"C\n\x13\x41ttachIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"(\n\x12\x43ommitIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"+\n\x13\x43ommitIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\"L\n\x14\x43opyDocumentsRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\"G\n\x15\x43opyDocumentsResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x18\n\x10\x63opied_documents\x18\x02 \x01(\r\"\xff\x01\n\x10\x43opyIndexRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\x12\x34\n\x04\x66ile\x18\x03 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x04 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\x06 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x15\n\x13target_index_engine\"A\n\x11\x43opyIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"?\n\x0bSortByField\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.Order\"\x19\n\x17\x43reateFileEngineRequest\"\x1b\n\x19\x43reateMemoryEngineRequest\"\x88\x02\n\x0fIndexAttributes\x12\x12\n\ncreated_at\x18\x01 \x01(\x04\x12\x15\n\runique_fields\x18\x02 \x03(\t\x12\x14\n\x0cmulti_fields\x18\x04 \x03(\t\x12\x1f\n\x12\x64\x65\x66\x61ult_index_name\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x10\x64\x65\x66\x61ult_snippets\x18\x07 \x03(\t\x12\x38\n\x11\x63onflict_strategy\x18\x08 \x01(\x0e\x32\x1d.summa.proto.ConflictStrategyB\x15\n\x13_default_index_nameB\x0e\n\x0c_description\"\xfa\x03\n\x12\x43reateIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x07 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x08 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12-\n\x0b\x63ompression\x18\x03 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x16\n\tblocksize\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x34\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x02\x88\x01\x01\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\x12.\n\x0cmerge_policy\x18\x14 \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x15 \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigB\x0e\n\x0cindex_engineB\x0c\n\n_blocksizeB\x10\n\x0e_sort_by_field\"C\n\x13\x43reateIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"O\n\x16\x44\x65leteDocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"4\n\x17\x44\x65leteDocumentsResponse\x12\x19\n\x11\x64\x65leted_documents\x18\x01 \x01(\x04\"(\n\x12\x44\x65leteIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"1\n\x13\x44\x65leteIndexResponse\x12\x1a\n\x12\x64\x65leted_index_name\x18\x01 \x01(\t\"\x1a\n\x18GetIndicesAliasesRequest\"\xa7\x01\n\x19GetIndicesAliasesResponse\x12S\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntry\x1a\x35\n\x13IndicesAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"%\n\x0fGetIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"@\n\x10GetIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"\x13\n\x11GetIndicesRequest\")\n\x12GetIndicesResponse\x12\x13\n\x0bindex_names\x18\x01 \x03(\t\"C\n\x1aIndexDocumentStreamRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x11\n\tdocuments\x18\x02 \x03(\x0c\"^\n\x1bIndexDocumentStreamResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x14\n\x0csuccess_docs\x18\x02 \x01(\x04\x12\x13\n\x0b\x66\x61iled_docs\x18\x03 \x01(\x04\"<\n\x14IndexDocumentRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocument\x18\x02 \x01(\x0c\"\x17\n\x15IndexDocumentResponse\"?\n\x14MergeSegmentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x13\n\x0bsegment_ids\x18\x02 \x03(\t\"?\n\x15MergeSegmentsResponse\x12\x17\n\nsegment_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_segment_id\"?\n\x14SetIndexAliasRequest\x12\x13\n\x0bindex_alias\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"G\n\x15SetIndexAliasResponse\x12\x1b\n\x0eold_index_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_old_index_name\"6\n\x10\x44ocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"%\n\x11\x44ocumentsResponse\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\"C\n\x12VacuumIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x19\n\x11\x65xcluded_segments\x18\x02 \x03(\t\"0\n\x13VacuumIndexResponse\x12\x19\n\x11\x66reed_space_bytes\x18\x01 \x01(\x04\"9\n\x12WarmupIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07is_full\x18\x02 \x01(\x08\"+\n\x13WarmupIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\" \n\x10\x46ileEngineConfig\x12\x0c\n\x04path\x18\x01 \x01(\t\"$\n\x12MemoryEngineConfig\x12\x0e\n\x06schema\x18\x01 \x01(\t\"!\n\x0b\x43\x61\x63heConfig\x12\x12\n\ncache_size\x18\x01 \x01(\x04\"\x9a\x02\n\x12RemoteEngineConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x14\n\x0curl_template\x18\x02 \x01(\t\x12N\n\x10headers_template\x18\x03 \x03(\x0b\x32\x34.summa.proto.RemoteEngineConfig.HeadersTemplateEntry\x12.\n\x0c\x63\x61\x63he_config\x18\x04 \x01(\x0b\x32\x18.summa.proto.CacheConfig\x12\x17\n\ntimeout_ms\x18\x05 \x01(\rH\x00\x88\x01\x01\x1a\x36\n\x14HeadersTemplateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\r\n\x0b_timeout_ms\"#\n\x0eLogMergePolicy\x12\x11\n\tis_frozen\x18\x01 \x01(\x08\"4\n\x13TemporalMergePolicy\x12\x1d\n\x15merge_older_then_secs\x18\x01 \x01(\x04\"\xa0\x03\n\x11IndexEngineConfig\x12-\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x1d.summa.proto.FileEngineConfigH\x00\x12\x31\n\x06memory\x18\x02 \x01(\x0b\x32\x1f.summa.proto.MemoryEngineConfigH\x00\x12\x31\n\x06remote\x18\x03 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfigH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x0b \x01(\x0b\x32\x1e.summa.proto.QueryParserConfig\x12I\n\x0e\x66ield_triggers\x18\x0c \x03(\x0b\x32\x31.summa.proto.IndexEngineConfig.FieldTriggersEntry\x1a\x34\n\x12\x46ieldTriggersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\n\x06\x63onfig\"\xec\x01\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x15\n\rindex_aliases\x18\x02 \x03(\t\x12\x34\n\x0cindex_engine\x18\x03 \x01(\x0b\x32\x1e.summa.proto.IndexEngineConfig\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12-\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\"*\n\x16IndexDocumentOperation\x12\x10\n\x08\x64ocument\x18\x01 \x01(\x0c\"\\\n\x0eIndexOperation\x12=\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00\x42\x0b\n\toperation*R\n\x10\x43onflictStrategy\x12\x0e\n\nDO_NOTHING\x10\x00\x12\x14\n\x10OVERWRITE_ALWAYS\x10\x01\x12\r\n\tOVERWRITE\x10\x02\x12\t\n\x05MERGE\x10\x03*|\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04\x12\t\n\x05Zstd7\x10\x05\x12\t\n\x05Zstd9\x10\x06\x12\n\n\x06Zstd14\x10\x07\x12\n\n\x06Zstd19\x10\x08\x12\n\n\x06Zstd22\x10\t2\xeb\x0b\n\x08IndexApi\x12S\n\x0c\x61ttach_index\x12\x1f.summa.proto.AttachIndexRequest\x1a .summa.proto.AttachIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12Y\n\x0e\x63opy_documents\x12!.summa.proto.CopyDocumentsRequest\x1a\".summa.proto.CopyDocumentsResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12M\n\ncopy_index\x12\x1d.summa.proto.CopyIndexRequest\x1a\x1e.summa.proto.CopyIndexResponse\"\x00\x12_\n\x10\x64\x65lete_documents\x12#.summa.proto.DeleteDocumentsRequest\x1a$.summa.proto.DeleteDocumentsResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12N\n\tdocuments\x12\x1d.summa.proto.DocumentsRequest\x1a\x1e.summa.proto.DocumentsResponse\"\x00\x30\x01\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x12S\n\x0cwarmup_index\x12\x1f.summa.proto.WarmupIndexRequest\x1a .summa.proto.WarmupIndexResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13index_service.proto\x12\x0bsumma.proto\x1a\x0bquery.proto\x1a\x0butils.proto\"3\n\nPrimaryKey\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03i64\x18\x02 \x01(\x03H\x00\x42\x07\n\x05value\"\x7f\n\x0bMergePolicy\x12*\n\x03log\x18\x0b \x01(\x0b\x32\x1b.summa.proto.LogMergePolicyH\x00\x12\x34\n\x08temporal\x18\x0c \x01(\x0b\x32 .summa.proto.TemporalMergePolicyH\x00\x42\x0e\n\x0cmerge_policy\"\x19\n\x17\x41ttachFileEngineRequest\"L\n\x19\x41ttachRemoteEngineRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfig\"\x95\x02\n\x12\x41ttachIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x02 \x01(\x0b\x32$.summa.proto.AttachFileEngineRequestH\x00\x12\x38\n\x06remote\x18\x03 \x01(\x0b\x32&.summa.proto.AttachRemoteEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x0b \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigB\x0e\n\x0cindex_engine\"C\n\x13\x41ttachIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"(\n\x12\x43ommitIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"+\n\x13\x43ommitIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\"L\n\x14\x43opyDocumentsRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\"G\n\x15\x43opyDocumentsResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x18\n\x10\x63opied_documents\x18\x02 \x01(\r\"\xff\x01\n\x10\x43opyIndexRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\x12\x34\n\x04\x66ile\x18\x03 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x04 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\x06 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x15\n\x13target_index_engine\"A\n\x11\x43opyIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"?\n\x0bSortByField\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.Order\"\x19\n\x17\x43reateFileEngineRequest\"\x1b\n\x19\x43reateMemoryEngineRequest\"\xb6\x01\n\x0fIndexAttributes\x12\x12\n\ncreated_at\x18\x01 \x01(\x04\x12\x15\n\runique_fields\x18\x02 \x03(\t\x12\x14\n\x0cmulti_fields\x18\x04 \x03(\t\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x00\x88\x01\x01\x12\x38\n\x11\x63onflict_strategy\x18\x08 \x01(\x0e\x32\x1d.summa.proto.ConflictStrategyB\x0e\n\x0c_description\"\xfa\x03\n\x12\x43reateIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x07 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x08 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12-\n\x0b\x63ompression\x18\x03 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x16\n\tblocksize\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x34\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x02\x88\x01\x01\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\x12.\n\x0cmerge_policy\x18\x14 \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x15 \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigB\x0e\n\x0cindex_engineB\x0c\n\n_blocksizeB\x10\n\x0e_sort_by_field\"C\n\x13\x43reateIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"O\n\x16\x44\x65leteDocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"4\n\x17\x44\x65leteDocumentsResponse\x12\x19\n\x11\x64\x65leted_documents\x18\x01 \x01(\x04\"(\n\x12\x44\x65leteIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"1\n\x13\x44\x65leteIndexResponse\x12\x1a\n\x12\x64\x65leted_index_name\x18\x01 \x01(\t\"\x1a\n\x18GetIndicesAliasesRequest\"\xa7\x01\n\x19GetIndicesAliasesResponse\x12S\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntry\x1a\x35\n\x13IndicesAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"%\n\x0fGetIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"@\n\x10GetIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"\x13\n\x11GetIndicesRequest\")\n\x12GetIndicesResponse\x12\x13\n\x0bindex_names\x18\x01 \x03(\t\"C\n\x1aIndexDocumentStreamRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x11\n\tdocuments\x18\x02 \x03(\x0c\"^\n\x1bIndexDocumentStreamResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x14\n\x0csuccess_docs\x18\x02 \x01(\x04\x12\x13\n\x0b\x66\x61iled_docs\x18\x03 \x01(\x04\"<\n\x14IndexDocumentRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocument\x18\x02 \x01(\x0c\"\x17\n\x15IndexDocumentResponse\"?\n\x14MergeSegmentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x13\n\x0bsegment_ids\x18\x02 \x03(\t\"?\n\x15MergeSegmentsResponse\x12\x17\n\nsegment_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_segment_id\"?\n\x14SetIndexAliasRequest\x12\x13\n\x0bindex_alias\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"G\n\x15SetIndexAliasResponse\x12\x1b\n\x0eold_index_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_old_index_name\"6\n\x10\x44ocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"%\n\x11\x44ocumentsResponse\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\"C\n\x12VacuumIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x19\n\x11\x65xcluded_segments\x18\x02 \x03(\t\"0\n\x13VacuumIndexResponse\x12\x19\n\x11\x66reed_space_bytes\x18\x01 \x01(\x04\"9\n\x12WarmupIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07is_full\x18\x02 \x01(\x08\"+\n\x13WarmupIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\" \n\x10\x46ileEngineConfig\x12\x0c\n\x04path\x18\x01 \x01(\t\"$\n\x12MemoryEngineConfig\x12\x0e\n\x06schema\x18\x01 \x01(\t\"!\n\x0b\x43\x61\x63heConfig\x12\x12\n\ncache_size\x18\x01 \x01(\x04\"\x9a\x02\n\x12RemoteEngineConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x14\n\x0curl_template\x18\x02 \x01(\t\x12N\n\x10headers_template\x18\x03 \x03(\x0b\x32\x34.summa.proto.RemoteEngineConfig.HeadersTemplateEntry\x12.\n\x0c\x63\x61\x63he_config\x18\x04 \x01(\x0b\x32\x18.summa.proto.CacheConfig\x12\x17\n\ntimeout_ms\x18\x05 \x01(\rH\x00\x88\x01\x01\x1a\x36\n\x14HeadersTemplateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\r\n\x0b_timeout_ms\"#\n\x0eLogMergePolicy\x12\x11\n\tis_frozen\x18\x01 \x01(\x08\"4\n\x13TemporalMergePolicy\x12\x1d\n\x15merge_older_then_secs\x18\x01 \x01(\x04\"\xa0\x03\n\x11IndexEngineConfig\x12-\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x1d.summa.proto.FileEngineConfigH\x00\x12\x31\n\x06memory\x18\x02 \x01(\x0b\x32\x1f.summa.proto.MemoryEngineConfigH\x00\x12\x31\n\x06remote\x18\x03 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfigH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x0b \x01(\x0b\x32\x1e.summa.proto.QueryParserConfig\x12I\n\x0e\x66ield_triggers\x18\x0c \x03(\x0b\x32\x31.summa.proto.IndexEngineConfig.FieldTriggersEntry\x1a\x34\n\x12\x46ieldTriggersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\n\x06\x63onfig\"\xec\x01\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x15\n\rindex_aliases\x18\x02 \x03(\t\x12\x34\n\x0cindex_engine\x18\x03 \x01(\x0b\x32\x1e.summa.proto.IndexEngineConfig\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12-\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\"*\n\x16IndexDocumentOperation\x12\x10\n\x08\x64ocument\x18\x01 \x01(\x0c\"\\\n\x0eIndexOperation\x12=\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00\x42\x0b\n\toperation*R\n\x10\x43onflictStrategy\x12\x0e\n\nDO_NOTHING\x10\x00\x12\x14\n\x10OVERWRITE_ALWAYS\x10\x01\x12\r\n\tOVERWRITE\x10\x02\x12\t\n\x05MERGE\x10\x03*|\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04\x12\t\n\x05Zstd7\x10\x05\x12\t\n\x05Zstd9\x10\x06\x12\n\n\x06Zstd14\x10\x07\x12\n\n\x06Zstd19\x10\x08\x12\n\n\x06Zstd22\x10\t2\xeb\x0b\n\x08IndexApi\x12S\n\x0c\x61ttach_index\x12\x1f.summa.proto.AttachIndexRequest\x1a .summa.proto.AttachIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12Y\n\x0e\x63opy_documents\x12!.summa.proto.CopyDocumentsRequest\x1a\".summa.proto.CopyDocumentsResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12M\n\ncopy_index\x12\x1d.summa.proto.CopyIndexRequest\x1a\x1e.summa.proto.CopyIndexResponse\"\x00\x12_\n\x10\x64\x65lete_documents\x12#.summa.proto.DeleteDocumentsRequest\x1a$.summa.proto.DeleteDocumentsResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12N\n\tdocuments\x12\x1d.summa.proto.DocumentsRequest\x1a\x1e.summa.proto.DocumentsResponse\"\x00\x30\x01\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x12S\n\x0cwarmup_index\x12\x1f.summa.proto.WarmupIndexRequest\x1a .summa.proto.WarmupIndexResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'index_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_options = b'8\001'
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._options = None
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_options = b'8\001'
   _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._options = None
   _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_options = b'8\001'
-  _CONFLICTSTRATEGY._serialized_start=4939
-  _CONFLICTSTRATEGY._serialized_end=5021
-  _COMPRESSION._serialized_start=5023
-  _COMPRESSION._serialized_end=5147
+  _CONFLICTSTRATEGY._serialized_start=4857
+  _CONFLICTSTRATEGY._serialized_end=4939
+  _COMPRESSION._serialized_start=4941
+  _COMPRESSION._serialized_end=5065
   _PRIMARYKEY._serialized_start=62
   _PRIMARYKEY._serialized_end=113
   _MERGEPOLICY._serialized_start=115
   _MERGEPOLICY._serialized_end=242
   _ATTACHFILEENGINEREQUEST._serialized_start=244
   _ATTACHFILEENGINEREQUEST._serialized_end=269
   _ATTACHREMOTEENGINEREQUEST._serialized_start=271
@@ -59,89 +59,89 @@
   _SORTBYFIELD._serialized_start=1261
   _SORTBYFIELD._serialized_end=1324
   _CREATEFILEENGINEREQUEST._serialized_start=1326
   _CREATEFILEENGINEREQUEST._serialized_end=1351
   _CREATEMEMORYENGINEREQUEST._serialized_start=1353
   _CREATEMEMORYENGINEREQUEST._serialized_end=1380
   _INDEXATTRIBUTES._serialized_start=1383
-  _INDEXATTRIBUTES._serialized_end=1647
-  _CREATEINDEXREQUEST._serialized_start=1650
-  _CREATEINDEXREQUEST._serialized_end=2156
-  _CREATEINDEXRESPONSE._serialized_start=2158
-  _CREATEINDEXRESPONSE._serialized_end=2225
-  _DELETEDOCUMENTSREQUEST._serialized_start=2227
-  _DELETEDOCUMENTSREQUEST._serialized_end=2306
-  _DELETEDOCUMENTSRESPONSE._serialized_start=2308
-  _DELETEDOCUMENTSRESPONSE._serialized_end=2360
-  _DELETEINDEXREQUEST._serialized_start=2362
-  _DELETEINDEXREQUEST._serialized_end=2402
-  _DELETEINDEXRESPONSE._serialized_start=2404
-  _DELETEINDEXRESPONSE._serialized_end=2453
-  _GETINDICESALIASESREQUEST._serialized_start=2455
-  _GETINDICESALIASESREQUEST._serialized_end=2481
-  _GETINDICESALIASESRESPONSE._serialized_start=2484
-  _GETINDICESALIASESRESPONSE._serialized_end=2651
-  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_start=2598
-  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_end=2651
-  _GETINDEXREQUEST._serialized_start=2653
-  _GETINDEXREQUEST._serialized_end=2690
-  _GETINDEXRESPONSE._serialized_start=2692
-  _GETINDEXRESPONSE._serialized_end=2756
-  _GETINDICESREQUEST._serialized_start=2758
-  _GETINDICESREQUEST._serialized_end=2777
-  _GETINDICESRESPONSE._serialized_start=2779
-  _GETINDICESRESPONSE._serialized_end=2820
-  _INDEXDOCUMENTSTREAMREQUEST._serialized_start=2822
-  _INDEXDOCUMENTSTREAMREQUEST._serialized_end=2889
-  _INDEXDOCUMENTSTREAMRESPONSE._serialized_start=2891
-  _INDEXDOCUMENTSTREAMRESPONSE._serialized_end=2985
-  _INDEXDOCUMENTREQUEST._serialized_start=2987
-  _INDEXDOCUMENTREQUEST._serialized_end=3047
-  _INDEXDOCUMENTRESPONSE._serialized_start=3049
-  _INDEXDOCUMENTRESPONSE._serialized_end=3072
-  _MERGESEGMENTSREQUEST._serialized_start=3074
-  _MERGESEGMENTSREQUEST._serialized_end=3137
-  _MERGESEGMENTSRESPONSE._serialized_start=3139
-  _MERGESEGMENTSRESPONSE._serialized_end=3202
-  _SETINDEXALIASREQUEST._serialized_start=3204
-  _SETINDEXALIASREQUEST._serialized_end=3267
-  _SETINDEXALIASRESPONSE._serialized_start=3269
-  _SETINDEXALIASRESPONSE._serialized_end=3340
-  _DOCUMENTSREQUEST._serialized_start=3342
-  _DOCUMENTSREQUEST._serialized_end=3396
-  _DOCUMENTSRESPONSE._serialized_start=3398
-  _DOCUMENTSRESPONSE._serialized_end=3435
-  _VACUUMINDEXREQUEST._serialized_start=3437
-  _VACUUMINDEXREQUEST._serialized_end=3504
-  _VACUUMINDEXRESPONSE._serialized_start=3506
-  _VACUUMINDEXRESPONSE._serialized_end=3554
-  _WARMUPINDEXREQUEST._serialized_start=3556
-  _WARMUPINDEXREQUEST._serialized_end=3613
-  _WARMUPINDEXRESPONSE._serialized_start=3615
-  _WARMUPINDEXRESPONSE._serialized_end=3658
-  _FILEENGINECONFIG._serialized_start=3660
-  _FILEENGINECONFIG._serialized_end=3692
-  _MEMORYENGINECONFIG._serialized_start=3694
-  _MEMORYENGINECONFIG._serialized_end=3730
-  _CACHECONFIG._serialized_start=3732
-  _CACHECONFIG._serialized_end=3765
-  _REMOTEENGINECONFIG._serialized_start=3768
-  _REMOTEENGINECONFIG._serialized_end=4050
-  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_start=3981
-  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_end=4035
-  _LOGMERGEPOLICY._serialized_start=4052
-  _LOGMERGEPOLICY._serialized_end=4087
-  _TEMPORALMERGEPOLICY._serialized_start=4089
-  _TEMPORALMERGEPOLICY._serialized_end=4141
-  _INDEXENGINECONFIG._serialized_start=4144
-  _INDEXENGINECONFIG._serialized_end=4560
-  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_start=4498
-  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_end=4550
-  _INDEXDESCRIPTION._serialized_start=4563
-  _INDEXDESCRIPTION._serialized_end=4799
-  _INDEXDOCUMENTOPERATION._serialized_start=4801
-  _INDEXDOCUMENTOPERATION._serialized_end=4843
-  _INDEXOPERATION._serialized_start=4845
-  _INDEXOPERATION._serialized_end=4937
-  _INDEXAPI._serialized_start=5150
-  _INDEXAPI._serialized_end=6665
+  _INDEXATTRIBUTES._serialized_end=1565
+  _CREATEINDEXREQUEST._serialized_start=1568
+  _CREATEINDEXREQUEST._serialized_end=2074
+  _CREATEINDEXRESPONSE._serialized_start=2076
+  _CREATEINDEXRESPONSE._serialized_end=2143
+  _DELETEDOCUMENTSREQUEST._serialized_start=2145
+  _DELETEDOCUMENTSREQUEST._serialized_end=2224
+  _DELETEDOCUMENTSRESPONSE._serialized_start=2226
+  _DELETEDOCUMENTSRESPONSE._serialized_end=2278
+  _DELETEINDEXREQUEST._serialized_start=2280
+  _DELETEINDEXREQUEST._serialized_end=2320
+  _DELETEINDEXRESPONSE._serialized_start=2322
+  _DELETEINDEXRESPONSE._serialized_end=2371
+  _GETINDICESALIASESREQUEST._serialized_start=2373
+  _GETINDICESALIASESREQUEST._serialized_end=2399
+  _GETINDICESALIASESRESPONSE._serialized_start=2402
+  _GETINDICESALIASESRESPONSE._serialized_end=2569
+  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_start=2516
+  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_end=2569
+  _GETINDEXREQUEST._serialized_start=2571
+  _GETINDEXREQUEST._serialized_end=2608
+  _GETINDEXRESPONSE._serialized_start=2610
+  _GETINDEXRESPONSE._serialized_end=2674
+  _GETINDICESREQUEST._serialized_start=2676
+  _GETINDICESREQUEST._serialized_end=2695
+  _GETINDICESRESPONSE._serialized_start=2697
+  _GETINDICESRESPONSE._serialized_end=2738
+  _INDEXDOCUMENTSTREAMREQUEST._serialized_start=2740
+  _INDEXDOCUMENTSTREAMREQUEST._serialized_end=2807
+  _INDEXDOCUMENTSTREAMRESPONSE._serialized_start=2809
+  _INDEXDOCUMENTSTREAMRESPONSE._serialized_end=2903
+  _INDEXDOCUMENTREQUEST._serialized_start=2905
+  _INDEXDOCUMENTREQUEST._serialized_end=2965
+  _INDEXDOCUMENTRESPONSE._serialized_start=2967
+  _INDEXDOCUMENTRESPONSE._serialized_end=2990
+  _MERGESEGMENTSREQUEST._serialized_start=2992
+  _MERGESEGMENTSREQUEST._serialized_end=3055
+  _MERGESEGMENTSRESPONSE._serialized_start=3057
+  _MERGESEGMENTSRESPONSE._serialized_end=3120
+  _SETINDEXALIASREQUEST._serialized_start=3122
+  _SETINDEXALIASREQUEST._serialized_end=3185
+  _SETINDEXALIASRESPONSE._serialized_start=3187
+  _SETINDEXALIASRESPONSE._serialized_end=3258
+  _DOCUMENTSREQUEST._serialized_start=3260
+  _DOCUMENTSREQUEST._serialized_end=3314
+  _DOCUMENTSRESPONSE._serialized_start=3316
+  _DOCUMENTSRESPONSE._serialized_end=3353
+  _VACUUMINDEXREQUEST._serialized_start=3355
+  _VACUUMINDEXREQUEST._serialized_end=3422
+  _VACUUMINDEXRESPONSE._serialized_start=3424
+  _VACUUMINDEXRESPONSE._serialized_end=3472
+  _WARMUPINDEXREQUEST._serialized_start=3474
+  _WARMUPINDEXREQUEST._serialized_end=3531
+  _WARMUPINDEXRESPONSE._serialized_start=3533
+  _WARMUPINDEXRESPONSE._serialized_end=3576
+  _FILEENGINECONFIG._serialized_start=3578
+  _FILEENGINECONFIG._serialized_end=3610
+  _MEMORYENGINECONFIG._serialized_start=3612
+  _MEMORYENGINECONFIG._serialized_end=3648
+  _CACHECONFIG._serialized_start=3650
+  _CACHECONFIG._serialized_end=3683
+  _REMOTEENGINECONFIG._serialized_start=3686
+  _REMOTEENGINECONFIG._serialized_end=3968
+  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_start=3899
+  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_end=3953
+  _LOGMERGEPOLICY._serialized_start=3970
+  _LOGMERGEPOLICY._serialized_end=4005
+  _TEMPORALMERGEPOLICY._serialized_start=4007
+  _TEMPORALMERGEPOLICY._serialized_end=4059
+  _INDEXENGINECONFIG._serialized_start=4062
+  _INDEXENGINECONFIG._serialized_end=4478
+  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_start=4416
+  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_end=4468
+  _INDEXDESCRIPTION._serialized_start=4481
+  _INDEXDESCRIPTION._serialized_end=4717
+  _INDEXDOCUMENTOPERATION._serialized_start=4719
+  _INDEXDOCUMENTOPERATION._serialized_end=4761
+  _INDEXOPERATION._serialized_start=4763
+  _INDEXOPERATION._serialized_end=4855
+  _INDEXAPI._serialized_start=5068
+  _INDEXAPI._serialized_end=6583
 # @@protoc_insertion_point(module_scope)
```

### Comparing `summa_embed-0.16.0/summa_embed/proto/index_service_pb2.pyi` & `summa_embed-0.17.0/summa_embed/proto/index_service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -231,30 +231,26 @@
 class GetIndicesResponse(_message.Message):
     __slots__ = ["index_names"]
     INDEX_NAMES_FIELD_NUMBER: _ClassVar[int]
     index_names: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, index_names: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class IndexAttributes(_message.Message):
-    __slots__ = ["conflict_strategy", "created_at", "default_index_name", "default_snippets", "description", "multi_fields", "unique_fields"]
+    __slots__ = ["conflict_strategy", "created_at", "description", "multi_fields", "unique_fields"]
     CONFLICT_STRATEGY_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    DEFAULT_INDEX_NAME_FIELD_NUMBER: _ClassVar[int]
-    DEFAULT_SNIPPETS_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     MULTI_FIELDS_FIELD_NUMBER: _ClassVar[int]
     UNIQUE_FIELDS_FIELD_NUMBER: _ClassVar[int]
     conflict_strategy: ConflictStrategy
     created_at: int
-    default_index_name: str
-    default_snippets: _containers.RepeatedScalarFieldContainer[str]
     description: str
     multi_fields: _containers.RepeatedScalarFieldContainer[str]
     unique_fields: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, created_at: _Optional[int] = ..., unique_fields: _Optional[_Iterable[str]] = ..., multi_fields: _Optional[_Iterable[str]] = ..., default_index_name: _Optional[str] = ..., description: _Optional[str] = ..., default_snippets: _Optional[_Iterable[str]] = ..., conflict_strategy: _Optional[_Union[ConflictStrategy, str]] = ...) -> None: ...
+    def __init__(self, created_at: _Optional[int] = ..., unique_fields: _Optional[_Iterable[str]] = ..., multi_fields: _Optional[_Iterable[str]] = ..., description: _Optional[str] = ..., conflict_strategy: _Optional[_Union[ConflictStrategy, str]] = ...) -> None: ...
 
 class IndexDescription(_message.Message):
     __slots__ = ["compression", "index_aliases", "index_attributes", "index_engine", "index_name", "num_docs"]
     COMPRESSION_FIELD_NUMBER: _ClassVar[int]
     INDEX_ALIASES_FIELD_NUMBER: _ClassVar[int]
     INDEX_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     INDEX_ENGINE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `summa_embed-0.16.0/summa_embed/proto/query_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/query_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import utils_pb2 as utils__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bquery.proto\x12\x0bsumma.proto\x1a\x0butils.proto\"2\n\x0b\x46ieldMapper\x12\x13\n\x0bmapper_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"\x1d\n\x1bMatchQueryBooleanShouldMode\"2\n\x1bMatchQueryDisjuctionMaxMode\x12\x13\n\x0btie_breaker\x18\x01 \x01(\x02\"B\n\x14\x45xactMatchesPromoter\x12\x0c\n\x04slop\x18\x01 \x01(\r\x12\x12\n\x05\x62oost\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x08\n\x06_boost\")\n\x10InflectionConfig\x12\x15\n\rderive_plural\x18\x01 \x01(\x08\"\xa3\x07\n\x11QueryParserConfig\x12G\n\rfield_aliases\x18\x01 \x03(\x0b\x32\x30.summa.proto.QueryParserConfig.FieldAliasesEntry\x12\x45\n\x0c\x66ield_boosts\x18\x02 \x03(\x0b\x32/.summa.proto.QueryParserConfig.FieldBoostsEntry\x12I\n\x0e\x66ield_mappings\x18\x03 \x03(\x0b\x32\x31.summa.proto.QueryParserConfig.FieldMappingsEntry\x12\x12\n\nterm_limit\x18\x04 \x01(\r\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x05 \x03(\t\x12G\n\x13\x62oolean_should_mode\x18\x06 \x01(\x0b\x32(.summa.proto.MatchQueryBooleanShouldModeH\x00\x12G\n\x13\x64isjuction_max_mode\x18\x07 \x01(\x0b\x32(.summa.proto.MatchQueryDisjuctionMaxModeH\x00\x12\x41\n\x16\x65xact_matches_promoter\x18\x08 \x01(\x0b\x32!.summa.proto.ExactMatchesPromoter\x12=\n\x14missing_field_policy\x18\t \x01(\x0e\x32\x1f.summa.proto.MissingFieldPolicy\x12Q\n\x12inflection_configs\x18\n \x03(\x0b\x32\x35.summa.proto.QueryParserConfig.InflectionConfigsEntry\x1a\x33\n\x11\x46ieldAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x46ieldBoostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1aN\n\x12\x46ieldMappingsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.FieldMapper:\x02\x38\x01\x1aW\n\x16InflectionConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.summa.proto.InflectionConfig:\x02\x38\x01\x42\x0e\n\x0c\x64\x65\x66\x61ult_mode\"_\n\x0eSearchResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x37\n\x11\x63ollector_outputs\x18\x02 \x03(\x0b\x32\x1c.summa.proto.CollectorOutput\"\xad\x04\n\x05Query\x12,\n\x07\x62oolean\x18\x01 \x01(\x0b\x32\x19.summa.proto.BooleanQueryH\x00\x12(\n\x05match\x18\x02 \x01(\x0b\x32\x17.summa.proto.MatchQueryH\x00\x12(\n\x05regex\x18\x03 \x01(\x0b\x32\x17.summa.proto.RegexQueryH\x00\x12&\n\x04term\x18\x04 \x01(\x0b\x32\x16.summa.proto.TermQueryH\x00\x12*\n\x06phrase\x18\x05 \x01(\x0b\x32\x18.summa.proto.PhraseQueryH\x00\x12(\n\x05range\x18\x06 \x01(\x0b\x32\x17.summa.proto.RangeQueryH\x00\x12$\n\x03\x61ll\x18\x07 \x01(\x0b\x32\x15.summa.proto.AllQueryH\x00\x12\x38\n\x0emore_like_this\x18\x08 \x01(\x0b\x32\x1e.summa.proto.MoreLikeThisQueryH\x00\x12(\n\x05\x62oost\x18\t \x01(\x0b\x32\x17.summa.proto.BoostQueryH\x00\x12;\n\x0f\x64isjunction_max\x18\n \x01(\x0b\x32 .summa.proto.DisjunctionMaxQueryH\x00\x12(\n\x05\x65mpty\x18\x0b \x01(\x0b\x32\x17.summa.proto.EmptyQueryH\x00\x12*\n\x06\x65xists\x18\x0c \x01(\x0b\x32\x18.summa.proto.ExistsQueryH\x00\x42\x07\n\x05query\"\n\n\x08\x41llQuery\"\x0c\n\nEmptyQuery\">\n\nBoostQuery\x12!\n\x05query\x18\x01 \x01(\x0b\x32\x12.summa.proto.Query\x12\r\n\x05score\x18\x02 \x01(\t\"Q\n\x13\x44isjunctionMaxQuery\x12%\n\tdisjuncts\x18\x01 \x03(\x0b\x32\x12.summa.proto.Query\x12\x13\n\x0btie_breaker\x18\x02 \x01(\t\"\x91\x03\n\x11MoreLikeThisQuery\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12\x1e\n\x11min_doc_frequency\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x1e\n\x11max_doc_frequency\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1f\n\x12min_term_frequency\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x1c\n\x0fmax_query_terms\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12\x1c\n\x0fmin_word_length\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12\x1c\n\x0fmax_word_length\x18\x07 \x01(\x04H\x05\x88\x01\x01\x12\x12\n\x05\x62oost\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x12\n\nstop_words\x18\t \x03(\tB\x14\n\x12_min_doc_frequencyB\x14\n\x12_max_doc_frequencyB\x15\n\x13_min_term_frequencyB\x12\n\x10_max_query_termsB\x12\n\x10_min_word_lengthB\x12\n\x10_max_word_lengthB\x08\n\x06_boost\"9\n\x0bPhraseQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04slop\x18\x03 \x01(\r\">\n\nRangeQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.summa.proto.Range\"u\n\nMatchQuery\x12\r\n\x05value\x18\x01 \x01(\t\x12@\n\x13query_parser_config\x18\x02 \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigH\x00\x88\x01\x01\x42\x16\n\x14_query_parser_config\"W\n\x0f\x42ooleanSubquery\x12!\n\x05occur\x18\x01 \x01(\x0e\x32\x12.summa.proto.Occur\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"@\n\x0c\x42ooleanQuery\x12\x30\n\nsubqueries\x18\x01 \x03(\x0b\x32\x1c.summa.proto.BooleanSubquery\"*\n\nRegexQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\")\n\tTermQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x1c\n\x0b\x45xistsQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\x80\x01\n\x0b\x41ggregation\x12\x30\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x1e.summa.proto.BucketAggregationH\x00\x12\x30\n\x06metric\x18\x02 \x01(\x0b\x32\x1e.summa.proto.MetricAggregationH\x00\x42\r\n\x0b\x61ggregation\"\xd7\x02\n\x11\x42ucketAggregation\x12.\n\x05range\x18\x01 \x01(\x0b\x32\x1d.summa.proto.RangeAggregationH\x00\x12\x36\n\thistogram\x18\x02 \x01(\x0b\x32!.summa.proto.HistogramAggregationH\x00\x12.\n\x05terms\x18\x03 \x01(\x0b\x32\x1d.summa.proto.TermsAggregationH\x00\x12K\n\x0fsub_aggregation\x18\x04 \x03(\x0b\x32\x32.summa.proto.BucketAggregation.SubAggregationEntry\x1aO\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\x42\x0c\n\nbucket_agg\"U\n\x10RangeAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x32\n\x06ranges\x18\x02 \x03(\x0b\x32\".summa.proto.RangeAggregationRange\"e\n\x15RangeAggregationRange\x12\x11\n\x04\x66rom\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03key\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x07\n\x05_fromB\x05\n\x03_toB\x06\n\x04_key\"\x9d\x02\n\x14HistogramAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x02 \x01(\x01\x12\x13\n\x06offset\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x04 \x01(\x04H\x01\x88\x01\x01\x12\x36\n\x0bhard_bounds\x18\x05 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x02\x88\x01\x01\x12:\n\x0f\x65xtended_bounds\x18\x06 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x10\n\x0e_min_doc_countB\x0e\n\x0c_hard_boundsB\x12\n\x10_extended_bounds\"+\n\x0fHistogramBounds\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\"\xbd\x02\n\x10TermsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\x04size\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x17\n\nsplit_size\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x19\n\x0csegment_size\x18\x04 \x01(\rH\x02\x88\x01\x01\x12&\n\x19show_term_doc_count_error\x18\x05 \x01(\x08H\x03\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12,\n\x05order\x18\x07 \x01(\x0b\x32\x18.summa.proto.CustomOrderH\x05\x88\x01\x01\x42\x07\n\x05_sizeB\r\n\x0b_split_sizeB\x0f\n\r_segment_sizeB\x1c\n\x1a_show_term_doc_count_errorB\x10\n\x0e_min_doc_countB\x08\n\x06_order\"\xa3\x01\n\x0b\x43ustomOrder\x12!\n\x03key\x18\x01 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12#\n\x05\x63ount\x18\x02 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12\x19\n\x0fsub_aggregation\x18\x03 \x01(\tH\x00\x12!\n\x05order\x18\x04 \x01(\x0e\x32\x12.summa.proto.OrderB\x0e\n\x0corder_target\"\x8d\x01\n\x11MetricAggregation\x12\x32\n\x07\x61verage\x18\x01 \x01(\x0b\x32\x1f.summa.proto.AverageAggregationH\x00\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1d.summa.proto.StatsAggregationH\x00\x42\x14\n\x12metric_aggregation\"#\n\x12\x41verageAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"!\n\x10StatsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\xdd\x01\n\x0b\x42ucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12\x45\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32,.summa.proto.BucketEntry.SubAggregationEntry\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"*\n\x03Key\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03\x66\x36\x34\x18\x02 \x01(\x01H\x00\x42\x05\n\x03key\"U\n\x05Range\x12\x0c\n\x04left\x18\x01 \x01(\t\x12\r\n\x05right\x18\x02 \x01(\t\x12\x16\n\x0eincluding_left\x18\x03 \x01(\x08\x12\x17\n\x0fincluding_right\x18\x04 \x01(\x08\"\x9b\x02\n\x10RangeBucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12J\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32\x31.summa.proto.RangeBucketEntry.SubAggregationEntry\x12\x11\n\x04\x66rom\x18\x04 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x05 \x01(\x01H\x01\x88\x01\x01\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\x42\x07\n\x05_fromB\x05\n\x03_to\":\n\x05Score\x12\x13\n\tf64_score\x18\x01 \x01(\x01H\x00\x12\x13\n\tu64_score\x18\x02 \x01(\x04H\x00\x42\x07\n\x05score\"%\n\tHighlight\x12\x0c\n\x04\x66rom\x18\x01 \x01(\r\x12\n\n\x02to\x18\x02 \x01(\r\"U\n\x07Snippet\x12\x10\n\x08\x66ragment\x18\x01 \x01(\x0c\x12*\n\nhighlights\x18\x02 \x03(\x0b\x32\x16.summa.proto.Highlight\x12\x0c\n\x04html\x18\x03 \x01(\t\"\xf0\x01\n\x0eScoredDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x10\n\x08position\x18\x03 \x01(\r\x12;\n\x08snippets\x18\x04 \x03(\x0b\x32).summa.proto.ScoredDocument.SnippetsEntry\x12\x13\n\x0bindex_alias\x18\x05 \x01(\t\x1a\x45\n\rSnippetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.summa.proto.Snippet:\x02\x38\x01\";\n\x06Scorer\x12\x13\n\teval_expr\x18\x01 \x01(\tH\x00\x12\x12\n\x08order_by\x18\x02 \x01(\tH\x00\x42\x08\n\x06scorer\"\xa8\x02\n\tCollector\x12\x31\n\x08top_docs\x18\x01 \x01(\x0b\x32\x1d.summa.proto.TopDocsCollectorH\x00\x12\x45\n\x12reservoir_sampling\x18\x02 \x01(\x0b\x32\'.summa.proto.ReservoirSamplingCollectorH\x00\x12,\n\x05\x63ount\x18\x03 \x01(\x0b\x32\x1b.summa.proto.CountCollectorH\x00\x12,\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32\x1b.summa.proto.FacetCollectorH\x00\x12\x38\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32!.summa.proto.AggregationCollectorH\x00\x42\x0b\n\tcollector\"\x89\x02\n\x0f\x43ollectorOutput\x12:\n\tdocuments\x18\x01 \x01(\x0b\x32%.summa.proto.DocumentsCollectorOutputH\x00\x12\x32\n\x05\x63ount\x18\x03 \x01(\x0b\x32!.summa.proto.CountCollectorOutputH\x00\x12\x32\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32!.summa.proto.FacetCollectorOutputH\x00\x12>\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32\'.summa.proto.AggregationCollectorOutputH\x00\x42\x12\n\x10\x63ollector_output\"\x10\n\x0e\x43ountCollector\"%\n\x14\x43ountCollectorOutput\x12\r\n\x05\x63ount\x18\x01 \x01(\r\"/\n\x0e\x46\x61\x63\x65tCollector\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x0e\n\x06\x66\x61\x63\x65ts\x18\x02 \x03(\t\"\x94\x01\n\x14\x46\x61\x63\x65tCollectorOutput\x12H\n\x0c\x66\x61\x63\x65t_counts\x18\x01 \x03(\x0b\x32\x32.summa.proto.FacetCollectorOutput.FacetCountsEntry\x1a\x32\n\x10\x46\x61\x63\x65tCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\";\n\x1aReservoirSamplingCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"Z\n\x0eRandomDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x13\n\x0bindex_alias\x18\x03 \x01(\t\"R\n ReservoirSamplingCollectorOutput\x12.\n\tdocuments\x18\x01 \x03(\x0b\x32\x1b.summa.proto.RandomDocument\"\x8a\x02\n\x10TopDocsCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06offset\x18\x02 \x01(\r\x12(\n\x06scorer\x18\x03 \x01(\x0b\x32\x13.summa.proto.ScorerH\x00\x88\x01\x01\x12J\n\x0fsnippet_configs\x18\x04 \x03(\x0b\x32\x31.summa.proto.TopDocsCollector.SnippetConfigsEntry\x12\x0f\n\x07\x65xplain\x18\x05 \x01(\x08\x12\x0e\n\x06\x66ields\x18\x06 \x03(\t\x1a\x35\n\x13SnippetConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\x42\t\n\x07_scorer\"c\n\x18\x44ocumentsCollectorOutput\x12\x35\n\x10scored_documents\x18\x01 \x03(\x0b\x32\x1b.summa.proto.ScoredDocument\x12\x10\n\x08has_next\x18\x02 \x01(\x08\"\xb0\x01\n\x14\x41ggregationCollector\x12I\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x33.summa.proto.AggregationCollector.AggregationsEntry\x1aM\n\x11\x41ggregationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\"\xd5\x01\n\x1a\x41ggregationCollectorOutput\x12\\\n\x13\x61ggregation_results\x18\x01 \x03(\x0b\x32?.summa.proto.AggregationCollectorOutput.AggregationResultsEntry\x1aY\n\x17\x41ggregationResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"\x83\x01\n\x11\x41ggregationResult\x12+\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x19.summa.proto.BucketResultH\x00\x12+\n\x06metric\x18\x02 \x01(\x0b\x32\x19.summa.proto.MetricResultH\x00\x42\x14\n\x12\x61ggregation_result\"\xa8\x01\n\x0c\x42ucketResult\x12)\n\x05range\x18\x01 \x01(\x0b\x32\x18.summa.proto.RangeResultH\x00\x12\x31\n\thistogram\x18\x02 \x01(\x0b\x32\x1c.summa.proto.HistogramResultH\x00\x12)\n\x05terms\x18\x03 \x01(\x0b\x32\x18.summa.proto.TermsResultH\x00\x42\x0f\n\rbucket_result\"=\n\x0bRangeResult\x12.\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x1d.summa.proto.RangeBucketEntry\"<\n\x0fHistogramResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\"\x9f\x01\n\x0bTermsResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\x12\x1b\n\x13sum_other_doc_count\x18\x02 \x01(\x04\x12(\n\x1b\x64oc_count_error_upper_bound\x18\x03 \x01(\x04H\x00\x88\x01\x01\x42\x1e\n\x1c_doc_count_error_upper_bound\"\x84\x01\n\x0cMetricResult\x12\x38\n\rsingle_metric\x18\x01 \x01(\x0b\x32\x1f.summa.proto.SingleMetricResultH\x00\x12)\n\x05stats\x18\x02 \x01(\x0b\x32\x18.summa.proto.StatsResultH\x00\x42\x0f\n\rmetric_result\"2\n\x12SingleMetricResult\x12\x12\n\x05value\x18\x01 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value\"w\n\x0bStatsResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\x12\x0b\n\x03sum\x18\x02 \x01(\x01\x12\x10\n\x03min\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x04 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03\x61vg\x18\x05 \x01(\x01H\x02\x88\x01\x01\x42\x06\n\x04_minB\x06\n\x04_maxB\x06\n\x04_avg*<\n\x12MissingFieldPolicy\x12\x10\n\x0c\x41sUsualTerms\x10\x00\x12\n\n\x06Remove\x10\x01\x12\x08\n\x04\x46\x61il\x10\x02*+\n\x05Occur\x12\n\n\x06should\x10\x00\x12\x08\n\x04must\x10\x01\x12\x0c\n\x08must_not\x10\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bquery.proto\x12\x0bsumma.proto\x1a\x0butils.proto\"\'\n\x15TermFieldMapperConfig\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"\x1d\n\x1bMatchQueryBooleanShouldMode\"2\n\x1bMatchQueryDisjuctionMaxMode\x12\x13\n\x0btie_breaker\x18\x01 \x01(\x02\"R\n\x14\x45xactMatchesPromoter\x12\x0c\n\x04slop\x18\x01 \x01(\r\x12\x12\n\x05\x62oost\x18\x02 \x01(\x02H\x00\x88\x01\x01\x12\x0e\n\x06\x66ields\x18\x03 \x03(\tB\x08\n\x06_boost\"B\n\x12NerMatchesPromoter\x12\x12\n\x05\x62oost\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x0e\n\x06\x66ields\x18\x02 \x03(\tB\x08\n\x06_boost\"X\n\x10MorphologyConfig\x12&\n\x19\x64\x65rive_tenses_coefficient\x18\x01 \x01(\x02H\x00\x88\x01\x01\x42\x1c\n\x1a_derive_tenses_coefficient\"\xb9\x08\n\x11QueryParserConfig\x12G\n\rfield_aliases\x18\x01 \x03(\x0b\x32\x30.summa.proto.QueryParserConfig.FieldAliasesEntry\x12\x45\n\x0c\x66ield_boosts\x18\x02 \x03(\x0b\x32/.summa.proto.QueryParserConfig.FieldBoostsEntry\x12]\n\x19term_field_mapper_configs\x18\x03 \x03(\x0b\x32:.summa.proto.QueryParserConfig.TermFieldMapperConfigsEntry\x12\x12\n\nterm_limit\x18\x04 \x01(\r\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x05 \x03(\t\x12G\n\x13\x62oolean_should_mode\x18\x06 \x01(\x0b\x32(.summa.proto.MatchQueryBooleanShouldModeH\x00\x12G\n\x13\x64isjuction_max_mode\x18\x07 \x01(\x0b\x32(.summa.proto.MatchQueryDisjuctionMaxModeH\x00\x12\x41\n\x16\x65xact_matches_promoter\x18\x08 \x01(\x0b\x32!.summa.proto.ExactMatchesPromoter\x12=\n\x14missing_field_policy\x18\t \x01(\x0e\x32\x1f.summa.proto.MissingFieldPolicy\x12Q\n\x12morphology_configs\x18\n \x03(\x0b\x32\x35.summa.proto.QueryParserConfig.MorphologyConfigsEntry\x12\x1b\n\x0equery_language\x18\x0b \x01(\tH\x01\x88\x01\x01\x12=\n\x14ner_matches_promoter\x18\x0c \x01(\x0b\x32\x1f.summa.proto.NerMatchesPromoter\x1a\x33\n\x11\x46ieldAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x46ieldBoostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1a\x61\n\x1bTermFieldMapperConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".summa.proto.TermFieldMapperConfig:\x02\x38\x01\x1aW\n\x16MorphologyConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.summa.proto.MorphologyConfig:\x02\x38\x01\x42\x0e\n\x0c\x64\x65\x66\x61ult_modeB\x11\n\x0f_query_language\"_\n\x0eSearchResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x37\n\x11\x63ollector_outputs\x18\x02 \x03(\x0b\x32\x1c.summa.proto.CollectorOutput\"\xad\x04\n\x05Query\x12,\n\x07\x62oolean\x18\x01 \x01(\x0b\x32\x19.summa.proto.BooleanQueryH\x00\x12(\n\x05match\x18\x02 \x01(\x0b\x32\x17.summa.proto.MatchQueryH\x00\x12(\n\x05regex\x18\x03 \x01(\x0b\x32\x17.summa.proto.RegexQueryH\x00\x12&\n\x04term\x18\x04 \x01(\x0b\x32\x16.summa.proto.TermQueryH\x00\x12*\n\x06phrase\x18\x05 \x01(\x0b\x32\x18.summa.proto.PhraseQueryH\x00\x12(\n\x05range\x18\x06 \x01(\x0b\x32\x17.summa.proto.RangeQueryH\x00\x12$\n\x03\x61ll\x18\x07 \x01(\x0b\x32\x15.summa.proto.AllQueryH\x00\x12\x38\n\x0emore_like_this\x18\x08 \x01(\x0b\x32\x1e.summa.proto.MoreLikeThisQueryH\x00\x12(\n\x05\x62oost\x18\t \x01(\x0b\x32\x17.summa.proto.BoostQueryH\x00\x12;\n\x0f\x64isjunction_max\x18\n \x01(\x0b\x32 .summa.proto.DisjunctionMaxQueryH\x00\x12(\n\x05\x65mpty\x18\x0b \x01(\x0b\x32\x17.summa.proto.EmptyQueryH\x00\x12*\n\x06\x65xists\x18\x0c \x01(\x0b\x32\x18.summa.proto.ExistsQueryH\x00\x42\x07\n\x05query\"\n\n\x08\x41llQuery\"\x0c\n\nEmptyQuery\">\n\nBoostQuery\x12!\n\x05query\x18\x01 \x01(\x0b\x32\x12.summa.proto.Query\x12\r\n\x05score\x18\x02 \x01(\t\"Q\n\x13\x44isjunctionMaxQuery\x12%\n\tdisjuncts\x18\x01 \x03(\x0b\x32\x12.summa.proto.Query\x12\x13\n\x0btie_breaker\x18\x02 \x01(\t\"\x91\x03\n\x11MoreLikeThisQuery\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12\x1e\n\x11min_doc_frequency\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x1e\n\x11max_doc_frequency\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1f\n\x12min_term_frequency\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x1c\n\x0fmax_query_terms\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12\x1c\n\x0fmin_word_length\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12\x1c\n\x0fmax_word_length\x18\x07 \x01(\x04H\x05\x88\x01\x01\x12\x12\n\x05\x62oost\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x12\n\nstop_words\x18\t \x03(\tB\x14\n\x12_min_doc_frequencyB\x14\n\x12_max_doc_frequencyB\x15\n\x13_min_term_frequencyB\x12\n\x10_max_query_termsB\x12\n\x10_min_word_lengthB\x12\n\x10_max_word_lengthB\x08\n\x06_boost\"9\n\x0bPhraseQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04slop\x18\x03 \x01(\r\">\n\nRangeQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.summa.proto.Range\"u\n\nMatchQuery\x12\r\n\x05value\x18\x01 \x01(\t\x12@\n\x13query_parser_config\x18\x02 \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigH\x00\x88\x01\x01\x42\x16\n\x14_query_parser_config\"W\n\x0f\x42ooleanSubquery\x12!\n\x05occur\x18\x01 \x01(\x0e\x32\x12.summa.proto.Occur\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"@\n\x0c\x42ooleanQuery\x12\x30\n\nsubqueries\x18\x01 \x03(\x0b\x32\x1c.summa.proto.BooleanSubquery\"*\n\nRegexQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\")\n\tTermQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x1c\n\x0b\x45xistsQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\x80\x01\n\x0b\x41ggregation\x12\x30\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x1e.summa.proto.BucketAggregationH\x00\x12\x30\n\x06metric\x18\x02 \x01(\x0b\x32\x1e.summa.proto.MetricAggregationH\x00\x42\r\n\x0b\x61ggregation\"\xd7\x02\n\x11\x42ucketAggregation\x12.\n\x05range\x18\x01 \x01(\x0b\x32\x1d.summa.proto.RangeAggregationH\x00\x12\x36\n\thistogram\x18\x02 \x01(\x0b\x32!.summa.proto.HistogramAggregationH\x00\x12.\n\x05terms\x18\x03 \x01(\x0b\x32\x1d.summa.proto.TermsAggregationH\x00\x12K\n\x0fsub_aggregation\x18\x04 \x03(\x0b\x32\x32.summa.proto.BucketAggregation.SubAggregationEntry\x1aO\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\x42\x0c\n\nbucket_agg\"U\n\x10RangeAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x32\n\x06ranges\x18\x02 \x03(\x0b\x32\".summa.proto.RangeAggregationRange\"e\n\x15RangeAggregationRange\x12\x11\n\x04\x66rom\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03key\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x07\n\x05_fromB\x05\n\x03_toB\x06\n\x04_key\"\x9d\x02\n\x14HistogramAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x02 \x01(\x01\x12\x13\n\x06offset\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x04 \x01(\x04H\x01\x88\x01\x01\x12\x36\n\x0bhard_bounds\x18\x05 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x02\x88\x01\x01\x12:\n\x0f\x65xtended_bounds\x18\x06 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x10\n\x0e_min_doc_countB\x0e\n\x0c_hard_boundsB\x12\n\x10_extended_bounds\"+\n\x0fHistogramBounds\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\"\xbd\x02\n\x10TermsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\x04size\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x17\n\nsplit_size\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x19\n\x0csegment_size\x18\x04 \x01(\rH\x02\x88\x01\x01\x12&\n\x19show_term_doc_count_error\x18\x05 \x01(\x08H\x03\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12,\n\x05order\x18\x07 \x01(\x0b\x32\x18.summa.proto.CustomOrderH\x05\x88\x01\x01\x42\x07\n\x05_sizeB\r\n\x0b_split_sizeB\x0f\n\r_segment_sizeB\x1c\n\x1a_show_term_doc_count_errorB\x10\n\x0e_min_doc_countB\x08\n\x06_order\"\xa3\x01\n\x0b\x43ustomOrder\x12!\n\x03key\x18\x01 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12#\n\x05\x63ount\x18\x02 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12\x19\n\x0fsub_aggregation\x18\x03 \x01(\tH\x00\x12!\n\x05order\x18\x04 \x01(\x0e\x32\x12.summa.proto.OrderB\x0e\n\x0corder_target\"\x8d\x01\n\x11MetricAggregation\x12\x32\n\x07\x61verage\x18\x01 \x01(\x0b\x32\x1f.summa.proto.AverageAggregationH\x00\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1d.summa.proto.StatsAggregationH\x00\x42\x14\n\x12metric_aggregation\"#\n\x12\x41verageAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"!\n\x10StatsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\xdd\x01\n\x0b\x42ucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12\x45\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32,.summa.proto.BucketEntry.SubAggregationEntry\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"*\n\x03Key\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03\x66\x36\x34\x18\x02 \x01(\x01H\x00\x42\x05\n\x03key\"U\n\x05Range\x12\x0c\n\x04left\x18\x01 \x01(\t\x12\r\n\x05right\x18\x02 \x01(\t\x12\x16\n\x0eincluding_left\x18\x03 \x01(\x08\x12\x17\n\x0fincluding_right\x18\x04 \x01(\x08\"\x9b\x02\n\x10RangeBucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12J\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32\x31.summa.proto.RangeBucketEntry.SubAggregationEntry\x12\x11\n\x04\x66rom\x18\x04 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x05 \x01(\x01H\x01\x88\x01\x01\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\x42\x07\n\x05_fromB\x05\n\x03_to\":\n\x05Score\x12\x13\n\tf64_score\x18\x01 \x01(\x01H\x00\x12\x13\n\tu64_score\x18\x02 \x01(\x04H\x00\x42\x07\n\x05score\"%\n\tHighlight\x12\x0c\n\x04\x66rom\x18\x01 \x01(\r\x12\n\n\x02to\x18\x02 \x01(\r\"U\n\x07Snippet\x12\x10\n\x08\x66ragment\x18\x01 \x01(\x0c\x12*\n\nhighlights\x18\x02 \x03(\x0b\x32\x16.summa.proto.Highlight\x12\x0c\n\x04html\x18\x03 \x01(\t\"\xf0\x01\n\x0eScoredDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x10\n\x08position\x18\x03 \x01(\r\x12;\n\x08snippets\x18\x04 \x03(\x0b\x32).summa.proto.ScoredDocument.SnippetsEntry\x12\x13\n\x0bindex_alias\x18\x05 \x01(\t\x1a\x45\n\rSnippetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.summa.proto.Snippet:\x02\x38\x01\";\n\x06Scorer\x12\x13\n\teval_expr\x18\x01 \x01(\tH\x00\x12\x12\n\x08order_by\x18\x02 \x01(\tH\x00\x42\x08\n\x06scorer\"\xa8\x02\n\tCollector\x12\x31\n\x08top_docs\x18\x01 \x01(\x0b\x32\x1d.summa.proto.TopDocsCollectorH\x00\x12\x45\n\x12reservoir_sampling\x18\x02 \x01(\x0b\x32\'.summa.proto.ReservoirSamplingCollectorH\x00\x12,\n\x05\x63ount\x18\x03 \x01(\x0b\x32\x1b.summa.proto.CountCollectorH\x00\x12,\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32\x1b.summa.proto.FacetCollectorH\x00\x12\x38\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32!.summa.proto.AggregationCollectorH\x00\x42\x0b\n\tcollector\"\x89\x02\n\x0f\x43ollectorOutput\x12:\n\tdocuments\x18\x01 \x01(\x0b\x32%.summa.proto.DocumentsCollectorOutputH\x00\x12\x32\n\x05\x63ount\x18\x03 \x01(\x0b\x32!.summa.proto.CountCollectorOutputH\x00\x12\x32\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32!.summa.proto.FacetCollectorOutputH\x00\x12>\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32\'.summa.proto.AggregationCollectorOutputH\x00\x42\x12\n\x10\x63ollector_output\"\x10\n\x0e\x43ountCollector\"%\n\x14\x43ountCollectorOutput\x12\r\n\x05\x63ount\x18\x01 \x01(\r\"/\n\x0e\x46\x61\x63\x65tCollector\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x0e\n\x06\x66\x61\x63\x65ts\x18\x02 \x03(\t\"\x94\x01\n\x14\x46\x61\x63\x65tCollectorOutput\x12H\n\x0c\x66\x61\x63\x65t_counts\x18\x01 \x03(\x0b\x32\x32.summa.proto.FacetCollectorOutput.FacetCountsEntry\x1a\x32\n\x10\x46\x61\x63\x65tCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\";\n\x1aReservoirSamplingCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"Z\n\x0eRandomDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x13\n\x0bindex_alias\x18\x03 \x01(\t\"R\n ReservoirSamplingCollectorOutput\x12.\n\tdocuments\x18\x01 \x03(\x0b\x32\x1b.summa.proto.RandomDocument\"\x8a\x02\n\x10TopDocsCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06offset\x18\x02 \x01(\r\x12(\n\x06scorer\x18\x03 \x01(\x0b\x32\x13.summa.proto.ScorerH\x00\x88\x01\x01\x12J\n\x0fsnippet_configs\x18\x04 \x03(\x0b\x32\x31.summa.proto.TopDocsCollector.SnippetConfigsEntry\x12\x0f\n\x07\x65xplain\x18\x05 \x01(\x08\x12\x0e\n\x06\x66ields\x18\x06 \x03(\t\x1a\x35\n\x13SnippetConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\x42\t\n\x07_scorer\"c\n\x18\x44ocumentsCollectorOutput\x12\x35\n\x10scored_documents\x18\x01 \x03(\x0b\x32\x1b.summa.proto.ScoredDocument\x12\x10\n\x08has_next\x18\x02 \x01(\x08\"\xb0\x01\n\x14\x41ggregationCollector\x12I\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x33.summa.proto.AggregationCollector.AggregationsEntry\x1aM\n\x11\x41ggregationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\"\xd5\x01\n\x1a\x41ggregationCollectorOutput\x12\\\n\x13\x61ggregation_results\x18\x01 \x03(\x0b\x32?.summa.proto.AggregationCollectorOutput.AggregationResultsEntry\x1aY\n\x17\x41ggregationResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"\x83\x01\n\x11\x41ggregationResult\x12+\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x19.summa.proto.BucketResultH\x00\x12+\n\x06metric\x18\x02 \x01(\x0b\x32\x19.summa.proto.MetricResultH\x00\x42\x14\n\x12\x61ggregation_result\"\xa8\x01\n\x0c\x42ucketResult\x12)\n\x05range\x18\x01 \x01(\x0b\x32\x18.summa.proto.RangeResultH\x00\x12\x31\n\thistogram\x18\x02 \x01(\x0b\x32\x1c.summa.proto.HistogramResultH\x00\x12)\n\x05terms\x18\x03 \x01(\x0b\x32\x18.summa.proto.TermsResultH\x00\x42\x0f\n\rbucket_result\"=\n\x0bRangeResult\x12.\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x1d.summa.proto.RangeBucketEntry\"<\n\x0fHistogramResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\"\x9f\x01\n\x0bTermsResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\x12\x1b\n\x13sum_other_doc_count\x18\x02 \x01(\x04\x12(\n\x1b\x64oc_count_error_upper_bound\x18\x03 \x01(\x04H\x00\x88\x01\x01\x42\x1e\n\x1c_doc_count_error_upper_bound\"\x84\x01\n\x0cMetricResult\x12\x38\n\rsingle_metric\x18\x01 \x01(\x0b\x32\x1f.summa.proto.SingleMetricResultH\x00\x12)\n\x05stats\x18\x02 \x01(\x0b\x32\x18.summa.proto.StatsResultH\x00\x42\x0f\n\rmetric_result\"2\n\x12SingleMetricResult\x12\x12\n\x05value\x18\x01 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value\"w\n\x0bStatsResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\x12\x0b\n\x03sum\x18\x02 \x01(\x01\x12\x10\n\x03min\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x04 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03\x61vg\x18\x05 \x01(\x01H\x02\x88\x01\x01\x42\x06\n\x04_minB\x06\n\x04_maxB\x06\n\x04_avg*<\n\x12MissingFieldPolicy\x12\x10\n\x0c\x41sUsualTerms\x10\x00\x12\n\n\x06Remove\x10\x01\x12\x08\n\x04\x46\x61il\x10\x02*+\n\x05Occur\x12\n\n\x06should\x10\x00\x12\x08\n\x04must\x10\x01\x12\x0c\n\x08must_not\x10\x02\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _QUERYPARSERCONFIG_FIELDALIASESENTRY._options = None
   _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_options = b'8\001'
   _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._options = None
   _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_options = b'8\001'
-  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._options = None
-  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._serialized_options = b'8\001'
-  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._options = None
-  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._serialized_options = b'8\001'
+  _QUERYPARSERCONFIG_TERMFIELDMAPPERCONFIGSENTRY._options = None
+  _QUERYPARSERCONFIG_TERMFIELDMAPPERCONFIGSENTRY._serialized_options = b'8\001'
+  _QUERYPARSERCONFIG_MORPHOLOGYCONFIGSENTRY._options = None
+  _QUERYPARSERCONFIG_MORPHOLOGYCONFIGSENTRY._serialized_options = b'8\001'
   _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._options = None
   _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_options = b'8\001'
   _BUCKETENTRY_SUBAGGREGATIONENTRY._options = None
   _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_options = b'8\001'
   _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._options = None
   _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_options = b'8\001'
   _SCOREDDOCUMENT_SNIPPETSENTRY._options = None
@@ -41,160 +41,162 @@
   _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_options = b'8\001'
   _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._options = None
   _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_options = b'8\001'
   _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._options = None
   _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_options = b'8\001'
   _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._options = None
   _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_options = b'8\001'
-  _MISSINGFIELDPOLICY._serialized_start=8528
-  _MISSINGFIELDPOLICY._serialized_end=8588
-  _OCCUR._serialized_start=8590
-  _OCCUR._serialized_end=8633
-  _FIELDMAPPER._serialized_start=41
-  _FIELDMAPPER._serialized_end=91
-  _MATCHQUERYBOOLEANSHOULDMODE._serialized_start=93
-  _MATCHQUERYBOOLEANSHOULDMODE._serialized_end=122
-  _MATCHQUERYDISJUCTIONMAXMODE._serialized_start=124
-  _MATCHQUERYDISJUCTIONMAXMODE._serialized_end=174
-  _EXACTMATCHESPROMOTER._serialized_start=176
-  _EXACTMATCHESPROMOTER._serialized_end=242
-  _INFLECTIONCONFIG._serialized_start=244
-  _INFLECTIONCONFIG._serialized_end=285
-  _QUERYPARSERCONFIG._serialized_start=288
-  _QUERYPARSERCONFIG._serialized_end=1219
-  _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_start=931
-  _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_end=982
-  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_start=984
-  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_end=1034
-  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._serialized_start=1036
-  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._serialized_end=1114
-  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._serialized_start=1116
-  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._serialized_end=1203
-  _SEARCHRESPONSE._serialized_start=1221
-  _SEARCHRESPONSE._serialized_end=1316
-  _QUERY._serialized_start=1319
-  _QUERY._serialized_end=1876
-  _ALLQUERY._serialized_start=1878
-  _ALLQUERY._serialized_end=1888
-  _EMPTYQUERY._serialized_start=1890
-  _EMPTYQUERY._serialized_end=1902
-  _BOOSTQUERY._serialized_start=1904
-  _BOOSTQUERY._serialized_end=1966
-  _DISJUNCTIONMAXQUERY._serialized_start=1968
-  _DISJUNCTIONMAXQUERY._serialized_end=2049
-  _MORELIKETHISQUERY._serialized_start=2052
-  _MORELIKETHISQUERY._serialized_end=2453
-  _PHRASEQUERY._serialized_start=2455
-  _PHRASEQUERY._serialized_end=2512
-  _RANGEQUERY._serialized_start=2514
-  _RANGEQUERY._serialized_end=2576
-  _MATCHQUERY._serialized_start=2578
-  _MATCHQUERY._serialized_end=2695
-  _BOOLEANSUBQUERY._serialized_start=2697
-  _BOOLEANSUBQUERY._serialized_end=2784
-  _BOOLEANQUERY._serialized_start=2786
-  _BOOLEANQUERY._serialized_end=2850
-  _REGEXQUERY._serialized_start=2852
-  _REGEXQUERY._serialized_end=2894
-  _TERMQUERY._serialized_start=2896
-  _TERMQUERY._serialized_end=2937
-  _EXISTSQUERY._serialized_start=2939
-  _EXISTSQUERY._serialized_end=2967
-  _AGGREGATION._serialized_start=2970
-  _AGGREGATION._serialized_end=3098
-  _BUCKETAGGREGATION._serialized_start=3101
-  _BUCKETAGGREGATION._serialized_end=3444
-  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_start=3351
-  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_end=3430
-  _RANGEAGGREGATION._serialized_start=3446
-  _RANGEAGGREGATION._serialized_end=3531
-  _RANGEAGGREGATIONRANGE._serialized_start=3533
-  _RANGEAGGREGATIONRANGE._serialized_end=3634
-  _HISTOGRAMAGGREGATION._serialized_start=3637
-  _HISTOGRAMAGGREGATION._serialized_end=3922
-  _HISTOGRAMBOUNDS._serialized_start=3924
-  _HISTOGRAMBOUNDS._serialized_end=3967
-  _TERMSAGGREGATION._serialized_start=3970
-  _TERMSAGGREGATION._serialized_end=4287
-  _CUSTOMORDER._serialized_start=4290
-  _CUSTOMORDER._serialized_end=4453
-  _METRICAGGREGATION._serialized_start=4456
-  _METRICAGGREGATION._serialized_end=4597
-  _AVERAGEAGGREGATION._serialized_start=4599
-  _AVERAGEAGGREGATION._serialized_end=4634
-  _STATSAGGREGATION._serialized_start=4636
-  _STATSAGGREGATION._serialized_end=4669
-  _BUCKETENTRY._serialized_start=4672
-  _BUCKETENTRY._serialized_end=4893
-  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=4808
-  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=4893
-  _KEY._serialized_start=4895
-  _KEY._serialized_end=4937
-  _RANGE._serialized_start=4939
-  _RANGE._serialized_end=5024
-  _RANGEBUCKETENTRY._serialized_start=5027
-  _RANGEBUCKETENTRY._serialized_end=5310
-  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=4808
-  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=4893
-  _SCORE._serialized_start=5312
-  _SCORE._serialized_end=5370
-  _HIGHLIGHT._serialized_start=5372
-  _HIGHLIGHT._serialized_end=5409
-  _SNIPPET._serialized_start=5411
-  _SNIPPET._serialized_end=5496
-  _SCOREDDOCUMENT._serialized_start=5499
-  _SCOREDDOCUMENT._serialized_end=5739
-  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_start=5670
-  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_end=5739
-  _SCORER._serialized_start=5741
-  _SCORER._serialized_end=5800
-  _COLLECTOR._serialized_start=5803
-  _COLLECTOR._serialized_end=6099
-  _COLLECTOROUTPUT._serialized_start=6102
-  _COLLECTOROUTPUT._serialized_end=6367
-  _COUNTCOLLECTOR._serialized_start=6369
-  _COUNTCOLLECTOR._serialized_end=6385
-  _COUNTCOLLECTOROUTPUT._serialized_start=6387
-  _COUNTCOLLECTOROUTPUT._serialized_end=6424
-  _FACETCOLLECTOR._serialized_start=6426
-  _FACETCOLLECTOR._serialized_end=6473
-  _FACETCOLLECTOROUTPUT._serialized_start=6476
-  _FACETCOLLECTOROUTPUT._serialized_end=6624
-  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_start=6574
-  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_end=6624
-  _RESERVOIRSAMPLINGCOLLECTOR._serialized_start=6626
-  _RESERVOIRSAMPLINGCOLLECTOR._serialized_end=6685
-  _RANDOMDOCUMENT._serialized_start=6687
-  _RANDOMDOCUMENT._serialized_end=6777
-  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_start=6779
-  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_end=6861
-  _TOPDOCSCOLLECTOR._serialized_start=6864
-  _TOPDOCSCOLLECTOR._serialized_end=7130
-  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_start=7066
-  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_end=7119
-  _DOCUMENTSCOLLECTOROUTPUT._serialized_start=7132
-  _DOCUMENTSCOLLECTOROUTPUT._serialized_end=7231
-  _AGGREGATIONCOLLECTOR._serialized_start=7234
-  _AGGREGATIONCOLLECTOR._serialized_end=7410
-  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_start=7333
-  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_end=7410
-  _AGGREGATIONCOLLECTOROUTPUT._serialized_start=7413
-  _AGGREGATIONCOLLECTOROUTPUT._serialized_end=7626
-  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_start=7537
-  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_end=7626
-  _AGGREGATIONRESULT._serialized_start=7629
-  _AGGREGATIONRESULT._serialized_end=7760
-  _BUCKETRESULT._serialized_start=7763
-  _BUCKETRESULT._serialized_end=7931
-  _RANGERESULT._serialized_start=7933
-  _RANGERESULT._serialized_end=7994
-  _HISTOGRAMRESULT._serialized_start=7996
-  _HISTOGRAMRESULT._serialized_end=8056
-  _TERMSRESULT._serialized_start=8059
-  _TERMSRESULT._serialized_end=8218
-  _METRICRESULT._serialized_start=8221
-  _METRICRESULT._serialized_end=8353
-  _SINGLEMETRICRESULT._serialized_start=8355
-  _SINGLEMETRICRESULT._serialized_end=8405
-  _STATSRESULT._serialized_start=8407
-  _STATSRESULT._serialized_end=8526
+  _MISSINGFIELDPOLICY._serialized_start=8798
+  _MISSINGFIELDPOLICY._serialized_end=8858
+  _OCCUR._serialized_start=8860
+  _OCCUR._serialized_end=8903
+  _TERMFIELDMAPPERCONFIG._serialized_start=41
+  _TERMFIELDMAPPERCONFIG._serialized_end=80
+  _MATCHQUERYBOOLEANSHOULDMODE._serialized_start=82
+  _MATCHQUERYBOOLEANSHOULDMODE._serialized_end=111
+  _MATCHQUERYDISJUCTIONMAXMODE._serialized_start=113
+  _MATCHQUERYDISJUCTIONMAXMODE._serialized_end=163
+  _EXACTMATCHESPROMOTER._serialized_start=165
+  _EXACTMATCHESPROMOTER._serialized_end=247
+  _NERMATCHESPROMOTER._serialized_start=249
+  _NERMATCHESPROMOTER._serialized_end=315
+  _MORPHOLOGYCONFIG._serialized_start=317
+  _MORPHOLOGYCONFIG._serialized_end=405
+  _QUERYPARSERCONFIG._serialized_start=408
+  _QUERYPARSERCONFIG._serialized_end=1489
+  _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_start=1163
+  _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_end=1214
+  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_start=1216
+  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_end=1266
+  _QUERYPARSERCONFIG_TERMFIELDMAPPERCONFIGSENTRY._serialized_start=1268
+  _QUERYPARSERCONFIG_TERMFIELDMAPPERCONFIGSENTRY._serialized_end=1365
+  _QUERYPARSERCONFIG_MORPHOLOGYCONFIGSENTRY._serialized_start=1367
+  _QUERYPARSERCONFIG_MORPHOLOGYCONFIGSENTRY._serialized_end=1454
+  _SEARCHRESPONSE._serialized_start=1491
+  _SEARCHRESPONSE._serialized_end=1586
+  _QUERY._serialized_start=1589
+  _QUERY._serialized_end=2146
+  _ALLQUERY._serialized_start=2148
+  _ALLQUERY._serialized_end=2158
+  _EMPTYQUERY._serialized_start=2160
+  _EMPTYQUERY._serialized_end=2172
+  _BOOSTQUERY._serialized_start=2174
+  _BOOSTQUERY._serialized_end=2236
+  _DISJUNCTIONMAXQUERY._serialized_start=2238
+  _DISJUNCTIONMAXQUERY._serialized_end=2319
+  _MORELIKETHISQUERY._serialized_start=2322
+  _MORELIKETHISQUERY._serialized_end=2723
+  _PHRASEQUERY._serialized_start=2725
+  _PHRASEQUERY._serialized_end=2782
+  _RANGEQUERY._serialized_start=2784
+  _RANGEQUERY._serialized_end=2846
+  _MATCHQUERY._serialized_start=2848
+  _MATCHQUERY._serialized_end=2965
+  _BOOLEANSUBQUERY._serialized_start=2967
+  _BOOLEANSUBQUERY._serialized_end=3054
+  _BOOLEANQUERY._serialized_start=3056
+  _BOOLEANQUERY._serialized_end=3120
+  _REGEXQUERY._serialized_start=3122
+  _REGEXQUERY._serialized_end=3164
+  _TERMQUERY._serialized_start=3166
+  _TERMQUERY._serialized_end=3207
+  _EXISTSQUERY._serialized_start=3209
+  _EXISTSQUERY._serialized_end=3237
+  _AGGREGATION._serialized_start=3240
+  _AGGREGATION._serialized_end=3368
+  _BUCKETAGGREGATION._serialized_start=3371
+  _BUCKETAGGREGATION._serialized_end=3714
+  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_start=3621
+  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_end=3700
+  _RANGEAGGREGATION._serialized_start=3716
+  _RANGEAGGREGATION._serialized_end=3801
+  _RANGEAGGREGATIONRANGE._serialized_start=3803
+  _RANGEAGGREGATIONRANGE._serialized_end=3904
+  _HISTOGRAMAGGREGATION._serialized_start=3907
+  _HISTOGRAMAGGREGATION._serialized_end=4192
+  _HISTOGRAMBOUNDS._serialized_start=4194
+  _HISTOGRAMBOUNDS._serialized_end=4237
+  _TERMSAGGREGATION._serialized_start=4240
+  _TERMSAGGREGATION._serialized_end=4557
+  _CUSTOMORDER._serialized_start=4560
+  _CUSTOMORDER._serialized_end=4723
+  _METRICAGGREGATION._serialized_start=4726
+  _METRICAGGREGATION._serialized_end=4867
+  _AVERAGEAGGREGATION._serialized_start=4869
+  _AVERAGEAGGREGATION._serialized_end=4904
+  _STATSAGGREGATION._serialized_start=4906
+  _STATSAGGREGATION._serialized_end=4939
+  _BUCKETENTRY._serialized_start=4942
+  _BUCKETENTRY._serialized_end=5163
+  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=5078
+  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=5163
+  _KEY._serialized_start=5165
+  _KEY._serialized_end=5207
+  _RANGE._serialized_start=5209
+  _RANGE._serialized_end=5294
+  _RANGEBUCKETENTRY._serialized_start=5297
+  _RANGEBUCKETENTRY._serialized_end=5580
+  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=5078
+  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=5163
+  _SCORE._serialized_start=5582
+  _SCORE._serialized_end=5640
+  _HIGHLIGHT._serialized_start=5642
+  _HIGHLIGHT._serialized_end=5679
+  _SNIPPET._serialized_start=5681
+  _SNIPPET._serialized_end=5766
+  _SCOREDDOCUMENT._serialized_start=5769
+  _SCOREDDOCUMENT._serialized_end=6009
+  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_start=5940
+  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_end=6009
+  _SCORER._serialized_start=6011
+  _SCORER._serialized_end=6070
+  _COLLECTOR._serialized_start=6073
+  _COLLECTOR._serialized_end=6369
+  _COLLECTOROUTPUT._serialized_start=6372
+  _COLLECTOROUTPUT._serialized_end=6637
+  _COUNTCOLLECTOR._serialized_start=6639
+  _COUNTCOLLECTOR._serialized_end=6655
+  _COUNTCOLLECTOROUTPUT._serialized_start=6657
+  _COUNTCOLLECTOROUTPUT._serialized_end=6694
+  _FACETCOLLECTOR._serialized_start=6696
+  _FACETCOLLECTOR._serialized_end=6743
+  _FACETCOLLECTOROUTPUT._serialized_start=6746
+  _FACETCOLLECTOROUTPUT._serialized_end=6894
+  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_start=6844
+  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_end=6894
+  _RESERVOIRSAMPLINGCOLLECTOR._serialized_start=6896
+  _RESERVOIRSAMPLINGCOLLECTOR._serialized_end=6955
+  _RANDOMDOCUMENT._serialized_start=6957
+  _RANDOMDOCUMENT._serialized_end=7047
+  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_start=7049
+  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_end=7131
+  _TOPDOCSCOLLECTOR._serialized_start=7134
+  _TOPDOCSCOLLECTOR._serialized_end=7400
+  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_start=7336
+  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_end=7389
+  _DOCUMENTSCOLLECTOROUTPUT._serialized_start=7402
+  _DOCUMENTSCOLLECTOROUTPUT._serialized_end=7501
+  _AGGREGATIONCOLLECTOR._serialized_start=7504
+  _AGGREGATIONCOLLECTOR._serialized_end=7680
+  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_start=7603
+  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_end=7680
+  _AGGREGATIONCOLLECTOROUTPUT._serialized_start=7683
+  _AGGREGATIONCOLLECTOROUTPUT._serialized_end=7896
+  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_start=7807
+  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_end=7896
+  _AGGREGATIONRESULT._serialized_start=7899
+  _AGGREGATIONRESULT._serialized_end=8030
+  _BUCKETRESULT._serialized_start=8033
+  _BUCKETRESULT._serialized_end=8201
+  _RANGERESULT._serialized_start=8203
+  _RANGERESULT._serialized_end=8264
+  _HISTOGRAMRESULT._serialized_start=8266
+  _HISTOGRAMRESULT._serialized_end=8326
+  _TERMSRESULT._serialized_start=8329
+  _TERMSRESULT._serialized_end=8488
+  _METRICRESULT._serialized_start=8491
+  _METRICRESULT._serialized_end=8623
+  _SINGLEMETRICRESULT._serialized_start=8625
+  _SINGLEMETRICRESULT._serialized_end=8675
+  _STATSRESULT._serialized_start=8677
+  _STATSRESULT._serialized_end=8796
 # @@protoc_insertion_point(module_scope)
```

### Comparing `summa_embed-0.16.0/summa_embed/proto/query_pb2.pyi` & `summa_embed-0.17.0/summa_embed/proto/query_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -203,20 +203,22 @@
     def __init__(self, scored_documents: _Optional[_Iterable[_Union[ScoredDocument, _Mapping]]] = ..., has_next: bool = ...) -> None: ...
 
 class EmptyQuery(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class ExactMatchesPromoter(_message.Message):
-    __slots__ = ["boost", "slop"]
+    __slots__ = ["boost", "fields", "slop"]
     BOOST_FIELD_NUMBER: _ClassVar[int]
+    FIELDS_FIELD_NUMBER: _ClassVar[int]
     SLOP_FIELD_NUMBER: _ClassVar[int]
     boost: float
+    fields: _containers.RepeatedScalarFieldContainer[str]
     slop: int
-    def __init__(self, slop: _Optional[int] = ..., boost: _Optional[float] = ...) -> None: ...
+    def __init__(self, slop: _Optional[int] = ..., boost: _Optional[float] = ..., fields: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class ExistsQuery(_message.Message):
     __slots__ = ["field"]
     FIELD_FIELD_NUMBER: _ClassVar[int]
     field: str
     def __init__(self, field: _Optional[str] = ...) -> None: ...
 
@@ -237,22 +239,14 @@
         key: str
         value: int
         def __init__(self, key: _Optional[str] = ..., value: _Optional[int] = ...) -> None: ...
     FACET_COUNTS_FIELD_NUMBER: _ClassVar[int]
     facet_counts: _containers.ScalarMap[str, int]
     def __init__(self, facet_counts: _Optional[_Mapping[str, int]] = ...) -> None: ...
 
-class FieldMapper(_message.Message):
-    __slots__ = ["fields", "mapper_name"]
-    FIELDS_FIELD_NUMBER: _ClassVar[int]
-    MAPPER_NAME_FIELD_NUMBER: _ClassVar[int]
-    fields: _containers.RepeatedScalarFieldContainer[str]
-    mapper_name: str
-    def __init__(self, mapper_name: _Optional[str] = ..., fields: _Optional[_Iterable[str]] = ...) -> None: ...
-
 class Highlight(_message.Message):
     __slots__ = ["to"]
     FROM_FIELD_NUMBER: _ClassVar[int]
     TO_FIELD_NUMBER: _ClassVar[int]
     to: int
     def __init__(self, to: _Optional[int] = ..., **kwargs) -> None: ...
 
@@ -282,20 +276,14 @@
 
 class HistogramResult(_message.Message):
     __slots__ = ["buckets"]
     BUCKETS_FIELD_NUMBER: _ClassVar[int]
     buckets: _containers.RepeatedCompositeFieldContainer[BucketEntry]
     def __init__(self, buckets: _Optional[_Iterable[_Union[BucketEntry, _Mapping]]] = ...) -> None: ...
 
-class InflectionConfig(_message.Message):
-    __slots__ = ["derive_plural"]
-    DERIVE_PLURAL_FIELD_NUMBER: _ClassVar[int]
-    derive_plural: bool
-    def __init__(self, derive_plural: bool = ...) -> None: ...
-
 class Key(_message.Message):
     __slots__ = ["f64", "str"]
     F64_FIELD_NUMBER: _ClassVar[int]
     STR_FIELD_NUMBER: _ClassVar[int]
     f64: float
     str: str
     def __init__(self, str: _Optional[str] = ..., f64: _Optional[float] = ...) -> None: ...
@@ -352,14 +340,28 @@
     max_word_length: int
     min_doc_frequency: int
     min_term_frequency: int
     min_word_length: int
     stop_words: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, document: _Optional[str] = ..., min_doc_frequency: _Optional[int] = ..., max_doc_frequency: _Optional[int] = ..., min_term_frequency: _Optional[int] = ..., max_query_terms: _Optional[int] = ..., min_word_length: _Optional[int] = ..., max_word_length: _Optional[int] = ..., boost: _Optional[str] = ..., stop_words: _Optional[_Iterable[str]] = ...) -> None: ...
 
+class MorphologyConfig(_message.Message):
+    __slots__ = ["derive_tenses_coefficient"]
+    DERIVE_TENSES_COEFFICIENT_FIELD_NUMBER: _ClassVar[int]
+    derive_tenses_coefficient: float
+    def __init__(self, derive_tenses_coefficient: _Optional[float] = ...) -> None: ...
+
+class NerMatchesPromoter(_message.Message):
+    __slots__ = ["boost", "fields"]
+    BOOST_FIELD_NUMBER: _ClassVar[int]
+    FIELDS_FIELD_NUMBER: _ClassVar[int]
+    boost: float
+    fields: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, boost: _Optional[float] = ..., fields: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class PhraseQuery(_message.Message):
     __slots__ = ["field", "slop", "value"]
     FIELD_FIELD_NUMBER: _ClassVar[int]
     SLOP_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
     field: str
     slop: int
@@ -391,64 +393,68 @@
     phrase: PhraseQuery
     range: RangeQuery
     regex: RegexQuery
     term: TermQuery
     def __init__(self, boolean: _Optional[_Union[BooleanQuery, _Mapping]] = ..., match: _Optional[_Union[MatchQuery, _Mapping]] = ..., regex: _Optional[_Union[RegexQuery, _Mapping]] = ..., term: _Optional[_Union[TermQuery, _Mapping]] = ..., phrase: _Optional[_Union[PhraseQuery, _Mapping]] = ..., range: _Optional[_Union[RangeQuery, _Mapping]] = ..., all: _Optional[_Union[AllQuery, _Mapping]] = ..., more_like_this: _Optional[_Union[MoreLikeThisQuery, _Mapping]] = ..., boost: _Optional[_Union[BoostQuery, _Mapping]] = ..., disjunction_max: _Optional[_Union[DisjunctionMaxQuery, _Mapping]] = ..., empty: _Optional[_Union[EmptyQuery, _Mapping]] = ..., exists: _Optional[_Union[ExistsQuery, _Mapping]] = ...) -> None: ...
 
 class QueryParserConfig(_message.Message):
-    __slots__ = ["boolean_should_mode", "default_fields", "disjuction_max_mode", "exact_matches_promoter", "field_aliases", "field_boosts", "field_mappings", "inflection_configs", "missing_field_policy", "term_limit"]
+    __slots__ = ["boolean_should_mode", "default_fields", "disjuction_max_mode", "exact_matches_promoter", "field_aliases", "field_boosts", "missing_field_policy", "morphology_configs", "ner_matches_promoter", "query_language", "term_field_mapper_configs", "term_limit"]
     class FieldAliasesEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     class FieldBoostsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: float
         def __init__(self, key: _Optional[str] = ..., value: _Optional[float] = ...) -> None: ...
-    class FieldMappingsEntry(_message.Message):
+    class MorphologyConfigsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
-        value: FieldMapper
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[FieldMapper, _Mapping]] = ...) -> None: ...
-    class InflectionConfigsEntry(_message.Message):
+        value: MorphologyConfig
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[MorphologyConfig, _Mapping]] = ...) -> None: ...
+    class TermFieldMapperConfigsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
-        value: InflectionConfig
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[InflectionConfig, _Mapping]] = ...) -> None: ...
+        value: TermFieldMapperConfig
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[TermFieldMapperConfig, _Mapping]] = ...) -> None: ...
     BOOLEAN_SHOULD_MODE_FIELD_NUMBER: _ClassVar[int]
     DEFAULT_FIELDS_FIELD_NUMBER: _ClassVar[int]
     DISJUCTION_MAX_MODE_FIELD_NUMBER: _ClassVar[int]
     EXACT_MATCHES_PROMOTER_FIELD_NUMBER: _ClassVar[int]
     FIELD_ALIASES_FIELD_NUMBER: _ClassVar[int]
     FIELD_BOOSTS_FIELD_NUMBER: _ClassVar[int]
-    FIELD_MAPPINGS_FIELD_NUMBER: _ClassVar[int]
-    INFLECTION_CONFIGS_FIELD_NUMBER: _ClassVar[int]
     MISSING_FIELD_POLICY_FIELD_NUMBER: _ClassVar[int]
+    MORPHOLOGY_CONFIGS_FIELD_NUMBER: _ClassVar[int]
+    NER_MATCHES_PROMOTER_FIELD_NUMBER: _ClassVar[int]
+    QUERY_LANGUAGE_FIELD_NUMBER: _ClassVar[int]
+    TERM_FIELD_MAPPER_CONFIGS_FIELD_NUMBER: _ClassVar[int]
     TERM_LIMIT_FIELD_NUMBER: _ClassVar[int]
     boolean_should_mode: MatchQueryBooleanShouldMode
     default_fields: _containers.RepeatedScalarFieldContainer[str]
     disjuction_max_mode: MatchQueryDisjuctionMaxMode
     exact_matches_promoter: ExactMatchesPromoter
     field_aliases: _containers.ScalarMap[str, str]
     field_boosts: _containers.ScalarMap[str, float]
-    field_mappings: _containers.MessageMap[str, FieldMapper]
-    inflection_configs: _containers.MessageMap[str, InflectionConfig]
     missing_field_policy: MissingFieldPolicy
+    morphology_configs: _containers.MessageMap[str, MorphologyConfig]
+    ner_matches_promoter: NerMatchesPromoter
+    query_language: str
+    term_field_mapper_configs: _containers.MessageMap[str, TermFieldMapperConfig]
     term_limit: int
-    def __init__(self, field_aliases: _Optional[_Mapping[str, str]] = ..., field_boosts: _Optional[_Mapping[str, float]] = ..., field_mappings: _Optional[_Mapping[str, FieldMapper]] = ..., term_limit: _Optional[int] = ..., default_fields: _Optional[_Iterable[str]] = ..., boolean_should_mode: _Optional[_Union[MatchQueryBooleanShouldMode, _Mapping]] = ..., disjuction_max_mode: _Optional[_Union[MatchQueryDisjuctionMaxMode, _Mapping]] = ..., exact_matches_promoter: _Optional[_Union[ExactMatchesPromoter, _Mapping]] = ..., missing_field_policy: _Optional[_Union[MissingFieldPolicy, str]] = ..., inflection_configs: _Optional[_Mapping[str, InflectionConfig]] = ...) -> None: ...
+    def __init__(self, field_aliases: _Optional[_Mapping[str, str]] = ..., field_boosts: _Optional[_Mapping[str, float]] = ..., term_field_mapper_configs: _Optional[_Mapping[str, TermFieldMapperConfig]] = ..., term_limit: _Optional[int] = ..., default_fields: _Optional[_Iterable[str]] = ..., boolean_should_mode: _Optional[_Union[MatchQueryBooleanShouldMode, _Mapping]] = ..., disjuction_max_mode: _Optional[_Union[MatchQueryDisjuctionMaxMode, _Mapping]] = ..., exact_matches_promoter: _Optional[_Union[ExactMatchesPromoter, _Mapping]] = ..., missing_field_policy: _Optional[_Union[MissingFieldPolicy, str]] = ..., morphology_configs: _Optional[_Mapping[str, MorphologyConfig]] = ..., query_language: _Optional[str] = ..., ner_matches_promoter: _Optional[_Union[NerMatchesPromoter, _Mapping]] = ...) -> None: ...
 
 class RandomDocument(_message.Message):
     __slots__ = ["document", "index_alias", "score"]
     DOCUMENT_FIELD_NUMBER: _ClassVar[int]
     INDEX_ALIAS_FIELD_NUMBER: _ClassVar[int]
     SCORE_FIELD_NUMBER: _ClassVar[int]
     document: str
@@ -618,14 +624,20 @@
     avg: float
     count: int
     max: float
     min: float
     sum: float
     def __init__(self, count: _Optional[int] = ..., sum: _Optional[float] = ..., min: _Optional[float] = ..., max: _Optional[float] = ..., avg: _Optional[float] = ...) -> None: ...
 
+class TermFieldMapperConfig(_message.Message):
+    __slots__ = ["fields"]
+    FIELDS_FIELD_NUMBER: _ClassVar[int]
+    fields: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, fields: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class TermQuery(_message.Message):
     __slots__ = ["field", "value"]
     FIELD_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
     field: str
     value: str
     def __init__(self, field: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
```

### Comparing `summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/reflection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.pyi` & `summa_embed-0.17.0/summa_embed/proto/reflection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/search_service_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/search_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/search_service_pb2.pyi` & `summa_embed-0.17.0/summa_embed/proto/search_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/unixfs_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.pyi` & `summa_embed-0.17.0/summa_embed/proto/unixfs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/summa_embed/proto/utils_pb2.py` & `summa_embed-0.17.0/summa_embed/proto/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.16.0/Cargo.lock` & `summa_embed-0.17.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,25 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "aes"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "433cfd6710c9986c576a25ca913c39d66a6474107b406f34f91d4a8923395241"
+dependencies = [
+ "cfg-if",
+ "cipher",
+ "cpufeatures",
+]
+
+[[package]]
 name = "ahash"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
  "getrandom",
  "once_cell",
@@ -104,17 +115,17 @@
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
+checksum = "8868f09ff8cea88b079da74ae569d9b8c62a23c68c746240b704ee6f7525c89c"
 
 [[package]]
 name = "async-broadcast"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c48ccdbf6ca6b121e0f586cbc0e73ae440e56c67c30fa0873b4e110d9c26d2b"
 dependencies = [
@@ -221,14 +232,20 @@
 [[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
+name = "base64ct"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
+
+[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
@@ -264,39 +281,39 @@
 name = "blake2b_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c2f0dc9a68c6317d884f97cc36cf5a3d20ba14ce404227df55e1af708ab04bc"
 dependencies = [
  "arrayref",
  "arrayvec",
- "constant_time_eq",
+ "constant_time_eq 0.2.6",
 ]
 
 [[package]]
 name = "blake2s_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6637f448b9e61dfadbdcbae9a885fadee1f3eaffb1f8d3c1965d3ade8bdfd44f"
 dependencies = [
  "arrayref",
  "arrayvec",
- "constant_time_eq",
+ "constant_time_eq 0.2.6",
 ]
 
 [[package]]
 name = "blake3"
-version = "1.3.3"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42ae2468a89544a466886840aa467a25b766499f4f04bf7d9fcd10ecee9fccef"
+checksum = "729b71f35bd3fa1a4c86b85d32c8b9069ea7fe14f7a53cfabb65f62d4265b888"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if",
- "constant_time_eq",
+ "constant_time_eq 0.2.6",
 ]
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
@@ -319,14 +336,57 @@
 [[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
+name = "bzip2"
+version = "0.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
+dependencies = [
+ "bzip2-sys",
+ "libc",
+]
+
+[[package]]
+name = "bzip2-sys"
+version = "0.1.11+1.0.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "736a955f3fa7875102d57c82b8cac37ec45224a07fd32d58f9f7a186b6cd4cdc"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+]
+
+[[package]]
+name = "cached-path"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "097968e38f1319207f057d0f4d76452e4f4f847a5de61c5215379f297fa034f3"
+dependencies = [
+ "flate2",
+ "fs2",
+ "glob",
+ "indicatif",
+ "log",
+ "rand 0.8.5",
+ "reqwest",
+ "serde",
+ "serde_json",
+ "sha2",
+ "tar",
+ "tempfile",
+ "thiserror",
+ "zip",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 dependencies = [
  "jobserver",
 ]
@@ -366,27 +426,37 @@
  "multibase",
  "multihash 0.18.1",
  "serde",
  "unsigned-varint",
 ]
 
 [[package]]
+name = "cipher"
+version = "0.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
+dependencies = [
+ "crypto-common",
+ "inout",
+]
+
+[[package]]
 name = "clap"
-version = "4.3.2"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "401a4694d2bf92537b6867d94de48c4842089645fdcdf6c71865b175d836e9c2"
+checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.1"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
+checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "once_cell",
  "strsim",
@@ -429,28 +499,46 @@
  "serde",
  "serde_json",
  "toml",
  "yaml-rust",
 ]
 
 [[package]]
+name = "console"
+version = "0.15.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
+dependencies = [
+ "encode_unicode",
+ "lazy_static",
+ "libc",
+ "windows-sys 0.45.0",
+]
+
+[[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "constant_time_eq"
-version = "0.2.5"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
+
+[[package]]
+name = "constant_time_eq"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13418e745008f7349ec7e449155f419a61b92b58a99cc3616942b926825ec76b"
+checksum = "21a53c0a4d288377e7415b53dcfc3c04da5cdc2cc95c8d5ac178b58f0b861ad6"
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
 dependencies = [
@@ -510,30 +598,30 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
@@ -547,14 +635,35 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "csv"
+version = "1.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "626ae34994d3d8d668f4269922248239db4ae42d538b14c398b74a52208e8086"
+dependencies = [
+ "csv-core",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
+name = "csv-core"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
 dependencies = [
  "darling_core",
  "darling_macro",
@@ -659,14 +768,35 @@
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
+ "subtle",
+]
+
+[[package]]
+name = "dirs"
+version = "4.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
+dependencies = [
+ "dirs-sys",
+]
+
+[[package]]
+name = "dirs-sys"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi",
 ]
 
 [[package]]
 name = "dlv-list"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0688c2a7f92e427f44895cd63841bff7b29f8d7a1648b9e7e07a4a365b2e1257"
@@ -680,14 +810,29 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
+name = "encode_unicode"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
+
+[[package]]
+name = "encoding_rs"
+version = "0.8.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
@@ -711,15 +856,15 @@
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "examples"
 version = "0.0.0"
 dependencies = [
  "serde_json",
- "summa-proto 0.27.0",
+ "summa-proto 0.28.0",
  "tokio",
  "tonic 0.9.2",
 ]
 
 [[package]]
 name = "fail"
 version = "0.5.1"
@@ -804,14 +949,23 @@
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
+name = "form_urlencoded"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+dependencies = [
+ "percent-encoding",
+]
+
+[[package]]
 name = "format-bytes"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48942366ef93975da38e175ac9e10068c6fc08ca9e85930d4f098f4d5b14c2fd"
 dependencies = [
  "format-bytes-macros",
 ]
@@ -990,14 +1144,20 @@
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "h2"
 version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
 dependencies = [
  "bytes",
  "fnv",
@@ -1015,14 +1175,23 @@
 [[package]]
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
+name = "half"
+version = "2.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
+dependencies = [
+ "crunchy",
+]
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
  "ahash 0.7.6",
 ]
@@ -1079,14 +1248,23 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "hmac"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
+dependencies = [
+ "digest",
+]
+
+[[package]]
 name = "htmlescape"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9025058dae765dee5070ec375f591e2ba14638c63feff74f13805a72e523163"
 
 [[package]]
 name = "http"
@@ -1180,30 +1358,61 @@
 [[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
+name = "idna"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
+name = "indicatif"
+version = "0.16.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d207dc617c7a380ab07ff572a6e52fa202a2a8f355860ac9c38e23f8196be1b"
+dependencies = [
+ "console",
+ "lazy_static",
+ "number_prefix",
+ "regex",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "inout"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
  "js-sys",
@@ -1250,14 +1459,20 @@
  "cid 0.10.1",
  "ipfs-hamt-directory",
  "multihash 0.18.1",
  "pyo3",
 ]
 
 [[package]]
+name = "ipnet"
+version = "2.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+
+[[package]]
 name = "is-terminal"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
@@ -1298,17 +1513,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json5"
 version = "0.4.1"
@@ -1473,17 +1688,17 @@
 name = "lockfree-object-pool"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee33defb27b106378a6efcfcde4dda6226dfdac8ba7a2904f5bc93363cb88557"
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "loom"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff50ecb28bb86013e935fb6683ab1f6d3a20016f123c76fd4c27470076ac30f5"
 dependencies = [
@@ -1522,14 +1737,24 @@
 [[package]]
 name = "matchit"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b87248edafb776e59e6ee64a79086f65890d3510f2c656c000bf2a7e8a0aea40"
 
 [[package]]
+name = "matrixmultiply"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
+dependencies = [
+ "autocfg",
+ "rawpointer",
+]
+
+[[package]]
 name = "measure_time"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56220900f1a0923789ecd6bf25fbae8af3b2f1ff3e9e297fc9b6b8674dd4d852"
 dependencies = [
  "instant",
  "log",
@@ -1556,14 +1781,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "minicbor"
@@ -1697,14 +1931,27 @@
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
+name = "ndarray"
+version = "0.15.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
+dependencies = [
+ "matrixmultiply",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "rawpointer",
+]
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -1717,14 +1964,42 @@
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
+name = "num-complex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
+name = "num-traits"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
@@ -1748,14 +2023,20 @@
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "number_prefix"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oneshot"
@@ -1876,14 +2157,23 @@
  "rand 0.8.5",
  "thiserror",
  "tokio",
  "tokio-stream",
 ]
 
 [[package]]
+name = "ordered-float"
+version = "3.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fc2dbde8f8a79f2102cc474ceb0ad68e3b80b85289ea62389b60e66777e4213"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "ordered-multimap"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccd746e37177e1711c20dd619a1620f34f5c8b569c53590a72dedd5344d8924a"
 dependencies = [
  "dlv-list",
  "hashbrown 0.12.3",
@@ -1894,15 +2184,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -1944,15 +2234,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.3.5",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.0",
+]
+
+[[package]]
+name = "password-hash"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7676374caaee8a325c9e7a2ae557f216c5563a171d6997b0ef8a65af35147700"
+dependencies = [
+ "base64ct",
+ "rand_core 0.6.4",
+ "subtle",
 ]
 
 [[package]]
 name = "path-absolutize"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43eb3595c63a214e1b37b44f44b0a84900ef7ae0b4c5efce59e123d246d7a0de"
@@ -1972,14 +2273,26 @@
 [[package]]
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
+name = "pbkdf2"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
+dependencies = [
+ "digest",
+ "hmac",
+ "password-hash",
+ "sha2",
+]
+
+[[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pest"
@@ -2273,15 +2586,15 @@
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "serde",
  "unindent",
 ]
@@ -2444,14 +2757,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
+name = "rawpointer"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
+
+[[package]]
 name = "rayon"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
@@ -2485,17 +2804,17 @@
  "serde_json",
  "slab",
  "tokio",
 ]
 
 [[package]]
 name = "rdkafka-sys"
-version = "4.4.0+1.9.2"
+version = "4.5.0+1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87ac9d87c3aba1748e3112318459f2ac8bff80bfff7359e338e0463549590249"
+checksum = "1bb0676c2112342ac7165decdedbc4e7086c0af384479ccce534546b10687a5d"
 dependencies = [
  "libc",
  "libz-sys",
  "num_enum",
  "pkg-config",
 ]
 
@@ -2523,14 +2842,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_users"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+dependencies = [
+ "getrandom",
+ "redox_syscall 0.2.16",
+ "thiserror",
+]
+
+[[package]]
 name = "regex"
 version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
@@ -2564,14 +2894,51 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "reqwest"
+version = "0.11.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
+dependencies = [
+ "base64 0.21.2",
+ "bytes",
+ "encoding_rs",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-tls",
+ "ipnet",
+ "js-sys",
+ "log",
+ "mime",
+ "native-tls",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "tokio",
+ "tokio-native-tls",
+ "tower-service",
+ "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "winreg",
+]
+
+[[package]]
 name = "rlimit"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8a29d87a652dc4d43c586328706bb5cdff211f3f39a530f240b53f7221dab8e"
 dependencies = [
  "libc",
 ]
@@ -2584,14 +2951,34 @@
 dependencies = [
  "base64 0.13.1",
  "bitflags",
  "serde",
 ]
 
 [[package]]
+name = "rust-bert"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8792cccdf842159ef04a35f247df68ccc42192e9a67e389e6cd0f1a83970a6a0"
+dependencies = [
+ "cached-path",
+ "dirs",
+ "half 2.2.1",
+ "lazy_static",
+ "ordered-float",
+ "regex",
+ "rust_tokenizers",
+ "serde",
+ "serde_json",
+ "tch",
+ "thiserror",
+ "uuid",
+]
+
+[[package]]
 name = "rust-ini"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6d5f2436026b4f6e79dc829837d467cc7e9a55ee40e750d716713540715a2df"
 dependencies = [
  "cfg-if",
  "ordered-multimap",
@@ -2617,24 +3004,44 @@
  "filetime",
  "libipld",
  "quick-protobuf",
  "sha2",
 ]
 
 [[package]]
+name = "rust_tokenizers"
+version = "8.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f367f6b13bc686e822237b97caeb4b2e366dd1936ec204f11d266ede402c31b"
+dependencies = [
+ "csv",
+ "hashbrown 0.13.2",
+ "itertools",
+ "lazy_static",
+ "protobuf",
+ "rayon",
+ "regex",
+ "serde",
+ "serde_json",
+ "thiserror",
+ "unicode-normalization",
+ "unicode-normalization-alignments",
+]
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.19"
+version = "0.37.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -2649,14 +3056,24 @@
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
+name = "safetensors"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1d818a2cb3f564a1844be835011acf5c7ec8ad1986a47f73abc7b5fea91cc3a"
+dependencies = [
+ "serde",
+ "serde_json",
+]
+
+[[package]]
 name = "schannel"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
  "windows-sys 0.42.0",
 ]
@@ -2727,15 +3144,15 @@
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2bef2ebfde456fb76bbcf9f59315333decc4fda0b2b44b420243c11e0f5ec1f5"
 dependencies = [
- "half",
+ "half 1.8.2",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2754,14 +3171,26 @@
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_urlencoded"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
+dependencies = [
+ "form_urlencoded",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
 name = "serde_yaml"
 version = "0.8.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578a7433b776b56a35785ed5ce9a7e777ac0598aac5a6dd1b4b18a307c7fc71b"
 dependencies = [
  "indexmap",
  "ryu",
@@ -2894,16 +3323,22 @@
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
+name = "subtle"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
+
+[[package]]
 name = "summa-core"
-version = "0.16.0"
+version = "0.17.0"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "config",
  "derive_builder",
@@ -2922,44 +3357,45 @@
  "pest",
  "pest_derive",
  "pluralize-rs",
  "prost",
  "rand 0.8.5",
  "rayon",
  "regex",
+ "rust-bert",
  "rustc-hash",
  "serde",
  "serde_bytes",
  "serde_cbor",
  "serde_json",
  "serde_yaml",
  "strfmt",
- "summa-proto 0.27.0",
+ "summa-proto 0.28.0",
  "take_mut",
  "tantivy",
  "tantivy-common",
  "tantivy-query-grammar",
  "thiserror",
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.16.0"
+version = "0.17.0"
 dependencies = [
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "serde_json",
  "summa-core",
- "summa-proto 0.27.0",
+ "summa-proto 0.28.0",
  "tantivy",
  "tokio",
 ]
 
 [[package]]
 name = "summa-proto"
 version = "0.26.0"
@@ -2974,30 +3410,30 @@
  "tonic 0.8.3",
  "tonic-build 0.8.4",
  "tonic-reflection 0.6.0",
 ]
 
 [[package]]
 name = "summa-proto"
-version = "0.27.0"
+version = "0.28.0"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
  "tokio",
  "tonic 0.9.2",
  "tonic-build 0.9.2",
  "tonic-reflection 0.9.2",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.16.0"
+version = "0.17.0"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3017,15 +3453,15 @@
  "rdkafka",
  "rlimit",
  "serde",
  "serde_derive",
  "serde_json",
  "serde_yaml",
  "summa-core",
- "summa-proto 0.27.0",
+ "summa-proto 0.28.0",
  "take_mut",
  "tantivy",
  "tantivy-fst",
  "tempdir",
  "thiserror",
  "tikv-jemallocator",
  "time",
@@ -3056,15 +3492,15 @@
  "js-sys",
  "parking_lot 0.12.1",
  "prost",
  "serde",
  "serde-wasm-bindgen",
  "strfmt",
  "summa-core",
- "summa-proto 0.27.0",
+ "summa-proto 0.28.0",
  "tantivy",
  "thiserror",
  "tokio",
  "tracing",
  "tracing-wasm",
  "wasm-bindgen",
  "wasm-bindgen-futures",
@@ -3115,16 +3551,16 @@
 name = "take_mut"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
-version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+version = "0.20.2"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
@@ -3167,44 +3603,44 @@
  "tantivy-tokenizer-api",
  "tempfile",
  "thiserror",
  "time",
  "tokio",
  "uuid",
  "winapi",
- "zstd",
+ "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
-version = "0.3.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+version = "0.4.0"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time",
 ]
@@ -3218,62 +3654,90 @@
  "byteorder",
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
-version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+version = "0.20.0"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
- "zstd",
+ "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
+name = "tar"
+version = "0.4.38"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b55807c0344e1e6c04d7c965f5289c39a8d94ae23ed5c0b57aabac549f871c6"
+dependencies = [
+ "filetime",
+ "libc",
+ "xattr",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
+name = "tch"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9cbd9ce6fb581a1b918db880b649d1364b50f7f6717eda8497bcdc929cddd4b9"
+dependencies = [
+ "half 2.2.1",
+ "lazy_static",
+ "libc",
+ "ndarray",
+ "rand 0.8.5",
+ "safetensors",
+ "thiserror",
+ "torch-sys",
+ "zip",
+]
+
+[[package]]
 name = "tempdir"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15f2b5fb00ccdf689e0149d1b1b3c03fead81c2b37735d812fa8bddbbf41b6d8"
 dependencies = [
  "rand 0.4.6",
  "remove_dir_all",
@@ -3368,14 +3832,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
 name = "tokio"
 version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
@@ -3588,14 +4067,26 @@
  "tower-http",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
+name = "torch-sys"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42b2b81a479510717464df1d07c02cb4aebb26539a39b5db6637dda114a476cb"
+dependencies = [
+ "anyhow",
+ "cc",
+ "libc",
+ "zip",
+]
+
+[[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
  "futures-core",
  "futures-util",
@@ -3765,20 +4256,44 @@
 [[package]]
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
+name = "unicode-bidi"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
+name = "unicode-normalization"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+dependencies = [
+ "tinyvec",
+]
+
+[[package]]
+name = "unicode-normalization-alignments"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43f613e4fa046e69818dd287fdc4bc78175ff20331479dab6e1b0f98d57062de"
+dependencies = [
+ "smallvec",
+]
+
+[[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
 name = "unicode-xid"
@@ -3795,14 +4310,25 @@
 [[package]]
 name = "unsigned-varint"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d86a8dc7f45e4c1b0d30e43038c38f274e77af056aa5f74b93c2cf9eb3c1c836"
 
 [[package]]
+name = "url"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
+dependencies = [
+ "form_urlencoded",
+ "idna",
+ "percent-encoding",
+]
+
+[[package]]
 name = "urlencoding"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
 
 [[package]]
 name = "utf8-ranges"
@@ -3814,17 +4340,17 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.3.3"
+version = "1.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
+checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "valuable"
@@ -3869,83 +4395,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.36"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "which"
@@ -3982,15 +4508,15 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
@@ -4002,19 +4528,43 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.0",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
@@ -4109,38 +4659,95 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
+name = "winreg"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
+name = "xattr"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d1526bbe5aaeb5eb06885f4d987bcdfa5e23187055de9b83fe00156a821fabc"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
+name = "zip"
+version = "0.6.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
+dependencies = [
+ "aes",
+ "byteorder",
+ "bzip2",
+ "constant_time_eq 0.1.5",
+ "crc32fast",
+ "crossbeam-utils",
+ "flate2",
+ "hmac",
+ "pbkdf2",
+ "sha1",
+ "time",
+ "zstd 0.11.2+zstd.1.5.2",
+]
+
+[[package]]
+name = "zstd"
+version = "0.11.2+zstd.1.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
+dependencies = [
+ "zstd-safe 5.0.2+zstd.1.5.2",
+]
+
+[[package]]
 name = "zstd"
 version = "0.12.3+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
- "zstd-safe",
+ "zstd-safe 6.0.5+zstd.1.5.4",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "5.0.2+zstd.1.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
+dependencies = [
+ "libc",
+ "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-safe"
 version = "6.0.5+zstd.1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
```

