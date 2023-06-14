# Comparing `tmp/whylogs-1.1.9.tar.gz` & `tmp/whylogs-1.1.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.1.9.tar", max compression
+gzip compressed data, was "whylogs-1.1.9.dev0.tar", max compression
```

## Comparing `whylogs-1.1.9.tar` & `whylogs-1.1.9.dev0.tar`

### file list

```diff
@@ -1,174 +1,173 @@
--rw-r--r--   0        0        0    18554 2022-10-26 18:43:15.469277 whylogs-1.1.9/README.md
--rw-r--r--   0        0        0     4826 2022-10-26 18:47:38.393920 whylogs-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     1761 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/annotations.py
--rw-r--r--   0        0        0       51 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     5520 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     3802 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0     3411 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    11148 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     8953 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     1935 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     5806 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      558 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      317 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     3013 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0      465 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     1916 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      190 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4555 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0      904 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      518 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/store/query.py
--rw-r--r--   0        0        0       97 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/store/s3.py
--rw-r--r--   0        0        0     5566 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0      947 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1423 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     1935 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3329 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    17238 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1217 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0      818 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/core/__init__.py
--rw-r--r--   0        0        0     2567 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/core/common.py
--rw-r--r--   0        0        0      776 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/core/configs.py
--rw-r--r--   0        0        0      219 2022-10-26 18:43:15.501277 whylogs-1.1.9/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0      774 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2077 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     5477 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0    10380 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    10028 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4120 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/errors.py
--rw-r--r--   0        0        0     2426 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0      984 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4086 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     3853 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6459 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     6598 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4853 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    20478 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     7475 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     1666 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/registry.py
--rw-r--r--   0        0        0     4530 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5445 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0     8914 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7407 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2838 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     8128 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2022-10-26 18:47:42.910000 whylogs-1.1.9/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    19918 2022-10-26 18:47:41.045967 whylogs-1.1.9/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2022-10-26 18:47:41.045967 whylogs-1.1.9/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29018 2022-10-26 18:47:41.045967 whylogs-1.1.9/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2022-10-26 18:47:43.082003 whylogs-1.1.9/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24057 2022-10-26 18:47:41.045967 whylogs-1.1.9/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2022-10-26 18:47:40.921965 whylogs-1.1.9/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21183 2022-10-26 18:47:40.921965 whylogs-1.1.9/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     3230 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/resolvers.py
--rw-r--r--   0        0        0     6731 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/segment.py
--rw-r--r--   0        0        0     2138 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0     1185 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/stubs.py
--rw-r--r--   0        0        0      278 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     1546 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0      742 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     1054 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      126 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     1465 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0      508 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     5609 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    11899 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     7913 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      150 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/base.py
--rw-r--r--   0        0        0     4121 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6422 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0    11285 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10336 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0     2349 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11124 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/datasets/weather.py
--rw-r--r--   0        0        0     9980 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    12819 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/migration/converters.py
--rw-r--r--   0        0        0     3608 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/__init__.py
--rw-r--r--   0        0        0        0 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     1022 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2022-10-26 18:43:15.505277 whylogs-1.1.9/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2022-10-26 18:43:15.509277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2022-10-26 18:43:15.513277 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2022-10-26 18:43:15.517278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    47279 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    24533 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    14040 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    16125 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41450 2022-10-26 18:43:15.521278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    18039 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2422 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0     8631 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3510 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2434 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1061 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0     9942 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3480 2022-10-26 18:43:15.529278 whylogs-1.1.9/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0    21567 1970-01-01 00:00:00.000000 whylogs-1.1.9/setup.py
--rw-r--r--   0        0        0    21003 1970-01-01 00:00:00.000000 whylogs-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0    18554 2022-10-11 21:07:57.570274 whylogs-1.1.9.dev0/README.md
+-rw-r--r--   0        0        0     4836 2022-10-19 17:52:35.040274 whylogs-1.1.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1761 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/api/annotations.py
+-rw-r--r--   0        0        0       51 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     5520 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     3802 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0     3375 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    10269 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     7149 2022-10-19 16:56:58.610274 whylogs-1.1.9.dev0/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     5715 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      644 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      317 2022-06-01 15:15:01.442491 whylogs-1.1.9.dev0/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     3013 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0      465 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     1916 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      190 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4555 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0      904 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      518 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/api/store/query.py
+-rw-r--r--   0        0        0       97 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/api/store/s3.py
+-rw-r--r--   0        0        0     5566 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0      947 2022-10-18 14:29:29.390275 whylogs-1.1.9.dev0/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     2726 2022-10-18 14:29:29.390275 whylogs-1.1.9.dev0/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     1423 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     1935 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     3329 2022-10-18 14:29:29.390275 whylogs-1.1.9.dev0/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    17216 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0     1217 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0      818 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     2567 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/core/common.py
+-rw-r--r--   0        0        0      776 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/core/configs.py
+-rw-r--r--   0        0        0      219 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0      774 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2077 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     5477 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0    10380 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    10490 2022-10-19 17:50:04.170275 whylogs-1.1.9.dev0/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4094 2022-10-18 14:29:29.400275 whylogs-1.1.9.dev0/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/core/errors.py
+-rw-r--r--   0        0        0     2426 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0      984 2022-10-08 17:03:10.597321 whylogs-1.1.9.dev0/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4086 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     3853 2022-10-12 18:40:16.900275 whylogs-1.1.9.dev0/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6459 2022-10-12 18:40:16.900275 whylogs-1.1.9.dev0/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0     6598 2022-10-12 18:40:16.900275 whylogs-1.1.9.dev0/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4853 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2022-10-11 21:07:57.580274 whylogs-1.1.9.dev0/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    20478 2022-10-12 18:40:16.900275 whylogs-1.1.9.dev0/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     7475 2022-10-12 18:40:16.900275 whylogs-1.1.9.dev0/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     1666 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/core/metrics/registry.py
+-rw-r--r--   0        0        0     4530 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5445 2022-10-11 21:07:57.590274 whylogs-1.1.9.dev0/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0     8914 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7407 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2838 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     8131 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2022-10-19 17:55:02.210275 whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    19918 2022-10-19 17:55:01.470275 whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2022-10-19 17:55:01.470275 whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29018 2022-10-19 17:55:01.470275 whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2022-10-19 17:55:02.360274 whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24057 2022-10-19 17:55:01.470275 whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2022-10-19 17:55:01.330274 whylogs-1.1.9.dev0/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21183 2022-10-19 17:55:01.330274 whylogs-1.1.9.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     3230 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0     6731 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2138 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      932 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      278 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     1546 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0      742 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     1054 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      126 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     1465 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0      508 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2022-09-09 00:34:16.153342 whylogs-1.1.9.dev0/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     5609 2022-10-12 18:40:16.900275 whylogs-1.1.9.dev0/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    11899 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     7825 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      150 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     4121 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6422 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0    11285 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10336 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0     2349 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11124 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0     9980 2022-10-11 21:07:57.590274 whylogs-1.1.9.dev0/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    12819 2022-10-17 16:37:19.010275 whylogs-1.1.9.dev0/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     3608 2022-10-11 21:07:57.590274 whylogs-1.1.9.dev0/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2502 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     1022 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2022-05-31 19:33:45.922491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    47279 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    24533 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    14040 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    16125 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41450 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    18039 2022-10-11 21:07:57.590274 whylogs-1.1.9.dev0/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2022-05-31 19:33:45.932491 whylogs-1.1.9.dev0/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2422 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0     8654 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3510 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2434 2022-07-21 17:22:42.022760 whylogs-1.1.9.dev0/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1061 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0     9942 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3480 2022-10-08 17:03:10.607321 whylogs-1.1.9.dev0/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0    21582 1970-01-01 00:00:00.000000 whylogs-1.1.9.dev0/setup.py
+-rw-r--r--   0        0        0    21013 1970-01-01 00:00:00.000000 whylogs-1.1.9.dev0/PKG-INFO
```

### Comparing `whylogs-1.1.9/README.md` & `whylogs-1.1.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/pyproject.toml` & `whylogs-1.1.9.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.1.9"
+version = "1.1.9.dev0"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "README.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
 
@@ -36,15 +36,15 @@
 sphinx-inline-tabs = { version = "*", optional = true }
 ipython_genutils = {version = "^0.2.0", optional = true}
 nbsphinx = {version = "^0.8.9", optional = true}
 nbconvert = {version = "^7.0.0", optional = true}
 
 # Integrations dependencies
 boto3 = {version = "^1.22.13", optional = true }
-whylabs-client = {version = "0.4.0", optional = true}
+whylabs-client = {version = "0.4.0.dev0", optional = true}
 mlflow-skinny = {version = "^1.26.1", optional = true}
 google-cloud-storage = {version = "^2.5.0", optional = true}
 
 # Pyspark related dependencies
 pyarrow = {version = "^8.0.0", optional = true}
 pyspark = {version = "^3.0.0", optional = true}
```

### Comparing `whylogs-1.1.9/whylogs/__init__.py` & `whylogs-1.1.9.dev0/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/annotations.py` & `whylogs-1.1.9.dev0/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/fugue/profiler.py` & `whylogs-1.1.9.dev0/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/logger/__init__.py` & `whylogs-1.1.9.dev0/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/logger/logger.py` & `whylogs-1.1.9.dev0/whylogs/api/logger/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 class Logger(ABC):
     def __init__(self, schema: Optional[DatasetSchema] = None):
         self._is_closed = False
         self._schema = schema
         self._writers: List[Writer] = []
         atexit.register(self.close)
         self._store_list: List[ProfileStore] = []
-        self._segment_cache = None
 
     def check_writer(self, _: Writer) -> None:
         """Checks if a writer is configured correctly for this class"""
 
     def append_writer(self, name: Optional[str] = None, *, writer: Optional[Writer] = None, **kwargs: Any) -> None:
         if name is None and writer is None:
             raise ValueError("Must specify either the writer name or a Writer object")
@@ -73,23 +72,24 @@
             raise LoggingError("Cannot log to a closed logger")
         if obj is None and pandas is None and row is None:
             # TODO: check for shell environment and emit more verbose error string to let user know how to correct.
             raise LoggingError("log() was called without passing in any input!")
 
         # If segments are defined use segment_processing to return a SegmentedResultSet
         if self._schema and self._schema.segments:
-            return segment_processing(self._schema, obj, pandas, row, self._segment_cache)
+            return segment_processing(self._schema, obj, pandas, row)
 
         profiles = self._get_matching_profiles(obj, pandas=pandas, row=row)
 
         for prof in profiles:
             prof.track(obj, pandas=pandas, row=row)
 
         return ProfileResultSet(profiles[0])
 
+    @abstractmethod
     def close(self) -> None:
         self._is_closed = True
 
     def __enter__(self) -> "Logger":
         return self
 
     def __exit__(self, exception_type: Any, exception_value: Any, traceback: Any) -> None:
```

### Comparing `whylogs-1.1.9/whylogs/api/logger/result_set.py` & `whylogs-1.1.9.dev0/whylogs/api/logger/result_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC, abstractmethod
-from datetime import datetime
 from logging import getLogger
 from typing import Any, Dict, List, Optional
 
 from whylogs.api.reader import Reader, Readers
 from whylogs.api.writer import Writer, Writers
 from whylogs.api.writer.writer import Writable
 from whylogs.core import DatasetProfile, DatasetProfileView, Segment
@@ -87,43 +86,29 @@
     @abstractmethod
     def profile(self) -> Optional[DatasetProfile]:
         pass
 
     def get_writables(self) -> Optional[List[Writable]]:
         return [self.view()]
 
-    def set_dataset_timestamp(self, dataset_timestamp: datetime) -> None:
-        profile = self.profile()
-        if profile is None:
-            raise ValueError("Cannot set timestamp on a result set without a profile!")
-        else:
-            profile.set_dataset_timestamp(dataset_timestamp)
-
-    @property
-    def count(self) -> int:
-        result = 0
-        if self.view() is not None:
-            result = 1
-        return result
-
     @property
     def performance_metrics(self) -> Optional[ModelPerformanceMetrics]:
         profile = self.profile()
         if profile:
             return profile.model_performance_metrics
         return None
 
     def add_model_performance_metrics(self, metrics: ModelPerformanceMetrics) -> None:
         profile = self.profile()
         if profile:
             profile.add_model_performance_metrics(metrics)
         else:
             raise ValueError("Cannot add performance metrics to a result set with no profile!")
 
-    def add_metric(self, name: str, metric: Metric) -> None:
+    def add_metrics(self, name: str, metric: Metric) -> None:
         profile = self.profile()
         if profile:
             profile.add_dataset_metric(name, metric)
         else:
             raise ValueError(f"Cannot add {name} metric {metric} to a result set with no profile!")
 
 
@@ -179,24 +164,14 @@
             f"A profile was requested from a segmented result set without specifying which segment to return: {self._segments}"
         )
 
     @property
     def partitions(self) -> Optional[List[SegmentationPartition]]:
         return self._partitions
 
-    def set_dataset_timestamp(self, dataset_timestamp: datetime) -> None:
-        # TODO: pull dataset_timestamp up into a result set scoped property
-        segment_keys = self.segments()
-        if not segment_keys:
-            return
-        for key in segment_keys:
-            profile = self.profile(segment=key)
-            if profile:
-                profile.set_dataset_timestamp(dataset_timestamp)
-
     def segments(self, restrict_to_parition_id: Optional[str] = None) -> Optional[List[Segment]]:
         result: Optional[List[Segment]] = None
         if not self._segments:
             return result
         result = list()
         if restrict_to_parition_id:
             segments = self._segments.get(restrict_to_parition_id)
```

### Comparing `whylogs-1.1.9/whylogs/api/logger/rolling.py` & `whylogs-1.1.9.dev0/whylogs/api/logger/rolling.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,17 @@
 from datetime import datetime
 from threading import Timer
 from typing import Any, Callable, Dict, List, Optional
 
 from typing_extensions import Literal
 
 from whylogs.api.logger.logger import Logger
-from whylogs.api.logger.result_set import ProfileResultSet, ResultSet
-from whylogs.api.logger.segment_cache import SegmentCache
 from whylogs.api.writer import Writer
 from whylogs.core import DatasetProfile, DatasetProfileView, DatasetSchema
 from whylogs.core.stubs import pd
-from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
 
 logger = logging.getLogger(__name__)
 
 
 class Scheduler(object):
     """
     Multithreading scheduler.
@@ -103,16 +100,14 @@
             self.interval = 60 * 60 * 24  # one day
             self.suffix = "%Y-%m-%d"
         self.interval = self.interval * interval  # multiply by units requested
         self.utc = utc
 
         now = time.time()
         self._current_batch_timestamp = self._compute_current_batch_timestamp(now)
-        if schema and schema.segments:
-            self._segment_cache = SegmentCache(schema)
 
         self._current_profile: DatasetProfile = DatasetProfile(
             schema=schema,
             dataset_timestamp=datetime.utcfromtimestamp(self._current_batch_timestamp),
         )
 
         initial_run_after = (self._current_batch_timestamp + self.interval) - now
@@ -143,37 +138,24 @@
         self, obj: Any = None, *, pandas: Optional[pd.DataFrame] = None, row: Optional[Dict[str, Any]] = None
     ) -> List[DatasetProfile]:
         return [self._current_profile]
 
     def _do_rollover(self) -> None:
         if self._is_closed:
             return
+        old_profile = self._current_profile
 
         self._current_batch_timestamp = self._compute_current_batch_timestamp()
         dataset_timestamp = datetime.utcfromtimestamp(self._current_batch_timestamp)
-
-        if self._segment_cache:
-            self._flush(self._segment_cache.flush(dataset_timestamp))
-            return
-
-        old_profile = self._current_profile
-
         self._current_profile = DatasetProfile(
             schema=self._schema,
             dataset_timestamp=dataset_timestamp,
         )
 
-        while old_profile.is_active:
-            time.sleep(1)
-
-        if self.skip_empty and old_profile.is_empty:
-            logger.debug("skip_empty is set for profile. Skipping empty profile.")
-            return
-
-        self._flush(ProfileResultSet(old_profile))
+        self._flush(old_profile)
 
     def _get_time_tuple(self) -> time.struct_time:
         if self.utc:
             time_tuple = time.gmtime(self._current_batch_timestamp)
         else:
             time_tuple = time.localtime(self._current_batch_timestamp)
             current_time = int(time.time())
@@ -184,66 +166,48 @@
                 if dst_now:
                     addend = 3600
                 else:
                     addend = -3600
                 time_tuple = time.localtime(self._current_batch_timestamp + addend)
         return time_tuple
 
-    def _flush(self, results: ResultSet) -> None:
-        if results is None:
-            logger.debug("The result is None, skipping flush of result set.")
+    def _flush(self, profile: DatasetProfile) -> None:
+        if profile is None:
             return
-        if results.count == 0:
-            logger.debug("The result's count is zero, skipping flush of result set.")
+        if self.skip_empty and profile.is_empty:
+            logger.debug("skip_empty is set. Skipping empty profiles")
             return
-        profiles = results.get_writables()
-        if profiles is None:
-            logger.debug("The result set's writable is None, skipping flush of result set.")
-            return
-        number_of_profiles = len(profiles)
-        if number_of_profiles == 0:
-            logger.debug("The result set's writable list has length zero, skipping flush of result set.")
-            return
-        logger.debug(f"about to write {number_of_profiles} profiles.")
 
         pid = 0
         if self.fork:
             pid = os.fork()
 
         if pid > 0:
             logger.debug("Forked child process. Child process ID: %d", pid)
         else:
             if self.fork:
                 logger.debug("In child process")
             else:
                 logger.debug("Didn't fork. Writing in the same process")
 
             time_tuple = self._get_time_tuple()
+            timed_filename = f"{self.base_name}.{time.strftime(self.suffix, time_tuple)}{self.file_extension}"
 
-            profile_count = 0
-            for profile in profiles:
-                has_segments = isinstance(profile, SegmentedDatasetProfileView)
-                if has_segments:
-                    timed_filename = f"{self.base_name}.{time.strftime(self.suffix, time_tuple)}_{profile.get_segment_string()}{self.file_extension}"
-                else:
-                    timed_filename = f"{self.base_name}.{time.strftime(self.suffix, time_tuple)}{self.file_extension}"
-                logging.debug("Writing out put with timed_filename: %s", timed_filename)
+            logging.debug("Writing out put with timed_filename: %s", timed_filename)
 
-                profile_count = profile_count + 1
-                logger.debug(f"Writing profile {profile_count} of {number_of_profiles}")
+            while profile.is_active:
+                time.sleep(1)
 
-                for store in self._store_list:
-                    store.write(profile_view=profile, profile_name=self.base_name)
+            for store in self._store_list:
+                store.write(profile_view=profile.view(), profile_name=self.base_name)
 
-                for w in self._writers:
-                    w.write(file=profile, dest=timed_filename)
-                    if self._callback and callable(self._callback):
-                        self._callback(w, profile, timed_filename)
-                if not self._writers and self._callback and callable(self._callback):
-                    self._callback(None, profile, timed_filename)
+            for w in self._writers:
+                w.write(file=profile.view(), dest=timed_filename)
+                if self._callback and callable(self._callback):
+                    self._callback(w, profile.view(), timed_filename)
 
     def close(self) -> None:
         logging.debug("Closing the writer")
         if not self._is_closed:
             self._scheduler.stop()
             self._do_rollover()
-        super(TimedRollingLogger, self).close()
+        self._is_closed: bool = True
```

### Comparing `whylogs-1.1.9/whylogs/api/logger/segment_processing.py` & `whylogs-1.1.9.dev0/whylogs/api/logger/segment_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple
 
 from whylogs.api.logger.result_set import SegmentedResultSet
-from whylogs.api.logger.segment_cache import SegmentCache
+from whylogs.api.store.profile_store import ProfileStore
 from whylogs.core import DatasetSchema
 from whylogs.core.dataset_profile import DatasetProfile
 from whylogs.core.input_resolver import _pandas_or_dict
 from whylogs.core.segment import Segment
 from whylogs.core.segmentation_partition import SegmentationPartition, SegmentFilter
 from whylogs.core.stubs import pd
 
@@ -16,19 +16,19 @@
 
 
 def _process_segment(
     segmented_data: Any,
     segment_key: Segment,
     segments: Dict[Segment, Any],
     schema: DatasetSchema,
-    segment_cache: Optional[SegmentCache] = None,
+    store: Optional[ProfileStore] = None,
 ):
     profile = None
-    if segment_cache:
-        profile = segment_cache.get_or_create_matching_profile(segment_key)
+    if store:
+        profile = store.get_matching_profiles(segmented_data, segment=segment_key)
 
     if profile is None:
         profile = DatasetProfile(schema)
 
     profile.track(segmented_data)
     segments[segment_key] = profile
 
@@ -36,33 +36,33 @@
 def _process_simple_partition(
     partition_id: str,
     schema: DatasetSchema,
     segments: Dict[Segment, Any],
     columns: List[str],
     pandas: Optional[pd.DataFrame] = None,
     row: Optional[Mapping[str, Any]] = None,
-    segment_cache: Optional[SegmentCache] = None,
+    profile_cache: Optional[ProfileStore] = None,
 ):
     if pandas is not None:
         # simple means we can segment on column values
         grouped_data = pandas.groupby(columns)
         for group in grouped_data.groups.keys():
             pandas_segment = grouped_data.get_group(group)
             if isinstance(group, str):
                 segment_tuple_key: Tuple[str, ...] = (group,)
             elif isinstance(group, (List, Iterable, Iterator)):
                 segment_tuple_key = tuple(str(k) for k in group)
             else:
                 segment_tuple_key = (str(group),)
             segment_key = Segment(segment_tuple_key, partition_id)
-            _process_segment(pandas_segment, segment_key, segments, schema, segment_cache)
+            _process_segment(pandas_segment, segment_key, segments, schema, profile_cache)
     elif row:
         # TODO: consider if we need to combine with the column names
         segment_key = Segment(tuple(str(row[element]) for element in columns), partition_id)
-        _process_segment(row, segment_key, segments, schema, segment_cache)
+        _process_segment(row, segment_key, segments, schema, profile_cache)
 
 
 def _filter_inputs(
     filter: SegmentFilter, pandas: Optional[pd.DataFrame] = None, row: Optional[Mapping[str, Any]] = None
 ) -> Tuple[Optional[pd.DataFrame], Optional[Dict[str, Any]]]:
     assert (
         filter.filter_function or filter.query_string
@@ -86,35 +86,34 @@
 
 def _log_segment(
     partition: SegmentationPartition,
     schema: DatasetSchema,
     obj: Any = None,
     pandas: Optional[pd.DataFrame] = None,
     row: Optional[Mapping[str, Any]] = None,
-    segment_cache: Optional[SegmentCache] = None,
+    store: Optional[ProfileStore] = None,
 ) -> Dict[Segment, Any]:
     segments: Dict[Segment, Any] = {}
     pandas, row = _pandas_or_dict(obj, pandas, row)
     if partition.filter:
         pandas, row = _filter_inputs(partition.filter, pandas, row)
     if partition.simple:
         columns = partition.mapper.col_names if partition.mapper else None
         if columns:
-            _process_simple_partition(partition.id, schema, segments, columns, pandas, row, segment_cache)
+            _process_simple_partition(partition.id, schema, segments, columns, pandas, row, store)
     else:
         raise NotImplementedError("custom mapped segments not yet implemented")
     return segments
 
 
 def segment_processing(
     schema: DatasetSchema,
     obj: Any = None,
     pandas: Optional[pd.DataFrame] = None,
     row: Optional[Dict[str, Any]] = None,
-    segment_cache: Optional[SegmentCache] = None,
 ) -> SegmentedResultSet:
     number_of_partitions = len(schema.segments)
     logger.info(f"The specified schema defines segments with {number_of_partitions} partitions.")
     assert not (
         number_of_partitions > _MAX_SEGMENT_PARTITIONS
     ), f"Attempt to process {number_of_partitions} partitions is larger than the max of {_MAX_SEGMENT_PARTITIONS}, use a lower number of partitions"
     segmented_profiles = dict()
@@ -127,12 +126,12 @@
         if segment_partition.filter:
             # TODO segments filter
             logger.debug(f"{partition_name}: defines filter ({segment_partition.filter})")
         if segment_partition.mapper:
             logger.debug(
                 f"{partition_name}: defines mapper on colums ({segment_partition.mapper.col_names}) and id ({segment_partition.mapper.id})"
             )
-        partition_segments = _log_segment(segment_partition, schema, obj, pandas, row, segment_cache)
+        partition_segments = _log_segment(segment_partition, schema, obj, pandas, row)
         segmented_profiles[segment_partition.id] = partition_segments
         segment_partitions.append(segment_partition)
         logger.debug(f"Done profiling for partition with name({partition_name})")
     return SegmentedResultSet(segments=segmented_profiles, partitions=segment_partitions)
```

### Comparing `whylogs-1.1.9/whylogs/api/logger/transient.py` & `whylogs-1.1.9.dev0/whylogs/api/logger/transient.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,7 +9,13 @@
     def __init__(self, schema: Optional[DatasetSchema] = None):
         super(TransientLogger, self).__init__(schema)
 
     def _get_matching_profiles(
         self, obj: Any = None, *, pandas: Optional[pd.DataFrame] = None, row: Optional[Dict[str, Any]] = None
     ) -> List[DatasetProfile]:
         return [DatasetProfile(schema=self._schema)]
+
+    def flush(self) -> None:
+        pass
+
+    def close(self) -> None:
+        pass
```

### Comparing `whylogs-1.1.9/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.1.9.dev0/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/reader/local.py` & `whylogs-1.1.9.dev0/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/reader/reader.py` & `whylogs-1.1.9.dev0/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/reader/s3.py` & `whylogs-1.1.9.dev0/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/store/local_store.py` & `whylogs-1.1.9.dev0/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/store/profile_store.py` & `whylogs-1.1.9.dev0/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/store/query.py` & `whylogs-1.1.9.dev0/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/usage_stats/__init__.py` & `whylogs-1.1.9.dev0/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/writer/__init__.py` & `whylogs-1.1.9.dev0/whylogs/api/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/writer/gcs.py` & `whylogs-1.1.9.dev0/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/writer/local.py` & `whylogs-1.1.9.dev0/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/writer/mlflow.py` & `whylogs-1.1.9.dev0/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/writer/s3.py` & `whylogs-1.1.9.dev0/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/api/writer/whylabs.py` & `whylogs-1.1.9.dev0/whylogs/api/writer/whylabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,14 @@
 
             dataset_timestamp = view.dataset_timestamp or datetime.datetime.now(datetime.timezone.utc)
             dataset_timestamp_epoch = int(dataset_timestamp.timestamp() * 1000)
             response = self._do_upload(
                 dataset_timestamp=dataset_timestamp_epoch,
                 profile_path=tmp_file.name,
             )
-        # TODO: retry
         return response
 
     def _validate_api_key(self) -> None:
         if self._api_key is None:
             raise ValueError("Missing API key. Set it via WHYLABS_API_KEY environment variable or as an api_key option")
         if len(self._api_key) < 12:
             raise ValueError("API key too short")
```

### Comparing `whylogs-1.1.9/whylogs/api/writer/writer.py` & `whylogs-1.1.9.dev0/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/__init__.py` & `whylogs-1.1.9.dev0/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/column_profile.py` & `whylogs-1.1.9.dev0/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/configs.py` & `whylogs-1.1.9.dev0/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.1.9.dev0/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.1.9.dev0/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.1.9.dev0/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.1.9.dev0/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.1.9.dev0/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.1.9.dev0/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/dataset_profile.py` & `whylogs-1.1.9.dev0/whylogs/core/dataset_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,25 @@
             self._initialize_new_columns(tuple(new_cols))
 
         if pandas is not None:
             # TODO: iterating over each column in order assumes single column metrics
             #   but if we instead iterate over a new artifact contained in dataset profile: "MetricProfiles", then
             #   each metric profile can specify which columns its tracks, and we can call like this:
             #   metric_profile.track(pandas)
+            if pandas.empty:
+                logger.warning("whylogs was passed an empty pandas DataFrame so nothing to profile in this call.")
+                return
             for k in pandas.keys():
-                self._columns[k].track_column(pandas[k])
+                column_values = pandas.get(k)
+                if column_values is None:
+                    logger.error(
+                        f"whylogs was passed a pandas DataFrame with key [{k}] but DataFrame.get({k}) returned nothing!"
+                    )
+                else:
+                    self._columns[k].track_column(column_values)
             return
 
         if row is not None:
             for k in row.keys():
                 self._columns[k].track_column([row[k]])
             return
```

### Comparing `whylogs-1.1.9/whylogs/core/datatypes.py` & `whylogs-1.1.9.dev0/whylogs/core/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from decimal import Decimal
 from typing import Any, Generic, List, Optional, Type, TypeVar, Union
 
-from whylogs.core.stubs import is_not_stub, np
+from whylogs.core.stubs import np
 
 try:
     from pandas.core.api import CategoricalDtype
 except:  # noqa
     CategoricalDtype = None  # type: ignore
 
 NT = TypeVar("NT")
@@ -51,15 +51,15 @@
         if maybe_type:
             dtype_or_type = maybe_type  # type: ignore
 
         if not isinstance(dtype_or_type, type):
             return False
 
         if issubclass(dtype_or_type, (bool, int, np.number, np.bool_)):
-            if is_not_stub(np.issubdtype) and np.issubdtype(dtype_or_type, np.floating):
+            if np.issubdtype and np.issubdtype(dtype_or_type, np.floating):
                 return False
             if issubclass(dtype_or_type, (np.datetime64, np.timedelta64)):
                 return False
             else:
                 return True
         return False
```

### Comparing `whylogs-1.1.9/whylogs/core/errors.py` & `whylogs-1.1.9.dev0/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/feature_weights.py` & `whylogs-1.1.9.dev0/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/input_resolver.py` & `whylogs-1.1.9.dev0/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/__init__.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/aggregators.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/column_metrics.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/compound_metric.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/decorators.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/deserializers.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/maths.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/metric_components.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/metrics.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/multimetric.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/registry.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/serializers.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/metrics/unicode_range.py` & `whylogs-1.1.9.dev0/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.1.9.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.1.9.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.1.9.dev0/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/preprocessing.py` & `whylogs-1.1.9.dev0/whylogs/core/preprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import itertools
 import logging
 from dataclasses import dataclass
 from typing import Any, Iterable, Iterator, List, Optional
 
-from whylogs.core.stubs import is_not_stub, np, pd
+from whylogs.core.stubs import np as np
+from whylogs.core.stubs import pd as pd
 
 logger = logging.getLogger("whylogs.core.views")
 
 try:
     import pandas.core.dtypes.common as pdc
 except:  # noqa
     pass
@@ -183,15 +184,15 @@
                     result.numpy = NumpyView(ints=data.astype(int))
             else:
                 raise ValueError(f"Unsupported numpy type: {data.dtype}")
             return result
 
         if isinstance(data, List):
             result.len = len(data)
-            if is_not_stub(pd.Series):
+            if pd.Series:
                 return PreprocessedColumn.apply(pd.Series(data, dtype="object"))
 
             int_list = []
             float_list = []
             string_list = []
             obj_list = []
             null_count = 0
@@ -204,15 +205,15 @@
                     string_list.append(x)
                 elif x is not None:
                     obj_list.append(x)
                 else:
                     null_count += 1
 
             result.null_count = null_count
-            if is_not_stub(np.ndarray):
+            if np.ndarray:
                 ints = np.asarray(int_list, dtype=int)
                 floats = np.asarray(float_list, dtype=float)
 
                 result.numpy = NumpyView(ints=ints, floats=floats)
                 result.list = ListView(strings=string_list, objs=obj_list)
                 return result
             else:
```

### Comparing `whylogs-1.1.9/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.1.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.1.9.dev0/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.1.9.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/resolvers.py` & `whylogs-1.1.9.dev0/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/schema.py` & `whylogs-1.1.9.dev0/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/segmentation_partition.py` & `whylogs-1.1.9.dev0/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/stubs.py` & `whylogs-1.1.9.dev0/whylogs/core/stubs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from dataclasses import dataclass
-from typing import Any
 
 logger = logging.getLogger(__name__)
 
 try:
     import pandas as _pd
 except ImportError:  # noqa
     _pd = None  # type: ignore
@@ -21,35 +20,28 @@
     pass
 
 
 @dataclass(frozen=True)
 class NumpyStub:
     dtype: type = _StubClass
     number: type = _StubClass
-    bool_: type = _StubClass
     floating: type = _StubClass
     ndarray: type = _StubClass
     timedelta64: type = _StubClass
     datetime64: type = _StubClass
     unicode_: type = _StubClass
     issubdtype: type = _StubClass
 
 
 @dataclass(frozen=True)
 class PandasStub(object):
     Series: type = _StubClass
     DataFrame: type = _StubClass
 
 
-def is_not_stub(stubbed_class: Any) -> bool:
-    if stubbed_class and stubbed_class is not _StubClass and not isinstance(stubbed_class, (PandasStub, NumpyStub)):
-        return True
-    return False
-
-
 if _np is None:
     _np = NumpyStub()
 
 if _pd is None:
     _pd = PandasStub()
 
 np = _np
```

### Comparing `whylogs-1.1.9/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.1.9.dev0/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/utils/stats_calculations.py` & `whylogs-1.1.9.dev0/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/utils/utils.py` & `whylogs-1.1.9.dev0/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/validators/condition_validator.py` & `whylogs-1.1.9.dev0/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/view/column_profile_view.py` & `whylogs-1.1.9.dev0/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.1.9.dev0/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.1.9.dev0/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,18 +64,15 @@
         return self.profile_view.dataset_timestamp
 
     @property
     def creation_timestamp(self):
         return self.profile_view.creation_timestamp
 
     def get_default_path(self) -> str:
-        return f"profile_{self._profile_view.creation_timestamp}_{self.get_segment_string()}.bin"
-
-    def get_segment_string(self) -> str:
-        return f"{self._segment.parent_id}_{'_'.join(self._segment.key)}"
+        return f"profile_{self._profile_view.creation_timestamp}_{self._segment.parent_id}_{'_'.join(self._segment.key)}.bin"
 
     def _write_as_v0_message(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, str]:
         message_v0 = v1_to_dataset_profile_message_v0(self.profile_view, self.segment, self.partition)
         path = path or self.get_default_path()
         with open(path, "w+b") as out_f:
             write_delimited_protobuf(out_f, message_v0)
         return True, path
```

### Comparing `whylogs-1.1.9/whylogs/datasets/base.py` & `whylogs-1.1.9.dev0/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/datasets/configs.py` & `whylogs-1.1.9.dev0/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.1.9.dev0/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/datasets/descr/weather.rst` & `whylogs-1.1.9.dev0/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/datasets/ecommerce.py` & `whylogs-1.1.9.dev0/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/datasets/utils.py` & `whylogs-1.1.9.dev0/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/datasets/weather.py` & `whylogs-1.1.9.dev0/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/extras/image_metric.py` & `whylogs-1.1.9.dev0/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/migration/converters.py` & `whylogs-1.1.9.dev0/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/migration/uncompound.py` & `whylogs-1.1.9.dev0/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/enums/enums.py` & `whylogs-1.1.9.dev0/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.1.9.dev0/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.1.9.dev0/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.1.9.dev0/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.1.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.1.9.dev0/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.1.9.dev0/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/js/d3.min.js` & `whylogs-1.1.9.dev0/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/js/handlebars.js` & `whylogs-1.1.9.dev0/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.1.9.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.1.9.dev0/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/html/templates/index.html` & `whylogs-1.1.9.dev0/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.1.9.dev0/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.1.9.dev0/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.1.9.dev0/whylogs/viz/utils/drift_calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from whylogs.core.view.dataset_profile_view import DatasetProfileView  # type: ignore
 from whylogs.viz.utils.frequent_items_calculations import (
     FrequentStats,
     get_frequent_stats,
     zero_padding_frequent_items,
 )
 
-QUANTILES = list(np.linspace(0, 1, 100))
+QUANTILES = [0.0, 0.01, 0.05, 0.25, 0.5, 0.75, 0.95, 0.99, 1.0]
 
 
 class ColumnDriftValue(TypedDict):
     """p-value for applied statistical test, along with the name of the applied test."""
 
     p_value: float
     test: str
```

### Comparing `whylogs-1.1.9/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.1.9.dev0/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.1.9.dev0/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.1.9.dev0/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.1.9.dev0/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.1.9.dev0/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.1.9/setup.py` & `whylogs-1.1.9.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,22 +63,22 @@
  'gcs': ['google-cloud-storage>=2.5.0,<3.0.0'],
  'image': ['Pillow>=9.2.0,<10.0.0'],
  'mlflow': ['mlflow-skinny>=1.26.1,<2.0.0'],
  's3': ['boto3>=1.22.13,<2.0.0'],
  'spark': ['pyarrow>=8.0.0,<9.0.0', 'pyspark>=3.0.0,<4.0.0'],
  'viz': ['pybars3>=0.9,<0.10',
          'ipython',
-         'whylabs-client==0.4.0',
+         'whylabs-client==0.4.0.dev0',
          'Pillow>=9.2.0,<10.0.0'],
  'viz:python_version < "3.11"': ['scipy>=1.5'],
- 'whylabs': ['whylabs-client==0.4.0']}
+ 'whylabs': ['whylabs-client==0.4.0.dev0']}
 
 setup_kwargs = {
     'name': 'whylogs',
-    'version': '1.1.9',
+    'version': '1.1.9.dev0',
     'description': 'Profile and monitor your ML data pipeline end-to-end',
     'long_description': '<img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">\n<img src="https://i.imgur.com/nv33goV.png" width="35%"/>\n</br>\n\n<h1 align="center">The open standard for data logging\n\n </h1>\n  <h3 align="center">\n   <a href="https://whylogs.readthedocs.io/"><b>Documentation</b></a> &bull;\n   <a href="https://bit.ly/whylogsslack"><b>Slack Community</b></a> &bull;\n   <a href="https://github.com/whylabs/whylogs#python-quickstart"><b>Python Quickstart</b></a> &bull;\n   <a href="https://whylogs.readthedocs.io/en/latest/examples/integrations/writers/Writing_to_WhyLabs.html"><b>WhyLabs Quickstart</b></a>\n </h3>\n\n<p align="center">\n<a href="https://github.com/whylabs/whylogs-python/blob/mainline/LICENSE" target="_blank">\n    <img src="http://img.shields.io/:license-Apache%202-blue.svg" alt="License">\n</a>\n<a href="https://badge.fury.io/py/whylogs" target="_blank">\n    <img src="https://badge.fury.io/py/whylogs.svg" alt="PyPi Version">\n</a>\n<a href="https://github.com/python/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">\n</a>\n<a href="https://pepy.tech/project/whylogs" target="_blank">\n    <img src="https://pepy.tech/badge/whylogs" alt="PyPi Downloads">\n</a>\n<a href="bit.ly/whylogs" target="_blank">\n    <img src="https://github.com/whylabs/whylogs-python/workflows/whylogs%20CI/badge.svg" alt="CI">\n</a>\n<a href="https://codeclimate.com/github/whylabs/whylogs-python/maintainability" target="_blank">\n    <img src="https://api.codeclimate.com/v1/badges/442f6ca3dca1e583a488/maintainability" alt="Maintainability">\n</a>\n</p>\n\n## What is whylogs\n\nwhylogs is an open source library for logging any kind of data. With whylogs, users are able to generate summaries of their datasets (called _whylogs profiles_) which they can use to:\n\n1. Track changes in their dataset\n2. Create _data constraints_ to know whether their data looks the way it should\n3. Quickly visualize key summary statistics about their datasets\n\nThese three functionalities enable a variety of use cases for data scientists, machine learning engineers, and data engineers:\n\n- Detect data drift in model input features\n- Detect training-serving skew, concept drift, and model performance degradation\n- Validate data quality in model inputs or in a data pipeline\n- Perform exploratory data analysis of massive datasets\n- Track data distributions & data quality for ML experiments\n- Enable data auditing and governance across the organization\n- Standardize data documentation practices across the organization\n- And more\n\nwhylogs can be run in Python or [Apache Spark](https://docs.whylabs.ai/docs/spark-integration) (both PySpark and Scala) environments on a variety of [data types](#data-types). We [integrate](#integrations) with lots of other tools including Pandas, [AWS Sagemaker](https://aws.amazon.com/blogs/startups/preventing-amazon-sagemaker-model-degradation-with-whylabs/), [MLflow](https://docs.whylabs.ai/docs/mlflow-integration), [Flask](https://whylabs.ai/blog/posts/deploy-and-monitor-your-ml-application-with-flask-and-whylabs), [Ray](https://docs.whylabs.ai/docs/ray-integration), [RAPIDS](https://whylabs.ai/blog/posts/monitoring-high-performance-machine-learning-models-with-rapids-and-whylogs), [Apache Kafka](https://docs.whylabs.ai/docs/kafka-integration), and more.\n\n<a href="https://hub.whylabsapp.com/signup" target="_blank">\n    <img src="https://user-images.githubusercontent.com/7946482/193939278-66a36574-2f2c-482a-9811-ad4479f0aafe.png" alt="WhyLabs Signup">\n</a>\n\nIf you have any questions, comments, or just want to hang out with us, please join [our Slack Community](https://bit.ly/rsqrd-slack). In addition to joining the Slack Community, you can also help this project by giving us a ⭐ in the upper right corner of this page.\n\n## Python Quickstart<a name="python-quickstart" />\n\nInstalling whylogs using the pip package manager is as easy as running `pip install whylogs` in your terminal.\n\nFrom here, you can quickly log a dataset:\n\n```python\nimport whylogs as why\nimport pandas as pd\n\n#dataframe\ndf = pd.read_csv("path/to/file.csv")\nresults = why.log(df)\n```\n\nAnd voila, you now have a whylogs profile. To learn more about about a whylogs profile is and what you can do with it, read on.\n\n## Table of Contents\n\n- [whylogs Profiles](#whylogs-profiles)\n- [Data Constraints](#data-constraints)\n- [Profile Visualization](#profile-visualization)\n- [Integrations](#integrations)\n- [Supported Data Types](#data-types)\n- [Examples](#examples)\n- [Usage Statistics](#usage-statistics)\n- [Community](#community)\n- [Contribute](#contribute)\n\n## whylogs Profiles<a name="whylogs-profiles" />\n\n### What are profiles\n\nwhylogs profiles are the core of the whylogs library. They capture key statistical properties of data, such as the distribution (far beyond simple mean, median, and standard deviation measures), the number of missing values, and a wide range of configurable custom metrics. By capturing these summary statistics, we are able to accurately represent the data and enable all of the use cases described in the introduction.\n\nwhylogs profiles have three properties that make them ideal for data logging: they are **efficient**, **customizable**, and **mergeable**.\n\n<br />\n\n<img align="left" src="https://user-images.githubusercontent.com/7946482/171064257-26bf727e-3480-4ec3-9c9d-5d8a79567bca.png">\n\n**Efficient**: whylogs profiles efficiently describe the dataset that they represent. This high fidelity representation of datasets is what enables whylogs profiles to be effective snapshots of the data. They are better at capturing the characteristics of a dataset than a sample would be—as discussed in our [Data Logging: Sampling versus Profiling](https://whylabs.ai/blog/posts/data-logging-sampling-versus-profiling) blog post—and are very compact.\n\n<br />\n\n<img align="left" src="https://user-images.githubusercontent.com/7946482/171064575-72ee0f76-7365-4fd1-9cab-4debb673baa8.png">\n\n**Customizable**: The statistics that whylogs profiles collect are easily configured and customizable. This is useful because different data types and use cases require different metrics, and whylogs users need to be able to easily define custom trackers for those metrics. It’s the customizability of whylogs that enables our text, image, and other complex data trackers.\n\n<br />\n\n<img align="left" src="https://user-images.githubusercontent.com/7946482/171064525-2d314534-6cdb-4c07-9d9f-5c74d5c03029.png">\n\n**Mergeable**: One of the most powerful features of whylogs profiles is their mergeability. Mergeability means that whylogs profiles can be combined together to form new profiles which represent the aggregate of their constituent profiles. This enables logging for distributed and streaming systems, and allows users to view aggregated data across any time granularity.\n\n<br />\n\n### How do you generate profiles\n\nOnce whylogs is installed, it\'s easy to generate profiles in both Python and Java environments.\n\nTo generate a profile from a Pandas dataframe in Python, simply run:\n\n```python\nimport whylogs as why\nimport pandas as pd\n\n#dataframe\ndf = pd.read_csv("path/to/file.csv")\nresults = why.log(df)\n```\n\n<!---\nFor images, replace `df` with `image="path/to/image.png"`. Similarly, you can profile Python dicts by replacing the dataframe within the `log()` function with a Python `dict` object.\n--->\n\n### What can you do with profiles\n\nOnce you’ve generated whylogs profiles, a few things can be done with them:\n\nIn your local Python environment, you can set data constraints or visualize your profiles. Setting data constraints on your profiles allows you to get notified when your data don’t match your expectations, allowing you to do data unit testing and some baseline data monitoring. With the Profile Visualizer, you can visually explore your data, allowing you to understand it and ensure that your ML models are ready for production.\n\nIn addition, you can send whylogs profiles to the SaaS ML monitoring and AI observability platform [WhyLabs](https://whylabs.ai). With WhyLabs, you can automatically set up monitoring for your machine learning models, getting notified on both data quality and data change issues (such as data drift). If you’re interested in trying out WhyLabs, check out the always free [Starter edition](https://whylabs.ai/free), which allows you to experience the entire platform’s capabilities with no credit card required.\n\n## WhyLabs<a name="whylabs" />\n\nWhyLabs is a managed service offering built for helping users make the most of their whylogs profiles. With WhyLabs, users can ingest profiles and set up automated monitoring as well as gain full observability into their data and ML systems. With WhyLabs, users can ensure the reliability of their data and models, and debug any problems that arise with them.\n\nIngesting whylogs profiles into WhyLabs is easy. After obtaining your access credentials from the platform, you’ll need to set them in your Python environment, log a dataset, and write it to WhyLabs, like so:\n\n```python\nimport whylogs as why\nimport os\n\nos.environ["WHYLABS_DEFAULT_ORG_ID"] = "org-0" # ORG-ID is case-sensitive\nos.environ["WHYLABS_API_KEY"] = "YOUR-API-KEY"\nos.environ["WHYLABS_DEFAULT_DATASET_ID"] = "model-0" # The selected model project "MODEL-NAME" is "model-0"\n\nresults = why.log(df)\n\nresults.writer("whylabs").write()\n```\n\n![image](<https://github.com/whylabs/whylogs/blob/assets/images/chrome-capture-2022-9-4%20(1).gif>)\n\nIf you’re interested in trying out WhyLabs, check out the always free [Starter edition](https://hub.whylabsapp.com/signup), which allows you to experience the entire platform’s capabilities with no credit card required.\n\n## Data Constraints<a name="data-constraints" />\n\nConstraints are a powerful feature built on top of whylogs profiles that enable you to quickly and easily validate that your data looks the way that it should. There are numerous types of constraints that you can set on your data (that numerical data will always fall within a certain range, that text data will always be in a JSON format, etc) and, if your dataset fails to satisfy a constraint, you can fail your unit tests or your CI/CD pipeline.\n\nA simple example of setting and testing a constraint is:\n\n```python\nimport whylogs as why\nfrom whylogs.core.constraints import Constraints, ConstraintsBuilder, MetricsSelector, MetricConstraint\n\nprofile_view = why.log(df).view()\nbuilder = ConstraintsBuilder(profile_view)\n\nbuilder.add_constraint(MetricConstraint(\n    name="col_name >= 0",\n    condition=lambda x: x.min >= 0,\n    metric_selector=MetricsSelector(metric_name=\'distribution\', column_name=\'col_name\')\n))\nconstraints: Constraints = builder.build()\nconstraints.report()\n```\n\nTo learn more about constraints, check out: the [Constraints Example](https://bit.ly/whylogsconstraintsexample).\n\n## Profile Visualization<a name="profile-visualization" />\n\nIn addition to being able to automatically get notified about potential issues in data, it’s also useful to be able to inspect your data manually. With the profile visualizer, you can generate interactive reports about your profiles (either a single profile or comparing profiles against each other) directly in your Jupyter notebook environment. This enables exploratory data analysis, data drift detection, and data observability.\n\nTo access the profile visualizer, install the `[viz]` module of whylogs by running `pip install whylogs[viz]` in your terminal. One type of profile visualization that we can create is a drift report; here\'s a simple example of how to analyze the drift between two profiles:\n\n```python\nimport whylogs as why\n\nfrom whylogs.viz import NotebookProfileVisualizer\n\nresult = why.log(pandas=df_target)\nprof_view = result.view()\n\nresult_ref = why.log(pandas=df_reference)\nprof_view_ref = result_ref.view()\n\nvisualization = NotebookProfileVisualizer()\nvisualization.set_profiles(target_profile_view=prof_view, reference_profile_view=prof_view_ref)\n\nvisualization.summary_drift_report()\n```\n\n![image](https://user-images.githubusercontent.com/7946482/169669536-a25cce95-acde-4637-b7b9-c2a685f0bc3f.png)\n\nTo learn more about visualizing your profiles, check out: the [Visualizer Example](https://bit.ly/whylogsvisualizerexample)\n\n## Data Types<a name="data-types" />\n\nwhylogs supports both structured and unstructured data, specifically:\n\n| Data type        | Features | Notebook Example                                                                                                                                                |\n| ---------------- | -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| Tabular Data     | ✅       | [Getting started with structured data](https://github.com/whylabs/whylogs/blob/mainline/python/examples/basic/Getting_Started.ipynb)                            |\n| Image Data       | ✅       | [Getting started with images](https://github.com/whylabs/whylogs/blob/maintenance/0.7.x/examples/logging_images.ipynb)                                          |\n| Text Data        | ✅       | [String Features](https://github.com/whylabs/whylogs/blob/maintenance/0.7.x/examples/String_Features.ipynb)                                                     |\n| Embeddings       | 🛠        |                                                                                                                                                                 |\n| Other Data Types | ✋       | Do you have a request for a data type that you don’t see listed here? Raise an issue or join our Slack community and make a request! We’re always happy to help |\n\n## Integrations\n\n![current integration](https://user-images.githubusercontent.com/7946482/171062942-01c420f2-7768-4b7c-88b5-e3f291e1b7d8.png)\n| Integration | Features | Resources |\n| --- | --- | --- |\n| Spark | Run whylogs in Apache Spark environment| <ul><li>[Code Example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/integrations/Pyspark_Profiling.ipynb)</li></ul> |\n| Pandas | Log and monitor any pandas dataframe | <ul><li>[Notebook Example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/basic/Getting_Started.ipynb)</li><li>[whylogs: Embrace Data Logging](https://whylabs.ai/blog/posts/whylogs-embrace-data-logging)</li></ul> |\n| MLflow | Enhance MLflow metrics with whylogs: | <ul><li>[Notebook Example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/integrations/Mlflow_Logging.ipynb)</li><li>[Streamlining data monitoring with whylogs and MLflow](https://whylabs.ai/blog/posts/on-model-lifecycle-and-monitoring)</li></ul> |\n| Java | Run whylogs in Java environment| <ul><li>[Notebook Example](https://github.com/whylabs/whylogs-examples/blob/mainline/java/demo1/src/main/java/com/whylogs/examples/WhyLogsDemo.java)</li></ul> |\n| Docker | Run whylogs as in Docker | <ul><li>[Rest Container](https://docs.whylabs.ai/docs/integrations-rest-container)</li></ul>|\n| AWS S3 | Store whylogs profiles in S3 | <ul><li>[S3 example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/integrations/writers/Writing_Profiles.ipynb)</li></ul>\n| Flask | Integrate whylogs with your Flask Application| <ul><li>[Code Example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/integrations/flask_streaming/flask_with_whylogs.ipynb)</li></ul> |\n| Feast | Log features from your Feature Store with feast and whylogs| <ul><li>[Code Example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/integrations/Feature_Stores_and_whylogs.ipynb)</li></ul> |\n| BigQuery | Profile data queried from a Google BigQuery table| <ul><li>[Code Example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/integrations/BigQuery_Example.ipynb)</li></ul> |\n| WhyLabs | Monitor your profiles continuously with the WhyLabs Observability Platform| <ul><li>[Code Example](https://github.com/whylabs/whylogs/blob/mainline/python/examples/integrations/writers/Writing_to_WhyLabs.ipynb)</li></ul> |\n\n<!--| Kafka | Log and monitor Kafka topics with whylogs| <ul><li>[Notebook Example](https://github.com/whylabs/whylogs-examples/blob/mainline/python/Kafka.ipynb)</li><li> [Integrating whylogs into your Kafka ML Pipeline](https://whylabs.ai/blog/posts/integrating-whylogs-into-your-kafka-ml-pipeline) </li></ul>|-->\n<!--| Github actions | Unit test data with whylogs and github actions| <ul><li>[Notebook Example](https://github.com/whylabs/whylogs-examples/tree/mainline/github-actions)</li></ul> |-->\n<!--| RAPIDS | Use whylogs in RAPIDS environment | <ul><li>[Notebook Example](https://github.com/whylabs/whylogs-examples/blob/mainline/python/RAPIDS%20GPU%20Integration%20Example.ipynb)</li><li>[Monitoring High-Performance Machine Learning Models with RAPIDS and whylogs](https://whylabs.ai/blog/posts/monitoring-high-performance-machine-learning-models-with-rapids-and-whylogs)</li></ul> |-->\n\n## Examples\n\nFor a full set of our examples, please check out the [examples folder](https://github.com/whylabs/whylogs/tree/mainline/python/examples).\n\n## Usage Statistics<a name="whylogs-profiles" />\n\nStarting with whylogs v1.0.0, whylogs by default collects anonymous information about a user’s environment. These usage statistics do not include any information about the user or the data that they are profiling, only the environment that the user in which the user is running whylogs.\n\nTo read more about what usage statistics whylogs collects, check out the relevant [documentation](https://docs.whylabs.ai/docs/usage-statistics/).\n\nTo turn off Usage Statistics, simply set the `WHYLOGS_NO_ANALYTICS` environment variable to True, like so:\n\n```python\nimport os\nos.environ[\'WHYLOGS_NO_ANALYTICS\']=\'True\'\n```\n\n## Community\n\nIf you have any questions, comments, or just want to hang out with us, please join [our Slack channel](http://join.slack.whylabs.ai/).\n\n## Contribute\n\n### How to Contribute\n\nWe welcome contributions to whylogs. Please see our [contribution guide](https://github.com/whylabs/whylogs/blob/mainline/.github/CONTRIBUTING.md) and our [development guide](https://github.com/whylabs/whylogs/blob/mainline/.github/DEVELOPMENT.md) for details.\n\n### Contributors\n\n<a href="https://github.com/whylabs/whylogs/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=whylabs/whylogs" />\n</a>\n\nMade with [contrib.rocks](https://contrib.rocks).\n',
     'author': 'WhyLabs.ai',
     'author_email': 'support@whylabs.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://docs.whylabs.ai',
```

#### html2text {}

```diff
@@ -19,19 +19,19 @@
 'furo>=2022.3.4,<2023.0.0', 'sphinx-autobuild>=2021.3.14,<2022.0.0',
 'sphinxext-opengraph>=0.6.3,<0.7.0', 'sphinx-inline-tabs',
 'ipython_genutils>=0.2.0,<0.3.0', 'nbsphinx>=0.8.9,<0.9.0',
 'nbconvert>=7.0.0,<8.0.0'], 'fugue': ['fugue>=0.7.3,<0.8.0'], 'gcs': ['google-
 cloud-storage>=2.5.0,<3.0.0'], 'image': ['Pillow>=9.2.0,<10.0.0'], 'mlflow':
 ['mlflow-skinny>=1.26.1,<2.0.0'], 's3': ['boto3>=1.22.13,<2.0.0'], 'spark':
 ['pyarrow>=8.0.0,<9.0.0', 'pyspark>=3.0.0,<4.0.0'], 'viz':
-['pybars3>=0.9,<0.10', 'ipython', 'whylabs-client==0.4.0',
+['pybars3>=0.9,<0.10', 'ipython', 'whylabs-client==0.4.0.dev0',
 'Pillow>=9.2.0,<10.0.0'], 'viz:python_version < "3.11"': ['scipy>=1.5'],
-'whylabs': ['whylabs-client==0.4.0']} setup_kwargs = { 'name': 'whylogs',
-'version': '1.1.9', 'description': 'Profile and monitor your ML data pipeline
-end-to-end', 'long_description': '[https://static.scarf.sh/a.png?x-
+'whylabs': ['whylabs-client==0.4.0.dev0']} setup_kwargs = { 'name': 'whylogs',
+'version': '1.1.9.dev0', 'description': 'Profile and monitor your ML data
+pipeline end-to-end', 'long_description': '[https://static.scarf.sh/a.png?x-
 pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                    \n[https://i.imgur.com/nv33goV.png]\n\n\n
              ****** The open standard for data logging\n\n ******
 \n
   **** \n Documentation •\n Slack_Community •\n Python_Quickstart •\n WhyLabs
                                Quickstart\n ****
 \n\n
```

### Comparing `whylogs-1.1.9/PKG-INFO` & `whylogs-1.1.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.1.9
+Version: 1.1.9.dev0
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -44,15 +44,15 @@
 Requires-Dist: sphinx-autoapi; extra == "docs"
 Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0); extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0); extra == "docs"
 Requires-Dist: sphinx-inline-tabs; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinxext-opengraph (>=0.6.3,<0.7.0); extra == "docs"
 Requires-Dist: typing-extensions (>=3.10); python_version < "3.11"
-Requires-Dist: whylabs-client (==0.4.0); extra == "viz" or extra == "whylabs"
+Requires-Dist: whylabs-client (==0.4.0.dev0); extra == "viz" or extra == "whylabs"
 Requires-Dist: whylogs-sketching (>=3.4.1.dev3)
 Description-Content-Type: text/markdown
 
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
 <img src="https://i.imgur.com/nv33goV.png" width="35%"/>
 </br>
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1 Name: whylogs Version: 1.1.9 Summary: Profile and monitor
-your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai License:
-Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai Requires-Python:
->=3.7.1,<4 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Provides-Extra: datasets
-Provides-Extra: docs Provides-Extra: fugue Provides-Extra: gcs Provides-Extra:
-image Provides-Extra: mlflow Provides-Extra: s3 Provides-Extra: spark Provides-
-Extra: viz Provides-Extra: whylabs Requires-Dist: Pillow (>=9.2.0,<10.0.0);
-extra == "viz" or extra == "image" Requires-Dist: boto3 (>=1.22.13,<2.0.0);
-extra == "s3" Requires-Dist: fugue (>=0.7.3,<0.8.0); extra == "fugue" Requires-
-Dist: furo (>=2022.3.4,<2023.0.0); extra == "docs" Requires-Dist: google-cloud-
-storage (>=2.5.0,<3.0.0); extra == "gcs" Requires-Dist: importlib-metadata
-(<4.3); python_version < "3.8" Requires-Dist: ipython; extra == "viz" Requires-
-Dist: ipython_genutils (>=0.2.0,<0.3.0); extra == "docs" Requires-Dist: mlflow-
-skinny (>=1.26.1,<2.0.0); extra == "mlflow" Requires-Dist: myst-parser[sphinx]
-(>=0.17.2,<0.18.0); extra == "docs" Requires-Dist: nbconvert (>=7.0.0,<8.0.0);
-extra == "docs" Requires-Dist: nbsphinx (>=0.8.9,<0.9.0); extra == "docs"
-Requires-Dist: pandas; extra == "datasets" Requires-Dist: protobuf (>=3.19.4)
-Requires-Dist: pyarrow (>=8.0.0,<9.0.0); extra == "spark" Requires-Dist:
-pybars3 (>=0.9,<0.10); extra == "viz" Requires-Dist: pyspark (>=3.0.0,<4.0.0);
-extra == "spark" Requires-Dist: requests (>=2.27,<3.0); extra == "viz" or extra
-== "whylabs" Requires-Dist: scipy (>=1.5); (python_version < "3.11") and (extra
-== "viz") Requires-Dist: sphinx-autoapi; extra == "docs" Requires-Dist: sphinx-
-autobuild (>=2021.3.14,<2022.0.0); extra == "docs" Requires-Dist: sphinx-
-copybutton (>=0.5.0,<0.6.0); extra == "docs" Requires-Dist: sphinx-inline-tabs;
-extra == "docs" Requires-Dist: sphinx; extra == "docs" Requires-Dist:
-sphinxext-opengraph (>=0.6.3,<0.7.0); extra == "docs" Requires-Dist: typing-
-extensions (>=3.10); python_version < "3.11" Requires-Dist: whylabs-client
-(==0.4.0); extra == "viz" or extra == "whylabs" Requires-Dist: whylogs-
-sketching (>=3.4.1.dev3) Description-Content-Type: text/markdown [https://
+Metadata-Version: 2.1 Name: whylogs Version: 1.1.9.dev0 Summary: Profile and
+monitor your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai
+License: Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai
+Requires-Python: >=3.7.1,<4 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Provides-
+Extra: datasets Provides-Extra: docs Provides-Extra: fugue Provides-Extra: gcs
+Provides-Extra: image Provides-Extra: mlflow Provides-Extra: s3 Provides-Extra:
+spark Provides-Extra: viz Provides-Extra: whylabs Requires-Dist: Pillow
+(>=9.2.0,<10.0.0); extra == "viz" or extra == "image" Requires-Dist: boto3
+(>=1.22.13,<2.0.0); extra == "s3" Requires-Dist: fugue (>=0.7.3,<0.8.0); extra
+== "fugue" Requires-Dist: furo (>=2022.3.4,<2023.0.0); extra == "docs"
+Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0); extra == "gcs" Requires-
+Dist: importlib-metadata (<4.3); python_version < "3.8" Requires-Dist: ipython;
+extra == "viz" Requires-Dist: ipython_genutils (>=0.2.0,<0.3.0); extra ==
+"docs" Requires-Dist: mlflow-skinny (>=1.26.1,<2.0.0); extra == "mlflow"
+Requires-Dist: myst-parser[sphinx] (>=0.17.2,<0.18.0); extra == "docs"
+Requires-Dist: nbconvert (>=7.0.0,<8.0.0); extra == "docs" Requires-Dist:
+nbsphinx (>=0.8.9,<0.9.0); extra == "docs" Requires-Dist: pandas; extra ==
+"datasets" Requires-Dist: protobuf (>=3.19.4) Requires-Dist: pyarrow
+(>=8.0.0,<9.0.0); extra == "spark" Requires-Dist: pybars3 (>=0.9,<0.10); extra
+== "viz" Requires-Dist: pyspark (>=3.0.0,<4.0.0); extra == "spark" Requires-
+Dist: requests (>=2.27,<3.0); extra == "viz" or extra == "whylabs" Requires-
+Dist: scipy (>=1.5); (python_version < "3.11") and (extra == "viz") Requires-
+Dist: sphinx-autoapi; extra == "docs" Requires-Dist: sphinx-autobuild
+(>=2021.3.14,<2022.0.0); extra == "docs" Requires-Dist: sphinx-copybutton
+(>=0.5.0,<0.6.0); extra == "docs" Requires-Dist: sphinx-inline-tabs; extra ==
+"docs" Requires-Dist: sphinx; extra == "docs" Requires-Dist: sphinxext-
+opengraph (>=0.6.3,<0.7.0); extra == "docs" Requires-Dist: typing-extensions
+(>=3.10); python_version < "3.11" Requires-Dist: whylabs-client (==0.4.0.dev0);
+extra == "viz" or extra == "whylabs" Requires-Dist: whylogs-sketching
+(>=3.4.1.dev3) Description-Content-Type: text/markdown [https://
 static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                       [https://i.imgur.com/nv33goV.png]
                ****** The open standard for data logging ******
  **** Documentation • Slack_Community • Python_Quickstart • WhyLabs_Quickstart
                                      ****
       [License] [PyPi_Version] [Code_style:_black] [PyPi_Downloads] [CI]
                                [Maintainability]
```

