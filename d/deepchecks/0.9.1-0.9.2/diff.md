# Comparing `tmp/deepchecks-0.9.1.tar.gz` & `tmp/deepchecks-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchecks-0.9.1.tar", last modified: Tue Oct 25 06:23:44 2022, max compression
+gzip compressed data, was "deepchecks-0.9.2.tar", last modified: Mon Oct 31 15:39:39 2022, max compression
```

## Comparing `deepchecks-0.9.1.tar` & `deepchecks-0.9.2.tar`

### file list

```diff
@@ -1,297 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.920382 deepchecks-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-25 06:23:34.000000 deepchecks-0.9.1/DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34856 2022-10-25 06:23:34.000000 deepchecks-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-25 06:23:34.000000 deepchecks-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-10-25 06:23:44.920382 deepchecks-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22944 2022-10-25 06:23:34.000000 deepchecks-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-25 06:23:34.000000 deepchecks-0.9.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.884381 deepchecks-0.9.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-10-25 06:23:34.000000 deepchecks-0.9.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-10-25 06:23:34.000000 deepchecks-0.9.1/benchmarks/tabular_bench.py
--rw-r--r--   0 runner    (1001) docker     (121)     3425 2022-10-25 06:23:34.000000 deepchecks-0.9.1/benchmarks/vision_bench.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.884381 deepchecks-0.9.1/deepchecks/
--rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.884381 deepchecks-0.9.1/deepchecks/analytics/
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/analytics/anonymous_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.884381 deepchecks-0.9.1/deepchecks/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4680 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/check_json.py
--rw-r--r--   0 runner    (1001) docker     (121)    21335 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/check_result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.884381 deepchecks-0.9.1/deepchecks/core/check_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/check_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8234 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/check_utils/class_performance_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11605 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/check_utils/feature_label_correlation_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8200 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/check_utils/multivariate_drift_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10411 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3561 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (121)    14239 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/reduce_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.896381 deepchecks-0.9.1/deepchecks/core/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  3763713 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/resources/jupyterlab-plotly.js
--rw-r--r--   0 runner    (1001) docker     (121)    17493 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/resources/requirejs.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     9236 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/resources/suite-template-full.html
--rw-r--r--   0 runner    (1001) docker     (121)     8071 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/resources/suite-template.html
--rw-r--r--   0 runner    (1001) docker     (121)  3872309 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/resources/widgets-embed-amd.js
--rw-r--r--   0 runner    (1001) docker     (121)  2983941 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/resources/widgets-embed.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.896381 deepchecks-0.9.1/deepchecks/core/serialization/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7033 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.900381 deepchecks-0.9.1/deepchecks/core/serialization/check_failure/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_failure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_failure/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_failure/ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_failure/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_failure/wandb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_failure/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.900381 deepchecks-0.9.1/deepchecks/core/serialization/check_result/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14372 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_result/html.py
--rw-r--r--   0 runner    (1001) docker     (121)    10134 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_result/ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_result/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_result/wandb.py
--rw-r--r--   0 runner    (1001) docker     (121)     9617 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/check_result/widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    14052 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.900381 deepchecks-0.9.1/deepchecks/core/serialization/dataframe/
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/dataframe/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/dataframe/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.900381 deepchecks-0.9.1/deepchecks/core/serialization/suite_result/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/suite_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13493 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/suite_result/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     8419 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/suite_result/ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/suite_result/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/suite_result/wandb.py
--rw-r--r--   0 runner    (1001) docker     (121)    11510 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/serialization/suite_result/widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    19939 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/core/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.900381 deepchecks-0.9.1/deepchecks/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23374 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/ppscore.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/suites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.900381 deepchecks-0.9.1/deepchecks/tabular/
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/_shared_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8419 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/base_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.900381 deepchecks-0.9.1/deepchecks/tabular/checks/
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.904382 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/class_imbalance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/columns_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/conflicting_labels.py
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/data_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (121)     6434 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/feature_feature_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/feature_label_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6339 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/identifier_label_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4421 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/is_single_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     7816 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/mixed_data_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8862 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/mixed_nulls.py
--rw-r--r--   0 runner    (1001) docker     (121)    10496 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/outlier_sample_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/percent_of_nulls.py
--rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/special_chars.py
--rw-r--r--   0 runner    (1001) docker     (121)    16298 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/string_length_out_of_bounds.py
--rw-r--r--   0 runner    (1001) docker     (121)     7995 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/string_mismatch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.908382 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11950 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/boosting_overfit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5642 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/calibration_score.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/confusion_matrix_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     3634 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/model_inference_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/model_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     5054 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/multi_model_performance_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     5086 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/regression_error_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     3943 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/regression_systematic_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     8467 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/roc_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     8609 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/segment_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    20233 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/simple_model_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     7774 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/single_dataset_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    10711 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/train_test_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    15453 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/train_test_prediction_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)    11884 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/unused_features.py
--rw-r--r--   0 runner    (1001) docker     (121)    22061 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/weak_segments_performance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.908382 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10101 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/category_mismatch_train_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4710 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/datasets_size_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_overlap.py
--rw-r--r--   0 runner    (1001) docker     (121)     9529 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/feature_label_correlation_change.py
--rw-r--r--   0 runner    (1001) docker     (121)     3814 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/index_leakage.py
--rw-r--r--   0 runner    (1001) docker     (121)     7547 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/multivariate_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/new_label_train_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9134 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/string_mismatch_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)    14188 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/train_test_feature_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)     9069 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/train_test_label_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)     7794 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/train_test_samples_mix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/whole_dataset_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)    21325 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    49335 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.908382 deepchecks-0.9.1/deepchecks/tabular/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.908382 deepchecks-0.9.1/deepchecks/tabular/datasets/classification/
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8598 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/classification/adult.py
--rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/classification/breast_cancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/classification/iris.py
--rw-r--r--   0 runner    (1001) docker     (121)     6976 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/classification/lending_club.py
--rw-r--r--   0 runner    (1001) docker     (121)    10168 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/classification/phishing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.908382 deepchecks-0.9.1/deepchecks/tabular/datasets/regression/
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6463 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/regression/airbnb.py
--rw-r--r--   0 runner    (1001) docker     (121)     6557 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/regression/avocado.py
--rw-r--r--   0 runner    (1001) docker     (121)     5383 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/datasets/regression/wine_quality.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4317 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/feature_importance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.908382 deepchecks-0.9.1/deepchecks/tabular/integrations/
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/integrations/h2o.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.912382 deepchecks-0.9.1/deepchecks/tabular/metric_utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/metric_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9124 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/metric_utils/additional_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    21891 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/metric_utils/scorers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/model_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7272 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.912382 deepchecks-0.9.1/deepchecks/tabular/suites/
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17355 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/suites/default_suites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.912382 deepchecks-0.9.1/deepchecks/tabular/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15792 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/utils/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/utils/feature_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/utils/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/utils/task_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/utils/task_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/tabular/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.912382 deepchecks-0.9.1/deepchecks/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/array_math.py
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/correlation_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     7092 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6517 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/dict_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.912382 deepchecks-0.9.1/deepchecks/utils/distribution/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22570 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/distribution/drift.py
--rw-r--r--   0 runner    (1001) docker     (121)    15146 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/distribution/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     9713 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/distribution/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3917 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/distribution/rare_category_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)    11425 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/distribution/trust_score.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/docref.py
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/function.py
--rw-r--r--   0 runner    (1001) docker     (121)     9941 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/gower_distance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (121)    11887 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3903 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.912382 deepchecks-0.9.1/deepchecks/utils/performance/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16006 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/performance/error_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    12625 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/performance/partition.py
--rw-r--r--   0 runner    (1001) docker     (121)     7290 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/simple_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4294 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/single_sample_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    20082 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/utils/wandb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/_shared_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11504 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/base_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     7398 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/batch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/checks/
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15400 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/abstract_property_outliers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3752 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/image_property_outliers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5348 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/label_property_outliers.py
--rw-r--r--   0 runner    (1001) docker     (121)     9301 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/property_label_correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9581 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/class_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    10119 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    16275 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/image_segment_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)     6244 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/mean_average_precision_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     4461 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/mean_average_recall_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     8699 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/model_error_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    22108 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/robustness_report.py
--rw-r--r--   0 runner    (1001) docker     (121)    17565 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/simple_model_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     9429 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/single_dataset_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    14783 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/train_test_prediction_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13667 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/heatmap_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     9489 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/image_dataset_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)    13794 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/image_property_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)     8767 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/new_labels.py
--rw-r--r--   0 runner    (1001) docker     (121)    18413 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/property_label_correlation_change.py
--rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/similar_image_leakage.py
--rw-r--r--   0 runner    (1001) docker     (121)    14067 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/train_test_label_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)     5578 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/classification_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    14174 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/datasets/classification/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7411 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/classification/mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.916382 deepchecks-0.9.1/deepchecks/vision/datasets/detection/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14563 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/detection/coco.py
--rw-r--r--   0 runner    (1001) docker     (121)     7336 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/detection/yolo_to_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.920382 deepchecks-0.9.1/deepchecks/vision/datasets/segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13897 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/datasets/segmentation/segmentation_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)    10236 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/detection_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.920382 deepchecks-0.9.1/deepchecks/vision/metrics_utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/confusion_matrix_counts_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/custom_scorer.py
--rw-r--r--   0 runner    (1001) docker     (121)    18114 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/detection_precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (121)     7420 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/detection_tp_fp_fn_calc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4079 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/iou_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/metric_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    13318 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/scorers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/semantic_segmentation_metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6428 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/metrics_utils/semantic_segmentation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/segmentation_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     8101 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/simple_classification_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11295 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.920382 deepchecks-0.9.1/deepchecks/vision/suites/
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14690 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/suites/default_suites.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/task_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.920382 deepchecks-0.9.1/deepchecks/vision/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11176 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/detection_formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7810 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/image_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6666 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/image_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6510 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/label_prediction_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/property_label_correlation_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9736 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/transformations.py
--rw-r--r--   0 runner    (1001) docker     (121)     8080 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/utils/vision_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    27677 2022-10-25 06:23:34.000000 deepchecks-0.9.1/deepchecks/vision/vision_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.884381 deepchecks-0.9.1/deepchecks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-10-25 06:23:44.000000 deepchecks-0.9.1/deepchecks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12127 2022-10-25 06:23:44.000000 deepchecks-0.9.1/deepchecks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 06:23:44.000000 deepchecks-0.9.1/deepchecks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-10-25 06:23:44.000000 deepchecks-0.9.1/deepchecks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-25 06:23:44.000000 deepchecks-0.9.1/deepchecks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:44.920382 deepchecks-0.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-10-25 06:23:34.000000 deepchecks-0.9.1/requirements/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 06:23:34.000000 deepchecks-0.9.1/requirements/nlp-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-10-25 06:23:34.000000 deepchecks-0.9.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-25 06:23:34.000000 deepchecks-0.9.1/requirements/vision-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-25 06:23:44.920382 deepchecks-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-10-25 06:23:34.000000 deepchecks-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.179315 deepchecks-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-31 15:39:28.000000 deepchecks-0.9.2/DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    34856 2022-10-31 15:39:28.000000 deepchecks-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-31 15:39:28.000000 deepchecks-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-10-31 15:39:39.179315 deepchecks-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    22944 2022-10-31 15:39:28.000000 deepchecks-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-31 15:39:28.000000 deepchecks-0.9.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.147315 deepchecks-0.9.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-10-31 15:39:28.000000 deepchecks-0.9.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-10-31 15:39:28.000000 deepchecks-0.9.2/benchmarks/tabular_bench.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3425 2022-10-31 15:39:28.000000 deepchecks-0.9.2/benchmarks/vision_bench.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.147315 deepchecks-0.9.2/deepchecks/
+-rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.147315 deepchecks-0.9.2/deepchecks/analytics/
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/analytics/anonymous_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.151315 deepchecks-0.9.2/deepchecks/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4680 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/check_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21335 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/check_result.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.151315 deepchecks-0.9.2/deepchecks/core/check_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/check_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8234 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/check_utils/class_performance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11605 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/check_utils/feature_label_correlation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8354 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/check_utils/multivariate_drift_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10411 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3561 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14239 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/reduce_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.159315 deepchecks-0.9.2/deepchecks/core/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)  3763713 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/resources/jupyterlab-plotly.js
+-rw-r--r--   0 runner    (1001) docker     (121)    17493 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/resources/requirejs.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9236 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/resources/suite-template-full.html
+-rw-r--r--   0 runner    (1001) docker     (121)     8071 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/resources/suite-template.html
+-rw-r--r--   0 runner    (1001) docker     (121)  3872309 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/resources/widgets-embed-amd.js
+-rw-r--r--   0 runner    (1001) docker     (121)  2983941 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/resources/widgets-embed.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.159315 deepchecks-0.9.2/deepchecks/core/serialization/
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7033 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.159315 deepchecks-0.9.2/deepchecks/core/serialization/check_failure/
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_failure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_failure/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_failure/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_failure/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_failure/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_failure/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.163315 deepchecks-0.9.2/deepchecks/core/serialization/check_result/
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14372 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_result/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10134 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_result/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_result/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6663 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_result/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9617 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/check_result/widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14052 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/common.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.163315 deepchecks-0.9.2/deepchecks/core/serialization/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/dataframe/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/dataframe/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.163315 deepchecks-0.9.2/deepchecks/core/serialization/suite_result/
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/suite_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13493 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/suite_result/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8419 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/suite_result/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/suite_result/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/suite_result/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11510 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/serialization/suite_result/widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19939 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/core/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.163315 deepchecks-0.9.2/deepchecks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23374 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/ppscore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/suites.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.163315 deepchecks-0.9.2/deepchecks/tabular/
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/_shared_docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9892 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/base_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.163315 deepchecks-0.9.2/deepchecks/tabular/checks/
+-rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.163315 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/class_imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/columns_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/conflicting_labels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/data_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6434 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/feature_feature_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/feature_label_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6339 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/identifier_label_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4421 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/is_single_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7816 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/mixed_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8862 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/mixed_nulls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10496 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/outlier_sample_detection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/percent_of_nulls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/special_chars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16298 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/string_length_out_of_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7995 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/string_mismatch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11950 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/boosting_overfit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5642 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/calibration_score.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/confusion_matrix_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3634 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/model_inference_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5653 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/multi_model_performance_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7135 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/regression_error_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/regression_systematic_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8467 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/roc_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8609 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/segment_performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20830 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/simple_model_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7782 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/single_dataset_performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10734 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/train_test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15453 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/train_test_prediction_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11884 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/unused_features.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22088 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/weak_segments_performance.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10101 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/category_mismatch_train_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4710 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/datasets_size_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9529 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/feature_label_correlation_change.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3814 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/index_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7547 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/multivariate_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/new_label_train_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9134 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/string_mismatch_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14188 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/train_test_feature_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9069 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/train_test_label_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7794 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/train_test_samples_mix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/whole_dataset_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21368 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48146 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/datasets/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8598 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/classification/adult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/classification/breast_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/classification/iris.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6976 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/classification/lending_club.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10168 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/classification/phishing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/datasets/regression/
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6463 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/regression/airbnb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6557 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/regression/avocado.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5383 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/datasets/regression/wine_quality.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/deprecation_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4871 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/feature_importance.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/integrations/
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/integrations/h2o.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/metric_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/metric_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12188 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/metric_utils/additional_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21491 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/metric_utils/scorers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7272 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/suites/
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17257 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/suites/default_suites.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.167315 deepchecks-0.9.2/deepchecks/tabular/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16791 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/utils/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/utils/feature_inference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/utils/messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4438 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/utils/task_inference.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/utils/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/tabular/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.171315 deepchecks-0.9.2/deepchecks/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/array_math.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5592 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/correlation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7092 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6517 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/dict_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.171315 deepchecks-0.9.2/deepchecks/utils/distribution/
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22570 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/distribution/drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15146 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/distribution/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9713 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/distribution/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3917 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/distribution/rare_category_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11425 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/distribution/trust_score.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/docref.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9941 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/gower_distance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11887 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3903 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.171315 deepchecks-0.9.2/deepchecks/utils/performance/
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16280 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/performance/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12625 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/performance/partition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7290 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/simple_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4294 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/single_sample_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20274 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/utils/wandb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.171315 deepchecks-0.9.2/deepchecks/vision/
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/_shared_docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12336 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/base_checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7398 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/batch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.171315 deepchecks-0.9.2/deepchecks/vision/checks/
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/
+-rw-r--r--   0 runner    (1001) docker     (121)      877 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15400 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/abstract_property_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3752 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/image_property_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5348 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/label_property_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9301 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/property_label_correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10107 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/class_performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10119 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16788 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/image_segment_performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6244 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/mean_average_precision_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4461 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/mean_average_recall_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8699 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/model_error_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22641 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/robustness_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17973 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/simple_model_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9429 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/single_dataset_performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14783 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/train_test_prediction_drift.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13667 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/heatmap_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9489 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/image_dataset_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13794 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/image_property_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8767 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/new_labels.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18413 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/property_label_correlation_change.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/similar_image_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14067 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/train_test_label_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5578 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/classification_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14174 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/datasets/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7411 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/classification/mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/datasets/detection/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14563 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/detection/coco.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7336 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/detection/yolo_to_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/datasets/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13897 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/datasets/segmentation/segmentation_coco.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/deprecation_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10236 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/detection_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/metrics_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/confusion_matrix_counts_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/custom_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18114 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/detection_precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7420 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/detection_tp_fp_fn_calc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4079 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/iou_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/metric_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13495 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/scorers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/semantic_segmentation_metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6428 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/metrics_utils/semantic_segmentation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/segmentation_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8101 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/simple_classification_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11295 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.175315 deepchecks-0.9.2/deepchecks/vision/suites/
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14690 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/suites/default_suites.py
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/task_type.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.179315 deepchecks-0.9.2/deepchecks/vision/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11176 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/detection_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7810 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/image_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6666 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/image_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6510 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/label_prediction_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/property_label_correlation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9736 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8080 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/utils/vision_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27677 2022-10-31 15:39:28.000000 deepchecks-0.9.2/deepchecks/vision/vision_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.147315 deepchecks-0.9.2/deepchecks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-10-31 15:39:39.000000 deepchecks-0.9.2/deepchecks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12127 2022-10-31 15:39:39.000000 deepchecks-0.9.2/deepchecks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 15:39:39.000000 deepchecks-0.9.2/deepchecks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-10-31 15:39:39.000000 deepchecks-0.9.2/deepchecks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-31 15:39:39.000000 deepchecks-0.9.2/deepchecks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:39.179315 deepchecks-0.9.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2022-10-31 15:39:28.000000 deepchecks-0.9.2/requirements/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 15:39:28.000000 deepchecks-0.9.2/requirements/nlp-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-10-31 15:39:28.000000 deepchecks-0.9.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-31 15:39:28.000000 deepchecks-0.9.2/requirements/vision-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 15:39:39.179315 deepchecks-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-10-31 15:39:28.000000 deepchecks-0.9.2/setup.py
```

### Comparing `deepchecks-0.9.1/DESCRIPTION.rst` & `deepchecks-0.9.2/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/LICENSE` & `deepchecks-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/PKG-INFO` & `deepchecks-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deepchecks
-Version: 0.9.1
+Version: 0.9.2
 Summary: Package for validating your machine learning model and data
 Home-page: https://github.com/deepchecks/deepchecks
 Author: deepchecks
 Author-email: info@deepchecks.com
 License: UNKNOWN
-Download-URL: https://github.com/deepchecks/deepchecks/releases/download/0.9.1/deepchecks-0.9.1.tar.gz
+Download-URL: https://github.com/deepchecks/deepchecks/releases/download/0.9.2/deepchecks-0.9.2.tar.gz
 Project-URL: Documentation, https://docs.deepchecks.com
 Project-URL: Bug Reports, https://github.com/deepchecks/deepchecks
 Project-URL: Source, https://github.com/deepchecks/deepchecks
 Project-URL: Contribute!, https://github.com/deepchecks/deepchecks/blob/master/CONTRIBUTING.md
 Keywords: Software Development,Machine Learning
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `deepchecks-0.9.1/README.md` & `deepchecks-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/benchmarks/__init__.py` & `deepchecks-0.9.2/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/benchmarks/tabular_bench.py` & `deepchecks-0.9.2/benchmarks/tabular_bench.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/benchmarks/vision_bench.py` & `deepchecks-0.9.2/benchmarks/vision_bench.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/__init__.py` & `deepchecks-0.9.2/deepchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/analytics/__init__.py` & `deepchecks-0.9.2/deepchecks/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/analytics/anonymous_telemetry.py` & `deepchecks-0.9.2/deepchecks/analytics/anonymous_telemetry.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/checks.py` & `deepchecks-0.9.2/deepchecks/checks.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/__init__.py` & `deepchecks-0.9.2/deepchecks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/check_json.py` & `deepchecks-0.9.2/deepchecks/core/check_json.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/check_result.py` & `deepchecks-0.9.2/deepchecks/core/check_result.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/check_utils/__init__.py` & `deepchecks-0.9.2/deepchecks/core/check_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/check_utils/class_performance_utils.py` & `deepchecks-0.9.2/deepchecks/core/check_utils/class_performance_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/check_utils/feature_label_correlation_utils.py` & `deepchecks-0.9.2/deepchecks/core/check_utils/feature_label_correlation_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/check_utils/multivariate_drift_utils.py` & `deepchecks-0.9.2/deepchecks/core/check_utils/multivariate_drift_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from sklearn.ensemble import HistGradientBoostingClassifier
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import OrdinalEncoder
 
 from deepchecks.tabular import Dataset
 from deepchecks.tabular.utils.feature_importance import N_TOP_MESSAGE, calculate_feature_importance_or_none
+from deepchecks.tabular.utils.task_type import TaskType
 from deepchecks.utils.dataframes import floatify_dataframe
 from deepchecks.utils.distribution.drift import get_drift_plot_sidenote
 from deepchecks.utils.distribution.plot import drift_score_bar_traces, feature_distribution_traces
 from deepchecks.utils.distribution.rare_category_encoder import RareCategoryEncoder
 from deepchecks.utils.plot import DEFAULT_DATASET_NAMES
 from deepchecks.utils.strings import format_percent
 from deepchecks.utils.typing import Hashable
@@ -69,14 +70,17 @@
                                   cat_features=cat_features, label='belongs_to_test')
 
     # calculate feature importance of domain_classifier, containing the information which features separate
     # the dataset best.
     fi, importance_type = calculate_feature_importance_or_none(
         domain_classifier,
         domain_test_dataset,
+        model_classes=[0, 1],
+        observed_classes=[0, 1],
+        task_type=TaskType.BINARY,
         force_permutation=True,
         permutation_kwargs={'n_repeats': 10,
                             'random_state': random_state,
                             'timeout': 120,
                             'skip_messages': True}
     )
```

### Comparing `deepchecks-0.9.1/deepchecks/core/checks.py` & `deepchecks-0.9.2/deepchecks/core/checks.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/common.py` & `deepchecks-0.9.2/deepchecks/core/common.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/condition.py` & `deepchecks-0.9.2/deepchecks/core/condition.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/display.py` & `deepchecks-0.9.2/deepchecks/core/display.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/errors.py` & `deepchecks-0.9.2/deepchecks/core/errors.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/reduce_classes.py` & `deepchecks-0.9.2/deepchecks/core/reduce_classes.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/resources/__init__.py` & `deepchecks-0.9.2/deepchecks/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/resources/jupyterlab-plotly.js` & `deepchecks-0.9.2/deepchecks/core/resources/jupyterlab-plotly.js`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/resources/requirejs.min.js` & `deepchecks-0.9.2/deepchecks/core/resources/requirejs.min.js`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/resources/suite-template-full.html` & `deepchecks-0.9.2/deepchecks/core/resources/suite-template-full.html`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/resources/suite-template.html` & `deepchecks-0.9.2/deepchecks/core/resources/suite-template.html`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/resources/widgets-embed-amd.js` & `deepchecks-0.9.2/deepchecks/core/resources/widgets-embed-amd.js`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/resources/widgets-embed.js` & `deepchecks-0.9.2/deepchecks/core/resources/widgets-embed.js`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/__init__.py` & `deepchecks-0.9.2/deepchecks/core/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/abc.py` & `deepchecks-0.9.2/deepchecks/core/serialization/abc.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_failure/__init__.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_failure/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_failure/html.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_failure/html.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_failure/ipython.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_failure/ipython.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_failure/json.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_failure/json.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_failure/wandb.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_failure/wandb.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_failure/widget.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_failure/widget.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_result/__init__.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_result/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_result/html.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_result/html.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_result/ipython.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_result/ipython.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_result/json.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_result/json.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_result/wandb.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_result/wandb.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/check_result/widget.py` & `deepchecks-0.9.2/deepchecks/core/serialization/check_result/widget.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/common.py` & `deepchecks-0.9.2/deepchecks/core/serialization/common.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/dataframe/__init__.py` & `deepchecks-0.9.2/deepchecks/core/serialization/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/dataframe/html.py` & `deepchecks-0.9.2/deepchecks/core/serialization/dataframe/html.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/dataframe/widget.py` & `deepchecks-0.9.2/deepchecks/core/serialization/dataframe/widget.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/suite_result/__init__.py` & `deepchecks-0.9.2/deepchecks/core/serialization/suite_result/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/suite_result/html.py` & `deepchecks-0.9.2/deepchecks/core/serialization/suite_result/html.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/suite_result/ipython.py` & `deepchecks-0.9.2/deepchecks/core/serialization/suite_result/ipython.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/suite_result/json.py` & `deepchecks-0.9.2/deepchecks/core/serialization/suite_result/json.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/suite_result/wandb.py` & `deepchecks-0.9.2/deepchecks/core/serialization/suite_result/wandb.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/serialization/suite_result/widget.py` & `deepchecks-0.9.2/deepchecks/core/serialization/suite_result/widget.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/core/suite.py` & `deepchecks-0.9.2/deepchecks/core/suite.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/datasets/__init__.py` & `deepchecks-0.9.2/deepchecks/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/ppscore.py` & `deepchecks-0.9.2/deepchecks/ppscore.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/suites.py` & `deepchecks-0.9.2/deepchecks/suites.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/_shared_docs.py` & `deepchecks-0.9.2/deepchecks/tabular/_shared_docs.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     Array of the model prediction over the train dataset.
 y_pred_test: Optional[np.ndarray] , default: None
     Array of the model prediction over the test dataset.
 y_proba_train: Optional[np.ndarray] , default: None
     Array of the model prediction probabilities over the train dataset.
 y_proba_test: Optional[np.ndarray] , default: None
     Array of the model prediction probabilities over the test dataset.
+model_classes: Optional[List] , default: None
+    For classification: list of classes known to the model
 """.strip('\n')
 
 _shared_docstrings['feature_aggregation_method_argument'] = """
 argument for the reduce_output functionality, decides how to aggregate the drift scores for a
 collective score. The collective score value is between 0 and 1 for all methods other than l2_combination.
 Possible values are:
 'l2_weighted': L2 norm over the combination of drift scores and feature importance, minus the
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/base_checks.py` & `deepchecks-0.9.2/deepchecks/tabular/base_checks.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module for tabular base checks."""
 import abc
+import warnings
 from typing import List, Mapping, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from deepchecks.core.check_result import CheckFailure, CheckResult
 from deepchecks.core.checks import (BaseCheck, DatasetKind, ModelOnlyBaseCheck, SingleDatasetBaseCheck,
                                     TrainTestBaseCheck)
-from deepchecks.core.errors import DeepchecksNotSupportedError
+from deepchecks.core.errors import DeepchecksNotSupportedError, DeepchecksValueError
 from deepchecks.tabular import deprecation_warnings  # pylint: disable=unused-import # noqa: F401
 from deepchecks.tabular._shared_docs import docstrings
 from deepchecks.tabular.context import Context
 from deepchecks.tabular.dataset import Dataset
 from deepchecks.tabular.model_base import ModelComparisonContext
 from deepchecks.utils.typing import BasicModel
 
@@ -44,41 +45,63 @@
         self,
         dataset: Union[Dataset, pd.DataFrame],
         model: Optional[BasicModel] = None,
         feature_importance: Optional[pd.Series] = None,
         feature_importance_force_permutation: bool = False,
         feature_importance_timeout: int = 120,
         with_display: bool = True,
+        y_pred: Optional[np.ndarray] = None,
+        y_proba: Optional[np.ndarray] = None,
         y_pred_train: Optional[np.ndarray] = None,
         y_pred_test: Optional[np.ndarray] = None,
         y_proba_train: Optional[np.ndarray] = None,
         y_proba_test: Optional[np.ndarray] = None,
+        model_classes: Optional[List] = None
     ) -> CheckResult:
         """Run check.
 
         Parameters
         ----------
         dataset: Union[Dataset, pd.DataFrame]
             Dataset or DataFrame object, representing data an estimator was fitted on
         model: Optional[BasicModel], default: None
             A scikit-learn-compatible fitted estimator instance
         {additional_context_params:2*indent}
         """
         assert self.context_type is not None
+        if y_pred_train is not None:
+            warnings.warn('y_pred_train is deprecated, please use y_pred instead.', DeprecationWarning, stacklevel=2)
+        if (y_pred_train is not None) and (y_pred is not None):
+            raise DeepchecksValueError('Cannot accept both y_pred_train and y_pred, please pass the data only'
+                                       ' to y_pred.')
+        if y_proba_train is not None:
+            warnings.warn('y_proba_train is deprecated, please use y_proba instead.', DeprecationWarning, stacklevel=2)
+        if (y_pred_train is not None) and (y_pred is not None):
+            raise DeepchecksValueError('Cannot accept both y_proba_train and y_proba, please pass the data only'
+                                       ' to y_proba.')
+
+        if y_pred_test is not None:
+            warnings.warn('y_pred_test is deprecated and ignored.', DeprecationWarning, stacklevel=2)
+        if y_proba_test is not None:
+            warnings.warn('y_proba_test is deprecated and ignored.', DeprecationWarning, stacklevel=2)
+
+        y_pred_train = y_pred_train if y_pred_train is not None else y_pred
+        y_proba_train = y_proba_train if y_proba_train is not None else y_proba
+
         context = self.context_type(  # pylint: disable=not-callable
             train=dataset,
             model=model,
             feature_importance=feature_importance,
             feature_importance_force_permutation=feature_importance_force_permutation,
             feature_importance_timeout=feature_importance_timeout,
             with_display=with_display,
             y_pred_train=y_pred_train,
-            y_pred_test=y_pred_test,
             y_proba_train=y_proba_train,
             y_proba_test=y_proba_test,
+            model_classes=model_classes
         )
         result = self.run_logic(context, dataset_kind=DatasetKind.TRAIN)
         context.finalize_check_result(result, self, DatasetKind.TRAIN)
         return result
 
     @abc.abstractmethod
     def run_logic(self, context, dataset_kind) -> CheckResult:
@@ -104,14 +127,15 @@
         feature_importance_force_permutation: bool = False,
         feature_importance_timeout: int = 120,
         with_display: bool = True,
         y_pred_train: Optional[np.ndarray] = None,
         y_pred_test: Optional[np.ndarray] = None,
         y_proba_train: Optional[np.ndarray] = None,
         y_proba_test: Optional[np.ndarray] = None,
+        model_classes: Optional[List] = None
     ) -> CheckResult:
         """Run check.
 
         Parameters
         ----------
         train_dataset: Union[Dataset, pd.DataFrame]
             Dataset or DataFrame object, representing data an estimator was fitted on
@@ -130,14 +154,15 @@
             feature_importance_force_permutation=feature_importance_force_permutation,
             feature_importance_timeout=feature_importance_timeout,
             y_pred_train=y_pred_train,
             y_pred_test=y_pred_test,
             y_proba_train=y_proba_train,
             y_proba_test=y_proba_test,
             with_display=with_display,
+            model_classes=model_classes
         )
         result = self.run_logic(context)
         context.finalize_check_result(result, self)
         return result
 
     @abc.abstractmethod
     def run_logic(self, context) -> CheckResult:
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/class_imbalance.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/class_imbalance.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/columns_info.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/columns_info.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/conflicting_labels.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/conflicting_labels.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/data_duplicates.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/data_duplicates.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/feature_feature_correlation.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/feature_feature_correlation.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/feature_label_correlation.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/feature_label_correlation.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/identifier_label_correlation.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/identifier_label_correlation.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/is_single_value.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/is_single_value.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/mixed_data_types.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/mixed_data_types.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/mixed_nulls.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/mixed_nulls.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/outlier_sample_detection.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/outlier_sample_detection.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/percent_of_nulls.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/percent_of_nulls.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/special_chars.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/special_chars.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/string_length_out_of_bounds.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/string_length_out_of_bounds.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/data_integrity/string_mismatch.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/data_integrity/string_mismatch.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/boosting_overfit.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/boosting_overfit.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/calibration_score.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/calibration_score.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/confusion_matrix_report.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/confusion_matrix_report.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/model_inference_time.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/model_inference_time.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/model_info.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/model_info.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/multi_model_performance_report.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/multi_model_performance_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module containing multi model performance report check."""
-from typing import TYPE_CHECKING, Callable, Dict, cast
+import warnings
+from typing import TYPE_CHECKING, Callable, Dict, List, Mapping, Union, cast
 
 import pandas as pd
 import plotly.express as px
 
 from deepchecks.core import CheckResult
 from deepchecks.tabular import ModelComparisonCheck, ModelComparisonContext
 from deepchecks.tabular.utils.task_type import TaskType
@@ -26,29 +27,38 @@
 
 
 class MultiModelPerformanceReport(ModelComparisonCheck):
     """Summarize performance scores for multiple models on test datasets.
 
     Parameters
     ----------
+    scorers: Union[Mapping[str, Union[str, Callable]], List[str]], default: None
+        Scorers to override the default scorers, find more about the supported formats at
+        https://docs.deepchecks.com/stable/user-guide/general/metrics_guide.html
     alternative_scorers : Dict[str, Callable] , default: None
-        An optional dictionary of scorer name to scorer functions.
-        If none given, using default scorers
+        Deprecated, please use scorers instead.
     n_samples : int , default: 1_000_000
         number of samples to use for this check.
     random_state : int, default: 42
         random seed for all check internals.
     """
 
-    def __init__(self, alternative_scorers: Dict[str, Callable] = None,
+    def __init__(self,
+                 scorers: Union[Mapping[str, Union[str, Callable]], List[str]] = None,
+                 alternative_scorers: Dict[str, Callable] = None,
                  n_samples: int = 1_000_000,
                  random_state: int = 42,
                  **kwargs):
         super().__init__(**kwargs)
-        self.alternative_scorers = alternative_scorers
+        if alternative_scorers is not None:
+            warnings.warn(f'{self.__class__.__name__}: alternative_scorers is deprecated. Please use scorers instead.',
+                          DeprecationWarning)
+            self.scorers = alternative_scorers
+        else:
+            self.alternative_scorers = scorers
         self.n_samples = n_samples
         self.random_state = random_state
 
     def run_logic(self, multi_context: ModelComparisonContext):
         """Run check logic."""
         first_context = multi_context[0]
         scorers = first_context.get_scorers(self.alternative_scorers, use_avg_defaults=False)
@@ -62,15 +72,15 @@
                 model = context.model
                 label = cast(pd.Series, test.label_col)
                 n_samples = label.groupby(label).count()
                 results.extend(
                     [model_name, class_score, scorer.name, class_name, n_samples[class_name]]
                     for scorer in scorers
                     # scorer returns numpy array of results with item per class
-                    for class_score, class_name in zip(scorer(model, test), context.classes)
+                    for class_score, class_name in zip(scorer(model, test), context.model_classes)
                 )
 
             results_df = pd.DataFrame(results, columns=['Model', 'Value', 'Metric', 'Class', 'Number of samples'])
 
         else:
             plot_x_axis = 'Model'
             results = [
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/regression_systematic_error.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/regression_systematic_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """The RegressionSystematicError check module."""
+import warnings
+
 import plotly.graph_objects as go
 from sklearn.metrics import mean_squared_error
 
 from deepchecks.core import CheckResult, ConditionResult
 from deepchecks.core.condition import ConditionCategory
 from deepchecks.tabular import Context, SingleDatasetCheck
 from deepchecks.utils.strings import format_number
@@ -33,14 +35,16 @@
 
     def __init__(
         self,
         n_samples: int = 1_000_000,
         random_state: int = 42,
         **kwargs
     ):
+        warnings.warn('RegressionSystematicError check is deprecated and will be removed in future version,'
+                      ' please use RegressionErrorDistribution check instead.', DeprecationWarning, stacklevel=2)
         super().__init__(**kwargs)
         self.n_samples = n_samples
         self.random_state = random_state
 
     def run_logic(self, context: Context, dataset_kind) -> CheckResult:
         """Run check.
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/roc_report.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/roc_report.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/segment_performance.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/segment_performance.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/simple_model_comparison.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/simple_model_comparison.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module containing simple comparison check."""
+import warnings
 from collections import defaultdict
-from typing import TYPE_CHECKING, Callable, Dict, Hashable, List
+from typing import TYPE_CHECKING, Callable, Dict, Hashable, List, Mapping, Union
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 from sklearn.dummy import DummyClassifier, DummyRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
@@ -53,17 +54,19 @@
         'most_frequent', 'tree'].
 
         * `stratified`: randomly draw a label based on the train set label distribution. (Previously 'random')
         * `uniform`: in regression samples predictions uniformly at random from the y ranges. in classification draws
            predictions uniformly at random from the list of values in y.
         * `most_frequent`: in regression is mean value, in classification the most common value. (Previously 'constant')
         * `tree`: runs a simple decision tree.
+    scorers: Union[Mapping[str, Union[str, Callable]], List[str]], default: None
+        Scorers to override the default scorers, find more about the supported formats at
+        https://docs.deepchecks.com/stable/user-guide/general/metrics_guide.html
     alternative_scorers : Dict[str, Callable], default: None
-        An optional dictionary of scorer title to scorer functions/names. If none given, using default scorers.
-        For description about scorers see Notes below.
+        Deprecated, please use scorers instead.
     max_gain : float , default: 50
         the maximum value for the gain value, limits from both sides [-max_gain, max_gain]
     max_depth : int , default: 3
         the max depth of the tree (used only if simple model type is tree).
     n_samples : int , default: 1_000_000
         number of samples to use for this check.
     random_state : int , default: 42
@@ -103,23 +106,29 @@
         # value to maximize.
         my_mse_scorer = make_scorer(my_mse, greater_is_better=False)
     """
 
     def __init__(
         self,
         strategy: str = 'most_frequent',
+        scorers: Union[Mapping[str, Union[str, Callable]], List[str]] = None,
         alternative_scorers: Dict[str, Callable] = None,
         max_gain: float = 50,
         max_depth: int = 3,
         n_samples: int = 1_000_000,
         random_state: int = 42,
         **kwargs
     ):
         super().__init__(**kwargs)
-        self.alternative_scorers = alternative_scorers
+        if alternative_scorers is not None:
+            warnings.warn(f'{self.__class__.__name__}: alternative_scorers is deprecated. Please use scorers instead.',
+                          DeprecationWarning)
+            self.alternative_scorers = alternative_scorers
+        else:
+            self.alternative_scorers = scorers
         self.max_gain = max_gain
         self.max_depth = max_depth
         self.n_samples = n_samples
         self.random_state = random_state
         self.strategy = strategy
 
         if self.strategy not in _allowed_strategies:
@@ -160,33 +169,35 @@
         models = [
             (f'{type(model).__name__} model', 'Origin', model),
             (f'Simple model - {self.strategy}', 'Simple', simple_model)
         ]
 
         # Multiclass have different return type from the scorer, list of score per class instead of single score
         if task_type in [TaskType.MULTICLASS, TaskType.BINARY]:
-            n_samples = test_label.groupby(test_label).count()
-            classes = [clazz for clazz in test_dataset.classes_in_label_col
-                       if clazz in train_dataset.classes_in_label_col]
+            class_counts = test_label.groupby(test_label).count()
 
             display_array = []
             # Dict in format { Scorer : Dict { Class : Dict { Origin/Simple : score } } }
             results_dict = {}
             for scorer in scorers:
                 model_dict = defaultdict(dict)
                 for model_name, model_type, model_instance in models:
-                    for class_score, class_value in zip(scorer(model_instance, test_dataset), classes):
+                    for class_value, class_score in scorer(model_instance, test_dataset).items():
+                        # New labels which do not exists on the model gets nan as score, skips them.
+                        # Also skips classes which are not in the test labels
+                        if np.isnan(class_score) or class_value not in class_counts:
+                            continue
                         model_dict[class_value][model_type] = class_score
                         if context.with_display:
                             display_array.append([model_name,
                                                   model_type,
                                                   class_score,
                                                   scorer.name,
                                                   class_value,
-                                                  n_samples[class_value]
+                                                  class_counts[class_value]
                                                   ])
                 results_dict[scorer.name] = model_dict
 
             if display_array:
                 display_df = pd.DataFrame(
                     display_array,
                     columns=['Model', 'Type', 'Value', 'Metric', 'Class', 'Number of samples']
@@ -208,16 +219,14 @@
                     .for_each_annotation(lambda a: a.update(text=a.text.split('=')[-1]))
                     .for_each_yaxis(lambda yaxis: yaxis.update(showticklabels=True))
                 )
             else:
                 fig = None
 
         else:
-            classes = None
-
             display_array = []
             # Dict in format { Scorer : Dict { Origin/Simple : score } }
             results_dict = {}
             for scorer in scorers:
                 model_dict = defaultdict(dict)
                 for model_name, model_type, model_instance in models:
                     score = scorer(model_instance, test_dataset)
@@ -258,15 +267,14 @@
 
         # For each scorer calculate perfect score in order to calculate later the ratio in conditions
         scorers_perfect = {scorer.name: scorer.score_perfect(test_dataset) for scorer in scorers}
 
         return CheckResult({'scores': results_dict,
                             'type': task_type,
                             'scorers_perfect': scorers_perfect,
-                            'classes': classes
                             }, display=fig)
 
     def config(self, include_version: bool = True) -> 'CheckConfig':
         """Return check instance config."""
         if self.alternative_scorers is not None:
             for k, v in self.alternative_scorers.items():
                 if callable(v):
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/single_dataset_performance.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/single_dataset_performance.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module containing the single dataset performance check."""
 from numbers import Number
-from typing import TYPE_CHECKING, Callable, Dict, List, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Callable, Dict, List, Mapping, TypeVar, Union, cast
 
 import pandas as pd
 
 from deepchecks.core import CheckResult, ConditionCategory, ConditionResult
 from deepchecks.core.errors import DeepchecksValueError
 from deepchecks.core.reduce_classes import ReduceMetricClassMixin
 from deepchecks.tabular import Context
@@ -33,25 +33,25 @@
 
 
 class SingleDatasetPerformance(SingleDatasetCheck, ReduceMetricClassMixin):
     """Summarize given model performance on the train and test datasets based on selected scorers.
 
     Parameters
     ----------
-    scorers : Union[List[str], Dict[str, Union[str, Callable]]], default: None
-        List of scorers to use. If None, use default scorers.
-        Scorers can be supplied as a list of scorer names or as a dictionary of names and functions.
+    scorers: Union[Mapping[str, Union[str, Callable]], List[str]], default: None
+        Scorers to override the default scorers, find more about the supported formats at
+        https://docs.deepchecks.com/stable/user-guide/general/metrics_guide.html
     n_samples : int , default: 1_000_000
         number of samples to use for this check.
     random_state : int, default: 42
         random seed for all check internals.
     """
 
     def __init__(self,
-                 scorers: Union[List[str], Dict[str, Union[str, Callable]]] = None,
+                 scorers: Union[Mapping[str, Union[str, Callable]], List[str]] = None,
                  n_samples: int = 1_000_000,
                  random_state: int = 42,
                  **kwargs):
         super().__init__(**kwargs)
         self.scorers = scorers
         self.n_samples = n_samples
         self.random_state = random_state
@@ -75,15 +75,15 @@
             for scorer in scorers:
                 scorer_value = scorer(model, dataset)
                 if isinstance(scorer_value, Number):
                     results.append([pd.NA, scorer.name, scorer_value])
                 else:
                     results.extend(
                         [[class_name, scorer.name, class_score]
-                         for class_score, class_name in zip(scorer_value, context.classes)])
+                         for class_name, class_score in scorer_value.items()])
             results_df = pd.DataFrame(results, columns=['Class', 'Metric', 'Value'])
 
             if context.with_display:
                 label = cast(pd.Series, dataset.label_col)
                 n_samples = label.groupby(label).count()
                 display_df = results_df.copy()
                 display_df['Number of samples'] = display_df['Class'].apply(n_samples.get)
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/train_test_performance.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/train_test_performance.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module containing the train test performance check."""
 from numbers import Number
-from typing import Callable, Dict, List, TypeVar, Union, cast
+from typing import Callable, Dict, List, Mapping, TypeVar, Union, cast
 
 import pandas as pd
 import plotly.express as px
 
 from deepchecks.core import CheckResult
 from deepchecks.core.check_utils.class_performance_utils import (
     get_condition_class_performance_imbalance_ratio_less_than, get_condition_test_performance_greater_than,
@@ -34,17 +34,17 @@
 
 
 class TrainTestPerformance(TrainTestCheck, ReduceMixin):
     """Summarize given model performance on the train and test datasets based on selected scorers.
 
     Parameters
     ----------
-    scorers : Union[List[str], Dict[str, Union[str, Callable]]], default: None
-        List of scorers to use. If None, use default scorers.
-        Scorers can be supplied as a list of scorer names or as a dictionary of names and functions.
+    scorers: Union[Mapping[str, Union[str, Callable]], List[str]], default: None
+        Scorers to override the default scorers, find more about the supported formats at
+        https://docs.deepchecks.com/stable/user-guide/general/metrics_guide.html
     reduce: Union[Callable, str], default: 'mean'
         An optional argument only used for the reduce_output function when using
         per-class scorers.
     n_samples : int , default: 1_000_000
         number of samples to use for this check.
     random_state : int, default: 42
         random seed for all check internals.
@@ -81,15 +81,15 @@
 
         # Mark greater_is_better=False, since scorers always suppose to return
         # value to maximize.
         my_mse_scorer = make_scorer(my_mse, greater_is_better=False)
     """
 
     def __init__(self,
-                 scorers: Union[List[str], Dict[str, Union[str, Callable]]] = None,
+                 scorers: Union[Mapping[str, Union[str, Callable]], List[str]] = None,
                  reduce: Union[Callable, str] = 'mean',
                  n_samples: int = 1_000_000,
                  random_state: int = 42,
                  **kwargs):
         super().__init__(**kwargs)
         self.scorers = scorers
         self.reduce = reduce
@@ -103,23 +103,23 @@
         model = context.model
         scorers = context.get_scorers(self.scorers, use_avg_defaults=False)
         datasets = {'Train': train_dataset, 'Test': test_dataset}
 
         results = []
         for dataset_name, dataset in datasets.items():
             label = cast(pd.Series, dataset.label_col)
-            n_samples = label.groupby(label).count()
+            n_samples_per_class = label.groupby(label).count()
             for scorer in scorers:
                 scorer_value = scorer(model, dataset)
                 if isinstance(scorer_value, Number):
-                    results.append([dataset_name, None, scorer.name, scorer_value, len(label)])
+                    results.append([dataset_name, pd.NA, scorer.name, scorer_value, len(label)])
                 else:
                     results.extend(
-                        [[dataset_name, class_name, scorer.name, class_score, n_samples[class_name]]
-                            for class_score, class_name in zip(scorer_value, dataset.classes_in_label_col)])
+                        [[dataset_name, class_name, scorer.name, class_score, n_samples_per_class.get(class_name, 0)]
+                            for class_name, class_score in scorer_value.items()])
 
         results_df = pd.DataFrame(results, columns=['Dataset', 'Class', 'Metric', 'Value', 'Number of samples'])
 
         if context.with_display:
             results_df_for_display = results_df.copy()
             results_df_for_display['Dataset']\
                 .replace({DEFAULT_DATASET_NAMES[0]: train_dataset.name, DEFAULT_DATASET_NAMES[1]: test_dataset.name},
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/train_test_prediction_drift.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/train_test_prediction_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/unused_features.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/unused_features.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/model_evaluation/weak_segments_performance.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/model_evaluation/weak_segments_performance.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,30 +115,30 @@
         if context.task_type in [TaskType.MULTICLASS, TaskType.BINARY]:
             if not hasattr(context.model, 'predict_proba'):
                 raise DeepchecksNotSupportedError('Predicted probabilities not supplied. The weak segment checks relies'
                                                   ' on log loss error that requires predicted probabilities, rather'
                                                   ' than only predicted classes.')
             y_proba = context.model.predict_proba(dataset.features_columns)
             # If proba shape does not match label, raise error
-            if y_proba.shape[1] != len(context.classes):
+            if y_proba.shape[1] != len(context.model_classes):
                 raise DeepchecksValueError(
                     f'Predicted probabilities shape {y_proba.shape} does not match the number of classes found in'
-                    f' the labels {context.classes}.')
+                    f' the labels {context.model_classes}.')
         else:
             y_proba = None
 
         if self.loss_per_sample is not None:
             loss_per_sample = self.loss_per_sample[list(dataset.data.index)]
         else:
             loss_per_sample = calculate_per_sample_loss(context.model, context.task_type, dataset,
-                                                        context.classes)
+                                                        context.model_classes)
         dataset = dataset.select(self.columns, self.ignore_columns, keep_label=True)
         if len(dataset.features) < 2:
             raise DeepchecksNotSupportedError('Check requires data to have at least two features in order to run.')
-        encoded_dataset = self._target_encode_categorical_features_fill_na(dataset, context.classes)
+        encoded_dataset = self._target_encode_categorical_features_fill_na(dataset, context.observed_classes)
         dummy_model = _DummyModel(test=encoded_dataset, y_pred_test=predictions, y_proba_test=y_proba,
                                   validate_data_on_predict=False)
 
         relevant_features = encoded_dataset.cat_features + encoded_dataset.numerical_features
         if context.feature_importance is not None:
             feature_rank = context.feature_importance.sort_values(ascending=False).keys()
             feature_rank = np.asarray([col for col in feature_rank if col in relevant_features], dtype='object')
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/category_mismatch_train_test.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/category_mismatch_train_test.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/datasets_size_comparison.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/datasets_size_comparison.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_duplicates.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_duplicates.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_overlap.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/date_train_test_leakage_overlap.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/feature_label_correlation_change.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/feature_label_correlation_change.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/index_leakage.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/index_leakage.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/multivariate_drift.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/multivariate_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/new_label_train_test.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/new_label_train_test.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/string_mismatch_comparison.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/string_mismatch_comparison.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/train_test_feature_drift.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/train_test_feature_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/train_test_label_drift.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/train_test_label_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/train_test_samples_mix.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/train_test_samples_mix.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/checks/train_test_validation/whole_dataset_drift.py` & `deepchecks-0.9.2/deepchecks/tabular/checks/train_test_validation/whole_dataset_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/context.py` & `deepchecks-0.9.2/deepchecks/tabular/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # ----------------------------------------------------------------------------
 #
 """Module for base tabular context."""
 import typing as t
 
 import numpy as np
 import pandas as pd
-from pandas._libs.lib import infer_dtype
 
 from deepchecks.core import CheckFailure, CheckResult, DatasetKind
 from deepchecks.core.errors import (DatasetValidationError, DeepchecksNotSupportedError, DeepchecksValueError,
                                     ModelValidationError)
 from deepchecks.tabular._shared_docs import docstrings
 from deepchecks.tabular.dataset import Dataset
 from deepchecks.tabular.metric_utils import DeepcheckScorer, get_default_scorers, init_validate_scorers
 from deepchecks.tabular.utils.feature_importance import calculate_feature_importance_or_none
-from deepchecks.tabular.utils.task_inference import get_possible_classes
+from deepchecks.tabular.utils.task_inference import infer_task_type_and_classes
 from deepchecks.tabular.utils.task_type import TaskType
 from deepchecks.tabular.utils.validation import (ensure_predictions_proba, ensure_predictions_shape,
                                                  model_type_validation, validate_model)
+from deepchecks.utils.docref import doclink
 from deepchecks.utils.logger import get_logger
 from deepchecks.utils.plot import DEFAULT_DATASET_NAMES
 from deepchecks.utils.typing import BasicModel
 
 __all__ = [
     'Context', '_DummyModel'
 ]
@@ -166,14 +166,15 @@
             feature_importance_force_permutation: bool = False,
             feature_importance_timeout: int = 120,
             with_display: bool = True,
             y_pred_train: t.Optional[np.ndarray] = None,
             y_pred_test: t.Optional[np.ndarray] = None,
             y_proba_train: t.Optional[np.ndarray] = None,
             y_proba_test: t.Optional[np.ndarray] = None,
+            model_classes: t.Optional[t.List] = None
     ):
         # Validations
         if train is None and test is None and model is None:
             raise DeepchecksValueError('At least one dataset (or model) must be passed to the method!')
         if train is not None:
             train = Dataset.cast_to_dataset(train)
             if train.name is None:
@@ -209,16 +210,24 @@
                                 y_pred_train=y_pred_train, y_pred_test=y_pred_test,
                                 y_proba_test=y_proba_test, y_proba_train=y_proba_train)
         if model is not None:
             # Here validate only type of model, later validating it can predict on the data if needed
             model_type_validation(model)
         if feature_importance is not None and not isinstance(feature_importance, pd.Series):
             raise DeepchecksValueError('feature_importance must be a pandas Series')
+        if model_classes and len(model_classes) == 0:
+            raise DeepchecksValueError('Received empty model_classes')
+        if model_classes and sorted(model_classes) != model_classes:
+            supported_models_link = doclink(
+                'supported-prediction-format',
+                template='For more information please refer to the Supported Models guide {link}')
+            raise DeepchecksValueError(f'Received unsorted model_classes. {supported_models_link}')
 
-        self._classes = None
+        self._task_type, self._observed_classes, self._model_classes = infer_task_type_and_classes(
+            model, train, test, model_classes)
         self._train = train
         self._test = test
         self._model = model
         self._feature_importance_force_permutation = feature_importance_force_permutation
         self._feature_importance = feature_importance
         self._feature_importance_timeout = feature_importance_timeout
         self._importance_type = None
@@ -255,59 +264,47 @@
         if not self._validated_model:
             if self._train:
                 validate_model(self._train, self._model)
             self._validated_model = True
         return self._model
 
     @property
-    def classes(self) -> t.List:
+    def model_classes(self) -> t.List:
         """Return ordered list of possible label classes for classification tasks or None for regression."""
-        if self._classes is None:
-            if self._train is not None and self._train.has_label() and self._train.label_type != TaskType.REGRESSION:
-                self._classes = get_possible_classes(self._model, self._train, self._test,
-                                                     self._train.label_type is not None)
-            else:
-                self._classes = None
+        if self._model_classes is None and self.task_type != TaskType.REGRESSION:
+            # If in infer_task_type we didn't find classes on model, or user didn't pass any, then using the observed
+            self._model_classes = self._observed_classes
+            get_logger().warning('Could not find model\'s classes, using the observed classes')
+        return self._model_classes
 
-            if self._classes is not None and infer_dtype(self._train.label_col) == 'integer' and \
-                    self._train.label_type is None:
-                get_logger().warning(
-                    'Due to the small number of unique labels task type was inferred as multiclass in spite of '
-                    'the label column is of type integer. '
-                    'Initialize your Dataset with either label_type=\"multiclass\" or '
-                    'label_type=\"regression\" to resolve this warning.')
-        return self._classes
+    @property
+    def observed_classes(self) -> t.List:
+        """Return the observed classes in both train and test. None for regression."""
+        return self._observed_classes
 
     @property
     def model_name(self):
         """Return model name."""
         return type(self.model).__name__
 
     @property
     def task_type(self) -> TaskType:
         """Return task type based on calculated classes argument."""
-        if self.classes is None:
-            return TaskType.REGRESSION
-        elif len(self.classes) == 2:
-            return TaskType.BINARY
-        elif len(self.classes) > 2:
-            return TaskType.MULTICLASS
-        else:
-            raise DatasetValidationError('Found only one class in label column, pass the full list of possible '
-                                         'label classes via the label_classes argument in the Dataset initialization.')
+        return self._task_type
 
     @property
     def feature_importance(self) -> t.Optional[pd.Series]:
         """Return feature importance, or None if not possible."""
         if not self._calculated_importance:
             if self._model and (self._train or self._test):
                 permutation_kwargs = {'timeout': self._feature_importance_timeout}
                 dataset = self.test if self.have_test() else self.train
                 importance, importance_type = calculate_feature_importance_or_none(
-                    self._model, dataset, self._feature_importance_force_permutation, permutation_kwargs
+                    self._model, dataset, self.model_classes, self._observed_classes, self.task_type,
+                    self._feature_importance_force_permutation, permutation_kwargs
                 )
                 self._feature_importance = importance
                 self._importance_type = importance_type
             else:
                 self._feature_importance = None
             self._calculated_importance = True
 
@@ -355,15 +352,15 @@
             an averaged metric, or default scorers that return a metric per class.
         Returns
         -------
         List[DeepcheckScorer]
             A list of initialized & validated scorers.
         """
         scorers = scorers or get_default_scorers(self.task_type, use_avg_defaults)
-        return init_validate_scorers(scorers, self.model, self.train, self.classes)
+        return init_validate_scorers(scorers, self.model, self.train, self.model_classes, self._observed_classes)
 
     def get_single_scorer(self,
                           scorers: t.Mapping[str, t.Union[str, t.Callable]] = None,
                           use_avg_defaults=True) -> DeepcheckScorer:
         """Return initialized & validated single scorer in a given priority.
 
         If receive `scorers` use them,
@@ -384,15 +381,16 @@
         List[DeepcheckScorer]
             An initialized & validated scorer.
         """
         scorers = scorers or get_default_scorers(self.task_type, use_avg_defaults)
         # The single scorer is the first one in the dict
         scorer_name = next(iter(scorers))
         single_scorer_dict = {scorer_name: scorers[scorer_name]}
-        return init_validate_scorers(single_scorer_dict, self.model, self.train, self.classes)[0]
+        return init_validate_scorers(single_scorer_dict, self.model, self.train, self.model_classes,
+                                     self._observed_classes)[0]
 
     def get_data_by_kind(self, kind: DatasetKind) -> Dataset:
         """Return the relevant Dataset by given kind."""
         if kind == DatasetKind.TRAIN:
             return self.train
         elif kind == DatasetKind.TEST:
             return self.test
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/dataset.py` & `deepchecks-0.9.2/deepchecks/tabular/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 from sklearn.model_selection import train_test_split
 from typing_extensions import Literal as L
 
 from deepchecks.core.errors import DatasetValidationError, DeepchecksNotSupportedError, DeepchecksValueError
 from deepchecks.tabular.utils.feature_inference import (infer_categorical_features, infer_numerical_features,
                                                         is_categorical)
 from deepchecks.tabular.utils.task_type import TaskType
-from deepchecks.utils.array_math import is_sequence
 from deepchecks.utils.dataframes import select_from_dataframe
-from deepchecks.utils.docref import doclink
 from deepchecks.utils.logger import get_logger
 from deepchecks.utils.strings import get_docs_link
 from deepchecks.utils.typing import Hashable
 
 __all__ = ['Dataset']
 
 TDataset = t.TypeVar('TDataset', bound='Dataset')
@@ -89,17 +87,14 @@
         categorical feature.
     max_categories : int , default: None
         The maximum number of categories in a column in order for it to be inferred as a categorical
         feature. if None, uses is_categorical default inference mechanism.
     label_type : str , default: None
         Used to determine the task type. If None, inferred when running a check based on label column and model.
         Possible values are: 'multiclass', 'binary' and 'regression'.
-    label_classes: t.List, default: None
-        Relevant only for classification tasks. The list of all possible classes in the order they appear at the
-        models' probabilities per class vector (in alphanumeric order).
     """
 
     _features: t.List[Hashable]
     _label_name: t.Optional[Hashable]
     _index_name: t.Optional[Hashable]
     _set_index_from_dataframe_index: t.Optional[bool]
     _datetime_name: t.Optional[Hashable]
@@ -107,15 +102,14 @@
     _convert_datetime: t.Optional[bool]
     _datetime_column: t.Optional[pd.Series]
     _cat_features: t.List[Hashable]
     _data: pd.DataFrame
     _max_categorical_ratio: float
     _max_categories: int
     _label_type: t.Optional[TaskType]
-    _label_classes: t.List
 
     def __init__(
             self,
             df: t.Any,
             label: t.Union[Hashable, pd.Series, pd.DataFrame, np.ndarray] = None,
             features: t.Optional[t.Sequence[Hashable]] = None,
             cat_features: t.Optional[t.Sequence[Hashable]] = None,
@@ -124,16 +118,16 @@
             datetime_name: t.Optional[Hashable] = None,
             set_datetime_from_dataframe_index: bool = False,
             convert_datetime: bool = True,
             datetime_args: t.Optional[t.Dict] = None,
             max_categorical_ratio: float = 0.01,
             max_categories: int = None,
             label_type: str = None,
-            label_classes: t.List = None,
             dataset_name: t.Optional[str] = None,
+            label_classes=None
     ):
 
         if len(df) == 0:
             raise DeepchecksValueError('Can\'t create a Dataset object with an empty dataframe')
         self._data = pd.DataFrame(df).copy()
 
         # Checking for duplicate columns
@@ -288,25 +282,16 @@
         elif label_type is not None:
             raise DeepchecksValueError(f'allowed value for label type are {[task.value for task in TaskType]},'
                                        f' received {label_type}.')
         else:
             self._label_type = None
 
         if label_classes is not None:
-            if not isinstance(label_classes, t.List) or any(is_sequence(x) for x in label_classes) or \
-                    len(set(label_classes)) != len(label_classes):
-                raise DeepchecksValueError('label_classes must be a flat list of unique values.')
-            if label is not None and not set(self.label_col).issubset(set(label_classes)):
-                raise DeepchecksValueError('label_classes does not contain all labels found in label column.')
-            if label_classes != sorted(label_classes):
-                reference = doclink('supported-prediction-format', template='For additional details see {link}')
-                raise DeepchecksValueError('label_classes order must correspond to the required order of the model\'s '
-                                           'probabilities per class (alphanumeric order). For additional details see'
-                                           f'{reference}')
-        self._label_classes = label_classes
+            warnings.warn('label_classes parameter is deprecated, use model_classes parameter on a check run function '
+                          'instead.', DeprecationWarning, stacklevel=2)
 
         unassigned_cols = [col for col in self._features if col not in self._cat_features]
         self._numerical_features = infer_numerical_features(self._data[unassigned_cols])
 
     @classmethod
     def from_numpy(
             cls: t.Type[TDataset],
@@ -442,15 +427,15 @@
 
         cls = type(self)
 
         return cls(new_data, features=features, cat_features=cat_features, label=label_name,
                    index_name=index, set_index_from_dataframe_index=self._set_index_from_dataframe_index,
                    datetime_name=date, set_datetime_from_dataframe_index=self._set_datetime_from_dataframe_index,
                    convert_datetime=self._convert_datetime, max_categorical_ratio=self._max_categorical_ratio,
-                   max_categories=self._max_categories, label_type=label_type, label_classes=self._label_classes,
+                   max_categories=self._max_categories, label_type=label_type,
                    dataset_name=self.name)
 
     def sample(self: TDataset, n_samples: t.Optional[int], replace: bool = False, random_state: t.Optional[int] = None,
                drop_na_label: bool = False) -> TDataset:
         """Create a copy of the dataset object, with the internal dataframe being a sample of the original dataframe.
 
         Parameters
@@ -551,15 +536,15 @@
         if is_categorical(label_col, max_categorical_ratio=0.05):
             if label_col.nunique(dropna=True) > 2:
                 if infer_dtype(label_col) == 'integer' \
                         and label_col.nunique() >= 5:
                     get_logger().warning(
                         'Integer label has many unique values. In this case, deepchecks automatically '
                         'infers label to be multiclass. If your label is a regression label and not multiclass, '
-                        'please use "label_type=\'regression_label\'" when initializing your Dataset.'
+                        'please use "label_type=\'regression\'" when initializing your Dataset.'
                     )
                 return TaskType.MULTICLASS
             else:
                 return TaskType.BINARY
         else:
             return TaskType.REGRESSION
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/classification/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/classification/adult.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/classification/adult.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/classification/breast_cancer.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/classification/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/classification/iris.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/classification/iris.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/classification/lending_club.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/classification/lending_club.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/classification/phishing.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/classification/phishing.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/regression/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/regression/airbnb.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/regression/airbnb.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/regression/avocado.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/regression/avocado.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/datasets/regression/wine_quality.py` & `deepchecks-0.9.2/deepchecks/tabular/datasets/regression/wine_quality.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/deprecation_warnings.py` & `deepchecks-0.9.2/deepchecks/vision/deprecation_warnings.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 # ----------------------------------------------------------------------------
 #
 """This file changes default 'ignore' action of DeprecationWarnings for specific deprecation messages."""
 import warnings
 
 warnings.filterwarnings(
     action='once',
-    message=r'The SegmentPerformance check is deprecated.*',
+    message=r'.*alternative_metrics is deprecated.*',
     category=DeprecationWarning,
     module=r'deepchecks.*'
 )
 
 warnings.filterwarnings(
     action='once',
-    message=r'The WholeDatasetDrift check is deprecated.*',
+    message=r'train_predictions is deprecated.*',
     category=DeprecationWarning,
     module=r'deepchecks.*'
 )
 
 warnings.filterwarnings(
     action='once',
-    message=r'.* label type is deprecated.*',
+    message=r'test_predictions is deprecated and ignored.*',
     category=DeprecationWarning,
     module=r'deepchecks.*'
 )
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/feature_importance.py` & `deepchecks-0.9.2/deepchecks/tabular/feature_importance.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from deepchecks.core.errors import DeepchecksValueError
 from deepchecks.tabular import Dataset
 from deepchecks.tabular.metric_utils import DeepcheckScorer
 from deepchecks.tabular.utils.feature_importance import _calculate_feature_importance
 
 __all__ = ['calculate_feature_importance']
 
+from deepchecks.tabular.utils.task_inference import infer_task_type_and_classes
+
 
 def calculate_feature_importance(
         model: t.Any,
         dataset: Dataset,
         n_repeats: int = 30,
         mask_high_variance_features: bool = False,
         n_samples: int = 10_000,
@@ -86,10 +88,17 @@
     }
 
     if isinstance(dataset, pd.DataFrame):
         raise DeepchecksValueError('Cannot calculate permutation feature importance on a pandas Dataframe. '
                                    'In order to force permutation feature importance, please use the Dataset'
                                    ' object.')
 
-    fi, _ = _calculate_feature_importance(model=model, dataset=dataset, force_permutation=True,
+    task_type, observed_classes, model_classes = infer_task_type_and_classes(model, dataset)
+    model_classes = model_classes if model_classes is not None else observed_classes
+    fi, _ = _calculate_feature_importance(model=model,
+                                          dataset=dataset,
+                                          model_classes=model_classes,
+                                          observed_classes=observed_classes,
+                                          task_type=task_type,
+                                          force_permutation=True,
                                           permutation_kwargs=permutation_kwargs)
     return fi
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/integrations/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/integrations/h2o.py` & `deepchecks-0.9.2/deepchecks/tabular/integrations/h2o.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/metric_utils/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/metric_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/metric_utils/scorers.py` & `deepchecks-0.9.2/deepchecks/tabular/metric_utils/scorers.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 """Utils module containing utilities for checks working with scorers."""
 import typing as t
 import warnings
 from numbers import Number
 
 import numpy as np
 import pandas as pd
-from sklearn.base import BaseEstimator, ClassifierMixin
+from sklearn.base import ClassifierMixin
 from sklearn.metrics import get_scorer, make_scorer, mean_absolute_error, mean_squared_error
 from sklearn.metrics._scorer import _BaseScorer, _ProbaScorer
+from sklearn.preprocessing import LabelBinarizer
 
 try:
     from deepchecks_metrics import f1_score, jaccard_score, precision_score, recall_score  # noqa: F401
 except ImportError:
     from sklearn.metrics import \
         f1_score, recall_score, precision_score, jaccard_score  # noqa: F401  pylint: disable=ungrouped-imports
 
@@ -32,16 +33,15 @@
                                                                                roc_auc_per_class,
                                                                                true_negative_rate_metric)
 from deepchecks.tabular.utils.task_type import TaskType
 from deepchecks.utils.docref import doclink
 from deepchecks.utils.logger import get_logger
 from deepchecks.utils.metrics import get_scorer_name
 from deepchecks.utils.simple_models import PerfectModel
-from deepchecks.utils.strings import is_string_column
-from deepchecks.utils.typing import BasicModel, ClassificationModel
+from deepchecks.utils.typing import BasicModel
 
 __all__ = [
     'DEFAULT_SCORERS_DICT',
     'DEFAULT_REGRESSION_SCORERS',
     'DEFAULT_BINARY_SCORERS',
     'DEFAULT_MULTICLASS_SCORERS',
     'MULTICLASS_SCORERS_NON_AVERAGE',
@@ -159,33 +159,40 @@
 }
 
 _str_to_scorer_dict = {**regression_scorers_higher_is_better_dict,
                        **regression_scorers_lower_is_better_dict,
                        **multiclass_scorers_dict,
                        **binary_scorers_dict}
 
+SUPPORTED_MODELS_DOCLINK = doclink('supported-prediction-format',
+                                   template='For more information please refer to the Supported Models guide {link}')
+
 
 class DeepcheckScorer:
     """Encapsulate scorer function with extra methods.
 
     Scorer functions are functions used to compute various performance metrics, using the model and data as inputs,
     rather than the labels and predictions. Scorers are callables with the signature scorer(model, features, y_true).
     Additional data on scorer functions can be found at https://scikit-learn.org/stable/modules/model_evaluation.html.
 
     Parameters
     ----------
     scorer : t.Union[str, t.Callable]
         sklearn scorer name or callable
-    possible_classes: t.Optional[t.List]
+    model_classes: t.Optional[t.List]
         possible classes output for model. None for regression tasks.
     name : str, default = None
         scorer name
     """
 
-    def __init__(self, scorer: t.Union[str, t.Callable], possible_classes: t.Optional[t.List], name: str = None):
+    def __init__(self,
+                 scorer: t.Union[str, t.Callable],
+                 model_classes: t.Optional[t.List],
+                 observed_classes: t.Optional[t.List],
+                 name: str = None):
         if isinstance(scorer, str):
             formatted_scorer_name = scorer.lower().replace('sensitivity', 'recall').replace('specificity', 'tnr') \
                 .replace(' ', '_')
             if formatted_scorer_name in regression_scorers_lower_is_better_dict:
                 warnings.warn(f'Deepchecks checks assume higher metric values represent better performance. '
                               f'{formatted_scorer_name} does not follow that convention.')
             if formatted_scorer_name in _str_to_scorer_dict:
@@ -199,200 +206,155 @@
         elif callable(scorer):
             self.scorer = scorer
         else:
             scorer_type = type(scorer).__name__
             msg = f'Scorer {name if name else ""} value should be either a callable or string but got: {scorer_type}'
             raise errors.DeepchecksValueError(msg)
         self.name = name if name else get_scorer_name(scorer)
-        self.possible_classes = possible_classes
+        self.model_classes = model_classes
+        self.observed_classes = observed_classes
 
     @classmethod
     def filter_nulls(cls, dataset: 'tabular.Dataset') -> 'tabular.Dataset':
         """Return data of dataset without null labels."""
         valid_idx = dataset.data[dataset.label_name].notna()
         return dataset.copy(dataset.data[valid_idx])
 
     def run_on_data_and_label(self, model, data: pd.DataFrame, label_col):
         """Run scorer with model, data and labels without null filtering."""
-        return self.scorer(model, data, label_col)
+        return self._run_score(model, data, label_col)
 
     def run_on_pred(self, y_true, y_pred=None, y_proba=None):
         """Run sklearn scorer on the labels and the pred/proba according to scorer type."""
         # pylint: disable=protected-access
         if isinstance(self.scorer, _BaseScorer):
             if y_proba and isinstance(self.scorer, _ProbaScorer):
                 pred_to_use = y_proba
             else:
                 pred_to_use = y_pred
             return self.scorer._score_func(y_true, pred_to_use, **self.scorer._kwargs) * self.scorer._sign
         raise errors.DeepchecksValueError('Only supports sklearn scorers')
 
-    def _wrap_classification_model(self, model, label_col: pd.Series):
-        """Convert labels to 0/1 if model is a binary classifier, update classes_ property and pad probas."""
+    def _wrap_classification_model(self, model):
+        """Convert labels to 0/1 if model is a binary classifier, and converts to multi-label if multiclass."""
 
         class MyModelWrapper:
-            """Convert labels to 0/1 if model is a binary classifier, update classes_ property and pad probas."""
+            """Convert labels to 0/1 if model is a binary classifier, and converts to multi-label if multiclass."""
 
-            def __init__(self, user_model, possible_classes):
+            def __init__(self, user_model, model_classes):
                 self.user_model = user_model
-                self.possible_classes = possible_classes
-                if hasattr(model, 'classes_') and len(model.classes_) > 0 \
-                        and len(model.classes_) != len(possible_classes):
-                    self.indexes_to_pad_around = [possible_classes.index(x) for x in list(model.classes_)]
-                else:
-                    self.indexes_to_pad_around = None
+                self.model_classes = model_classes
+                self.is_binary = self.model_classes and len(self.model_classes) == 2
 
             def predict(self, data: pd.DataFrame) -> np.ndarray:
                 """Convert labels to 0/1 if model is a binary classifier."""
-                if len(self.possible_classes) == 2:
-                    transfer_func = np.vectorize(lambda x: 0 if x == self.possible_classes[0] else 1)
-                    return transfer_func(np.asarray(self.user_model.predict(data)))
-                else:
-                    return self.user_model.predict(data)
+                predicitions: np.ndarray = np.asarray(self.user_model.predict(data))
+                # In case of binary converts into 0 and 1 the labels
+                if self.is_binary:
+                    transfer_func = np.vectorize(lambda x: 0 if x == self.model_classes[0] else 1)
+                    predicitions = transfer_func(predicitions)
+                # In case of multiclass with single label, convert into multi-label
+                elif self.model_classes:
+                    predicitions = _transform_to_multi_label_format(predicitions, self.model_classes)
+                return predicitions
 
             def predict_proba(self, data: pd.DataFrame) -> np.ndarray:
-                """Pad probabilities per class to match the length of possible classes."""
+                """Validate model have predict_proba, and the proba matches the model classes."""
                 if not hasattr(self.user_model, 'predict_proba'):
                     if isinstance(self.user_model, ClassifierMixin):
                         raise errors.DeepchecksValueError('Model is a sklearn classification model but lacks the'
                                                           ' predict_proba method. Please train the model with'
                                                           ' probability=True.')
-                    raise errors.DeepchecksValueError('Scorer requires predicted probabilities, but the predict_proba'
-                                                      ' method was not implemented in the model, or precalculated '
-                                                      'predicted probabilities where not passed.')
+                    raise errors.DeepchecksValueError(f'Scorer requires predicted probabilities, either implement '
+                                                      f'predict_proba functionalities within the model objects or pass '
+                                                      f'pre calculated probabilities. {SUPPORTED_MODELS_DOCLINK}')
                 probabilities_per_class = self.user_model.predict_proba(data)
-                if self.indexes_to_pad_around is not None:
-                    padded_probabilities_per_class = np.zeros((len(data), len(self.possible_classes)))
-                    for idx, i in enumerate(self.indexes_to_pad_around):
-                        padded_probabilities_per_class[:, i] = probabilities_per_class[:, idx]
-                    return padded_probabilities_per_class
-                elif probabilities_per_class.shape[1] != len(self.possible_classes):
+                if probabilities_per_class.shape[1] != len(self.model_classes):
                     raise errors.ModelValidationError(
                         f'Model probabilities per class has {probabilities_per_class.shape[1]} '
-                        f'columns while observed classes include {self.possible_classes}.')
-                else:
-                    return probabilities_per_class
+                        f'classes while known model classes has {len(self.model_classes)}. You can set the model\'s'
+                        f'classes manually using the model_classes argument in the run function.')
+                return probabilities_per_class
 
             @property
             def classes_(self):
-                return np.asarray([0, 1] if len(self.possible_classes) == 2 else self.possible_classes)
+                return np.asarray([0, 1] if len(self.model_classes) == 2 else self.model_classes)
 
-        updated_label_col = label_col.map({self.possible_classes[0]: 0, self.possible_classes[1]: 1}) \
-            if len(self.possible_classes) == 2 else label_col
-        return MyModelWrapper(model, self.possible_classes), updated_label_col
+        return MyModelWrapper(model, self.model_classes)
 
-    def _run_score(self, model, dataset: 'tabular.Dataset'):
+    def _run_score(self, model, data: pd.DataFrame, label_col):
         # If scorer 'needs_threshold' or 'needs_proba' than the model has to have a predict_proba method.
         if ('needs' in self.scorer._factory_args()) and not hasattr(model,  # pylint: disable=protected-access
                                                                     'predict_proba'):
-            doclink_str = doclink('supported_models',
-                                  template='For more information please refer to the Supported Models guide {link}')
             raise errors.DeepchecksValueError(
                 f'Can\'t compute scorer {self.scorer} when predicted probabilities are '
                 f'not provided. Please use a model with predict_proba method or '
                 f'manually provide predicted probabilities to the check. '
-                f'{doclink_str}')
-        if self.possible_classes is not None:
-            updated_model, transformed_label_col = self._wrap_classification_model(model, dataset.label_col)
-            return self.scorer(updated_model, dataset.features_columns, transformed_label_col)
+                f'{SUPPORTED_MODELS_DOCLINK}')
+        if self.model_classes is not None:
+            updated_model = self._wrap_classification_model(model)
+            if updated_model.is_binary:
+                label = label_col.map({self.model_classes[0]: 0, self.model_classes[1]: 1}).to_numpy()
+            else:
+                label = _transform_to_multi_label_format(np.array(label_col), self.model_classes)
+
+            scores = self.scorer(updated_model, data, label)
+
+            # The scores returned are for the observed classes but we want scores of the observed classes
+            if isinstance(scores, t.Sized):
+                if len(scores) != len(self.model_classes):
+                    raise errors.DeepchecksValueError(
+                        f'Scorer returned {len(scores)} scores, but model contains '
+                        f'{len(self.model_classes)} classes. Can\'t proceed')
+                scores = dict(zip(self.model_classes, scores))
+                # Add classes which been seen in the data but are not known to the model
+                scores.update({cls: np.nan for cls in set(self.observed_classes) - set(self.model_classes)})
+            return scores
         else:
-            return self.scorer(model, dataset.features_columns, dataset.label_col)
+            return self.scorer(model, data, label_col)
 
     def __call__(self, model, dataset: 'tabular.Dataset'):
         """Run score with labels null filtering."""
-        return self._run_score(model, self.filter_nulls(dataset))
+        dataset_without_nulls = self.filter_nulls(dataset)
+        return self._run_score(model, dataset_without_nulls.features_columns, dataset_without_nulls.label_col)
 
     def score_perfect(self, dataset: 'tabular.Dataset'):
         """Calculate the perfect score of the current scorer for given dataset."""
         dataset = self.filter_nulls(dataset)
         perfect_model = PerfectModel()
         perfect_model.fit(None, dataset.label_col)
-        score = self._run_score(perfect_model, dataset)
-        if isinstance(score, np.ndarray):
+        score = self._run_score(perfect_model, dataset.features_columns, dataset.label_col)
+        if isinstance(score, dict):
             # We expect the perfect score to be equal for all the classes, so takes the first one
-            first_score = score[0]
-            if any(score != first_score):
+            score_values = np.asarray(list(score.values()))
+            first_score = score_values[0]
+            if any(score_values != first_score):
                 get_logger().warning('Scorer %s return different perfect score for different classes', self.name)
             return first_score
         return score
 
     def validate_fitting(self, model, dataset: 'tabular.Dataset'):
         """Validate given scorer for the model and dataset."""
         dataset.assert_features()
         # In order for scorer to return result in right dimensions need to pass it samples from all labels
         single_label_data = dataset.data[dataset.data[dataset.label_name].notna()].groupby(dataset.label_name).head(1)
-        result = self._run_score(model, dataset.copy(single_label_data))
+        new_dataset = dataset.copy(single_label_data)
+        result = self._run_score(model, new_dataset.features_columns, new_dataset.label_col)
 
-        if isinstance(result, np.ndarray):
-            expected_types = t.cast(
-                str,
-                np.typecodes['AllInteger'] + np.typecodes['AllFloat']  # type: ignore
-            )
-            kind = result.dtype.kind
-            if kind not in expected_types:
-                raise errors.DeepchecksValueError(f'Expected scorer {self.name} to return np.ndarray of number kind '
-                                                  f'but got: {kind}')
+        if isinstance(result, dict):
             # Validate returns value for each class
-            if len(result) != len(single_label_data):
-                raise errors.DeepchecksValueError(f'Found {len(single_label_data)} classes, but scorer {self.name} '
+            all_classes = set(self.model_classes) | set(self.observed_classes)
+            if len(result) != len(all_classes):
+                raise errors.DeepchecksValueError(f'Expected {len(all_classes)} classes, but scorer {self.name} '
                                                   f'returned {len(result)} elements in the score array value')
         elif not isinstance(result, Number):
-            raise errors.DeepchecksValueError(f'Expected scorer {self.name} to return number or np.ndarray '
+            raise errors.DeepchecksValueError(f'Expected scorer {self.name} to return number or dict '
                                               f'but got: {type(result).__name__}')
 
 
-def task_type_check(
-        model: BasicModel,
-        dataset: 'tabular.Dataset'
-) -> TaskType:
-    """Check task type (regression, binary, multiclass) according to model object and label column.
-
-    Parameters
-    ----------
-    model : BasicModel
-        Model object - used to check if it has predict_proba()
-    dataset : tabular.Dataset
-        dataset - used to count the number of unique labels
-
-    Returns
-    -------
-    TaskType
-        TaskType enum corresponding to the model and dataset
-    """
-    label_col = dataset.label_col
-    if not model:
-        return dataset.label_type
-    if isinstance(model, BaseEstimator):
-        if not hasattr(model, 'predict_proba'):
-            if is_string_column(label_col):
-                raise errors.DeepchecksValueError(
-                    'Model was identified as a regression model, but label column was found to contain strings.'
-                )
-            elif isinstance(model, ClassifierMixin):
-                raise errors.DeepchecksValueError(
-                    'Model is a sklearn classification model (a subclass of ClassifierMixin), but lacks the '
-                    'predict_proba method. Please train the model with probability=True, or skip / ignore this check.'
-                )
-            else:
-                return TaskType.REGRESSION
-        else:
-            return (
-                TaskType.MULTICLASS
-                if label_col.nunique() > 2
-                else TaskType.BINARY
-            )
-    if isinstance(model, ClassificationModel):
-        return (
-            TaskType.MULTICLASS
-            if label_col.nunique() > 2
-            else TaskType.BINARY
-        )
-    return TaskType.REGRESSION
-
-
 def get_default_scorers(model_type, class_avg: bool = True):
     """Get default scorers based on model type.
 
     Parameters
     ----------
     model_type : TaskType
         model type to return scorers for
@@ -406,32 +368,49 @@
     else:
         return DEFAULT_SCORERS_DICT[model_type]
 
 
 def init_validate_scorers(scorers: t.Union[t.Mapping[str, t.Union[str, t.Callable]], t.List[str]],
                           model: BasicModel,
                           dataset: 'tabular.Dataset',
-                          possible_classes: t.Optional[t.List]) -> t.List[DeepcheckScorer]:
+                          model_classes: t.Optional[t.List],
+                          observed_classes: t.Optional[t.List]) -> t.List[DeepcheckScorer]:
     """Initialize scorers and return all of them as deepchecks scorers.
 
     Parameters
     ----------
     scorers : Mapping[str, Union[str, Callable]]
         dict of scorers names to scorer sklearn_name/function or a list without a name
     model : BasicModel
         used to validate the scorers, and calculate mode_type if None.
     dataset : Dataset
         used to validate the scorers, and calculate mode_type if None.
-    possible_classes: t.Optional[t.List], default = None
+    model_classes: t.Optional[t.List]
         possible classes output for model. None for regression tasks.
+    observed_classes: t.Optional[t.List]
+        observed classes from labels and predictions. None for regression tasks.
     Returns
     --------
     scorers: t.List[DeepcheckScorer]
         A list of initialized DeepcheckScorers.
     """
     if isinstance(scorers, t.Mapping):
-        scorers = [DeepcheckScorer(scorer, possible_classes, name) for name, scorer in scorers.items()]
+        scorers = [DeepcheckScorer(scorer, model_classes, observed_classes, name) for name, scorer in scorers.items()]
     else:
-        scorers = [DeepcheckScorer(scorer, possible_classes) for scorer in scorers]
+        scorers = [DeepcheckScorer(scorer, model_classes, observed_classes) for scorer in scorers]
     for s in scorers:
         s.validate_fitting(model, dataset)
     return scorers
+
+
+def _transform_to_multi_label_format(y: np.ndarray, classes):
+    # Some classifiers like catboost might return shape like (n_rows, 1), therefore squeezing the array.
+    y = np.squeeze(y) if y.ndim > 1 else y
+    if y.ndim == 1:
+        binarizer = LabelBinarizer()
+        binarizer.fit(classes)
+        return binarizer.transform(y)
+    # If after squeeze there are still 2 dimensions, then it must have column for each model class.
+    elif y.ndim == 2 and y.shape[1] == len(classes):
+        return y
+    else:
+        raise errors.DeepchecksValueError(f'got y with unworkable shape: {y.shape}. {SUPPORTED_MODELS_DOCLINK}')
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/model_base.py` & `deepchecks-0.9.2/deepchecks/tabular/model_base.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/suite.py` & `deepchecks-0.9.2/deepchecks/tabular/suite.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/suites/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/suites/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/suites/default_suites.py` & `deepchecks-0.9.2/deepchecks/tabular/suites/default_suites.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,18 @@
 from deepchecks.tabular.checks import (BoostingOverfit, CalibrationScore, CategoryMismatchTrainTest, ConflictingLabels,
                                        ConfusionMatrixReport, DataDuplicates, DatasetsSizeComparison,
                                        DateTrainTestLeakageDuplicates, DateTrainTestLeakageOverlap,
                                        FeatureFeatureCorrelation, FeatureLabelCorrelation,
                                        FeatureLabelCorrelationChange, IdentifierLabelCorrelation, IndexTrainTestLeakage,
                                        IsSingleValue, MixedDataTypes, MixedNulls, ModelInferenceTime, MultivariateDrift,
                                        NewLabelTrainTest, OutlierSampleDetection, RegressionErrorDistribution,
-                                       RegressionSystematicError, RocReport, SimpleModelComparison, SpecialCharacters,
-                                       StringLengthOutOfBounds, StringMismatch, StringMismatchComparison,
-                                       TrainTestFeatureDrift, TrainTestLabelDrift, TrainTestPerformance,
-                                       TrainTestPredictionDrift, TrainTestSamplesMix, UnusedFeatures,
-                                       WeakSegmentsPerformance)
+                                       RocReport, SimpleModelComparison, SpecialCharacters, StringLengthOutOfBounds,
+                                       StringMismatch, StringMismatchComparison, TrainTestFeatureDrift,
+                                       TrainTestLabelDrift, TrainTestPerformance, TrainTestPredictionDrift,
+                                       TrainTestSamplesMix, UnusedFeatures, WeakSegmentsPerformance)
 
 __all__ = ['data_integrity', 'train_test_validation', 'model_evaluation', 'full_suite']
 
 from deepchecks.utils.typing import Hashable
 
 
 def data_integrity(columns: Union[Hashable, List[Hashable]] = None,
@@ -314,16 +313,16 @@
         TrainTestPerformance(**kwargs).add_condition_train_test_relative_degradation_less_than(),
         RocReport(**kwargs).add_condition_auc_greater_than(),
         ConfusionMatrixReport(**kwargs),
         TrainTestPredictionDrift(**kwargs).add_condition_drift_score_less_than(),
         SimpleModelComparison(**kwargs).add_condition_gain_greater_than(),
         WeakSegmentsPerformance(**kwargs).add_condition_segments_relative_performance_greater_than(),
         CalibrationScore(**kwargs),
-        RegressionSystematicError(**kwargs).add_condition_systematic_error_ratio_to_rmse_less_than(),
-        RegressionErrorDistribution(**kwargs).add_condition_kurtosis_greater_than(),
+        RegressionErrorDistribution(
+            **kwargs).add_condition_kurtosis_greater_than().add_condition_systematic_error_ratio_to_rmse_less_than(),
         UnusedFeatures(**kwargs).add_condition_number_of_high_variance_unused_features_less_or_equal(),
         BoostingOverfit(**kwargs).add_condition_test_score_percent_decline_less_than(),
         ModelInferenceTime(**kwargs).add_condition_inference_time_less_than(),
     )
 
 
 def full_suite(**kwargs) -> Suite:
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/utils/__init__.py` & `deepchecks-0.9.2/deepchecks/tabular/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/utils/feature_importance.py` & `deepchecks-0.9.2/deepchecks/tabular/utils/feature_importance.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import pandas as pd
 from sklearn.inspection import permutation_importance
 from sklearn.pipeline import Pipeline
 
 from deepchecks import tabular
 from deepchecks.core import errors
 from deepchecks.tabular.metric_utils.scorers import DeepcheckScorer, get_default_scorers, init_validate_scorers
-from deepchecks.tabular.utils.task_inference import get_possible_classes, infer_task_type
 from deepchecks.tabular.utils.validation import validate_model
 from deepchecks.utils.logger import get_logger
 from deepchecks.utils.typing import Hashable
 
 __all__ = [
     '_calculate_feature_importance',
     'calculate_feature_importance_or_none',
@@ -37,25 +36,34 @@
 
 N_TOP_MESSAGE = 'Showing only the top %s columns, you can change it using n_top_columns param'
 
 
 def calculate_feature_importance_or_none(
         model: t.Any,
         dataset: t.Union['tabular.Dataset', pd.DataFrame],
+        model_classes,
+        observed_classes,
+        task_type,
         force_permutation: bool = False,
         permutation_kwargs: t.Optional[t.Dict[str, t.Any]] = None,
 ) -> t.Tuple[t.Optional[pd.Series], t.Optional[str]]:
     """Calculate features effect on the label or None if the input is incorrect.
 
     Parameters
     ----------
     model : t.Any
         a fitted model
     dataset : t.Union['tabular.Dataset', pd.DataFrame]
         dataset used to fit the model
+    model_classes
+        possible classes output for model. None for regression tasks.
+    observed_classes
+        Observed classes in the data. None for regression tasks.
+    task_type
+        The task type of the model.
     force_permutation : bool , default: False
         force permutation importance calculation
     permutation_kwargs : t.Optional[t.Dict[str, t.Any]] , default: None
         kwargs for permutation importance calculation
 
     Returns
     -------
@@ -67,14 +75,17 @@
     try:
         if model is None:
             return None
         # calculate feature importance if dataset has a label and the model is fitted on it
         fi, calculation_type = _calculate_feature_importance(
             model=model,
             dataset=dataset,
+            model_classes=model_classes,
+            observed_classes=observed_classes,
+            task_type=task_type,
             force_permutation=force_permutation,
             permutation_kwargs=permutation_kwargs,
         )
 
         return fi, calculation_type
     except (
             errors.DeepchecksValueError,
@@ -96,25 +107,34 @@
         get_logger().warning('Features importance was not calculated:\n%s', error)
         return None, None
 
 
 def _calculate_feature_importance(
         model: t.Any,
         dataset: t.Union['tabular.Dataset', pd.DataFrame],
+        model_classes,
+        observed_classes,
+        task_type,
         force_permutation: bool = False,
         permutation_kwargs: t.Dict[str, t.Any] = None,
 ) -> t.Tuple[pd.Series, str]:
     """Calculate features effect on the label.
 
     Parameters
     ----------
     model : t.Any
         a fitted model
     dataset : t.Union['tabular.Dataset', pd.DataFrame]
         dataset used to fit the model
+    model_classes
+        possible classes output for model. None for regression tasks.
+    observed_classes
+        Observed classes in the data. None for regression tasks.
+    task_type
+        The task type of the model.
     force_permutation : bool, default: False
         force permutation importance calculation
     permutation_kwargs : t.Dict[str, t.Any] , default: None
         kwargs for permutation importance calculation
 
     Returns
     -------
@@ -142,15 +162,16 @@
 
     if force_permutation:
         if isinstance(dataset, pd.DataFrame):
             raise errors.DeepchecksValueError('Cannot calculate permutation feature importance on a pandas Dataframe. '
                                               'In order to force permutation feature importance, please use the Dataset'
                                               ' object.')
         else:
-            importance = _calc_permutation_importance(model, dataset, **permutation_kwargs)
+            importance = _calc_permutation_importance(model, dataset, model_classes, observed_classes,
+                                                      task_type, **permutation_kwargs)
             calc_type = 'permutation_importance'
 
     # If there was no force permutation, or if it failed while trying to calculate importance,
     # we don't take built-in importance in pipelines because the pipeline is changing the features
     # (for example one-hot encoding) which leads to the inner model features
     # being different than the original dataset features
     if importance is None and not isinstance(model, Pipeline):
@@ -165,15 +186,16 @@
         if not permutation_kwargs.get('skip_messages', False):
             if isinstance(model, Pipeline):
                 pre_text = 'Cannot use model\'s built-in feature importance on a Scikit-learn Pipeline,'
             else:
                 pre_text = 'Could not find built-in feature importance on the model,'
             get_logger().warning('%s using permutation feature importance calculation instead', pre_text)
 
-        importance = _calc_permutation_importance(model, dataset, **permutation_kwargs)
+        importance = _calc_permutation_importance(model, dataset, model_classes, observed_classes,
+                                                  task_type, **permutation_kwargs)
         calc_type = 'permutation_importance'
 
     # If after all importance is still none raise error
     if importance is None:
         # FIXME: better message
         raise errors.DeepchecksValueError('Was not able to calculate features importance')
     return importance.fillna(0), calc_type
@@ -201,30 +223,39 @@
 
     return None, None
 
 
 def _calc_permutation_importance(
         model: t.Any,
         dataset: 'tabular.Dataset',
+        model_classes,
+        observed_classes,
+        task_type,
         n_repeats: int = 30,
         mask_high_variance_features: bool = False,
         random_state: int = 42,
         n_samples: int = 10_000,
         alternative_scorer: t.Optional[DeepcheckScorer] = None,
         skip_messages: bool = False,
-        timeout: int = None
+        timeout: int = None,
 ) -> pd.Series:
     """Calculate permutation feature importance. Return nonzero value only when std doesn't mask signal.
 
     Parameters
     ----------
     model: t.Any
         A fitted model
     dataset: tabular.Dataset
         dataset used to fit the model
+    model_classes
+        possible classes output for model. None for regression tasks.
+    observed_classes
+        Observed classes in the data. None for regression tasks.
+    task_type
+        The task type of the model.
     n_repeats: int, default: 30
         Number of times to permute a feature
     mask_high_variance_features : bool , default: False
         If true, features for which calculated permutation importance values
         varied greatly would be returned has having 0 feature importance
     random_state: int, default: 42
         Random seed for permutation importance calculation.
@@ -255,20 +286,18 @@
 
     dataset_sample = dataset.sample(n_samples, drop_na_label=True, random_state=random_state)
 
     # Test score time on the dataset sample
     if alternative_scorer:
         scorer = alternative_scorer
     else:
-        task_type = infer_task_type(model, dataset)
         default_scorers = get_default_scorers(task_type)
         scorer_name = next(iter(default_scorers))
         single_scorer_dict = {scorer_name: default_scorers[scorer_name]}
-        possible_classes = get_possible_classes(model, dataset)
-        scorer = init_validate_scorers(single_scorer_dict, model, dataset, possible_classes)[0]
+        scorer = init_validate_scorers(single_scorer_dict, model, dataset, model_classes, observed_classes)[0]
 
     start_time = time.time()
     scorer(model, dataset_sample)
     calc_time = time.time() - start_time
 
     predicted_time_to_run = int(np.ceil(calc_time * n_repeats * len(dataset.features))) or 1
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/utils/feature_inference.py` & `deepchecks-0.9.2/deepchecks/tabular/utils/feature_inference.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/utils/messages.py` & `deepchecks-0.9.2/deepchecks/tabular/utils/messages.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/utils/task_inference.py` & `deepchecks-0.9.2/deepchecks/tabular/utils/task_inference.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,98 +6,93 @@
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Utils module containing functionalities to infer the task type and possible label classes."""
 
-__all__ = ['get_possible_classes', 'infer_task_type']
+__all__ = ['infer_task_type_and_classes']
 
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import pandas as pd
+from pandas._libs.lib import infer_dtype
 
-from deepchecks import tabular
-from deepchecks.core.errors import DeepchecksValueError
+from deepchecks import tabular  # pylint: disable=unused-import; it is used for type annotations
+from deepchecks.core.errors import ValidationError
 from deepchecks.tabular.utils.feature_inference import is_categorical
 from deepchecks.tabular.utils.task_type import TaskType
 from deepchecks.utils.array_math import convert_into_flat_list
 from deepchecks.utils.logger import get_logger
 from deepchecks.utils.typing import BasicModel
 
 
-# pylint: disable=protected-access
-def get_possible_classes(model: Optional[BasicModel], train_dataset: 'tabular.Dataset',
-                         test_dataset: Optional['tabular.Dataset'] = None, force_classification: bool = False) \
-        -> Optional[List]:
-    """Return the list of allowed classes for classification tasks or None for regression.
+def infer_task_type_and_classes(model: Optional[BasicModel], train_dataset: 'tabular.Dataset',
+                                test_dataset: Optional['tabular.Dataset'] = None,
+                                model_classes: Optional[List] = None) -> \
+        Tuple[TaskType, Optional[List], Optional[List]]:
+    """Infer the task type based on labels in the data and the model. For classification also computes the classes in \
+    the model and the observed classes.
 
     Parameters
     ----------
     model : BasicModel
         Model object used in task
     train_dataset : 'tabular.Dataset'
         Train Dataset of task
     test_dataset : Optional['tabular.Dataset'], default = None
         Test Dataset of task
-    force_classification: bool, default = False
-        Whether to disable the auto infer for task type and return all observed label values.
-    Returns
-    -------
-    Optional[List]
-        The list of possible classes for classification tasks or None for regression
-    """
-    if not isinstance(train_dataset, tabular.Dataset) or (test_dataset is not None and
-                                                          not isinstance(test_dataset, tabular.Dataset)):
-        raise DeepchecksValueError('train_dataset and test_dataset must be of type tabular.Dataset')
-
-    if train_dataset._label_classes is not None:
-        if hasattr(model, 'classes_') and len(model.classes_) > 0 and \
-                list(model.classes_) != train_dataset._label_classes:
-            raise DeepchecksValueError('Model output classes and train dataset label classes do not match')
-        return train_dataset._label_classes
-
-    observed_labels = list(train_dataset.label_col)
-    if test_dataset is not None:
-        observed_labels += list(test_dataset.label_col)
-    if hasattr(model, 'classes_') and len(model.classes_) > 0:
-        if not set(pd.Series(observed_labels).dropna().unique()).issubset(set(model.classes_)):
-            get_logger().warning('Model classes attribute does not contain all observed labels in train and test data.')
-        observed_labels += list(model.classes_)
-
-    if model is not None:  # classification model without classes_ attribute
-        observed_labels += convert_into_flat_list(model.predict(train_dataset.features_columns))
-        if test_dataset is not None:
-            observed_labels += convert_into_flat_list(model.predict(test_dataset.features_columns))
-        if hasattr(model, 'predict_proba'):  # This means it's a classification model
-            return sorted(pd.Series(observed_labels).dropna().unique())
-    label_series = pd.Series(observed_labels)
-    if is_categorical(label_series, max_categorical_ratio=0.05) or force_classification:
-        return sorted(label_series.dropna().unique())
-    else:  # no predict_proba method + not categorical column (regression)
-        return None
-
-
-def infer_task_type(model: Optional[BasicModel], train_dataset: 'tabular.Dataset',
-                    test_dataset: Optional['tabular.Dataset'] = None) -> TaskType:
-    """Infer the task type based on get_possible_classes.
+    model_classes
+        Model's classes if provided by the user manually.
 
-    Parameters
-    ----------
-    model : BasicModel
-        Model object used in task
-    train_dataset : 'tabular.Dataset'
-        Train Dataset of task
-    test_dataset : Optional['tabular.Dataset'], default = None
-        Test Dataset of task
     Returns
     -------
-    TaskType
-        The type of the Task
+    (TaskType, List, List)
+        The type of the Task, The observed classes, The model classes
     """
-    classes = get_possible_classes(model, train_dataset, test_dataset)
-    if classes is None:
-        return TaskType.REGRESSION
-    elif len(classes) == 2:
-        return TaskType.BINARY
+    train_labels = []
+    test_labels = []
+    have_model = model is not None
+    if train_dataset:
+        if train_dataset.has_label():
+            train_labels += train_dataset.label_col.to_list()
+        if have_model:
+            train_labels += convert_into_flat_list(model.predict(train_dataset.features_columns))
+    if test_dataset:
+        if test_dataset.has_label():
+            test_labels += test_dataset.label_col.to_list()
+        if have_model:
+            test_labels += convert_into_flat_list(model.predict(test_dataset.features_columns))
+
+    observed_labels = pd.Series(test_labels + train_labels)
+    if model_classes is None and have_model and hasattr(model, 'classes_') and len(model.classes_) > 0:
+        model_classes = sorted(list(model.classes_))
+
+    if train_dataset and train_dataset.label_type is not None:
+        task_type = train_dataset.label_type
+    elif model_classes:
+        task_type = infer_by_class_number(len(model_classes))
+    elif len(observed_labels) > 0 and is_categorical(observed_labels, max_categorical_ratio=0.05):
+        num_classes = len(observed_labels.dropna().unique())
+        task_type = infer_by_class_number(num_classes)
+        if infer_dtype(observed_labels) == 'integer' and train_dataset and train_dataset.label_type is None:
+            get_logger().warning(
+                'Due to the small number of unique labels task type was inferred as classification in spite of '
+                'the label column is of type integer. '
+                'Initialize your Dataset with either label_type=\"multiclass\" or '
+                'label_type=\"regression\" to resolve this warning.')
     else:
-        return TaskType.MULTICLASS
+        task_type = TaskType.REGRESSION
+
+    if task_type in [TaskType.BINARY, TaskType.MULTICLASS]:
+        return task_type, sorted(observed_labels.dropna().unique()), model_classes
+    else:
+        return task_type, None, None
+
+
+def infer_by_class_number(num_classes):
+    if num_classes == 0:
+        raise ValidationError('Found zero number of classes')
+    if num_classes == 1:
+        raise ValidationError('Found only one class in label column, pass the full list of possible '
+                              'label classes via the model_classes argument of the run function.')
+    return TaskType.BINARY if num_classes == 2 else TaskType.MULTICLASS
```

### Comparing `deepchecks-0.9.1/deepchecks/tabular/utils/task_type.py` & `deepchecks-0.9.2/deepchecks/tabular/utils/task_type.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/tabular/utils/validation.py` & `deepchecks-0.9.2/deepchecks/tabular/utils/validation.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/__init__.py` & `deepchecks-0.9.2/deepchecks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/array_math.py` & `deepchecks-0.9.2/deepchecks/utils/array_math.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/correlation_methods.py` & `deepchecks-0.9.2/deepchecks/utils/correlation_methods.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/dataframes.py` & `deepchecks-0.9.2/deepchecks/utils/dataframes.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/decorators.py` & `deepchecks-0.9.2/deepchecks/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/dict_funcs.py` & `deepchecks-0.9.2/deepchecks/utils/dict_funcs.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/display.py` & `deepchecks-0.9.2/deepchecks/utils/display.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/distribution/__init__.py` & `deepchecks-0.9.2/deepchecks/utils/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/distribution/drift.py` & `deepchecks-0.9.2/deepchecks/utils/distribution/drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/distribution/plot.py` & `deepchecks-0.9.2/deepchecks/utils/distribution/plot.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/distribution/preprocessing.py` & `deepchecks-0.9.2/deepchecks/utils/distribution/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/distribution/rare_category_encoder.py` & `deepchecks-0.9.2/deepchecks/utils/distribution/rare_category_encoder.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/distribution/trust_score.py` & `deepchecks-0.9.2/deepchecks/utils/distribution/trust_score.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/docref.py` & `deepchecks-0.9.2/deepchecks/utils/docref.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/function.py` & `deepchecks-0.9.2/deepchecks/utils/function.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/gower_distance.py` & `deepchecks-0.9.2/deepchecks/utils/gower_distance.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/html.py` & `deepchecks-0.9.2/deepchecks/utils/html.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/ipython.py` & `deepchecks-0.9.2/deepchecks/utils/ipython.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/json_utils.py` & `deepchecks-0.9.2/deepchecks/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/logger.py` & `deepchecks-0.9.2/deepchecks/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/metrics.py` & `deepchecks-0.9.2/deepchecks/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/model.py` & `deepchecks-0.9.2/deepchecks/utils/model.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/outliers.py` & `deepchecks-0.9.2/deepchecks/utils/outliers.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/performance/__init__.py` & `deepchecks-0.9.2/deepchecks/utils/performance/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/performance/error_model.py` & `deepchecks-0.9.2/deepchecks/utils/performance/error_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from sklearn.pipeline import Pipeline
 from sklearn.tree import DecisionTreeRegressor
 
 from deepchecks import tabular
 from deepchecks.core.errors import DeepchecksProcessError
 from deepchecks.tabular import Dataset
 from deepchecks.tabular.utils.feature_importance import _calculate_feature_importance
+from deepchecks.tabular.utils.task_type import TaskType
 from deepchecks.utils.plot import colors
 from deepchecks.utils.strings import format_number, format_percent
 
 
 def model_error_contribution(train_dataset: pd.DataFrame,
                              train_scores: pd.Series,
                              test_dataset: pd.DataFrame,
@@ -51,14 +52,17 @@
 
     # This check should be ignored if no information gained from the error model (low r2_score)
     if error_model_score < min_error_model_score:
         raise DeepchecksProcessError(f'Unable to train meaningful error model '
                                      f'(r^2 score: {format_number(error_model_score)})')
     error_fi, _ = _calculate_feature_importance(error_model,
                                                 Dataset(test_dataset, test_scores, cat_features=categorical_features),
+                                                model_classes=None,
+                                                observed_classes=None,
+                                                task_type=TaskType.REGRESSION,
                                                 permutation_kwargs={'random_state': random_state,
                                                                     'skip_messages': True})
     error_fi.index = new_feature_order
     error_fi.sort_values(ascending=False, inplace=True)
     return error_fi, error_model_predicted
```

### Comparing `deepchecks-0.9.1/deepchecks/utils/performance/partition.py` & `deepchecks-0.9.2/deepchecks/utils/performance/partition.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/plot.py` & `deepchecks-0.9.2/deepchecks/utils/plot.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/simple_models.py` & `deepchecks-0.9.2/deepchecks/utils/simple_models.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/single_sample_metrics.py` & `deepchecks-0.9.2/deepchecks/utils/single_sample_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/strings.py` & `deepchecks-0.9.2/deepchecks/utils/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,17 @@
         whether to return full html page or not
     """
     state = dependency_state(widget)
     data = embed_data(views=[widget], drop_defaults=True, state=state)
 
     snippet = snippet_template.format(
         load='',  # will be added below
-        json_data=escape_script(json.dumps(data['manager_state'])),
+        json_data=escape_script(json.dumps(data['manager_state'], default=json_encoder)),
         widget_views='\n'.join(
-            widget_view_template.format(view_spec=escape_script(json.dumps(view_spec)))
+            widget_view_template.format(view_spec=escape_script(json.dumps(view_spec, default=json_encoder)))
             for view_spec in data['view_specs']
         )
     )
 
     template = suite_template(full_html=full_html)
     html = template.replace('$Title', title).replace('$WidgetSnippet', snippet)
 
@@ -655,7 +655,13 @@
         ext = default_suffix
     file_name = f'{basename}.{ext}'
     c = itertools.count()
     next(c)
     while os.path.exists(file_name):
         file_name = f'{basename} ({str(next(c))}).{ext}'
     return file_name
+
+
+def json_encoder(obj):
+    """Handle numpy objects for json dumps."""
+    if isinstance(obj, (np.generic, np.ndarray)):
+        return obj.item()
```

### Comparing `deepchecks-0.9.1/deepchecks/utils/typing.py` & `deepchecks-0.9.2/deepchecks/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/validation.py` & `deepchecks-0.9.2/deepchecks/utils/validation.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/utils/wandb_utils.py` & `deepchecks-0.9.2/deepchecks/utils/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/_shared_docs.py` & `deepchecks-0.9.2/deepchecks/vision/_shared_docs.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/base_checks.py` & `deepchecks-0.9.2/deepchecks/vision/base_checks.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module for vision base checks."""
+import warnings
 from typing import Any, Dict, Mapping, Optional, Sequence, Union
 
 import torch
 from ignite.metrics import Metric
 from torch import nn
 
 from deepchecks.core.check_result import CheckResult
 from deepchecks.core.checks import DatasetKind, ModelOnlyBaseCheck, SingleDatasetBaseCheck, TrainTestBaseCheck
+from deepchecks.core.errors import DeepchecksValueError
 from deepchecks.utils.ipython import ProgressBarGroup
 from deepchecks.vision import deprecation_warnings  # pylint: disable=unused-import # noqa: F401
 from deepchecks.vision._shared_docs import docstrings
 from deepchecks.vision.batch_wrapper import Batch
 from deepchecks.vision.context import Context
 from deepchecks.vision.utils.vision_properties import STATIC_PROPERTIES_FORMAT
 from deepchecks.vision.vision_data import VisionData
@@ -45,31 +47,43 @@
         model_name: str = '',
         scorers: Optional[Mapping[str, Metric]] = None,
         scorers_per_class: Optional[Mapping[str, Metric]] = None,
         device: Union[str, torch.device, None] = None,
         random_state: int = 42,
         n_samples: Optional[int] = 10_000,
         with_display: bool = True,
+        predictions: Optional[Dict[int, Union[Sequence[torch.Tensor], torch.Tensor]]] = None,
         train_predictions: Optional[Dict[int, Union[Sequence[torch.Tensor], torch.Tensor]]] = None,
         test_predictions: Optional[Dict[int, Union[Sequence[torch.Tensor], torch.Tensor]]] = None,
         train_properties: Optional[STATIC_PROPERTIES_FORMAT] = None,
         test_properties: Optional[STATIC_PROPERTIES_FORMAT] = None
+
     ) -> CheckResult:
         """Run check.
 
         Parameters
         ----------
         dataset: VisionData
             VisionData object to process
         model: Optional[nn.Module] , default None
             pytorch neural network module instance
         {additional_context_params:2*indent}
         """
         assert self.context_type is not None
+        if train_predictions is not None:
+            warnings.warn('train_predictions is deprecated, please use predictions instead.',
+                          DeprecationWarning, stacklevel=2)
+        if test_predictions is not None:
+            warnings.warn('test_predictions is deprecated and ignored.',
+                          DeprecationWarning, stacklevel=2)
+        if (train_predictions is not None) and (predictions is not None):
+            raise DeepchecksValueError('Cannot accept both train_predictions and predictions, please pass the data only'
+                                       ' to predictions.')
 
+        train_predictions = train_predictions if train_predictions is not None else predictions
         with ProgressBarGroup() as progressbar_factory:
 
             with progressbar_factory.create_dummy(name='Validating Input'):
                 # Context is copying the data object, then not using the original after the init
                 context: Context = self.context_type(
                     dataset,
                     model=model,
@@ -77,15 +91,14 @@
                     scorers=scorers,
                     scorers_per_class=scorers_per_class,
                     device=device,
                     random_state=random_state,
                     n_samples=n_samples,
                     with_display=with_display,
                     train_predictions=train_predictions,
-                    test_predictions=test_predictions,
                     train_properties=train_properties,
                     test_properties=test_properties
                 )
                 self.initialize_run(context, DatasetKind.TRAIN)
 
             context.train.init_cache()
```

### Comparing `deepchecks-0.9.1/deepchecks/vision/batch_wrapper.py` & `deepchecks-0.9.2/deepchecks/vision/batch_wrapper.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/abstract_property_outliers.py` & `deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/abstract_property_outliers.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/image_property_outliers.py` & `deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/image_property_outliers.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/label_property_outliers.py` & `deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/label_property_outliers.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/data_integrity/property_label_correlation.py` & `deepchecks-0.9.2/deepchecks/vision/checks/data_integrity/property_label_correlation.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/class_performance.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/class_performance.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module containing class performance check."""
-from typing import Dict, List, TypeVar, Union
+import warnings
+from typing import Any, Callable, Dict, List, TypeVar, Union
 
 import pandas as pd
 import plotly.express as px
 from ignite.metrics import Metric
 
 from deepchecks.core import CheckResult, DatasetKind
 from deepchecks.core.check_utils.class_performance_utils import (
@@ -32,17 +33,19 @@
 
 
 class ClassPerformance(TrainTestCheck):
     """Summarize given metrics on a dataset and model.
 
     Parameters
     ----------
+    scorers: Union[Dict[str, Union[Metric, Callable, str]], List[Any]], default: None
+        Scorers to override the default scorers (metrics), find more about the supported formats at
+        https://docs.deepchecks.com/stable/user-guide/general/metrics_guide.html
     alternative_metrics : Union[Dict[str, Union[Metric,str]], List[str]], default: None
-        A dictionary of metrics, where the key is the metric name and the value is an ignite.Metric object whose score
-        should be used. If None are given, use the default metrics.
+        Deprecated, please use scorers instead.
     n_to_show : int, default: 20
         Number of classes to show in the report. If None, show all classes.
     show_only : str, default: 'largest'
         Specify which classes to show in the report. Can be one of the following:
         - 'largest': Show the largest classes.
         - 'smallest': Show the smallest classes.
         - 'random': Show random classes.
@@ -53,22 +56,28 @@
         If None, sorting by the first metric in the default metrics list.
     class_list_to_show: List[int], default: None
         Specify the list of classes to show in the report. If specified, n_to_show, show_only and metric_to_show_by
         are ignored.
     """
 
     def __init__(self,
+                 scorers: Union[Dict[str, Union[Metric, Callable, str]], List[Any]] = None,
                  alternative_metrics: Union[Dict[str, Union[Metric, str]], List[str]] = None,
                  n_to_show: int = 20,
                  show_only: str = 'largest',
                  metric_to_show_by: str = None,
                  class_list_to_show: List[int] = None,
                  **kwargs):
         super().__init__(**kwargs)
-        self.alternative_metrics = alternative_metrics
+        if alternative_metrics is not None:
+            warnings.warn(f'{self.__class__.__name__}: alternative_metrics is deprecated. Please use scorers instead.',
+                          DeprecationWarning)
+            self.alternative_metrics = alternative_metrics
+        else:
+            self.alternative_metrics = scorers
         self.n_to_show = n_to_show
         self.class_list_to_show = class_list_to_show
 
         if self.class_list_to_show is None:
             if show_only not in ['largest', 'smallest', 'random', 'best', 'worst']:
                 raise DeepchecksValueError(f'Invalid value for show_only: {show_only}. Should be one of: '
                                            f'["largest", "smallest", "random", "best", "worst"]')
```

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/confusion_matrix.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/image_segment_performance.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/image_segment_performance.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module of segment performance check."""
 import math
 import typing as t
+import warnings
 from collections import Counter, defaultdict
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import torch
 from ignite.metrics import Metric
@@ -33,47 +34,55 @@
 
 
 class ImageSegmentPerformance(SingleDatasetCheck):
     """Segment the data by various properties of the image, and compare the performance of the segments.
 
     Parameters
     ----------
+    scorers: Union[Dict[str, Union[Metric, Callable, str]], List[Any]], default: None
+        Scorers to override the default scorers (metrics), find more about the supported formats at
+        https://docs.deepchecks.com/stable/user-guide/general/metrics_guide.html
     image_properties : List[Dict[str, Any]], default: None
         List of properties. Replaces the default deepchecks properties.
         Each property is a dictionary with keys ``'name'`` (str), ``method`` (Callable) and ``'output_type'`` (str),
         representing attributes of said method. 'output_type' must be one of:
 
         - ``'numeric'`` - for continuous ordinal outputs.
         - ``'categorical'`` - for discrete, non-ordinal outputs. These can still be numbers,
           but these numbers do not have inherent value.
 
         For more on image / label properties, see the guide about :ref:`vision_properties_guide`.
     alternative_metrics : Dict[str, Metric], default: None
-        A dictionary of metrics, where the key is the metric name and the value is an ignite. Metric object whose score
-        should be used. If None are given, use the default metrics.
+        Deprecated, please use scorers instead.
     number_of_bins: int, default : 5
         Maximum number of bins to segment a single property into.
     number_of_samples_to_infer_bins : int, default : 1000
         Minimum number of samples to use to infer the bounds of the segments' bins
     n_show_top : int , default: 3
         number of properties to show (shows by top diffrence by first metric)
     """
 
     def __init__(
         self,
+        scorers: t.Union[t.Dict[str, t.Union[Metric, t.Callable, str]], t.List[t.Any]] = None,
         image_properties: t.List[t.Dict[str, t.Any]] = None,
         alternative_metrics: t.Optional[t.Dict[str, Metric]] = None,
         number_of_bins: int = 5,
         number_of_samples_to_infer_bins: int = 1000,
         n_to_show: int = 3,
         **kwargs
     ):
         super().__init__(**kwargs)
         self.image_properties = image_properties if image_properties else default_image_properties
-        self.alternative_metrics = alternative_metrics
+        if alternative_metrics is not None:
+            warnings.warn(f'{self.__class__.__name__}: alternative_metrics is deprecated. Please use scorers instead.',
+                          DeprecationWarning)
+            self.alternative_metrics = alternative_metrics
+        else:
+            self.alternative_metrics = scorers
         self.number_of_bins = number_of_bins
         self.number_of_samples_to_infer_bins = number_of_samples_to_infer_bins
         self.n_to_show = n_to_show
 
         self._state = None
 
     def initialize_run(self, context: Context, dataset_kind: DatasetKind):
```

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/mean_average_precision_report.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/mean_average_precision_report.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/mean_average_recall_report.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/mean_average_recall_report.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/model_error_analysis.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/model_error_analysis.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/robustness_report.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/robustness_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module containing robustness report check."""
 import string
+import warnings
 from collections import defaultdict
 from random import choice
-from typing import Dict, List, Optional, Sequence, Sized, TypeVar
+from typing import Any, Callable, Dict, List, Optional, Sequence, Sized, TypeVar, Union
 
 import albumentations
 import imgaug
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import torch
@@ -42,30 +43,38 @@
 
 
 class RobustnessReport(SingleDatasetCheck):
     """Compare performance of model on original dataset and augmented dataset.
 
     Parameters
     ----------
+    scorers: Union[Dict[str, Union[Metric, Callable, str]], List[Any]], default: None
+        Scorers to override the default scorers (metrics), find more about the supported formats at
+        https://docs.deepchecks.com/stable/user-guide/general/metrics_guide.html
     alternative_metrics : Dict[str, Metric], default: None
-        A dictionary of metrics, where the key is the metric name and the value is an ignite.Metric object whose score
-        should be used. If None are given, use the default metrics.
+        Deprecated, please use scorers instead.
     augmentations : List, default: None
         A list of augmentations to test on the data. If none are given default augmentations are used.
         Supported augmentations are of albumentations and imgaug.
     """
 
     _THUMBNAIL_SIZE = (150, 150)
 
     def __init__(self,
+                 scorers: Union[Dict[str, Union[Metric, Callable, str]], List[Any]] = None,
                  alternative_metrics: Optional[Dict[str, Metric]] = None,
                  augmentations: List = None,
                  **kwargs):
         super().__init__(**kwargs)
-        self.alternative_metrics = alternative_metrics
+        if alternative_metrics is not None:
+            warnings.warn(f'{self.__class__.__name__}: alternative_metrics is deprecated. Please use scorers instead.',
+                          DeprecationWarning)
+            self.alternative_metrics = alternative_metrics
+        else:
+            self.alternative_metrics = scorers
         self.augmentations = augmentations
 
         self._state = None
 
     def initialize_run(self, context: Context, dataset_kind):
         """Initialize the metrics for the check, and validate task type is relevant."""
         dataset = context.get_data_by_kind(dataset_kind)
```

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/simple_model_comparison.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/simple_model_comparison.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 # Deepchecks is distributed under the terms of the GNU Affero General
 # Public License (version 3 or later).
 # You should have received a copy of the GNU Affero General Public License
 # along with Deepchecks.  If not, see <http://www.gnu.org/licenses/>.
 # ----------------------------------------------------------------------------
 #
 """Module containing simple comparison check."""
-from typing import Any, Dict, Hashable, List
+import warnings
+from typing import Any, Callable, Dict, Hashable, List, Union
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import torch
-from ignite.metrics import Fbeta
+from ignite.metrics import Fbeta, Metric
 
 from deepchecks.core import CheckResult, ConditionCategory, ConditionResult, DatasetKind
 from deepchecks.core.errors import DeepchecksValueError
 from deepchecks.utils import plot
 from deepchecks.utils.metrics import get_gain
 from deepchecks.utils.strings import format_percent
 from deepchecks.vision import Batch, Context, TrainTestCheck
@@ -77,14 +78,15 @@
         are ignored.
 
     """
 
     _state: Dict[Hashable, Any] = {}
 
     def __init__(self,
+                 scorers: Union[Dict[str, Union[Metric, Callable, str]], List[Any]] = None,
                  strategy: str = 'most_frequent',
                  alternative_metrics=None,
                  n_to_show: int = 20,
                  show_only: str = 'largest',
                  metric_to_show_by: str = None,
                  class_list_to_show: List[int] = None,
                  **kwargs):
@@ -92,15 +94,20 @@
         self.strategy = strategy
 
         if self.strategy not in _allowed_strategies:
             raise DeepchecksValueError(
                 f'Unknown strategy type: {self.strategy}, expected one of{_allowed_strategies}.'
             )
 
-        self.alternative_metrics = alternative_metrics
+        if alternative_metrics is not None:
+            warnings.warn(f'{self.__class__.__name__}: alternative_metrics is deprecated. Please use scorers instead.',
+                          DeprecationWarning)
+            self.alternative_metrics = alternative_metrics
+        else:
+            self.alternative_metrics = scorers
         self.n_to_show = n_to_show
         self.class_list_to_show = class_list_to_show
 
         if self.class_list_to_show is None:
             if show_only not in ['largest', 'smallest', 'random', 'best', 'worst']:
                 raise DeepchecksValueError(f'Invalid value for show_only: {show_only}. Should be one of: '
                                            f'["largest", "smallest", "random", "best", "worst"]')
```

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/single_dataset_performance.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/single_dataset_performance.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/model_evaluation/train_test_prediction_drift.py` & `deepchecks-0.9.2/deepchecks/vision/checks/model_evaluation/train_test_prediction_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/heatmap_comparison.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/heatmap_comparison.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/image_dataset_drift.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/image_dataset_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/image_property_drift.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/image_property_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/new_labels.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/new_labels.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/property_label_correlation_change.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/property_label_correlation_change.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/similar_image_leakage.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/similar_image_leakage.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/checks/train_test_validation/train_test_label_drift.py` & `deepchecks-0.9.2/deepchecks/vision/checks/train_test_validation/train_test_label_drift.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/classification_data.py` & `deepchecks-0.9.2/deepchecks/vision/classification_data.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/context.py` & `deepchecks-0.9.2/deepchecks/vision/context.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/classification/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/classification/mnist.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/classification/mnist.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/detection/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/detection/coco.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/detection/coco.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/detection/yolo_to_coco.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/detection/yolo_to_coco.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/segmentation/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/datasets/segmentation/segmentation_coco.py` & `deepchecks-0.9.2/deepchecks/vision/datasets/segmentation/segmentation_coco.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/detection_data.py` & `deepchecks-0.9.2/deepchecks/vision/detection_data.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/confusion_matrix_counts_metrics.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/confusion_matrix_counts_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/custom_scorer.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/custom_scorer.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,9 +89,11 @@
         """Compute metric value."""
         y_proba = np.concatenate(self._y_proba)
         y = np.concatenate(self._y)
 
         dummy_dataset = Dataset(df=pd.DataFrame(y_proba), label=y, cat_features=[])
         dummy_model = _DummyModel(test=dummy_dataset, y_proba_test=y_proba)
 
-        deep_checks_scorer = DeepcheckScorer(self.scorer, possible_classes=list(range(y_proba.shape[1])))
+        classes = list(range(y_proba.shape[1]))
+
+        deep_checks_scorer = DeepcheckScorer(self.scorer, model_classes=classes, observed_classes=classes)
         return deep_checks_scorer(dummy_model, dummy_dataset)
```

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/detection_precision_recall.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/detection_precision_recall.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/detection_tp_fp_fn_calc.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/detection_tp_fp_fn_calc.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/iou_utils.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/iou_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/metric_mixin.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/metric_mixin.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/scorers.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/scorers.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,16 +209,18 @@
 
     for metric, scores in results.items():
         if isinstance(scores, Number):
             result_list.append([metric, pd.NA, pd.NA, scores])
         elif len(scores) == 1:
             score = scores[0].item() if isinstance(scores[0], torch.Tensor) else scores[0]
             result_list.append([metric, pd.NA, pd.NA, score])
-        elif isinstance(scores, (torch.Tensor, list, np.ndarray)):
-            for class_id, class_score in enumerate(scores):
+        elif isinstance(scores, (torch.Tensor, list, np.ndarray, dict)):
+            # Deepchecks scorers returns classification class scores as dict
+            scores_iterator = scores.items() if isinstance(scores, dict) else enumerate(scores)
+            for class_id, class_score in scores_iterator:
                 # The data might contain fewer classes than the model was trained on. filtering out
                 # any class id which is not presented in the data.
                 if np.isnan(class_score) or class_id not in data_classes:
                     continue
                 score = class_score.item() if isinstance(class_score, torch.Tensor) else class_score
                 result_list.append([metric, class_id, dataset.label_id_to_name(class_id), score])
         else:
```

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/semantic_segmentation_metric_utils.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/semantic_segmentation_metric_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/metrics_utils/semantic_segmentation_metrics.py` & `deepchecks-0.9.2/deepchecks/vision/metrics_utils/semantic_segmentation_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/segmentation_data.py` & `deepchecks-0.9.2/deepchecks/vision/segmentation_data.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/simple_classification_data.py` & `deepchecks-0.9.2/deepchecks/vision/simple_classification_data.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/suite.py` & `deepchecks-0.9.2/deepchecks/vision/suite.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/suites/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/suites/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/suites/default_suites.py` & `deepchecks-0.9.2/deepchecks/vision/suites/default_suites.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/task_type.py` & `deepchecks-0.9.2/deepchecks/vision/task_type.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/__init__.py` & `deepchecks-0.9.2/deepchecks/vision/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/detection_formatters.py` & `deepchecks-0.9.2/deepchecks/vision/utils/detection_formatters.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/image_functions.py` & `deepchecks-0.9.2/deepchecks/vision/utils/image_functions.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/image_properties.py` & `deepchecks-0.9.2/deepchecks/vision/utils/image_properties.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/label_prediction_properties.py` & `deepchecks-0.9.2/deepchecks/vision/utils/label_prediction_properties.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/property_label_correlation_utils.py` & `deepchecks-0.9.2/deepchecks/vision/utils/property_label_correlation_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/test_utils.py` & `deepchecks-0.9.2/deepchecks/vision/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/transformations.py` & `deepchecks-0.9.2/deepchecks/vision/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/validation.py` & `deepchecks-0.9.2/deepchecks/vision/utils/validation.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/utils/vision_properties.py` & `deepchecks-0.9.2/deepchecks/vision/utils/vision_properties.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks/vision/vision_data.py` & `deepchecks-0.9.2/deepchecks/vision/vision_data.py`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks.egg-info/PKG-INFO` & `deepchecks-0.9.2/deepchecks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deepchecks
-Version: 0.9.1
+Version: 0.9.2
 Summary: Package for validating your machine learning model and data
 Home-page: https://github.com/deepchecks/deepchecks
 Author: deepchecks
 Author-email: info@deepchecks.com
 License: UNKNOWN
-Download-URL: https://github.com/deepchecks/deepchecks/releases/download/0.9.1/deepchecks-0.9.1.tar.gz
+Download-URL: https://github.com/deepchecks/deepchecks/releases/download/0.9.2/deepchecks-0.9.2.tar.gz
 Project-URL: Documentation, https://docs.deepchecks.com
 Project-URL: Bug Reports, https://github.com/deepchecks/deepchecks
 Project-URL: Source, https://github.com/deepchecks/deepchecks
 Project-URL: Contribute!, https://github.com/deepchecks/deepchecks/blob/master/CONTRIBUTING.md
 Keywords: Software Development,Machine Learning
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `deepchecks-0.9.1/deepchecks.egg-info/SOURCES.txt` & `deepchecks-0.9.2/deepchecks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/deepchecks.egg-info/requires.txt` & `deepchecks-0.9.2/deepchecks.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 jsonpickle>=2
 PyNomaly>=0.3.3
 typing_extensions>=4.0.0
 tqdm>=4.62.3
 category-encoders>=2.3.0
 statsmodels>=0.11.0
 scipy>=1.4.1
-plotly==5.5.0
+plotly>=5.5.0
 matplotlib>=3.3.4
 pyzmq<24.0.0
 
 [:python_version < "3.7"]
 dataclasses>=0.6
 
 [:python_version < "3.8"]
```

### Comparing `deepchecks-0.9.1/requirements/dev-requirements.txt` & `deepchecks-0.9.2/requirements/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `deepchecks-0.9.1/requirements/requirements.txt` & `deepchecks-0.9.2/requirements/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,12 +22,11 @@
 importlib_metadata>=1.4; python_version < '3.8'
 
 # Category encoder depends on old statsmodels version which raises pandas warning. until dependency in category-encoders
 # is updated, explicitly add it here
 statsmodels>=0.11.0
 scipy>=1.4.1
 dataclasses>=0.6; python_version < '3.7'
-# jupyterlab-plotly extension that is used to display plotly figures in jupyterlab env
-# is incompatiable with plotly version >5.5.0 therefore sticking to the version 5.5.0 for now
-plotly==5.5.0
+# jupyterlab-plotly extension that is used to display plotly figures
+plotly>=5.5.0
 matplotlib>=3.3.4
 pyzmq<24.0.0
```

### Comparing `deepchecks-0.9.1/setup.py` & `deepchecks-0.9.2/setup.py`

 * *Files identical despite different names*

