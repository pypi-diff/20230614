# Comparing `tmp/tsfresh-0.8.1.tar.gz` & `tmp/tsfresh-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tsfresh-0.8.1.tar", last modified: Wed Jun 21 17:24:06 2017, max compression
+gzip compressed data, was "dist/tsfresh-0.9.0.tar", last modified: Wed Aug  2 12:41:39 2017, max compression
```

## Comparing `tsfresh-0.8.1.tar` & `tsfresh-0.9.0.tar`

### file list

```diff
@@ -1,134 +1,146 @@
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/
--rw-r--r--   0 mchrist    (502) staff       (20)      875 2017-02-15 11:25:49.000000 tsfresh-0.8.1/.coveragerc
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/.github/
--rw-r--r--   0 mchrist    (502) staff       (20)      545 2017-05-20 16:32:19.000000 tsfresh-0.8.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 mchrist    (502) staff       (20)     1348 2017-06-11 20:51:57.000000 tsfresh-0.8.1/.travis.yml
--rw-r--r--   0 mchrist    (502) staff       (20)      364 2017-02-15 11:25:49.000000 tsfresh-0.8.1/AUTHORS.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     3946 2017-06-21 16:34:27.000000 tsfresh-0.8.1/CHANGES.rst
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/docs/
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/docs/_static/
--rw-r--r--   0 mchrist    (502) staff       (20)       18 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/_static/.gitignore
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/docs/api/
--rw-r--r--   0 mchrist    (502) staff       (20)      101 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/api/modules.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      484 2017-05-28 10:56:44.000000 tsfresh-0.8.1/docs/api/tests.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      289 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/api/tsfresh.convenience.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      406 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/api/tsfresh.examples.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      565 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/api/tsfresh.feature_extraction.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      577 2017-05-28 10:56:44.000000 tsfresh-0.8.1/docs/api/tsfresh.feature_selection.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      288 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/api/tsfresh.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      757 2017-06-01 14:46:24.000000 tsfresh-0.8.1/docs/api/tsfresh.transformers.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      389 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/api/tsfresh.utilities.rst
--rw-r--r--   0 mchrist    (502) staff       (20)       41 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/authors.rst
--rw-r--r--   0 mchrist    (502) staff       (20)       41 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/changes.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     8750 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/conf.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/docs/images/
--rw-r--r--   0 mchrist    (502) staff       (20)   124735 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/images/feature_extraction_process_20160815_mc_1.png
--rw-r--r--   0 mchrist    (502) staff       (20)    69041 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/images/introduction_ts_exa.png
--rw-r--r--   0 mchrist    (502) staff       (20)    95648 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/images/introduction_ts_exa_features.png
--rw-r--r--   0 mchrist    (502) staff       (20)    58875 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/images/ts_example_robot_failures_fail.png
--rw-r--r--   0 mchrist    (502) staff       (20)    50238 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/images/ts_example_robot_failures_nofail.png
--rw-r--r--   0 mchrist    (502) staff       (20)     1499 2017-05-28 10:56:44.000000 tsfresh-0.8.1/docs/index.rst
--rw-r--r--   0 mchrist    (502) staff       (20)       74 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/license.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     6763 2017-02-15 11:25:49.000000 tsfresh-0.8.1/docs/Makefile
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/docs/text/
--rw-r--r--   0 mchrist    (502) staff       (20)     8089 2017-05-20 16:32:19.000000 tsfresh-0.8.1/docs/text/data_formats.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     1857 2017-05-29 08:41:57.000000 tsfresh-0.8.1/docs/text/faq.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     1908 2017-05-28 10:56:44.000000 tsfresh-0.8.1/docs/text/feature_calculation.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     6478 2017-05-29 08:41:57.000000 tsfresh-0.8.1/docs/text/feature_extraction_settings.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     3118 2017-05-20 16:32:19.000000 tsfresh-0.8.1/docs/text/feature_filtering.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     4875 2017-05-28 10:56:44.000000 tsfresh-0.8.1/docs/text/how_to_add_custom_feature.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     2770 2017-05-28 10:56:44.000000 tsfresh-0.8.1/docs/text/how_to_contribute.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     2533 2017-05-20 16:32:19.000000 tsfresh-0.8.1/docs/text/introduction.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     3031 2017-05-28 10:56:44.000000 tsfresh-0.8.1/docs/text/parallelization.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     4564 2017-05-20 16:32:19.000000 tsfresh-0.8.1/docs/text/quick_start.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     5823 2017-05-20 16:32:19.000000 tsfresh-0.8.1/docs/text/rolling.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     3249 2017-05-20 16:38:10.000000 tsfresh-0.8.1/docs/text/sklearn_transformers.rst
--rw-r--r--   0 mchrist    (502) staff       (20)     1091 2017-02-15 11:25:49.000000 tsfresh-0.8.1/LICENSE.txt
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/notebooks/
--rw-r--r--   0 mchrist    (502) staff       (20)    47822 2017-05-28 11:41:53.000000 tsfresh-0.8.1/notebooks/basic_pipeline_example.ipynb
--rw-r--r--   0 mchrist    (502) staff       (20)   321896 2017-05-28 11:41:53.000000 tsfresh-0.8.1/notebooks/compare-runtimes-of-feature-calculators.ipynb
--rw-r--r--   0 mchrist    (502) staff       (20)    76773 2017-05-28 11:41:53.000000 tsfresh-0.8.1/notebooks/friedrich_coefficients.ipynb
--rw-r--r--   0 mchrist    (502) staff       (20)    62687 2017-06-21 17:05:13.000000 tsfresh-0.8.1/notebooks/human_activity_recognition_multi_class_example.ipynb
--rw-r--r--   0 mchrist    (502) staff       (20)    38021 2017-05-28 11:41:53.000000 tsfresh-0.8.1/notebooks/pipeline_with_two_datasets.ipynb
--rw-r--r--   0 mchrist    (502) staff       (20)   200817 2017-06-02 15:19:34.000000 tsfresh-0.8.1/notebooks/robot_failure_example.ipynb
--rw-r--r--   0 mchrist    (502) staff       (20)    53571 2017-05-30 11:44:59.000000 tsfresh-0.8.1/notebooks/the-fc_parameters-extraction-dictionary.ipynb
--rw-r--r--   0 mchrist    (502) staff       (20)       63 2017-05-20 16:32:19.000000 tsfresh-0.8.1/notebooks-requirements.txt
--rw-r--r--   0 mchrist    (502) staff       (20)     6160 2017-06-21 17:24:06.000000 tsfresh-0.8.1/PKG-INFO
--rw-r--r--   0 mchrist    (502) staff       (20)      403 2017-02-15 11:25:49.000000 tsfresh-0.8.1/pypi_index.zip
--rw-r--r--   0 mchrist    (502) staff       (20)       51 2017-02-15 11:25:49.000000 tsfresh-0.8.1/rdocs-requirements.txt
--rw-r--r--   0 mchrist    (502) staff       (20)     4419 2017-05-20 16:32:19.000000 tsfresh-0.8.1/README.md
--rw-r--r--   0 mchrist    (502) staff       (20)     4587 2017-02-15 11:25:49.000000 tsfresh-0.8.1/README.rst
--rw-r--r--   0 mchrist    (502) staff       (20)      152 2017-02-15 11:25:49.000000 tsfresh-0.8.1/requirements.txt
--rw-r--r--   0 mchrist    (502) staff       (20)     1106 2017-06-21 17:24:06.000000 tsfresh-0.8.1/setup.cfg
--rw-r--r--   0 mchrist    (502) staff       (20)      619 2017-06-21 17:19:33.000000 tsfresh-0.8.1/setup.py
--rw-r--r--   0 mchrist    (502) staff       (20)       77 2017-02-15 11:25:49.000000 tsfresh-0.8.1/test-requirements.txt
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tests/
--rw-r--r--   0 mchrist    (502) staff       (20)        0 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tests/__init__.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tests/examples/
--rw-r--r--   0 mchrist    (502) staff       (20)     3845 2017-06-21 07:08:20.000000 tsfresh-0.8.1/tests/examples/test_driftbif_simulation.py
--rw-r--r--   0 mchrist    (502) staff       (20)      920 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tests/examples/test_har_dataset.py
--rw-r--r--   0 mchrist    (502) staff       (20)     1190 2017-05-20 16:32:19.000000 tsfresh-0.8.1/tests/examples/test_robot_execution_failures.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tests/feature_extraction/
--rw-r--r--   0 mchrist    (502) staff       (20)    13356 2017-06-21 07:08:20.000000 tsfresh-0.8.1/tests/feature_extraction/test_extraction.py
--rw-r--r--   0 mchrist    (502) staff       (20)    41810 2017-06-11 20:51:57.000000 tsfresh-0.8.1/tests/feature_extraction/test_feature_calculations.py
--rw-r--r--   0 mchrist    (502) staff       (20)     6608 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/feature_extraction/test_settings.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tests/feature_selection/
--rw-r--r--   0 mchrist    (502) staff       (20)    15145 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/feature_selection/test_feature_selectors.py
--rw-r--r--   0 mchrist    (502) staff       (20)     1073 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tests/feature_selection/test_selection.py
--rw-r--r--   0 mchrist    (502) staff       (20)     2026 2017-05-20 16:32:19.000000 tsfresh-0.8.1/tests/fixtures.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tests/scripts/
--rw-r--r--   0 mchrist    (502) staff       (20)     4224 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tests/scripts/test_run_tsfresh.py
--rw-r--r--   0 mchrist    (502) staff       (20)    10810 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/test_feature_significance.py
--rw-r--r--   0 mchrist    (502) staff       (20)     3908 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/test_relevant_feature_extraction.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tests/transformers/
--rw-r--r--   0 mchrist    (502) staff       (20)     3148 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/transformers/test_feature_augmenter.py
--rw-r--r--   0 mchrist    (502) staff       (20)     4245 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/transformers/test_feature_selector.py
--rw-r--r--   0 mchrist    (502) staff       (20)     3710 2017-05-20 16:32:19.000000 tsfresh-0.8.1/tests/transformers/test_full_pipeline.py
--rw-r--r--   0 mchrist    (502) staff       (20)     6606 2017-06-01 14:46:24.000000 tsfresh-0.8.1/tests/transformers/test_per_column_imputer.py
--rw-r--r--   0 mchrist    (502) staff       (20)     4355 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/transformers/test_relevant_feature_extractor.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tests/utilities/
--rw-r--r--   0 mchrist    (502) staff       (20)    29848 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tests/utilities/test_dataframe_functions.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/
--rw-r--r--   0 mchrist    (502) staff       (20)      946 2017-05-20 16:32:19.000000 tsfresh-0.8.1/tsfresh/__init__.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/convenience/
--rw-r--r--   0 mchrist    (502) staff       (20)      132 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/convenience/__init__.py
--rw-r--r--   0 mchrist    (502) staff       (20)     8638 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/convenience/relevant_extraction.py
--rw-r--r--   0 mchrist    (502) staff       (20)      629 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/defaults.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/examples/
--rw-r--r--   0 mchrist    (502) staff       (20)      405 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/examples/__init__.py
--rw-r--r--   0 mchrist    (502) staff       (20)     6464 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/examples/driftbif_simulation.py
--rw-r--r--   0 mchrist    (502) staff       (20)     2785 2017-06-11 20:51:57.000000 tsfresh-0.8.1/tsfresh/examples/har_dataset.py
--rw-r--r--   0 mchrist    (502) staff       (20)     4375 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/examples/robot_execution_failures.py
--rw-r--r--   0 mchrist    (502) staff       (20)     1446 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/examples/test_tsfresh_baseline_dataset.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/feature_extraction/
--rw-r--r--   0 mchrist    (502) staff       (20)      307 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/feature_extraction/__init__.py
--rw-r--r--   0 mchrist    (502) staff       (20)    23499 2017-06-21 07:08:20.000000 tsfresh-0.8.1/tsfresh/feature_extraction/extraction.py
--rw-r--r--   0 mchrist    (502) staff       (20)    47047 2017-06-11 20:51:57.000000 tsfresh-0.8.1/tsfresh/feature_extraction/feature_calculators.py
--rw-r--r--   0 mchrist    (502) staff       (20)    12912 2017-06-21 14:08:32.000000 tsfresh-0.8.1/tsfresh/feature_extraction/settings.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/feature_selection/
--rw-r--r--   0 mchrist    (502) staff       (20)      586 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/feature_selection/__init__.py
--rw-r--r--   0 mchrist    (502) staff       (20)    11669 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/feature_selection/feature_selector.py
--rw-r--r--   0 mchrist    (502) staff       (20)     6069 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/feature_selection/selection.py
--rw-r--r--   0 mchrist    (502) staff       (20)     7943 2017-06-21 07:08:20.000000 tsfresh-0.8.1/tsfresh/feature_selection/significance_tests.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/scripts/
--rw-r--r--   0 mchrist    (502) staff       (20)        0 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/scripts/__init__.py
--rwxr-xr-x   0 mchrist    (502) staff       (20)  6041350 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/scripts/data.txt
--rw-r--r--   0 mchrist    (502) staff       (20)     4547 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/scripts/run_tsfresh.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/transformers/
--rw-r--r--   0 mchrist    (502) staff       (20)      413 2017-06-01 14:46:24.000000 tsfresh-0.8.1/tsfresh/transformers/__init__.py
--rw-r--r--   0 mchrist    (502) staff       (20)    10632 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/transformers/feature_augmenter.py
--rw-r--r--   0 mchrist    (502) staff       (20)     7139 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/transformers/feature_selector.py
--rw-r--r--   0 mchrist    (502) staff       (20)     5325 2017-06-01 14:46:24.000000 tsfresh-0.8.1/tsfresh/transformers/per_column_imputer.py
--rw-r--r--   0 mchrist    (502) staff       (20)    18924 2017-05-28 10:56:44.000000 tsfresh-0.8.1/tsfresh/transformers/relevant_feature_augmenter.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh/utilities/
--rw-r--r--   0 mchrist    (502) staff       (20)      137 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/utilities/__init__.py
--rw-r--r--   0 mchrist    (502) staff       (20)    20411 2017-05-20 16:32:19.000000 tsfresh-0.8.1/tsfresh/utilities/dataframe_functions.py
--rw-r--r--   0 mchrist    (502) staff       (20)     2128 2017-02-15 11:25:49.000000 tsfresh-0.8.1/tsfresh/utilities/profiling.py
-drwxr-xr-x   0 mchrist    (502) staff       (20)        0 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh.egg-info/
--rw-r--r--   0 mchrist    (502) staff       (20)        1 2017-06-21 17:24:05.000000 tsfresh-0.8.1/tsfresh.egg-info/dependency_links.txt
--rw-r--r--   0 mchrist    (502) staff       (20)       66 2017-06-21 17:24:05.000000 tsfresh-0.8.1/tsfresh.egg-info/entry_points.txt
--rw-r--r--   0 mchrist    (502) staff       (20)        1 2017-06-21 17:24:05.000000 tsfresh-0.8.1/tsfresh.egg-info/not-zip-safe
--rw-r--r--   0 mchrist    (502) staff       (20)     6160 2017-06-21 17:24:05.000000 tsfresh-0.8.1/tsfresh.egg-info/PKG-INFO
--rw-r--r--   0 mchrist    (502) staff       (20)      152 2017-06-21 17:24:05.000000 tsfresh-0.8.1/tsfresh.egg-info/requires.txt
--rw-r--r--   0 mchrist    (502) staff       (20)     3591 2017-06-21 17:24:06.000000 tsfresh-0.8.1/tsfresh.egg-info/SOURCES.txt
--rw-r--r--   0 mchrist    (502) staff       (20)        8 2017-06-21 17:24:05.000000 tsfresh-0.8.1/tsfresh.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:39.000000 tsfresh-0.9.0/
+-rw-r--r--   0 max        (501) staff       (20)     1003 2017-07-21 16:31:02.000000 tsfresh-0.9.0/.coveragerc
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/.github/
+-rw-r--r--   0 max        (501) staff       (20)      545 2017-07-10 05:53:52.000000 tsfresh-0.9.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 max        (501) staff       (20)     1361 2017-07-16 12:50:14.000000 tsfresh-0.9.0/.travis.yml
+-rw-r--r--   0 max        (501) staff       (20)      364 2017-07-10 05:53:52.000000 tsfresh-0.9.0/AUTHORS.rst
+-rw-r--r--   0 max        (501) staff       (20)     5428 2017-08-02 12:39:11.000000 tsfresh-0.9.0/CHANGES.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/docs/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/docs/_static/
+-rw-r--r--   0 max        (501) staff       (20)       18 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/_static/.gitignore
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/docs/api/
+-rw-r--r--   0 max        (501) staff       (20)      101 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/modules.rst
+-rw-r--r--   0 max        (501) staff       (20)      484 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/tests.rst
+-rw-r--r--   0 max        (501) staff       (20)      289 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/tsfresh.convenience.rst
+-rw-r--r--   0 max        (501) staff       (20)      406 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/tsfresh.examples.rst
+-rw-r--r--   0 max        (501) staff       (20)      565 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/tsfresh.feature_extraction.rst
+-rw-r--r--   0 max        (501) staff       (20)      815 2017-08-02 12:33:45.000000 tsfresh-0.9.0/docs/api/tsfresh.feature_selection.rst
+-rw-r--r--   0 max        (501) staff       (20)      288 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/tsfresh.rst
+-rw-r--r--   0 max        (501) staff       (20)      757 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/tsfresh.transformers.rst
+-rw-r--r--   0 max        (501) staff       (20)      389 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/api/tsfresh.utilities.rst
+-rw-r--r--   0 max        (501) staff       (20)       41 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/authors.rst
+-rw-r--r--   0 max        (501) staff       (20)       41 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/changes.rst
+-rw-r--r--   0 max        (501) staff       (20)     8750 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/conf.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/docs/images/
+-rw-r--r--   0 max        (501) staff       (20)   124735 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/images/feature_extraction_process_20160815_mc_1.png
+-rw-r--r--   0 max        (501) staff       (20)    69041 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/images/introduction_ts_exa.png
+-rw-r--r--   0 max        (501) staff       (20)    95648 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/images/introduction_ts_exa_features.png
+-rw-r--r--   0 max        (501) staff       (20)    19480 2017-07-27 20:06:27.000000 tsfresh-0.9.0/docs/images/rolling_mechanism_1.png
+-rw-r--r--   0 max        (501) staff       (20)    34825 2017-07-27 20:06:27.000000 tsfresh-0.9.0/docs/images/rolling_mechanism_2.png
+-rw-r--r--   0 max        (501) staff       (20)     2297 2017-07-27 20:06:27.000000 tsfresh-0.9.0/docs/images/rolling_mechanism_drawio_template.xml
+-rw-r--r--   0 max        (501) staff       (20)    58875 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/images/ts_example_robot_failures_fail.png
+-rw-r--r--   0 max        (501) staff       (20)    50238 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/images/ts_example_robot_failures_nofail.png
+-rw-r--r--   0 max        (501) staff       (20)     1545 2017-07-27 20:06:27.000000 tsfresh-0.9.0/docs/index.rst
+-rw-r--r--   0 max        (501) staff       (20)       74 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/license.rst
+-rw-r--r--   0 max        (501) staff       (20)     6763 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/Makefile
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/docs/text/
+-rw-r--r--   0 max        (501) staff       (20)     8089 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/text/data_formats.rst
+-rw-r--r--   0 max        (501) staff       (20)     1900 2017-07-27 20:06:27.000000 tsfresh-0.9.0/docs/text/faq.rst
+-rw-r--r--   0 max        (501) staff       (20)     1908 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/text/feature_calculation.rst
+-rw-r--r--   0 max        (501) staff       (20)     6497 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/text/feature_extraction_settings.rst
+-rw-r--r--   0 max        (501) staff       (20)     3193 2017-08-02 12:33:45.000000 tsfresh-0.9.0/docs/text/feature_filtering.rst
+-rw-r--r--   0 max        (501) staff       (20)    10379 2017-07-27 20:06:27.000000 tsfresh-0.9.0/docs/text/forecasting.rst
+-rw-r--r--   0 max        (501) staff       (20)     4999 2017-07-23 19:43:04.000000 tsfresh-0.9.0/docs/text/how_to_add_custom_feature.rst
+-rw-r--r--   0 max        (501) staff       (20)     2770 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/text/how_to_contribute.rst
+-rw-r--r--   0 max        (501) staff       (20)     2533 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/text/introduction.rst
+-rw-r--r--   0 max        (501) staff       (20)     1611 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/text/parallelization.rst
+-rw-r--r--   0 max        (501) staff       (20)     4816 2017-07-28 07:31:25.000000 tsfresh-0.9.0/docs/text/quick_start.rst
+-rw-r--r--   0 max        (501) staff       (20)     3249 2017-07-10 05:53:52.000000 tsfresh-0.9.0/docs/text/sklearn_transformers.rst
+-rw-r--r--   0 max        (501) staff       (20)     1091 2017-07-10 05:53:52.000000 tsfresh-0.9.0/LICENSE.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/notebooks/
+-rw-r--r--   0 max        (501) staff       (20)    48327 2017-08-02 12:33:45.000000 tsfresh-0.9.0/notebooks/basic_pipeline_example.ipynb
+-rw-r--r--   0 max        (501) staff       (20)   321896 2017-07-10 05:53:52.000000 tsfresh-0.9.0/notebooks/compare-runtimes-of-feature-calculators.ipynb
+-rw-r--r--   0 max        (501) staff       (20)    77284 2017-07-16 12:50:14.000000 tsfresh-0.9.0/notebooks/friedrich_coefficients.ipynb
+-rw-r--r--   0 max        (501) staff       (20)    58648 2017-07-28 07:31:25.000000 tsfresh-0.9.0/notebooks/human_activity_recognition_multi_class_example.ipynb
+-rw-r--r--   0 max        (501) staff       (20)  1204503 2017-07-22 12:42:04.000000 tsfresh-0.9.0/notebooks/inspect_dft_features.ipynb
+-rw-r--r--   0 max        (501) staff       (20)     8015 2017-07-22 12:42:04.000000 tsfresh-0.9.0/notebooks/pipeline_with_two_datasets.ipynb
+-rw-r--r--   0 max        (501) staff       (20)   128392 2017-07-22 13:20:30.000000 tsfresh-0.9.0/notebooks/robot_failure_example.ipynb
+-rw-r--r--   0 max        (501) staff       (20)   103363 2017-07-28 07:31:25.000000 tsfresh-0.9.0/notebooks/the-fc_parameters-extraction-dictionary.ipynb
+-rw-r--r--   0 max        (501) staff       (20)   154533 2017-07-27 20:06:27.000000 tsfresh-0.9.0/notebooks/timeseries_forecasting_basic_example.ipynb
+-rw-r--r--   0 max        (501) staff       (20)   237853 2017-07-27 20:06:27.000000 tsfresh-0.9.0/notebooks/timeseries_forecasting_google_stock.ipynb
+-rw-r--r--   0 max        (501) staff       (20)     6160 2017-08-02 12:41:39.000000 tsfresh-0.9.0/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      403 2017-07-10 05:53:52.000000 tsfresh-0.9.0/pypi_index.zip
+-rw-r--r--   0 max        (501) staff       (20)       51 2017-07-10 05:53:52.000000 tsfresh-0.9.0/rdocs-requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)     4419 2017-07-10 05:53:52.000000 tsfresh-0.9.0/README.md
+-rw-r--r--   0 max        (501) staff       (20)     4587 2017-07-10 05:53:52.000000 tsfresh-0.9.0/README.rst
+-rw-r--r--   0 max        (501) staff       (20)      162 2017-07-27 20:06:27.000000 tsfresh-0.9.0/requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)     1106 2017-08-02 12:41:39.000000 tsfresh-0.9.0/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      619 2017-07-10 05:53:52.000000 tsfresh-0.9.0/setup.py
+-rw-r--r--   0 max        (501) staff       (20)      176 2017-07-27 20:06:27.000000 tsfresh-0.9.0/test-requirements.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tests/
+-rw-r--r--   0 max        (501) staff       (20)        0 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/__init__.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tests/examples/
+-rw-r--r--   0 max        (501) staff       (20)     3845 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/examples/test_driftbif_simulation.py
+-rw-r--r--   0 max        (501) staff       (20)      920 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/examples/test_har_dataset.py
+-rw-r--r--   0 max        (501) staff       (20)     1539 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/examples/test_robot_execution_failures.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tests/feature_extraction/
+-rw-r--r--   0 max        (501) staff       (20)     9142 2017-07-22 10:19:50.000000 tsfresh-0.9.0/tests/feature_extraction/test_extraction.py
+-rw-r--r--   0 max        (501) staff       (20)    50227 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/feature_extraction/test_feature_calculations.py
+-rw-r--r--   0 max        (501) staff       (20)     5824 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/feature_extraction/test_settings.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tests/feature_selection/
+-rw-r--r--   0 max        (501) staff       (20)     3312 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/feature_selection/test_checks.py
+-rw-r--r--   0 max        (501) staff       (20)     5600 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/feature_selection/test_relevance.py
+-rw-r--r--   0 max        (501) staff       (20)     1637 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/feature_selection/test_selection.py
+-rw-r--r--   0 max        (501) staff       (20)     7104 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/feature_selection/test_significance_tests.py
+-rw-r--r--   0 max        (501) staff       (20)     2026 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/fixtures.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tests/scripts/
+-rw-r--r--   0 max        (501) staff       (20)     4224 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/scripts/test_run_tsfresh.py
+-rw-r--r--   0 max        (501) staff       (20)    10902 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/test_feature_significance.py
+-rw-r--r--   0 max        (501) staff       (20)     2540 2017-07-22 12:42:04.000000 tsfresh-0.9.0/tests/test_notebooks.py
+-rw-r--r--   0 max        (501) staff       (20)     3908 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/test_relevant_feature_extraction.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tests/transformers/
+-rw-r--r--   0 max        (501) staff       (20)     3148 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/transformers/test_feature_augmenter.py
+-rw-r--r--   0 max        (501) staff       (20)     4245 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/transformers/test_feature_selector.py
+-rw-r--r--   0 max        (501) staff       (20)     2589 2017-07-23 19:43:04.000000 tsfresh-0.9.0/tests/transformers/test_full_pipeline.py
+-rw-r--r--   0 max        (501) staff       (20)     6606 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tests/transformers/test_per_column_imputer.py
+-rw-r--r--   0 max        (501) staff       (20)     4513 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tests/transformers/test_relevant_feature_augmenter.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tests/utilities/
+-rw-r--r--   0 max        (501) staff       (20)    32778 2017-07-28 07:31:25.000000 tsfresh-0.9.0/tests/utilities/test_dataframe_functions.py
+-rw-r--r--   0 max        (501) staff       (20)      892 2017-07-22 12:42:04.000000 tsfresh-0.9.0/tests/utilities/test_string_manipilations.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh/
+-rw-r--r--   0 max        (501) staff       (20)      946 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/__init__.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh/convenience/
+-rw-r--r--   0 max        (501) staff       (20)      132 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/convenience/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     8319 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/convenience/relevant_extraction.py
+-rw-r--r--   0 max        (501) staff       (20)      651 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/defaults.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh/examples/
+-rw-r--r--   0 max        (501) staff       (20)      405 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/examples/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     6464 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/examples/driftbif_simulation.py
+-rw-r--r--   0 max        (501) staff       (20)     2863 2017-07-22 12:42:04.000000 tsfresh-0.9.0/tsfresh/examples/har_dataset.py
+-rw-r--r--   0 max        (501) staff       (20)     4693 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/examples/robot_execution_failures.py
+-rw-r--r--   0 max        (501) staff       (20)     1446 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/examples/test_tsfresh_baseline_dataset.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh/feature_extraction/
+-rw-r--r--   0 max        (501) staff       (20)      307 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/feature_extraction/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    13056 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/feature_extraction/extraction.py
+-rw-r--r--   0 max        (501) staff       (20)    51551 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/feature_extraction/feature_calculators.py
+-rw-r--r--   0 max        (501) staff       (20)     8922 2017-07-28 08:00:12.000000 tsfresh-0.9.0/tsfresh/feature_extraction/settings.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh/feature_selection/
+-rw-r--r--   0 max        (501) staff       (20)      586 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/feature_selection/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     2719 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/feature_selection/benjamini_hochberg_test.py
+-rw-r--r--   0 max        (501) staff       (20)    11065 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/feature_selection/relevance.py
+-rw-r--r--   0 max        (501) staff       (20)     6938 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/feature_selection/selection.py
+-rw-r--r--   0 max        (501) staff       (20)     7943 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/feature_selection/significance_tests.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:39.000000 tsfresh-0.9.0/tsfresh/scripts/
+-rw-r--r--   0 max        (501) staff       (20)        0 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/scripts/__init__.py
+-rwxr-xr-x   0 max        (501) staff       (20)  6041350 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/scripts/data.txt
+-rw-r--r--   0 max        (501) staff       (20)     4547 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/scripts/run_tsfresh.py
+-rw-r--r--   0 max        (501) staff       (20)     2172 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/scripts/test_timing.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:39.000000 tsfresh-0.9.0/tsfresh/transformers/
+-rw-r--r--   0 max        (501) staff       (20)      413 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/transformers/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    10137 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/transformers/feature_augmenter.py
+-rw-r--r--   0 max        (501) staff       (20)     7947 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/transformers/feature_selector.py
+-rw-r--r--   0 max        (501) staff       (20)     5325 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/transformers/per_column_imputer.py
+-rw-r--r--   0 max        (501) staff       (20)    18567 2017-08-02 12:33:45.000000 tsfresh-0.9.0/tsfresh/transformers/relevant_feature_augmenter.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:39.000000 tsfresh-0.9.0/tsfresh/utilities/
+-rw-r--r--   0 max        (501) staff       (20)      137 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/utilities/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    22066 2017-07-28 07:31:25.000000 tsfresh-0.9.0/tsfresh/utilities/dataframe_functions.py
+-rw-r--r--   0 max        (501) staff       (20)     2128 2017-07-10 05:53:52.000000 tsfresh-0.9.0/tsfresh/utilities/profiling.py
+-rw-r--r--   0 max        (501) staff       (20)     2404 2017-07-22 12:42:04.000000 tsfresh-0.9.0/tsfresh/utilities/string_manipulation.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)        1 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       66 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/not-zip-safe
+-rw-r--r--   0 max        (501) staff       (20)     6160 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      152 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)     4101 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        8 2017-08-02 12:41:38.000000 tsfresh-0.9.0/tsfresh.egg-info/top_level.txt
```

### Comparing `tsfresh-0.8.1/.coveragerc` & `tsfresh-0.9.0/.coveragerc`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# .coveragerc to control coverage.py
-[run]
-branch = True
-source = tsfresh
-omit = tsfresh/utilities/profiling.py 
-       tsfresh/__init__.py
-       tsfresh/feature_extraction/__init__.py
-       tsfresh/example/__init__.py
-       tsfresh/utilities/__init__.py
-       tsfresh/transformers/__init__.py
-       tsfresh/convenience/__init__.py
-       tsfresh/examples/har_dataset.py
-       tsfresh/examples/robot_execution_failures.py
-
-[report]
-# Regexes for lines to exclude from consideration
-exclude_lines =
-    # Have to re-enable the standard pragma
-    pragma: no cover
-
-    # Don't complain about missing debug-only code:
-    def __repr__
-    if self\.debug
-
-    # Don't complain if tests don't hit defensive assertion code:
-    raise AssertionError
-    raise NotImplementedError
-
-    # Don't complain if non-runnable code isn't run:
-    if 0:
-    if __name__ == .__main__.:
+# .coveragerc to control coverage.py
+[run]
+branch = True
+source = tsfresh
+omit = tsfresh/utilities/profiling.py 
+       tsfresh/__init__.py
+       tsfresh/feature_extraction/__init__.py
+       tsfresh/example/__init__.py
+       tsfresh/utilities/__init__.py
+       tsfresh/transformers/__init__.py
+       tsfresh/convenience/__init__.py
+       tsfresh/examples/har_dataset.py
+       tsfresh/examples/robot_execution_failures.py
+       tsfresh/examples/test_tsfresh_baseline_dataset.py
+       tsfresh/scripts/test_timing.py
+
+[report]
+# Regexes for lines to exclude from consideration
+exclude_lines =
+    # Have to re-enable the standard pragma
+    pragma: no cover
+
+    # Don't complain about missing debug-only code:
+    def __repr__
+    if self\.debug
+
+    # Don't complain if tests don't hit defensive assertion code:
+    raise AssertionError
+    raise NotImplementedError
+
+    # Don't complain if non-runnable code isn't run:
+    if 0:
+    if __name__ == .__main__.:
```

### Comparing `tsfresh-0.8.1/.github/ISSUE_TEMPLATE.md` & `tsfresh-0.9.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/.travis.yml` & `tsfresh-0.9.0/.travis.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 - pip install --upgrade pip
 - pip install numpy
 - pip install scipy
 - pip install coveralls
 - pip install .
 - pip install -r requirements.txt
 - pip install -r test-requirements.txt
+- pip freeze
 env:
 - NUMBER_OF_CPUS=1
 script:
 # hack to set xdist to use only 1 node instead of 32
 - sed -i 's/\-n 4/\-n 1/g' setup.cfg
 - python setup.py test
 deploy:
```

### Comparing `tsfresh-0.8.1/docs/api/tsfresh.feature_extraction.rst` & `tsfresh-0.9.0/docs/api/tsfresh.feature_extraction.rst`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/api/tsfresh.feature_selection.rst` & `tsfresh-0.9.0/docs/api/tsfresh.transformers.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-feature_selection
-=================
+transformers
+============
 
-.. automodule:: tsfresh.feature_selection
+.. automodule:: tsfresh.transformers
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+feature_augmenter
+-----------------
+
+.. automodule:: tsfresh.transformers.feature_augmenter
     :members:
     :undoc-members:
     :show-inheritance:
 
 feature_selector
 ----------------
 
-.. automodule:: tsfresh.feature_selection.feature_selector
+.. automodule:: tsfresh.transformers.feature_selector
     :members:
     :undoc-members:
     :show-inheritance:
 
-selection
----------
+relevant_feature_augmenter
+--------------------------
 
-.. automodule:: tsfresh.feature_selection.selection
+.. automodule:: tsfresh.transformers.relevant_feature_augmenter
     :members:
     :undoc-members:
     :show-inheritance:
 
-significance_tests
-------------------
+per_column_imputer
+--------------------------
 
-.. automodule:: tsfresh.feature_selection.significance_tests
+.. automodule:: tsfresh.transformers.per_column_imputer
     :members:
     :undoc-members:
     :show-inheritance:
+
```

### Comparing `tsfresh-0.8.1/docs/conf.py` & `tsfresh-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/images/feature_extraction_process_20160815_mc_1.png` & `tsfresh-0.9.0/docs/images/feature_extraction_process_20160815_mc_1.png`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/images/introduction_ts_exa.png` & `tsfresh-0.9.0/docs/images/introduction_ts_exa.png`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/images/introduction_ts_exa_features.png` & `tsfresh-0.9.0/docs/images/introduction_ts_exa_features.png`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/images/ts_example_robot_failures_fail.png` & `tsfresh-0.9.0/docs/images/ts_example_robot_failures_fail.png`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/images/ts_example_robot_failures_nofail.png` & `tsfresh-0.9.0/docs/images/ts_example_robot_failures_nofail.png`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/Makefile` & `tsfresh-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/text/data_formats.rst` & `tsfresh-0.9.0/docs/text/data_formats.rst`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/text/faq.rst` & `tsfresh-0.9.0/docs/text/faq.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-FAQ
-===
-
-
-    1. **Does tsfresh support different time series lengths?**
-
-       Yes, it supports different time series lengths. However, some feature calculators can demand a minimal length
-       of the time series. If a shorter time series is passed to the calculator, a NaN is returned for those
-       features.
-
-
-
-    2. **Is it possible to extract features from rolling/shifted time series?**
-
-       Yes, the :func:`tsfresh.dataframe_functions.roll_time_series` function allows to conviniently create a rolled
-       time series datframe from your data. You just have to transform your data into one of the supported tsfresh
-       :ref:`data-formats-label`.
-       Then, the :func:`tsfresh.dataframe_functions.roll_time_series` give you a DataFrame with the rolled time series,
-       that you can pass to tsfresh.
-       On the following page you can find a detailed description: :ref:`rolling-label`.
-
-
-    3. **How can I use tsfresh with windows?**
-
-       We recommend to use `Anaconda <https://www.continuum.io/downloads#windows>`_. After installing, open the
-       Anaconda Prompt, create an environment and set up tsfresh
-       (Please be aware that we're using multiprocessing, which can be `problematic <http://stackoverflow.com/questions/18204782/runtimeerror-on-windows-trying-python-multiprocessing>`_.):
-
-       .. code:: Bash
-
-           conda create -n ENV_NAME python=VERSION
-           conda install -n ENV_NAME pip requests numpy pandas scipy statsmodels patsy scikit-learn future six tqdm
-           activate ENV_NAME
-           pip install tsfresh
-
-
-    4. **Does tsfresh support different sampling rates in the time series?**
-
-        Yes! The feature calculators in tsfresh do not care about the sampling frequency.
+FAQ
+===
+
+
+    1. **Does tsfresh support different time series lengths?**
+
+       Yes, it supports different time series lengths. However, some feature calculators can demand a minimal length
+       of the time series. If a shorter time series is passed to the calculator, a NaN is returned for those
+       features.
+
+
+
+    2. **Is it possible to extract features from rolling/shifted time series?**
+
+       Yes, the :func:`tsfresh.dataframe_functions.roll_time_series` function allows to conviniently create a rolled
+       time series datframe from your data. You just have to transform your data into one of the supported tsfresh
+       :ref:`data-formats-label`.
+       Then, the :func:`tsfresh.dataframe_functions.roll_time_series` give you a DataFrame with the rolled time series,
+       that you can pass to tsfresh.
+       On the following page you can find a detailed description: :ref:`forecasting-label`.
+
+
+    3. **How can I use tsfresh with windows?**
+
+       We recommend to use `Anaconda <https://www.continuum.io/downloads#windows>`_. After installing, open the
+       Anaconda Prompt, create an environment and set up tsfresh
+       (Please be aware that we're using multiprocessing, which can be `problematic <http://stackoverflow.com/questions/18204782/runtimeerror-on-windows-trying-python-multiprocessing>`_.):
+
+       .. code:: Bash
+
+           conda create -n ENV_NAME python=VERSION
+           conda install -n ENV_NAME pip requests numpy pandas scipy statsmodels patsy scikit-learn future six tqdm
+           activate ENV_NAME
+           pip install tsfresh
+
+
+    4. **Does tsfresh support different sampling rates in the time series?**
+
+        Yes! The feature calculators in tsfresh do not care about the sampling frequency.
         You will have to use the second input format, the stacked DataFramed (see :ref:`data-formats-label`)
```

### Comparing `tsfresh-0.8.1/docs/text/feature_calculation.rst` & `tsfresh-0.9.0/docs/text/feature_calculation.rst`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/text/feature_extraction_settings.rst` & `tsfresh-0.9.0/docs/text/feature_extraction_settings.rst`

 * *Files 2% similar despite different names*

```diff
@@ -119,11 +119,11 @@
     # X_tsfresh containes the extracted tsfresh features
     X_tsfresh = extract_features(...)
 
     # which are now filtered to only contain relevant features
     X_tsfresh_filtered = some_feature_selection(X_tsfresh, y, ....)
 
     # we can easily construct the corresponding settings object
-    kind_to_fc_parameters = tsfresh.settings.from_columns(X_tsfresh_filtered)
+    kind_to_fc_parameters = tsfresh.feature_extraction.settings.from_columns(X_tsfresh_filtered)
 
 this will construct you the `kind_to_fc_parameters` dictionary that corresponds to the features and parameters (!) from
 the tsfresh features that were filtered by the `some_feature_selection` feature selection algorithm.
```

### Comparing `tsfresh-0.8.1/docs/text/feature_filtering.rst` & `tsfresh-0.9.0/docs/text/feature_filtering.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-Feature filtering
-=================
-
-
-The all-relevant problem of feature selection is the identification of all strongly and weakly relevant attributes.
-This problem is especially hard to solve for time series classification and regression in industrial applications such
-as predictive maintenance or production line optimization, for which each label or regression target is associated with
-several time series and meta-information simultaneously.
-
-To limit the number of irrelevant features, tsfresh deploys the fresh algorithm (fresh stands for `FeatuRe Extraction
-based on Scalable Hypothesis tests`) [1]_.
-
-The algorithm is called by :func:`tsfresh.feature_selection.feature_selector.check_fs_sig_bh`.
-It is an efficient, scalable feature extraction algorithm, which filters the available features in an early stage of the
-machine learning pipeline with respect to their significance for the classification or regression task, while
-controlling the expected percentage of selected but irrelevant features.
-
-The filtering process consists of three phases which are sketched in the following figure:
-
-.. image:: ../images/feature_extraction_process_20160815_mc_1.png
-   :scale: 70 %
-   :alt: the time series
-   :align: center
-
-Phase 1 - Feature extraction
-''''''''''''''''''''''''''''
-
-Firstly, the algorithm characterizes time series with comprehensive and well-established feature mappings and considers
-additional features describing meta-information.
-The feature calculators used to derive the features are contained in
-:mod:`tsfresh.feature_extraction.feature_calculators`.
-
-In the figure from above, this corresponds to the change from raw time series to aggregated features.
-
-Phase 2 - Feature significance testing
-''''''''''''''''''''''''''''''''''''''
-
-In a second step, each feature vector is individually and independently evaluated with respect to its significance for
-predicting the target under investigation.
-Those tests are contained in the submodule :mod:`tsfresh.feature_selection.significance_tests`.
-The result of these tests is a vector of p-values, quantifying the significance of each feature for predicting the
-label/target.
-
-In the figure from above, this corresponds to the change from aggregated features to p-values.
-
-Phase 3 - Multiple test procedure
-'''''''''''''''''''''''''''''''''
-
-The vector of p-values is evaluated on basis of the Benjamini-Yekutieli procedure [2]_ in order to decide which features
-to keep.
-This multiple testing procedure is contained in the submodule :mod:`tsfresh.feature_selection.feature_selector`.
-
-In the figure from above, this corresponds to the change from p-values to selected features.
-
-
-References
-''''''''''
-
-    .. [1] Christ, M., Kempa-Liehr, A.W. and Feindt, M. (2016).
-         Distributed and parallel time series feature extraction for industrial big data applications.
-         ArXiv e-prints: 1610.07717 URL: http://adsabs.harvard.edu/abs/2016arXiv161007717C
-
-    .. [2] Benjamini, Y. and Yekutieli, D. (2001).
-        The control of the false discovery rate in multiple testing under dependency.
-        Annals of statistics, 1165--1188
+Feature filtering
+=================
+
+
+The all-relevant problem of feature selection is the identification of all strongly and weakly relevant attributes.
+This problem is especially hard to solve for time series classification and regression in industrial applications such
+as predictive maintenance or production line optimization, for which each label or regression target is associated with
+several time series and meta-information simultaneously.
+
+To limit the number of irrelevant features, tsfresh deploys the fresh algorithm (fresh stands for `FeatuRe Extraction
+based on Scalable Hypothesis tests`) [1]_.
+
+The algorithm is called by :func:`tsfresh.feature_selection.relevance.calculate_relevance_table`.
+It is an efficient, scalable feature extraction algorithm, which filters the available features in an early stage of the
+machine learning pipeline with respect to their significance for the classification or regression task, while
+controlling the expected percentage of selected but irrelevant features.
+
+The filtering process consists of three phases which are sketched in the following figure:
+
+.. image:: ../images/feature_extraction_process_20160815_mc_1.png
+   :scale: 70 %
+   :alt: the time series
+   :align: center
+
+Phase 1 - Feature extraction
+''''''''''''''''''''''''''''
+
+Firstly, the algorithm characterizes time series with comprehensive and well-established feature mappings and considers
+additional features describing meta-information.
+The feature calculators used to derive the features are contained in
+:mod:`tsfresh.feature_extraction.feature_calculators`.
+
+In the figure from above, this corresponds to the change from raw time series to aggregated features.
+
+Phase 2 - Feature significance testing
+''''''''''''''''''''''''''''''''''''''
+
+In a second step, each feature vector is individually and independently evaluated with respect to its significance for
+predicting the target under investigation.
+Those tests are contained in the submodule :mod:`tsfresh.feature_selection.significance_tests`.
+The result of these tests is a vector of p-values, quantifying the significance of each feature for predicting the
+label/target.
+
+In the figure from above, this corresponds to the change from aggregated features to p-values.
+
+Phase 3 - Multiple test procedure
+'''''''''''''''''''''''''''''''''
+
+The vector of p-values is evaluated on basis of the Benjamini-Yekutieli procedure [2]_ in order to decide which features
+to keep.
+This multiple testing procedure is contained in the submodule :mod:`tsfresh.feature_selection.benjamini_hochberg_test`.
+
+In the figure from above, this corresponds to the change from p-values to selected features.
+
+
+References
+''''''''''
+
+    .. [1] Christ, M., Kempa-Liehr, A.W. and Feindt, M. (2016).
+         Distributed and parallel time series feature extraction for industrial big data applications.
+         ArXiv e-prints: 1610.07717 URL: http://adsabs.harvard.edu/abs/2016arXiv161007717C
+
+    .. [2] Benjamini, Y. and Yekutieli, D. (2001).
+        The control of the false discovery rate in multiple testing under dependency.
+        Annals of statistics, 1165--1188
```

### Comparing `tsfresh-0.8.1/docs/text/how_to_add_custom_feature.rst` & `tsfresh-0.9.0/docs/text/how_to_add_custom_feature.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,133 @@
-How to add a custom feature
-===========================
-
-It may be beneficial to add a custom feature to those that are calculated by tsfresh. To do so, one has to adapt certain
-steps:
-
-Step 1. Decide which type of feature you want to implement
-----------------------------------------------------------
-
-In tsfresh we differentiate between three types of feature calculation methods
-
-    *1.* aggregate features without parameter
-
-    *2.* aggregate features with parameter
-
-    *3.* apply features with parameters
-
-So if you want to add a singular feature with out any parameters, stick with *1.*, the aggregate feature without
-parameters.
-
-Then, if your features can be calculated independently for each possible parameter set, stick with type *2.*, the
-aggregate features with parameters.
-
-If both cases from above do not apply, because it is beneficial to calculate the features for the different
-parameter settings at the same time (to e.g. perform auxiliary calculations only once for all features), stick with
-type *3.*, the apply features with parameters.
-
-
-Step 2. Write the feature calculator
-------------------------------------
-
-Depending on which type of feature you are implementing, you can use the following feature calculator skeletons:
-
-*1.* aggregate features without parameter
-
-.. code:: python
-
-    @set_property("fctype", "aggregate")
-    def your_feature_calculator(x):
-        """
-        The description of your feature
-
-        :param x: the time series to calculate the feature of
-        :type x: pandas.Series
-        :return: the value of this feature
-        :return type: bool or float
-        """
-        # Calculation of feature as float, int or bool
-        f = f(x)
-        return f
-
-
-
-*2.* aggregate features with parameter
-
-.. code:: python
-
-    @set_property("fctype", "aggregate_with_parameters")
-    def your_feature_calculator(x, p1, p2, ...):
-        """
-        Description of your feature
-
-        :param x: the time series to calculate the feature of
-        :type x: pandas.Series
-        :param p1: description of your parameter p1
-        :type p1: type of your parameter p1
-        :param p2: description of your parameter p2
-        :type p2: type of your parameter p2
-        ...
-        :return: the value of this feature
-        :return type: bool or float
-        """
-        # Calculation of feature as float, int or bool
-        f = f(x)
-        return f
-
-
-*3.* apply features with parameters
-
-.. code:: python
-
-    @set_property("fctype", "apply")
-    def your_feature_calculator(x, c, param):
-        """
-        Description of your feature
-
-        :param x: the time series to calculate the feature of
-        :type x: pandas.Series
-        :param c: the time series name
-        :type c: str
-        :param param: contains dictionaries {"p1": x, "p2": y, ...} with p1 float, p2 int ...
-        :type param: list
-        :return: the different feature values
-        :return type: pandas.Series
-        """
-        # Calculation of feature as pandas.Series s, the index is the name of the feature
-        s = f(x)
-        return s
-
-
-After implementing the feature calculator, please add it to the :mod:`tsfresh.feature_extraction.feature_calculators`
-submodule. tsfresh will only find feature calculators that are in this submodule.
-
-
-Step 3. Add custom settings for your feature
---------------------------------------------
-
-Finally, you have to add custom settings if your feature is an apply or aggregate feature with parameters. To do so,
-just append your feature with sane default parameters to the ``name_to_param`` dictionary inside the
-:class:`tsfresh.ComprehensiveFCParameters` constructor:
-
-.. code:: python
-
-    name_to_param.update({
-        # here are the existing settings
-        ...
-        # Now the settings of your feature calculator
-        "your_feature_calculator" = [{"p1": x, "p2": y, ...} for x,y in ...],
-    })
-
-
-That is it, tsfresh will calculate your feature the next time you run it.
-
-Please make sure, that the different feature extraction settings
-(e.g. :class:`tsfresh.feature_extraction.settings.EfficientCParameters`,
-:class:`tsfresh.feature_extraction.settings.MinimalFCParameters` or
-:class:`tsfresh.feature_extraction.settings.ComprehensiveFCParameters`) do include different sets of
-feature calculators to use. You can control, which feature extraction settings object will include your new
-feature calculator by giving your function attributes like "minimal" or "high_comp_cost". Please see the
-classes in :mod:`tsfresh.feature_extraction.settings` for more information.
-
-
-Step 4. Add a pull request
---------------------------
-
-We would very happy if you contribute your implemented features to tsfresh. So make sure to create a pull request at our
-`github page <https://github.com/blue-yonder/tsfresh>`_. We happily accept partly implemented features that we can
-finalize.
+How to add a custom feature
+===========================
+
+It may be beneficial to add a custom feature to those that are calculated by tsfresh. To do so, one has to follow four
+simple steps:
+
+Step 1. Decide which type of feature you want to implement
+----------------------------------------------------------
+
+In tsfresh we differentiate between two types of feature calculation methods
+
+    *1.* simple
+
+    *2.* combiner
+
+The difference lays in the number of calculated features for a singular time series.
+The feature_calculator returns either one (*1.*) or multiple features (*2.*).
+So if you want to add a singular feature stick with *1.*, the simple feature calculator class.
+If it is beneficial to calculate multiples features at the same time (to e.g. perform auxiliary calculations only once
+for all features), stick with type *2.*.
+
+
+Step 2. Write the feature calculator
+------------------------------------
+
+Depending on which type of feature you are implementing, you can use the following feature calculator skeletons:
+
+*1.* simple features
+
+You can write such a simple feature calculator, that returns exactly one feature, without parameter
+
+.. code:: python
+
+    @set_property("fctype", "simple")
+    def your_feature_calculator(x):
+        """
+        The description of your feature
+
+        :param x: the time series to calculate the feature of
+        :type x: pandas.Series
+        :return: the value of this feature
+        :return type: bool, int or float
+        """
+        # Calculation of feature as float, int or bool
+        f = f(x)
+        return f
+
+or with parameter
+
+.. code:: python
+
+    @set_property("fctype", "simple"")
+    def your_feature_calculator(x, p1, p2, ...):
+        """
+        Description of your feature
+
+        :param x: the time series to calculate the feature of
+        :type x: pandas.Series
+        :param p1: description of your parameter p1
+        :type p1: type of your parameter p1
+        :param p2: description of your parameter p2
+        :type p2: type of your parameter p2
+        ...
+        :return: the value of this feature
+        :return type: bool, int or float
+        """
+        # Calculation of feature as float, int or bool
+        f = f(x)
+        return f
+
+
+*2.* combiner features
+
+.. code:: python
+
+    @set_property("fctype", "combiner")
+    def your_feature_calculator(x, param):
+        """
+        Description of your feature
+
+        :param x: the time series to calculate the feature of
+        :type x: pandas.Series
+        :param c: the time series name
+        :type c: str
+        :param param: contains dictionaries {"p1": x, "p2": y, ...} with p1 float, p2 int ...
+        :type param: list
+        :return: list of tuples (s, f) where s are the parameters, serialized as a string, and f the respective feature
+            value as bool, int or float
+        :return type: pandas.Series
+        """
+        # s is a function that serializes the config
+        # f is a function that calculates the feature value for the config
+        return [(s(config), f(x, config)) for config in param]
+
+
+After implementing the feature calculator, please add it to the :mod:`tsfresh.feature_extraction.feature_calculators`
+submodule. tsfresh will only find feature calculators that are in this submodule.
+
+
+Step 3. Add custom settings for your feature
+--------------------------------------------
+
+Finally, you have to add custom settings if your feature is a simple or combiner feature with parameters. To do so,
+just append your feature with sane default parameters to the ``name_to_param`` dictionary inside the
+:class:`tsfresh.ComprehensiveFCParameters` constructor:
+
+.. code:: python
+
+    name_to_param.update({
+        # here are the existing settings
+        ...
+        # Now the settings of your feature calculator
+        "your_feature_calculator" = [{"p1": x, "p2": y, ...} for x,y in ...],
+    })
+
+
+That is it, tsfresh will calculate your feature the next time you run it.
+
+Please make sure, that the different feature extraction settings
+(e.g. :class:`tsfresh.feature_extraction.settings.EfficientCParameters`,
+:class:`tsfresh.feature_extraction.settings.MinimalFCParameters` or
+:class:`tsfresh.feature_extraction.settings.ComprehensiveFCParameters`) do include different sets of
+feature calculators to use. You can control, which feature extraction settings object will include your new
+feature calculator by giving your function attributes like "minimal" or "high_comp_cost". Please see the
+classes in :mod:`tsfresh.feature_extraction.settings` for more information.
+
+
+Step 4. Add a pull request
+--------------------------
+
+We would very happy if you contribute your implemented features to tsfresh. So make sure to create a pull request at our
+`github page <https://github.com/blue-yonder/tsfresh>`_. We happily accept partly implemented features that we can
+finalize.
```

### Comparing `tsfresh-0.8.1/docs/text/how_to_contribute.rst` & `tsfresh-0.9.0/docs/text/how_to_contribute.rst`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/text/introduction.rst` & `tsfresh-0.9.0/docs/text/introduction.rst`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/docs/text/parallelization.rst` & `tsfresh-0.9.0/docs/text/parallelization.rst`

 * *Files 18% similar despite different names*

```diff
@@ -12,48 +12,24 @@
 well as the default settings.
 
 Parallelization of Feature Selection
 ------------------------------------
 
 We use a :class:`multiprocessing.Pool` to parallelize the calculation of the p-values for each feature. On
 instantiation we set the Pool's number of worker processes to
-`n_processes`. This field defaults to
+`n_jobs`. This field defaults to
 the number of processors on the current system. We recommend setting it to the maximum number of available (and
 otherwise idle) processors.
 
 The chunksize of the Pool's map function is another important parameter to consider. It can be set via the
 `chunksize` field. By default it is up to
 :class:`multiprocessing.Pool` to decide on the chunksize.
 
 Parallelization of Feature Extraction
 -------------------------------------
 
 For the feature extraction tsfresh exposes the parameters
-`n_processes` and
-`chunksize`. Both behave anlogue to the parameters
+`n_jobs` and `chunksize`. Both behave analogue to the parameters
 for the feature selection.
 
-Additionally there are two options for how the parallelization is done:
-
-1.  ``'per_kind'`` parallelizes the feature calculation per kind of time series.
-2.  ``'per_sample'`` parallelizes per kind and per sample.
-
-To enforce an option, either pass ``'per_kind'`` or ``'per_sample'`` as the ``parallelization=`` parameter of the
-:func:`tsfresh.extract_features` function. By default the option is chosen with a rule of thumb:
-
-If the number of different time series (kinds) is less than half of the number of available worker
-processes (``n_processes``) then ``'per_sample'`` is chosen, otherwise ``'per_kind'``.
-
-Generally, there is no perfect setting for all cases. On the one hand more parallelization can speed up the calculation
-as the work is better distributed among the computers resources. On the other hand parallelization
-introduces overheads such as copying data to the worker processes, splitting the data to enable the distribution and
-combining the results.
-
-Implementing the parallelization we observed the following aspects:
-
--   For small data sets the difference between parallelization per kind or per sample should be negligible.
--   For data sets with one kind of time series parallelization per sample results in a decent speed up that grows
-    with the number of samples.
--   The more kinds of time series the data set contains, the more samples are necessary to make parallelization
-    per sample worthwhile.
--   If the data set contains more kinds of time series than available cpu cores, parallelization per kind is
-    the way to go.
+To do performance studies and profiling, it sometimes quite useful to turn off parallelization at all. This can be
+setting the parameter `n_jobs` to 0.
```

### Comparing `tsfresh-0.8.1/docs/text/quick_start.rst` & `tsfresh-0.9.0/docs/text/quick_start.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-.. _quick-start-label:
-
-Quick Start
-===========
-
-
-Install tsfresh
----------------
-
-As the compiled tsfresh package is hosted on pypy you can easily install it with pip
-
-.. code:: shell
-
-   pip install tsfresh
-
-
-Dive in
--------
-
-Before boring yourself by reading the docs in detail, you can dive right into tsfresh with the following example:
-
-We are given a data set containing robot failures as discussed in [1]_.
-Each robot records time series from six different sensors.
-For each sample denoted by a different id we are going to classify if the robot reports a failure or not.
-From a machine learning point of view, our goal is to classify each group of time series.
-
-To start, we load the data into python
-
-.. code:: python
-
-    from tsfresh.examples.robot_execution_failures import download_robot_execution_failures, \
-        load_robot_execution_failures
-    download_robot_execution_failures()
-    timeseries, y = load_robot_execution_failures()
-
-and end up with a pandas.DataFrame `timeseries` having the following shape
-
-+-----+-----+-----+----+----+----+----+----+----+
-|     | id  | time| a  | b  | c  | d  | e  | f  |
-+=====+=====+=====+====+====+====+====+====+====+
-| 0   | 1   | 0   | -1 |-1  | 63 | -3 | -1 | 0  |
-+-----+-----+-----+----+----+----+----+----+----+
-| 1   | 1   | 1   | 0  | 0  | 62 | -3 | -1 | 0  |
-+-----+-----+-----+----+----+----+----+----+----+
-| 2   | 1   | 2   | -1 |-1  | 61 | -3 | 0  | 0  |
-+-----+-----+-----+----+----+----+----+----+----+
-| 3   | 1   | 3   | -1 |-1  | 63 | -2 | -1 | 0  |
-+-----+-----+-----+----+----+----+----+----+----+
-| 4   | 1   | 4   | -1 |-1  | 63 | -3 | -1 | 0  |
-+-----+-----+-----+----+----+----+----+----+----+
-| ... | ... | ... | ...| ...|... | ...| ...| ...|
-+-----+-----+-----+----+----+----+----+----+----+
-
-The first column is the DataFrame index and has no meaning here.
-There are six different time series (a-f) for the different sensors. The different robots are denoted by the ids column.
-
-On the other hand, ``y`` contains the information which robot `id` reported a failure and which not:
-
-+---+---+
-| 1 | 0 |
-+---+---+
-| 2 | 0 |
-+---+---+
-| 3 | 0 |
-+---+---+
-| 4 | 0 |
-+---+---+
-| 5 | 0 |
-+---+---+
-|...|...|
-+---+---+
-
-Here, for the samples with ids 1 to 5 no failure was reported.
-
-In the following we illustrate the time series of the sample id 3 reporting no failure:
-
-.. image:: ../images/ts_example_robot_failures_nofail.png
-   :scale: 100 %
-   :alt: the time series for id 3 (no failure)
-   :align: center
-
-And for id 20 reporting a failure:
-
-.. image:: ../images/ts_example_robot_failures_fail.png
-   :scale: 100 %
-   :alt: the time series for id 20 (failure)
-   :align: center
-
-You can already see some differences by eye - but for successful machine learning we have to put these differences into
-numbers.
-
-For this, tsfresh comes into place.
-It allows us to automatically extract over 1200 features from those six different time series for each robot.
-
-For extracting all features, we do:
-
-.. code:: python
-
-    from tsfresh import extract_features
-    extracted_features = extract_features(timeseries, column_id="id", column_sort="time")
-
-You end up with a DataFrame `extracted_features` with all more than 1200 different extracted features.
-We will now remove all ``NaN`` values (that were created by feature calculators, than can not be used on the given
-data, e.g. because it has too low statistics) and select only the relevant features next:
-
-.. code-block:: python
-
-    from tsfresh import select_features
-    from tsfresh.utilities.dataframe_functions import impute
-
-    impute(extracted_features)
-    features_filtered = select_features(extracted_features, y)
-
-
-Only around 300 features were classified as relevant enough.
-
-Further, you can even perform the extraction, imputing and filtering at the same time with the
-:func:`tsfresh.extract_relevant_features` function:
-
-.. code-block:: python
-
-    from tsfresh import extract_relevant_features
-
-    features_filtered_direct = extract_relevant_features(timeseries, y,
-                                                         column_id='id', column_sort='time')
-
-
-You can now use the features contained in the DataFrame `features_filtered` (which is equal to
-`features_filtered_direct`) in conjunction with `y` to train your classification model.
-Please see the `robot_failure_example.ipynb` Jupyter Notebook in the folder named notebook for this.
-In this notebook a RandomForestClassifier is trained on the extracted features.
-
-References
-
-.. [1] http://archive.ics.uci.edu/ml/datasets/Robot+Execution+Failures
+.. _quick-start-label:
+
+Quick Start
+===========
+
+
+Install tsfresh
+---------------
+
+As the compiled tsfresh package is hosted on the Python Package Index (PyPI) you can easily install it with pip
+
+.. code:: shell
+
+   pip install tsfresh
+
+
+Dive in
+-------
+
+Before boring yourself by reading the docs in detail, you can dive right into tsfresh with the following example:
+
+We are given a data set containing robot failures as discussed in [1]_.
+Each robot records time series from six different sensors.
+For each sample denoted by a different id we are going to classify if the robot reports a failure or not.
+From a machine learning point of view, our goal is to classify each group of time series.
+
+To start, we load the data into python
+
+.. code:: python
+
+    from tsfresh.examples.robot_execution_failures import download_robot_execution_failures, \
+        load_robot_execution_failures
+    download_robot_execution_failures()
+    timeseries, y = load_robot_execution_failures()
+
+and end up with a pandas.DataFrame `timeseries` having the following shape
+
++-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|     | id  | time| F_x | F_y | F_z | T_x | T_y | T_z |
++=====+=====+=====+=====+=====+=====+=====+=====+=====+
+| 0   | 1   | 0   | -1  | -1  | 63  | -3  | -1  | 0   |
++-----+-----+-----+-----+-----+-----+-----+-----+-----+
+| 1   | 1   | 1   | 0   | 0   | 62  | -3  | -1  | 0   |
++-----+-----+-----+-----+-----+-----+-----+-----+-----+
+| 2   | 1   | 2   | -1  | -1  | 61  | -3  | 0   | 0   |
++-----+-----+-----+-----+-----+-----+-----+-----+-----+
+| 3   | 1   | 3   | -1  | -1  | 63  | -2  | -1  | 0   |
++-----+-----+-----+-----+-----+-----+-----+-----+-----+
+| 4   | 1   | 4   | -1  | -1  | 63  | -3  | -1  | 0   |
++-----+-----+-----+-----+-----+-----+-----+-----+-----+
+| ... | ... | ... | ... | ... | ... | ... | ... | ... |
++-----+-----+-----+-----+-----+-----+-----+-----+-----+
+
+The first column is the DataFrame index and has no meaning here.
+There are six different time series (a-f) for the different sensors. The different robots are denoted by the ids column.
+
+On the other hand, ``y`` contains the information which robot `id` reported a failure and which not:
+
++---+---+
+| 1 | 0 |
++---+---+
+| 2 | 0 |
++---+---+
+| 3 | 0 |
++---+---+
+| 4 | 0 |
++---+---+
+| 5 | 0 |
++---+---+
+|...|...|
++---+---+
+
+Here, for the samples with ids 1 to 5 no failure was reported.
+
+In the following we illustrate the time series of the sample id 3 reporting no failure:
+
+.. image:: ../images/ts_example_robot_failures_nofail.png
+   :scale: 100 %
+   :alt: the time series for id 3 (no failure)
+   :align: center
+
+And for id 20 reporting a failure:
+
+.. image:: ../images/ts_example_robot_failures_fail.png
+   :scale: 100 %
+   :alt: the time series for id 20 (failure)
+   :align: center
+
+You can already see some differences by eye - but for successful machine learning we have to put these differences into
+numbers.
+
+For this, tsfresh comes into place.
+It allows us to automatically extract over 1200 features from those six different time series for each robot.
+
+For extracting all features, we do:
+
+.. code:: python
+
+    from tsfresh import extract_features
+    extracted_features = extract_features(timeseries, column_id="id", column_sort="time")
+
+You end up with a DataFrame `extracted_features` with all more than 1200 different extracted features.
+We will now remove all ``NaN`` values (that were created by feature calculators, than can not be used on the given
+data, e.g. because it has too low statistics) and select only the relevant features next:
+
+.. code-block:: python
+
+    from tsfresh import select_features
+    from tsfresh.utilities.dataframe_functions import impute
+
+    impute(extracted_features)
+    features_filtered = select_features(extracted_features, y)
+
+
+Only around 300 features were classified as relevant enough.
+
+Further, you can even perform the extraction, imputing and filtering at the same time with the
+:func:`tsfresh.extract_relevant_features` function:
+
+.. code-block:: python
+
+    from tsfresh import extract_relevant_features
+
+    features_filtered_direct = extract_relevant_features(timeseries, y,
+                                                         column_id='id', column_sort='time')
+
+
+You can now use the features contained in the DataFrame `features_filtered` (which is equal to
+`features_filtered_direct`) in conjunction with `y` to train your classification model.
+Please see the `robot_failure_example.ipynb` Jupyter Notebook in the folder named notebook for this.
+In this notebook a RandomForestClassifier is trained on the extracted features.
+
+References
+
+.. [1] http://archive.ics.uci.edu/ml/datasets/Robot+Execution+Failures
```

### Comparing `tsfresh-0.8.1/docs/text/sklearn_transformers.rst` & `tsfresh-0.9.0/docs/text/sklearn_transformers.rst`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/LICENSE.txt` & `tsfresh-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/notebooks/compare-runtimes-of-feature-calculators.ipynb` & `tsfresh-0.9.0/notebooks/compare-runtimes-of-feature-calculators.ipynb`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/notebooks/friedrich_coefficients.ipynb` & `tsfresh-0.9.0/notebooks/friedrich_coefficients.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9840261466823967%*

 * *Differences: {"'cells'": "{5: {'outputs': {0: {'text': {insert: [(0, "*

 * *            "'/usr/local/lib/python2.7/site-packages/IPython/html.py:14: ShimWarning: The "*

 * *            '`IPython.html` package has been deprecated since IPython 4.0. You should import from '*

 * *            "`notebook` instead. `IPython.html.widgets` has moved to `ipywidgets`.\\n'), (2, "*

 * *            "'/usr/local/lib/python2.7/site-packages/statsmodels/compat/pandas.py:56: "*

 * *            'FutureWarning: The pandas.core.datetools module is deprecated and  […]*

```diff
@@ -65,17 +65,17 @@
                 "editable": true
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/Users/mchrist/Documents/Research/tsfresh/venv/lib/python2.7/site-packages/IPython/html.py:14: ShimWarning: The `IPython.html` package has been deprecated since IPython 4.0. You should import from `notebook` instead. `IPython.html.widgets` has moved to `ipywidgets`.\n",
+                        "/usr/local/lib/python2.7/site-packages/IPython/html.py:14: ShimWarning: The `IPython.html` package has been deprecated since IPython 4.0. You should import from `notebook` instead. `IPython.html.widgets` has moved to `ipywidgets`.\n",
                         "  \"`IPython.html.widgets` has moved to `ipywidgets`.\", ShimWarning)\n",
-                        "/Users/mchrist/Documents/Research/tsfresh/venv/lib/python2.7/site-packages/statsmodels/compat/pandas.py:56: FutureWarning: The pandas.core.datetools module is deprecated and will be removed in a future version. Please use the pandas.tseries module instead.\n",
+                        "/usr/local/lib/python2.7/site-packages/statsmodels/compat/pandas.py:56: FutureWarning: The pandas.core.datetools module is deprecated and will be removed in a future version. Please use the pandas.tseries module instead.\n",
                         "  from pandas.core import datetools\n"
                     ]
                 }
             ],
             "source": [
                 "from matplotlib import pylab as plt\n",
                 "import numpy as np\n",
@@ -112,15 +112,15 @@
                 "settings = ComprehensiveFCParameters()\n",
                 "default_params = settings['max_langevin_fixed_point'][0]\n",
                 "default = settings['friedrich_coefficients']"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 14,
             "metadata": {
                 "collapsed": false,
                 "deletable": true,
                 "editable": true
             },
             "outputs": [],
             "source": [
@@ -129,15 +129,16 @@
                 "    df['quantiles']=pd.qcut(df.velocity.values, 30)\n",
                 "    groups = df.groupby('quantiles')\n",
                 "    result = pd.DataFrame({'a_mean': groups.acceleration.mean(),\n",
                 "                           'a_std': groups.acceleration.std(),\n",
                 "                           'v_mean': groups.velocity.mean(),\n",
                 "                           'v_std': groups.velocity.std()\n",
                 "                          })\n",
-                "    dynamics = friedrich_coefficients(v[:,0], 'DriftBif', param).values\n",
+                "    dynamics = friedrich_coefficients(v[:,0], param)\n",
+                "    dynamics = [d[1] for d in dynamics]\n",
                 "    v0 = max_langevin_fixed_point(v[:,0], **default_params)\n",
                 "    \n",
                 "    plt.subplot(2,1,1)\n",
                 "    plt.plot(v[:,0])\n",
                 "    plt.axhline(y=v0, color='r')\n",
                 "    plt.xlabel('time')\n",
                 "    plt.ylabel('velocity')\n",
@@ -149,14 +150,15 @@
                 "        active=''\n",
                 "        \n",
                 "    plt.title('{} Brownian Motion (largest equilibrium velocity in red)'.format(active))\n",
                 "    plt.subplot(2,1,2)\n",
                 "    ax = plt.errorbar(result.v_mean,result.a_mean,\n",
                 "                 xerr=result.v_std,fmt='o')\n",
                 "    x = np.linspace(-0.004, 0.004, 201)\n",
+                "    print(dynamics)\n",
                 "    plt.plot(x, np.poly1d(dynamics)(x), label='estimated dynamics')\n",
                 "    plt.plot(v0,0.,'ro')\n",
                 "    plt.axvline(x=v0, color='r')\n",
                 "    plt.xlabel('mean velocity')\n",
                 "    plt.ylabel('mean acceleration')"
             ]
         },
@@ -168,35 +170,52 @@
             },
             "source": [
                 "# Beyond drift-bifurcation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 15,
             "metadata": {
                 "collapsed": false,
                 "deletable": true,
                 "editable": true
             },
+            "outputs": [],
+            "source": [
+                "ds = velocity(tau=3.8, delta_t=0.05, R=3e-4, seed=0)\n",
+                "v = ds.simulate(1000000, v0=np.zeros(1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "metadata": {
+                "collapsed": false
+            },
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[-343.32787387478442, 0.037453057120062423, 0.0022569679511866667, -1.0236536382788926e-07]\n"
+                    ]
+                },
+                {
                     "data": {
                         "image/png": "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\n",
                         "text/plain": [
-                            "<matplotlib.figure.Figure at 0x10f636050>"
+                            "<matplotlib.figure.Figure at 0x1152c3d90>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "ds = velocity(tau=3.8, delta_t=0.05, R=3e-4, seed=0)\n",
-                "v = ds.simulate(1000000, v0=np.zeros(1))\n",
                 "friedrich_method(v, default)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "deletable": true,
@@ -204,40 +223,47 @@
             },
             "source": [
                 "# Before drift-bifurcation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 17,
             "metadata": {
                 "collapsed": true,
                 "deletable": true,
                 "editable": true
             },
             "outputs": [],
             "source": [
                 "ds = velocity(tau=2./0.3-3.8, delta_t=0.05, R=3e-4, seed=0)\n",
                 "v = ds.simulate(1000000, v0=np.zeros(1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 18,
             "metadata": {
                 "collapsed": false,
                 "deletable": true,
                 "editable": true
             },
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[-430.63544990116668, 0.083476393069130017, -0.0020234721659708023, 4.3026801890000346e-08]\n"
+                    ]
+                },
+                {
                     "data": {
                         "image/png": "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\nrkJggg==\n",
                         "text/plain": [
-                            "<matplotlib.figure.Figure at 0x1139e7ed0>"
+                            "<matplotlib.figure.Figure at 0x11565e150>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
@@ -257,13 +283,13 @@
                 "version": 2
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython2",
-            "version": "2.7.11"
+            "version": "2.7.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `tsfresh-0.8.1/PKG-INFO` & `tsfresh-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tsfresh
-Version: 0.8.1
+Version: 0.9.0
 Summary: tsfresh extracts relevant characteristics from time series
 Home-page: https://github.com/blue-yonder/tsfresh
 Author: Maximilian Christ, Nils Braun, Julius Neuffer
 Author-email: max.christ@me.com
 License: MIT
 Description: |Documentation Status| |Build Status| |Coverage Status| |license|
         |Gitter chat| |py27 status| |py352 status|
```

### Comparing `tsfresh-0.8.1/README.md` & `tsfresh-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/README.rst` & `tsfresh-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/setup.cfg` & `tsfresh-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/setup.py` & `tsfresh-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/examples/test_driftbif_simulation.py` & `tsfresh-0.9.0/tests/examples/test_driftbif_simulation.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/examples/test_har_dataset.py` & `tsfresh-0.9.0/tests/examples/test_har_dataset.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/examples/test_robot_execution_failures.py` & `tsfresh-0.9.0/tests/examples/test_robot_execution_failures.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,40 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-from unittest import TestCase
-
-from tsfresh import extract_features
-from tsfresh.examples.robot_execution_failures import load_robot_execution_failures, download_robot_execution_failures
-from pandas import DataFrame, Series
-import six
-
-
-class RobotExecutionFailuresTestCase(TestCase):
-    def setUp(self):
-        download_robot_execution_failures()
-        self.X, self.y = load_robot_execution_failures()
-
-    def test_characteristics_downloaded_robot_execution_failures(self):
-        self.assertEqual(len(self.X), 1320)
-        self.assertIsInstance(self.X, DataFrame)
-        self.assertIsInstance(self.y, Series)
-        six.assertCountEqual(self, ['id', 'time', 'a', 'b', 'c', 'd', 'e', 'f'], list(self.X.columns))
-
-if __name__ == '__main__':
-    timeseries, y = load_robot_execution_failures()
-    extracted_features = extract_features(timeseries[timeseries.id < 20], column_id="id", column_sort="time",
-                                          parallelization="no_parallelization")
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+from unittest import TestCase
+
+from tsfresh import extract_features
+from tsfresh.examples.robot_execution_failures import load_robot_execution_failures, download_robot_execution_failures
+from pandas import DataFrame, Series
+import six
+import numpy as np
+
+
+class RobotExecutionFailuresTestCase(TestCase):
+    def setUp(self):
+        download_robot_execution_failures()
+        self.X, self.y = load_robot_execution_failures()
+
+    def test_characteristics_downloaded_robot_execution_failures(self):
+        self.assertEqual(len(self.X), 1320)
+        self.assertIsInstance(self.X, DataFrame)
+        self.assertIsInstance(self.y, Series)
+        six.assertCountEqual(self, ['id', 'time', 'F_x', 'F_y', 'F_z', 'T_x', 'T_y', 'T_z'], list(self.X.columns))
+
+    def test_extraction_runs_through(self):
+        df = extract_features(self.X[self.X.id < 3], column_id="id", column_sort="time")
+
+        six.assertCountEqual(self, df.index.values, [1, 2])
+        self.assertGreater(len(df), 0)
+
+    def test_binary_target_is_default(self):
+        _, y = load_robot_execution_failures()
+
+        assert len(y.unique()) == 2
+
+    def test_multilabel_target_on_request(self):
+        _, y = load_robot_execution_failures(multiclass=True)
+
+        assert len(y.unique()) > 2
+        assert y.dtype == np.object
```

### Comparing `tsfresh-0.8.1/tests/feature_extraction/test_extraction.py` & `tsfresh-0.9.0/tests/feature_extraction/test_extraction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,215 +1,166 @@
 # -*- coding: utf-8 -*-
 # This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
 # Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
 
 from __future__ import absolute_import, division
+
+import os
+
 import numpy as np
 import pandas as pd
+import six
+
 from tests.fixtures import DataTestCase
-from tsfresh.feature_extraction.extraction import extract_features, _extract_features_for_one_time_series
+from tsfresh.feature_extraction.extraction import extract_features
 from tsfresh.feature_extraction.settings import ComprehensiveFCParameters
-import six
-import os
 
 
 class ExtractionTestCase(DataTestCase):
     """The unit tests in this module make sure if the time series features are created properly"""
 
     def setUp(self):
-        self.n_processes = 1
-
-    def test_extract_features_per_kind(self):
-        # todo: implement more methods and test more aspects
-        df = self.create_test_data_sample()
-        extracted_features = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
-                                              column_value="val", parallelization='per_kind',
-                                              n_processes=self.n_processes)
+        self.n_jobs = 1
 
-        self.assertIsInstance(extracted_features, pd.DataFrame)
-        self.assertTrue(np.all(extracted_features.a__maximum == np.array([71, 77])))
-        self.assertTrue(np.all(extracted_features.a__sum_values == np.array([691, 1017])))
-        self.assertTrue(np.all(extracted_features.a__abs_energy == np.array([32211, 63167])))
-        self.assertTrue(np.all(extracted_features.b__sum_values == np.array([757, 695])))
-        self.assertTrue(np.all(extracted_features.b__minimum == np.array([3, 1])))
-        self.assertTrue(np.all(extracted_features.b__abs_energy == np.array([36619, 35483])))
-        self.assertTrue(np.all(extracted_features.b__mean == np.array([37.85, 34.75])))
-        self.assertTrue(np.all(extracted_features.b__median == np.array([39.5, 28.0])))
-
-        df_sts = self.create_one_valued_time_series()
-        extracted_features_sts = extract_features(df_sts, column_id="id", column_sort="sort", column_kind="kind",
-                                                  column_value="val", parallelization='per_kind',
-                                                  n_processes=self.n_processes)
-
-        self.assertIsInstance(extracted_features_sts, pd.DataFrame)
-        self.assertTrue(np.all(extracted_features_sts.a__maximum == np.array([1.0, 6.0])))
-        self.assertTrue(np.all(extracted_features_sts.a__sum_values == np.array([1.0, 11.0])))
-        self.assertTrue(np.all(extracted_features_sts.a__count_above_mean == np.array([0, 1])))
-
-    def test_extract_features_per_sample(self):
+    def test_extract_features(self):
         # todo: implement more methods and test more aspects
         df = self.create_test_data_sample()
         extracted_features = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
-                                              column_value="val", parallelization='per_sample',
-                                              n_processes=self.n_processes)
+                                              column_value="val",
+                                              n_jobs=self.n_jobs)
 
         self.assertIsInstance(extracted_features, pd.DataFrame)
         self.assertTrue(np.all(extracted_features.a__maximum == np.array([71, 77])))
         self.assertTrue(np.all(extracted_features.a__sum_values == np.array([691, 1017])))
         self.assertTrue(np.all(extracted_features.a__abs_energy == np.array([32211, 63167])))
         self.assertTrue(np.all(extracted_features.b__sum_values == np.array([757, 695])))
         self.assertTrue(np.all(extracted_features.b__minimum == np.array([3, 1])))
         self.assertTrue(np.all(extracted_features.b__abs_energy == np.array([36619, 35483])))
         self.assertTrue(np.all(extracted_features.b__mean == np.array([37.85, 34.75])))
         self.assertTrue(np.all(extracted_features.b__median == np.array([39.5, 28.0])))
 
         df_sts = self.create_one_valued_time_series()
         extracted_features_sts = extract_features(df_sts, column_id="id", column_sort="sort", column_kind="kind",
-                                                  column_value="val", parallelization='per_sample',
-                                                  n_processes=self.n_processes)
+                                                  column_value="val",
+                                                  n_jobs=self.n_jobs)
 
         self.assertIsInstance(extracted_features_sts, pd.DataFrame)
         self.assertTrue(np.all(extracted_features_sts.a__maximum == np.array([1.0, 6.0])))
         self.assertTrue(np.all(extracted_features_sts.a__sum_values == np.array([1.0, 11.0])))
         self.assertTrue(np.all(extracted_features_sts.a__count_above_mean == np.array([0, 1])))
 
     def test_extract_features_for_one_time_series(self):
         # todo: implement more methods and test more aspects
         df = self.create_test_data_sample()
         settings = ComprehensiveFCParameters()
 
-        extracted_features = _extract_features_for_one_time_series(["b", df.loc[df.kind == "b", ["val", "id"]]],
-                                                                   default_fc_parameters=settings,
-                                                                   column_value="val", column_id="id")
+        extracted_features = extract_features(df, default_fc_parameters=settings,
+                                              column_value="val", column_id="id", column_kind="kind",
+                                              column_sort="sort")
 
         self.assertIsInstance(extracted_features, pd.DataFrame)
         self.assertTrue(np.all(extracted_features.b__sum_values == np.array([757, 695])))
         self.assertTrue(np.all(extracted_features.b__minimum == np.array([3, 1])))
         self.assertTrue(np.all(extracted_features.b__abs_energy == np.array([36619, 35483])))
         self.assertTrue(np.all(extracted_features.b__mean == np.array([37.85, 34.75])))
         self.assertTrue(np.all(extracted_features.b__median == np.array([39.5, 28.0])))
 
         df_sts = self.create_one_valued_time_series()
-        extracted_features_sts = _extract_features_for_one_time_series(["a", df_sts[["val", "id"]]],
-                                                                       default_fc_parameters=settings,
-                                                                       column_value="val", column_id="id")
+        extracted_features_sts = extract_features(df_sts, default_fc_parameters=settings,
+                                                  column_value="val", column_id="id", column_kind="kind",
+                                                  column_sort="sort")
 
         self.assertIsInstance(extracted_features_sts, pd.DataFrame)
         self.assertTrue(np.all(extracted_features_sts.a__maximum == np.array([1.0, 6.0])))
         self.assertTrue(np.all(extracted_features_sts.a__sum_values == np.array([1.0, 11.0])))
         self.assertTrue(np.all(extracted_features_sts.a__count_above_mean == np.array([0, 1])))
 
-    def test_extract_features_after_randomisation_per_kind(self):
-        df = self.create_test_data_sample()
-        df_random = df.copy().sample(frac=1)
-
-        extracted_features = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
-                                              column_value="val", parallelization='per_kind',
-                                              n_processes=self.n_processes).sort_index()
-        extracted_features_from_random = extract_features(df_random, column_id="id", column_sort="sort",
-                                                          column_kind="kind",
-                                                          column_value="val", parallelization='per_kind',
-                                                          n_processes=self.n_processes).sort_index()
-
-        six.assertCountEqual(self, extracted_features.columns, extracted_features_from_random.columns)
-
-        for col in extracted_features:
-            self.assertIsNone(np.testing.assert_array_almost_equal(extracted_features[col],
-                                                                   extracted_features_from_random[col]))
-
-    def test_extract_features_after_randomisation_per_sample(self):
+    def test_extract_features_after_randomisation(self):
         df = self.create_test_data_sample()
         df_random = df.copy().sample(frac=1)
 
         extracted_features = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
-                                              column_value="val", parallelization='per_sample',
-                                              n_processes=self.n_processes).sort_index()
+                                              column_value="val",
+                                              n_jobs=self.n_jobs).sort_index()
         extracted_features_from_random = extract_features(df_random, column_id="id", column_sort="sort",
                                                           column_kind="kind",
-                                                          column_value="val", parallelization='per_sample',
-                                                          n_processes=self.n_processes).sort_index()
+                                                          column_value="val",
+                                                          n_jobs=self.n_jobs).sort_index()
 
         six.assertCountEqual(self, extracted_features.columns, extracted_features_from_random.columns)
 
         for col in extracted_features:
             self.assertIsNone(np.testing.assert_array_almost_equal(extracted_features[col],
                                                                    extracted_features_from_random[col]))
 
     def test_profiling_file_written_out(self):
 
         df = pd.DataFrame(data={"id": np.repeat([1, 2], 10), "val": np.random.normal(0, 1, 20)})
         profiling_filename = "test_profiling.txt"
         X = extract_features(df, column_id="id",
-                             column_value="val", parallelization='per_kind', n_processes=self.n_processes,
+                             column_value="val", n_jobs=self.n_jobs,
                              profile=True, profiling_filename=profiling_filename)
 
         self.assertTrue(os.path.isfile(profiling_filename))
         os.remove(profiling_filename)
 
     def test_profiling_cumulative_file_written_out(self):
         PROFILING_FILENAME = "test_profiling_cumulative.txt"
         PROFILING_SORTING = "cumulative"
 
         df = pd.DataFrame(data={"id": np.repeat([1, 2], 10), "val": np.random.normal(0, 1, 20)})
         extract_features(df, column_id="id",
-                         column_value="val", parallelization='per_sample', n_processes=self.n_processes,
+                         column_value="val", n_jobs=self.n_jobs,
                          profile=True, profiling_filename=PROFILING_FILENAME, profiling_sorting=PROFILING_SORTING)
 
         self.assertTrue(os.path.isfile(PROFILING_FILENAME))
         os.remove(PROFILING_FILENAME)
 
     def test_extract_features_without_settings(self):
         df = pd.DataFrame(data={"id": np.repeat([1, 2], 10),
                                 "value1": np.random.normal(0, 1, 20),
                                 "value2": np.random.normal(0, 1, 20)})
         X = extract_features(df, column_id="id",
-                             n_processes=self.n_processes)
+                             n_jobs=self.n_jobs)
         self.assertIn("value1__maximum", list(X.columns))
         self.assertIn("value2__maximum", list(X.columns))
 
-    def test_extract_features_per_sample_equals_per_kind(self):
+    def test_extract_features_with_and_without_parallelization(self):
         df = self.create_test_data_sample()
 
-        features_per_sample = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
-                                               column_value="val", parallelization='per_sample',
-                                               n_processes=self.n_processes)
-        features_per_kind = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
-                                             column_value="val", parallelization='per_kind',
-                                             n_processes=self.n_processes)
+        features_parallel = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
+                                             column_value="val",
+                                             n_jobs=self.n_jobs)
         features_serial = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
-                                           column_value="val", parallelization='serial')
+                                           column_value="val", n_jobs=0)
 
-        six.assertCountEqual(self, features_per_sample.columns, features_per_kind.columns)
-        six.assertCountEqual(self, features_per_sample.columns, features_serial.columns)
+        six.assertCountEqual(self, features_parallel.columns, features_serial.columns)
 
-        for col in features_per_sample.columns:
-            self.assertIsNone(np.testing.assert_array_almost_equal(features_per_sample[col],
-                                                                   features_per_kind[col]))
-            self.assertIsNone(np.testing.assert_array_almost_equal(features_per_sample[col],
-                                                                   features_serial[col]))
+        for col in features_parallel.columns:
+            np.testing.assert_array_almost_equal(features_parallel[col], features_serial[col])
 
 
 class ParallelExtractionTestCase(DataTestCase):
     def setUp(self):
-        self.n_processes = 2
+        self.n_jobs = 2
 
         # only calculate some features to reduce load on travis ci
         self.name_to_param = {"maximum": None,
                               "sum_values": None,
                               "abs_energy": None,
                               "minimum": None,
                               "mean": None,
                               "median": None}
 
     def test_extract_features(self):
         # todo: implement more methods and test more aspects
         df = self.create_test_data_sample()
         extracted_features = extract_features(df, column_id="id", column_sort="sort", column_kind="kind",
                                               column_value="val",
-                                              n_processes=self.n_processes)
+                                              n_jobs=self.n_jobs)
 
         self.assertIsInstance(extracted_features, pd.DataFrame)
         self.assertTrue(np.all(extracted_features.a__maximum == np.array([71, 77])))
         self.assertTrue(np.all(extracted_features.a__sum_values == np.array([691, 1017])))
         self.assertTrue(np.all(extracted_features.a__abs_energy == np.array([32211, 63167])))
         self.assertTrue(np.all(extracted_features.b__sum_values == np.array([757, 695])))
         self.assertTrue(np.all(extracted_features.b__minimum == np.array([3, 1])))
```

### Comparing `tsfresh-0.8.1/tests/feature_extraction/test_feature_calculations.py` & `tsfresh-0.9.0/tests/feature_extraction/test_feature_calculations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,708 +1,900 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-from __future__ import absolute_import, division
-from __future__ import print_function
-from builtins import range
-from random import shuffle
-from unittest import TestCase
-from tsfresh.feature_extraction.feature_calculators import *
-from tsfresh.feature_extraction.feature_calculators import _get_length_sequences_where
-from tsfresh.feature_extraction.feature_calculators import _estimate_friedrich_coefficients
-from tsfresh.feature_extraction.feature_calculators import _aggregate_on_chunks
-from tsfresh.examples.driftbif_simulation import velocity
-import six
-import math
-
-
-class FeatureCalculationTestCase(TestCase):
-
-    def assertIsNaN(self, result):
-        self.assertTrue(np.isnan(result), msg="{} is not np.NaN")
-
-    def assertEqualOnAllArrayTypes(self, f, input_to_f, result, *args, **kwargs):
-        self.assertEqual(f(input_to_f, *args, **kwargs), result,
-                         msg="Not equal for lists: %s != %s" % (f(input_to_f, *args, **kwargs), result))
-        self.assertEqual(f(np.array(input_to_f), *args, **kwargs), result,
-                         msg="Not equal for numpy.arrays: %s != %s" % (
-                         f(np.array(input_to_f), *args, **kwargs), result))
-        self.assertEqual(f(pd.Series(input_to_f), *args, **kwargs), result,
-                         msg="Not equal for pandas.Series: %s != %s" % (
-                         f(pd.Series(input_to_f), *args, **kwargs), result))
-
-    def assertTrueOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
-        self.assertTrue(f(input_to_f, *args, **kwargs), msg="Not true for lists")
-        self.assertTrue(f(np.array(input_to_f), *args, **kwargs), msg="Not true for numpy.arrays")
-        self.assertTrue(f(pd.Series(input_to_f), *args, **kwargs), msg="Not true for pandas.Series")
-
-    def assertAllTrueOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
-        self.assertTrue(all(f(input_to_f, *args, **kwargs)), msg="Not true for lists")
-        self.assertTrue(all(f(np.array(input_to_f), *args, **kwargs)), msg="Not true for numpy.arrays")
-        self.assertTrue(all(f(pd.Series(input_to_f), *args, **kwargs)), msg="Not true for pandas.Series")
-
-    def assertFalseOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
-        self.assertFalse(f(input_to_f, *args, **kwargs), msg="Not false for lists")
-        self.assertFalse(f(np.array(input_to_f), *args, **kwargs), msg="Not false for numpy.arrays")
-        self.assertFalse(f(pd.Series(input_to_f), *args, **kwargs), msg="Not false for pandas.Series")
-
-    def assertAllFalseOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
-        self.assertFalse(any(f(input_to_f, *args, **kwargs)), msg="Not false for lists")
-        self.assertFalse(any(f(np.array(input_to_f), *args, **kwargs)), msg="Not false for numpy.arrays")
-        self.assertFalse(any(f(pd.Series(input_to_f), *args, **kwargs)), msg="Not false for pandas.Series")
-
-    def assertAlmostEqualOnAllArrayTypes(self, f, input_t_f, result, *args, **kwargs):
-        self.assertAlmostEqual(f(input_t_f, *args, **kwargs), result,
-                               msg="Not almost equal for lists: %s != %s" % (f(input_t_f, *args, **kwargs), result))
-        self.assertAlmostEqual(f(np.array(input_t_f), *args, **kwargs), result,
-                               msg="Not almost equal for np.arrays: %s != %s" % (
-                                   f(np.array(input_t_f), *args, **kwargs), result))
-        self.assertAlmostEqual(f(pd.Series(input_t_f), *args, **kwargs), result,
-                               msg="Not almost equal for pd.Series: %s != %s" % (
-                                   f(pd.Series(input_t_f), *args, **kwargs), result))
-
-    def assertIsNanOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
-        self.assertTrue(np.isnan(f(input_to_f, *args, **kwargs)), msg="Not NaN for lists")
-        self.assertTrue(np.isnan(f(np.array(input_to_f), *args, **kwargs)), msg="Not NaN for numpy.arrays")
-        self.assertTrue(np.isnan(f(pd.Series(input_to_f), *args, **kwargs)), msg="Not NaN for pandas.Series")
-
-    def assertEqualPandasSeriesWrapper(self, f, input_to_f, result, *args, **kwargs):
-        self.assertEqual(f(pd.Series(input_to_f), *args, **kwargs), result,
-                         msg="Not equal for pandas.Series: %s != %s" % (
-                             f(pd.Series(input_to_f), *args, **kwargs), result))
-
-    def test_catch_Numbers(self):
-        def f(x, y):
-            return [x, y]
-
-        fdeco = not_apply_to_raw_numbers(f)
-        self.assertEqual(fdeco(3, 5), 0)
-        self.assertEqual(fdeco([], 5), [[], 5])
-        self.assertEqual(fdeco(np.NaN, 10), 0)
-
-    def test___get_length_sequences_where(self):
-        self.assertEqualOnAllArrayTypes(_get_length_sequences_where, [0, 1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 1],
-                                        [1, 3, 1, 2])
-        self.assertEqualOnAllArrayTypes(_get_length_sequences_where,
-                                        [0, True, 0, 0, True, True, True, 0, 0, True, 0, True, True],
-                                        [1, 3, 1, 2])
-        self.assertEqualOnAllArrayTypes(_get_length_sequences_where,
-                                        [0, True, 0, 0, 1, True, 1, 0, 0, True, 0, 1, True], [1, 3, 1, 2])
-        self.assertEqualOnAllArrayTypes(_get_length_sequences_where, [0] * 10, [0])
-        self.assertEqualOnAllArrayTypes(_get_length_sequences_where, [], [0])
-
-    def test_variance_larger_than_standard_deviation(self):
-        self.assertFalseOnAllArrayTypes(variance_larger_than_standard_deviation, [-1, -1, 1, 1, 1])
-        self.assertTrueOnAllArrayTypes(variance_larger_than_standard_deviation, [-1, -1, 1, 1, 2])
-
-    def test_large_standard_deviation(self):
-        self.assertFalseOnAllArrayTypes(large_standard_deviation, [1, 1, 1, 1], r=0)
-        self.assertFalseOnAllArrayTypes(large_standard_deviation, [1, 1, 1, 1], r=0)
-        self.assertTrueOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0)
-        self.assertTrueOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0.25)
-        self.assertTrueOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0.3)
-        self.assertFalseOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0.5)
-
-    def test_symmetry_looking(self):
-        self.assertAllTrueOnAllArrayTypes(symmetry_looking, [-1, -1, 1, 1],
-                                          "c", [dict(r=0.05), dict(r=0.75)])
-        self.assertAllFalseOnAllArrayTypes(symmetry_looking, [-1, -1, 1, 1], "c", [dict(r=0)])
-        self.assertAllFalseOnAllArrayTypes(symmetry_looking, [-1, -1, -1, -1, 1], "c", [dict(r=0.05)])
-        self.assertAllTrueOnAllArrayTypes(symmetry_looking, [-2, -2, -2, -1, -1, -1], "c", [dict(r=0.05)])
-        self.assertAllTrueOnAllArrayTypes(symmetry_looking, [-0.9, -0.900001], "c", [dict(r=0.05)])
-
-    def test_has_duplicate_max(self):
-        self.assertTrueOnAllArrayTypes(has_duplicate_max, [2.1, 0, 0, 2.1, 1.1])
-        self.assertFalseOnAllArrayTypes(has_duplicate_max, np.array([2.1, 0, 0, 2, 1.1]))
-        self.assertTrueOnAllArrayTypes(has_duplicate_max, [1, 1, 1, 1])
-        self.assertFalseOnAllArrayTypes(has_duplicate_max, np.array([0]))
-        self.assertTrueOnAllArrayTypes(has_duplicate_max, np.array([1, 1]))
-
-    def test_has_duplicate_min(self):
-        self.assertTrueOnAllArrayTypes(has_duplicate_min, [-2.1, 0, 0, -2.1, 1.1])
-        self.assertFalseOnAllArrayTypes(has_duplicate_min, [2.1, 0, -1, 2, 1.1])
-        self.assertTrueOnAllArrayTypes(has_duplicate_min, np.array([1, 1, 1, 1]))
-        self.assertFalseOnAllArrayTypes(has_duplicate_min, np.array([0]))
-        self.assertTrueOnAllArrayTypes(has_duplicate_min, np.array([1, 1]))
-
-    def test_has_duplicate(self):
-        self.assertTrueOnAllArrayTypes(has_duplicate, np.array([-2.1, 0, 0, -2.1]))
-        self.assertTrueOnAllArrayTypes(has_duplicate, [-2.1, 2.1, 2.1, 2.1])
-        self.assertFalseOnAllArrayTypes(has_duplicate, [1.1, 1.2, 1.3, 1.4])
-        self.assertFalseOnAllArrayTypes(has_duplicate, [1])
-        self.assertFalseOnAllArrayTypes(has_duplicate, [])
-
-    def test_sum(self):
-        self.assertEqualOnAllArrayTypes(sum_values, [1, 2, 3, 4.1], 10.1)
-        self.assertEqualOnAllArrayTypes(sum_values, [-1.2, -2, -3, -4], -10.2)
-        self.assertEqualOnAllArrayTypes(sum_values, [], 0)
-
-    def test_large_number_of_peaks(self):
-        x = [0, 0, 1, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1]
-        self.assertTrueOnAllArrayTypes(large_number_of_peaks, x, 1)
-        self.assertTrueOnAllArrayTypes(large_number_of_peaks, x, 2)
-        self.assertFalseOnAllArrayTypes(large_number_of_peaks, x, 3)
-        self.assertFalseOnAllArrayTypes(large_number_of_peaks, x, 4)
-        self.assertFalseOnAllArrayTypes(large_number_of_peaks, x, 5)
-        self.assertFalseOnAllArrayTypes(large_number_of_peaks, x, 6)
-
-    def test_mean_autocorrelation(self):
-
-        x = [1, 1, 1, 1, 1, 1, 1]
-        self.assertAlmostEqualOnAllArrayTypes(mean_autocorrelation, x, 0)
-
-        x = [1, 2, -3]
-        expected_res = 1 / np.var(x) * (1 * 2 + 2 * (-3) - 3 / 2) / 2
-        self.assertAlmostEqualOnAllArrayTypes(mean_autocorrelation, x, expected_res)
-
-    def test_augmented_dickey_fuller(self):
-        pass
-        # todo: add unit test
-
-    def test_abs_energy(self):
-        self.assertEqualOnAllArrayTypes(abs_energy, [1, 1, 1], 3)
-        self.assertEqualOnAllArrayTypes(abs_energy, [1, 2, 3], 14)
-        self.assertEqualOnAllArrayTypes(abs_energy, [-1, 2, -3], 14)
-        self.assertAlmostEqualOnAllArrayTypes(abs_energy, [-1, 1.3], 2.69)
-        self.assertEqualOnAllArrayTypes(abs_energy, [1], 1)
-
-    def test_mean_abs_change(self):
-        self.assertEqualOnAllArrayTypes(mean_abs_change, [-2, 2, 5], 3.5)
-        self.assertEqualOnAllArrayTypes(mean_abs_change, [1, 2, -1], 2)
-
-    def test_mean_change(self):
-        self.assertEqualOnAllArrayTypes(mean_change, [-2, 2, 5], 3.5)
-        self.assertEqualOnAllArrayTypes(mean_change, [1, 2, -1], -1)
-
-    def test_mean_second_derivate_central(self):
-        self.assertEqualOnAllArrayTypes(mean_second_derivate_central, list(range(10)), 0)
-        self.assertEqualOnAllArrayTypes(mean_second_derivate_central, [1, 3, 5], 0)
-        self.assertEqualOnAllArrayTypes(mean_second_derivate_central, [1, 3, 7, -3], -3)
-
-    def test_median(self):
-        self.assertEqualOnAllArrayTypes(median, [1, 1, 2, 2], 1.5)
-        self.assertEqualOnAllArrayTypes(median, [0.5, 0.5, 2, 3.5, 10], 2)
-        self.assertEqualOnAllArrayTypes(median, [0.5], 0.5)
-        self.assertIsNanOnAllArrayTypes(median, [])
-
-    def test_mean(self):
-        self.assertEqualOnAllArrayTypes(mean, [1, 1, 2, 2], 1.5)
-        self.assertEqualOnAllArrayTypes(mean, [0.5, 0.5, 2, 3.5, 10], 3.3)
-        self.assertEqualOnAllArrayTypes(mean, [0.5], 0.5)
-        self.assertIsNanOnAllArrayTypes(mean, [])
-
-    def test_length(self):
-        self.assertEqualOnAllArrayTypes(length, [1, 2, 3, 4], 4)
-        self.assertEqualOnAllArrayTypes(length, [1, 2, 3], 3)
-        self.assertEqualOnAllArrayTypes(length, [1, 2], 2)
-        self.assertEqualOnAllArrayTypes(length, [1, 2, 3, np.NaN], 4)
-        self.assertEqualOnAllArrayTypes(length, [], 0)
-
-    def test_standard_deviation(self):
-        self.assertAlmostEqualOnAllArrayTypes(standard_deviation, [1, 1, -1, -1], 1)
-        self.assertAlmostEqualOnAllArrayTypes(standard_deviation, [1, 2, -2, -1], 1.58113883008)
-        self.assertIsNanOnAllArrayTypes(standard_deviation, [])
-
-    def test_variance(self):
-        self.assertAlmostEqualOnAllArrayTypes(variance, [1, 1, -1, -1], 1)
-        self.assertAlmostEqualOnAllArrayTypes(variance, [1, 2, -2, -1], 2.5)
-        self.assertIsNanOnAllArrayTypes(variance, [])
-
-    def test_skewness(self):
-        self.assertEqualOnAllArrayTypes(skewness, [1, 1, 1, 2, 2, 2], 0)
-        self.assertAlmostEqualOnAllArrayTypes(skewness, [1, 1, 1, 2, 2], 0.6085806194501855)
-        self.assertEqualOnAllArrayTypes(skewness, [1, 1, 1], 0)
-        self.assertIsNanOnAllArrayTypes(skewness, [1, 1])
-
-    def test_kurtosis(self):
-        self.assertAlmostEqualOnAllArrayTypes(kurtosis, [1, 1, 1, 2, 2], -3.333333333333333)
-        self.assertAlmostEqualOnAllArrayTypes(kurtosis, [1, 1, 1, 1], 0)
-        self.assertIsNanOnAllArrayTypes(kurtosis, [1, 1, 1])
-
-    def test_absolute_sum_of_changes(self):
-        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [1, 1, 1, 1, 2, 1], 2)
-        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [1, -1, 1, -1], 6)
-        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [1], 0)
-        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [], 0)
-
-    def test_longest_strike_below_mean(self):
-        self.assertEqualOnAllArrayTypes(longest_strike_below_mean, [1, 2, 1, 1, 1, 2, 2, 2], 3)
-        self.assertEqualOnAllArrayTypes(longest_strike_below_mean, [1, 2, 1], 1)
-        self.assertEqualOnAllArrayTypes(longest_strike_below_mean, [], 0)
-
-    def test_longest_strike_above_mean(self):
-        self.assertEqualOnAllArrayTypes(longest_strike_above_mean, [1, 2, 1, 2, 1, 2, 2, 1], 2)
-        self.assertEqualOnAllArrayTypes(longest_strike_above_mean, [1, 2, 1], 1)
-        self.assertEqualOnAllArrayTypes(longest_strike_above_mean, [], 0)
-
-    def test_count_above_mean(self):
-        self.assertEqualOnAllArrayTypes(count_above_mean, [1, 2, 1, 2, 1, 2], 3)
-        self.assertEqualOnAllArrayTypes(count_above_mean, [1, 1, 1, 1, 1, 2], 1)
-        self.assertEqualOnAllArrayTypes(count_above_mean, [1, 1, 1, 1, 1], 0)
-        self.assertEqualOnAllArrayTypes(count_above_mean, [], 0)
-
-    def test_count_below_mean(self):
-        self.assertEqualOnAllArrayTypes(count_below_mean, [1, 2, 1, 2, 1, 2], 3)
-        self.assertEqualOnAllArrayTypes(count_below_mean, [1, 1, 1, 1, 1, 2], 5)
-        self.assertEqualOnAllArrayTypes(count_below_mean, [1, 1, 1, 1, 1], 0)
-        self.assertEqualOnAllArrayTypes(count_below_mean, [], 0)
-
-    def test_last_location_maximum(self):
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1, 2, 1, 2, 1], 0.8)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1, 2, 1, 1, 2], 1.0)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [2, 1, 1, 1, 1], 0.2)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1, 1, 1, 1, 1], 1.0)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1], 1.0)
-        self.assertIsNanOnAllArrayTypes(last_location_of_maximum, [])
-
-    def test_first_location_of_maximum(self):
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1, 2, 1, 2, 1], 0.2)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1, 2, 1, 1, 2], 0.2)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [2, 1, 1, 1, 1], 0.0)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1, 1, 1, 1, 1], 0.0)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1], 0.0)
-        self.assertIsNanOnAllArrayTypes(first_location_of_maximum, [])
-
-    def test_last_location_of_minimum(self):
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1, 2, 1, 2, 1], 1.0)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1, 2, 1, 2, 2], 0.6)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [2, 1, 1, 1, 2], 0.8)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1, 1, 1, 1, 1], 1.0)
-        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1], 1.0)
-        self.assertIsNanOnAllArrayTypes(last_location_of_minimum, [])
-
-    def test_first_location_of_minimum(self):
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [1, 2, 1, 2, 1], 0.0)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [2, 2, 1, 2, 2], 0.4)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [2, 1, 1, 1, 2], 0.2)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [1, 1, 1, 1, 1], 0.0)
-        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [1], 0.0)
-        self.assertIsNanOnAllArrayTypes(first_location_of_minimum, [])
-
-    def test_percentage_of_doubled_datapoints(self):
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [1, 1, 2, 3, 4],
-                                              0.25)
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [1, 1.5, 2, 3], 0)
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [1], 0)
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints,
-                                              [1.111, -2.45, 1.111, 2.45], 1.0 / 3.0)
-        self.assertIsNanOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [])
-
-    def test_ratio_of_doubled_values(self):
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [1, 1, 2, 3, 4], 0.4)
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [1, 1.5, 2, 3], 0)
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [1], 0)
-        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values,
-                                              [1.111, -2.45, 1.111, 2.45], 0.5)
-        self.assertIsNanOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [])
-
-    def test_sum_of_reoccurring_values(self):
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1, 1, 2, 3, 4, 4], 5)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1, 1.5, 2, 3], 0)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1], 0)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1.111, -2.45, 1.111, 2.45], 1.111)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [], 0)
-
-    def test_sum_of_reoccurring_data_points(self):
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1, 1, 2, 3, 4, 4], 10)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1, 1.5, 2, 3], 0)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1], 0)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1.111, -2.45, 1.111, 2.45], 2.222)
-        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [], 0)
-
-    def test_uniqueness_factor(self):
-        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1, 1, 2, 3, 4], 0.8)
-        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1, 1.5, 2, 3], 1)
-        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1], 1)
-        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1.111, -2.45, 1.111, 2.45],
-                                              0.75)
-        self.assertIsNanOnAllArrayTypes(ratio_value_number_to_time_series_length, [])
-
-    def test_fft_coefficient(self):
-        pass
-        # todo: add unit test
-
-    def test_number_peaks(self):
-        x = np.array([0, 1, 2, 1, 0, 1, 2, 3, 4, 5, 4, 3, 2, 1])
-        self.assertEqualOnAllArrayTypes(number_peaks, x, 2, 1)
-        self.assertEqualOnAllArrayTypes(number_peaks, x, 2, 2)
-        self.assertEqualOnAllArrayTypes(number_peaks, x, 1, 3)
-        self.assertEqualOnAllArrayTypes(number_peaks, x, 1, 4)
-        self.assertEqualOnAllArrayTypes(number_peaks, x, 0, 5)
-        self.assertEqualOnAllArrayTypes(number_peaks, x, 0, 6)
-
-    def test_mass_quantile(self):
-
-        x = [1] * 101
-        c = "TEST"
-        param = [{"q": 0.5}]
-        expected_index = ["TEST__index_mass_quantile__q_0.5"]
-        res = index_mass_quantile(x, c, param)
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEqual(res["TEST__index_mass_quantile__q_0.5"], 0.5, places=1)
-
-        # Test for parts of pandas series
-        x = pd.Series([0] * 55 + [1] * 101)
-        c = "TEST"
-        param = [{"q": 0.5}]
-        expected_index = ["TEST__index_mass_quantile__q_0.5"]
-        res = index_mass_quantile(x[x > 0], c, param)
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEqual(res["TEST__index_mass_quantile__q_0.5"], 0.5, places=1)
-
-        x = [0] * 1000 + [1]
-        c = "TEST"
-        param = [{"q": 0.5}, {"q": 0.99}]
-        expected_index = ["TEST__index_mass_quantile__q_0.5", "TEST__index_mass_quantile__q_0.99"]
-        res = index_mass_quantile(x, c, param)
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEqual(res["TEST__index_mass_quantile__q_0.5"], 1, places=1)
-        self.assertAlmostEqual(res["TEST__index_mass_quantile__q_0.99"], 1, places=1)
-
-        x = [0, 1, 1, 0, 0, 1, 0, 0]
-        c = "TEST"
-        param = [{"q": 0.30}, {"q": 0.60}, {"q": 0.90}]
-        expected_index = ["TEST__index_mass_quantile__q_0.3", "TEST__index_mass_quantile__q_0.6",
-                          "TEST__index_mass_quantile__q_0.9"]
-        res = index_mass_quantile(x, c, param)
-        self.assertIsInstance(res, pd.Series)
-
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEqual(res["TEST__index_mass_quantile__q_0.3"], 0.25, places=1)
-        self.assertAlmostEqual(res["TEST__index_mass_quantile__q_0.6"], 0.375, places=1)
-        self.assertAlmostEqual(res["TEST__index_mass_quantile__q_0.9"], 0.75, places=1)
-
-        x = [0, 0, 0]
-        c = "TEST"
-        param = [{"q": 0.5}]
-        expected_index = ["TEST__index_mass_quantile__q_0.5"]
-        res = index_mass_quantile(x, c, param)
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertTrue(np.isnan(res["TEST__index_mass_quantile__q_0.5"]))
-
-        x = []
-        c = "TEST"
-        param = [{"q": 0.5}]
-        expected_index = ["TEST__index_mass_quantile__q_0.5"]
-        res = index_mass_quantile(x, c, param)
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertTrue(np.isnan(res["TEST__index_mass_quantile__q_0.5"]))
-
-    def test_number_cwt_peaks(self):
-        x = [1, 1, 1, 1, 1, 1, 1, 5, 1, 1, 1, 1, 1, 1, 5, 1, 1, 1, 1, 1, 1]
-        self.assertEqualOnAllArrayTypes(number_cwt_peaks, x, 2, 2)
-
-    def test_spkt_welch_density(self):
-        pass
-        # todo: add unit test
-
-    def test_cwt_coefficients(self):
-        x = [0.1, 0.2, 0.3]
-        c = "TEST"
-        param = [{"widths": (1, 2, 3), "coeff": 2, "w": 1},
-                 {"widths": (1, 3), "coeff": 2, "w": 3},
-                 {"widths": (1, 3), "coeff": 5, "w": 3}]
-        shuffle(param)
-
-        expected_index = ["TEST__cwt_coefficients__widths_(1, 2, 3)__coeff_2__w_1",
-                          "TEST__cwt_coefficients__widths_(1, 3)__coeff_2__w_3",
-                          "TEST__cwt_coefficients__widths_(1, 3)__coeff_5__w_3"]
-
-        res = cwt_coefficients(x, c, param)
-
-        # todo: add unit test for the values
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertTrue(math.isnan(res["TEST__cwt_coefficients__widths_(1, 3)__coeff_5__w_3"]))
-
-    def test_ar_coefficient(self):
-
-        # Test for X_i = 2.5 * X_{i-1} + 1
-        c = "TEST"
-        param = [{"k": 1, "coeff": 0}, {"k": 1, "coeff": 1}]
-        shuffle(param)
-
-        x = [1] + 9 * [0]
-        for i in range(1, len(x)):
-            x[i] = 2.5 * x[i - 1] + 1
-
-        res = ar_coefficient(x, c, param)
-        expected_index = ["TEST__ar_coefficient__k_1__coeff_0", "TEST__ar_coefficient__k_1__coeff_1"]
-
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEqual(res["TEST__ar_coefficient__k_1__coeff_0"], 1, places=2)
-        self.assertAlmostEqual(res["TEST__ar_coefficient__k_1__coeff_1"], 2.5, places=2)
-
-        # Test for X_i = 1.4 * X_{i-1} - 1 X_{i-2} + 1
-        c = "TEST"
-        param = [{"k": 1, "coeff": 0}, {"k": 1, "coeff": 1},
-                 {"k": 2, "coeff": 0}, {"k": 2, "coeff": 1}, {"k": 2, "coeff": 2}, {"k": 2, "coeff": 3}]
-        shuffle(param)
-
-        x = [1, 1] + 5 * [0]
-        for i in range(2, len(x)):
-            x[i] = (-2) * x[i - 2] + 3.5 * x[i - 1] + 1
-
-        res = ar_coefficient(x, c, param)
-        expected_index = ["TEST__ar_coefficient__k_1__coeff_0", "TEST__ar_coefficient__k_1__coeff_1",
-                          "TEST__ar_coefficient__k_2__coeff_0", "TEST__ar_coefficient__k_2__coeff_1",
-                          "TEST__ar_coefficient__k_2__coeff_2", "TEST__ar_coefficient__k_2__coeff_3"]
-
-        print(res.sort_index())
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEqual(res["TEST__ar_coefficient__k_2__coeff_0"], 1, places=2)
-        self.assertAlmostEqual(res["TEST__ar_coefficient__k_2__coeff_1"], 3.5, places=2)
-        self.assertAlmostEqual(res["TEST__ar_coefficient__k_2__coeff_2"], -2, places=2)
-        self.assertTrue(np.isnan(res["TEST__ar_coefficient__k_2__coeff_3"]))
-
-    def test_time_reversal_asymmetry_statistic(self):
-        x = [1] * 10
-        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 0)
-        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 1)
-        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 2)
-        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 3)
-
-        x = [1, 2, -3, 4]
-        # 1/2 * ( (4^2 * 2 + 3 * 2^2) + (3^2*1)-(2*1^1)) = 1/2 * (32+12+9-2) = 51/2
-        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 25.5, 1)
-        # 4^2 * 1 - 2 * 1^2 = 16 -2
-        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 14, 2)
-        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 3)
-
-    def test_binned_entropy(self):
-        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 100, 0, 10)
-        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 10 + [1], - (10 / 11 * np.math.log(10 / 11) +
-                                                                                  1 / 11 * np.math.log(1 / 11)), 10)
-        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 10 + [1], - (10 / 11 * np.math.log(10 / 11) +
-                                                                                  1 / 11 * np.math.log(1 / 11)), 10)
-        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 10 + [1], - (10 / 11 * np.math.log(10 / 11) +
-                                                                                  1 / 11 * np.math.log(1 / 11)), 100)
-        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, list(range(10)), - np.math.log(1 / 10), 100)
-        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, list(range(100)), - np.math.log(1 / 2), 2)
-
-    def test_sample_entropy(self):
-        ts = [1, 4, 5, 1, 7, 3, 1, 2, 5, 8, 9, 7, 3, 7, 9, 5, 4, 3, 9, 1, 2, 3, 4, 2, 9, 6, 7, 4, 9, 2, 9, 9, 6, 5, 1,
-              3, 8, 1, 5, 3, 8, 4, 1, 2, 2, 1, 6, 5, 3, 6, 5, 4, 8, 9, 6, 7, 5, 3, 2, 5, 4, 2, 5, 1, 6, 5, 3, 5, 6, 7,
-              8, 5, 2, 8, 6, 3, 8, 2, 7, 1, 7, 3, 5, 6, 2, 1, 3, 7, 3, 5, 3, 7, 6, 7, 7, 2, 3, 1, 7, 8]
-        self.assertAlmostEqualOnAllArrayTypes(sample_entropy, ts, 2.21187685)
-
-    def test_autocorrelation(self):
-        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], -1, 1)
-        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], 1, 2)
-        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], -1, 3)
-        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], 1, 4)
-        self.assertIsNanOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], 200)
-
-    def test_quantile(self):
-        self.assertAlmostEqualOnAllArrayTypes(quantile, [1, 1, 1, 3, 4, 7, 9, 11, 13, 13], 1.0, 0.2)
-        self.assertAlmostEqualOnAllArrayTypes(quantile, [1, 1, 1, 3, 4, 7, 9, 11, 13, 13], 13, 0.9)
-        self.assertAlmostEqualOnAllArrayTypes(quantile, [1, 1, 1, 3, 4, 7, 9, 11, 13, 13], 13, 1.0)
-        self.assertAlmostEqualOnAllArrayTypes(quantile, [1], 1, 0.5)
-        self.assertIsNanOnAllArrayTypes(quantile, [], 0.5)
-
-    def test_mean_abs_change_quantiles(self):
-
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, list(range(10)), 1, ql=0.1, qh=0.9)
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, list(range(10)), 0, ql=0.15, qh=0.18)
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, [0, 1, 0, 0, 0], 0.5, ql=0, qh=1)
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, [0, 1, 0, 0, 0], 0.5, ql=0.1, qh=1)
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, [0, 1, 0, 0, 0], 0, ql=0.1, qh=0.6)
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, [0, 1, -9, 0, 0], 5, ql=0, qh=1)
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, [0, 1, -9, 0, 0], 0.5, ql=0.1, qh=1)
-        self.assertAlmostEqualOnAllArrayTypes(mean_abs_change_quantiles, [0, 1, -9, 0, 0, 1, 0], 0.75, ql=0.1, qh=1)
-
-    def test_value_count(self):
-        self.assertEqualPandasSeriesWrapper(value_count, [1] * 10, 10, value=1)
-        self.assertEqualPandasSeriesWrapper(value_count, list(range(10)), 1, value=0)
-        self.assertEqualPandasSeriesWrapper(value_count, [1] * 10, 0, value=0)
-        self.assertEqualPandasSeriesWrapper(value_count, [np.NaN, 0, 1] * 3, 3, value=0)
-        self.assertEqualPandasSeriesWrapper(value_count, [np.NINF, 0, 1] * 3, 3, value=0)
-        self.assertEqualPandasSeriesWrapper(value_count, [np.PINF, 0, 1] * 3, 3, value=0)
-        self.assertEqualPandasSeriesWrapper(value_count, [0.1, 0.2, 0.3] * 3, 3, value=0.2)
-        self.assertEqualPandasSeriesWrapper(value_count, [np.NaN, 0, 1] * 3, 3, value=np.NaN)
-        self.assertEqualPandasSeriesWrapper(value_count, [np.NINF, 0, 1] * 3, 3, value=np.NINF)
-        self.assertEqualPandasSeriesWrapper(value_count, [np.PINF, 0, 1] * 3, 3, value=np.PINF)
-
-    def test_range_count(self):
-        self.assertEqualPandasSeriesWrapper(range_count, [1] * 10, 0, min=1, max=1)
-        self.assertEqualPandasSeriesWrapper(range_count, [1] * 10, 0, min=0.9, max=1)
-        self.assertEqualPandasSeriesWrapper(range_count, [1] * 10, 10, min=1, max=1.1)
-        self.assertEqualPandasSeriesWrapper(range_count, list(range(10)), 9, min=0, max=9)
-        self.assertEqualPandasSeriesWrapper(range_count, list(range(10)), 10, min=0, max=10)
-        self.assertEqualPandasSeriesWrapper(range_count, list(range(0, -10, -1)), 9, min=-10, max=0)
-        self.assertEqualPandasSeriesWrapper(range_count, [np.NaN, np.PINF, np.NINF] + list(range(10)), 10, min=0,
-                                            max=10)
-
-    def test_approximate_entropy(self):
-        self.assertEqualOnAllArrayTypes(approximate_entropy, [1], 0, m=2, r=0.5)
-        self.assertEqualOnAllArrayTypes(approximate_entropy, [1, 2], 0, m=2, r=0.5)
-        self.assertEqualOnAllArrayTypes(approximate_entropy, [1, 2, 3], 0, m=2, r=0.5)
-        self.assertEqualOnAllArrayTypes(approximate_entropy, [1, 2, 3], 0, m=2, r=0.5)
-        self.assertAlmostEqualOnAllArrayTypes(approximate_entropy, [12, 13, 15, 16, 17] * 10, 0.282456191, m=2, r=0.9)
-        self.assertRaises(ValueError, approximate_entropy, x=[12, 13, 15, 16, 17] * 10, m=2, r=-0.5)
-
-    def test_estimate_friedrich_coefficients(self):
-        """
-        Estimate friedrich coefficients
-        """
-        default_params = {"m": 3, "r": 30}
-
-        # active Brownian motion
-        ds = velocity(tau=3.8, delta_t=0.05, R=3e-4, seed=0)
-        v = ds.simulate(1000000, v0=np.zeros(1))
-        coeff = _estimate_friedrich_coefficients(v[:, 0], **default_params)
-        self.assertTrue(abs(coeff[-1]) < 0.0001)
-
-        # Brownian motion
-        ds = velocity(tau=2.0 / 0.3 - 3.8, delta_t=0.05, R=3e-4, seed=0)
-        v = ds.simulate(1000000, v0=np.zeros(1))
-        coeff = _estimate_friedrich_coefficients(v[:, 0], **default_params)
-        self.assertTrue(abs(coeff[-1]) < 0.0001)
-
-    def test_friedrich_coefficients(self):
-        # Test binning error returns vector of NaNs
-        c = "TEST"
-        param = [{"coeff": coeff, "m": 2, "r": 30} for coeff in range(4)]
-        x = np.zeros(1000)
-
-        res = friedrich_coefficients(x, c, param)
-        expected_index = ["TEST__friedrich_coefficients__m_2__r_30__coeff_0",
-                          "TEST__friedrich_coefficients__m_2__r_30__coeff_1",
-                          "TEST__friedrich_coefficients__m_2__r_30__coeff_2"]
-
-        self.assertIsInstance(res, pd.Series)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertTrue(np.sum(np.isnan(res)), 3)
-
-    def test_max_langevin_fixed_point(self):
-        """
-        Estimating the intrinsic velocity of a dissipative soliton
-        """
-        default_params = {"m": 3, "r": 30}
-
-        # active Brownian motion
-        ds = velocity(tau=3.8, delta_t=0.05, R=3e-4, seed=0)
-        v = ds.simulate(1000000, v0=np.zeros(1))
-        v0 = max_langevin_fixed_point(v[:, 0], **default_params)
-        self.assertTrue(abs(ds.deterministic - v0) < 0.0001)
-
-        # Brownian motion
-        ds = velocity(tau=2.0 / 0.3 - 3.8, delta_t=0.05, R=3e-4, seed=0)
-        v = ds.simulate(1000000, v0=np.zeros(1))
-        v0 = max_langevin_fixed_point(v[:, 0], **default_params)
-        self.assertTrue(v0 < 0.001)
-
-    def test_linear_trend(self):
-        # check linear up trend
-        x = range(10)
-        param = [{"attr": "pvalue"}, {"attr": "rvalue"}, {"attr": "intercept"}, {"attr": "slope"}, {"attr": "stderr"}]
-        c = "TEST"
-        res = linear_trend(x, c, param)
-
-        expected_index = ["TEST__linear_trend__attr_\"pvalue\"", "TEST__linear_trend__attr_\"intercept\"",
-                          "TEST__linear_trend__attr_\"rvalue\"", "TEST__linear_trend__attr_\"slope\"",
-                          "TEST__linear_trend__attr_\"stderr\""]
-
-        self.assertEqual(len(res), 5)
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEquals(res["TEST__linear_trend__attr_\"pvalue\""], 0)
-        self.assertAlmostEquals(res["TEST__linear_trend__attr_\"stderr\""], 0)
-        self.assertAlmostEquals(res["TEST__linear_trend__attr_\"intercept\""], 0)
-        self.assertAlmostEquals(res["TEST__linear_trend__attr_\"slope\""], 1.0)
-
-        # check p value for random trend
-        np.random.seed(42)
-        x = np.random.uniform(size=100)
-        param = [{"attr": "rvalue"}]
-        res = linear_trend(x, c, param)
-        self.assertLess(abs(res["TEST__linear_trend__attr_\"rvalue\""]), 0.1)
-
-        # check slope and intercept decreasing trend with intercept
-        x = [42 - 2 * x for x in range(10)]
-        param = [{"attr": "intercept"}, {"attr": "slope"}]
-        res = linear_trend(x, c, param)
-        self.assertAlmostEquals(res["TEST__linear_trend__attr_\"intercept\""], 42)
-        self.assertAlmostEquals(res["TEST__linear_trend__attr_\"slope\""], -2)
-
-    def test__aggregate_on_chunks(self):
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3]), f_agg="max", chunk_len=2), [1, 3])
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([1, 1, 3, 3]),  f_agg="max", chunk_len=2), [1, 3])
-
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3]), f_agg="min", chunk_len=2), [0, 2])
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3, 5]), f_agg="min", chunk_len=2), [0, 2, 5])
-
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3]), f_agg="mean", chunk_len=2), [0.5, 2.5])
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 0, 4, 5]), f_agg="mean", chunk_len=2), [0.5, 2, 5])
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 0, 4, 5]), f_agg="mean", chunk_len=3), [1/3, 4.5])
-
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3, 5, -2]),
-                                                  f_agg="median", chunk_len=2), [0.5, 2.5, 1.5])
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([-10, 5, 3, -3, 4, -6]),
-                                                  f_agg="median", chunk_len=3), [3, -3])
-        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, np.NaN, 5]),
-                                                  f_agg="median", chunk_len=2), [0.5, 2, 5])
-
-    def test_agg_linear_trend(self):
-        x = pd.Series(range(9), index=range(9))
-        c = "TEST"
-        param = [{"attr": "intercept", "chunk_len": 3, "f_agg": "max"},
-                 {"attr": "slope", "chunk_len": 3, "f_agg": "max"},
-                 {"attr": "intercept", "chunk_len": 3, "f_agg": "min"},
-                 {"attr": "slope", "chunk_len": 3, "f_agg": "min"},
-                 {"attr": "intercept", "chunk_len": 3, "f_agg": "mean"},
-                 {"attr": "slope", "chunk_len": 3, "f_agg": "mean"},
-                 {"attr": "intercept", "chunk_len": 3, "f_agg": "median"},
-                 {"attr": "slope", "chunk_len": 3, "f_agg": "median"}]
-        expected_index = ['TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"intercept"',
-                          'TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"slope"',
-                          'TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"intercept"',
-                          'TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"slope"',
-                          'TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"intercept"',
-                          'TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"slope"',
-                          'TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"intercept"',
-                          'TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"slope"']
-
-        res = agg_linear_trend(x=x, c=c, param=param)
-
-        self.assertEqual(len(res), 8)
-        print(res.index)
-        self.maxDiff = 2000
-        six.assertCountEqual(self, list(res.index), expected_index)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"intercept"'], 2)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"slope"'], 3)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"intercept"'], 0)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"slope"'], 3)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"intercept"'], 1)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"slope"'], 3)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"intercept"'], 1)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"slope"'], 3)
-
-        x = pd.Series([np.NaN, np.NaN, np.NaN, -3, -3, -3])
-        res = agg_linear_trend(x=x, c=c, param=param)
-
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"intercept"'])
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"slope"'])
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"intercept"'])
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"slope"'])
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"intercept"'])
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"slope"'])
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"intercept"'])
-        self.assertIsNaN(res['TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"slope"'])
-
-
-        x = pd.Series([np.NaN, np.NaN, -3, -3, -3, -3])
-        res = agg_linear_trend(x=x, c=c, param=param)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"intercept"'], -3)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"max"__chunk_len_3__attr_"slope"'], 0)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"intercept"'], -3)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"min"__chunk_len_3__attr_"slope"'], 0)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"intercept"'], -3)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"mean"__chunk_len_3__attr_"slope"'], 0)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"intercept"'], -3)
-        self.assertAlmostEquals(res['TEST__agg_linear_trend__f_agg_"median"__chunk_len_3__attr_"slope"'], 0)
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+from __future__ import absolute_import, division
+from __future__ import print_function
+from builtins import range
+from random import shuffle
+from unittest import TestCase
+from tsfresh.feature_extraction.feature_calculators import *
+from tsfresh.feature_extraction.feature_calculators import _get_length_sequences_where
+from tsfresh.feature_extraction.feature_calculators import _estimate_friedrich_coefficients
+from tsfresh.feature_extraction.feature_calculators import _aggregate_on_chunks
+from tsfresh.examples.driftbif_simulation import velocity
+import six
+import math
+from tsfresh.feature_extraction.settings import ComprehensiveFCParameters
+
+
+class FeatureCalculationTestCase(TestCase):
+
+    def assertIsNaN(self, result):
+        self.assertTrue(np.isnan(result), msg="{} is not np.NaN")
+
+    def assertEqualOnAllArrayTypes(self, f, input_to_f, result, *args, **kwargs):
+        self.assertEqual(f(input_to_f, *args, **kwargs), result,
+                         msg="Not equal for lists: %s != %s" % (f(input_to_f, *args, **kwargs), result))
+        self.assertEqual(f(np.array(input_to_f), *args, **kwargs), result,
+                         msg="Not equal for numpy.arrays: %s != %s" % (
+                         f(np.array(input_to_f), *args, **kwargs), result))
+        self.assertEqual(f(pd.Series(input_to_f), *args, **kwargs), result,
+                         msg="Not equal for pandas.Series: %s != %s" % (
+                         f(pd.Series(input_to_f), *args, **kwargs), result))
+
+    def assertTrueOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
+        self.assertTrue(f(input_to_f, *args, **kwargs), msg="Not true for lists")
+        self.assertTrue(f(np.array(input_to_f), *args, **kwargs), msg="Not true for numpy.arrays")
+        self.assertTrue(f(pd.Series(input_to_f), *args, **kwargs), msg="Not true for pandas.Series")
+
+    def assertAllTrueOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
+        self.assertTrue(all(dict(f(input_to_f, *args, **kwargs)).values()), msg="Not true for lists")
+        self.assertTrue(all(dict(f(np.array(input_to_f), *args, **kwargs)).values()), msg="Not true for numpy.arrays")
+        self.assertTrue(all(dict(f(pd.Series(input_to_f), *args, **kwargs)).values()), msg="Not true for pandas.Series")
+
+    def assertFalseOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
+        self.assertFalse(f(input_to_f, *args, **kwargs), msg="Not false for lists")
+        self.assertFalse(f(np.array(input_to_f), *args, **kwargs), msg="Not false for numpy.arrays")
+        self.assertFalse(f(pd.Series(input_to_f), *args, **kwargs), msg="Not false for pandas.Series")
+
+    def assertAllFalseOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
+        self.assertFalse(any(dict(f(input_to_f, *args, **kwargs)).values()), msg="Not false for lists")
+        self.assertFalse(any(dict(f(np.array(input_to_f), *args, **kwargs)).values()), msg="Not false for numpy.arrays")
+        self.assertFalse(any(dict(f(pd.Series(input_to_f), *args, **kwargs)).values()), msg="Not false for pandas.Series")
+
+    def assertAlmostEqualOnAllArrayTypes(self, f, input_t_f, result, *args, **kwargs):
+        self.assertAlmostEqual(f(input_t_f, *args, **kwargs), result,
+                               msg="Not almost equal for lists: %s != %s" % (f(input_t_f, *args, **kwargs), result))
+        self.assertAlmostEqual(f(np.array(input_t_f), *args, **kwargs), result,
+                               msg="Not almost equal for np.arrays: %s != %s" % (
+                                   f(np.array(input_t_f), *args, **kwargs), result))
+        self.assertAlmostEqual(f(pd.Series(input_t_f), *args, **kwargs), result,
+                               msg="Not almost equal for pd.Series: %s != %s" % (
+                                   f(pd.Series(input_t_f), *args, **kwargs), result))
+
+    def assertIsNanOnAllArrayTypes(self, f, input_to_f, *args, **kwargs):
+        self.assertTrue(np.isnan(f(input_to_f, *args, **kwargs)), msg="Not NaN for lists")
+        self.assertTrue(np.isnan(f(np.array(input_to_f), *args, **kwargs)), msg="Not NaN for numpy.arrays")
+        self.assertTrue(np.isnan(f(pd.Series(input_to_f), *args, **kwargs)), msg="Not NaN for pandas.Series")
+
+    def assertEqualPandasSeriesWrapper(self, f, input_to_f, result, *args, **kwargs):
+        self.assertEqual(f(pd.Series(input_to_f), *args, **kwargs), result,
+                         msg="Not equal for pandas.Series: %s != %s" % (
+                             f(pd.Series(input_to_f), *args, **kwargs), result))
+
+    def test___get_length_sequences_where(self):
+        self.assertEqualOnAllArrayTypes(_get_length_sequences_where, [0, 1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 1],
+                                        [1, 3, 1, 2])
+        self.assertEqualOnAllArrayTypes(_get_length_sequences_where,
+                                        [0, True, 0, 0, True, True, True, 0, 0, True, 0, True, True],
+                                        [1, 3, 1, 2])
+        self.assertEqualOnAllArrayTypes(_get_length_sequences_where,
+                                        [0, True, 0, 0, 1, True, 1, 0, 0, True, 0, 1, True], [1, 3, 1, 2])
+        self.assertEqualOnAllArrayTypes(_get_length_sequences_where, [0] * 10, [0])
+        self.assertEqualOnAllArrayTypes(_get_length_sequences_where, [], [0])
+
+    def test_variance_larger_than_standard_deviation(self):
+        self.assertFalseOnAllArrayTypes(variance_larger_than_standard_deviation, [-1, -1, 1, 1, 1])
+        self.assertTrueOnAllArrayTypes(variance_larger_than_standard_deviation, [-1, -1, 1, 1, 2])
+
+    def test_large_standard_deviation(self):
+        self.assertFalseOnAllArrayTypes(large_standard_deviation, [1, 1, 1, 1], r=0)
+        self.assertFalseOnAllArrayTypes(large_standard_deviation, [1, 1, 1, 1], r=0)
+        self.assertTrueOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0)
+        self.assertTrueOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0.25)
+        self.assertTrueOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0.3)
+        self.assertFalseOnAllArrayTypes(large_standard_deviation, [-1, -1, 1, 1], r=0.5)
+
+    def test_symmetry_looking(self):
+        self.assertAllTrueOnAllArrayTypes(symmetry_looking, [-1, -1, 1, 1],
+                                           [dict(r=0.05), dict(r=0.75)])
+        self.assertAllFalseOnAllArrayTypes(symmetry_looking, [-1, -1, 1, 1], [dict(r=0)])
+        self.assertAllFalseOnAllArrayTypes(symmetry_looking, [-1, -1, -1, -1, 1], [dict(r=0.05)])
+        self.assertAllTrueOnAllArrayTypes(symmetry_looking, [-2, -2, -2, -1, -1, -1], [dict(r=0.05)])
+        self.assertAllTrueOnAllArrayTypes(symmetry_looking, [-0.9, -0.900001], [dict(r=0.05)])
+
+    def test_has_duplicate_max(self):
+        self.assertTrueOnAllArrayTypes(has_duplicate_max, [2.1, 0, 0, 2.1, 1.1])
+        self.assertFalseOnAllArrayTypes(has_duplicate_max, np.array([2.1, 0, 0, 2, 1.1]))
+        self.assertTrueOnAllArrayTypes(has_duplicate_max, [1, 1, 1, 1])
+        self.assertFalseOnAllArrayTypes(has_duplicate_max, np.array([0]))
+        self.assertTrueOnAllArrayTypes(has_duplicate_max, np.array([1, 1]))
+
+    def test_has_duplicate_min(self):
+        self.assertTrueOnAllArrayTypes(has_duplicate_min, [-2.1, 0, 0, -2.1, 1.1])
+        self.assertFalseOnAllArrayTypes(has_duplicate_min, [2.1, 0, -1, 2, 1.1])
+        self.assertTrueOnAllArrayTypes(has_duplicate_min, np.array([1, 1, 1, 1]))
+        self.assertFalseOnAllArrayTypes(has_duplicate_min, np.array([0]))
+        self.assertTrueOnAllArrayTypes(has_duplicate_min, np.array([1, 1]))
+
+    def test_has_duplicate(self):
+        self.assertTrueOnAllArrayTypes(has_duplicate, np.array([-2.1, 0, 0, -2.1]))
+        self.assertTrueOnAllArrayTypes(has_duplicate, [-2.1, 2.1, 2.1, 2.1])
+        self.assertFalseOnAllArrayTypes(has_duplicate, [1.1, 1.2, 1.3, 1.4])
+        self.assertFalseOnAllArrayTypes(has_duplicate, [1])
+        self.assertFalseOnAllArrayTypes(has_duplicate, [])
+
+    def test_sum(self):
+        self.assertEqualOnAllArrayTypes(sum_values, [1, 2, 3, 4.1], 10.1)
+        self.assertEqualOnAllArrayTypes(sum_values, [-1.2, -2, -3, -4], -10.2)
+        self.assertEqualOnAllArrayTypes(sum_values, [], 0)
+
+    def test_agg_autocorrelation(self):
+
+        param = [{"f_agg": "mean"}]
+        x = [1, 1, 1, 1, 1, 1, 1]
+        expected_res = 0
+        res = dict(agg_autocorrelation(x, param=param))["f_agg_\"mean\""]
+        self.assertAlmostEqual(res, expected_res, places=4)
+
+        x = [1, 2, -3]
+        expected_res = 1 / np.var(x) * (((1 * 2 + 2 * (-3)) / 2 + (1 * -3)) / 2)
+        res = dict(agg_autocorrelation(x, param=param))["f_agg_\"mean\""]
+        self.assertAlmostEqual(res, expected_res, places=4)
+
+        np.random.seed(42)
+        x = np.random.normal(size=3000)
+        expected_res = 0
+        res = dict(agg_autocorrelation(x, param=param))["f_agg_\"mean\""]
+        self.assertAlmostEqual(res, expected_res, places=2)
+
+        param=[{"f_agg": "median"}]
+        x = [1, 1, 1, 1, 1, 1, 1]
+        expected_res = 0
+        res = dict(agg_autocorrelation(x, param=param))["f_agg_\"median\""]
+        self.assertAlmostEqual(res, expected_res, places=4)
+
+        x = [1, 2, -3]
+        expected_res = 1 / np.var(x) * (((1 * 2 + 2 * (-3)) / 2 + (1 * -3)) / 2)
+        res = dict(agg_autocorrelation(x, param=param))["f_agg_\"median\""]
+        self.assertAlmostEqual(res, expected_res, places=4)
+
+
+    def test_augmented_dickey_fuller(self):
+        # todo: add unit test for the values of the test statistic
+
+        # the adf hypothesis test checks for unit roots,
+        # so H_0 = {random drift} vs H_1 = {AR(1) model}
+
+        # H0 is true
+        np.random.seed(seed=42)
+        x = np.cumsum(np.random.uniform(size=100))
+        param = [{"attr": "teststat"}, {"attr": "pvalue"}, {"attr": "usedlag"}]
+        expected_index = ['attr_teststat', 'attr_pvalue', 'attr_usedlag']
+
+        res = augmented_dickey_fuller(x=x, param=param)
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertGreater(res["attr_pvalue"], 0.10)
+        self.assertEqual(res["attr_usedlag"], 0)
+
+        # H0 should be rejected for AR(1) model with x_{t} = 1/2 x_{t-1} + e_{t}
+        np.random.seed(seed=42)
+        e = np.random.normal(0.1, 0.1, size=100)
+        m = 50
+        x = [0] * m
+        x[0] = 100
+        for i in range(1, m):
+            x[i] = x[i-1] * 0.5 + e[i]
+        param = [{"attr": "teststat"}, {"attr": "pvalue"}, {"attr": "usedlag"}]
+        expected_index = ['attr_teststat', 'attr_pvalue', 'attr_usedlag']
+
+        res = augmented_dickey_fuller(x=x, param=param)
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertLessEqual(res["attr_pvalue"], 0.05)
+        self.assertEqual(res["attr_usedlag"], 0)
+
+    def test_abs_energy(self):
+        self.assertEqualOnAllArrayTypes(abs_energy, [1, 1, 1], 3)
+        self.assertEqualOnAllArrayTypes(abs_energy, [1, 2, 3], 14)
+        self.assertEqualOnAllArrayTypes(abs_energy, [-1, 2, -3], 14)
+        self.assertAlmostEqualOnAllArrayTypes(abs_energy, [-1, 1.3], 2.69)
+        self.assertEqualOnAllArrayTypes(abs_energy, [1], 1)
+
+    def test_ratio_beyond_r_sigma(self):
+
+        x = [0, 1]*10 + [10, 20, -30] # std of x is 7.21, mean 3.04
+        self.assertEqualOnAllArrayTypes(ratio_beyond_r_sigma, x, 3./len(x), r=1)
+        self.assertEqualOnAllArrayTypes(ratio_beyond_r_sigma, x, 2./len(x), r=2)
+        self.assertEqualOnAllArrayTypes(ratio_beyond_r_sigma, x, 1./len(x), r=3)
+        self.assertEqualOnAllArrayTypes(ratio_beyond_r_sigma, x, 0, r=20)
+
+    def test_mean_abs_change(self):
+        self.assertEqualOnAllArrayTypes(mean_abs_change, [-2, 2, 5], 3.5)
+        self.assertEqualOnAllArrayTypes(mean_abs_change, [1, 2, -1], 2)
+
+    def test_mean_change(self):
+        self.assertEqualOnAllArrayTypes(mean_change, [-2, 2, 5], 3.5)
+        self.assertEqualOnAllArrayTypes(mean_change, [1, 2, -1], -1)
+
+    def test_mean_second_derivate_central(self):
+        self.assertEqualOnAllArrayTypes(mean_second_derivate_central, list(range(10)), 0)
+        self.assertEqualOnAllArrayTypes(mean_second_derivate_central, [1, 3, 5], 0)
+        self.assertEqualOnAllArrayTypes(mean_second_derivate_central, [1, 3, 7, -3], -3)
+
+    def test_median(self):
+        self.assertEqualOnAllArrayTypes(median, [1, 1, 2, 2], 1.5)
+        self.assertEqualOnAllArrayTypes(median, [0.5, 0.5, 2, 3.5, 10], 2)
+        self.assertEqualOnAllArrayTypes(median, [0.5], 0.5)
+        self.assertIsNanOnAllArrayTypes(median, [])
+
+    def test_mean(self):
+        self.assertEqualOnAllArrayTypes(mean, [1, 1, 2, 2], 1.5)
+        self.assertEqualOnAllArrayTypes(mean, [0.5, 0.5, 2, 3.5, 10], 3.3)
+        self.assertEqualOnAllArrayTypes(mean, [0.5], 0.5)
+        self.assertIsNanOnAllArrayTypes(mean, [])
+
+    def test_length(self):
+        self.assertEqualOnAllArrayTypes(length, [1, 2, 3, 4], 4)
+        self.assertEqualOnAllArrayTypes(length, [1, 2, 3], 3)
+        self.assertEqualOnAllArrayTypes(length, [1, 2], 2)
+        self.assertEqualOnAllArrayTypes(length, [1, 2, 3, np.NaN], 4)
+        self.assertEqualOnAllArrayTypes(length, [], 0)
+
+    def test_standard_deviation(self):
+        self.assertAlmostEqualOnAllArrayTypes(standard_deviation, [1, 1, -1, -1], 1)
+        self.assertAlmostEqualOnAllArrayTypes(standard_deviation, [1, 2, -2, -1], 1.58113883008)
+        self.assertIsNanOnAllArrayTypes(standard_deviation, [])
+
+    def test_variance(self):
+        self.assertAlmostEqualOnAllArrayTypes(variance, [1, 1, -1, -1], 1)
+        self.assertAlmostEqualOnAllArrayTypes(variance, [1, 2, -2, -1], 2.5)
+        self.assertIsNanOnAllArrayTypes(variance, [])
+
+    def test_skewness(self):
+        self.assertEqualOnAllArrayTypes(skewness, [1, 1, 1, 2, 2, 2], 0)
+        self.assertAlmostEqualOnAllArrayTypes(skewness, [1, 1, 1, 2, 2], 0.6085806194501855)
+        self.assertEqualOnAllArrayTypes(skewness, [1, 1, 1], 0)
+        self.assertIsNanOnAllArrayTypes(skewness, [1, 1])
+
+    def test_kurtosis(self):
+        self.assertAlmostEqualOnAllArrayTypes(kurtosis, [1, 1, 1, 2, 2], -3.333333333333333)
+        self.assertAlmostEqualOnAllArrayTypes(kurtosis, [1, 1, 1, 1], 0)
+        self.assertIsNanOnAllArrayTypes(kurtosis, [1, 1, 1])
+
+    def test_absolute_sum_of_changes(self):
+        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [1, 1, 1, 1, 2, 1], 2)
+        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [1, -1, 1, -1], 6)
+        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [1], 0)
+        self.assertEqualOnAllArrayTypes(absolute_sum_of_changes, [], 0)
+
+    def test_longest_strike_below_mean(self):
+        self.assertEqualOnAllArrayTypes(longest_strike_below_mean, [1, 2, 1, 1, 1, 2, 2, 2], 3)
+        self.assertEqualOnAllArrayTypes(longest_strike_below_mean, [1, 2, 1], 1)
+        self.assertEqualOnAllArrayTypes(longest_strike_below_mean, [], 0)
+
+    def test_longest_strike_above_mean(self):
+        self.assertEqualOnAllArrayTypes(longest_strike_above_mean, [1, 2, 1, 2, 1, 2, 2, 1], 2)
+        self.assertEqualOnAllArrayTypes(longest_strike_above_mean, [1, 2, 1], 1)
+        self.assertEqualOnAllArrayTypes(longest_strike_above_mean, [], 0)
+
+    def test_count_above_mean(self):
+        self.assertEqualOnAllArrayTypes(count_above_mean, [1, 2, 1, 2, 1, 2], 3)
+        self.assertEqualOnAllArrayTypes(count_above_mean, [1, 1, 1, 1, 1, 2], 1)
+        self.assertEqualOnAllArrayTypes(count_above_mean, [1, 1, 1, 1, 1], 0)
+        self.assertEqualOnAllArrayTypes(count_above_mean, [], 0)
+
+    def test_count_below_mean(self):
+        self.assertEqualOnAllArrayTypes(count_below_mean, [1, 2, 1, 2, 1, 2], 3)
+        self.assertEqualOnAllArrayTypes(count_below_mean, [1, 1, 1, 1, 1, 2], 5)
+        self.assertEqualOnAllArrayTypes(count_below_mean, [1, 1, 1, 1, 1], 0)
+        self.assertEqualOnAllArrayTypes(count_below_mean, [], 0)
+
+    def test_last_location_maximum(self):
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1, 2, 1, 2, 1], 0.8)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1, 2, 1, 1, 2], 1.0)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [2, 1, 1, 1, 1], 0.2)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1, 1, 1, 1, 1], 1.0)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_maximum, [1], 1.0)
+        self.assertIsNanOnAllArrayTypes(last_location_of_maximum, [])
+
+    def test_first_location_of_maximum(self):
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1, 2, 1, 2, 1], 0.2)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1, 2, 1, 1, 2], 0.2)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [2, 1, 1, 1, 1], 0.0)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1, 1, 1, 1, 1], 0.0)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_maximum, [1], 0.0)
+        self.assertIsNanOnAllArrayTypes(first_location_of_maximum, [])
+
+    def test_last_location_of_minimum(self):
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1, 2, 1, 2, 1], 1.0)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1, 2, 1, 2, 2], 0.6)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [2, 1, 1, 1, 2], 0.8)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1, 1, 1, 1, 1], 1.0)
+        self.assertAlmostEqualOnAllArrayTypes(last_location_of_minimum, [1], 1.0)
+        self.assertIsNanOnAllArrayTypes(last_location_of_minimum, [])
+
+    def test_first_location_of_minimum(self):
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [1, 2, 1, 2, 1], 0.0)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [2, 2, 1, 2, 2], 0.4)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [2, 1, 1, 1, 2], 0.2)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [1, 1, 1, 1, 1], 0.0)
+        self.assertAlmostEqualOnAllArrayTypes(first_location_of_minimum, [1], 0.0)
+        self.assertIsNanOnAllArrayTypes(first_location_of_minimum, [])
+
+    def test_percentage_of_doubled_datapoints(self):
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [1, 1, 2, 3, 4],
+                                              0.25)
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [1, 1.5, 2, 3], 0)
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [1], 0)
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints,
+                                              [1.111, -2.45, 1.111, 2.45], 1.0 / 3.0)
+        self.assertIsNanOnAllArrayTypes(percentage_of_reoccurring_datapoints_to_all_datapoints, [])
+
+    def test_ratio_of_doubled_values(self):
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [1, 1, 2, 3, 4], 0.4)
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [1, 1.5, 2, 3], 0)
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [1], 0)
+        self.assertAlmostEqualOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values,
+                                              [1.111, -2.45, 1.111, 2.45], 0.5)
+        self.assertIsNanOnAllArrayTypes(percentage_of_reoccurring_values_to_all_values, [])
+
+    def test_sum_of_reoccurring_values(self):
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1, 1, 2, 3, 4, 4], 5)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1, 1.5, 2, 3], 0)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1], 0)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [1.111, -2.45, 1.111, 2.45], 1.111)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_values, [], 0)
+
+    def test_sum_of_reoccurring_data_points(self):
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1, 1, 2, 3, 4, 4], 10)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1, 1.5, 2, 3], 0)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1], 0)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [1.111, -2.45, 1.111, 2.45], 2.222)
+        self.assertAlmostEqualOnAllArrayTypes(sum_of_reoccurring_data_points, [], 0)
+
+    def test_uniqueness_factor(self):
+        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1, 1, 2, 3, 4], 0.8)
+        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1, 1.5, 2, 3], 1)
+        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1], 1)
+        self.assertAlmostEqualOnAllArrayTypes(ratio_value_number_to_time_series_length, [1.111, -2.45, 1.111, 2.45],
+                                              0.75)
+        self.assertIsNanOnAllArrayTypes(ratio_value_number_to_time_series_length, [])
+
+    def test_fft_coefficient(self):
+        x = range(10)
+        param = [{"coeff": 0, "attr": "real"}, {"coeff": 1, "attr": "real"}, {"coeff": 2, "attr": "real"},
+                 {"coeff": 0, "attr": "imag"}, {"coeff": 1, "attr": "imag"}, {"coeff": 2, "attr": "imag"},
+                 {"coeff": 0, "attr": "angle"}, {"coeff": 1, "attr": "angle"}, {"coeff": 2, "attr": "angle"},
+                 {"coeff": 0, "attr": "abs"}, {"coeff": 1, "attr": "abs"}, {"coeff": 2, "attr": "abs"} ]
+        expected_index = ['coeff_0__attr_"real"', 'coeff_1__attr_"real"', 'coeff_2__attr_"real"',
+                          'coeff_0__attr_"imag"', 'coeff_1__attr_"imag"', 'coeff_2__attr_"imag"',
+                          'coeff_0__attr_"angle"', 'coeff_1__attr_"angle"', 'coeff_2__attr_"angle"',
+                          'coeff_0__attr_"abs"', 'coeff_1__attr_"abs"', 'coeff_2__attr_"abs"']
+
+        res = pd.Series(dict(fft_coefficient(x, param)))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEqual(res['coeff_0__attr_"imag"'], 0, places=6)
+        self.assertAlmostEqual(res['coeff_0__attr_"real"'], sum(x), places=6)
+        self.assertAlmostEqual(res['coeff_0__attr_"angle"'], 0, places=6)
+        self.assertAlmostEqual(res['coeff_0__attr_"abs"'], sum(x), places=6)
+
+        x = [0, 1, 0, 0]
+        res = pd.Series(dict(fft_coefficient(x, param)))
+        # see documentation of fft in numpy
+        # should return array([1. + 0.j, 0. - 1.j, -1. + 0.j])
+        self.assertAlmostEqual(res['coeff_0__attr_"imag"'], 0, places=6)
+        self.assertAlmostEqual(res['coeff_0__attr_"real"'], 1, places=6)
+        self.assertAlmostEqual(res['coeff_1__attr_"imag"'], -1, places=6)
+        self.assertAlmostEqual(res['coeff_1__attr_"angle"'], -90, places=6)
+        self.assertAlmostEqual(res['coeff_1__attr_"real"'], 0, places=6)
+        self.assertAlmostEqual(res['coeff_2__attr_"imag"'], 0, places=6)
+        self.assertAlmostEqual(res['coeff_2__attr_"real"'], -1, places=6)
+
+        # test what happens if coeff is biger than time series lenght
+        x = range(5)
+        param = [{"coeff": 10, "attr": "real"}]
+        expected_index = ['coeff_10__attr_"real"']
+
+        res = pd.Series(dict(fft_coefficient(x, param)))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertIsNaN(res['coeff_10__attr_"real"'])
+
+    def test_number_peaks(self):
+        x = np.array([0, 1, 2, 1, 0, 1, 2, 3, 4, 5, 4, 3, 2, 1])
+        self.assertEqualOnAllArrayTypes(number_peaks, x, 2, 1)
+        self.assertEqualOnAllArrayTypes(number_peaks, x, 2, 2)
+        self.assertEqualOnAllArrayTypes(number_peaks, x, 1, 3)
+        self.assertEqualOnAllArrayTypes(number_peaks, x, 1, 4)
+        self.assertEqualOnAllArrayTypes(number_peaks, x, 0, 5)
+        self.assertEqualOnAllArrayTypes(number_peaks, x, 0, 6)
+
+    def test_mass_quantile(self):
+
+        x = [1] * 101
+        param = [{"q": 0.5}]
+        expected_index = ["q_0.5"]
+        res = index_mass_quantile(x, param)
+        
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEqual(res["q_0.5"], 0.5, places=1)
+
+        # Test for parts of pandas series
+        x = pd.Series([0] * 55 + [1] * 101)
+        param = [{"q": 0.5}]
+        expected_index = ["q_0.5"]
+        res = index_mass_quantile(x[x > 0], param)
+        
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEqual(res["q_0.5"], 0.5, places=1)
+
+        x = [0] * 1000 + [1]
+        param = [{"q": 0.5}, {"q": 0.99}]
+        expected_index = ["q_0.5", "q_0.99"]
+        res = index_mass_quantile(x, param)
+        
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEqual(res["q_0.5"], 1, places=1)
+        self.assertAlmostEqual(res["q_0.99"], 1, places=1)
+
+        x = [0, 1, 1, 0, 0, 1, 0, 0]
+        param = [{"q": 0.30}, {"q": 0.60}, {"q": 0.90}]
+        expected_index = ["q_0.3", "q_0.6",
+                          "q_0.9"]
+        res = index_mass_quantile(x, param)
+        
+        res = pd.Series(dict(res))
+
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEqual(res["q_0.3"], 0.25, places=1)
+        self.assertAlmostEqual(res["q_0.6"], 0.375, places=1)
+        self.assertAlmostEqual(res["q_0.9"], 0.75, places=1)
+
+        x = [0, 0, 0]
+        param = [{"q": 0.5}]
+        expected_index = ["q_0.5"]
+        res = index_mass_quantile(x, param)
+        
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertTrue(np.isnan(res["q_0.5"]))
+
+        x = []
+        param = [{"q": 0.5}]
+        expected_index = ["q_0.5"]
+        res = index_mass_quantile(x, param)
+        
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertTrue(np.isnan(res["q_0.5"]))
+
+    def test_number_cwt_peaks(self):
+        x = [1, 1, 1, 1, 1, 1, 1, 5, 1, 1, 1, 1, 1, 1, 5, 1, 1, 1, 1, 1, 1]
+        self.assertEqualOnAllArrayTypes(number_cwt_peaks, x, 2, 2)
+
+    def test_spkt_welch_density(self):
+
+        # todo: improve tests
+        x = range(10)
+        param = [{"coeff": 1}, {"coeff": 10}]
+        expected_index = ["coeff_1", "coeff_10"]
+        res = pd.Series(dict(spkt_welch_density(x, param)))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertIsNaN(res["coeff_10"])
+
+    def test_cwt_coefficients(self):
+        x = [0.1, 0.2, 0.3]
+        param = [{"widths": (1, 2, 3), "coeff": 2, "w": 1},
+                 {"widths": (1, 3), "coeff": 2, "w": 3},
+                 {"widths": (1, 3), "coeff": 5, "w": 3}]
+        shuffle(param)
+
+        expected_index = ["widths_(1, 2, 3)__coeff_2__w_1",
+                          "widths_(1, 3)__coeff_2__w_3",
+                          "widths_(1, 3)__coeff_5__w_3"]
+
+        res = cwt_coefficients(x, param)
+
+        
+        res = pd.Series(dict(res))
+
+        # todo: add unit test for the values
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertTrue(math.isnan(res["widths_(1, 3)__coeff_5__w_3"]))
+
+    def test_ar_coefficient(self):
+
+        # Test for X_i = 2.5 * X_{i-1} + 1
+        param = [{"k": 1, "coeff": 0}, {"k": 1, "coeff": 1}]
+        shuffle(param)
+
+        x = [1] + 9 * [0]
+        for i in range(1, len(x)):
+            x[i] = 2.5 * x[i - 1] + 1
+
+        res = ar_coefficient(x, param)
+        expected_index = ["k_1__coeff_0", "k_1__coeff_1"]
+
+        
+        res = pd.Series(dict(res))
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEqual(res["k_1__coeff_0"], 1, places=2)
+        self.assertAlmostEqual(res["k_1__coeff_1"], 2.5, places=2)
+
+        # Test for X_i = 1.4 * X_{i-1} - 1 X_{i-2} + 1
+        param = [{"k": 1, "coeff": 0}, {"k": 1, "coeff": 1},
+                 {"k": 2, "coeff": 0}, {"k": 2, "coeff": 1}, {"k": 2, "coeff": 2}, {"k": 2, "coeff": 3}]
+        shuffle(param)
+
+        x = [1, 1] + 5 * [0]
+        for i in range(2, len(x)):
+            x[i] = (-2) * x[i - 2] + 3.5 * x[i - 1] + 1
+
+        res = ar_coefficient(x, param)
+        expected_index = ["k_1__coeff_0", "k_1__coeff_1",
+                          "k_2__coeff_0", "k_2__coeff_1",
+                          "k_2__coeff_2", "k_2__coeff_3"]
+
+        
+        res = pd.Series(dict(res))
+
+        self.assertIsInstance(res, pd.Series)
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEqual(res["k_2__coeff_0"], 1, places=2)
+        self.assertAlmostEqual(res["k_2__coeff_1"], 3.5, places=2)
+        self.assertAlmostEqual(res["k_2__coeff_2"], -2, places=2)
+        self.assertTrue(np.isnan(res["k_2__coeff_3"]))
+
+    def test_time_reversal_asymmetry_statistic(self):
+        x = [1] * 10
+        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 0)
+        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 1)
+        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 2)
+        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 3)
+
+        x = [1, 2, -3, 4]
+        # 1/2 * ( (4^2 * -3 + 3 * 2^2) + (3^2*2)-(2*1^1)) = 1/2 * (-48+12+18-2) = 20/2
+        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, -10, 1)
+        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 2)
+        self.assertAlmostEqualOnAllArrayTypes(time_reversal_asymmetry_statistic, x, 0, 3)
+
+    def test_number_crossing_m(self):
+        x = [10, -10, 10, -10]
+        self.assertEqualOnAllArrayTypes(number_crossing_m, x, 3, 0)
+        self.assertEqualOnAllArrayTypes(number_crossing_m, x, 0, 10)
+
+        x = [10, 20, 20, 30]
+        self.assertEqualOnAllArrayTypes(number_crossing_m, x, 0, 0)
+        self.assertEqualOnAllArrayTypes(number_crossing_m, x, 1, 15)
+
+    def test_c3(self):
+        x = [1] * 10
+        self.assertAlmostEqualOnAllArrayTypes(c3, x, 1, 0)
+        self.assertAlmostEqualOnAllArrayTypes(c3, x, 1, 1)
+        self.assertAlmostEqualOnAllArrayTypes(c3, x, 1, 2)
+        self.assertAlmostEqualOnAllArrayTypes(c3, x, 1, 3)
+
+        x = [1, 2, -3, 4]
+        # 1/2 *(1*2*(-3)+2*(-3)*4) = 1/2 *(-6-24) = -30/2
+        self.assertAlmostEqualOnAllArrayTypes(c3, x, -15, 1)
+        self.assertAlmostEqualOnAllArrayTypes(c3, x, 0, 2)
+        self.assertAlmostEqualOnAllArrayTypes(c3, x, 0, 3)
+
+    def test_binned_entropy(self):
+        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 100, 0, 10)
+        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 10 + [1], - (10 / 11 * np.math.log(10 / 11) +
+                                                                                  1 / 11 * np.math.log(1 / 11)), 10)
+        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 10 + [1], - (10 / 11 * np.math.log(10 / 11) +
+                                                                                  1 / 11 * np.math.log(1 / 11)), 10)
+        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, [10] * 10 + [1], - (10 / 11 * np.math.log(10 / 11) +
+                                                                                  1 / 11 * np.math.log(1 / 11)), 100)
+        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, list(range(10)), - np.math.log(1 / 10), 100)
+        self.assertAlmostEqualOnAllArrayTypes(binned_entropy, list(range(100)), - np.math.log(1 / 2), 2)
+
+    def test_sample_entropy(self):
+        ts = [1, 4, 5, 1, 7, 3, 1, 2, 5, 8, 9, 7, 3, 7, 9, 5, 4, 3, 9, 1, 2, 3, 4, 2, 9, 6, 7, 4, 9, 2, 9, 9, 6, 5, 1,
+              3, 8, 1, 5, 3, 8, 4, 1, 2, 2, 1, 6, 5, 3, 6, 5, 4, 8, 9, 6, 7, 5, 3, 2, 5, 4, 2, 5, 1, 6, 5, 3, 5, 6, 7,
+              8, 5, 2, 8, 6, 3, 8, 2, 7, 1, 7, 3, 5, 6, 2, 1, 3, 7, 3, 5, 3, 7, 6, 7, 7, 2, 3, 1, 7, 8]
+        self.assertAlmostEqualOnAllArrayTypes(sample_entropy, ts, 2.21187685)
+
+    def test_autocorrelation(self):
+        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], -1, 1)
+        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], 1, 2)
+        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], -1, 3)
+        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], 1, 4)
+        self.assertAlmostEqualOnAllArrayTypes(autocorrelation, pd.Series([0, 1, 2, 0, 1, 2]), -0.75, 2)
+        # Autocorrelation lag is larger than length of the time series
+        self.assertIsNanOnAllArrayTypes(autocorrelation, [1, 2, 1, 2, 1, 2], 200)
+        self.assertIsNanOnAllArrayTypes(autocorrelation, [np.nan], 0)
+        self.assertIsNanOnAllArrayTypes(autocorrelation, [], 0)
+        # time series with length 1 has no variance, therefore no result for autocorrelation at lag 0
+        self.assertIsNanOnAllArrayTypes(autocorrelation, [1], 0)
+
+    def test_quantile(self):
+        self.assertAlmostEqualOnAllArrayTypes(quantile, [1, 1, 1, 3, 4, 7, 9, 11, 13, 13], 1.0, 0.2)
+        self.assertAlmostEqualOnAllArrayTypes(quantile, [1, 1, 1, 3, 4, 7, 9, 11, 13, 13], 13, 0.9)
+        self.assertAlmostEqualOnAllArrayTypes(quantile, [1, 1, 1, 3, 4, 7, 9, 11, 13, 13], 13, 1.0)
+        self.assertAlmostEqualOnAllArrayTypes(quantile, [1], 1, 0.5)
+        self.assertIsNanOnAllArrayTypes(quantile, [], 0.5)
+
+    def test_mean_abs_change_quantiles(self):
+
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, list(range(10)), 1,
+                                              ql=0.1, qh=0.9, isabs=True, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, list(range(10)), 0,
+                                              ql=0.15, qh=0.18, isabs=True, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 0, 0], 0.5,
+                                              ql=0, qh=1, isabs=True, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 0, 0], 0.5,
+                                              ql=0.1, qh=1, isabs=True, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 0, 0], 0,
+                                              ql=0.1, qh=0.6, isabs=True, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, -9, 0, 0], 5,
+                                              ql=0, qh=1, isabs=True, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, -9, 0, 0], 0.5,
+                                              ql=0.1, qh=1, isabs=True, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, -9, 0, 0, 1, 0], 0.75,
+                                              ql=0.1, qh=1, isabs=True, f_agg="mean")
+        
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, list(range(10)), 1,
+                                              ql=0.1, qh=0.9, isabs=False, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, list(range(10)), 0,
+                                              ql=0.15, qh=0.18, isabs=False, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 0, 0], 0,
+                                              ql=0, qh=1, isabs=False, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 0, 0], 0,
+                                              ql=0.1, qh=1, isabs=False, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 0, 0], 0,
+                                              ql=0.1, qh=0.6, isabs=False, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, -9, 0, 0], 0,
+                                              ql=0, qh=1, isabs=False, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, -9, 0, 0], 0.5,
+                                              ql=0.1, qh=1, isabs=False, f_agg="mean")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, -9, 0, 0, 1, 0], 0.25,
+                                              ql=0.1, qh=1, isabs=False, f_agg="mean")
+
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, list(range(10)), 0,
+                                              ql=0.1, qh=0.9, isabs=True, f_agg="std")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 0, 0], 0.5,
+                                              ql=0, qh=1, isabs=True, f_agg="std")
+
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, list(range(10)), 0,
+                                              ql=0.1, qh=0.9, isabs=False, f_agg="std")
+        self.assertAlmostEqualOnAllArrayTypes(change_quantiles, [0, 1, 0, 1, 0], 1,
+                                              ql=0, qh=1, isabs=False, f_agg="std")
+
+    def test_value_count(self):
+        self.assertEqualPandasSeriesWrapper(value_count, [1] * 10, 10, value=1)
+        self.assertEqualPandasSeriesWrapper(value_count, list(range(10)), 1, value=0)
+        self.assertEqualPandasSeriesWrapper(value_count, [1] * 10, 0, value=0)
+        self.assertEqualPandasSeriesWrapper(value_count, [np.NaN, 0, 1] * 3, 3, value=0)
+        self.assertEqualPandasSeriesWrapper(value_count, [np.NINF, 0, 1] * 3, 3, value=0)
+        self.assertEqualPandasSeriesWrapper(value_count, [np.PINF, 0, 1] * 3, 3, value=0)
+        self.assertEqualPandasSeriesWrapper(value_count, [0.1, 0.2, 0.3] * 3, 3, value=0.2)
+        self.assertEqualPandasSeriesWrapper(value_count, [np.NaN, 0, 1] * 3, 3, value=np.NaN)
+        self.assertEqualPandasSeriesWrapper(value_count, [np.NINF, 0, 1] * 3, 3, value=np.NINF)
+        self.assertEqualPandasSeriesWrapper(value_count, [np.PINF, 0, 1] * 3, 3, value=np.PINF)
+
+    def test_range_count(self):
+        self.assertEqualPandasSeriesWrapper(range_count, [1] * 10, 0, min=1, max=1)
+        self.assertEqualPandasSeriesWrapper(range_count, [1] * 10, 0, min=0.9, max=1)
+        self.assertEqualPandasSeriesWrapper(range_count, [1] * 10, 10, min=1, max=1.1)
+        self.assertEqualPandasSeriesWrapper(range_count, list(range(10)), 9, min=0, max=9)
+        self.assertEqualPandasSeriesWrapper(range_count, list(range(10)), 10, min=0, max=10)
+        self.assertEqualPandasSeriesWrapper(range_count, list(range(0, -10, -1)), 9, min=-10, max=0)
+        self.assertEqualPandasSeriesWrapper(range_count, [np.NaN, np.PINF, np.NINF] + list(range(10)), 10, min=0,
+                                            max=10)
+
+    def test_approximate_entropy(self):
+        self.assertEqualOnAllArrayTypes(approximate_entropy, [1], 0, m=2, r=0.5)
+        self.assertEqualOnAllArrayTypes(approximate_entropy, [1, 2], 0, m=2, r=0.5)
+        self.assertEqualOnAllArrayTypes(approximate_entropy, [1, 2, 3], 0, m=2, r=0.5)
+        self.assertEqualOnAllArrayTypes(approximate_entropy, [1, 2, 3], 0, m=2, r=0.5)
+        self.assertAlmostEqualOnAllArrayTypes(approximate_entropy, [12, 13, 15, 16, 17] * 10, 0.282456191, m=2, r=0.9)
+        self.assertRaises(ValueError, approximate_entropy, x=[12, 13, 15, 16, 17] * 10, m=2, r=-0.5)
+
+    def test_estimate_friedrich_coefficients(self):
+        """
+        Estimate friedrich coefficients
+        """
+        default_params = {"m": 3, "r": 30}
+
+        # active Brownian motion
+        ds = velocity(tau=3.8, delta_t=0.05, R=3e-4, seed=0)
+        v = ds.simulate(1000000, v0=np.zeros(1))
+        coeff = _estimate_friedrich_coefficients(v[:, 0], **default_params)
+        self.assertTrue(abs(coeff[-1]) < 0.0001)
+
+        # Brownian motion
+        ds = velocity(tau=2.0 / 0.3 - 3.8, delta_t=0.05, R=3e-4, seed=0)
+        v = ds.simulate(1000000, v0=np.zeros(1))
+        coeff = _estimate_friedrich_coefficients(v[:, 0], **default_params)
+        self.assertTrue(abs(coeff[-1]) < 0.0001)
+
+    def test_friedrich_coefficients(self):
+        # Test binning error returns vector of NaNs
+        param = [{"coeff": coeff, "m": 2, "r": 30} for coeff in range(4)]
+        x = np.zeros(1000)
+
+        res = friedrich_coefficients(x, param)
+        
+        res = pd.Series(dict(res))
+
+        expected_index = ["m_2__r_30__coeff_0",
+                          "m_2__r_30__coeff_1",
+                          "m_2__r_30__coeff_2"]
+
+        self.assertIsInstance(res, pd.Series)
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertTrue(np.sum(np.isnan(res)), 3)
+
+    def test_max_langevin_fixed_point(self):
+        """
+        Estimating the intrinsic velocity of a dissipative soliton
+        """
+        default_params = {"m": 3, "r": 30}
+
+        # active Brownian motion
+        ds = velocity(tau=3.8, delta_t=0.05, R=3e-4, seed=0)
+        v = ds.simulate(1000000, v0=np.zeros(1))
+        v0 = max_langevin_fixed_point(v[:, 0], **default_params)
+        self.assertTrue(abs(ds.deterministic - v0) < 0.0001)
+
+        # Brownian motion
+        ds = velocity(tau=2.0 / 0.3 - 3.8, delta_t=0.05, R=3e-4, seed=0)
+        v = ds.simulate(1000000, v0=np.zeros(1))
+        v0 = max_langevin_fixed_point(v[:, 0], **default_params)
+        self.assertTrue(v0 < 0.001)
+
+    def test_linear_trend(self):
+        # check linear up trend
+        x = range(10)
+        param = [{"attr": "pvalue"}, {"attr": "rvalue"}, {"attr": "intercept"}, {"attr": "slope"}, {"attr": "stderr"}]
+        res = linear_trend(x, param)
+
+
+        res = pd.Series(dict(res))
+
+        expected_index = ["attr_\"pvalue\"", "attr_\"intercept\"",
+                          "attr_\"rvalue\"", "attr_\"slope\"",
+                          "attr_\"stderr\""]
+
+        self.assertEqual(len(res), 5)
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEquals(res["attr_\"pvalue\""], 0)
+        self.assertAlmostEquals(res["attr_\"stderr\""], 0)
+        self.assertAlmostEquals(res["attr_\"intercept\""], 0)
+        self.assertAlmostEquals(res["attr_\"slope\""], 1.0)
+
+        # check p value for random trend
+        np.random.seed(42)
+        x = np.random.uniform(size=100)
+        param = [{"attr": "rvalue"}]
+        res = linear_trend(x, param)
+
+        
+        res = pd.Series(dict(res))
+
+        self.assertLess(abs(res["attr_\"rvalue\""]), 0.1)
+
+        # check slope and intercept decreasing trend with intercept
+        x = [42 - 2 * x for x in range(10)]
+        param = [{"attr": "intercept"}, {"attr": "slope"}]
+        res = linear_trend(x, param)
+
+        
+        res = pd.Series(dict(res))
+
+        self.assertAlmostEquals(res["attr_\"intercept\""], 42)
+        self.assertAlmostEquals(res["attr_\"slope\""], -2)
+
+    def test__aggregate_on_chunks(self):
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3]), f_agg="max", chunk_len=2), [1, 3])
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([1, 1, 3, 3]),  f_agg="max", chunk_len=2), [1, 3])
+
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3]), f_agg="min", chunk_len=2), [0, 2])
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3, 5]), f_agg="min", chunk_len=2), [0, 2, 5])
+
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3]), f_agg="mean", chunk_len=2), [0.5, 2.5])
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 0, 4, 5]), f_agg="mean", chunk_len=2), [0.5, 2, 5])
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 0, 4, 5]), f_agg="mean", chunk_len=3), [1/3, 4.5])
+
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, 3, 5, -2]),
+                                                  f_agg="median", chunk_len=2), [0.5, 2.5, 1.5])
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([-10, 5, 3, -3, 4, -6]),
+                                                  f_agg="median", chunk_len=3), [3, -3])
+        self.assertListEqual(_aggregate_on_chunks(x=pd.Series([0, 1, 2, np.NaN, 5]),
+                                                  f_agg="median", chunk_len=2), [0.5, 2, 5])
+
+    def test_agg_linear_trend(self):
+        x = pd.Series(range(9), index=range(9))
+        param = [{"attr": "intercept", "chunk_len": 3, "f_agg": "max"},
+                 {"attr": "slope", "chunk_len": 3, "f_agg": "max"},
+                 {"attr": "intercept", "chunk_len": 3, "f_agg": "min"},
+                 {"attr": "slope", "chunk_len": 3, "f_agg": "min"},
+                 {"attr": "intercept", "chunk_len": 3, "f_agg": "mean"},
+                 {"attr": "slope", "chunk_len": 3, "f_agg": "mean"},
+                 {"attr": "intercept", "chunk_len": 3, "f_agg": "median"},
+                 {"attr": "slope", "chunk_len": 3, "f_agg": "median"}]
+        expected_index = ['f_agg_"max"__chunk_len_3__attr_"intercept"',
+                          'f_agg_"max"__chunk_len_3__attr_"slope"',
+                          'f_agg_"min"__chunk_len_3__attr_"intercept"',
+                          'f_agg_"min"__chunk_len_3__attr_"slope"',
+                          'f_agg_"mean"__chunk_len_3__attr_"intercept"',
+                          'f_agg_"mean"__chunk_len_3__attr_"slope"',
+                          'f_agg_"median"__chunk_len_3__attr_"intercept"',
+                          'f_agg_"median"__chunk_len_3__attr_"slope"']
+
+        res = agg_linear_trend(x=x, param=param)
+
+        res = pd.Series(dict(res))
+        self.assertEqual(len(res), 8)
+        self.maxDiff = 2000
+        six.assertCountEqual(self, list(res.index), expected_index)
+        self.assertAlmostEquals(res['f_agg_"max"__chunk_len_3__attr_"intercept"'], 2)
+        self.assertAlmostEquals(res['f_agg_"max"__chunk_len_3__attr_"slope"'], 3)
+        self.assertAlmostEquals(res['f_agg_"min"__chunk_len_3__attr_"intercept"'], 0)
+        self.assertAlmostEquals(res['f_agg_"min"__chunk_len_3__attr_"slope"'], 3)
+        self.assertAlmostEquals(res['f_agg_"mean"__chunk_len_3__attr_"intercept"'], 1)
+        self.assertAlmostEquals(res['f_agg_"mean"__chunk_len_3__attr_"slope"'], 3)
+        self.assertAlmostEquals(res['f_agg_"median"__chunk_len_3__attr_"intercept"'], 1)
+        self.assertAlmostEquals(res['f_agg_"median"__chunk_len_3__attr_"slope"'], 3)
+
+        x = pd.Series([np.NaN, np.NaN, np.NaN, -3, -3, -3])
+        res = agg_linear_trend(x=x, param=param)
+
+        
+        res = pd.Series(dict(res))
+
+        self.assertIsNaN(res['f_agg_"max"__chunk_len_3__attr_"intercept"'])
+        self.assertIsNaN(res['f_agg_"max"__chunk_len_3__attr_"slope"'])
+        self.assertIsNaN(res['f_agg_"min"__chunk_len_3__attr_"intercept"'])
+        self.assertIsNaN(res['f_agg_"min"__chunk_len_3__attr_"slope"'])
+        self.assertIsNaN(res['f_agg_"mean"__chunk_len_3__attr_"intercept"'])
+        self.assertIsNaN(res['f_agg_"mean"__chunk_len_3__attr_"slope"'])
+        self.assertIsNaN(res['f_agg_"median"__chunk_len_3__attr_"intercept"'])
+        self.assertIsNaN(res['f_agg_"median"__chunk_len_3__attr_"slope"'])
+
+        x = pd.Series([np.NaN, np.NaN, -3, -3, -3, -3])
+        res = agg_linear_trend(x=x, param=param)
+
+        
+        res = pd.Series(dict(res))
+
+        self.assertAlmostEquals(res['f_agg_"max"__chunk_len_3__attr_"intercept"'], -3)
+        self.assertAlmostEquals(res['f_agg_"max"__chunk_len_3__attr_"slope"'], 0)
+        self.assertAlmostEquals(res['f_agg_"min"__chunk_len_3__attr_"intercept"'], -3)
+        self.assertAlmostEquals(res['f_agg_"min"__chunk_len_3__attr_"slope"'], 0)
+        self.assertAlmostEquals(res['f_agg_"mean"__chunk_len_3__attr_"intercept"'], -3)
+        self.assertAlmostEquals(res['f_agg_"mean"__chunk_len_3__attr_"slope"'], 0)
+        self.assertAlmostEquals(res['f_agg_"median"__chunk_len_3__attr_"intercept"'], -3)
+        self.assertAlmostEquals(res['f_agg_"median"__chunk_len_3__attr_"slope"'], 0)
+
+    def test_energy_ratio_by_chunks(self):
+        x = pd.Series(range(90), index=range(90))
+        param = [{"num_segments" : 6, "segment_focus": i} for i in range(6)]
+        output = energy_ratio_by_chunks(x=x, param=param)
+
+        self.assertAlmostEqual(output[0][1], 0.0043, places=3)
+        self.assertAlmostEqual(output[1][1], 0.0316, places=3)
+        self.assertAlmostEqual(output[2][1], 0.0871, places=3)
+        self.assertAlmostEqual(output[3][1], 0.1709, places=3)
+        self.assertAlmostEqual(output[4][1], 0.2829, places=3)
+        self.assertAlmostEqual(output[5][1], 0.4232, places=3)
+
+        # Sum of the ratios should be 1.0
+        sum = 0.0
+        for name,dat in output:
+            sum = sum + dat
+        self.assertAlmostEqual(sum, 1.0)
+
+
+
+    def test_ComprehensiveFCParameters(self):
+        import pprint
+        pp = pprint.PrettyPrinter(indent=4)
+        pp.pprint(ComprehensiveFCParameters())
```

### Comparing `tsfresh-0.8.1/tests/feature_extraction/test_settings.py` & `tsfresh-0.9.0/tests/feature_extraction/test_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
 
 from __future__ import absolute_import, division
 
 from unittest import TestCase
 import numpy as np
 import pandas as pd
-from tsfresh.feature_extraction.extraction import extract_features, _extract_features_for_one_time_series
+from tsfresh.feature_extraction.extraction import extract_features
 from tsfresh.feature_extraction.settings import ComprehensiveFCParameters, MinimalFCParameters, \
     EfficientFCParameters, from_columns
 import six
 from tsfresh.feature_extraction import feature_calculators
 
 
 class TestSettingsObject(TestCase):
@@ -106,33 +106,22 @@
         self.assertIn("median", mfs)
         self.assertIn("minimum", mfs)
         self.assertIn("maximum", mfs)
         self.assertIn("length", mfs)
         self.assertIn("sum_values", mfs)
         self.assertIn("standard_deviation", mfs)
         self.assertIn("variance", mfs)
+        self.assertNotIn("fft_coefficient", mfs)
 
     def test_extraction_runs_through(self):
         mfs = MinimalFCParameters()
 
         data = pd.DataFrame([[0, 0, 0, 0], [1, 0, 0, 0]], columns=["id", "time", "kind", "value"])
 
         extracted_features = extract_features(data, default_fc_parameters=mfs,
                                               column_kind="kind", column_value="value",
                                               column_sort="time", column_id="id")
 
         six.assertCountEqual(self, extracted_features.columns, ["0__median", "0__standard_deviation", "0__sum_values",
                                                                 "0__maximum", "0__variance", "0__minimum", "0__mean",
                                                                 "0__length"])
-        six.assertCountEqual(self, extracted_features.index, [0, 1])
-
-    def test_extraction_for_one_time_series_runs_through(self):
-        mfs = MinimalFCParameters()
-
-        data = pd.DataFrame([[0, 0, 0, 0], [1, 0, 0, 0]], columns=["id", "time", "kind", "value"])
-        extracted_features = _extract_features_for_one_time_series([0, data],
-                                                                   default_fc_parameters=mfs,
-                                                                   column_value="value", column_id="id")
-        six.assertCountEqual(self, extracted_features.columns,
-                             ["0__median", "0__standard_deviation", "0__sum_values", "0__maximum", "0__variance",
-                              "0__minimum", "0__mean", "0__length"])
-        six.assertCountEqual(self, extracted_features.index, [0, 1])
+        six.assertCountEqual(self, extracted_features.index, [0, 1])
```

### Comparing `tsfresh-0.8.1/tests/fixtures.py` & `tsfresh-0.9.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/scripts/test_run_tsfresh.py` & `tsfresh-0.9.0/tests/scripts/test_run_tsfresh.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/test_feature_significance.py` & `tsfresh-0.9.0/tests/test_feature_significance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-import numpy as np
-import pandas as pd
-from unittest import TestCase
-import tsfresh.feature_selection.feature_selector
-
-
-class FeatureSignificanceTestCase(TestCase):
-    """Test cases for the whole feature selection algorithm."""
-
-    def setUp(self):
-        """Fix the random seed."""
-        np.random.seed(seed=42)
-
-    def test_binary_target_mixed_case(self):
-        # Mixed case with binomial target
-        np.random.seed(42)
-        y = pd.Series(np.random.binomial(1, 0.5, 1000))
-        X = pd.DataFrame(index=range(1000))
-
-        z = y - np.random.binomial(1, 0.1, 1000) + np.random.binomial(1, 0.1, 1000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-
-        X["rel1"] = z
-        X["rel2"] = y * np.abs(np.random.normal(0, 1, 1000)) + np.random.normal(0, 1, 1000)
-        X["rel3"] = y + np.random.normal(0, 0.3, 1000)
-        X["rel4"] = y ** 2 + np.random.normal(0, 1, 1000)
-        X["rel5"] = np.sqrt(y) + np.random.binomial(2, 0.1, 1000)
-
-        X["irr_constant"] = 1.113344
-
-        X["irr1"] = np.random.normal(0, 1, 1000)
-        X["irr2"] = np.random.poisson(1, 1000)
-        X["irr3"] = np.random.binomial(1, 0.3, 1000)
-        X["irr4"] = np.random.normal(0, 1, 1000)
-        X["irr5"] = np.random.poisson(1, 1000)
-        X["irr6"] = np.random.binomial(1, 0.3, 1000)
-        X["irr7"] = np.random.normal(0, 1, 1000)
-        X["irr8"] = np.random.poisson(1, 1000)
-        X["irr9"] = np.random.binomial(1, 0.3, 1000)
-
-        df_bh = tsfresh.feature_selection.feature_selector.check_fs_sig_bh(X, y)
-        feat_rej = df_bh.loc[df_bh.rejected].Feature
-
-        # Make sure all selected variables are relevant
-        for kept_feature in feat_rej:
-            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4', 'rel5'])
-
-        self.assertGreater(len(feat_rej), 0)
-
-        # Test type outputs
-        for i in range(1, 6):
-            row = df_bh.loc["rel{}".format(i)]
-            self.assertEqual(row.Feature, "rel{}".format(i))
-            if i == 1:
-                self.assertEqual(row.type, "binary")
-            else:
-                self.assertEqual(row.type, "real")
-
-        for i in range(1, 10):
-            row = df_bh.loc["irr{}".format(i)]
-            self.assertEqual(row.Feature, "irr{}".format(i))
-            if i not in [3, 6, 9]:
-                self.assertEqual(row.type, "real")
-            else:
-                self.assertEqual(row.type, "binary")
-
-            self.assertEqual(row.rejected, False)
-
-            # Assert that all of the relevant features are kept.
-            # THIS FAILS!
-            # self.assertEqual(len(kept_feature), 5)
-
-    def test_binary_target_binary_features(self):
-        # Binomial random variables and binomial target
-        y = pd.Series(np.random.binomial(1, 0.5, 5000))
-        X = pd.DataFrame(index=range(5000))
-
-        for i in range(10):
-            X["irr{}".format(i)] = np.random.binomial(1, 0.1, 5000)
-
-        for i in range(10, 20):
-            X["irr{}".format(i)] = np.random.binomial(1, 0.8, 5000)
-
-        z = y - np.random.binomial(1, 0.01, 5000) + np.random.binomial(1, 0.01, 5000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel1"] = z
-
-        z = y - np.random.binomial(1, 0.05, 5000) + np.random.binomial(1, 0.05, 5000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel2"] = z
-
-        z = y - np.random.binomial(1, 0.10, 5000) + np.random.binomial(1, 0.10, 5000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel3"] = z
-
-        z = y - np.random.binomial(1, 0.15, 5000) + np.random.binomial(1, 0.15, 5000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel4"] = z
-
-        z = y - np.random.binomial(1, 0.20, 5000) + np.random.binomial(1, 0.20, 5000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel5"] = z
-
-        df_bh = tsfresh.feature_selection.feature_selector.check_fs_sig_bh(X, y)
-        feat_rej = df_bh.loc[df_bh.rejected].Feature
-
-        # Make sure all selected variables are relevant
-        for kept_feature in feat_rej:
-            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4', 'rel5'])
-
-        self.assertGreater(len(feat_rej), 0)
-
-        # Test type outputs
-        for i in range(1, 6):
-            row = df_bh.loc["rel{}".format(i)]
-            self.assertEqual(row.Feature, "rel{}".format(i))
-            self.assertEqual(row.type, "binary")
-
-        for i in range(1, 20):
-            row = df_bh.loc["irr{}".format(i)]
-            self.assertEqual(row.Feature, "irr{}".format(i))
-            self.assertEqual(row.type, "binary")
-
-            self.assertEqual(row.rejected, False)
-
-    def test_binomial_target_realvalued_features(self):
-        # Real valued random variables and binomial target
-        y = pd.Series(np.random.binomial(1, 0.5, 5000))
-        X = pd.DataFrame(index=range(5000))
-
-        for i in range(10):
-            X["irr{}".format(i)] = np.random.normal(1, 0.3, 5000)
-
-        for i in range(10, 20):
-            X["irr{}".format(i)] = np.random.normal(1, 0.5, 5000)
-
-        for i in range(20, 30):
-            X["irr{}".format(i)] = np.random.normal(1, 0.8, 5000)
-
-        X["rel1"] = y * np.random.normal(0, 1, 5000) + np.random.normal(0, 1, 5000)
-        X["rel2"] = y + np.random.normal(0, 1, 5000)
-        X["rel3"] = y ** 2 + np.random.normal(0, 1, 5000)
-        X["rel4"] = np.sqrt(y) + np.random.binomial(2, 0.1, 5000)
-
-        df_bh = tsfresh.feature_selection.feature_selector.check_fs_sig_bh(X, y)
-        feat_rej = df_bh.loc[df_bh.rejected].Feature
-
-        # Make sure all selected variables are relevant
-        for kept_feature in feat_rej:
-            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4'])
-
-        self.assertGreater(len(feat_rej), 0)
-
-        # Test type outputs
-        for i in range(1, 5):
-            row = df_bh.loc["rel{}".format(i)]
-            self.assertEqual(row.Feature, "rel{}".format(i))
-            self.assertEqual(row.type, "real")
-
-        for i in range(1, 30):
-            row = df_bh.loc["irr{}".format(i)]
-            self.assertEqual(row.Feature, "irr{}".format(i))
-            self.assertEqual(row.type, "real")
-
-            self.assertEqual(row.rejected, False)
-
-    def test_real_target_mixed_case(self):
-        # Mixed case with real target
-        y = pd.Series(np.random.normal(0, 1, 5000))
-        X = pd.DataFrame(index=range(5000))
-
-        z = y.copy()
-        z[z <= 0] = 0
-        z[z > 0] = 1
-
-        X["rel1"] = z
-        X["rel2"] = y
-        X["rel3"] = y ** 2
-        X["rel4"] = np.sqrt(abs(y))
-
-        X["irr1"] = np.random.normal(0, 1, 5000)
-        X["irr2"] = np.random.poisson(1, 5000)
-        X["irr3"] = np.random.binomial(1, 0.1, 5000)
-        X["irr4"] = np.random.normal(0, 1, 5000)
-        X["irr5"] = np.random.poisson(1, 5000)
-        X["irr6"] = np.random.binomial(1, 0.05, 5000)
-        X["irr7"] = np.random.normal(0, 1, 5000)
-        X["irr8"] = np.random.poisson(1, 5000)
-        X["irr9"] = np.random.binomial(1, 0.2, 5000)
-
-        df_bh = tsfresh.feature_selection.feature_selector.check_fs_sig_bh(X, y)
-        feat_rej = df_bh.loc[df_bh.rejected].Feature
-
-        # Make sure all selected variables are relevant
-        for kept_feature in feat_rej:
-            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4'])
-
-        self.assertGreater(len(feat_rej), 0)
-
-        # Test type outputs
-        for i in range(1, 5):
-            row = df_bh.loc["rel{}".format(i)]
-            self.assertEqual(row.Feature, "rel{}".format(i))
-            if i == 1:
-                self.assertEqual(row.type, "binary")
-            else:
-                self.assertEqual(row.type, "real")
-
-        for i in range(1, 10):
-            row = df_bh.loc["irr{}".format(i)]
-            self.assertEqual(row.Feature, "irr{}".format(i))
-            if i in [3, 6, 9]:
-                self.assertEqual(row.type, "binary")
-            else:
-                self.assertEqual(row.type, "real")
-
-            self.assertEqual(row.rejected, False)
-
-    def test_real_target_binary_features(self):
-        # Mixed case with real target
-        y = pd.Series(np.random.normal(0, 1, 1000))
-        X = pd.DataFrame(index=range(1000))
-
-        z = y - np.random.binomial(1, 0.20, 1000) + np.random.binomial(1, 0.20, 1000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel1"] = z
-
-        z = y - np.random.binomial(1, 0.10, 1000) + np.random.binomial(1, 0.10, 1000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel2"] = z
-
-        X["irr1"] = np.random.binomial(0, 0.1, 1000)
-        X["irr2"] = np.random.binomial(0, 0.15, 1000)
-        X["irr3"] = np.random.binomial(0, 0.05, 1000)
-        X["irr4"] = np.random.binomial(0, 0.2, 1000)
-        X["irr5"] = np.random.binomial(0, 0.25, 1000)
-        X["irr6"] = np.random.binomial(0, 0.01, 1000)
-
-        df_bh = tsfresh.feature_selection.feature_selector.check_fs_sig_bh(X, y)
-        feat_rej = df_bh.loc[df_bh.rejected].Feature
-
-        # Make sure all selected variables are relevant
-        for kept_feature in feat_rej:
-            self.assertIn(kept_feature, ['rel1', 'rel2'])
-
-        self.assertGreater(len(feat_rej), 0)
-
-    def test_all_features_good(self):
-        # Mixed case with real target
-        y = pd.Series(np.random.normal(0, 1, 1000))
-        X = pd.DataFrame(index=range(1000))
-
-        z = y - np.random.binomial(1, 0.20, 1000) + np.random.binomial(1, 0.20, 1000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel1"] = z
-
-        z = y - np.random.binomial(1, 0.10, 1000) + np.random.binomial(1, 0.10, 1000)
-        z[z == -1] = 0
-        z[z == 2] = 1
-        X["rel2"] = z
-
-        df_bh = tsfresh.feature_selection.feature_selector.check_fs_sig_bh(X, y)
-        feat_rej = df_bh.loc[df_bh.rejected].Feature
-
-        # Make sure all selected variables are relevant
-        for kept_feature in feat_rej:
-            self.assertIn(kept_feature, ['rel1', 'rel2'])
-
-        self.assertGreater(len(feat_rej), 0)
-
-    def test_all_features_bad(self):
-        # Mixed case with real target
-        y = pd.Series(np.random.normal(0, 1, 1000))
-        X = pd.DataFrame(index=range(1000))
-
-        X["irr1"] = np.random.binomial(0, 0.1, 1000)
-        X["irr2"] = np.random.binomial(0, 0.15, 1000)
-        X["irr3"] = np.random.binomial(0, 0.05, 1000)
-        X["irr4"] = np.random.binomial(0, 0.2, 1000)
-        X["irr5"] = np.random.binomial(0, 0.25, 1000)
-        X["irr6"] = np.random.binomial(0, 0.01, 1000)
-
-        df_bh = tsfresh.feature_selection.feature_selector.check_fs_sig_bh(X, y)
-        feat_rej = df_bh.loc[df_bh.rejected].Feature
-
-        self.assertEqual(len(feat_rej), 0)
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+import numpy as np
+import pandas as pd
+from unittest import TestCase
+from tsfresh.feature_selection.relevance import calculate_relevance_table
+
+
+class FeatureSignificanceTestCase(TestCase):
+    """Test cases for the whole feature selection algorithm."""
+
+    def setUp(self):
+        """Fix the random seed."""
+        np.random.seed(seed=42)
+
+    def test_binary_target_mixed_case(self):
+        # Mixed case with binomial target
+        np.random.seed(42)
+        y = pd.Series(np.random.binomial(1, 0.5, 1000))
+        X = pd.DataFrame(index=range(1000))
+
+        z = y - np.random.binomial(1, 0.1, 1000) + np.random.binomial(1, 0.1, 1000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+
+        X["rel1"] = z
+        X["rel2"] = y * np.abs(np.random.normal(0, 1, 1000)) + np.random.normal(0, 1, 1000)
+        X["rel3"] = y + np.random.normal(0, 0.3, 1000)
+        X["rel4"] = y ** 2 + np.random.normal(0, 1, 1000)
+        X["rel5"] = np.sqrt(y) + np.random.binomial(2, 0.1, 1000)
+
+        X["irr_constant"] = 1.113344
+
+        X["irr1"] = np.random.normal(0, 1, 1000)
+        X["irr2"] = np.random.poisson(1, 1000)
+        X["irr3"] = np.random.binomial(1, 0.3, 1000)
+        X["irr4"] = np.random.normal(0, 1, 1000)
+        X["irr5"] = np.random.poisson(1, 1000)
+        X["irr6"] = np.random.binomial(1, 0.3, 1000)
+        X["irr7"] = np.random.normal(0, 1, 1000)
+        X["irr8"] = np.random.poisson(1, 1000)
+        X["irr9"] = np.random.binomial(1, 0.3, 1000)
+
+        df_bh = calculate_relevance_table(X, y)
+        feat_rej = df_bh.loc[df_bh.relevant].feature
+
+        # Make sure all selected variables are relevant
+        for kept_feature in feat_rej:
+            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4', 'rel5'])
+
+        self.assertGreater(len(feat_rej), 0)
+
+        # Test type outputs
+        for i in range(1, 6):
+            row = df_bh.loc["rel{}".format(i)]
+            self.assertEqual(row.feature, "rel{}".format(i))
+            if i == 1:
+                self.assertEqual(row.type, "binary")
+            else:
+                self.assertEqual(row.type, "real")
+
+        for i in range(1, 10):
+            row = df_bh.loc["irr{}".format(i)]
+            self.assertEqual(row.feature, "irr{}".format(i))
+            if i not in [3, 6, 9]:
+                self.assertEqual(row.type, "real")
+            else:
+                self.assertEqual(row.type, "binary")
+
+            self.assertEqual(row.relevant, False)
+
+            # Assert that all of the relevant features are kept.
+            # THIS FAILS!
+            # self.assertEqual(len(kept_feature), 5)
+
+    def test_binary_target_binary_features(self):
+        # Binomial random variables and binomial target
+        y = pd.Series(np.random.binomial(1, 0.5, 5000))
+        X = pd.DataFrame(index=range(5000))
+
+        for i in range(10):
+            X["irr{}".format(i)] = np.random.binomial(1, 0.1, 5000)
+
+        for i in range(10, 20):
+            X["irr{}".format(i)] = np.random.binomial(1, 0.8, 5000)
+
+        z = y - np.random.binomial(1, 0.01, 5000) + np.random.binomial(1, 0.01, 5000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel1"] = z
+
+        z = y - np.random.binomial(1, 0.05, 5000) + np.random.binomial(1, 0.05, 5000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel2"] = z
+
+        z = y - np.random.binomial(1, 0.10, 5000) + np.random.binomial(1, 0.10, 5000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel3"] = z
+
+        z = y - np.random.binomial(1, 0.15, 5000) + np.random.binomial(1, 0.15, 5000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel4"] = z
+
+        z = y - np.random.binomial(1, 0.20, 5000) + np.random.binomial(1, 0.20, 5000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel5"] = z
+
+        df_bh = calculate_relevance_table(X, y)
+        feat_rej = df_bh.loc[df_bh.relevant].feature
+
+        # Make sure all selected variables are relevant
+        for kept_feature in feat_rej:
+            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4', 'rel5'])
+
+        self.assertGreater(len(feat_rej), 0)
+
+        # Test type outputs
+        for i in range(1, 6):
+            row = df_bh.loc["rel{}".format(i)]
+            self.assertEqual(row.feature, "rel{}".format(i))
+            self.assertEqual(row.type, "binary")
+
+        for i in range(1, 20):
+            row = df_bh.loc["irr{}".format(i)]
+            self.assertEqual(row.feature, "irr{}".format(i))
+            self.assertEqual(row.type, "binary")
+
+            self.assertEqual(row.relevant, False)
+
+    def test_binomial_target_realvalued_features(self):
+        # Real valued random variables and binomial target
+        y = pd.Series(np.random.binomial(1, 0.5, 5000))
+        X = pd.DataFrame(index=range(5000))
+
+        for i in range(10):
+            X["irr{}".format(i)] = np.random.normal(1, 0.3, 5000)
+
+        for i in range(10, 20):
+            X["irr{}".format(i)] = np.random.normal(1, 0.5, 5000)
+
+        for i in range(20, 30):
+            X["irr{}".format(i)] = np.random.normal(1, 0.8, 5000)
+
+        X["rel1"] = y * np.random.normal(0, 1, 5000) + np.random.normal(0, 1, 5000)
+        X["rel2"] = y + np.random.normal(0, 1, 5000)
+        X["rel3"] = y ** 2 + np.random.normal(0, 1, 5000)
+        X["rel4"] = np.sqrt(y) + np.random.binomial(2, 0.1, 5000)
+
+        df_bh = calculate_relevance_table(X, y)
+        feat_rej = df_bh.loc[df_bh.relevant].feature
+
+        # Make sure all selected variables are relevant
+        for kept_feature in feat_rej:
+            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4'])
+
+        self.assertGreater(len(feat_rej), 0)
+
+        # Test type outputs
+        for i in range(1, 5):
+            row = df_bh.loc["rel{}".format(i)]
+            self.assertEqual(row.feature, "rel{}".format(i))
+            self.assertEqual(row.type, "real")
+
+        for i in range(1, 30):
+            row = df_bh.loc["irr{}".format(i)]
+            self.assertEqual(row.feature, "irr{}".format(i))
+            self.assertEqual(row.type, "real")
+
+            self.assertEqual(row.relevant, False)
+
+    def test_real_target_mixed_case(self):
+        # Mixed case with real target
+        y = pd.Series(np.random.normal(0, 1, 5000))
+        X = pd.DataFrame(index=range(5000))
+
+        z = y.copy()
+        z[z <= 0] = 0
+        z[z > 0] = 1
+
+        X["rel1"] = z
+        X["rel2"] = y
+        X["rel3"] = y ** 2
+        X["rel4"] = np.sqrt(abs(y))
+
+        X["irr1"] = np.random.normal(0, 1, 5000)
+        X["irr2"] = np.random.poisson(1, 5000)
+        X["irr3"] = np.random.binomial(1, 0.1, 5000)
+        X["irr4"] = np.random.normal(0, 1, 5000)
+        X["irr5"] = np.random.poisson(1, 5000)
+        X["irr6"] = np.random.binomial(1, 0.05, 5000)
+        X["irr7"] = np.random.normal(0, 1, 5000)
+        X["irr8"] = np.random.poisson(1, 5000)
+        X["irr9"] = np.random.binomial(1, 0.2, 5000)
+
+        df_bh = calculate_relevance_table(X, y)
+        feat_rej = df_bh.loc[df_bh.relevant].feature
+
+        # Make sure all selected variables are relevant
+        for kept_feature in feat_rej:
+            self.assertIn(kept_feature, ['rel1', 'rel2', 'rel3', 'rel4'])
+
+        self.assertGreater(len(feat_rej), 0)
+
+        # Test type outputs
+        for i in range(1, 5):
+            row = df_bh.loc["rel{}".format(i)]
+            self.assertEqual(row.feature, "rel{}".format(i))
+            if i == 1:
+                self.assertEqual(row.type, "binary")
+            else:
+                self.assertEqual(row.type, "real")
+
+        for i in range(1, 10):
+            row = df_bh.loc["irr{}".format(i)]
+            self.assertEqual(row.feature, "irr{}".format(i))
+            if i in [3, 6, 9]:
+                self.assertEqual(row.type, "binary")
+            else:
+                self.assertEqual(row.type, "real")
+
+            self.assertEqual(row.relevant, False)
+
+    def test_real_target_binary_features(self):
+        # Mixed case with real target
+        y = pd.Series(np.random.normal(0, 1, 1000))
+        X = pd.DataFrame(index=range(1000))
+
+        z = y - np.random.binomial(1, 0.20, 1000) + np.random.binomial(1, 0.20, 1000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel1"] = z
+
+        z = y - np.random.binomial(1, 0.10, 1000) + np.random.binomial(1, 0.10, 1000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel2"] = z
+
+        X["irr1"] = np.random.binomial(0, 0.1, 1000)
+        X["irr2"] = np.random.binomial(0, 0.15, 1000)
+        X["irr3"] = np.random.binomial(0, 0.05, 1000)
+        X["irr4"] = np.random.binomial(0, 0.2, 1000)
+        X["irr5"] = np.random.binomial(0, 0.25, 1000)
+        X["irr6"] = np.random.binomial(0, 0.01, 1000)
+
+        df_bh = calculate_relevance_table(X, y)
+        feat_rej = df_bh.loc[df_bh.relevant].feature
+
+        # Make sure all selected variables are relevant
+        for kept_feature in feat_rej:
+            self.assertIn(kept_feature, ['rel1', 'rel2'])
+
+        self.assertGreater(len(feat_rej), 0)
+
+    def test_all_features_good(self):
+        # Mixed case with real target
+        y = pd.Series(np.random.normal(0, 1, 1000))
+        X = pd.DataFrame(index=range(1000))
+
+        z = y - np.random.binomial(1, 0.20, 1000) + np.random.binomial(1, 0.20, 1000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel1"] = z
+
+        z = y - np.random.binomial(1, 0.10, 1000) + np.random.binomial(1, 0.10, 1000)
+        z[z == -1] = 0
+        z[z == 2] = 1
+        X["rel2"] = z
+
+        df_bh = calculate_relevance_table(X, y)
+        feat_rej = df_bh.loc[df_bh.relevant].feature
+
+        # Make sure all selected variables are relevant
+        for kept_feature in feat_rej:
+            self.assertIn(kept_feature, ['rel1', 'rel2'])
+
+        self.assertGreater(len(feat_rej), 0)
+
+    def test_all_features_bad(self):
+        # Mixed case with real target
+        y = pd.Series(np.random.normal(0, 1, 1000))
+        X = pd.DataFrame(index=range(1000))
+
+        X["irr1"] = np.random.binomial(0, 0.1, 1000)
+        X["irr2"] = np.random.binomial(0, 0.15, 1000)
+        X["irr3"] = np.random.binomial(0, 0.05, 1000)
+        X["irr4"] = np.random.binomial(0, 0.2, 1000)
+        X["irr5"] = np.random.binomial(0, 0.25, 1000)
+        X["irr6"] = np.random.binomial(0, 0.01, 1000)
+
+        df_bh = calculate_relevance_table(X, y)
+        feat_rej = df_bh.loc[df_bh.relevant].feature
+
+        self.assertEqual(len(feat_rej), 0)
```

### Comparing `tsfresh-0.8.1/tests/test_relevant_feature_extraction.py` & `tsfresh-0.9.0/tests/test_relevant_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/transformers/test_feature_augmenter.py` & `tsfresh-0.9.0/tests/transformers/test_feature_augmenter.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/transformers/test_feature_selector.py` & `tsfresh-0.9.0/tests/transformers/test_feature_selector.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/transformers/test_per_column_imputer.py` & `tsfresh-0.9.0/tests/transformers/test_per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tests/transformers/test_relevant_feature_extractor.py` & `tsfresh-0.9.0/tests/transformers/test_relevant_feature_augmenter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,106 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-import pandas as pd
-import numpy as np
-from tests.fixtures import DataTestCase
-from tsfresh.feature_extraction import ComprehensiveFCParameters
-from tsfresh.transformers.relevant_feature_augmenter import RelevantFeatureAugmenter
-
-
-class RelevantFeatureAugmenterTestCase(DataTestCase):
-    def setUp(self):
-        self.test_df = self.create_test_data_sample()
-        fc_parameters = {"length": None}
-        self.kind_to_fc_parameters = {"a": fc_parameters.copy(),
-                                      "b": fc_parameters.copy()}
-
-    def test_not_fitted(self):
-        augmenter = RelevantFeatureAugmenter()
-
-        X = pd.DataFrame()
-
-        self.assertRaises(RuntimeError, augmenter.transform, X)
-
-    def test_no_timeseries(self):
-        augmenter = RelevantFeatureAugmenter()
-
-        X = pd.DataFrame()
-        y = pd.Series()
-
-        self.assertRaises(RuntimeError, augmenter.fit, X, y)
-
-    def test_nothing_relevant(self):
-        augmenter = RelevantFeatureAugmenter(kind_to_fc_parameters=self.kind_to_fc_parameters,
-                                             column_value="val", column_id="id", column_sort="sort",
-                                             column_kind="kind")
-
-        y = pd.Series({10: 1, 500: 0})
-        X = pd.DataFrame(index=[10, 500])
-
-        augmenter.set_timeseries_container(self.test_df)
-        augmenter.fit(X, y)
-
-        transformed_X = augmenter.transform(X.copy())
-
-        self.assertEqual(list(transformed_X.columns), [])
-        self.assertEqual(list(transformed_X.index), list(X.index))
-
-    def test_impute_works(self):
-        self.kind_to_fc_parameters["a"].update({"kurtosis": None})
-
-        augmeter = RelevantFeatureAugmenter(kind_to_fc_parameters=self.kind_to_fc_parameters,
-                                            column_value="val", column_id="id", column_sort="sort",
-                                            column_kind="kind")
-
-        y = pd.Series({10: 1, 500: 0})
-        X = pd.DataFrame(index=[10, 500])
-
-        augmeter.set_timeseries_container(self.test_df)
-        augmeter.fit(X, y)
-
-        transformed_X = augmeter.transform(X.copy())
-
-        self.assertEqual(list(transformed_X.columns), [])
-        self.assertEqual(list(transformed_X.index), list(X.index))
-
-    def test_evaluate_only_added_features_true(self):
-        """
-        The boolean flag `evaluate_only_extracted_features` makes sure that only the time series based features are
-        filtered. This unit tests checks that
-        """
-
-        augmenter = RelevantFeatureAugmenter(kind_to_fc_parameters=self.kind_to_fc_parameters,
-                                             filter_only_tsfresh_features=True,
-                                             column_value="val", column_id="id", column_sort="sort", column_kind="kind")
-
-        y = pd.Series({10: 1, 500: 0})
-        X = pd.DataFrame(index=[10, 500])
-        X["pre_feature"] = 0
-
-        augmenter.set_timeseries_container(self.test_df)
-        augmenter.fit(X, y)
-        transformed_X = augmenter.transform(X.copy())
-
-        self.assertEqual(sum(["pre_feature" == column for column in transformed_X.columns]), 1)
-
-    def test_evaluate_only_added_features_false(self):
-        """
-        The boolean flag `evaluate_only_extracted_features` makes sure that only the time series based features are
-        filtered. This unit tests checks that
-        """
-
-        augmenter = RelevantFeatureAugmenter(kind_to_fc_parameters=self.kind_to_fc_parameters,
-                                             filter_only_tsfresh_features=False,
-                                             column_value="val", column_id="id", column_sort="sort", column_kind="kind")
-
-        df, y = self.create_test_data_sample_with_target()
-        X = pd.DataFrame(index=np.unique(df.id))
-        X["pre_drop"] = 0
-        X["pre_keep"] = y
-
-        augmenter.set_timeseries_container(df)
-        augmenter.fit(X, y)
-        transformed_X = augmenter.transform(X.copy())
-
-        self.assertEqual(sum(["pre_keep" == column for column in transformed_X.columns]), 1)
-        self.assertEqual(sum(["pre_drop" == column for column in transformed_X.columns]), 0)
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+import pandas as pd
+import numpy as np
+from tests.fixtures import DataTestCase
+import mock
+from tsfresh.transformers.relevant_feature_augmenter import RelevantFeatureAugmenter
+
+
+class RelevantFeatureAugmenterTestCase(DataTestCase):
+    def setUp(self):
+        self.test_df = self.create_test_data_sample()
+        fc_parameters = {"length": None}
+        self.kind_to_fc_parameters = {"a": fc_parameters.copy(),
+                                      "b": fc_parameters.copy()}
+
+    def test_not_fitted(self):
+        augmenter = RelevantFeatureAugmenter()
+
+        X = pd.DataFrame()
+
+        self.assertRaises(RuntimeError, augmenter.transform, X)
+
+    def test_no_timeseries(self):
+        augmenter = RelevantFeatureAugmenter()
+
+        X = pd.DataFrame()
+        y = pd.Series()
+
+        self.assertRaises(RuntimeError, augmenter.fit, X, y)
+
+    def test_nothing_relevant(self):
+        augmenter = RelevantFeatureAugmenter(kind_to_fc_parameters=self.kind_to_fc_parameters,
+                                             column_value="val", column_id="id", column_sort="sort",
+                                             column_kind="kind")
+
+        y = pd.Series({10: 1, 500: 0})
+        X = pd.DataFrame(index=[10, 500])
+
+        augmenter.set_timeseries_container(self.test_df)
+        augmenter.fit(X, y)
+
+        transformed_X = augmenter.transform(X.copy())
+
+        self.assertEqual(list(transformed_X.columns), [])
+        self.assertEqual(list(transformed_X.index), list(X.index))
+
+    def test_evaluate_only_added_features_true(self):
+        """
+        The boolean flag `evaluate_only_extracted_features` makes sure that only the time series based features are
+        filtered. This unit tests checks that
+        """
+
+        augmenter = RelevantFeatureAugmenter(kind_to_fc_parameters=self.kind_to_fc_parameters,
+                                             filter_only_tsfresh_features=True,
+                                             column_value="val", column_id="id", column_sort="sort", column_kind="kind")
+
+        y = pd.Series({10: 1, 500: 0})
+        X = pd.DataFrame(index=[10, 500])
+        X["pre_feature"] = 0
+
+        augmenter.set_timeseries_container(self.test_df)
+        augmenter.fit(X, y)
+        transformed_X = augmenter.transform(X.copy())
+
+        self.assertEqual(sum(["pre_feature" == column for column in transformed_X.columns]), 1)
+
+    def test_evaluate_only_added_features_false(self):
+        """
+        The boolean flag `evaluate_only_extracted_features` makes sure that only the time series based features are
+        filtered. This unit tests checks that
+        """
+
+        augmenter = RelevantFeatureAugmenter(kind_to_fc_parameters=self.kind_to_fc_parameters,
+                                             filter_only_tsfresh_features=False,
+                                             column_value="val", column_id="id", column_sort="sort", column_kind="kind")
+
+        df, y = self.create_test_data_sample_with_target()
+        X = pd.DataFrame(index=np.unique(df.id))
+        X["pre_drop"] = 0
+        X["pre_keep"] = y
+
+        augmenter.set_timeseries_container(df)
+        augmenter.fit(X, y)
+        transformed_X = augmenter.transform(X.copy())
+
+        self.assertEqual(sum(["pre_keep" == column for column in transformed_X.columns]), 1)
+        self.assertEqual(sum(["pre_drop" == column for column in transformed_X.columns]), 0)
+
+
+    @mock.patch('tsfresh.transformers.feature_selector.calculate_relevance_table')
+    def test_does_impute(self, calculate_relevance_table_mock):
+        df = pd.DataFrame([[1, 1, 1], [2, 1, 1]], columns=['id', 'time', 'value'])
+        X = pd.DataFrame(index=[1])
+        y = pd.Series([0, 1])
+        fc_parameters = {"autocorrelation": [{'lag': 2}]}
+
+        calculate_relevance_table_mock.return_value = pd.DataFrame(columns=['feature', 'p_value', 'relevant'])
+        augmenter = RelevantFeatureAugmenter(column_id='id', column_sort='time', default_fc_parameters=fc_parameters)
+        augmenter.set_timeseries_container(df)
+        augmenter.fit(X, y)
+
+        assert calculate_relevance_table_mock.call_count == 1
+        assert not calculate_relevance_table_mock.call_args[0][0].isnull().any().any()
```

### Comparing `tsfresh-0.8.1/tests/utilities/test_dataframe_functions.py` & `tsfresh-0.9.0/tests/utilities/test_dataframe_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,592 +1,650 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-import warnings
-from unittest import TestCase
-
-import pandas as pd
-from tsfresh.utilities import dataframe_functions
-import numpy as np
-import six
-
-
-class NormalizeTestCase(TestCase):
-    def test_with_dictionaries_one_row(self):
-        test_df = pd.DataFrame([{"value": 1, "id": "id_1"}])
-        test_dict = {"a": test_df, "b": test_df}
-
-        # A kind is not allowed with dicts
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_dict,
-                          "id", None, "a kind", None)
-
-        # The value must be present
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_dict,
-                          "id", None, None, "something other")
-
-        # Nothing should have changed compared to the input data
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_dict, "id", None, None, "value")
-        self.assertEqual(column_value, "value")
-        self.assertEqual(column_id, "id")
-        six.assertCountEqual(self, list(test_dict.keys()), list(result_dict.keys()))
-        self.assertEqual(result_dict["a"].iloc[0].to_dict(), {"value": 1, "id": "id_1"})
-
-        # The algo should choose the correct value column
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_dict, "id", None, None, None)
-        self.assertEqual(column_value, "value")
-        self.assertEqual(column_id, "id")
-
-    def test_with_dictionaries_two_rows(self):
-        test_df = pd.DataFrame([{"value": 2, "sort": 2, "id": "id_1"},
-                                {"value": 1, "sort": 1, "id": "id_1"}])
-        test_dict = {"a": test_df, "b": test_df}
-
-        # If there are more than one column, the algorithm can not choose the correct column
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_dict,
-                          "id", None, None, None)
-
-        # Sorting should work
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_dict, "id", "sort", None, "value")
-        self.assertEqual(column_value, "value")
-        self.assertEqual(column_id, "id")
-
-        # Assert sorted and without sort column
-        self.assertEqual(result_dict["a"].iloc[0].to_dict(), {"value": 1, "id": "id_1"})
-        self.assertEqual(result_dict["a"].iloc[1].to_dict(), {"value": 2, "id": "id_1"})
-
-        # Assert the algo has found the correct column
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_dict, "id", "sort", None, None)
-        self.assertEqual(column_value, "value")
-        self.assertEqual(column_id, "id")
-
-    def test_with_dictionaries_two_rows_sorted(self):
-        test_df = pd.DataFrame([{"value": 2, "id": "id_1"},
-                                {"value": 1, "id": "id_1"}])
-        test_dict = {"a": test_df, "b": test_df}
-
-        # Pass the id
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_dict, "id", None, None, "value")
-        self.assertEqual(column_value, "value")
-        self.assertEqual(column_id, "id")
-
-        self.assertEqual(result_dict["a"].iloc[0].to_dict(), {"value": 2, "id": "id_1"})
-
-        # The algo should have found the correct value column
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_dict, "id", None, None, None)
-        self.assertEqual(column_value, "value")
-        self.assertEqual(column_id, "id")
-
-    def test_with_df(self):
-        # give everyting
-        test_df = pd.DataFrame([{"id": 0, "kind": "a", "value": 3, "sort": 1}])
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_df, "id", "sort", "kind", "value")
-
-        self.assertEqual(column_id, "id")
-        self.assertEqual(column_value, "value")
-        self.assertIn("a", result_dict)
-        six.assertCountEqual(self, list(result_dict["a"].columns), ["id", "value"])
-        self.assertEqual(list(result_dict["a"]["value"]), [3])
-        self.assertEqual(list(result_dict["a"]["id"]), [0])
-
-        # give no kind
-        test_df = pd.DataFrame([{"id": 0, "value": 3, "sort": 1}])
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_df, "id", "sort", None, "value")
-
-        self.assertEqual(column_id, "id")
-        self.assertEqual(column_value, "value")
-        self.assertIn("value", result_dict)
-        six.assertCountEqual(self, list(result_dict["value"].columns), ["id", "value"])
-        self.assertEqual(list(result_dict["value"]["value"]), [3])
-        self.assertEqual(list(result_dict["value"]["id"]), [0])
-
-        # Let the function find the values
-        test_df = pd.DataFrame([{"id": 0, "a": 3, "b": 5, "sort": 1}])
-        result_dict, column_id, column_value = \
-            dataframe_functions.normalize_input_to_internal_representation(test_df, "id", "sort", None, None)
-
-        self.assertEqual(column_id, "id")
-        self.assertEqual(column_value, "_value")
-        self.assertIn("a", result_dict)
-        self.assertIn("b", result_dict)
-        six.assertCountEqual(self, list(result_dict["a"].columns), ["_value", "id"])
-        self.assertEqual(list(result_dict["a"]["_value"]), [3])
-        self.assertEqual(list(result_dict["a"]["id"]), [0])
-        six.assertCountEqual(self, list(result_dict["b"].columns), ["_value", "id"])
-        self.assertEqual(list(result_dict["b"]["_value"]), [5])
-        self.assertEqual(list(result_dict["b"]["id"]), [0])
-
-    def test_with_wrong_input(self):
-        test_df = pd.DataFrame([{"id": 0, "kind": "a", "value": 3, "sort": np.NaN}])
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_df,
-                          "id", "sort", "kind", "value")
-
-        test_df = pd.DataFrame([{"id": 0, "kind": "a", "value": 3, "sort": 1}])
-        self.assertRaises(AttributeError, dataframe_functions.normalize_input_to_internal_representation, test_df,
-                          "strange_id", "sort", "kind", "value")
-
-        test_df = pd.DataFrame([{"id": np.NaN, "kind": "a", "value": 3, "sort": 1}])
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_df,
-                          "id", "sort", "kind", "value")
-
-        test_df = pd.DataFrame([{"id": 0}])
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_df,
-                          "id", None, None, None)
-
-        test_df = pd.DataFrame([{"id": 2}, {"id": 1}])
-        test_dict = {"a": test_df, "b": test_df}
-
-        # If there are more than one column, the algorithm can not choose the correct column
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_dict,
-                          "id", None, None, None)
-
-        test_dict = {"a": pd.DataFrame([{"id": 2, "value_a": 3}, {"id": 1, "value_a": 4}]),
-                     "b": pd.DataFrame([{"id": 2}, {"id": 1}])}
-
-        # If there are more than one column, the algorithm can not choose the correct column
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_dict,
-                          "id", None, None, None)
-
-        test_df = pd.DataFrame([{"id": 0, "value": np.NaN}])
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_df,
-                          "id", None, None, "value")
-
-        test_df = pd.DataFrame([{"id": 0, "value": np.NaN}])
-        self.assertRaises(ValueError, dataframe_functions.normalize_input_to_internal_representation, test_df,
-                          None, None, None, "value")
-
-
-class RollingTestCase(TestCase):
-    def test_with_wrong_input(self):
-        test_df = pd.DataFrame({"id": [0, 0], "kind": ["a", "b"], "value": [3, 3], "sort": [np.NaN, np.NaN]})
-        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
-                          df_or_dict=test_df, column_id="id",
-                          column_sort="sort", column_kind="kind",
-                          rolling_direction=1)
-
-        test_df = pd.DataFrame({"id": [0, 0], "kind": ["a", "b"], "value": [3, 3], "sort": [1, 1]})
-        self.assertRaises(AttributeError, dataframe_functions.roll_time_series,
-                          df_or_dict=test_df, column_id="strange_id",
-                          column_sort="sort", column_kind="kind",
-                          rolling_direction=1)
-
-        test_df = {"a": pd.DataFrame([{"id": 0}])}
-        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
-                          df_or_dict=test_df, column_id="id",
-                          column_sort=None, column_kind="kind",
-                          rolling_direction=1)
-
-        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
-                          df_or_dict=test_df, column_id=None,
-                          column_sort=None, column_kind="kind",
-                          rolling_direction=1)
-
-        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
-                          df_or_dict=test_df, column_id="id",
-                          column_sort=None, column_kind=None,
-                          rolling_direction=0)
-
-        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
-                          df_or_dict=test_df, column_id=None,
-                          column_sort=None, column_kind=None,
-                          rolling_direction=0)
-
-    def test_assert_single_row(self):
-        test_df = pd.DataFrame([{"id": np.NaN, "kind": "a", "value": 3, "sort": 1}])
-        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
-                          df_or_dict=test_df, column_id="id",
-                          column_sort="sort", column_kind="kind",
-                          rolling_direction=1)
-
-    def test_positive_rolling(self):
-        first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": range(4)})
-        second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
-
-        first_class["id"] = 1
-        second_class["id"] = 2
-
-        df_full = pd.concat([first_class, second_class], ignore_index=True)
-
-        correct_indices = (["id=1, shift=3"] * 1 +
-                           ["id=1, shift=2"] * 2 +
-                           ["id=1, shift=1"] * 3 +
-                           ["id=2, shift=1"] * 1 +
-                           ["id=1, shift=0"] * 4 +
-                           ["id=2, shift=0"] * 2)
-        correct_values_a = [1, 1, 2, 1, 2, 3, 10, 1, 2, 3, 4, 10, 11]
-        correct_values_b = [5, 5, 6, 5, 6, 7, 12, 5, 6, 7, 8, 12, 13]
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=1)
-
-        self.assertListEqual(list(df["id"]), correct_indices)
-        self.assertListEqual(list(df["a"].values), correct_values_a)
-        self.assertListEqual(list(df["b"].values), correct_values_b)
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=1,
-                                                  maximum_number_of_timeshifts=None)
-
-        self.assertListEqual(list(df["id"]), correct_indices)
-        self.assertListEqual(list(df["a"].values), correct_values_a)
-        self.assertListEqual(list(df["b"].values), correct_values_b)
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=1,
-                                                  maximum_number_of_timeshifts=1)
-
-        self.assertListEqual(list(df["id"]), correct_indices[3:])
-        self.assertListEqual(list(df["a"].values), correct_values_a[3:])
-        self.assertListEqual(list(df["b"].values), correct_values_b[3:])
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=1,
-                                                  maximum_number_of_timeshifts=2)
-
-        self.assertListEqual(list(df["id"]), correct_indices[1:])
-        self.assertListEqual(list(df["a"].values), correct_values_a[1:])
-        self.assertListEqual(list(df["b"].values), correct_values_b[1:])
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=1,
-                                                  maximum_number_of_timeshifts=4)
-
-        self.assertListEqual(list(df["id"]), correct_indices[:])
-        self.assertListEqual(list(df["a"].values), correct_values_a[:])
-        self.assertListEqual(list(df["b"].values), correct_values_b[:])
-
-    def test_negative_rolling(self):
-        first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": range(4)})
-        second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
-
-        first_class["id"] = 1
-        second_class["id"] = 2
-
-        df_full = pd.concat([first_class, second_class], ignore_index=True)
-
-        correct_indices = (["id=1, shift=-3"] * 1 +
-                           ["id=1, shift=-2"] * 2 +
-                           ["id=1, shift=-1"] * 3 +
-                           ["id=2, shift=-1"] * 1 +
-                           ["id=1, shift=0"] * 4 +
-                           ["id=2, shift=0"] * 2)
-        correct_values_a = [4, 3, 4, 2, 3, 4, 11, 1, 2, 3, 4, 10, 11]
-        correct_values_b = [8, 7, 8, 6, 7, 8, 13, 5, 6, 7, 8, 12, 13]
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=-1)
-
-        self.assertListEqual(list(df["id"].values), correct_indices)
-        self.assertListEqual(list(df["a"].values), correct_values_a)
-        self.assertListEqual(list(df["b"].values), correct_values_b)
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=-1,
-                                                  maximum_number_of_timeshifts=None)
-
-        self.assertListEqual(list(df["id"].values), correct_indices)
-        self.assertListEqual(list(df["a"].values), correct_values_a)
-        self.assertListEqual(list(df["b"].values), correct_values_b)
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=-1,
-                                                  maximum_number_of_timeshifts=1)
-
-        self.assertListEqual(list(df["id"].values), correct_indices[3:])
-        self.assertListEqual(list(df["a"].values), correct_values_a[3:])
-        self.assertListEqual(list(df["b"].values), correct_values_b[3:])
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=-1,
-                                                  maximum_number_of_timeshifts=2)
-
-        self.assertListEqual(list(df["id"].values), correct_indices[1:])
-        self.assertListEqual(list(df["a"].values), correct_values_a[1:])
-        self.assertListEqual(list(df["b"].values), correct_values_b[1:])
-
-        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                  column_kind=None, rolling_direction=-1,
-                                                  maximum_number_of_timeshifts=4)
-
-        self.assertListEqual(list(df["id"].values), correct_indices[:])
-        self.assertListEqual(list(df["a"].values), correct_values_a[:])
-        self.assertListEqual(list(df["b"].values), correct_values_b[:])
-
-    def test_stacked_rolling(self):
-        first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": range(4)})
-        second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
-
-        first_class["id"] = 1
-        second_class["id"] = 2
-
-        df_full = pd.concat([first_class, second_class], ignore_index=True)
-
-        df_stacked = pd.concat([df_full[["time", "id", "a"]].rename(columns={"a": "_value"}),
-                                df_full[["time", "id", "b"]].rename(columns={"b": "_value"})], ignore_index=True)
-        df_stacked["kind"] = ["a"] * 6 + ["b"] * 6
-
-        df = dataframe_functions.roll_time_series(df_stacked, column_id="id", column_sort="time",
-                                                  column_kind="kind", rolling_direction=-1)
-
-        correct_indices = (["id=1, shift=-3"] * 2 +
-                           ["id=1, shift=-2"] * 4 +
-                           ["id=1, shift=-1"] * 6 +
-                           ["id=2, shift=-1"] * 2 +
-                           ["id=1, shift=0"] * 8 +
-                           ["id=2, shift=0"] * 4)
-
-        self.assertListEqual(list(df["id"].values), correct_indices)
-
-        self.assertListEqual(list(df["kind"].values), ["a", "b"] * 13)
-        self.assertListEqual(list(df["_value"].values),
-                             [4, 8, 3, 7, 4, 8, 2, 6, 3, 7, 4, 8, 11, 13, 1, 5, 2, 6, 3, 7, 4, 8, 10, 12, 11, 13])
-
-    def test_dict_rolling(self):
-        df_dict = {
-            "a": pd.DataFrame({"_value": [1, 2, 3, 4, 10, 11], "id": [1, 1, 1, 1, 2, 2]}),
-            "b": pd.DataFrame({"_value": [5, 6, 7, 8, 12, 13], "id": [1, 1, 1, 1, 2, 2]})
-        }
-
-        df = dataframe_functions.roll_time_series(df_dict, column_id="id", column_sort=None,
-                                                  column_kind=None, rolling_direction=-1)
-
-        correct_indices = (["id=1, shift=-3"] * 1 +
-                           ["id=1, shift=-2"] * 2 +
-                           ["id=1, shift=-1"] * 3 +
-                           ["id=2, shift=-1"] * 1 +
-                           ["id=1, shift=0"] * 4 +
-                           ["id=2, shift=0"] * 2)
-
-        self.assertListEqual(list(df["a"]["id"].values), correct_indices)
-        self.assertListEqual(list(df["b"]["id"].values), correct_indices)
-
-        self.assertListEqual(list(df["a"]["_value"].values),
-                             [4, 3, 4, 2, 3, 4, 11, 1, 2, 3, 4, 10, 11])
-        self.assertListEqual(list(df["b"]["_value"].values),
-                             [8, 7, 8, 6, 7, 8, 13, 5, 6, 7, 8, 12, 13])
-
-    def test_warning_on_non_uniform_time_steps(self):
-        with warnings.catch_warnings(record=True) as w:
-            first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": [1, 2, 4, 5]})
-            second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
-
-            first_class["id"] = 1
-            second_class["id"] = 2
-
-            df_full = pd.concat([first_class, second_class], ignore_index=True)
-
-            dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
-                                                 column_kind=None, rolling_direction=1)
-
-            self.assertEqual(len(w), 1)
-            self.assertEqual(str(w[0].message),
-                             "Your time stamps are not uniformly sampled, which makes rolling "
-                             "nonsensical in some domains.")
-
-
-class CheckForNanTestCase(TestCase):
-    def test_all_columns(self):
-        test_df = pd.DataFrame([[1, 2, 3], [4, 5, 6]], index=[0, 1])
-
-        # should not raise an exception
-        dataframe_functions.check_for_nans_in_columns(test_df)
-
-        test_df = pd.DataFrame([[1, 2, 3], [4, np.NaN, 6]], index=[0, 1])
-
-        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df)
-
-    def test_not_all_columns(self):
-        test_df = pd.DataFrame([[1, 2, 3], [4, np.NaN, 6]], index=[0, 1], columns=["a", "b", "c"])
-
-        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df)
-        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, ["a", "b"])
-        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, ["b"])
-        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, "b")
-        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, ["c", "b"])
-
-        dataframe_functions.check_for_nans_in_columns(test_df, columns=["a", "c"])
-        dataframe_functions.check_for_nans_in_columns(test_df, columns="a")
-
-
-class ImputeTestCase(TestCase):
-    def test_impute_zero(self):
-        df = pd.DataFrame([{"value": np.NaN}])
-        dataframe_functions.impute_dataframe_zero(df)
-        self.assertEqual(list(df.value), [0])
-
-        df = pd.DataFrame([{"value": np.PINF}])
-        dataframe_functions.impute_dataframe_zero(df)
-        self.assertEqual(list(df.value), [0])
-
-        df = pd.DataFrame([{"value": np.NINF}])
-        dataframe_functions.impute_dataframe_zero(df)
-        self.assertEqual(list(df.value), [0])
-
-        df = pd.DataFrame([{"value": np.NINF}, {"value": np.NaN}, {"value": np.PINF}, {"value": 1}])
-        dataframe_functions.impute_dataframe_zero(df)
-        self.assertEqual(list(df.value), [0, 0, 0, 1])
-
-        df = pd.DataFrame([{"value": np.NINF}, {"value": np.NaN}, {"value": np.PINF}, {"value": 1}])
-        df = df.astype(np.float64)
-        df = dataframe_functions.impute_dataframe_zero(df)
-        self.assertEqual(list(df.value), [0, 0, 0, 1])
-
-        df = pd.DataFrame([{"value": np.NINF}, {"value": np.NaN}, {"value": np.PINF}, {"value": 1}])
-        df = df.astype(np.float32)
-        df = dataframe_functions.impute_dataframe_zero(df)
-        self.assertEqual(list(df.value), [0, 0, 0, 1])
-
-    def test_toplevel_impute(self):
-        df = pd.DataFrame(np.transpose([[0, 1, 2, np.NaN], [1, np.PINF, 2, 3], [1, -3, np.NINF, 3]]),
-                          columns=["value_a", "value_b", "value_c"])
-
-        dataframe_functions.impute(df)
-
-        self.assertEqual(list(df.value_a), [0, 1, 2, 1])
-        self.assertEqual(list(df.value_b), [1, 3, 2, 3])
-        self.assertEqual(list(df.value_c), [1, -3, -3, 3])
-
-        df = pd.DataFrame(np.transpose([[0, 1, 2, np.NaN], [1, np.PINF, 2, 3], [1, -3, np.NINF, 3]]),
-                          columns=["value_a", "value_b", "value_c"])
-        df = df.astype(np.float64, inplace=True)
-        dataframe_functions.impute(df)
-
-        df = pd.DataFrame(np.transpose([[0, 1, 2, np.NaN], [1, np.PINF, 2, 3], [1, -3, np.NINF, 3]]),
-                          columns=["value_a", "value_b", "value_c"])
-        df = df.astype(np.float32, inplace=True)
-        dataframe_functions.impute(df)
-
-        self.assertEqual(list(df.value_a), [0, 1, 2, 1])
-        self.assertEqual(list(df.value_b), [1, 3, 2, 3])
-        self.assertEqual(list(df.value_c), [1, -3, -3, 3])
-
-    def test_impute_range(self):
-        def get_df():
-            return pd.DataFrame(np.transpose([[0, 1, 2, np.NaN],
-                                              [1, np.PINF, 2, 3],
-                                              [1, -3, np.NINF, 3]]),
-                                columns=["value_a", "value_b", "value_c"])
-
-        # check if values are replaced correctly
-        df = get_df()
-        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
-        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
-        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55}
-        dataframe_functions.impute_dataframe_range(df, col_to_max, col_to_min, col_to_median)
-        self.assertEqual(list(df.value_a), [0, 1, 2, 55])
-        self.assertEqual(list(df.value_b), [1, 200, 2, 3])
-        self.assertEqual(list(df.value_c), [1, -3, -134, 3])
-
-        # check for error if column key is missing
-        df = get_df()
-        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
-        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
-        col_to_median = {"value_a": 55, "value_c": 55}
-        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
-                          df, col_to_max, col_to_min, col_to_median)
-
-        # check for no error if column key is too much
-        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
-        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
-        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55, "value_d": 55}
-        dataframe_functions.impute_dataframe_range(df, col_to_max, col_to_min, col_to_median)
-
-        # check for error if replacement value is not finite
-        df = get_df()
-        col_to_max = {"value_a": 200, "value_b": np.NaN, "value_c": 200}
-        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
-        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55}
-        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
-                          df, col_to_max, col_to_min, col_to_median)
-        df = get_df()
-        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
-        col_to_min = {"value_a": -134, "value_b": np.NINF, "value_c": -134}
-        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55}
-        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
-                          df, col_to_max, col_to_min, col_to_median)
-
-        df = get_df()
-        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
-        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
-        col_to_median = {"value_a": 55, "value_b": 55, "value_c": np.PINF}
-        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
-                          df, col_to_max, col_to_min, col_to_median)
-
-
-        df = pd.DataFrame([0, 1, 2, 3, 4], columns=["test"])
-        col_dict = {"test": 0}
-        dataframe_functions.impute_dataframe_range(df, col_dict, col_dict, col_dict)
-
-        self.assertEqual(df.columns, ["test"])
-        self.assertListEqual(list(df["test"].values), [0, 1, 2, 3, 4])
-
-
-class RestrictTestCase(TestCase):
-    def test_restrict_dataframe(self):
-        df = pd.DataFrame({'id': [1, 2, 3] * 2})
-
-        df_restricted = dataframe_functions.restrict_input_to_index(df, 'id', [2])
-        self.assertEqual(list(df_restricted.id), [2, 2])
-
-        df_restricted2 = dataframe_functions.restrict_input_to_index(df, 'id', [1, 2, 3])
-        self.assertTrue(df_restricted2.equals(df))
-
-    def test_restrict_dict(self):
-        kind_to_df = {'a': pd.DataFrame({'id': [1, 2, 3]}), 'b': pd.DataFrame({'id': [3, 4, 5]})}
-
-        kind_to_df_restricted = dataframe_functions.restrict_input_to_index(kind_to_df, 'id', [3])
-        self.assertEqual(list(kind_to_df_restricted['a'].id), [3])
-        self.assertEqual(list(kind_to_df_restricted['b'].id), [3])
-
-        kind_to_df_restricted2 = dataframe_functions.restrict_input_to_index(kind_to_df, 'id', [1, 2, 3, 4, 5])
-        self.assertTrue(kind_to_df_restricted2['a'].equals(kind_to_df['a']))
-        self.assertTrue(kind_to_df_restricted2['b'].equals(kind_to_df['b']))
-
-    def test_restrict_wrong(self):
-        other_type = np.array([1, 2, 3])
-
-        self.assertRaises(TypeError, dataframe_functions.restrict_input_to_index, other_type, "id", [1, 2, 3])
-
-
-class GetRangeValuesPerColumnTestCase(TestCase):
-    def test_ignores_non_finite_values(self):
-        df = pd.DataFrame([0, 1, 2, 3, np.NaN, np.PINF, np.NINF], columns=["value"])
-
-        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
-
-        self.assertEqual(col_to_max, {"value": 3})
-        self.assertEqual(col_to_min, {"value": 0})
-        self.assertEqual(col_to_median, {"value": 1.5})
-
-    def test_range_values_correct_with_even_length(self):
-        df = pd.DataFrame([0, 1, 2, 3], columns=["value"])
-
-        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
-
-        self.assertEqual(col_to_max, {"value": 3})
-        self.assertEqual(col_to_min, {"value": 0})
-        self.assertEqual(col_to_median, {"value": 1.5})
-
-    def test_range_values_correct_with_uneven_length(self):
-        df = pd.DataFrame([0, 1, 2], columns=["value"])
-
-        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
-
-        self.assertEqual(col_to_max, {"value": 2})
-        self.assertEqual(col_to_min, {"value": 0})
-        self.assertEqual(col_to_median, {"value": 1})
-
-    def test_no_finite_values_yields_0(self):
-        df = pd.DataFrame([np.NaN, np.PINF, np.NINF], columns=["value"])
-
-        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
-
-        self.assertEqual(col_to_max, {"value": 0})
-        self.assertEqual(col_to_min, {"value": 0})
-        self.assertEqual(col_to_median, {"value": 0})
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+import warnings
+from unittest import TestCase
+
+import pandas as pd
+from tsfresh.utilities import dataframe_functions
+import numpy as np
+import six
+from pandas.testing import assert_frame_equal, assert_series_equal
+
+
+class NormalizeTestCase(TestCase):
+    def test_with_dictionaries_one_row(self):
+        test_df = pd.DataFrame([{"value": 1, "id": "id_1"}])
+        test_dict = {"a": test_df, "b": test_df}
+
+        # A kind is not allowed with dicts
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_dict,
+                          "id", None, "a kind", None)
+
+        # The value must be present
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_dict,
+                          "id", None, None, "something other")
+
+    def test_with_dictionaries_two_rows(self):
+        test_df = pd.DataFrame([{"value": 2, "sort": 2, "id": "id_1"},
+                                {"value": 1, "sort": 1, "id": "id_1"}])
+        test_dict = {"a": test_df, "b": test_df}
+
+        # If there are more than one column, the algorithm can not choose the correct column
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_dict,
+                          "id", None, None, None)
+
+        # Sorting should work
+        result_df, column_id, column_kind, column_value = \
+            dataframe_functions._normalize_input_to_internal_representation(test_dict, "id", "sort", None, "value")
+        self.assertEqual(column_value, "value")
+        self.assertEqual(column_id, "id")
+
+        # Assert sorted and without sort column
+        self.assertEqual(result_df[result_df[column_kind] == "a"].iloc[0].to_dict(), {"_variables": "a", "value": 1, "id": "id_1"})
+        self.assertEqual(result_df[result_df[column_kind] == "a"].iloc[1].to_dict(), {"_variables": "a", "value": 2, "id": "id_1"})
+
+    def test_with_dictionaries_two_rows_sorted(self):
+        test_df = pd.DataFrame([{"value": 2, "id": "id_1"},
+                                {"value": 1, "id": "id_1"}])
+        test_dict = {"a": test_df, "b": test_df}
+
+        # Pass the id
+        result_df, column_id, column_kind, column_value = \
+            dataframe_functions._normalize_input_to_internal_representation(test_dict, "id", None, None, "value")
+        self.assertEqual(column_value, "value")
+        self.assertEqual(column_id, "id")
+
+        self.assertEqual(result_df[result_df[column_kind] == "a"].iloc[0].to_dict(), {"_variables": "a", "value": 2, "id": "id_1"})
+
+    def test_with_df(self):
+        # give everyting
+        test_df = pd.DataFrame([{"id": 0, "kind": "a", "value": 3, "sort": 1}])
+        result_df, column_id, column_kind, column_value = \
+            dataframe_functions._normalize_input_to_internal_representation(test_df, "id", "sort", "kind", "value")
+
+        self.assertEqual(column_id, "id")
+        self.assertEqual(column_value, "value")
+        self.assertEqual(column_kind, "kind")
+        self.assertIn("a", set(result_df[column_kind]))
+        six.assertCountEqual(self, list(result_df.columns), ["id", "value", "kind"])
+        self.assertEqual(list(result_df[result_df[column_kind] == "a"]["value"]), [3])
+        self.assertEqual(list(result_df[result_df[column_kind] == "a"]["id"]), [0])
+
+        # give no kind
+        test_df = pd.DataFrame([{"id": 0, "value": 3, "sort": 1}])
+        result_df, column_id, column_kind, column_value = \
+            dataframe_functions._normalize_input_to_internal_representation(test_df, "id", "sort", None, "value")
+
+        self.assertEqual(column_id, "id")
+        self.assertEqual(column_value, "value")
+        self.assertEqual(column_kind, "_variables")
+        self.assertIn("feature", set(result_df[column_kind]))
+        six.assertCountEqual(self, list(result_df.columns), ["id", "value", "_variables"])
+        self.assertEqual(list(result_df[result_df[column_kind] == "feature"]["value"]), [3])
+        self.assertEqual(list(result_df[result_df[column_kind] == "feature"]["id"]), [0])
+
+        # Let the function find the values
+        test_df = pd.DataFrame([{"id": 0, "a": 3, "b": 5, "sort": 1}])
+        result_df, column_id, column_kind, column_value = \
+            dataframe_functions._normalize_input_to_internal_representation(test_df, "id", "sort", None, None)
+
+        self.assertEqual(column_id, "id")
+        self.assertEqual(column_value, "_values")
+        self.assertEqual(column_kind, "_variables")
+        self.assertIn("a", set(result_df[column_kind]))
+        self.assertIn("b", set(result_df[column_kind]))
+        six.assertCountEqual(self, list(result_df.columns), ["_values", "_variables", "id"])
+        self.assertEqual(list(result_df[result_df[column_kind] == "a"]["_values"]), [3])
+        self.assertEqual(list(result_df[result_df[column_kind] == "a"]["id"]), [0])
+        self.assertEqual(list(result_df[result_df[column_kind] == "b"]["_values"]), [5])
+        self.assertEqual(list(result_df[result_df[column_kind] == "b"]["id"]), [0])
+
+    def test_with_wrong_input(self):
+        test_df = pd.DataFrame([{"id": 0, "kind": "a", "value": 3, "sort": np.NaN}])
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_df,
+                          "id", "sort", "kind", "value")
+
+        test_df = pd.DataFrame([{"id": 0, "kind": "a", "value": 3, "sort": 1}])
+        self.assertRaises(AttributeError, dataframe_functions._normalize_input_to_internal_representation, test_df,
+                          "strange_id", "sort", "kind", "value")
+
+        test_df = pd.DataFrame([{"id": np.NaN, "kind": "a", "value": 3, "sort": 1}])
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_df,
+                          "id", "sort", "kind", "value")
+
+        test_df = pd.DataFrame([{"id": 2}, {"id": 1}])
+        test_dict = {"a": test_df, "b": test_df}
+
+        # If there are more than one column, the algorithm can not choose the correct column
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_dict,
+                          "id", None, None, None)
+
+        test_dict = {"a": pd.DataFrame([{"id": 2, "value_a": 3}, {"id": 1, "value_a": 4}]),
+                     "b": pd.DataFrame([{"id": 2}, {"id": 1}])}
+
+        # If there are more than one column, the algorithm can not choose the correct column
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_dict,
+                          "id", None, None, None)
+
+        test_df = pd.DataFrame([{"id": 0, "value": np.NaN}])
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_df,
+                          "id", None, None, "value")
+
+        test_df = pd.DataFrame([{"id": 0, "value": np.NaN}])
+        self.assertRaises(ValueError, dataframe_functions._normalize_input_to_internal_representation, test_df,
+                          None, None, None, "value")
+
+
+class RollingTestCase(TestCase):
+    def test_with_wrong_input(self):
+        test_df = pd.DataFrame({"id": [0, 0], "kind": ["a", "b"], "value": [3, 3], "sort": [np.NaN, np.NaN]})
+        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
+                          df_or_dict=test_df, column_id="id",
+                          column_sort="sort", column_kind="kind",
+                          rolling_direction=1)
+
+        test_df = pd.DataFrame({"id": [0, 0], "kind": ["a", "b"], "value": [3, 3], "sort": [1, 1]})
+        self.assertRaises(AttributeError, dataframe_functions.roll_time_series,
+                          df_or_dict=test_df, column_id="strange_id",
+                          column_sort="sort", column_kind="kind",
+                          rolling_direction=1)
+
+        test_df = {"a": pd.DataFrame([{"id": 0}])}
+        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
+                          df_or_dict=test_df, column_id="id",
+                          column_sort=None, column_kind="kind",
+                          rolling_direction=1)
+
+        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
+                          df_or_dict=test_df, column_id=None,
+                          column_sort=None, column_kind="kind",
+                          rolling_direction=1)
+
+        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
+                          df_or_dict=test_df, column_id="id",
+                          column_sort=None, column_kind=None,
+                          rolling_direction=0)
+
+        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
+                          df_or_dict=test_df, column_id=None,
+                          column_sort=None, column_kind=None,
+                          rolling_direction=0)
+
+    def test_assert_single_row(self):
+        test_df = pd.DataFrame([{"id": np.NaN, "kind": "a", "value": 3, "sort": 1}])
+        self.assertRaises(ValueError, dataframe_functions.roll_time_series,
+                          df_or_dict=test_df, column_id="id",
+                          column_sort="sort", column_kind="kind",
+                          rolling_direction=1)
+
+    def test_positive_rolling(self):
+        first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": range(4)})
+        second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
+
+        first_class["id"] = 1
+        second_class["id"] = 2
+
+        df_full = pd.concat([first_class, second_class], ignore_index=True)
+
+        """ df_full is
+            a   b  time  id
+        0   1   5     0   1
+        1   2   6     1   1
+        2   3   7     2   1
+        3   4   8     3   1
+        4  10  12    20   2
+        5  11  13    21   2
+        """
+        correct_indices = [0, 1, 1, 2, 2, 2, 3, 3, 3, 3, 20, 21, 21]
+        correct_values_a = [1.0, 1.0, 2.0, 1.0, 2.0, 3.0, 1.0, 2.0, 3.0, 4.0, 10.0, 10.0, 11.0]
+        correct_values_b = [5.0, 5.0, 6.0, 5.0, 6.0, 7.0, 5.0, 6.0, 7.0, 8.0, 12.0, 12.0, 13.0]
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=1)
+
+        self.assertListEqual(list(df["id"]), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=1,
+                                                  max_timeshift=4)
+
+
+        self.assertListEqual(list(df["id"]), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=1,
+                                                  max_timeshift=2)
+
+        correct_indices = [0, 1, 1, 2, 2, 2,  3, 3, 3, 20, 21, 21]
+        correct_values_a = [1.0, 1.0, 2.0, 1.0, 2.0, 3.0, 2.0, 3.0, 4.0, 10.0, 10.0, 11.0]
+        correct_values_b = [5.0, 5.0, 6.0, 5.0, 6.0, 7.0, 6.0, 7.0, 8.0, 12.0, 12.0, 13.0]
+
+        self.assertListEqual(list(df["id"]), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+
+    def test_negative_rolling(self):
+        first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": range(4)})
+        second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
+
+        first_class["id"] = 1
+        second_class["id"] = 2
+
+        df_full = pd.concat([first_class, second_class], ignore_index=True)
+        """ df_full is 
+            a   b  time  id
+        0   1   5     0   1
+        1   2   6     1   1
+        2   3   7     2   1
+        3   4   8     3   1
+        4  10  12    20   2
+        5  11  13    21   2
+        """
+
+        correct_indices = ([0, 0, 0, 0, 1, 1, 1, 2, 2, 3, 20, 20, 21])
+        correct_values_a = [1.0, 2.0, 3.0, 4.0, 2.0, 3.0, 4.0, 3.0, 4.0, 4.0, 10.0, 11.0, 11.0]
+        correct_values_b = [5.0, 6.0, 7.0, 8.0, 6.0, 7.0, 8.0, 7.0, 8.0, 8.0, 12.0, 13.0, 13.0]
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=-1)
+
+        self.assertListEqual(list(df["id"].values), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=-1,
+                                                  max_timeshift=None)
+
+        self.assertListEqual(list(df["id"].values), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=-1,
+                                                  max_timeshift=1)
+
+        correct_indices = ([0, 0, 1, 1, 2, 2, 3, 20, 20, 21])
+        correct_values_a = [1.0, 2.0, 2.0, 3.0, 3.0, 4.0, 4.0, 10.0, 11.0, 11.0]
+        correct_values_b = [5.0, 6.0, 6.0, 7.0, 7.0, 8.0, 8.0, 12.0, 13.0, 13.0]
+
+        self.assertListEqual(list(df["id"].values), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=-1,
+                                                  max_timeshift=2)
+
+        correct_indices = ([0, 0, 0, 1, 1, 1, 2, 2, 3, 20, 20, 21])
+        correct_values_a = [1.0, 2.0, 3.0, 2.0, 3.0, 4.0, 3.0, 4.0, 4.0, 10.0, 11.0, 11.0]
+        correct_values_b = [5.0, 6.0, 7.0, 6.0, 7.0, 8.0, 7.0, 8.0, 8.0, 12.0, 13.0, 13.0]
+
+        self.assertListEqual(list(df["id"].values), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+        df = dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                  column_kind=None, rolling_direction=-1,
+                                                  max_timeshift=4)
+
+        correct_indices = ([0, 0, 0, 0, 1, 1, 1, 2, 2, 3, 20, 20, 21])
+        correct_values_a = [1.0, 2.0, 3.0, 4.0, 2.0, 3.0, 4.0, 3.0, 4.0, 4.0, 10.0, 11.0, 11.0]
+        correct_values_b = [5.0, 6.0, 7.0, 8.0, 6.0, 7.0, 8.0, 7.0, 8.0, 8.0, 12.0, 13.0, 13.0]
+
+        self.assertListEqual(list(df["id"].values), correct_indices)
+        self.assertListEqual(list(df["a"].values), correct_values_a)
+        self.assertListEqual(list(df["b"].values), correct_values_b)
+
+    def test_stacked_rolling(self):
+        first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": range(4)})
+        second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
+
+        first_class["id"] = 1
+        second_class["id"] = 2
+
+        df_full = pd.concat([first_class, second_class], ignore_index=True)
+
+        df_stacked = pd.concat([df_full[["time", "id", "a"]].rename(columns={"a": "_value"}),
+                                df_full[["time", "id", "b"]].rename(columns={"b": "_value"})], ignore_index=True)
+        df_stacked["kind"] = ["a"] * 6 + ["b"] * 6
+
+        """ df_stacked is 
+            time  id  _value kind
+        0      0   1       1    a
+        1      1   1       2    a
+        2      2   1       3    a
+        3      3   1       4    a
+        4     20   2      10    a
+        5     21   2      11    a
+        6      0   1       5    b
+        7      1   1       6    b
+        8      2   1       7    b
+        9      3   1       8    b
+        10    20   2      12    b
+        11    21   2      13    b
+        """
+
+        df = dataframe_functions.roll_time_series(df_stacked, column_id="id", column_sort="time",
+                                                  column_kind="kind", rolling_direction=-1)
+
+        correct_indices = ([0]*2*4 + [1]*2*3 + [2]*2*2 + [3]*2*1 + [20]*4 + [21] *2)
+        self.assertListEqual(list(df["id"].values), correct_indices)
+
+        print(df["_value"].values)
+        self.assertListEqual(list(df["kind"].values), ["a", "b"] * 13)
+        self.assertListEqual(list(df["_value"].values),
+                             [1., 5., 2., 6., 3., 7., 4., 8., 2., 6., 3., 7., 4., 8., 3., 7., 4., 8., 4., 8., 10., 12.,
+                              11., 13., 11., 13.])
+
+    def test_dict_rolling(self):
+        df_dict = {
+            "a": pd.DataFrame({"_value": [1, 2, 3, 4, 10, 11], "id": [1, 1, 1, 1, 2, 2]}),
+            "b": pd.DataFrame({"_value": [5, 6, 7, 8, 12, 13], "id": [1, 1, 1, 1, 2, 2]})
+        }
+
+        df = dataframe_functions.roll_time_series(df_dict, column_id="id", column_sort=None,
+                                                  column_kind=None, rolling_direction=-1)
+        """ df is 
+        {a: _value  sort id
+         7      1.0   0.0  0
+         3      2.0   1.0  0
+         1      3.0   2.0  0
+         0      4.0   3.0  0
+         8      2.0   1.0  1
+         4      3.0   2.0  1
+         2      4.0   3.0  1
+         9      3.0   2.0  2
+         5      4.0   3.0  2
+         10     4.0   3.0  3
+         11    10.0   4.0  4
+         6     11.0   5.0  4
+         12    11.0   5.0  5, 
+         
+         b: _value  sort id
+         7      5.0   0.0  0
+         3      6.0   1.0  0
+         1      7.0   2.0  0
+         0      8.0   3.0  0
+         8      6.0   1.0  1
+         4      7.0   2.0  1
+         2      8.0   3.0  1
+         9      7.0   2.0  2
+         5      8.0   3.0  2
+         10     8.0   3.0  3
+         11    12.0   4.0  4
+         6     13.0   5.0  4
+         12    13.0   5.0  5}
+        """
+
+        correct_indices = [0, 0, 0, 0, 1, 1, 1, 2, 2, 3, 4, 4, 5]
+
+        self.assertListEqual(list(df["a"]["id"].values), correct_indices)
+        self.assertListEqual(list(df["b"]["id"].values), correct_indices)
+
+        self.assertListEqual(list(df["a"]["_value"].values),
+                             [1.0, 2.0, 3.0, 4.0, 2.0, 3.0, 4.0, 3.0, 4.0, 4.0, 10.0, 11.0, 11.0])
+        self.assertListEqual(list(df["b"]["_value"].values),
+                             [5.0, 6.0, 7.0, 8.0, 6.0, 7.0, 8.0, 7.0, 8.0, 8.0, 12.0, 13.0, 13.0])
+
+    def test_warning_on_non_uniform_time_steps(self):
+        with warnings.catch_warnings(record=True) as w:
+            first_class = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8], "time": [1, 2, 4, 5]})
+            second_class = pd.DataFrame({"a": [10, 11], "b": [12, 13], "time": range(20, 22)})
+
+            first_class["id"] = 1
+            second_class["id"] = 2
+
+            df_full = pd.concat([first_class, second_class], ignore_index=True)
+
+            dataframe_functions.roll_time_series(df_full, column_id="id", column_sort="time",
+                                                 column_kind=None, rolling_direction=1)
+
+            self.assertEqual(len(w), 1)
+            self.assertEqual(str(w[0].message),
+                             "Your time stamps are not uniformly sampled, which makes rolling "
+                             "nonsensical in some domains.")
+
+
+class CheckForNanTestCase(TestCase):
+    def test_all_columns(self):
+        test_df = pd.DataFrame([[1, 2, 3], [4, 5, 6]], index=[0, 1])
+
+        # should not raise an exception
+        dataframe_functions.check_for_nans_in_columns(test_df)
+
+        test_df = pd.DataFrame([[1, 2, 3], [4, np.NaN, 6]], index=[0, 1])
+
+        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df)
+
+    def test_not_all_columns(self):
+        test_df = pd.DataFrame([[1, 2, 3], [4, np.NaN, 6]], index=[0, 1], columns=["a", "b", "c"])
+
+        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df)
+        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, ["a", "b"])
+        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, ["b"])
+        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, "b")
+        self.assertRaises(ValueError, dataframe_functions.check_for_nans_in_columns, test_df, ["c", "b"])
+
+        dataframe_functions.check_for_nans_in_columns(test_df, columns=["a", "c"])
+        dataframe_functions.check_for_nans_in_columns(test_df, columns="a")
+
+
+class ImputeTestCase(TestCase):
+    def test_impute_zero(self):
+        df = pd.DataFrame([{"value": np.NaN}])
+        dataframe_functions.impute_dataframe_zero(df)
+        self.assertEqual(list(df.value), [0])
+
+        df = pd.DataFrame([{"value": np.PINF}])
+        dataframe_functions.impute_dataframe_zero(df)
+        self.assertEqual(list(df.value), [0])
+
+        df = pd.DataFrame([{"value": np.NINF}])
+        dataframe_functions.impute_dataframe_zero(df)
+        self.assertEqual(list(df.value), [0])
+
+        df = pd.DataFrame([{"value": np.NINF}, {"value": np.NaN}, {"value": np.PINF}, {"value": 1}])
+        dataframe_functions.impute_dataframe_zero(df)
+        self.assertEqual(list(df.value), [0, 0, 0, 1])
+
+        df = pd.DataFrame([{"value": np.NINF}, {"value": np.NaN}, {"value": np.PINF}, {"value": 1}])
+        df = df.astype(np.float64)
+        df = dataframe_functions.impute_dataframe_zero(df)
+        self.assertEqual(list(df.value), [0, 0, 0, 1])
+
+        df = pd.DataFrame([{"value": np.NINF}, {"value": np.NaN}, {"value": np.PINF}, {"value": 1}])
+        df = df.astype(np.float32)
+        df = dataframe_functions.impute_dataframe_zero(df)
+        self.assertEqual(list(df.value), [0, 0, 0, 1])
+
+    def test_toplevel_impute(self):
+        df = pd.DataFrame(np.transpose([[0, 1, 2, np.NaN], [1, np.PINF, 2, 3], [1, -3, np.NINF, 3]]),
+                          columns=["value_a", "value_b", "value_c"])
+
+        dataframe_functions.impute(df)
+
+        self.assertEqual(list(df.value_a), [0, 1, 2, 1])
+        self.assertEqual(list(df.value_b), [1, 3, 2, 3])
+        self.assertEqual(list(df.value_c), [1, -3, -3, 3])
+
+        df = pd.DataFrame(np.transpose([[0, 1, 2, np.NaN], [1, np.PINF, 2, np.NaN], [np.NaN, -3, np.NINF, 3]]),
+                          columns=["value_a", "value_b", "value_c"])
+        df = df.astype(np.float64, inplace=True)
+        dataframe_functions.impute(df)
+
+        self.assertEqual(list(df.value_a), [0, 1, 2, 1])
+        self.assertEqual(list(df.value_b), [1, 2, 2, 1.5])
+        self.assertEqual(list(df.value_c), [0, -3, -3, 3])
+
+        df = pd.DataFrame(np.transpose([[0, 1, 2, np.NaN], [1, np.PINF, 2, 3], [np.PINF, -3, np.NINF, 3]]),
+                          columns=["value_a", "value_b", "value_c"])
+        df = df.astype(np.float32, inplace=True)
+        dataframe_functions.impute(df)
+
+        self.assertEqual(list(df.value_a), [0, 1, 2, 1])
+        self.assertEqual(list(df.value_b), [1, 3, 2, 3])
+        self.assertEqual(list(df.value_c), [3, -3, -3, 3])
+
+    def test_impute_range(self):
+        def get_df():
+            return pd.DataFrame(np.transpose([[0, 1, 2, np.NaN],
+                                              [1, np.PINF, 2, 3],
+                                              [1, -3, np.NINF, 3]]),
+                                columns=["value_a", "value_b", "value_c"])
+
+        # check if values are replaced correctly
+        df = get_df()
+        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
+        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
+        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55}
+        dataframe_functions.impute_dataframe_range(df, col_to_max, col_to_min, col_to_median)
+        self.assertEqual(list(df.value_a), [0, 1, 2, 55])
+        self.assertEqual(list(df.value_b), [1, 200, 2, 3])
+        self.assertEqual(list(df.value_c), [1, -3, -134, 3])
+
+        # check for error if column key is missing
+        df = get_df()
+        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
+        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
+        col_to_median = {"value_a": 55, "value_c": 55}
+        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
+                          df, col_to_max, col_to_min, col_to_median)
+
+        # check for no error if column key is too much
+        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
+        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
+        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55, "value_d": 55}
+        dataframe_functions.impute_dataframe_range(df, col_to_max, col_to_min, col_to_median)
+
+        # check for error if replacement value is not finite
+        df = get_df()
+        col_to_max = {"value_a": 200, "value_b": np.NaN, "value_c": 200}
+        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
+        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55}
+        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
+                          df, col_to_max, col_to_min, col_to_median)
+        df = get_df()
+        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
+        col_to_min = {"value_a": -134, "value_b": np.NINF, "value_c": -134}
+        col_to_median = {"value_a": 55, "value_b": 55, "value_c": 55}
+        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
+                          df, col_to_max, col_to_min, col_to_median)
+
+        df = get_df()
+        col_to_max = {"value_a": 200, "value_b": 200, "value_c": 200}
+        col_to_min = {"value_a": -134, "value_b": -134, "value_c": -134}
+        col_to_median = {"value_a": 55, "value_b": 55, "value_c": np.PINF}
+        self.assertRaises(ValueError, dataframe_functions.impute_dataframe_range,
+                          df, col_to_max, col_to_min, col_to_median)
+
+
+        df = pd.DataFrame([0, 1, 2, 3, 4], columns=["test"])
+        col_dict = {"test": 0}
+        dataframe_functions.impute_dataframe_range(df, col_dict, col_dict, col_dict)
+
+        self.assertEqual(df.columns, ["test"])
+        self.assertListEqual(list(df["test"].values), [0, 1, 2, 3, 4])
+
+
+class RestrictTestCase(TestCase):
+    def test_restrict_dataframe(self):
+        df = pd.DataFrame({'id': [1, 2, 3] * 2})
+
+        df_restricted = dataframe_functions.restrict_input_to_index(df, 'id', [2])
+        self.assertEqual(list(df_restricted.id), [2, 2])
+
+        df_restricted2 = dataframe_functions.restrict_input_to_index(df, 'id', [1, 2, 3])
+        self.assertTrue(df_restricted2.equals(df))
+
+    def test_restrict_dict(self):
+        kind_to_df = {'a': pd.DataFrame({'id': [1, 2, 3]}), 'b': pd.DataFrame({'id': [3, 4, 5]})}
+
+        kind_to_df_restricted = dataframe_functions.restrict_input_to_index(kind_to_df, 'id', [3])
+        self.assertEqual(list(kind_to_df_restricted['a'].id), [3])
+        self.assertEqual(list(kind_to_df_restricted['b'].id), [3])
+
+        kind_to_df_restricted2 = dataframe_functions.restrict_input_to_index(kind_to_df, 'id', [1, 2, 3, 4, 5])
+        self.assertTrue(kind_to_df_restricted2['a'].equals(kind_to_df['a']))
+        self.assertTrue(kind_to_df_restricted2['b'].equals(kind_to_df['b']))
+
+    def test_restrict_wrong(self):
+        other_type = np.array([1, 2, 3])
+
+        self.assertRaises(TypeError, dataframe_functions.restrict_input_to_index, other_type, "id", [1, 2, 3])
+
+
+class GetRangeValuesPerColumnTestCase(TestCase):
+    def test_ignores_non_finite_values(self):
+        df = pd.DataFrame([0, 1, 2, 3, np.NaN, np.PINF, np.NINF], columns=["value"])
+
+        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
+
+        self.assertEqual(col_to_max, {"value": 3})
+        self.assertEqual(col_to_min, {"value": 0})
+        self.assertEqual(col_to_median, {"value": 1.5})
+
+    def test_range_values_correct_with_even_length(self):
+        df = pd.DataFrame([0, 1, 2, 3], columns=["value"])
+
+        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
+
+        self.assertEqual(col_to_max, {"value": 3})
+        self.assertEqual(col_to_min, {"value": 0})
+        self.assertEqual(col_to_median, {"value": 1.5})
+
+    def test_range_values_correct_with_uneven_length(self):
+        df = pd.DataFrame([0, 1, 2], columns=["value"])
+
+        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
+
+        self.assertEqual(col_to_max, {"value": 2})
+        self.assertEqual(col_to_min, {"value": 0})
+        self.assertEqual(col_to_median, {"value": 1})
+
+    def test_no_finite_values_yields_0(self):
+        df = pd.DataFrame([np.NaN, np.PINF, np.NINF], columns=["value"])
+
+        col_to_max, col_to_min, col_to_median = dataframe_functions.get_range_values_per_column(df)
+
+        self.assertEqual(col_to_max, {"value": 0})
+        self.assertEqual(col_to_min, {"value": 0})
+        self.assertEqual(col_to_median, {"value": 0})
+
+
+class MakeForecastingFrameTestCase(TestCase):
+
+    def test_make_forecasting_frame_list(self):
+        df, y = dataframe_functions.make_forecasting_frame(x=range(4), kind="test", max_timeshift=1, rolling_direction=1)
+        expected_df = pd.DataFrame({"id": [1, 2, 3], "kind": ["test"]*3, "value": [0., 1., 2.], "time": [0., 1., 2.]})
+
+        expected_y = pd.Series(data=[1, 2, 3], index=[1, 2, 3], name="value")
+        assert_frame_equal(df.sort_index(axis=1), expected_df.sort_index(axis=1))
+        assert_series_equal(y, expected_y)
+
+    def test_make_forecasting_frame_range(self):
+        df, y = dataframe_functions.make_forecasting_frame(x=np.arange(4), kind="test", max_timeshift=1, rolling_direction=1)
+        expected_df = pd.DataFrame({"id": [1, 2, 3], "kind": ["test"]*3, "value": [0., 1., 2.], "time": [0., 1., 2.]})
+        assert_frame_equal(df.sort_index(axis=1), expected_df.sort_index(axis=1))
+
+    def test_make_forecasting_frame_pdSeries(self):
+
+        t_index = pd.date_range('1/1/2011', periods=4, freq='H')
+        df, y = dataframe_functions.make_forecasting_frame(x=pd.Series(data=range(4), index=t_index),
+                                                           kind="test", max_timeshift=1, rolling_direction=1)
+
+        expected_y = pd.Series(data=[1, 2, 3], index=pd.DatetimeIndex(["2011-01-01 01:00:00", "2011-01-01 02:00:00",
+                                                                       "2011-01-01 03:00:00"]), name="value")
+        expected_df = pd.DataFrame({"id": pd.DatetimeIndex(["2011-01-01 01:00:00", "2011-01-01 02:00:00",
+                                                            "2011-01-01 03:00:00"]),
+                                    "kind": ["test"]*3, "value": [0., 1., 2.],
+                                    "time": pd.DatetimeIndex(["2011-01-01 00:00:00", "2011-01-01 01:00:00",
+                                                              "2011-01-01 02:00:00"])
+                                    })
+        assert_frame_equal(df.sort_index(axis=1), expected_df.sort_index(axis=1))
+        assert_series_equal(y, expected_y)
```

### Comparing `tsfresh-0.8.1/tsfresh/__init__.py` & `tsfresh-0.9.0/tsfresh/__init__.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/convenience/relevant_extraction.py` & `tsfresh-0.9.0/tsfresh/convenience/relevant_extraction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,160 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-from __future__ import absolute_import
-import pandas as pd
-from tsfresh.feature_extraction import extract_features
-from tsfresh import defaults
-from tsfresh.feature_selection import select_features
-from tsfresh.utilities.dataframe_functions import restrict_input_to_index, impute
-
-
-def extract_relevant_features(timeseries_container, y, X=None,
-                              default_fc_parameters=None,
-                              kind_to_fc_parameters=None,
-                              column_id=None, column_sort=None, column_kind=None, column_value=None,
-                              parallelization=defaults.PARALLELISATION,
-                              show_warnings=defaults.SHOW_WARNINGS,
-                              disable_progressbar=defaults.DISABLE_PROGRESSBAR,
-                              profile=defaults.PROFILING,
-                              profiling_filename=defaults.PROFILING_FILENAME,
-                              profiling_sorting=defaults.PROFILING_SORTING,
-                              test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
-                              test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
-                              test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
-                              test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
-                              fdr_level=defaults.FDR_LEVEL,
-                              hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
-                              n_processes=defaults.N_PROCESSES,
-                              chunksize=defaults.CHUNKSIZE):
-    """
-    High level convenience function to extract time series features from `timeseries_container`. Then return feature
-    matrix `X` possibly augmented with relevent features with respect to target vector `y`.
-
-    For more details see the documentation of :func:`~tsfresh.feature_extraction.extraction.extract_features` and
-    :func:`~tsfresh.feature_selection.selection.select_features`.
-
-    Examples
-    ========
-
-    >>> from tsfresh.examples import load_robot_execution_failures
-    >>> from tsfresh import extract_relevant_features
-    >>> df, y = load_robot_execution_failures()
-    >>> X = extract_relevant_features(df, y, column_id='id', column_sort='time')
-
-    :param timeseries_container: The pandas.DataFrame with the time series to compute the features for, or a
-            dictionary of pandas.DataFrames.
-            See :func:`~tsfresh.feature_extraction.extraction.extract_features`.
-
-    :param X: A DataFrame containing additional features
-    :type X: pandas.DataFrame
-
-    :param y: The target vector
-    :type y: pandas.Series
-
-    :param default_fc_parameters: mapping from feature calculator names to parameters. Only those names
-           which are keys in this dict will be calculated. See the class:`ComprehensiveFCParameters` for
-           more information.
-    :type default_fc_parameters: dict
-
-    :param kind_to_fc_parameters: mapping from kind names to objects of the same type as the ones for
-            default_fc_parameters. If you put a kind as a key here, the fc_parameters
-            object (which is the value), will be used instead of the default_fc_parameters.
-    :type kind_to_fc_parameters: dict
-
-    :param column_id: The name of the id column to group by.
-    :type column_id: str
-
-    :param column_sort: The name of the sort column.
-    :type column_sort: str
-
-    :param column_kind: The name of the column keeping record on the kind of the value.
-    :type column_kind: str
-
-    :param column_value: The name for the column keeping the value itself.
-    :type column_value: str
-
-    :param parallelization: Either ``'per_sample'`` or ``'per_kind'``   , see
-                            :func:`~tsfresh.feature_extraction.extraction._extract_features_parallel_per_sample`,
-                            :func:`~tsfresh.feature_extraction.extraction._extract_features_parallel_per_kind` and
-                            :ref:`parallelization-label` for details.
-                            Choosing None makes the algorithm look for the best parallelization technique by applying
-                            some general remarks.
-    :type parallelization: str
-
-    :param chunksize: The size of one chunk for the parallelisation
-    :type chunksize: None or int
-
-    :param n_processes: The number of processes to use for parallelisation.
-    :type n_processes: int
-
-    :param: show_warnings: Show warnings during the feature extraction (needed for debugging of calculators).
-    :type show_warnings: bool
-
-    :param disable_progressbar: Do not show a progressbar while doing the calculation.
-    :type disable_progressbar: bool
-
-    :param profile: Turn on profiling during feature extraction
-    :type profile: bool
-
-    :param profiling_sorting: How to sort the profiling results (see the documentation of the profiling package for
-           more information)
-    :type profiling_sorting: basestring
-
-    :param profiling_filename: Where to save the profiling results.
-    :type profiling_filename: basestring
-
-    :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
-    :type test_for_binary_target_binary_feature: str
-
-    :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
-    :type test_for_binary_target_real_feature: str
-
-    :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
-    :type test_for_real_target_binary_feature: str
-
-    :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
-    :type test_for_real_target_real_feature: str
-
-    :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
-                      features among all created features.
-    :type fdr_level: float
-
-    :param hypotheses_independent: Can the significance of the features be assumed to be independent?
-                                   Normally, this should be set to False as the features are never
-                                   independent (e.g. mean and median)
-    :type hypotheses_independent: bool
-
-    :param write_selection_report: Whether to store the selection report after the Benjamini Hochberg procedure has
-                                   finished.
-    :type write_selection_report: bool
-
-    :param result_dir: Where to store the selection report
-    :type result_dir: str
-
-    :return: Feature matrix X, possibly extended with relevant time series features.
-    """
-    if X is not None:
-        timeseries_container = restrict_input_to_index(timeseries_container, column_id, X.index)
-
-    X_ext = extract_features(timeseries_container,
-                             default_fc_parameters=default_fc_parameters,
-                             kind_to_fc_parameters=kind_to_fc_parameters,
-                             parallelization=parallelization,
-                             show_warnings=show_warnings,
-                             disable_progressbar=disable_progressbar,
-                             profile=profile,
-                             profiling_filename=profiling_filename,
-                             profiling_sorting=profiling_sorting,
-                             column_id=column_id, column_sort=column_sort,
-                             column_kind=column_kind, column_value=column_value,
-                             impute_function=impute)
-
-    X_sel = select_features(X_ext, y,
-                            test_for_binary_target_binary_feature=test_for_binary_target_binary_feature,
-                            test_for_binary_target_real_feature=test_for_binary_target_real_feature,
-                            test_for_real_target_binary_feature=test_for_real_target_binary_feature,
-                            test_for_real_target_real_feature=test_for_real_target_real_feature,
-                            fdr_level=fdr_level, hypotheses_independent=hypotheses_independent,
-                            n_processes=n_processes,
-                            chunksize=chunksize)
-
-    if X is None:
-        X = X_sel
-    else:
-        X = pd.merge(X, X_sel, left_index=True, right_index=True, how="left")
-
-    return X
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+from __future__ import absolute_import
+import pandas as pd
+from tsfresh.feature_extraction import extract_features
+from tsfresh import defaults
+from tsfresh.feature_selection import select_features
+from tsfresh.utilities.dataframe_functions import restrict_input_to_index, impute
+
+
+def extract_relevant_features(timeseries_container, y, X=None,
+                              default_fc_parameters=None,
+                              kind_to_fc_parameters=None,
+                              column_id=None, column_sort=None, column_kind=None, column_value=None,
+                              show_warnings=defaults.SHOW_WARNINGS,
+                              disable_progressbar=defaults.DISABLE_PROGRESSBAR,
+                              profile=defaults.PROFILING,
+                              profiling_filename=defaults.PROFILING_FILENAME,
+                              profiling_sorting=defaults.PROFILING_SORTING,
+                              test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
+                              test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
+                              test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
+                              test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
+                              fdr_level=defaults.FDR_LEVEL,
+                              hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
+                              n_jobs=defaults.N_PROCESSES,
+                              chunksize=defaults.CHUNKSIZE,
+                              ml_task='auto'):
+    """
+    High level convenience function to extract time series features from `timeseries_container`. Then return feature
+    matrix `X` possibly augmented with relevent features with respect to target vector `y`.
+
+    For more details see the documentation of :func:`~tsfresh.feature_extraction.extraction.extract_features` and
+    :func:`~tsfresh.feature_selection.selection.select_features`.
+
+    Examples
+    ========
+
+    >>> from tsfresh.examples import load_robot_execution_failures
+    >>> from tsfresh import extract_relevant_features
+    >>> df, y = load_robot_execution_failures()
+    >>> X = extract_relevant_features(df, y, column_id='id', column_sort='time')
+
+    :param timeseries_container: The pandas.DataFrame with the time series to compute the features for, or a
+            dictionary of pandas.DataFrames.
+            See :func:`~tsfresh.feature_extraction.extraction.extract_features`.
+
+    :param X: A DataFrame containing additional features
+    :type X: pandas.DataFrame
+
+    :param y: The target vector
+    :type y: pandas.Series
+
+    :param default_fc_parameters: mapping from feature calculator names to parameters. Only those names
+           which are keys in this dict will be calculated. See the class:`ComprehensiveFCParameters` for
+           more information.
+    :type default_fc_parameters: dict
+
+    :param kind_to_fc_parameters: mapping from kind names to objects of the same type as the ones for
+            default_fc_parameters. If you put a kind as a key here, the fc_parameters
+            object (which is the value), will be used instead of the default_fc_parameters.
+    :type kind_to_fc_parameters: dict
+
+    :param column_id: The name of the id column to group by.
+    :type column_id: str
+
+    :param column_sort: The name of the sort column.
+    :type column_sort: str
+
+    :param column_kind: The name of the column keeping record on the kind of the value.
+    :type column_kind: str
+
+    :param column_value: The name for the column keeping the value itself.
+    :type column_value: str
+
+    :param chunksize: The size of one chunk for the parallelisation
+    :type chunksize: None or int
+
+    :param n_jobs: The number of processes to use for parallelization. If zero, no parallelization is used.
+    :type n_jobs: int
+
+    :param: show_warnings: Show warnings during the feature extraction (needed for debugging of calculators).
+    :type show_warnings: bool
+
+    :param disable_progressbar: Do not show a progressbar while doing the calculation.
+    :type disable_progressbar: bool
+
+    :param profile: Turn on profiling during feature extraction
+    :type profile: bool
+
+    :param profiling_sorting: How to sort the profiling results (see the documentation of the profiling package for
+           more information)
+    :type profiling_sorting: basestring
+
+    :param profiling_filename: Where to save the profiling results.
+    :type profiling_filename: basestring
+
+    :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
+    :type test_for_binary_target_binary_feature: str
+
+    :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
+    :type test_for_binary_target_real_feature: str
+
+    :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
+    :type test_for_real_target_binary_feature: str
+
+    :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
+    :type test_for_real_target_real_feature: str
+
+    :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
+                      features among all created features.
+    :type fdr_level: float
+
+    :param hypotheses_independent: Can the significance of the features be assumed to be independent?
+                                   Normally, this should be set to False as the features are never
+                                   independent (e.g. mean and median)
+    :type hypotheses_independent: bool
+
+    :param ml_task: The intended machine learning task. Either `'classification'`, `'regression'` or `'auto'`.
+                    Defaults to `'auto'`, meaning the intended task is inferred from `y`.
+                    If `y` has a boolean, integer or object dtype, the task is assumend to be classification,
+                    else regression.
+    :type ml_task: str
+
+    :return: Feature matrix X, possibly extended with relevant time series features.
+    """
+    if X is not None:
+        timeseries_container = restrict_input_to_index(timeseries_container, column_id, X.index)
+
+    X_ext = extract_features(timeseries_container,
+                             default_fc_parameters=default_fc_parameters,
+                             kind_to_fc_parameters=kind_to_fc_parameters,
+                             show_warnings=show_warnings,
+                             disable_progressbar=disable_progressbar,
+                             profile=profile,
+                             profiling_filename=profiling_filename,
+                             profiling_sorting=profiling_sorting,
+                             n_jobs=n_jobs,
+                             column_id=column_id, column_sort=column_sort,
+                             column_kind=column_kind, column_value=column_value,
+                             impute_function=impute)
+
+    X_sel = select_features(X_ext, y,
+                            test_for_binary_target_binary_feature=test_for_binary_target_binary_feature,
+                            test_for_binary_target_real_feature=test_for_binary_target_real_feature,
+                            test_for_real_target_binary_feature=test_for_real_target_binary_feature,
+                            test_for_real_target_real_feature=test_for_real_target_real_feature,
+                            fdr_level=fdr_level, hypotheses_independent=hypotheses_independent,
+                            n_jobs=n_jobs,
+                            chunksize=chunksize,
+                            ml_task=ml_task)
+
+    if X is None:
+        X = X_sel
+    else:
+        X = pd.merge(X, X_sel, left_index=True, right_index=True, how="left")
+
+    return X
```

### Comparing `tsfresh-0.8.1/tsfresh/defaults.py` & `tsfresh-0.9.0/tsfresh/defaults.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import os
-from multiprocessing import cpu_count
-
-n_cores = int(os.getenv("NUMBER_OF_CPUS") or cpu_count())
-
-CHUNKSIZE = None
-N_PROCESSES = max(1, n_cores // 2)
-PROFILING = False
-PROFILING_SORTING = "cumulative"
-PROFILING_FILENAME = "profile.txt"
-IMPUTE_FUNCTION = None
-DISABLE_PROGRESSBAR = False
-SHOW_WARNINGS = False
-PARALLELISATION = None
-TEST_FOR_BINARY_TARGET_BINARY_FEATURE = "fisher"
-TEST_FOR_BINARY_TARGET_REAL_FEATURE = "mann"
-TEST_FOR_REAL_TARGET_BINARY_FEATURE = "mann"
-TEST_FOR_REAL_TARGET_REAL_FEATURE = "kendall"
-FDR_LEVEL = 0.05
-HYPOTHESES_INDEPENDENT = False
-WRITE_SELECTION_REPORT = False
-RESULT_DIR = "logging"
+import os
+from multiprocessing import cpu_count
+
+n_cores = int(os.getenv("NUMBER_OF_CPUS") or cpu_count())
+
+CHUNKSIZE = None
+N_PROCESSES = max(1, n_cores // 2)
+PROFILING = False
+PROFILING_SORTING = "cumulative"
+PROFILING_FILENAME = "profile.txt"
+IMPUTE_FUNCTION = None
+DISABLE_PROGRESSBAR = False
+SHOW_WARNINGS = False
+PARALLELISATION = True
+TEST_FOR_BINARY_TARGET_BINARY_FEATURE = "fisher"
+TEST_FOR_BINARY_TARGET_REAL_FEATURE = "mann"
+TEST_FOR_REAL_TARGET_BINARY_FEATURE = "mann"
+TEST_FOR_REAL_TARGET_REAL_FEATURE = "kendall"
+FDR_LEVEL = 0.05
+HYPOTHESES_INDEPENDENT = False
+WRITE_SELECTION_REPORT = False
+RESULT_DIR = "logging"
```

### Comparing `tsfresh-0.8.1/tsfresh/examples/driftbif_simulation.py` & `tsfresh-0.9.0/tsfresh/examples/driftbif_simulation.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/examples/har_dataset.py` & `tsfresh-0.9.0/tsfresh/examples/har_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-"""
-This module implements functions to download and load the Human Activity Recognition dataset [4].
-A description of the data set can be found in [5].
-
-
-References
-----------
-
-.. [4] http://mlr.cs.umass.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
-.. [5] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. (2013)
-     A Public Domain Dataset for Human Activity Recognition Using Smartphones.
-     21th European Symposium on Artificial Neural Networks,
-     Computational Intelligence and Machine Learning, ESANN 2013. Bruges, Belgium 24-26 April 2013.
-
-"""
-
-from __future__ import absolute_import, division
-from io import BytesIO
-from urllib.request import urlopen
-from zipfile import ZipFile
-import pandas as pd
-import os
-import logging
-
-_logger = logging.getLogger(__name__)
-
-module_path = os.path.dirname(__file__)
-data_file_name = os.path.join(module_path, 'data')
-data_file_name_dataset = os.path.join(module_path, 'data', 'UCI HAR Dataset', 'train', 'Inertial Signals',
-                                      'body_acc_x_train.txt')
-data_file_name_classes = os.path.join(module_path, 'data', 'UCI HAR Dataset', 'train', 'y_train.txt')
-
-
-def download_har_dataset():
-    """
-    Download human activity recognition dataset from UCI ML Repository and store it at /tsfresh/notebooks/data.
-    
-    Examples
-    ========
-
-    >>> from tsfresh.examples import har_dataset
-    >>> har_dataset.download_har_dataset()
-    """
-
-    zipurl = 'https://github.com/MaxBenChrist/human-activity-dataset/blob/master/UCI%20HAR%20Dataset.zip?raw=true'
-
-    if os.path.exists(data_file_name_dataset) and os.path.exists(data_file_name_classes):
-        _logger.warning("You have already downloaded the Human Activity Data Set.")
-        return
-
-    with urlopen(zipurl) as zipresp:
-        with ZipFile(BytesIO(zipresp.read())) as zfile:
-            zfile.extractall(path=data_file_name)
-        zfile.close()
-
-
-def load_har_dataset():
-    try:
-        return pd.read_csv(data_file_name_dataset, delim_whitespace=True, header=None)
-    except IOError:
-        raise IOError('File {} was not found. Have you downloaded the dataset with download_har_dataset() '
-                      'before?'.format(data_file_name_dataset))
-
-
-def load_har_classes():
-    try:
-        return pd.read_csv(data_file_name_classes, delim_whitespace=True, header=None, squeeze=True)
-    except IOError:
-        raise IOError('File {} was not found. Have you downloaded the dataset with download_har_dataset() '
-                      'before?'.format(data_file_name_classes))
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+"""
+This module implements functions to download and load the Human Activity Recognition dataset [4].
+A description of the data set can be found in [5].
+
+
+References
+----------
+
+.. [4] https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
+.. [5] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. (2013)
+     A Public Domain Dataset for Human Activity Recognition Using Smartphones.
+     21th European Symposium on Artificial Neural Networks,
+     Computational Intelligence and Machine Learning, ESANN 2013. Bruges, Belgium 24-26 April 2013.
+
+"""
+
+from __future__ import absolute_import, division
+from io import BytesIO
+from urllib.request import urlopen
+from zipfile import ZipFile
+import pandas as pd
+import os
+import logging
+
+_logger = logging.getLogger(__name__)
+
+module_path = os.path.dirname(__file__)
+data_file_name = os.path.join(module_path, 'data')
+data_file_name_dataset = os.path.join(module_path, 'data', 'UCI HAR Dataset', 'train', 'Inertial Signals',
+                                      'body_acc_x_train.txt')
+data_file_name_classes = os.path.join(module_path, 'data', 'UCI HAR Dataset', 'train', 'y_train.txt')
+
+
+def download_har_dataset():
+    """
+    Download human activity recognition dataset from UCI ML Repository and store it at /tsfresh/notebooks/data.
+    
+    Examples
+    ========
+
+    >>> from tsfresh.examples import har_dataset
+    >>> har_dataset.download_har_dataset()
+    """
+
+    zipurl = 'https://github.com/MaxBenChrist/human-activity-dataset/blob/master/UCI%20HAR%20Dataset.zip?raw=true'
+
+    if os.path.exists(data_file_name_dataset) and os.path.exists(data_file_name_classes):
+        _logger.warning("You have already downloaded the Human Activity Data Set.")
+        return
+
+    with urlopen(zipurl) as zipresp:
+        with ZipFile(BytesIO(zipresp.read())) as zfile:
+            zfile.extractall(path=data_file_name)
+        zfile.close()
+
+
+def load_har_dataset():
+    try:
+        return pd.read_csv(data_file_name_dataset, delim_whitespace=True, header=None)
+    except IOError:
+        raise IOError('File {} was not found. Have you downloaded the dataset with download_har_dataset() '
+                      'before?'.format(data_file_name_dataset))
+
+
+def load_har_classes():
+    try:
+        return pd.read_csv(data_file_name_classes, delim_whitespace=True, header=None, squeeze=True)
+    except IOError:
+        raise IOError('File {} was not found. Have you downloaded the dataset with download_har_dataset() '
+                      'before?'.format(data_file_name_classes))
```

### Comparing `tsfresh-0.8.1/tsfresh/examples/robot_execution_failures.py` & `tsfresh-0.9.0/tsfresh/examples/robot_execution_failures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,118 +1,120 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-"""
-This module implements functions to download the Robot Execution Failures LP1 Data Set[1] and load it as as DataFrame.
-
-*Important:* You need to download the data set yourself, either manually or via the function
-:func:`~tsfresh.examples.robot_execution_failures.download_robot_execution_failures`
-
-References
-----------
-.. [1] http://mlr.cs.umass.edu/ml/datasets/Robot+Execution+Failures
-.. [2] Lichman, M. (2013).
-    UCI Machine Learning Repository [http://mlr.cs.umass.edu/ml].
-    Irvine, CA: University of California, School of Information and Computer Science.
-.. [3] Camarinha-Matos, L.M., L. Seabra Lopes, and J. Barata (1996).
-    Integration and Learning in Supervision of Flexible Assembly Systems.
-    "IEEE Transactions on Robotics and Automation", 12 (2), 202-219
-
-"""
-
-from __future__ import absolute_import, division
-
-from builtins import map
-import os
-import pandas as pd
-import requests
-import logging
-
-_logger = logging.getLogger(__name__)
-
-UCI_MLD_REF_MSG = ("The example data could not be found. You need to download the Robot Execution Failures "
-                   "LP1 Data Set from the UCI Machine Learning Repository. To do so, you can call the function "
-                   "tsfresh.examples.robot_execution_failures.download_robot_execution_failures")
-UCI_MLD_REF_URL = "https://raw.githubusercontent.com/MaxBenChrist/robot-failure-dataset/master/lp1.data.txt"
-
-module_path = os.path.dirname(__file__)
-data_file_name = os.path.join(module_path, 'data', 'robotfailure-mld', 'lp1.data')
-
-
-def download_robot_execution_failures():
-    """
-    Download the Robot Execution Failures LP1 Data Set[1] from the UCI Machine Learning Repository[2] and store it locally.
-    :return:
-
-    Examples
-    ========
-
-    >>> from tsfresh.examples import download_robot_execution_failures
-    >>> download_robot_execution_failures()
-    """
-    if os.path.exists(data_file_name):
-        _logger.warning("You have already downloaded the Robot Execution Failures LP1 Data Set.")
-        return
-
-    if not os.access(module_path, os.W_OK):
-        raise RuntimeError("You don't have the necessary permissions to download the Robot Execution Failures LP1 Data "
-                           "Set into the module path. Consider installing the module in a virtualenv you "
-                           "own or run this function with appropriate permissions.")
-
-    os.makedirs(os.path.dirname(data_file_name))
-
-    r = requests.get(UCI_MLD_REF_URL)
-
-    if r.status_code != 200:
-        raise RuntimeError("Could not download the Robot Execution Failures LP1 Data Set from the UCI Machine Learning "
-                           "Repository. HTTP status code: {}".format(r.status_code))
-
-    with open(data_file_name, "w") as f:
-        f.write(r.text)
-
-
-def load_robot_execution_failures():
-    """
-    Load the Robot Execution Failures LP1 Data Set[1].
-    The Time series are passed as a flat DataFrame.
-
-    Examples
-    ========
-
-    >>> from tsfresh.examples import load_robot_execution_failures
-    >>> df, y = load_robot_execution_failures()
-    >>> print(df.shape)
-    (1320, 8)
-
-    :return: time series data as :class:`pandas.DataFrame` and target vector as :class:`pandas.Series`
-    :rtype: tuple
-    """
-    if not os.path.exists(data_file_name):
-        raise RuntimeError(UCI_MLD_REF_MSG)
-
-    id_to_target = {}
-    df_rows = []
-
-    with open(data_file_name) as f:
-        cur_id = 0
-        time = 0
-
-        for line in f.readlines():
-            # New sample --> increase id, reset time and determine target
-            if line[0] not in ['\t', '\n']:
-                cur_id += 1
-                time = 0
-                if line.strip() == 'normal':
-                    id_to_target[cur_id] = 0
-                else:
-                    id_to_target[cur_id] = 1
-            # Data row --> split and convert values, create complete df row
-            elif line[0] == '\t':
-                values = list(map(int, line.split('\t')[1:]))
-                df_rows.append([cur_id, time] + values)
-                time += 1
-
-    df = pd.DataFrame(df_rows, columns=['id', 'time', 'a', 'b', 'c', 'd', 'e', 'f'])
-    y = pd.Series(id_to_target)
-
-    return df, y
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+"""
+This module implements functions to download the Robot Execution Failures LP1 Data Set[1] and load it as as DataFrame.
+
+*Important:* You need to download the data set yourself, either manually or via the function
+:func:`~tsfresh.examples.robot_execution_failures.download_robot_execution_failures`
+
+References
+----------
+.. [1] https://archive.ics.uci.edu/ml/datasets/Robot+Execution+Failures
+.. [2] Lichman, M. (2013).
+    UCI Machine Learning Repository [https://archive.ics.uci.edu/ml].
+    Irvine, CA: University of California, School of Information and Computer Science.
+.. [3] Camarinha-Matos, L.M., L. Seabra Lopes, and J. Barata (1996).
+    Integration and Learning in Supervision of Flexible Assembly Systems.
+    "IEEE Transactions on Robotics and Automation", 12 (2), 202-219
+
+"""
+
+from __future__ import absolute_import, division
+
+from builtins import map
+import os
+import pandas as pd
+import requests
+import logging
+
+_logger = logging.getLogger(__name__)
+
+UCI_MLD_REF_MSG = ("The example data could not be found. You need to download the Robot Execution Failures "
+                   "LP1 Data Set from the UCI Machine Learning Repository. To do so, you can call the function "
+                   "tsfresh.examples.robot_execution_failures.download_robot_execution_failures")
+UCI_MLD_REF_URL = "https://raw.githubusercontent.com/MaxBenChrist/robot-failure-dataset/master/lp1.data.txt"
+
+module_path = os.path.dirname(__file__)
+data_file_name = os.path.join(module_path, 'data', 'robotfailure-mld', 'lp1.data')
+
+
+def download_robot_execution_failures():
+    """
+    Download the Robot Execution Failures LP1 Data Set[1] from the UCI Machine Learning Repository[2] and store it locally.
+    :return:
+
+    Examples
+    ========
+
+    >>> from tsfresh.examples import download_robot_execution_failures
+    >>> download_robot_execution_failures()
+    """
+    if os.path.exists(data_file_name):
+        _logger.warning("You have already downloaded the Robot Execution Failures LP1 Data Set.")
+        return
+
+    if not os.access(module_path, os.W_OK):
+        raise RuntimeError("You don't have the necessary permissions to download the Robot Execution Failures LP1 Data "
+                           "Set into the module path. Consider installing the module in a virtualenv you "
+                           "own or run this function with appropriate permissions.")
+
+    os.makedirs(os.path.dirname(data_file_name))
+
+    r = requests.get(UCI_MLD_REF_URL)
+
+    if r.status_code != 200:
+        raise RuntimeError("Could not download the Robot Execution Failures LP1 Data Set from the UCI Machine Learning "
+                           "Repository. HTTP status code: {}".format(r.status_code))
+
+    with open(data_file_name, "w") as f:
+        f.write(r.text)
+
+
+def load_robot_execution_failures(multiclass=False):
+    """
+    Load the Robot Execution Failures LP1 Data Set[1].
+    The Time series are passed as a flat DataFrame.
+
+    Examples
+    ========
+
+    >>> from tsfresh.examples import load_robot_execution_failures
+    >>> df, y = load_robot_execution_failures()
+    >>> print(df.shape)
+    (1320, 8)
+
+    :param multiclass: If True, return all target labels. The default returns only "normal" vs all other labels.
+    :type multiclass: bool
+    :return: time series data as :class:`pandas.DataFrame` and target vector as :class:`pandas.Series`
+    :rtype: tuple
+    """
+    if not os.path.exists(data_file_name):
+        raise RuntimeError(UCI_MLD_REF_MSG)
+
+    id_to_target = {}
+    df_rows = []
+
+    with open(data_file_name) as f:
+        cur_id = 0
+        time = 0
+
+        for line in f.readlines():
+            # New sample --> increase id, reset time and determine target
+            if line[0] not in ['\t', '\n']:
+                cur_id += 1
+                time = 0
+                if multiclass:
+                    id_to_target[cur_id] = line.strip()
+                else:
+                    id_to_target[cur_id] = (line.strip() == 'normal')
+            # Data row --> split and convert values, create complete df row
+            elif line[0] == '\t':
+                values = list(map(int, line.split('\t')[1:]))
+                df_rows.append([cur_id, time] + values)
+                time += 1
+
+    df = pd.DataFrame(df_rows, columns=['id', 'time', 'F_x', 'F_y', 'F_z', 'T_x', 'T_y', 'T_z'])
+    y = pd.Series(id_to_target)
+
+    return df, y
```

### Comparing `tsfresh-0.8.1/tsfresh/examples/test_tsfresh_baseline_dataset.py` & `tsfresh-0.9.0/tsfresh/examples/test_tsfresh_baseline_dataset.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/feature_extraction/feature_calculators.py` & `tsfresh-0.9.0/tsfresh/feature_extraction/feature_calculators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1511 +1,1583 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-"""
-This module contains the feature calculators that take time series as input and calculate the values of the feature.
-There are three types of features:
-
-1. aggregate features without parameter
-2. aggregate features with parameter
-3. apply features with parameters
-
-While type 1 and 2 are designed to be used with pandas aggregate, they will only return one singular feature.
-To not unnecessarily redo auxiliary calculations, in type 3 a group of features is calculated at the same time. They
-can be used with pandas apply.
-"""
-
-from __future__ import absolute_import, division
-from builtins import range
-import itertools
-import numpy as np
-from numpy.linalg import LinAlgError
-import numbers
-from functools import wraps
-
-import pandas as pd
-from scipy.signal import welch, cwt, ricker, find_peaks_cwt
-from scipy.stats import linregress
-from statsmodels.tsa.ar_model import AR
-from statsmodels.tsa.stattools import adfuller
-from scipy.stats import linregress
-
-# todo: make sure '_' works in parameter names in all cases, add a warning if not
-
-def _get_length_sequences_where(x):
-    """
-    This method calculates the length of all sub-sequences where the array x is either True or 1.
-
-    Examples
-    --------
-    >>> x = [0,1,0,0,1,1,1,0,0,1,0,1,1]
-    >>> _get_length_sequences_where(x)
-    >>> [1, 3, 1, 2]
-
-    >>> x = [0,True,0,0,True,True,True,0,0,True,0,True,True]
-    >>> _get_length_sequences_where(x)
-    >>> [1, 3, 1, 2]
-
-    >>> x = [0,True,0,0,1,True,1,0,0,True,0,1,True]
-    >>> _get_length_sequences_where(x)
-    >>> [1, 3, 1, 2]
-
-    :param x: An iterable containing only 1, True, 0 and False values
-    :return: A list with the length of all sub-sequences where the array is either True or False. If no ones or Trues
-    contained, the list [0] is returned.
-    """
-    if len(x) == 0:
-        return [0]
-    else:
-        res = [len(list(group)) for value, group in itertools.groupby(x) if value == 1]
-        return res if len(res) > 0 else [0]
-
-
-def not_apply_to_raw_numbers(func):
-    """
-    This decorator makes sure that the function func is only called on objects that are not numbers.Number
-
-    :param func: the method that should only be executed on objects which are not a numbers.Number
-    :return: the decorated version of func which returns 0 if the first argument x is a numbers.Number. For every
-                other x the output of func is returned
-    """
-
-    @wraps(func)
-    def func_on_nonNumberObject(x, *arg, **args):
-        if isinstance(x, numbers.Number):
-            return 0
-        else:
-            return func(x, *arg, **args)
-    return func_on_nonNumberObject
-
-
-def set_property(key, value):
-    """
-    This method returns a decorator that sets the property key of the function to value
-    """
-    def decorate_func(func):
-        setattr(func, key, value)
-        if func.__doc__ and key == "fctype":
-            func.__doc__ = func.__doc__ + "\n\n    *This function is of type: " + value + "*\n"
-        return func
-    return decorate_func
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def variance_larger_than_standard_deviation(x):
-    """
-    Boolean variable denoting if the variance of x is greater than its standard deviation. Is equal to variance of x
-    being larger than 1
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: bool
-    """
-    return np.var(x) > np.std(x)
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def large_standard_deviation(x, r):
-    """
-    Boolean variable denoting if the standard dev of x is higher
-    than 'r' times the range = difference between max and min of x.
-    Hence it checks if
-
-    .. math::
-
-        std(x) > r * (max(X)-min(X))
-
-    According to a rule of the thumb, the standard deviation should be a forth of the range of the values.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param r: the percentage of the range to compare with
-    :type r: float
-    :return: the value of this feature
-    :return type: bool
-    """
-    x = np.asarray(x)
-    return np.std(x) > (r * (max(x) - min(x)))
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def symmetry_looking(x, c, param):
-    """
-    Boolean variable denoting if the distribution of x *looks symmetric*. This is the case if
-
-    .. math::
-
-        | mean(X)-median(X)| < r * (max(X)-min(X))
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param r: the percentage of the range to compare with
-    :type r: float
-    :return: the value of this feature
-    :return type: bool
-    """
-    x = np.asarray(x)
-    mean_median_difference = abs(np.mean(x) - np.median(x))
-    max_min_difference = max(x) - min(x)
-    return pd.Series({"{}__symmetry_looking__r_{}".format(c, r["r"]):
-                          mean_median_difference < (r["r"] * max_min_difference) for r in param})
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def has_duplicate_max(x):
-    """
-    Checks if the maximum value of x is observed more than once
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: bool
-    """
-    return sum(np.asarray(x) == max(x)) >= 2
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def has_duplicate_min(x):
-    """
-    Checks if the minimal value of x is observed more than once
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: bool
-    """
-    return sum(np.asarray(x) == min(x)) >= 2
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def has_duplicate(x):
-    """
-    Checks if any value in x occurs more than once
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: bool
-    """
-    return len(x) != len(set(x))
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-def sum_values(x):
-    """
-    Calculates the sum over the time series values
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: bool
-    """
-    return np.sum(x)
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def large_number_of_peaks(x, n):
-    """
-    Checks if the number of peaks is higher than n.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param n: the number of peaks to compare
-    :type n: int
-    :return: the value of this feature
-    :return type: bool
-    """
-    return number_peaks(x, n=n) > 5
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def mean_autocorrelation(x):
-    """
-    Calculates the average autocorrelation (Compare to http://en.wikipedia.org/wiki/Autocorrelation#Estimation),
-    taken over different all possible lags (1 to length of x)
-
-    .. math::
-
-        \\frac{1}{n} \\sum_{l=1,\ldots, n} \\frac{1}{(n-l)\sigma^{2}} \\sum_{t=1}^{n-l}(X_{t}-\\mu )(X_{t+l}-\\mu)
-
-    where :math:`n` is the length of the time series :math:`X_i`, :math:`\sigma^2` its variance and :math:`\mu` its
-    mean.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    var = np.var(x)
-    n = len(x)
-
-    if abs(var) < 10**-10 or n == 1:
-        return 0
-    else:
-        r = np.correlate(x - np.mean(x), x - np.mean(x), mode='full')
-        r = r[0: (n - 1)] / np.arange(n - 1, 0, -1)
-        return np.nanmean(r / var)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def augmented_dickey_fuller(x):
-    """
-    The Augmented Dickey-Fuller test is a hypothesis test which checks whether a unit root is present in a time
-    series sample. This feature calculator returns the value of the respective test statistic.
-
-    See the statsmodels implementation for references and more details.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    try:
-        return adfuller(x)[0]
-    except LinAlgError:
-        return np.NaN
-    except ValueError:  # occurs if sample size is too small
-        return np.NaN
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def abs_energy(x):
-    """
-    Returns the absolute energy of the time series which is the sum over the squared values
-
-    .. math::
-
-        E = \\sum_{i=1,\ldots, n} x_i^2
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = np.asarray(x)
-    return sum(x * x)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def mean_abs_change(x):
-    """
-    Returns the mean over the absolute differences between subsequent time series values which is
-
-    .. math::
-
-        \\frac{1}{n} \\sum_{i=1,\ldots, n-1} | x_{i+1} - x_{i}|
-
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return np.mean(abs(np.diff(x)))
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def mean_change(x):
-    """
-    Returns the mean over the absolute differences between subsequent time series values which is
-
-    .. math::
-
-        \\frac{1}{n} \\sum_{i=1,\ldots, n-1}  x_{i+1} - x_{i}
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return np.mean(np.diff(x))
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def mean_second_derivate_central(x):
-    """
-    Returns the mean value of a central approximation of the second derivative
-
-    .. math::
-
-        \\frac{1}{n} \\sum_{i=1,\ldots, n-1}  \\frac{1}{2} (x_{i+2} - 2 \\cdot x_{i+1} + x_i)
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    diff = (np.roll(x, 1) - 2 * np.array(x) + np.roll(x, -1)) / 2.0
-    return np.mean(diff[1:-1])
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-def median(x):
-    """
-    Returns the median of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return np.median(x)
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-def mean(x):
-    """
-    Returns the mean of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return np.mean(x)
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-@not_apply_to_raw_numbers
-def length(x):
-    """
-    Returns the length of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: int
-    """
-    return len(x)
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-@not_apply_to_raw_numbers
-def standard_deviation(x):
-    """
-    Returns the standard deviation of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return np.std(x)
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-@not_apply_to_raw_numbers
-def variance(x):
-    """
-    Returns the variance of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return np.var(x)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def skewness(x):
-    """
-    Returns the sample skewness of x (calculated with the adjusted Fisher-Pearson standardized
-    moment coefficient G1).
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = pd.Series(x)
-    return pd.Series.skew(x)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def kurtosis(x):
-    """
-    Returns the kurtosis of x (calculated with the adjusted Fisher-Pearson standardized
-    moment coefficient G2).
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = pd.Series(x)
-    return pd.Series.kurtosis(x)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def absolute_sum_of_changes(x):
-    """
-    Returns the sum over the absolute value of consecutive changes in the series x
-
-    .. math::
-
-        \\sum_{i=1, \ldots, n-1} \\mid x_{i+1}- x_i \\mid
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return np.sum(abs(np.diff(x)))
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def longest_strike_below_mean(x):
-    """
-    Returns the length of the longest consecutive subsequence in x that is smaller than the mean of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    return max(_get_length_sequences_where(x <= np.mean(x))) if len(x) > 0 else 0
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def longest_strike_above_mean(x):
-    """
-    Returns the length of the longest consecutive subsequence in x that is bigger than the mean of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    return max(_get_length_sequences_where(x >= np.mean(x))) if len(x) > 0 else 0
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def count_above_mean(x):
-    """
-    Returns the number of values in x that are higher than the mean of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    x = np.asarray(x)
-    m = np.mean(x)
-    return np.where(x > m)[0].shape[0]
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def count_below_mean(x):
-    """
-    Returns the number of values in x that are lower than the mean of x
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    x = np.asarray(x)
-    m = np.mean(x)
-    return np.where(x < m)[0].shape[0]
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def last_location_of_maximum(x):
-    """
-    Returns the relative last location of the maximum value of x.
-    The position is calculated relatively to the length of x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = np.asarray(x)
-    return 1.0 - np.argmax(x[::-1]) / len(x) if len(x) > 0 else np.NaN
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def first_location_of_maximum(x):
-    """
-    Returns the first location of the maximum value of x.
-    The position is calculated relatively to the length of x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = np.asarray(x)
-    return np.argmax(x) / len(x) if len(x) > 0 else np.NaN
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def last_location_of_minimum(x):
-    """
-    Returns the last location of the minimal value of x.
-    The position is calculated relatively to the length of x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = np.asarray(x)
-    return 1.0 - np.argmin(x[::-1]) / len(x) if len(x) > 0 else np.NaN
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def first_location_of_minimum(x):
-    """
-    Returns the first location of the minimal value of x.
-    The position is calculated relatively to the length of x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = np.asarray(x)
-    return np.argmin(x) / len(x) if len(x) > 0 else np.NaN
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def percentage_of_reoccurring_datapoints_to_all_datapoints(x):
-    """
-    Returns the percentage of unique values, that are present in the time series
-    more than once.
-
-        len(different values occurring more than once) / len(different values)
-
-    This means the percentage is normalized to the number of unique values,
-    in contrast to the percentage_of_reoccurring_values_to_all_values.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    unique, counts = np.unique(x, return_counts=True)
-    return np.sum(counts > 1) / float(counts.shape[0])
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def percentage_of_reoccurring_values_to_all_values(x):
-    """
-    Returns the ratio of unique values, that are present in the time series
-    more than once.
-
-        # of data points occurring more than once / # of all data points
-
-    This means the ratio is normalized to the number of data points in the time series,
-    in contrast to the percentage_of_reoccurring_datapoints_to_all_datapoints.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    x = pd.Series(x)
-
-    if len(x) == 0:
-        return np.nan
-
-    value_counts = x.value_counts()
-    return value_counts[value_counts > 1].sum() / len(x)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def sum_of_reoccurring_values(x):
-    """
-    Returns the sum of all values, that are present in the time series
-    more than once.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    unique, counts = np.unique(x, return_counts=True)
-    counts[counts < 2] = 0
-    counts[counts > 1] = 1
-    return np.sum(counts * unique)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def sum_of_reoccurring_data_points(x):
-    """
-    Returns the sum of all data points, that are present in the time series
-    more than once.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    unique, counts = np.unique(x, return_counts=True)
-    counts[counts < 2] = 0
-    return np.sum(counts * unique)
-
-
-@set_property("fctype", "aggregate")
-@not_apply_to_raw_numbers
-def ratio_value_number_to_time_series_length(x):
-    """
-    Returns a factor which is 1 if all values in the time series occur only once,
-    and below one if this is not the case.
-    In principle, it just returns
-
-        # unique values / # values
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-
-    if len(x) == 0:
-        return np.nan
-
-    return len(set(x))/len(x)
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def fft_coefficient(x, c, param):
-    """
-    Calculates the fourier coefficients of the one-dimensional discrete Fourier Transform for real input by fast
-    fourier transformation algorithm
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"coeff": x} with x int and x >= 0
-    :type param: list
-    :return: the different feature values
-    :return type: pandas.Series
-    """
-
-    coefficients = set([config["coeff"] for config in param])
-    for coeff in coefficients:
-        if coeff < 0:
-            raise ValueError("Coefficients must be positive or zero.")
-
-    maximum_coefficient = max(max(coefficients), 1)
-    fft = np.fft.rfft(x, min(len(x), 2 * maximum_coefficient))
-
-    res = [fft[q] if q < len(fft) else 0 for q in coefficients]
-    res = [r.real if isinstance(r, complex) else r for r in res]
-    return pd.Series(res, index=["{}__fft_coefficient__coeff_{}".format(c, q) for q in coefficients])
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def number_peaks(x, n):
-    """
-    Calculates the number of peaks of at least support n in the time series x. A peak of support n is defined as a
-    subsequence of x where a value occurs, which is bigger than its n neighbours to the left and to the right.
-
-    Hence in the sequence
-
-    >>> x = [3, 0, 0, 4, 0, 0, 13]
-
-    4 is a peak of support 1 and 2 because in the subsequences
-
-    >>> [0, 4, 0]
-    >>> [0, 0, 4, 0, 0]
-
-    4 is still the highest value. Here, 4 is not a peak of support 3 because 13 is the 3th neighbour to the right of 4
-    and its bigger than 4.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param n: the support of the peak
-    :type n: int
-    :return: the value of this feature
-    :return type: float
-    """
-    x = np.asarray(x)
-    x_reduced = x[n:-n]
-
-    res = None
-    for i in range(1, n + 1):
-        result_first = (x_reduced > np.roll(x, i)[n:-n])
-
-        if res is None:
-            res = result_first
-        else:
-            res &= result_first
-
-        res &= (x_reduced > np.roll(x, -i)[n:-n])
-    return sum(res)
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def index_mass_quantile(x, c, param):
-    """
-    Those apply features calculate the relative index i where q% of the mass of the time series x lie left of i.
-    For example for q = 50% this feature calculator will return the mass center of the time series
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"q": x} with x float
-    :type param: list
-    :return: the different feature values
-    :return type: pandas.Series
-    """
-
-    x = np.asarray(x)
-    abs_x = np.abs(x)
-    s = sum(abs_x)
-
-    res = {}
-
-    if s == 0:
-        # all values in x are zero or it has length 0
-        for config in param:
-            res["{}__index_mass_quantile__q_{}".format(c, config["q"])] = np.NaN
-    else:
-        # at least one value is not zero
-        mass_centralized = np.cumsum(abs_x) / s
-        for config in param:
-            res["{}__index_mass_quantile__q_{}".format(c, config["q"])] = \
-                (np.argmax(mass_centralized >= config["q"])+1)/len(x)
-    return pd.Series(res)
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def number_cwt_peaks(x, n):
-    """
-    This feature calculator searches for different peaks in x. To do so, x is smoothed by a ricker wavelet and for
-    widths ranging from 1 to n. This feature calculator returns the number of peaks that occur at enough width scales
-    and with sufficiently high Signal-to-Noise-Ratio (SNR)
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param n: maximum width to consider
-    :type n: int
-    :return: the value of this feature
-    :return type: int
-    """
-    return len(find_peaks_cwt(vector=x, widths=np.array(list(range(1, n + 1))), wavelet=ricker))
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def linear_trend(x, c, param):
-    """
-    Calculate a linear least-squares regression for the values of the time series versus the sequence from 0 to
-    length of the time series minus one.
-    This feature assumes the signal to be uniformly sampled. It will not use the time stamps to fit the model.
-    The parameters control which of the characteristics are returned.
-
-    Possible extracted attributes are "pvalue", "rvalue", "intercept", "slope", "stderr", see the documentation of
-    linregress for more information.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"attr": x} with x an string, the attribute name of the regression model
-    :type param: list
-    :return: the different feature values
-    :return type: pandas.Series
-    """
-    # todo: we could use the index of the DataFrame here
-
-    linReg = linregress(range(len(x)), x)
-
-    return pd.Series(data=[getattr(linReg, config["attr"]) for config in param],
-                     index=["{}__linear_trend__attr_\"{}\"".format(c, config["attr"]) for config in param])
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def cwt_coefficients(x, c, param):
-    """
-    Calculates a Continuous wavelet transform for the Ricker wavelet, also known as the "Mexican hat wavelet" which is
-    defined by
-
-    .. math::
-        \\frac{2}{\\sqrt{3a} \\pi^{\\frac{1}{4}}} (1 - \\frac{x^2}{a^2}) exp(-\\frac{x^2}{2a^2})
-
-    where :math:`a` is the width parameter of the wavelet function.
-
-    This feature calculator takes three different parameter: widths, coeff and w. The feature calculater takes all the
-    different widths arrays and then calculates the cwt one time for each different width array. Then the values for the
-    different coefficient for coeff and width w are returned. (For each dic in param one feature is returned)
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"widths":x, "coeff": y, "w": z} with x array of int and y,z int
-    :type param: list
-    :return: the different feature values
-    :return type: pandas.Series
-    """
-
-    calculated_cwt = {}
-    res = []
-    indices = []
-
-    for parameter_combination in param:
-        widths = parameter_combination["widths"]
-        w = parameter_combination["w"]
-        coeff = parameter_combination["coeff"]
-
-        if widths not in calculated_cwt:
-            calculated_cwt[widths] = cwt(x, ricker, widths)
-
-        calculated_cwt_for_widths = calculated_cwt[widths]
-
-        indices += ["{}__cwt_coefficients__widths_{}__coeff_{}__w_{}".format(c, widths, coeff, w)]
-
-        i = widths.index(w)
-        if calculated_cwt_for_widths.shape[1] <= coeff:
-            res += [np.NaN]
-        else:
-            res += [calculated_cwt_for_widths[i, coeff]]
-
-    return pd.Series(res, index=indices)
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def spkt_welch_density(x, c, param):
-    """
-    This feature calculator estimates the cross power spectral density of the time series x at different frequencies.
-    To do so, the time series is first shifted from the time domain to the frequency domain.
-
-    The feature calculators returns the power spectrum of the different frequencies.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"coeff": x} with x int
-    :type param: list
-    :return: the different feature values
-    :return type: pandas.Series
-    """
-
-    freq, pxx = welch(x)
-    coeff = [config["coeff"] for config in param]
-
-    if len(pxx) <= max(coeff):  # There are fewer data points in the time series than requested coefficients
-
-        # filter coefficients that are not contained in pxx
-        reduced_coeff = [coefficient for coefficient in coeff if len(pxx) > coefficient]
-        not_calculated_coefficients = [coefficient for coefficient in coeff
-                                       if coefficient not in reduced_coeff]
-
-        # Fill up the rest of the requested coefficients with np.NaNs
-        return pd.Series(list(pxx[reduced_coeff]) + [np.NaN] * len(not_calculated_coefficients),
-                         index=["{}__spkt_welch_density__coeff_{}".format(c, i) for i in coeff])
-    else:
-        return pd.Series(pxx[coeff], index=["{}__spkt_welch_density__coeff_{}".format(c, i) for i in coeff])
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def ar_coefficient(x, c, param):
-    """
-    This feature calculator fits the unconditional maximum likelihood
-    of an autoregressive AR(k) process.
-    The k parameter is the maximum lag of the process
-
-    .. math::
-
-        X_{t}=\\varphi_0 +\\sum _{{i=1}}^{k}\\varphi_{i}X_{{t-i}}+\\varepsilon_{t}
-
-    For the configurations from param which should contain the maxlag "k" and such an AR process is calculated. Then
-    the coefficients :math:`\\varphi_{i}` whose index :math:`i` contained from "coeff" are returned.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"coeff": x, "k": y} with x,y int
-    :type param: list
-    :return x: the different feature values
-    :return type: pandas.Series
-    """
-    calculated_ar_params = {}
-
-    x_as_list = list(x)
-    calculated_AR = AR(x_as_list)
-
-    res = {}
-
-    for parameter_combination in param:
-        k = parameter_combination["k"]
-        p = parameter_combination["coeff"]
-
-        column_name = "{}__ar_coefficient__k_{}__coeff_{}".format(c, k, p)
-
-        if k not in calculated_ar_params:
-            try:
-                calculated_ar_params[k] = calculated_AR.fit(maxlag=k, solver="mle").params
-            except (LinAlgError, ValueError):
-                calculated_ar_params[k] = [np.NaN]*k
-
-        mod = calculated_ar_params[k]
-
-        if p <= k:
-            try:
-                res[column_name] = mod[p]
-            except IndexError:
-                res[column_name] = 0
-        else:
-            res[column_name] = np.NaN
-
-    return pd.Series(res)
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def mean_abs_change_quantiles(x, ql, qh):
-    """
-    First fixes a corridor given by the quantiles ql and qh of the distribution of x. Then calculates the average
-    absolute value of consecutive changes of the series x inside this corridor. Think about selecting a corridor on the
-    y-Axis and only calculating the mean of the absolute change of the time series inside this corridor.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param ql: the lower quantile of the corridor
-    :type ql: float
-    :param qh: the higher quantile of the corridor
-    :type qh: float
-    :return: the value of this feature
-    :return type: float
-    """
-    x = np.asarray(x)
-
-    if ql >= qh:
-        ValueError("ql={} should be lower than qh={}".format(ql, qh))
-    div = np.abs(np.diff(x))
-    # All values that originate from the corridor between the quantiles ql and qh will have the category 0,
-    # other will be np.NaN
-    try:
-        bin_cat = pd.qcut(x, [ql, qh], labels=False)
-        bin_cat_0 = bin_cat == 0
-    except ValueError:  # Occurs when ql are qh effectively equal, e.g. x is not long enough or is too categorical
-        return 0
-    # We only count changes that start and end inside the corridor
-    ind = (bin_cat_0 * np.roll(bin_cat_0, 1))[1:]
-    if sum(ind) == 0:
-        return 0
-    else:
-        ind_inside_corridor = np.where(ind == 1)
-        return np.mean(div[ind_inside_corridor])
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def time_reversal_asymmetry_statistic(x, lag):
-    """
-    This function calculates the value of
-
-    .. math::
-
-        \\frac{1}{n-2lag} \sum_{i=0}^{n-2lag} x_{i + 2 \cdot lag}^2 \cdot x_{i + lag} - x_{i + lag} \cdot  x_{i}^2
-
-    which is
-
-    .. math::
-
-        \\mathbb{E}[L^2(X)^2 \cdot L(X) - L(X) \cdot X^2]
-
-    where :math:`\\mathbb{E}` is the mean and :math:`L` is the lag operator. It was proposed in [1] as a
-    promising feature to extract from time series.
-
-    References
-    ----------
-
-    .. [1] Fulcher, B.D., Jones, N.S. (2014).
-       Highly comparative feature-based time-series classification.
-       Knowledge and Data Engineering, IEEE Transactions on 26, 3026–3037.
-
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param lag: the lag that should be used in the calculation of the feature
-    :type lag: int
-    :return: the value of this feature
-    :return type: float
-    """
-    n = len(x)
-    x = np.asarray(x)
-    if 2 * lag > n:
-        return 0
-    elif 2 * lag == n:
-        return x[n-1] * x[n-1] * x[0] - x[lag-1] * x[0] * x[0]
-    else:
-        return np.mean((np.roll(x, 2 * -lag) * np.roll(x, 2 * -lag) * x - np.roll(x, -lag) * x * x)[0:(n - 2 * lag)])
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def binned_entropy(x, max_bins):
-    """
-    First bins the values of x into max_bins equidistant bins.
-    Then calculates the value of
-
-    .. math::
-
-        - \\sum_{k=0}^{min(max\\_bins, len(x))} p_k log(p_k) \\cdot \\mathbf{1}_{(p_k > 0)}
-
-    where :math:`p_k` is the percentage of samples in bin :math:`k`.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param max_bins: the maximal number of bins
-    :type max_bins: int
-    :return: the value of this feature
-    :return type: float
-    """
-    hist, bin_edges = np.histogram(x, bins=max_bins)
-    probs = hist / len(x)
-    return - np.sum(p * np.math.log(p) for p in probs if p != 0)
-
-# todo - include latex formula
-# todo - check if vectorizable
-@set_property("high_comp_cost", True)
-@set_property("fctype", "aggregate")
-def sample_entropy(x):
-    """
-    Calculate and return sample entropy of x.
-    References:
-    ----------
-    [1] http://en.wikipedia.org/wiki/Sample_Entropy
-    [2] https://www.ncbi.nlm.nih.gov/pubmed/10843903?dopt=Abstract
-    
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param tolerance: normalization factor; equivalent to the common practice of expressing the tolerance as r times the standard deviation
-    :type tolerance: float
-    :return: the value of this feature
-    :return type: float
-    """ 
-    x = np.array(x)
-    
-    sample_length = 1 # number of sequential points of the time series
-    tolerance = 0.2 * np.std(x) # 0.2 is a common value for r - why?
-
-    n = len(x)
-    prev = np.zeros(n)
-    curr = np.zeros(n)
-    A = np.zeros((1, 1))  # number of matches for m = [1,...,template_length - 1]
-    B = np.zeros((1, 1))  # number of matches for m = [1,...,template_length]
-
-    for i in range(n - 1):
-        nj = n - i - 1
-        ts1 = x[i]
-        for jj in range(nj):
-            j = jj + i + 1
-            if abs(x[j] - ts1) < tolerance:  # distance between two vectors
-                curr[jj] = prev[jj] + 1
-                temp_ts_length = min(sample_length, curr[jj])
-                for m in range(int(temp_ts_length)):
-                    A[m] += 1
-                    if j < n - 1:
-                        B[m] += 1
-            else:
-                curr[jj] = 0
-        for j in range(nj):
-            prev[j] = curr[j]
-            
-    N = n * (n - 1) / 2
-    B = np.vstack(([N], B[0]))
-    
-    # sample entropy = -1 * (log (A/B))
-    similarity_ratio = A / B 
-    se = -1 * np.log(similarity_ratio)
-    se = np.reshape(se, -1)
-    return se[0]
-    
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def autocorrelation(x, lag):
-    """
-    Calculates the lag autocorrelation of a lag value of lag.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param lag: the lag
-    :type lag: int
-    :return: the value of this feature
-    :return type: float
-    """
-    x = pd.Series(x)
-    return pd.Series.autocorr(x, lag)
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@not_apply_to_raw_numbers
-def quantile(x, q):
-    """
-    Calculates the q quantile of x. This is the value of x greater than q% of the ordered values from x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param q: the quantile to calculate
-    :type q: float
-    :return: the value of this feature
-    :return type: float
-    """
-    x = pd.Series(x)
-    return pd.Series.quantile(x, q)
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-def maximum(x):
-    """
-    Calculates the highest value of the time series x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return max(x)
-
-
-@set_property("fctype", "aggregate")
-@set_property("minimal", True)
-def minimum(x):
-    """
-    Calculates the lowest value of the time series x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :return: the value of this feature
-    :return type: float
-    """
-    return min(x)
-
-
-@set_property("fctype", "aggregate_with_parameters")
-def value_count(x, value):
-    """
-    Count occurrences of `value` in time series x.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param value: the value to be counted
-    :type value: int or float
-    :return: the count
-    :rtype: int
-    """
-
-    if np.isnan(value):
-        return x.isnull().sum()
-    else:
-        return x[x == value].count()
-
-
-@set_property("fctype", "aggregate_with_parameters")
-def range_count(x, min, max):
-    """
-    Count observed values within the interval [min, max).
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param min: the inclusive lower bound of the range
-    :type min: int or float
-    :param max: the exclusive upper bound of the range
-    :type max: int or float
-    :return: the count of values within the range
-    :rtype: int
-    """
-
-    return x[(x >= min) & (x < max)].count()
-
-
-@set_property("fctype", "aggregate_with_parameters")
-@set_property("high_comp_cost", True)
-def approximate_entropy(x, m, r):
-    """
-    Implements a vectorized Approximate entropy algorithm.
-
-        https://en.wikipedia.org/wiki/Approximate_entropy
-
-    For short time-series this method is highly dependent on the parameters,
-    but should be stable for N > 2000, see:
-
-        Yentes et al. (2012) - 
-        *The Appropriate Use of Approximate Entropy and Sample Entropy with Short Data Sets*
-
-
-    Other shortcomings and alternatives discussed in:
-
-        Richman & Moorman (2000) -
-        *Physiological time-series analysis using approximate entropy and sample entropy*
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param m: Length of compared run of data
-    :type m: int
-    :param r: Filtering level, must be positive
-    :type r: float
-
-    :return: Approximate entropy
-    :return type: float
-    """
-    x = np.asarray(x)
-    N = len(x)
-    r *= np.std(x)
-    if r < 0:
-        raise ValueError("Parameter r must be positive.")
-    if N <= m+1:
-        return 0
-
-    def _phi(m):
-        x_re = np.array([x[i:i+m] for i in range(N - m + 1)])
-        C = np.sum(np.max(np.abs(x_re[:, np.newaxis] - x_re[np.newaxis, :]),
-                          axis=2) <= r, axis=0) / (N-m+1)
-        return np.sum(np.log(C)) / (N - m + 1.0)
-
-    return np.abs(_phi(m) - _phi(m + 1))
-
-def _estimate_friedrich_coefficients(x, m, r):
-    """
-    Coefficients of polynomial :math:`h(x)`, which has been fitted to 
-    the deterministic dynamics of Langevin model 
-    .. math::
-        \dot{x}(t) = h(x(t)) + \mathcal{N}(0,R)
-
-    As described by
-
-        Friedrich et al. (2000): Physics Letters A 271, p. 217-222
-        *Extracting model equations from experimental data*
-
-    For short time-series this method is highly dependent on the parameters.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param m: order of polynom to fit for estimating fixed points of dynamics
-    :type m: int
-    :param r: number of quantils to use for averaging
-    :type r: float
-
-    :return: coefficients of polynomial of deterministic dynamics
-    :return type: ndarray
-    """
-    df = pd.DataFrame({'signal': x[:-1], 'delta': np.diff(x)})
-    try:
-        df['quantiles'] = pd.qcut(df.signal, r)
-        binned = True
-    except ValueError:
-        binned = False
-        coeff = [np.NaN] * (m+1)
-
-    if binned:
-        quantiles = df.groupby('quantiles')
-        
-        result = pd.DataFrame({'x_mean': quantiles.signal.mean(),
-                               'y_mean': quantiles.delta.mean()
-        })
-
-        result.dropna(inplace=True)
-
-        try:
-            coeff = np.polyfit(result.x_mean, result.y_mean, deg=m)
-        except (np.linalg.LinAlgError, ValueError):
-            coeff = [np.NaN] * (m+1)
-    return coeff
-
-@set_property("fctype", "apply")
-def friedrich_coefficients(x, c, param):
-    """
-    Coefficients of polynomial :math:`h(x)`, which has been fitted to 
-    the deterministic dynamics of Langevin model 
-    .. math::
-        \dot{x}(t) = h(x(t)) + \mathcal{N}(0,R)
-
-    as described by
-
-        Friedrich et al. (2000): Physics Letters A 271, p. 217-222
-        *Extracting model equations from experimental data*
-
-
-    For short time-series this method is highly dependent on the parameters.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"coeff": x} with x int and x >= 0
-    :type param: list
-    :return: the different feature values
-    :return type: pandas.Series
-    """
-    coefficients = set([config["coeff"] for config in param])
-    for coeff in coefficients:
-        if coeff < 0:
-            raise ValueError("Coefficients must be positive or zero.")
-
-    m = param[0]['m']
-    r = param[0]['r']
-
-    coeff = _estimate_friedrich_coefficients(x, m, r)
-
-    name = lambda q: "{}__friedrich_coefficients__m_{}__r_{}__coeff_{}".format(c,m,r,q)
-    return pd.Series(coeff, index=[name(q) for q in range(m,-1,-1)])
-
-@set_property("fctype", "aggregate_with_parameters")
-def max_langevin_fixed_point(x, r, m):
-    """
-    Largest fixed point of dynamics  :math:argmax_x {h(x)=0}` estimated from polynomial :math:`h(x)`, 
-    which has been fitted to the deterministic dynamics of Langevin model
-    .. math::
-        \dot(x)(t) = h(x(t)) + R \mathcal(N)(0,1)
-
-    as described by
-
-        Friedrich et al. (2000): Physics Letters A 271, p. 217-222
-        *Extracting model equations from experimental data*
-
-    For short time-series this method is highly dependent on the parameters.
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param m: order of polynom to fit for estimating fixed points of dynamics
-    :type m: int
-    :param r: number of quantils to use for averaging
-    :type r: float
-
-    :return: Largest fixed point of deterministic dynamics
-    :return type: float
-    """
-
-    coeff = _estimate_friedrich_coefficients(x, m, r)
-
-    try:
-        max_fixed_point = np.max(np.real(np.roots(coeff)))
-    except (np.linalg.LinAlgError, ValueError):
-        return np.nan
-    
-    return max_fixed_point
-
-
-def _aggregate_on_chunks(x, f_agg, chunk_len):
-    """
-    Takes the time series x and constructs a lower sampled version of it by applying the aggregation function f_agg on
-    consecutive chunks of length chunk_len
-
-    :param x: the time series to calculate the aggregation of
-    :type x: pandas.Series
-    :param f_agg: The name of the aggregation function that should be an attribute of the pandas.Series
-    :type f_agg: str
-    :param chunk_len: The size of the chunks where to aggregate the time series
-    :type chunk_len: int
-    :return: A list of the aggregation function over the chunks
-    :return type: list
-    """
-    return [getattr(x[i * chunk_len: (i + 1) * chunk_len], f_agg)() for i in range(int(np.ceil(len(x) / chunk_len)))]
-
-
-@set_property("fctype", "apply")
-@not_apply_to_raw_numbers
-def agg_linear_trend(x, c, param):
-    """
-    Calculates a linear least-squares regression for values of the time series that were aggregated over chunks versus
-    the sequence from 0 up to the number of chunks minus one.
-
-    This feature assumes the signal to be uniformly sampled. It will not use the time stamps to fit the model.
-
-    The parameters attr controls which of the characteristics are returned. Possible extracted attributes are "pvalue",
-    "rvalue", "intercept", "slope", "stderr", see the documentation of linregress for more information.
-
-    The chunksize is regulated by "chunk_len". It specifies how many time series values are in each chunk.
-
-    Further, the aggregation function is controlled by "f_agg", which can use "max", "min" or , "mean", "median"
-
-    :param x: the time series to calculate the feature of
-    :type x: pandas.Series
-    :param c: the time series name
-    :type c: str
-    :param param: contains dictionaries {"attr": x, "chunk_len": l, "f_agg": f} with x, f an string and l an int
-    :type param: list
-    :return: the different feature values
-    :return type: pandas.Series
-    """
-    # todo: we could use the index of the DataFrame here
-
-    calculated_agg = {}
-    res_data = []
-    res_index = []
-
-    for parameter_combination in param:
-
-        chunk_len = parameter_combination["chunk_len"]
-        f_agg = parameter_combination["f_agg"]
-
-        aggregate_result = _aggregate_on_chunks(x, f_agg, chunk_len)
-        if f_agg not in calculated_agg or chunk_len not in calculated_agg[f_agg]:
-            if chunk_len >= len(x):
-                calculated_agg[f_agg] = {chunk_len: np.NaN}
-            else:
-                lin_reg_result = linregress(range(len(aggregate_result)), aggregate_result)
-                calculated_agg[f_agg] = {chunk_len: lin_reg_result}
-
-        attr = parameter_combination["attr"]
-
-        if chunk_len >= len(x):
-            res_data.append(np.NaN)
-        else:
-            res_data.append(getattr(calculated_agg[f_agg][chunk_len], attr))
-
-        res_index.append("{}__agg_linear_trend__f_agg_\"{}\"__chunk_len_{}__attr_\"{}\"".format(c, f_agg, chunk_len, attr))
-
-    return pd.Series(data=res_data, index=res_index)
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+"""
+This module contains the feature calculators that take time series as input and calculate the values of the feature.
+There are two types of features:
+
+1. feature calculators which calculate a single number (simple)
+2. feature calculators which calculate a bunch of features for a list of parameters at once,
+   to use e.g. cached results (combiner). They return a list of (key, value) pairs for each input parameter.
+
+They are specified using the "fctype" parameter of each feature calculator, which is added using the
+set_property function. Only functions in this python module, which have a parameter called  "fctype" are
+seen by tsfresh as a feature calculator. Others will not be calculated.
+"""
+
+from __future__ import absolute_import, division
+from builtins import range
+import itertools
+import numpy as np
+from numpy.linalg import LinAlgError
+
+import pandas as pd
+from scipy.signal import welch, cwt, ricker, find_peaks_cwt
+from statsmodels.tsa.ar_model import AR
+from statsmodels.tsa.stattools import adfuller
+from statsmodels.tsa.stattools import acf
+from scipy.stats import linregress
+
+# todo: make sure '_' works in parameter names in all cases, add a warning if not
+
+
+def _get_length_sequences_where(x):
+    """
+    This method calculates the length of all sub-sequences where the array x is either True or 1.
+
+    Examples
+    --------
+    >>> x = [0,1,0,0,1,1,1,0,0,1,0,1,1]
+    >>> _get_length_sequences_where(x)
+    >>> [1, 3, 1, 2]
+
+    >>> x = [0,True,0,0,True,True,True,0,0,True,0,True,True]
+    >>> _get_length_sequences_where(x)
+    >>> [1, 3, 1, 2]
+
+    >>> x = [0,True,0,0,1,True,1,0,0,True,0,1,True]
+    >>> _get_length_sequences_where(x)
+    >>> [1, 3, 1, 2]
+
+    :param x: An iterable containing only 1, True, 0 and False values
+    :return: A list with the length of all sub-sequences where the array is either True or False. If no ones or Trues
+    contained, the list [0] is returned.
+    """
+    if len(x) == 0:
+        return [0]
+    else:
+        res = [len(list(group)) for value, group in itertools.groupby(x) if value == 1]
+        return res if len(res) > 0 else [0]
+
+
+def _estimate_friedrich_coefficients(x, m, r):
+    """
+    Coefficients of polynomial :math:`h(x)`, which has been fitted to
+    the deterministic dynamics of Langevin model
+    .. math::
+        \dot{x}(t) = h(x(t)) + \mathcal{N}(0,R)
+
+    As described by
+
+        Friedrich et al. (2000): Physics Letters A 271, p. 217-222
+        *Extracting model equations from experimental data*
+
+    For short time-series this method is highly dependent on the parameters.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param m: order of polynom to fit for estimating fixed points of dynamics
+    :type m: int
+    :param r: number of quantils to use for averaging
+    :type r: float
+
+    :return: coefficients of polynomial of deterministic dynamics
+    :return type: ndarray
+    """
+    df = pd.DataFrame({'signal': x[:-1], 'delta': np.diff(x)})
+    try:
+        df['quantiles'] = pd.qcut(df.signal, r)
+    except ValueError:
+        return [np.NaN] * (m + 1)
+
+    quantiles = df.groupby('quantiles')
+
+    result = pd.DataFrame({'x_mean': quantiles.signal.mean(),
+                           'y_mean': quantiles.delta.mean()
+                           })
+
+    result.dropna(inplace=True)
+
+    try:
+        return np.polyfit(result.x_mean, result.y_mean, deg=m)
+    except (np.linalg.LinAlgError, ValueError):
+        return [np.NaN] * (m + 1)
+
+
+def _aggregate_on_chunks(x, f_agg, chunk_len):
+    """
+    Takes the time series x and constructs a lower sampled version of it by applying the aggregation function f_agg on
+    consecutive chunks of length chunk_len
+
+    :param x: the time series to calculate the aggregation of
+    :type x: pandas.Series
+    :param f_agg: The name of the aggregation function that should be an attribute of the pandas.Series
+    :type f_agg: str
+    :param chunk_len: The size of the chunks where to aggregate the time series
+    :type chunk_len: int
+    :return: A list of the aggregation function over the chunks
+    :return type: list
+    """
+    return [getattr(x[i * chunk_len: (i + 1) * chunk_len], f_agg)() for i in range(int(np.ceil(len(x) / chunk_len)))]
+
+
+def set_property(key, value):
+    """
+    This method returns a decorator that sets the property key of the function to value
+    """
+    def decorate_func(func):
+        setattr(func, key, value)
+        if func.__doc__ and key == "fctype":
+            func.__doc__ = func.__doc__ + "\n\n    *This function is of type: " + value + "*\n"
+        return func
+    return decorate_func
+
+
+@set_property("fctype", "simple")
+def variance_larger_than_standard_deviation(x):
+    """
+    Boolean variable denoting if the variance of x is greater than its standard deviation. Is equal to variance of x
+    being larger than 1
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: bool
+    """
+    return np.var(x) > np.std(x)
+
+
+@set_property("fctype", "simple")
+def ratio_beyond_r_sigma(x, r):
+    """
+    Ratio of values that are more than r*std(x) (so r sigma) away from the mean of x.
+
+    :param x: the time series to calculate the feature of
+    :type x: iterable
+    :return: the value of this feature
+    :return type: bool
+    """
+    x = np.asarray(x)
+    return sum(abs(x - np.mean(x)) > r * np.std(x))/len(x)
+
+
+@set_property("fctype", "simple")
+def large_standard_deviation(x, r):
+    """
+    Boolean variable denoting if the standard dev of x is higher
+    than 'r' times the range = difference between max and min of x.
+    Hence it checks if
+
+    .. math::
+
+        std(x) > r * (max(X)-min(X))
+
+    According to a rule of the thumb, the standard deviation should be a forth of the range of the values.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param r: the percentage of the range to compare with
+    :type r: float
+    :return: the value of this feature
+    :return type: bool
+    """
+    x = np.asarray(x)
+    return np.std(x) > (r * (max(x) - min(x)))
+
+
+@set_property("fctype", "combiner")
+def symmetry_looking(x, param):
+    """
+    Boolean variable denoting if the distribution of x *looks symmetric*. This is the case if
+
+    .. math::
+
+        | mean(X)-median(X)| < r * (max(X)-min(X))
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param r: the percentage of the range to compare with
+    :type r: float
+    :return: the value of this feature
+    :return type: bool
+    """
+    x = np.asarray(x)
+    mean_median_difference = abs(np.mean(x) - np.median(x))
+    max_min_difference = max(x) - min(x)
+    return [("r_{}".format(r["r"]), mean_median_difference < (r["r"] * max_min_difference))
+            for r in param]
+
+
+@set_property("fctype", "simple")
+def has_duplicate_max(x):
+    """
+    Checks if the maximum value of x is observed more than once
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: bool
+    """
+    return sum(np.asarray(x) == max(x)) >= 2
+
+
+@set_property("fctype", "simple")
+def has_duplicate_min(x):
+    """
+    Checks if the minimal value of x is observed more than once
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: bool
+    """
+    return sum(np.asarray(x) == min(x)) >= 2
+
+
+@set_property("fctype", "simple")
+def has_duplicate(x):
+    """
+    Checks if any value in x occurs more than once
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: bool
+    """
+    return len(x) != len(set(x))
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def sum_values(x):
+    """
+    Calculates the sum over the time series values
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: bool
+    """
+    return np.sum(x)
+
+
+@set_property("fctype", "combiner")
+def agg_autocorrelation(x, param):
+    """
+    Calculates the value of an aggregation function f_agg (e.g. var or mean) of the autocorrelation
+    (Compare to http://en.wikipedia.org/wiki/Autocorrelation#Estimation), taken over different all possible lags
+    (1 to length of x)
+
+    .. math::
+
+        \\frac{1}{n-1} \\sum_{l=1,\ldots, n} \\frac{1}{(n-l)\sigma^{2}} \\sum_{t=1}^{n-l}(X_{t}-\\mu )(X_{t+l}-\\mu)
+
+    where :math:`n` is the length of the time series :math:`X_i`, :math:`\sigma^2` its variance and :math:`\mu` its
+    mean.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"attr": x} with x str, name of a numpy function (e.g. mean, var, std, median),
+                   the name of the aggregator function that is applied to the autocorrelations
+    :type param: list
+    :return: the value of this feature
+    :return type: float
+    """
+    var = np.var(x)
+    n = len(x)
+    if abs(var) < 10**-10 or n == 1:
+        a = 0
+    else:
+        a = acf(x, unbiased=True, fft=n > 1250)[1:]
+    return [("f_agg_\"{}\"".format(config["f_agg"]), getattr(np, config["f_agg"])(a)) for config in param]
+
+
+@set_property("fctype", "combiner")
+def augmented_dickey_fuller(x, param):
+    """
+    The Augmented Dickey-Fuller test is a hypothesis test which checks whether a unit root is present in a time
+    series sample. This feature calculator returns the value of the respective test statistic.
+
+    See the statsmodels implementation for references and more details.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"attr": x} with x str, either "teststat", "pvalue" or "usedlag"
+    :type param: list
+    :return: the value of this feature
+    :return type: float
+    """
+    res = None
+    try:
+        res = adfuller(x)
+    except LinAlgError:
+        res = np.NaN, np.NaN, np.NaN
+    except ValueError:  # occurs if sample size is too small
+        res = np.NaN, np.NaN, np.NaN
+
+    return [("attr_{}".format(config["attr"]),
+                  res[0] if config["attr"] == "teststat"
+             else res[1] if config["attr"] == "pvalue"
+             else res[2] if config["attr"] == "usedlag" else np.NaN)
+            for config in param]
+
+
+@set_property("fctype", "simple")
+def abs_energy(x):
+    """
+    Returns the absolute energy of the time series which is the sum over the squared values
+
+    .. math::
+
+        E = \\sum_{i=1,\ldots, n} x_i^2
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+    return sum(x * x)
+
+
+@set_property("fctype", "simple")
+def mean_abs_change(x):
+    """
+    Returns the mean over the absolute differences between subsequent time series values which is
+
+    .. math::
+
+        \\frac{1}{n} \\sum_{i=1,\ldots, n-1} | x_{i+1} - x_{i}|
+
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return np.mean(abs(np.diff(x)))
+
+
+@set_property("fctype", "simple")
+def mean_change(x):
+    """
+    Returns the mean over the absolute differences between subsequent time series values which is
+
+    .. math::
+
+        \\frac{1}{n} \\sum_{i=1,\ldots, n-1}  x_{i+1} - x_{i}
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return np.mean(np.diff(x))
+
+
+@set_property("fctype", "simple")
+def mean_second_derivate_central(x):
+    """
+    Returns the mean value of a central approximation of the second derivative
+
+    .. math::
+
+        \\frac{1}{n} \\sum_{i=1,\ldots, n-1}  \\frac{1}{2} (x_{i+2} - 2 \\cdot x_{i+1} + x_i)
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+
+    diff = (np.roll(x, 1) - 2 * np.array(x) + np.roll(x, -1)) / 2.0
+    return np.mean(diff[1:-1])
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def median(x):
+    """
+    Returns the median of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return np.median(x)
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def mean(x):
+    """
+    Returns the mean of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return np.mean(x)
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def length(x):
+    """
+    Returns the length of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: int
+    """
+    return len(x)
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def standard_deviation(x):
+    """
+    Returns the standard deviation of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return np.std(x)
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def variance(x):
+    """
+    Returns the variance of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return np.var(x)
+
+
+@set_property("fctype", "simple")
+def skewness(x):
+    """
+    Returns the sample skewness of x (calculated with the adjusted Fisher-Pearson standardized
+    moment coefficient G1).
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = pd.Series(x)
+    return pd.Series.skew(x)
+
+
+@set_property("fctype", "simple")
+def kurtosis(x):
+    """
+    Returns the kurtosis of x (calculated with the adjusted Fisher-Pearson standardized
+    moment coefficient G2).
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = pd.Series(x)
+    return pd.Series.kurtosis(x)
+
+
+@set_property("fctype", "simple")
+def absolute_sum_of_changes(x):
+    """
+    Returns the sum over the absolute value of consecutive changes in the series x
+
+    .. math::
+
+        \\sum_{i=1, \ldots, n-1} \\mid x_{i+1}- x_i \\mid
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return np.sum(abs(np.diff(x)))
+
+
+@set_property("fctype", "simple")
+def longest_strike_below_mean(x):
+    """
+    Returns the length of the longest consecutive subsequence in x that is smaller than the mean of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+
+    return max(_get_length_sequences_where(x <= np.mean(x))) if len(x) > 0 else 0
+
+
+@set_property("fctype", "simple")
+def longest_strike_above_mean(x):
+    """
+    Returns the length of the longest consecutive subsequence in x that is bigger than the mean of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+
+    return max(_get_length_sequences_where(x >= np.mean(x))) if len(x) > 0 else 0
+
+
+@set_property("fctype", "simple")
+def count_above_mean(x):
+    """
+    Returns the number of values in x that are higher than the mean of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+
+    x = np.asarray(x)
+    m = np.mean(x)
+    return np.where(x > m)[0].shape[0]
+
+
+@set_property("fctype", "simple")
+def count_below_mean(x):
+    """
+    Returns the number of values in x that are lower than the mean of x
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+
+    x = np.asarray(x)
+    m = np.mean(x)
+    return np.where(x < m)[0].shape[0]
+
+
+@set_property("fctype", "simple")
+def last_location_of_maximum(x):
+    """
+    Returns the relative last location of the maximum value of x.
+    The position is calculated relatively to the length of x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+    return 1.0 - np.argmax(x[::-1]) / len(x) if len(x) > 0 else np.NaN
+
+
+@set_property("fctype", "simple")
+def first_location_of_maximum(x):
+    """
+    Returns the first location of the maximum value of x.
+    The position is calculated relatively to the length of x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+    return np.argmax(x) / len(x) if len(x) > 0 else np.NaN
+
+
+@set_property("fctype", "simple")
+def last_location_of_minimum(x):
+    """
+    Returns the last location of the minimal value of x.
+    The position is calculated relatively to the length of x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+    return 1.0 - np.argmin(x[::-1]) / len(x) if len(x) > 0 else np.NaN
+
+
+@set_property("fctype", "simple")
+def first_location_of_minimum(x):
+    """
+    Returns the first location of the minimal value of x.
+    The position is calculated relatively to the length of x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+    return np.argmin(x) / len(x) if len(x) > 0 else np.NaN
+
+
+@set_property("fctype", "simple")
+def percentage_of_reoccurring_datapoints_to_all_datapoints(x):
+    """
+    Returns the percentage of unique values, that are present in the time series
+    more than once.
+
+        len(different values occurring more than once) / len(different values)
+
+    This means the percentage is normalized to the number of unique values,
+    in contrast to the percentage_of_reoccurring_values_to_all_values.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+
+    unique, counts = np.unique(x, return_counts=True)
+    return np.sum(counts > 1) / float(counts.shape[0])
+
+
+@set_property("fctype", "simple")
+def percentage_of_reoccurring_values_to_all_values(x):
+    """
+    Returns the ratio of unique values, that are present in the time series
+    more than once.
+
+        # of data points occurring more than once / # of all data points
+
+    This means the ratio is normalized to the number of data points in the time series,
+    in contrast to the percentage_of_reoccurring_datapoints_to_all_datapoints.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    x = pd.Series(x)
+
+    if len(x) == 0:
+        return np.nan
+
+    value_counts = x.value_counts()
+    return value_counts[value_counts > 1].sum() / len(x)
+
+
+@set_property("fctype", "simple")
+def sum_of_reoccurring_values(x):
+    """
+    Returns the sum of all values, that are present in the time series
+    more than once.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    unique, counts = np.unique(x, return_counts=True)
+    counts[counts < 2] = 0
+    counts[counts > 1] = 1
+    return np.sum(counts * unique)
+
+
+@set_property("fctype", "simple")
+def sum_of_reoccurring_data_points(x):
+    """
+    Returns the sum of all data points, that are present in the time series
+    more than once.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    unique, counts = np.unique(x, return_counts=True)
+    counts[counts < 2] = 0
+    return np.sum(counts * unique)
+
+
+@set_property("fctype", "simple")
+def ratio_value_number_to_time_series_length(x):
+    """
+    Returns a factor which is 1 if all values in the time series occur only once,
+    and below one if this is not the case.
+    In principle, it just returns
+
+        # unique values / # values
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+
+    if len(x) == 0:
+        return np.nan
+
+    return len(set(x))/len(x)
+
+
+@set_property("fctype", "combiner")
+def fft_coefficient(x, param):
+    """
+    Calculates the fourier coefficients of the one-dimensional discrete Fourier Transform for real input by fast
+    fourier transformation algorithm
+
+    .. math::
+        A_k =  \\sum_{m=0}^{n-1} a_m \\exp \\left \\{ -2 \\pi i \\frac{m k}{n} \\right \\}, \\qquad k = 0, \\ldots , n-1.
+
+    The resulting coefficients will be complex, this feature calculator can return the real part (attr=="real"),
+    the imaginary part (attr=="imag), the absolute value (attr=""abs) and the angle in degrees (attr=="angle).
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"coeff": x, "attr": s} with x int and x >= 0, s str and in ["real", "imag",
+        "abs", "angle"]
+    :type param: list
+    :return: the different feature values
+    :return type: pandas.Series
+    """
+
+    assert min([config["coeff"] for config in param]) >= 0, "Coefficients must be positive or zero."
+    assert set([config["attr"] for config in param]) <= set(["imag", "real", "abs", "angle"]), \
+        'Attribute must be "real", "imag", "angle" or "abs"'
+
+    fft = np.fft.rfft(x)
+
+    def complex_agg(x, agg):
+        if agg == "real":
+            return x.real
+        elif agg == "imag":
+            return x.imag
+        elif agg == "abs":
+            return np.abs(x)
+        elif agg == "angle":
+            return np.angle(x, deg=True)
+
+    res = [complex_agg(fft[config["coeff"]], config["attr"]) if config["coeff"] < len(fft)
+           else np.NaN for config in param]
+    index = ['coeff_{}__attr_"{}"'.format(config["coeff"], config["attr"]) for config in param]
+    return zip(index, res)
+
+
+@set_property("fctype", "simple")
+def number_peaks(x, n):
+    """
+    Calculates the number of peaks of at least support n in the time series x. A peak of support n is defined as a
+    subsequence of x where a value occurs, which is bigger than its n neighbours to the left and to the right.
+
+    Hence in the sequence
+
+    >>> x = [3, 0, 0, 4, 0, 0, 13]
+
+    4 is a peak of support 1 and 2 because in the subsequences
+
+    >>> [0, 4, 0]
+    >>> [0, 0, 4, 0, 0]
+
+    4 is still the highest value. Here, 4 is not a peak of support 3 because 13 is the 3th neighbour to the right of 4
+    and its bigger than 4.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param n: the support of the peak
+    :type n: int
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+    x_reduced = x[n:-n]
+
+    res = None
+    for i in range(1, n + 1):
+        result_first = (x_reduced > np.roll(x, i)[n:-n])
+
+        if res is None:
+            res = result_first
+        else:
+            res &= result_first
+
+        res &= (x_reduced > np.roll(x, -i)[n:-n])
+    return sum(res)
+
+
+@set_property("fctype", "combiner")
+def index_mass_quantile(x, param):
+    """
+    Those apply features calculate the relative index i where q% of the mass of the time series x lie left of i.
+    For example for q = 50% this feature calculator will return the mass center of the time series
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"q": x} with x float
+    :type param: list
+    :return: the different feature values
+    :return type: pandas.Series
+    """
+
+    x = np.asarray(x)
+    abs_x = np.abs(x)
+    s = sum(abs_x)
+
+    if s == 0:
+        # all values in x are zero or it has length 0
+        return [("q_{}".format(config["q"]), np.NaN) for config in param]
+    else:
+        # at least one value is not zero
+        mass_centralized = np.cumsum(abs_x) / s
+        return [("q_{}".format(config["q"]),
+                (np.argmax(mass_centralized >= config["q"])+1)/len(x)) for config in param]
+
+
+@set_property("fctype", "simple")
+def number_cwt_peaks(x, n):
+    """
+    This feature calculator searches for different peaks in x. To do so, x is smoothed by a ricker wavelet and for
+    widths ranging from 1 to n. This feature calculator returns the number of peaks that occur at enough width scales
+    and with sufficiently high Signal-to-Noise-Ratio (SNR)
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param n: maximum width to consider
+    :type n: int
+    :return: the value of this feature
+    :return type: int
+    """
+    return len(find_peaks_cwt(vector=x, widths=np.array(list(range(1, n + 1))), wavelet=ricker))
+
+
+@set_property("fctype", "combiner")
+def linear_trend(x, param):
+    """
+    Calculate a linear least-squares regression for the values of the time series versus the sequence from 0 to
+    length of the time series minus one.
+    This feature assumes the signal to be uniformly sampled. It will not use the time stamps to fit the model.
+    The parameters control which of the characteristics are returned.
+
+    Possible extracted attributes are "pvalue", "rvalue", "intercept", "slope", "stderr", see the documentation of
+    linregress for more information.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"attr": x} with x an string, the attribute name of the regression model
+    :type param: list
+    :return: the different feature values
+    :return type: pandas.Series
+    """
+    # todo: we could use the index of the DataFrame here
+
+    linReg = linregress(range(len(x)), x)
+
+    return [("attr_\"{}\"".format(config["attr"]), getattr(linReg, config["attr"]))
+            for config in param]
+
+
+@set_property("fctype", "combiner")
+def cwt_coefficients(x, param):
+    """
+    Calculates a Continuous wavelet transform for the Ricker wavelet, also known as the "Mexican hat wavelet" which is
+    defined by
+
+    .. math::
+        \\frac{2}{\\sqrt{3a} \\pi^{\\frac{1}{4}}} (1 - \\frac{x^2}{a^2}) exp(-\\frac{x^2}{2a^2})
+
+    where :math:`a` is the width parameter of the wavelet function.
+
+    This feature calculator takes three different parameter: widths, coeff and w. The feature calculater takes all the
+    different widths arrays and then calculates the cwt one time for each different width array. Then the values for the
+    different coefficient for coeff and width w are returned. (For each dic in param one feature is returned)
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"widths":x, "coeff": y, "w": z} with x array of int and y,z int
+    :type param: list
+    :return: the different feature values
+    :return type: pandas.Series
+    """
+
+    calculated_cwt = {}
+    res = []
+    indices = []
+
+    for parameter_combination in param:
+        widths = parameter_combination["widths"]
+        w = parameter_combination["w"]
+        coeff = parameter_combination["coeff"]
+
+        if widths not in calculated_cwt:
+            calculated_cwt[widths] = cwt(x, ricker, widths)
+
+        calculated_cwt_for_widths = calculated_cwt[widths]
+
+        indices += ["widths_{}__coeff_{}__w_{}".format(widths, coeff, w)]
+
+        i = widths.index(w)
+        if calculated_cwt_for_widths.shape[1] <= coeff:
+            res += [np.NaN]
+        else:
+            res += [calculated_cwt_for_widths[i, coeff]]
+
+    return zip(indices, res)
+
+
+@set_property("fctype", "combiner")
+def spkt_welch_density(x, param):
+    """
+    This feature calculator estimates the cross power spectral density of the time series x at different frequencies.
+    To do so, the time series is first shifted from the time domain to the frequency domain.
+
+    The feature calculators returns the power spectrum of the different frequencies.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"coeff": x} with x int
+    :type param: list
+    :return: the different feature values
+    :return type: pandas.Series
+    """
+
+    freq, pxx = welch(x)
+    coeff = [config["coeff"] for config in param]
+    indices = ["coeff_{}".format(i) for i in coeff]
+
+    if len(pxx) <= max(coeff):  # There are fewer data points in the time series than requested coefficients
+
+        # filter coefficients that are not contained in pxx
+        reduced_coeff = [coefficient for coefficient in coeff if len(pxx) > coefficient]
+        not_calculated_coefficients = [coefficient for coefficient in coeff
+                                       if coefficient not in reduced_coeff]
+
+        # Fill up the rest of the requested coefficients with np.NaNs
+        return zip(indices, list(pxx[reduced_coeff]) + [np.NaN] * len(not_calculated_coefficients))
+    else:
+        return zip(indices, pxx[coeff])
+
+
+@set_property("fctype", "combiner")
+def ar_coefficient(x, param):
+    """
+    This feature calculator fits the unconditional maximum likelihood
+    of an autoregressive AR(k) process.
+    The k parameter is the maximum lag of the process
+
+    .. math::
+
+        X_{t}=\\varphi_0 +\\sum _{{i=1}}^{k}\\varphi_{i}X_{{t-i}}+\\varepsilon_{t}
+
+    For the configurations from param which should contain the maxlag "k" and such an AR process is calculated. Then
+    the coefficients :math:`\\varphi_{i}` whose index :math:`i` contained from "coeff" are returned.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"coeff": x, "k": y} with x,y int
+    :type param: list
+    :return x: the different feature values
+    :return type: pandas.Series
+    """
+    calculated_ar_params = {}
+
+    x_as_list = list(x)
+    calculated_AR = AR(x_as_list)
+
+    res = {}
+
+    for parameter_combination in param:
+        k = parameter_combination["k"]
+        p = parameter_combination["coeff"]
+
+        column_name = "k_{}__coeff_{}".format(k, p)
+
+        if k not in calculated_ar_params:
+            try:
+                calculated_ar_params[k] = calculated_AR.fit(maxlag=k, solver="mle").params
+            except (LinAlgError, ValueError):
+                calculated_ar_params[k] = [np.NaN]*k
+
+        mod = calculated_ar_params[k]
+
+        if p <= k:
+            try:
+                res[column_name] = mod[p]
+            except IndexError:
+                res[column_name] = 0
+        else:
+            res[column_name] = np.NaN
+
+    return [(key, value) for key, value in res.items()]
+
+
+@set_property("fctype", "simple")
+def change_quantiles(x, ql, qh, isabs, f_agg):
+    """
+    First fixes a corridor given by the quantiles ql and qh of the distribution of x.
+    Then calculates the average, absolute value of consecutive changes of the series x inside this corridor.
+
+    Think about selecting a corridor on the
+    y-Axis and only calculating the mean of the absolute change of the time series inside this corridor.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param ql: the lower quantile of the corridor
+    :type ql: float
+    :param qh: the higher quantile of the corridor
+    :type qh: float
+    :param isabs: should the absolute differences be taken?
+    :type isabs: bool
+    :param f_agg: the aggregator function that is applied to the differences in the bin
+    :type f_agg: str, name of a numpy function (e.g. mean, var, std, median)
+
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+
+    if ql >= qh:
+        ValueError("ql={} should be lower than qh={}".format(ql, qh))
+
+    div = np.diff(x)
+    if isabs:
+        div = np.abs(div)
+    # All values that originate from the corridor between the quantiles ql and qh will have the category 0,
+    # other will be np.NaN
+    try:
+        bin_cat = pd.qcut(x, [ql, qh], labels=False)
+        bin_cat_0 = bin_cat == 0
+    except ValueError:  # Occurs when ql are qh effectively equal, e.g. x is not long enough or is too categorical
+        return 0
+    # We only count changes that start and end inside the corridor
+    ind = (bin_cat_0 * np.roll(bin_cat_0, 1))[1:]
+    if sum(ind) == 0:
+        return 0
+    else:
+        ind_inside_corridor = np.where(ind == 1)
+        aggregator = getattr(np, f_agg)
+        return aggregator(div[ind_inside_corridor])
+
+
+
+@set_property("fctype", "simple")
+def time_reversal_asymmetry_statistic(x, lag):
+    """
+    This function calculates the value of
+
+    .. math::
+
+        \\frac{1}{n-2lag} \sum_{i=0}^{n-2lag} x_{i + 2 \cdot lag}^2 \cdot x_{i + lag} - x_{i + lag} \cdot  x_{i}^2
+
+    which is
+
+    .. math::
+
+        \\mathbb{E}[L^2(X)^2 \cdot L(X) - L(X) \cdot X^2]
+
+    where :math:`\\mathbb{E}` is the mean and :math:`L` is the lag operator. It was proposed in [1] as a
+    promising feature to extract from time series.
+
+    References
+    ----------
+
+    .. [1] Fulcher, B.D., Jones, N.S. (2014).
+       Highly comparative feature-based time-series classification.
+       Knowledge and Data Engineering, IEEE Transactions on 26, 3026–3037.
+
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param lag: the lag that should be used in the calculation of the feature
+    :type lag: int
+    :return: the value of this feature
+    :return type: float
+    """
+    n = len(x)
+    x = np.asarray(x)
+    if 2 * lag >= n:
+        return 0
+    else:
+        return np.mean((np.roll(x, 2 * -lag) * np.roll(x, 2 * -lag) * np.roll(x, -lag) -
+                        np.roll(x, -lag) * x * x)[0:(n - 2 * lag)])
+
+
+@set_property("fctype", "simple")
+def c3(x, lag):
+    """
+    This function calculates the value of
+
+    .. math::
+
+        \\frac{1}{n-2lag} \sum_{i=0}^{n-2lag} x_{i + 2 \cdot lag}^2 \cdot x_{i + lag} \cdot x_{i}
+
+    which is
+
+    .. math::
+
+        \\mathbb{E}[L^2(X)^2 \cdot L(X) \cdot X]
+
+    where :math:`\\mathbb{E}` is the mean and :math:`L` is the lag operator. It was proposed in [1] as a measure of
+    non linearity in the time series.
+
+    References
+    ----------
+
+    .. [1] Schreiber, T. and Schmitz, A. (1997).
+       Discrimination power of measures for nonlinearity in a time series
+       PHYSICAL REVIEW E, VOLUME 55, NUMBER 5
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param lag: the lag that should be used in the calculation of the feature
+    :type lag: int
+    :return: the value of this feature
+    :return type: float
+    """
+    n = len(x)
+    x = np.asarray(x)
+    if 2 * lag >= n:
+        return 0
+    else:
+        return np.mean((np.roll(x, 2 * -lag) * np.roll(x, -lag) * x)[0:(n - 2 * lag)])
+
+
+@set_property("fctype", "simple")
+def binned_entropy(x, max_bins):
+    """
+    First bins the values of x into max_bins equidistant bins.
+    Then calculates the value of
+
+    .. math::
+
+        - \\sum_{k=0}^{min(max\\_bins, len(x))} p_k log(p_k) \\cdot \\mathbf{1}_{(p_k > 0)}
+
+    where :math:`p_k` is the percentage of samples in bin :math:`k`.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param max_bins: the maximal number of bins
+    :type max_bins: int
+    :return: the value of this feature
+    :return type: float
+    """
+    hist, bin_edges = np.histogram(x, bins=max_bins)
+    probs = hist / len(x)
+    return - np.sum(p * np.math.log(p) for p in probs if p != 0)
+
+# todo - include latex formula
+# todo - check if vectorizable
+@set_property("high_comp_cost", True)
+@set_property("fctype", "simple")
+def sample_entropy(x):
+    """
+    Calculate and return sample entropy of x.
+    References:
+    ----------
+    [1] http://en.wikipedia.org/wiki/Sample_Entropy
+    [2] https://www.ncbi.nlm.nih.gov/pubmed/10843903?dopt=Abstract
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param tolerance: normalization factor; equivalent to the common practice of expressing the tolerance as r times the standard deviation
+    :type tolerance: float
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.array(x)
+
+    sample_length = 1 # number of sequential points of the time series
+    tolerance = 0.2 * np.std(x) # 0.2 is a common value for r - why?
+
+    n = len(x)
+    prev = np.zeros(n)
+    curr = np.zeros(n)
+    A = np.zeros((1, 1))  # number of matches for m = [1,...,template_length - 1]
+    B = np.zeros((1, 1))  # number of matches for m = [1,...,template_length]
+
+    for i in range(n - 1):
+        nj = n - i - 1
+        ts1 = x[i]
+        for jj in range(nj):
+            j = jj + i + 1
+            if abs(x[j] - ts1) < tolerance:  # distance between two vectors
+                curr[jj] = prev[jj] + 1
+                temp_ts_length = min(sample_length, curr[jj])
+                for m in range(int(temp_ts_length)):
+                    A[m] += 1
+                    if j < n - 1:
+                        B[m] += 1
+            else:
+                curr[jj] = 0
+        for j in range(nj):
+            prev[j] = curr[j]
+
+    N = n * (n - 1) / 2
+    B = np.vstack(([N], B[0]))
+
+    # sample entropy = -1 * (log (A/B))
+    similarity_ratio = A / B
+    se = -1 * np.log(similarity_ratio)
+    se = np.reshape(se, -1)
+    return se[0]
+
+
+@set_property("fctype", "simple")
+def autocorrelation(x, lag):
+    """
+    Calculates the autocorrelation of the specified lag, according to the formula [1]
+
+    .. math::
+
+        \\frac{1}{(n-l)\sigma^{2}} \\sum_{t=1}^{n-l}(X_{t}-\\mu )(X_{t+l}-\\mu)
+
+    where :math:`n` is the length of the time series :math:`X_i`, :math:`\sigma^2` its variance and :math:`\mu` its
+    mean. `l` denotes the lag.
+
+    .. rubric:: References
+
+    [1] https://en.wikipedia.org/wiki/Autocorrelation#Estimation
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param lag: the lag
+    :type lag: int
+    :return: the value of this feature
+    :return type: float
+    """
+    # This is important: If a series is passed, the product below is calculated
+    # based on the index, which corresponds to squaring the series.
+    if type(x) is pd.Series:
+        x = x.values
+    if len(x) < lag:
+        return np.nan
+    # Slice the relevant subseries based on the lag
+    y1 = x[:(len(x)-lag)]
+    y2 = x[lag:]
+    # Subtract the mean of the whole series x
+    x_mean = np.mean(x)
+    # The result is sometimes referred to as "covariation"
+    sum_product = np.sum((y1-x_mean)*(y2-x_mean))
+    # Return the normalized unbiased covariance
+    return sum_product / ((len(x) - lag) * np.var(x))
+
+
+@set_property("fctype", "simple")
+def quantile(x, q):
+    """
+    Calculates the q quantile of x. This is the value of x greater than q% of the ordered values from x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param q: the quantile to calculate
+    :type q: float
+    :return: the value of this feature
+    :return type: float
+    """
+    x = pd.Series(x)
+    return pd.Series.quantile(x, q)
+
+
+@set_property("fctype", "simple")
+def number_crossing_m(x, m):
+    """
+    Calculates the number of crossings of x on m. A crossing is defined as two sequential values where the first value
+    is lower than m and the next is greater, or vice-versa. If you set m to zero, you will get the number of zero
+    crossings.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param m: the threshold for the crossing
+    :type m: float
+    :return: the value of this feature
+    :return type: float
+    """
+    x = np.asarray(x)
+    x = x[x != m]
+    return sum(np.abs(np.diff(np.sign(x - m))))/2
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def maximum(x):
+    """
+    Calculates the highest value of the time series x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return max(x)
+
+
+@set_property("fctype", "simple")
+@set_property("minimal", True)
+def minimum(x):
+    """
+    Calculates the lowest value of the time series x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :return: the value of this feature
+    :return type: float
+    """
+    return min(x)
+
+
+@set_property("fctype", "simple")
+def value_count(x, value):
+    """
+    Count occurrences of `value` in time series x.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param value: the value to be counted
+    :type value: int or float
+    :return: the count
+    :rtype: int
+    """
+    if np.isnan(value):
+        return np.isnan(x).sum()
+    else:
+        return x[x == value].shape[0]
+
+
+@set_property("fctype", "simple")
+def range_count(x, min, max):
+    """
+    Count observed values within the interval [min, max).
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param min: the inclusive lower bound of the range
+    :type min: int or float
+    :param max: the exclusive upper bound of the range
+    :type max: int or float
+    :return: the count of values within the range
+    :rtype: int
+    """
+    return np.sum((x >= min) & (x < max))
+
+
+@set_property("fctype", "simple")
+@set_property("high_comp_cost", True)
+def approximate_entropy(x, m, r):
+    """
+    Implements a vectorized Approximate entropy algorithm.
+
+        https://en.wikipedia.org/wiki/Approximate_entropy
+
+    For short time-series this method is highly dependent on the parameters,
+    but should be stable for N > 2000, see:
+
+        Yentes et al. (2012) -
+        *The Appropriate Use of Approximate Entropy and Sample Entropy with Short Data Sets*
+
+
+    Other shortcomings and alternatives discussed in:
+
+        Richman & Moorman (2000) -
+        *Physiological time-series analysis using approximate entropy and sample entropy*
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param m: Length of compared run of data
+    :type m: int
+    :param r: Filtering level, must be positive
+    :type r: float
+
+    :return: Approximate entropy
+    :return type: float
+    """
+    x = np.asarray(x)
+    N = len(x)
+    r *= np.std(x)
+    if r < 0:
+        raise ValueError("Parameter r must be positive.")
+    if N <= m+1:
+        return 0
+
+    def _phi(m):
+        x_re = np.array([x[i:i+m] for i in range(N - m + 1)])
+        C = np.sum(np.max(np.abs(x_re[:, np.newaxis] - x_re[np.newaxis, :]),
+                          axis=2) <= r, axis=0) / (N-m+1)
+        return np.sum(np.log(C)) / (N - m + 1.0)
+
+    return np.abs(_phi(m) - _phi(m + 1))
+
+
+@set_property("fctype", "combiner")
+def friedrich_coefficients(x, param):
+    """
+    Coefficients of polynomial :math:`h(x)`, which has been fitted to
+    the deterministic dynamics of Langevin model
+
+    .. math::
+        \dot{x}(t) = h(x(t)) + \mathcal{N}(0,R)
+
+    as described by
+
+        Friedrich et al. (2000): Physics Letters A 271, p. 217-222
+        *Extracting model equations from experimental data*
+
+
+    For short time-series this method is highly dependent on the parameters.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param c: the time series name
+    :type c: str
+    :param param: contains dictionaries {"coeff": x} with x int and x >= 0
+    :type param: list
+    :return: the different feature values
+    :return type: pandas.Series
+    """
+    coefficients = set([config["coeff"] for config in param])
+    for coeff in coefficients:
+        if coeff < 0:
+            raise ValueError("Coefficients must be positive or zero.")
+
+    m = param[0]['m']
+    r = param[0]['r']
+
+    coeff = _estimate_friedrich_coefficients(x, m, r)
+    indices = ["m_{}__r_{}__coeff_{}".format(m, r, q) for q in range(m, -1, -1)]
+
+    return zip(indices, coeff)
+
+
+@set_property("fctype", "simple")
+def max_langevin_fixed_point(x, r, m):
+    """
+    Largest fixed point of dynamics  :math:argmax_x {h(x)=0}` estimated from polynomial :math:`h(x)`,
+    which has been fitted to the deterministic dynamics of Langevin model
+
+    .. math::
+        \dot(x)(t) = h(x(t)) + R \mathcal(N)(0,1)
+
+    as described by
+
+        Friedrich et al. (2000): Physics Letters A 271, p. 217-222
+        *Extracting model equations from experimental data*
+
+    For short time-series this method is highly dependent on the parameters.
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param m: order of polynom to fit for estimating fixed points of dynamics
+    :type m: int
+    :param r: number of quantils to use for averaging
+    :type r: float
+
+    :return: Largest fixed point of deterministic dynamics
+    :return type: float
+    """
+
+    coeff = _estimate_friedrich_coefficients(x, m, r)
+
+    try:
+        max_fixed_point = np.max(np.real(np.roots(coeff)))
+    except (np.linalg.LinAlgError, ValueError):
+        return np.nan
+
+    return max_fixed_point
+
+
+@set_property("fctype", "combiner")
+def agg_linear_trend(x, param):
+    """
+    Calculates a linear least-squares regression for values of the time series that were aggregated over chunks versus
+    the sequence from 0 up to the number of chunks minus one.
+
+    This feature assumes the signal to be uniformly sampled. It will not use the time stamps to fit the model.
+
+    The parameters attr controls which of the characteristics are returned. Possible extracted attributes are "pvalue",
+    "rvalue", "intercept", "slope", "stderr", see the documentation of linregress for more information.
+
+    The chunksize is regulated by "chunk_len". It specifies how many time series values are in each chunk.
+
+    Further, the aggregation function is controlled by "f_agg", which can use "max", "min" or , "mean", "median"
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"attr": x, "chunk_len": l, "f_agg": f} with x, f an string and l an int
+    :type param: list
+    :return: the different feature values
+    :return type: pandas.Series
+    """
+    # todo: we could use the index of the DataFrame here
+
+    calculated_agg = {}
+    res_data = []
+    res_index = []
+
+    for parameter_combination in param:
+
+        chunk_len = parameter_combination["chunk_len"]
+        f_agg = parameter_combination["f_agg"]
+
+        aggregate_result = _aggregate_on_chunks(x, f_agg, chunk_len)
+        if f_agg not in calculated_agg or chunk_len not in calculated_agg[f_agg]:
+            if chunk_len >= len(x):
+                calculated_agg[f_agg] = {chunk_len: np.NaN}
+            else:
+                lin_reg_result = linregress(range(len(aggregate_result)), aggregate_result)
+                calculated_agg[f_agg] = {chunk_len: lin_reg_result}
+
+        attr = parameter_combination["attr"]
+
+        if chunk_len >= len(x):
+            res_data.append(np.NaN)
+        else:
+            res_data.append(getattr(calculated_agg[f_agg][chunk_len], attr))
+
+        res_index.append("f_agg_\"{}\"__chunk_len_{}__attr_\"{}\"".format(f_agg, chunk_len, attr))
+
+    return zip(res_index, res_data)
+
+
+@set_property("fctype", "combiner")
+def energy_ratio_by_chunks(x, param):
+    """
+    Calculates the sum of squares of chunk i out of N chunks expressed as a ratio with the sum of squares over the whole series
+
+    Takes as input parameters the number num_segments of segments to divide the series into and segment_focus
+    which is the segment number (starting at zero) to return a feature on.
+
+    Note that the answer for num_segments=1 is a trivial "1" but we handle this scenario
+    in case somebody calls it. Sum of the ratios should be 1.0.
+
+    Returns an error for N <= 0
+
+    :param x: the time series to calculate the feature of
+    :type x: pandas.Series
+    :param param: contains dictionaries {"num_segments": N, "segment_focus": i} with N, i both ints
+    :return: the feature values
+    :return feature name, feature value
+    """
+
+    res_data = []
+    res_index = []
+    full_series_energy = np.sum(x ** 2)
+
+    for parameter_combination in param:
+        num_segments = parameter_combination["num_segments"]
+        segment_focus = parameter_combination["segment_focus"]
+        assert segment_focus < num_segments
+
+        segment_length = len(x)//num_segments
+        start = segment_focus*segment_length
+        end = min((segment_focus+1)*segment_length, len(x))
+        res_data.append(np.sum(x[start:end]**2.0)/full_series_energy)
+        res_index.append("num_segments_{}__segment_focus_{}".format(num_segments, segment_focus))
+
+    return list(zip(res_index, res_data)) # Materialize as list for Python 3 compatibility with name handling
```

### Comparing `tsfresh-0.8.1/tsfresh/feature_selection/__init__.py` & `tsfresh-0.9.0/tsfresh/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/feature_selection/feature_selector.py` & `tsfresh-0.9.0/tsfresh/feature_selection/relevance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,278 +1,247 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-"""
-Contains a feature selection method that evaluates the importance of the different extracted features. To do so,
-for every feature the influence on the target is evaluated by an univariate tests and the p-Value is calculated.
-The methods that calculate the p-values are called feature selectors.
-
-Afterwards the Benjamini Hochberg procedure which is a multiple testing procedure decides which features to keep and
-which to cut off (solely based on the p-values).
-"""
-
-from __future__ import absolute_import, division, print_function
-
-from functools import partial
-
-from builtins import zip
-from builtins import range
-import os
-import numpy as np
-import pandas as pd
-import logging
-from multiprocessing import Pool
-from tsfresh.feature_selection.significance_tests import target_binary_feature_real_test, \
-    target_real_feature_binary_test, target_real_feature_real_test, target_binary_feature_binary_test
-from tsfresh import defaults
-
-
-_logger = logging.getLogger(__name__)
-
-
-def check_fs_sig_bh(X, y,
-                    n_processes=defaults.N_PROCESSES,
-                    chunksize=defaults.CHUNKSIZE,
-                    fdr_level=defaults.FDR_LEVEL,
-                    hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
-                    test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE):
-    """
-    The wrapper function that calls the significance test functions in this package.
-    In total, for each feature from the input pandas.DataFrame an univariate feature significance test is conducted.
-    Those tests generate p values that are then evaluated by the Benjamini Hochberg procedure to decide which features
-    to keep and which to delete.
-
-    We are testing
-    
-        :math:`H_0` = the Feature is not relevant and can not be added
-
-    against
-
-        :math:`H_1` = the Feature is relevant and should be kept
-   
-    or in other words
- 
-        :math:`H_0` = Target and Feature are independent / the Feature has no influence on the target
-
-        :math:`H_1` = Target and Feature are associated / dependent
-
-    When the target is binary this becomes
-    
-        :math:`H_0 = \\left( F_{\\text{target}=1} = F_{\\text{target}=0} \\right)`
-
-        :math:`H_1 = \\left( F_{\\text{target}=1} \\neq F_{\\text{target}=0} \\right)`
-    
-    Where :math:`F` is the distribution of the target.
-
-    In the same way we can state the hypothesis when the feature is binary
-    
-        :math:`H_0 =  \\left( T_{\\text{feature}=1} = T_{\\text{feature}=0} \\right)`
-
-        :math:`H_1 = \\left( T_{\\text{feature}=1} \\neq T_{\\text{feature}=0} \\right)`
-
-    Here :math:`T` is the distribution of the target.
-
-    TODO: And for real valued?
-
-    :param X: The DataFrame containing all the features and the target
-    :type X: pandas.DataFrame
-
-    :param y: The target vector
-    :type y: pandas.Series
-
-    :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
-    :type test_for_binary_target_real_feature: str
-
-    :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
-                      features among all created features.
-    :type fdr_level: float
-
-    :param hypotheses_independent: Can the significance of the features be assumed to be independent?
-                                   Normally, this should be set to False as the features are never
-                                   independent (e.g. mean and median)
-    :type hypotheses_independent: bool
-
-    :param n_processes: Number of processes to use during the p-value calculation
-    :type n_processes: int
-
-    :param chunksize: Size of the chunks submitted to the worker processes
-    :type chunksize: int
-
-    :return: A pandas.DataFrame with each column of the input DataFrame X as index with information on the significance
-            of this particular feature. The DataFrame has the columns
-            "Feature",
-            "type" (binary, real or const),
-            "p_value" (the significance of this feature as a p-value, lower means more significant)
-            "rejected" (if the Benjamini Hochberg procedure rejected this feature)
-    :rtype: pandas.DataFrame
-
-    """
-    target_is_binary = len(set(y)) == 2
-
-    # todo: solve the multiclassification case. for a multi classification the algorithm considers the target to be
-    # regression. Instead one could perform a binary one versus all classification.
-
-    # Only allow entries for which the target is known!
-    y = y.astype(np.float)
-    X = X.copy().loc[~(y == np.NaN), :]
-
-    # Create the DataFrame df_features containing the information about the different hypotheses
-    # Every row contains information over one feature column from X
-    df_features = pd.DataFrame()
-
-    df_features['Feature'] = list(set(X.columns))
-    df_features = df_features.set_index('Feature', drop=False)
-
-    # Add relevant columns to df_features
-    df_features["rejected"] = np.nan
-    df_features["type"] = np.nan
-    df_features["p_value"] = np.nan
-
-    # Calculate the feature significance in parallel
-    pool = Pool(n_processes)
-
-    # Helper function which wrapps the _calculate_p_value with many arguments already set
-    f = partial(_calculate_p_value, y=y,
-                target_is_binary=target_is_binary,
-                test_for_binary_target_real_feature=test_for_binary_target_real_feature)
-    results = pool.map(f, [X[feature] for feature in df_features['Feature']], chunksize=chunksize)
-    p_values_of_features = pd.DataFrame(results)
-    df_features.update(p_values_of_features)
-
-    pool.close()
-    pool.join()
-
-    # Perform the real feature rejection
-    if "const" in set(df_features.type):
-        df_features_bh = benjamini_hochberg_test(df_features.loc[~(df_features.type == "const")],
-                                                 hypotheses_independent, fdr_level)
-        df_features = pd.concat([df_features_bh, df_features.loc[df_features.type == "const"]])
-    else:
-        df_features = benjamini_hochberg_test(df_features, hypotheses_independent, fdr_level)
-        
-    # It is very important that we have a boolean "rejected" column, so we do a cast here to be sure
-    df_features["rejected"] = df_features["rejected"].astype("bool")
-
-    if defaults.WRITE_SELECTION_REPORT:
-        # Write results of BH - Test to file
-        if not os.path.exists(defaults.RESULT_DIR):
-            os.mkdir(defaults.RESULT_DIR)
-
-        with open(os.path.join(defaults.RESULT_DIR, "fs_bh_results.txt"), 'w') as file_out:
-            file_out.write(("Performed BH Test to control the false discovery rate(FDR); \n"
-                            "FDR-Level={0};Hypothesis independent={1}\n"
-                            ).format(fdr_level, hypotheses_independent))
-            df_features.to_csv(index=False, path_or_buf=file_out, sep=';', float_format='%.4f')
-    return df_features
-
-
-def _calculate_p_value(feature_column, y, target_is_binary, test_for_binary_target_real_feature):
-    """
-    Internal helper function to calculate the p-value of a given feature using one of the dedicated
-    functions target_*_feature_*_test.
-
-    :param feature_column: the feature column.
-    :type feature_column: pandas.Series
-
-    :param y: the binary target vector
-    :type y: pandas.Series
-
-    :param target_is_binary: Whether the target is binary or not
-    :type target_is_binary: bool
-
-    :param test_for_binary_target_real_feature: The significance test to be used for binary target and real valued
-                                                features. Either ``'mann'`` for the Mann-Whitney-U test or ``'smir'``
-                                                for the Kolmogorov-Smirnov test.
-    :type test_for_binary_target_real_feature: str
-
-    :return: the p-value of the feature significance test and the type of the tested feature as a Series.
-             Lower p-values indicate a higher feature significance.
-    :rtype: pd.Series
-    """
-    # Do not process constant features
-    if len(pd.unique(feature_column.values)) == 1:
-        _logger.warning("[test_feature_significance] Feature {} is constant".format(feature_column.name))
-        return pd.Series({"type": "const", "rejected": False}, name=feature_column.name)
-
-    else:
-        if target_is_binary:
-            # Decide if the current feature is binary or not
-            if len(set(feature_column.values)) == 2:
-                type = "binary"
-                p_value = target_binary_feature_binary_test(feature_column, y)
-            else:
-                type = "real"
-                p_value = target_binary_feature_real_test(feature_column, y, test_for_binary_target_real_feature)
-        else:
-            # Decide if the current feature is binary or not
-            if len(set(feature_column.values)) == 2:
-                type = "binary"
-                p_value = target_real_feature_binary_test(feature_column, y)
-            else:
-                type = "real"
-                p_value = target_real_feature_real_test(feature_column, y)
-
-        return pd.Series({"p_value": p_value, "type": type}, name=feature_column.name)
-
-
-def benjamini_hochberg_test(df_pvalues, hypotheses_independent, fdr_level):
-    """
-    This is an implementation of the benjamini hochberg procedure that calculates which of the hypotheses belonging
-    to the different p-Values from df_p to reject. While doing so, this test controls the false discovery rate,
-    which is the ratio of false rejections by all rejections:
-
-    .. math::
-
-        FDR = \\mathbb{E} \\left [ \\frac{ |\\text{false rejections}| }{ |\\text{all rejections}|} \\right]
-
-
-    References
-    ----------
-
-    .. [1] Benjamini, Yoav and Yekutieli, Daniel (2001).
-        The control of the false discovery rate in multiple testing under dependency.
-        Annals of statistics, 1165--1188
-
-
-    :param df_pvalues: This DataFrame should contain the p_values of the different hypotheses in a column named
-                       "p_values".
-    :type df_pvalues: pandas.DataFrame
-
-    :param hypotheses_independent: Can the significance of the features be assumed to be independent?
-                                   Normally, this should be set to False as the features are never
-                                   independent (e.g. mean and median)
-    :type hypotheses_independent: bool
-
-    :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
-                      features among all created features.
-    :type fdr_level: float
-
-    :return: The same DataFrame as the input, but with an added boolean column "rejected".
-    :rtype: pandas.DataFrame
-    """
-
-    # Get auxiliary variables and vectors
-    df_pvalues = df_pvalues.sort_values(by="p_value")
-    m = len(df_pvalues)
-    K = list(range(1, m + 1))
-
-    # Calculate the weight vector C
-    if hypotheses_independent:
-        # c(k) = 1
-        C = [1] * m
-    else:
-        # c(k) = \sum_{i=1}^m 1/i
-        C = [sum([1.0 / i for i in range(1, k + 1)]) for k in K]
-
-    # Calculate the vector T to compare to the p_value
-    T = [fdr_level * k / m * 1.0 / c for k, c in zip(K, C)]
-
-    # Get the last rejected p_value
-    try:
-        k_max = list(df_pvalues.p_value <= T).index(False)
-    except ValueError:
-        k_max = m
-
-    # Add the column denoting if hypothesis was rejected
-    df_pvalues["rejected"] = [True] * k_max + [False] * (m - k_max)
-
-    return df_pvalues
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+"""
+Contains a feature selection method that evaluates the importance of the different extracted features. To do so,
+for every feature the influence on the target is evaluated by an univariate tests and the p-Value is calculated.
+The methods that calculate the p-values are called feature selectors.
+
+Afterwards the Benjamini Hochberg procedure which is a multiple testing procedure decides which features to keep and
+which to cut off (solely based on the p-values).
+"""
+
+from __future__ import absolute_import, division, print_function
+
+import logging
+from multiprocessing import Pool
+
+import numpy as np
+import os
+import pandas as pd
+from functools import partial, reduce
+
+from tsfresh import defaults
+from tsfresh.feature_selection.benjamini_hochberg_test import benjamini_hochberg_test
+from tsfresh.feature_selection.significance_tests import target_binary_feature_real_test, \
+    target_real_feature_binary_test, target_real_feature_real_test, target_binary_feature_binary_test
+
+_logger = logging.getLogger(__name__)
+
+
+def calculate_relevance_table(X, y, ml_task='auto', n_jobs=defaults.N_PROCESSES, chunksize=defaults.CHUNKSIZE,
+                   test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
+                   test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
+                   test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
+                   test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
+                   fdr_level=defaults.FDR_LEVEL, hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT):
+    """
+    Calculate the relevance table for the features contained in feature matrix `X` with respect to target vector `y`.
+    The relevance table is calculated for the intended machine learning task `ml_task`.
+
+    To accomplish this for each feature from the input pandas.DataFrame an univariate feature significance test
+    is conducted. Those tests generate p values that are then evaluated by the Benjamini Hochberg procedure to
+    decide which features to keep and which to delete.
+
+    We are testing
+
+        :math:`H_0` = the Feature is not relevant and should not be added
+
+    against
+
+        :math:`H_1` = the Feature is relevant and should be kept
+
+    or in other words
+
+        :math:`H_0` = Target and Feature are independent / the Feature has no influence on the target
+
+        :math:`H_1` = Target and Feature are associated / dependent
+
+    When the target is binary this becomes
+
+        :math:`H_0 = \\left( F_{\\text{target}=1} = F_{\\text{target}=0} \\right)`
+
+        :math:`H_1 = \\left( F_{\\text{target}=1} \\neq F_{\\text{target}=0} \\right)`
+
+    Where :math:`F` is the distribution of the target.
+
+    In the same way we can state the hypothesis when the feature is binary
+
+        :math:`H_0 =  \\left( T_{\\text{feature}=1} = T_{\\text{feature}=0} \\right)`
+
+        :math:`H_1 = \\left( T_{\\text{feature}=1} \\neq T_{\\text{feature}=0} \\right)`
+
+    Here :math:`T` is the distribution of the target.
+
+    TODO: And for real valued?
+
+    :param X: Feature matrix in the format mentioned before which will be reduced to only the relevant features.
+              It can contain both binary or real-valued features at the same time.
+    :type X: pandas.DataFrame
+
+    :param y: Target vector which is needed to test which features are relevant. Can be binary or real-valued.
+    :type y: pandas.Series or numpy.ndarray
+
+    :param ml_task: The intended machine learning task. Either `'classification'`, `'regression'` or `'auto'`.
+                    Defaults to `'auto'`, meaning the intended task is inferred from `y`.
+                    If `y` has a boolean, integer or object dtype, the task is assumend to be classification,
+                    else regression.
+    :type ml_task: str
+
+    :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
+    :type test_for_binary_target_binary_feature: str
+
+    :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
+    :type test_for_binary_target_real_feature: str
+
+    :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
+    :type test_for_real_target_binary_feature: str
+
+    :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
+    :type test_for_real_target_real_feature: str
+
+    :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
+                      features among all created features.
+    :type fdr_level: float
+
+    :param hypotheses_independent: Can the significance of the features be assumed to be independent?
+                                   Normally, this should be set to False as the features are never
+                                   independent (e.g. mean and median)
+    :type hypotheses_independent: bool
+
+    :param n_jobs: Number of processes to use during the p-value calculation
+    :type n_jobs: int
+
+    :param chunksize: Size of the chunks submitted to the worker processes
+    :type chunksize: int
+
+    :return: A pandas.DataFrame with each column of the input DataFrame X as index with information on the significance
+             of this particular feature. The DataFrame has the columns
+             "Feature",
+             "type" (binary, real or const),
+             "p_value" (the significance of this feature as a p-value, lower means more significant)
+             "relevant" (True if the Benjamini Hochberg procedure rejected the null hypothesis [the feature is
+             not relevant] for this feature)
+    :rtype: pandas.DataFrame
+    """
+    if ml_task not in ['auto', 'classification', 'regression']:
+        raise ValueError('ml_task must be one of: \'auto\', \'classification\', \'regression\'')
+    elif ml_task == 'auto':
+        ml_task = infer_ml_task(y)
+
+    if n_jobs == 0:
+        map_function = map
+    else:
+        pool = Pool(n_jobs)
+        map_function = partial(pool.map, chunksize=chunksize)
+
+    relevance_table = pd.DataFrame(index=pd.Series(X.columns, name='feature'))
+    relevance_table['feature'] = relevance_table.index
+    relevance_table['type'] = pd.Series(
+        map_function(get_feature_type, [X[feature] for feature in relevance_table.index]),
+        index=relevance_table.index
+    )
+    table_real = relevance_table[relevance_table.type == 'real'].copy()
+    table_binary = relevance_table[relevance_table.type == 'binary'].copy()
+
+    table_const = relevance_table[relevance_table.type == 'constant'].copy()
+    table_const['p_value'] = np.NaN
+    table_const['relevant'] = False
+
+    if len(table_const) == len(relevance_table):
+        return table_const
+
+    if ml_task == 'classification':
+        tables = []
+        for label in y.unique():
+            _test_real_feature = partial(target_binary_feature_real_test, y=(y == label),
+                                              test=test_for_binary_target_real_feature)
+            _test_binary_feature = partial(target_binary_feature_binary_test, y=(y == label))
+            tmp = _calculate_relevance_table_for_implicit_target(
+                table_real, table_binary, X, _test_real_feature, _test_binary_feature, hypotheses_independent,
+                fdr_level, map_function
+            )
+            tables.append(tmp)
+        relevance_table = combine_relevance_tables(tables)
+    elif ml_task == 'regression':
+        _test_real_feature = partial(target_real_feature_real_test, y=y)
+        _test_binary_feature = partial(target_real_feature_binary_test, y=y)
+        relevance_table = _calculate_relevance_table_for_implicit_target(
+            table_real, table_binary, X, _test_real_feature, _test_binary_feature, hypotheses_independent, fdr_level,
+            map_function
+        )
+
+    relevance_table = pd.concat([relevance_table, table_const], axis=0)
+
+    return relevance_table
+
+
+def _calculate_relevance_table_for_implicit_target(table_real, table_binary, X, test_real_feature, test_binary_feature,
+                                                   hypotheses_independent, fdr_level, map_function):
+    table_real['p_value'] = pd.Series(
+        map_function(test_real_feature, [X[feature] for feature in table_real.index]),
+        index=table_real.index
+    )
+    table_binary['p_value'] = pd.Series(
+        map_function(test_binary_feature, [X[feature] for feature in table_binary.index]),
+        index=table_binary.index
+    )
+    relevance_table = pd.concat([table_real, table_binary])
+    return benjamini_hochberg_test(relevance_table, hypotheses_independent, fdr_level)
+
+
+def infer_ml_task(y):
+    """
+    Infer the machine learning task to select for.
+    The result will be either `'regression'` or `'classification'`.
+    If the target vector only consists of integer typed values or objects, we assume the task is `'classification'`.
+    Else `'regression'`.
+
+    :param y: The target vector y.
+    :type y: pandas.Series
+    :return: 'classification' or 'regression'
+    :rtype: str
+    """
+    if y.dtype.kind in np.typecodes['AllInteger'] or y.dtype == np.object:
+        ml_task = 'classification'
+    else:
+        ml_task = 'regression'
+
+    _logger.warning('Infered {} as machine learning task'.format(ml_task))
+    return ml_task
+
+
+def combine_relevance_tables(relevance_tables):
+    """
+    Create a combined relevance table out of a list of relevance tables,
+    aggregating the p-values and the relevances.
+
+    :param relevance_tables: A list of relevance tables
+    :type relevance_tables: List[pd.DataFrame]
+    :return: The combined relevance table
+    :rtype: pandas.DataFrame
+    """
+    def _combine(a, b):
+        a.relevant |= b.relevant
+        a.p_value = a.p_value.combine(b.p_value, min, 1)
+        return a
+
+    return reduce(_combine, relevance_tables)
+
+
+def get_feature_type(feature_column):
+    """
+    For a given feature, determine if it is real, binary or constant.
+    Here binary means that only two unique values occur in the feature.
+
+    :param feature_column: The feature column
+    :type feature_column: pandas.Series
+    :return: 'constant', 'binary' or 'real'
+    """
+    n_unique_values = len(set(feature_column.values))
+    if n_unique_values == 1:
+        _logger.warning("[test_feature_significance] Feature {} is constant".format(feature_column.name))
+        return 'constant'
+    elif n_unique_values == 2:
+        return 'binary'
+    else:
+        return 'real'
```

### Comparing `tsfresh-0.8.1/tsfresh/feature_selection/selection.py` & `tsfresh-0.9.0/tsfresh/feature_selection/selection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,130 +1,147 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-"""
-This module contains the filtering process for the extracted features. The filtering procedure can also be used on
-other features that are not based on time series.
-"""
-
-from __future__ import absolute_import
-
-import pandas as pd
-import numpy as np
-from tsfresh import defaults
-from tsfresh.utilities.dataframe_functions import check_for_nans_in_columns
-from tsfresh.feature_selection.feature_selector import check_fs_sig_bh
-
-
-def select_features(X, y, test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
-                    test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
-                    test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
-                    test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
-                    fdr_level=defaults.FDR_LEVEL, hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
-                    n_processes=defaults.N_PROCESSES, chunksize=defaults.CHUNKSIZE):
-    """
-    Check the significance of all features (columns) of feature matrix X and return a possibly reduced feature matrix
-    only containing relevant features.
-
-    The feature matrix must be a pandas.DataFrame in the format:
-
-        +-------+-----------+-----------+-----+-----------+
-        | index | feature_1 | feature_2 | ... | feature_N |
-        +=======+===========+===========+=====+===========+
-        | A     | ...       | ...       | ... | ...       |
-        +-------+-----------+-----------+-----+-----------+
-        | B     | ...       | ...       | ... | ...       |
-        +-------+-----------+-----------+-----+-----------+
-        | ...   | ...       | ...       | ... | ...       |
-        +-------+-----------+-----------+-----+-----------+
-        | ...   | ...       | ...       | ... | ...       |
-        +-------+-----------+-----------+-----+-----------+
-        | ...   | ...       | ...       | ... | ...       |
-        +-------+-----------+-----------+-----+-----------+
-
-
-    Each column will be handled as a feature and tested for its significance to the target.
-
-    The target vector must be a pandas.Series or numpy.array in the form
-
-        +-------+--------+
-        | index | target |
-        +=======+========+
-        | A     | ...    |
-        +-------+--------+
-        | B     | ...    |
-        +-------+--------+
-        | .     | ...    |
-        +-------+--------+
-        | .     | ...    |
-        +-------+--------+
-
-    and must contain all id's that are in the feature matrix. If y is a numpy.array without index, it is assumed
-    that y has the same order and length than X and the rows correspond to each other.
-
-    Examples
-    ========
-
-    >>> from tsfresh.examples import load_robot_execution_failures
-    >>> from tsfresh import extract_features, select_features
-    >>> df, y = load_robot_execution_failures()
-    >>> X_extracted = extract_features(df, column_id='id', column_sort='time')
-    >>> X_selected = select_features(X_extracted, y)
-
-    :param X: Feature matrix in the format mentioned before which will be reduced to only the relevant features.
-              It can contain both binary or real-valued features at the same time.
-    :type X: pandas.DataFrame
-
-    :param y: Target vector which is needed to test which features are relevant. Can be binary or real-valued.
-    :type y: pandas.Series or numpy.ndarray
-
-    :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
-    :type test_for_binary_target_binary_feature: str
-
-    :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
-    :type test_for_binary_target_real_feature: str
-
-    :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
-    :type test_for_real_target_binary_feature: str
-
-    :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
-    :type test_for_real_target_real_feature: str
-
-    :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
-                      features among all created features.
-    :type fdr_level: float
-
-    :param hypotheses_independent: Can the significance of the features be assumed to be independent?
-                                   Normally, this should be set to False as the features are never
-                                   independent (e.g. mean and median)
-    :type hypotheses_independent: bool
-
-    :param n_processes: Number of processes to use during the p-value calculation
-    :type n_processes: int
-
-    :param chunksize: Size of the chunks submitted to the worker processes
-    :type chunksize: int
-
-    :return: The same DataFrame as X, but possibly with reduced number of columns ( = features).
-    :rtype: pandas.DataFrame
-
-    :raises: ``ValueError`` when the target vector does not fit to the feature matrix.
-    """
-    check_for_nans_in_columns(X)
-
-    if not isinstance(y, (pd.Series, np.ndarray)):
-        raise TypeError("The type of target vector y must be one of: pandas.Series, numpy.ndarray")
-
-    if len(X) < 2:
-        raise ValueError("X must contain at least two samples.")
-    elif isinstance(y, pd.Series) and not X.index.isin(y.index).all():
-        raise ValueError("Index of X must be a subset of y's index")
-    elif isinstance(y, np.ndarray):
-        if not len(y) >= len(X):
-            raise ValueError("Target vector y is shorter than feature matrix X")
-
-        y = pd.Series(y, index=X.index)
-
-    df_bh = check_fs_sig_bh(X, y, n_processes, chunksize, fdr_level, hypotheses_independent,
-                            test_for_binary_target_real_feature)
-
-    return X.loc[:, df_bh[df_bh.rejected].Feature]
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+"""
+This module contains the filtering process for the extracted features. The filtering procedure can also be used on
+other features that are not based on time series.
+"""
+
+from __future__ import absolute_import
+
+import logging
+import pandas as pd
+import numpy as np
+from tsfresh import defaults
+from tsfresh.utilities.dataframe_functions import check_for_nans_in_columns
+from tsfresh.feature_selection.relevance import calculate_relevance_table
+
+
+_logger = logging.getLogger(__name__)
+
+
+def select_features(X, y, test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
+                    test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
+                    test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
+                    test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
+                    fdr_level=defaults.FDR_LEVEL, hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
+                    n_jobs=defaults.N_PROCESSES, chunksize=defaults.CHUNKSIZE,
+                    ml_task='auto'):
+    """
+    Check the significance of all features (columns) of feature matrix X and return a possibly reduced feature matrix
+    only containing relevant features.
+
+    The feature matrix must be a pandas.DataFrame in the format:
+
+        +-------+-----------+-----------+-----+-----------+
+        | index | feature_1 | feature_2 | ... | feature_N |
+        +=======+===========+===========+=====+===========+
+        | A     | ...       | ...       | ... | ...       |
+        +-------+-----------+-----------+-----+-----------+
+        | B     | ...       | ...       | ... | ...       |
+        +-------+-----------+-----------+-----+-----------+
+        | ...   | ...       | ...       | ... | ...       |
+        +-------+-----------+-----------+-----+-----------+
+        | ...   | ...       | ...       | ... | ...       |
+        +-------+-----------+-----------+-----+-----------+
+        | ...   | ...       | ...       | ... | ...       |
+        +-------+-----------+-----------+-----+-----------+
+
+
+    Each column will be handled as a feature and tested for its significance to the target.
+
+    The target vector must be a pandas.Series or numpy.array in the form
+
+        +-------+--------+
+        | index | target |
+        +=======+========+
+        | A     | ...    |
+        +-------+--------+
+        | B     | ...    |
+        +-------+--------+
+        | .     | ...    |
+        +-------+--------+
+        | .     | ...    |
+        +-------+--------+
+
+    and must contain all id's that are in the feature matrix. If y is a numpy.array without index, it is assumed
+    that y has the same order and length than X and the rows correspond to each other.
+
+    Examples
+    ========
+
+    >>> from tsfresh.examples import load_robot_execution_failures
+    >>> from tsfresh import extract_features, select_features
+    >>> df, y = load_robot_execution_failures()
+    >>> X_extracted = extract_features(df, column_id='id', column_sort='time')
+    >>> X_selected = select_features(X_extracted, y)
+
+    :param X: Feature matrix in the format mentioned before which will be reduced to only the relevant features.
+              It can contain both binary or real-valued features at the same time.
+    :type X: pandas.DataFrame
+
+    :param y: Target vector which is needed to test which features are relevant. Can be binary or real-valued.
+    :type y: pandas.Series or numpy.ndarray
+
+    :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
+    :type test_for_binary_target_binary_feature: str
+
+    :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
+    :type test_for_binary_target_real_feature: str
+
+    :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
+    :type test_for_real_target_binary_feature: str
+
+    :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
+    :type test_for_real_target_real_feature: str
+
+    :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
+                      features among all created features.
+    :type fdr_level: float
+
+    :param hypotheses_independent: Can the significance of the features be assumed to be independent?
+                                   Normally, this should be set to False as the features are never
+                                   independent (e.g. mean and median)
+    :type hypotheses_independent: bool
+
+    :param n_jobs: Number of processes to use during the p-value calculation
+    :type n_jobs: int
+
+    :param chunksize: Size of the chunks submitted to the worker processes
+    :type chunksize: int
+
+    :param ml_task: The intended machine learning task. Either `'classification'`, `'regression'` or `'auto'`.
+                    Defaults to `'auto'`, meaning the intended task is inferred from `y`.
+                    If `y` has a boolean, integer or object dtype, the task is assumend to be classification,
+                    else regression.
+    :type ml_task: str
+
+    :return: The same DataFrame as X, but possibly with reduced number of columns ( = features).
+    :rtype: pandas.DataFrame
+
+    :raises: ``ValueError`` when the target vector does not fit to the feature matrix
+             or `ml_task` is not one of `'auto'`, `'classification'` or `'regression'`.
+    """
+    check_for_nans_in_columns(X)
+
+    if not isinstance(y, (pd.Series, np.ndarray)):
+        raise TypeError("The type of target vector y must be one of: pandas.Series, numpy.ndarray")
+
+    if len(X) < 2:
+        raise ValueError("X must contain at least two samples.")
+    elif isinstance(y, pd.Series) and not X.index.isin(y.index).all():
+        raise ValueError("Index of X must be a subset of y's index")
+    elif isinstance(y, np.ndarray):
+        if not len(y) >= len(X):
+            raise ValueError("Target vector y is shorter than feature matrix X")
+
+        y = pd.Series(y, index=X.index)
+
+    relevance_table = calculate_relevance_table(
+        X, y, ml_task=ml_task, n_jobs=n_jobs, chunksize=chunksize,
+        test_for_binary_target_real_feature=test_for_binary_target_real_feature,
+        fdr_level=fdr_level, hypotheses_independent=hypotheses_independent,
+    )
+
+    relevant_features = relevance_table[relevance_table.relevant].feature
+
+    return X.loc[:, relevant_features]
```

### Comparing `tsfresh-0.8.1/tsfresh/feature_selection/significance_tests.py` & `tsfresh-0.9.0/tsfresh/feature_selection/significance_tests.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/scripts/data.txt` & `tsfresh-0.9.0/tsfresh/scripts/data.txt`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/scripts/run_tsfresh.py` & `tsfresh-0.9.0/tsfresh/scripts/run_tsfresh.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/transformers/feature_augmenter.py` & `tsfresh-0.9.0/tsfresh/transformers/feature_augmenter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,204 +1,195 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-import pandas as pd
-from sklearn.base import BaseEstimator, TransformerMixin
-import tsfresh.defaults
-from tsfresh.feature_extraction import extract_features
-from tsfresh.utilities.dataframe_functions import restrict_input_to_index
-
-
-class FeatureAugmenter(BaseEstimator, TransformerMixin):
-    """
-    Sklearn-compatible estimator, for calculating and adding many features calculated from a given time series
-    to the data. Is is basically a wrapper around :func:`~tsfresh.feature_extraction.extract_features`.
-
-    The features include basic ones like min, max or median, and advanced features like fourier
-    transformations or statistical tests. For a list of all possible features, see the module
-    :mod:`~tsfresh.feature_extraction.feature_calculators`. The column name of each added feature contains the name
-    of the function of that module, which was used for the calculation.
-
-    For this estimator, two datasets play a crucial role:
-
-    1. the time series container with the timeseries data. This container (for the format see :ref:`data-formats-label`)
-       contains the data which is used for calculating the
-       features. It must be groupable by ids which are used to identify which feature should be attached to which row
-       in the second dataframe:
-
-    2. the input data, where the features will be added to.
-
-    Imagine the following situation: You want to classify 10 different financial shares and you have their development
-    in the last year as a time series. You would then start by creating features from the metainformation of the
-    shares, e.g. how long they were on the market etc. and filling up a table - the features of one stock in one row.
-
-    >>> df = pandas.DataFrame()
-    >>> # Fill in the information of the stocks
-    >>> df["started_since_days"] = 0 # add a feature
-
-    You can then extract all the features from the time development of the shares, by using this estimator:
-
-    >>> time_series = read_in_timeseries() # get the development of the shares
-    >>> from tsfresh.transformers import FeatureAugmenter
-    >>> augmenter = FeatureAugmenter()
-    >>> augmenter.set_timeseries_container(time_series)
-    >>> df_with_time_series_features = augmenter.transform(df)
-
-    The settings for the feature calculation can be controlled with the settings object. If you pass ``None``, the default
-    settings are used. Please refer to :class:`~tsfresh.feature_extraction.settings.ComprehensiveFCParameters` for
-    more information.
-
-    This estimator does not select the relevant features, but calculates and adds all of them to the DataFrame. See the
-    :class:`~tsfresh.transformers.relevant_feature_augmenter.RelevantFeatureAugmenter` for calculating and selecting
-    features.
-
-    For a description what the parameters column_id, column_sort, column_kind and column_value mean, please see
-    :mod:`~tsfresh.feature_extraction.extraction`.
-    """
-    def __init__(self, default_fc_parameters=None,
-                 kind_to_fc_parameters=None, column_id=None, column_sort=None,
-                 column_kind=None, column_value=None, timeseries_container=None,
-                 parallelization=None, chunksize=tsfresh.defaults.CHUNKSIZE,
-                 n_processes=tsfresh.defaults.N_PROCESSES, show_warnings=tsfresh.defaults.SHOW_WARNINGS,
-                 disable_progressbar=tsfresh.defaults.DISABLE_PROGRESSBAR,
-                 impute_function=tsfresh.defaults.IMPUTE_FUNCTION,
-                 profile=tsfresh.defaults.PROFILING,
-                 profiling_filename=tsfresh.defaults.PROFILING_FILENAME,
-                 profiling_sorting=tsfresh.defaults.PROFILING_SORTING
-                 ):
-        """
-        Create a new FeatureAugmenter instance.
-
-        :param settings: The extraction settings to use. Leave empty to use the default ones.
-        :type settings: tsfresh.feature_extraction.settings.ComprehensiveFCParameters
-
-        :param column_id: The column with the id. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_id: basestring
-        :param column_sort: The column with the sort data. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_sort: basestring
-        :param column_kind: The column with the kind data. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_kind: basestring
-        :param column_value: The column with the values. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_value: basestring
-
-        :param parallelization: Either ``'per_sample'`` or ``'per_kind'``   , see
-                            :func:`~tsfresh.feature_extraction.extraction._extract_features_parallel_per_sample`,
-                            :func:`~tsfresh.feature_extraction.extraction._extract_features_parallel_per_kind` and
-                            :ref:`parallelization-label` for details.
-                            Choosing None makes the algorithm look for the best parallelization technique by applying
-                            some general remarks.
-        :type parallelization: str
-
-        :param chunksize: The size of one chunk for the parallelisation
-        :type chunksize: None or int
-
-        :param n_processes: The number of processes to use for parallelisation.
-        :type n_processes: int
-
-        :param: show_warnings: Show warnings during the feature extraction (needed for debugging of calculators).
-        :type show_warnings: bool
-
-        :param disable_progressbar: Do not show a progressbar while doing the calculation.
-        :type disable_progressbar: bool
-
-        :param impute_function: None, if no imputing should happen or the function to call for imputing.
-        :type impute_function: None or function
-
-        :param profile: Turn on profiling during feature extraction
-        :type profile: bool
-
-        :param profiling_sorting: How to sort the profiling results (see the documentation of the profiling package for
-               more information)
-        :type profiling_sorting: basestring
-
-        :param profiling_filename: Where to save the profiling results.
-        :type profiling_filename: basestring
-        """
-        self.default_fc_parameters = default_fc_parameters
-        self.kind_to_fc_parameters = kind_to_fc_parameters
-
-        self.column_id = column_id
-        self.column_sort = column_sort
-        self.column_kind = column_kind
-        self.column_value = column_value
-
-        self.parallelization = parallelization
-        self.chunksize = chunksize
-        self.n_processes = n_processes
-        self.show_warnings = show_warnings
-        self.disable_progressbar = disable_progressbar
-        self.impute_function = impute_function
-        self.profile = profile
-        self.profiling_filename = profiling_filename
-        self.profiling_sorting = profiling_sorting
-
-        self.timeseries_container = timeseries_container
-
-    def set_timeseries_container(self, timeseries_container):
-        """
-        Set the timeseries, with which the features will be calculated. For a format of the time series container,
-        please refer to :mod:`~tsfresh.feature_extraction.extraction`. The timeseries must contain the same indices
-        as the later DataFrame, to which the features will be added (the one you will pass to :func:`~transform`). You
-        can call this function as often as you like, to change the timeseries later (e.g. if you want to extract for
-        different ids).
-
-        :param timeseries_container: The timeseries as a pandas.DataFrame or a dict. See
-            :mod:`~tsfresh.feature_extraction.extraction` for the format.
-        :type timeseries_container: pandas.DataFrame or dict
-        :return: None
-        :rtype: None
-        """
-        self.timeseries_container = timeseries_container
-
-    def fit(self, X=None, y=None):
-        """
-        The fit function is not needed for this estimator. It just does nothing and is here for compatibility reasons.
-
-        :param X: Unneeded.
-        :type X: Any
-
-        :param y: Unneeded.
-        :type y: Any
-
-        :return: The estimator instance itself
-        :rtype: FeatureAugmenter
-        """
-        return self
-
-    def transform(self, X):
-        """
-        Add the features calculated using the timeseries_container and add them to the corresponding rows in the input
-        pandas.DataFrame X.
-
-        To save some computing time, you should only include those time serieses in the container, that you
-        need. You can set the timeseries container with the method :func:`set_timeseries_container`.
-
-        :param X: the DataFrame to which the calculated timeseries features will be added. This is *not* the
-               dataframe with the timeseries itself.
-        :type X: pandas.DataFrame
-
-        :return: The input DataFrame, but with added features.
-        :rtype: pandas.DataFrame
-        """
-        if self.timeseries_container is None:
-            raise RuntimeError("You have to provide a time series using the set_timeseries_container function before.")
-
-        # Extract only features for the IDs in X.index
-        timeseries_container_X = restrict_input_to_index(self.timeseries_container, self.column_id, X.index)
-
-        extracted_features = extract_features(timeseries_container_X,
-                                              default_fc_parameters=self.default_fc_parameters,
-                                              kind_to_fc_parameters=self.kind_to_fc_parameters,
-                                              column_id=self.column_id, column_sort=self.column_sort,
-                                              column_kind=self.column_kind, column_value=self.column_value,
-                                              parallelization=self.parallelization, chunksize=self.chunksize,
-                                              n_processes=self.n_processes, show_warnings=self.show_warnings,
-                                              disable_progressbar=self.disable_progressbar,
-                                              impute_function=self.impute_function,
-                                              profile=self.profile,
-                                              profiling_filename=self.profiling_filename,
-                                              profiling_sorting=self.profiling_sorting)
-
-        X = pd.merge(X, extracted_features, left_index=True, right_index=True, how="left")
-
-        return X
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+import pandas as pd
+from sklearn.base import BaseEstimator, TransformerMixin
+import tsfresh.defaults
+from tsfresh.feature_extraction import extract_features
+from tsfresh.utilities.dataframe_functions import restrict_input_to_index
+
+
+class FeatureAugmenter(BaseEstimator, TransformerMixin):
+    """
+    Sklearn-compatible estimator, for calculating and adding many features calculated from a given time series
+    to the data. Is is basically a wrapper around :func:`~tsfresh.feature_extraction.extract_features`.
+
+    The features include basic ones like min, max or median, and advanced features like fourier
+    transformations or statistical tests. For a list of all possible features, see the module
+    :mod:`~tsfresh.feature_extraction.feature_calculators`. The column name of each added feature contains the name
+    of the function of that module, which was used for the calculation.
+
+    For this estimator, two datasets play a crucial role:
+
+    1. the time series container with the timeseries data. This container (for the format see :ref:`data-formats-label`)
+       contains the data which is used for calculating the
+       features. It must be groupable by ids which are used to identify which feature should be attached to which row
+       in the second dataframe:
+
+    2. the input data, where the features will be added to.
+
+    Imagine the following situation: You want to classify 10 different financial shares and you have their development
+    in the last year as a time series. You would then start by creating features from the metainformation of the
+    shares, e.g. how long they were on the market etc. and filling up a table - the features of one stock in one row.
+
+    >>> df = pandas.DataFrame()
+    >>> # Fill in the information of the stocks
+    >>> df["started_since_days"] = 0 # add a feature
+
+    You can then extract all the features from the time development of the shares, by using this estimator:
+
+    >>> time_series = read_in_timeseries() # get the development of the shares
+    >>> from tsfresh.transformers import FeatureAugmenter
+    >>> augmenter = FeatureAugmenter()
+    >>> augmenter.set_timeseries_container(time_series)
+    >>> df_with_time_series_features = augmenter.transform(df)
+
+    The settings for the feature calculation can be controlled with the settings object. If you pass ``None``, the default
+    settings are used. Please refer to :class:`~tsfresh.feature_extraction.settings.ComprehensiveFCParameters` for
+    more information.
+
+    This estimator does not select the relevant features, but calculates and adds all of them to the DataFrame. See the
+    :class:`~tsfresh.transformers.relevant_feature_augmenter.RelevantFeatureAugmenter` for calculating and selecting
+    features.
+
+    For a description what the parameters column_id, column_sort, column_kind and column_value mean, please see
+    :mod:`~tsfresh.feature_extraction.extraction`.
+    """
+    def __init__(self, default_fc_parameters=None,
+                 kind_to_fc_parameters=None, column_id=None, column_sort=None,
+                 column_kind=None, column_value=None, timeseries_container=None,
+                 chunksize=tsfresh.defaults.CHUNKSIZE,
+                 n_jobs=tsfresh.defaults.N_PROCESSES, show_warnings=tsfresh.defaults.SHOW_WARNINGS,
+                 disable_progressbar=tsfresh.defaults.DISABLE_PROGRESSBAR,
+                 impute_function=tsfresh.defaults.IMPUTE_FUNCTION,
+                 profile=tsfresh.defaults.PROFILING,
+                 profiling_filename=tsfresh.defaults.PROFILING_FILENAME,
+                 profiling_sorting=tsfresh.defaults.PROFILING_SORTING
+                 ):
+        """
+        Create a new FeatureAugmenter instance.
+
+        :param settings: The extraction settings to use. Leave empty to use the default ones.
+        :type settings: tsfresh.feature_extraction.settings.ComprehensiveFCParameters
+
+        :param column_id: The column with the id. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_id: basestring
+        :param column_sort: The column with the sort data. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_sort: basestring
+        :param column_kind: The column with the kind data. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_kind: basestring
+        :param column_value: The column with the values. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_value: basestring
+
+        :param n_jobs: The number of processes to use for parallelization. If zero, no parallelization is used.
+        :type n_jobs: int
+
+        :param chunksize: The size of one chunk for the parallelisation
+        :type chunksize: None or int
+
+        :param: show_warnings: Show warnings during the feature extraction (needed for debugging of calculators).
+        :type show_warnings: bool
+
+        :param disable_progressbar: Do not show a progressbar while doing the calculation.
+        :type disable_progressbar: bool
+
+        :param impute_function: None, if no imputing should happen or the function to call for imputing.
+        :type impute_function: None or function
+
+        :param profile: Turn on profiling during feature extraction
+        :type profile: bool
+
+        :param profiling_sorting: How to sort the profiling results (see the documentation of the profiling package for
+               more information)
+        :type profiling_sorting: basestring
+
+        :param profiling_filename: Where to save the profiling results.
+        :type profiling_filename: basestring
+        """
+        self.default_fc_parameters = default_fc_parameters
+        self.kind_to_fc_parameters = kind_to_fc_parameters
+
+        self.column_id = column_id
+        self.column_sort = column_sort
+        self.column_kind = column_kind
+        self.column_value = column_value
+
+        self.n_jobs = n_jobs
+        self.chunksize = chunksize
+        self.show_warnings = show_warnings
+        self.disable_progressbar = disable_progressbar
+        self.impute_function = impute_function
+        self.profile = profile
+        self.profiling_filename = profiling_filename
+        self.profiling_sorting = profiling_sorting
+
+        self.timeseries_container = timeseries_container
+
+    def set_timeseries_container(self, timeseries_container):
+        """
+        Set the timeseries, with which the features will be calculated. For a format of the time series container,
+        please refer to :mod:`~tsfresh.feature_extraction.extraction`. The timeseries must contain the same indices
+        as the later DataFrame, to which the features will be added (the one you will pass to :func:`~transform`). You
+        can call this function as often as you like, to change the timeseries later (e.g. if you want to extract for
+        different ids).
+
+        :param timeseries_container: The timeseries as a pandas.DataFrame or a dict. See
+            :mod:`~tsfresh.feature_extraction.extraction` for the format.
+        :type timeseries_container: pandas.DataFrame or dict
+        :return: None
+        :rtype: None
+        """
+        self.timeseries_container = timeseries_container
+
+    def fit(self, X=None, y=None):
+        """
+        The fit function is not needed for this estimator. It just does nothing and is here for compatibility reasons.
+
+        :param X: Unneeded.
+        :type X: Any
+
+        :param y: Unneeded.
+        :type y: Any
+
+        :return: The estimator instance itself
+        :rtype: FeatureAugmenter
+        """
+        return self
+
+    def transform(self, X):
+        """
+        Add the features calculated using the timeseries_container and add them to the corresponding rows in the input
+        pandas.DataFrame X.
+
+        To save some computing time, you should only include those time serieses in the container, that you
+        need. You can set the timeseries container with the method :func:`set_timeseries_container`.
+
+        :param X: the DataFrame to which the calculated timeseries features will be added. This is *not* the
+               dataframe with the timeseries itself.
+        :type X: pandas.DataFrame
+
+        :return: The input DataFrame, but with added features.
+        :rtype: pandas.DataFrame
+        """
+        if self.timeseries_container is None:
+            raise RuntimeError("You have to provide a time series using the set_timeseries_container function before.")
+
+        # Extract only features for the IDs in X.index
+        timeseries_container_X = restrict_input_to_index(self.timeseries_container, self.column_id, X.index)
+
+        extracted_features = extract_features(timeseries_container_X,
+                                              default_fc_parameters=self.default_fc_parameters,
+                                              kind_to_fc_parameters=self.kind_to_fc_parameters,
+                                              column_id=self.column_id, column_sort=self.column_sort,
+                                              column_kind=self.column_kind, column_value=self.column_value,
+                                              chunksize=self.chunksize,
+                                              n_jobs=self.n_jobs, show_warnings=self.show_warnings,
+                                              disable_progressbar=self.disable_progressbar,
+                                              impute_function=self.impute_function,
+                                              profile=self.profile,
+                                              profiling_filename=self.profiling_filename,
+                                              profiling_sorting=self.profiling_sorting)
+
+        X = pd.merge(X, extracted_features, left_index=True, right_index=True, how="left")
+
+        return X
```

### Comparing `tsfresh-0.8.1/tsfresh/transformers/feature_selector.py` & `tsfresh-0.9.0/tsfresh/transformers/feature_selector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,158 +1,167 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-
-import pandas as pd
-from tsfresh import defaults
-from sklearn.base import BaseEstimator, TransformerMixin
-from tsfresh.feature_selection.feature_selector import check_fs_sig_bh
-
-
-class FeatureSelector(BaseEstimator, TransformerMixin):
-    """
-    Sklearn-compatible estimator, for reducing the number of features in a dataset to only those,
-    that are relevant and significant to a given target. It is basically a wrapper around
-    :func:`~tsfresh.feature_selection.feature_selector.check_fs_sig_bh`.
-
-    The check is done by testing the hypothesis
-
-        :math:`H_0` = the Feature is not relevant and can not be added`
-
-    against
-
-        :math:`H_1` = the Feature is relevant and should be kept
-
-    using several statistical tests (depending on whether the feature or/and the target is binary
-    or not). Using the Benjamini Hochberg procedure, only features in :math:`H_0` are rejected.
-
-    This estimator - as most of the sklearn estimators - works in a two step procedure. First, it is fitted
-    on training data, where the target is known:
-
-    >>> import pandas as pd
-    >>> X_train, y_train = pd.DataFrame(), pd.Series() # fill in with your features and target
-    >>> from tsfresh.transformers import FeatureSelector
-    >>> selector = FeatureSelector()
-    >>> selector.fit(X_train, y_train)
-
-    In this example the list of relevant features is empty:
-    >>> selector.relevant_features
-    >>> []
-
-    The same holds for the feature importance:
-    >>> selector.feature_importances_
-    >>> array([], dtype=float64)
-
-    The estimator keeps track on those features, that were relevant in the training step. If you
-    apply the estimator after the training, it will delete all other features in the testing
-    data sample:
-
-    >>> X_test = pd.DataFrame()
-    >>> X_selected = selector.transform(X_test)
-
-    After that, X_selected will only contain the features that were relevant during the training.
-
-    If you are interested in more information on the features, you can look into the member
-    ``relevant_features`` after the fit.
-    """
-    def __init__(self, test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
-                 test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
-                 test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
-                 test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
-                 fdr_level=defaults.FDR_LEVEL, hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
-                 n_processes=defaults.N_PROCESSES, chunksize=defaults.CHUNKSIZE):
-        """
-        Create a new FeatureSelector instance.
-
-        :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
-        :type test_for_binary_target_binary_feature: str
-
-        :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
-        :type test_for_binary_target_real_feature: str
-
-        :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
-        :type test_for_real_target_binary_feature: str
-
-        :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
-        :type test_for_real_target_real_feature: str
-
-        :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
-                      features among all created features.
-        :type fdr_level: float
-
-        :param hypotheses_independent: Can the significance of the features be assumed to be independent?
-                                       Normally, this should be set to False as the features are never
-                                       independent (e.g. mean and median)
-        :type hypotheses_independent: bool
-
-        :param n_processes: Number of processes to use during the p-value calculation
-        :type n_processes: int
-
-        :param chunksize: Size of the chunks submitted to the worker processes
-        :type chunksize: int
-        """
-        self.relevant_features = None
-        self.feature_importances_ = None
-        self.p_values = None
-        self.features = None
-
-        self.test_for_binary_target_binary_feature = test_for_binary_target_binary_feature
-        self.test_for_binary_target_real_feature = test_for_binary_target_real_feature
-        self.test_for_real_target_binary_feature = test_for_real_target_binary_feature
-        self.test_for_real_target_real_feature = test_for_real_target_real_feature
-
-        self.fdr_level = fdr_level
-        self.hypotheses_independent = hypotheses_independent
-
-        self.n_processes = n_processes
-        self.chunksize = chunksize
-
-    def fit(self, X, y):
-        """
-        Extract the information, which of the features are relevent using the given target.
-
-        For more information, please see the :func:`~tsfresh.festure_selection.festure_selector.check_fs_sig_bh`
-        function. All columns in the input data sample are treated as feature. The index of all
-        rows in X must be present in y.
-
-        :param X: data sample with the features, which will be classified as relevant or not
-        :type X: pandas.DataFrame or numpy.array
-
-        :param y: target vecotr to be used, to classify the features
-        :type y: pandas.Series or numpy.array
-
-        :return: the fitted estimator with the information, which features are relevant
-        :rtype: FeatureSelector
-        """
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X.copy())
-
-        if not isinstance(y, pd.Series):
-            y = pd.Series(y.copy())
-
-        df_bh = check_fs_sig_bh(X, y, self.n_processes, self.chunksize,
-                                self.fdr_level, self.hypotheses_independent,
-                                self.test_for_binary_target_real_feature)
-        self.relevant_features = df_bh.loc[df_bh.rejected].Feature.tolist()
-        self.feature_importances_ = 1.0 - df_bh.p_value.values
-        self.p_values = df_bh.p_value.values
-        self.features = df_bh.Feature.tolist()
-
-        return self
-
-    def transform(self, X):
-        """
-        Delete all features, which were not relevant in the fit phase.
-
-        :param X: data sample with all features, which will be reduced to only those that are relevant
-        :type X: pandas.DataSeries or numpy.array
-
-        :return: same data sample as X, but with only the relevant features
-        :rtype: pandas.DataFrame or numpy.array
-        """
-        if self.relevant_features is None:
-            raise RuntimeError("You have to call fit before.")
-
-        if isinstance(X, pd.DataFrame):
-            return X.copy().loc[:, self.relevant_features]
-        else:
-            return X[:, self.relevant_features]
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+
+import pandas as pd
+from tsfresh import defaults
+from sklearn.base import BaseEstimator, TransformerMixin
+from tsfresh.feature_selection.relevance import calculate_relevance_table
+
+
+class FeatureSelector(BaseEstimator, TransformerMixin):
+    """
+    Sklearn-compatible estimator, for reducing the number of features in a dataset to only those,
+    that are relevant and significant to a given target. It is basically a wrapper around
+    :func:`~tsfresh.feature_selection.feature_selector.check_fs_sig_bh`.
+
+    The check is done by testing the hypothesis
+
+        :math:`H_0` = the Feature is not relevant and can not be added`
+
+    against
+
+        :math:`H_1` = the Feature is relevant and should be kept
+
+    using several statistical tests (depending on whether the feature or/and the target is binary
+    or not). Using the Benjamini Hochberg procedure, only features in :math:`H_0` are rejected.
+
+    This estimator - as most of the sklearn estimators - works in a two step procedure. First, it is fitted
+    on training data, where the target is known:
+
+    >>> import pandas as pd
+    >>> X_train, y_train = pd.DataFrame(), pd.Series() # fill in with your features and target
+    >>> from tsfresh.transformers import FeatureSelector
+    >>> selector = FeatureSelector()
+    >>> selector.fit(X_train, y_train)
+
+    In this example the list of relevant features is empty:
+    >>> selector.relevant_features
+    >>> []
+
+    The same holds for the feature importance:
+    >>> selector.feature_importances_
+    >>> array([], dtype=float64)
+
+    The estimator keeps track on those features, that were relevant in the training step. If you
+    apply the estimator after the training, it will delete all other features in the testing
+    data sample:
+
+    >>> X_test = pd.DataFrame()
+    >>> X_selected = selector.transform(X_test)
+
+    After that, X_selected will only contain the features that were relevant during the training.
+
+    If you are interested in more information on the features, you can look into the member
+    ``relevant_features`` after the fit.
+    """
+    def __init__(self, test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
+                 test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
+                 test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
+                 test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
+                 fdr_level=defaults.FDR_LEVEL, hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
+                 n_jobs=defaults.N_PROCESSES, chunksize=defaults.CHUNKSIZE, ml_task='auto'):
+        """
+        Create a new FeatureSelector instance.
+
+        :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
+        :type test_for_binary_target_binary_feature: str
+
+        :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
+        :type test_for_binary_target_real_feature: str
+
+        :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
+        :type test_for_real_target_binary_feature: str
+
+        :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
+        :type test_for_real_target_real_feature: str
+
+        :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
+                      features among all created features.
+        :type fdr_level: float
+
+        :param hypotheses_independent: Can the significance of the features be assumed to be independent?
+                                       Normally, this should be set to False as the features are never
+                                       independent (e.g. mean and median)
+        :type hypotheses_independent: bool
+
+        :param n_jobs: Number of processes to use during the p-value calculation
+        :type n_jobs: int
+
+        :param chunksize: Size of the chunks submitted to the worker processes
+        :type chunksize: int
+
+        :param ml_task: The intended machine learning task. Either `'classification'`, `'regression'` or `'auto'`.
+                    Defaults to `'auto'`, meaning the intended task is inferred from `y`.
+                    If `y` has a boolean, integer or object dtype, the task is assumend to be classification,
+                    else regression.
+        :type ml_task: str
+        """
+        self.relevant_features = None
+        self.feature_importances_ = None
+        self.p_values = None
+        self.features = None
+
+        self.test_for_binary_target_binary_feature = test_for_binary_target_binary_feature
+        self.test_for_binary_target_real_feature = test_for_binary_target_real_feature
+        self.test_for_real_target_binary_feature = test_for_real_target_binary_feature
+        self.test_for_real_target_real_feature = test_for_real_target_real_feature
+
+        self.fdr_level = fdr_level
+        self.hypotheses_independent = hypotheses_independent
+
+        self.n_jobs = n_jobs
+        self.chunksize = chunksize
+        self.ml_task = ml_task
+
+    def fit(self, X, y):
+        """
+        Extract the information, which of the features are relevent using the given target.
+
+        For more information, please see the :func:`~tsfresh.festure_selection.festure_selector.check_fs_sig_bh`
+        function. All columns in the input data sample are treated as feature. The index of all
+        rows in X must be present in y.
+
+        :param X: data sample with the features, which will be classified as relevant or not
+        :type X: pandas.DataFrame or numpy.array
+
+        :param y: target vector to be used, to classify the features
+        :type y: pandas.Series or numpy.array
+
+        :return: the fitted estimator with the information, which features are relevant
+        :rtype: FeatureSelector
+        """
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X.copy())
+
+        if not isinstance(y, pd.Series):
+            y = pd.Series(y.copy())
+
+        relevance_table = calculate_relevance_table(
+                                X, y, ml_task=self.ml_task, n_jobs=self.n_jobs,
+                                chunksize=self.chunksize, fdr_level=self.fdr_level,
+                                hypotheses_independent=self.hypotheses_independent,
+                                test_for_binary_target_real_feature=self.test_for_binary_target_real_feature)
+        self.relevant_features = relevance_table.loc[relevance_table.relevant].feature.tolist()
+        self.feature_importances_ = 1.0 - relevance_table.p_value.values
+        self.p_values = relevance_table.p_value.values
+        self.features = relevance_table.index.tolist()
+
+        return self
+
+    def transform(self, X):
+        """
+        Delete all features, which were not relevant in the fit phase.
+
+        :param X: data sample with all features, which will be reduced to only those that are relevant
+        :type X: pandas.DataSeries or numpy.array
+
+        :return: same data sample as X, but with only the relevant features
+        :rtype: pandas.DataFrame or numpy.array
+        """
+        if self.relevant_features is None:
+            raise RuntimeError("You have to call fit before.")
+
+        if isinstance(X, pd.DataFrame):
+            return X.copy().loc[:, self.relevant_features]
+        else:
+            return X[:, self.relevant_features]
```

### Comparing `tsfresh-0.8.1/tsfresh/transformers/per_column_imputer.py` & `tsfresh-0.9.0/tsfresh/transformers/per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh/transformers/relevant_feature_augmenter.py` & `tsfresh-0.9.0/tsfresh/transformers/relevant_feature_augmenter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,321 +1,314 @@
-# -*- coding: utf-8 -*-
-# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
-# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
-from functools import partial
-
-import pandas as pd
-from sklearn.base import BaseEstimator, TransformerMixin
-from tsfresh import defaults
-from tsfresh.feature_extraction.settings import from_columns
-from tsfresh.transformers.feature_augmenter import FeatureAugmenter
-from tsfresh.transformers.feature_selector import FeatureSelector
-from tsfresh.utilities.dataframe_functions import impute_dataframe_range, get_range_values_per_column
-
-
-# Pro: It offers more control
-# Contra: The Transformer is more than an Augmenter
-class RelevantFeatureAugmenter(BaseEstimator, TransformerMixin):
-    """
-    Sklearn-compatible estimator to calculate relevant features out of a time series and add them to a data sample.
-
-    As many other sklearn estimators, this estimator works in two steps:
-
-    In the fit phase, all possible time series features are calculated using the time series, that is set by the
-    set_timeseries_container function (if the features are not manually changed by handing in a
-    feature_extraction_settings object). Then, their significance and relevance to the target is computed using
-    statistical methods and only the relevant ones are selected using the Benjamini Hochberg procedure. These features
-    are stored internally.
-
-    In the transform step, the information on which features are relevant from the fit step is used and those features
-    are extracted from the time series. These extracted features are then added to the input data sample.
-
-    This estimator is a wrapper around most of the functionality in the tsfresh package. For more information on the
-    subtasks, please refer to the single modules and functions, which are:
-
-    * Settings for the feature extraction: :class:`~tsfresh.feature_extraction.settings.ComprehensiveFCParameters`
-    * Feature extraction method: :func:`~tsfresh.feature_extraction.extraction.extract_features`
-    * Extracted features: :mod:`~tsfresh.feature_extraction.feature_calculators`
-    * Feature selection: :func:`~tsfresh.feature_selection.feature_selector.check_fs_sig_bh`
-
-    This estimator works analogue to the :class:`~tsfresh.transformers.feature_augmenter.FeatureAugmenter` with
-    the difference that this estimator does only output and calculate the relevant features,
-    whereas the other outputs all features.
-
-    Also for this estimator, two datasets play a crucial role:
-
-    1. the time series container with the timeseries data. This container (for the format see
-       :mod:`~tsfresh.feature_extraction.extraction`) contains the data which is used for calculating the
-       features. It must be groupable by ids which are used to identify which feature should be attached to which row
-       in the second dataframe:
-
-    2. the input data, where the features will be added to.
-
-    Imagine the following situation: You want to classify 10 different financial shares and you have their development
-    in the last year as a time series. You would then start by creating features from the metainformation of the
-    shares, e.g. how long they were on the market etc. and filling up a table - the features of one stock in one row.
-
-    >>> # Fill in the information of the stocks and the target
-    >>> X_train, X_test, y_train = pd.DataFrame(), pd.DataFrame(), pd.Series()
-
-    You can then extract all the relevant features from the time development of the shares, by using this estimator:
-
-    >>> train_time_series, test_time_series = read_in_timeseries() # get the development of the shares
-    >>> from tsfresh.transformers import RelevantFeatureAugmenter
-    >>> augmenter = RelevantFeatureAugmenter()
-    >>> augmenter.set_timeseries_container(train_time_series)
-    >>> augmenter.fit(X_train, y_train)
-    >>> augmenter.set_timeseries_container(test_time_series)
-    >>> X_test_with_features = augmenter.transform(X_test)
-
-    X_test_with_features will then contain the same information as X_test (with all the meta information you have
-    probably added) plus some relevant time series features calculated on the time series you handed in.
-
-    Please keep in mind that the time series you hand in before fit or transform must contain data for the rows that are
-    present in X.
-
-    If your set filter_only_tsfresh_features to True, your manually-created features that were present in X_train (or
-    X_test) before using this estimator are not touched. Otherwise, also those features are evaluated and may be
-    rejected from the data sample, because they are irrelevant.
-
-    For a description what the parameters column_id, column_sort, column_kind and column_value mean, please see
-    :mod:`~tsfresh.feature_extraction.extraction`.
-
-    You can control the feature extraction in the fit step (the feature extraction in the transform step is done
-    automatically) as well as the feature selection in the fit step by handing in settings.
-    However, the default settings which are used if you pass no flags are often quite sensible.
-    """
-
-    def __init__(self,
-                 filter_only_tsfresh_features=True,
-                 default_fc_parameters=None,
-                 kind_to_fc_parameters=None,
-                 column_id=None, column_sort=None, column_kind=None, column_value=None,
-                 timeseries_container=None,
-                 parallelization=defaults.PARALLELISATION,
-                 chunksize=defaults.CHUNKSIZE,
-                 impute_function=defaults.IMPUTE_FUNCTION,
-                 n_processes=defaults.N_PROCESSES,
-                 show_warnings=defaults.SHOW_WARNINGS,
-                 disable_progressbar=defaults.DISABLE_PROGRESSBAR,
-                 profile=defaults.PROFILING,
-                 profiling_filename=defaults.PROFILING_FILENAME,
-                 profiling_sorting=defaults.PROFILING_SORTING,
-                 test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
-                 test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
-                 test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
-                 test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
-                 fdr_level=defaults.FDR_LEVEL,
-                 hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT):
-
-        """
-        Create a new RelevantFeatureAugmenter instance.
-
-        :param settings: The extraction settings to use. Leave empty to use the default ones.
-        :type settings: tsfresh.feature_extraction.settings.ExtendedFCParameters
-
-        :param filter_only_tsfresh_features: Whether to touch the manually-created features during feature selection or
-                                             not.
-        :type filter_only_tsfresh_features: bool
-        :param feature_selection_settings: The feature selection settings.
-        :type feature_selection_settings: tsfresh.feature_selection.settings.FeatureSelectionSettings
-        :param feature_extraction_settings: The feature extraction settings.
-        :type feature_selection_settings: tsfresh.feature_extraction.settings.ComprehensiveFCParameters
-        :param column_id: The column with the id. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_id: basestring
-        :param column_sort: The column with the sort data. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_sort: basestring
-        :param column_kind: The column with the kind data. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_kind: basestring
-        :param column_value: The column with the values. See :mod:`~tsfresh.feature_extraction.extraction`.
-        :type column_value: basestring
-
-        :param parallelization: Either ``'per_sample'`` or ``'per_kind'``   , see
-                            :func:`~tsfresh.feature_extraction.extraction._extract_features_parallel_per_sample`,
-                            :func:`~tsfresh.feature_extraction.extraction._extract_features_parallel_per_kind` and
-                            :ref:`parallelization-label` for details.
-                            Choosing None makes the algorithm look for the best parallelization technique by applying
-                            some general remarks.
-        :type parallelization: str
-
-        :param chunksize: The size of one chunk for the parallelisation
-        :type chunksize: None or int
-
-        :param n_processes: The number of processes to use for parallelisation.
-        :type n_processes: int
-
-        :param: show_warnings: Show warnings during the feature extraction (needed for debugging of calculators).
-        :type show_warnings: bool
-
-        :param disable_progressbar: Do not show a progressbar while doing the calculation.
-        :type disable_progressbar: bool
-
-        :param profile: Turn on profiling during feature extraction
-        :type profile: bool
-
-        :param profiling_sorting: How to sort the profiling results (see the documentation of the profiling package for
-               more information)
-        :type profiling_sorting: basestring
-
-        :param profiling_filename: Where to save the profiling results.
-        :type profiling_filename: basestring
-
-        :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
-        :type test_for_binary_target_binary_feature: str
-
-        :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
-        :type test_for_binary_target_real_feature: str
-
-        :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
-        :type test_for_real_target_binary_feature: str
-
-        :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
-        :type test_for_real_target_real_feature: str
-
-        :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
-                          features among all created features.
-        :type fdr_level: float
-
-        :param hypotheses_independent: Can the significance of the features be assumed to be independent?
-                                       Normally, this should be set to False as the features are never
-                                       independent (e.g. mean and median)
-        :type hypotheses_independent: bool
-        """
-
-        self.feature_extractor = FeatureAugmenter(column_id=column_id, column_sort=column_sort, column_kind=column_kind,
-                                                  column_value=column_value,
-                                                  default_fc_parameters=default_fc_parameters,
-                                                  kind_to_fc_parameters=kind_to_fc_parameters,
-                                                  parallelization=parallelization, chunksize=chunksize,
-                                                  n_processes=n_processes, show_warnings=show_warnings,
-                                                  disable_progressbar=disable_progressbar,
-                                                  impute_function=impute_function,
-                                                  profile=profile,
-                                                  profiling_filename=profiling_filename,
-                                                  profiling_sorting=profiling_sorting
-                                                  )
-
-        self.feature_selector = FeatureSelector(
-            test_for_binary_target_binary_feature=test_for_binary_target_binary_feature,
-            test_for_binary_target_real_feature=test_for_binary_target_real_feature,
-            test_for_real_target_binary_feature=test_for_real_target_binary_feature,
-            test_for_real_target_real_feature=test_for_real_target_real_feature,
-            fdr_level=fdr_level, hypotheses_independent=hypotheses_independent,
-            n_processes=n_processes, chunksize=chunksize
-        )
-
-        self.filter_only_tsfresh_features = filter_only_tsfresh_features
-        self.timeseries_container = timeseries_container
-
-    def set_timeseries_container(self, timeseries_container):
-        """
-        Set the timeseries, with which the features will be calculated. For a format of the time series container,
-        please refer to :mod:`~tsfresh.feature_extraction.extraction`. The timeseries must contain the same indices
-        as the later DataFrame, to which the features will be added (the one you will pass to :func:`~transform` or
-        :func:`~fit`). You can call this function as often as you like, to change the timeseries later
-        (e.g. if you want to extract for different ids).
-
-        :param timeseries_container: The timeseries as a pandas.DataFrame or a dict. See
-            :mod:`~tsfresh.feature_extraction.extraction` for the format.
-        :type timeseries_container: pandas.DataFrame or dict
-        :return: None
-        :rtype: None
-        """
-        self.timeseries_container = timeseries_container
-
-    def fit(self, X, y):
-        """
-        Use the given timeseries from :func:`~set_timeseries_container` and calculate features from it and add them
-        to the data sample X (which can contain other manually-designed features).
-
-        Then determine which of the features of X are relevant for the given target y.
-        Store those relevant features internally to only extract them in the transform step.
-
-        If filter_only_tsfresh_features is True, only reject newly, automatically added features. If it is False,
-        also look at the features that are already present in the DataFrame.
-
-        :param X: The data frame without the time series features. The index rows should be present in the timeseries
-           and in the target vector.
-        :type X: pandas.DataFrame or numpy.array
-
-        :param y: The target vector to define, which features are relevant.
-        :type y: pandas.Series or numpy.array
-
-        :return: the fitted estimator with the information, which features are relevant.
-        :rtype: RelevantFeatureAugmenter
-        """
-        if self.timeseries_container is None:
-            raise RuntimeError("You have to provide a time series using the set_timeseries_container function before.")
-
-        self.feature_extractor.set_timeseries_container(self.timeseries_container)
-
-        if self.filter_only_tsfresh_features:
-            # Do not merge the time series features to the old features
-            X_tmp = pd.DataFrame(index=X.index)
-        else:
-            X_tmp = X
-
-        X_augmented = self.feature_extractor.transform(X_tmp)
-
-        if self.feature_extractor.impute_function is impute_dataframe_range:
-            self.col_to_max, self.col_to_min, self.col_to_median = get_range_values_per_column(X_augmented)
-
-        self.feature_selector.fit(X_augmented, y)
-
-        return self
-
-    def transform(self, X):
-        """
-        After the fit step, it is known which features are relevant, Only extract those from the time series handed in
-        with the function :func:`~set_timeseries_container`.
-
-        If filter_only_tsfresh_features is False, also delete the irrelevant, already present features in the data frame.
-
-        :param X: the data sample to add the relevant (and delete the irrelevant) features to.
-        :type X: pandas.DataFrame or numpy.array
-
-        :return: a data sample with the same information as X, but with added relevant time series features and
-            deleted irrelevant information (only if filter_only_tsfresh_features is False).
-        :rtype: pandas.DataFrame
-        """
-        if self.feature_selector.relevant_features is None:
-            raise RuntimeError("You have to call fit before.")
-
-        if self.timeseries_container is None:
-            raise RuntimeError("You have to provide a time series using the set_timeseries_container function before.")
-
-        self.feature_extractor.set_timeseries_container(self.timeseries_container)
-
-        relevant_time_series_features = set(self.feature_selector.relevant_features) - set(pd.DataFrame(X).columns)
-        relevant_extraction_settings = from_columns(relevant_time_series_features)
-
-        # Set imputing strategy
-        if self.feature_extractor.impute_function is impute_dataframe_range:
-            self.feature_extractor.impute_function = partial(impute_dataframe_range,
-                                                             col_to_max=self.col_to_max,
-                                                             col_to_min=self.col_to_min,
-                                                             col_to_median=self.col_to_median)
-
-        relevant_feature_extractor = FeatureAugmenter(kind_to_fc_parameters=relevant_extraction_settings,
-                                                      default_fc_parameters={},
-                                                      column_id=self.feature_extractor.column_id,
-                                                      column_sort=self.feature_extractor.column_sort,
-                                                      column_kind=self.feature_extractor.column_kind,
-                                                      column_value=self.feature_extractor.column_value,
-                                                      parallelization=self.feature_extractor.parallelization,
-                                                      chunksize=self.feature_extractor.chunksize,
-                                                      n_processes=self.feature_extractor.n_processes,
-                                                      show_warnings=self.feature_extractor.show_warnings,
-                                                      disable_progressbar=self.feature_extractor.disable_progressbar,
-                                                      impute_function=self.feature_extractor.impute_function,
-                                                      profile=self.feature_extractor.profile,
-                                                      profiling_filename=self.feature_extractor.profiling_filename,
-                                                      profiling_sorting=self.feature_extractor.profiling_sorting)
-
-        relevant_feature_extractor.set_timeseries_container(self.feature_extractor.timeseries_container)
-
-        X_augmented = relevant_feature_extractor.transform(X)
-
-        if self.filter_only_tsfresh_features:
-            return X_augmented.copy().loc[:, self.feature_selector.relevant_features + X.columns.tolist()]
-        else:
-            return X_augmented.copy().loc[:, self.feature_selector.relevant_features]
+# -*- coding: utf-8 -*-
+# This file as well as the whole tsfresh package are licenced under the MIT licence (see the LICENCE.txt)
+# Maximilian Christ (maximilianchrist.com), Blue Yonder Gmbh, 2016
+from functools import partial
+
+import pandas as pd
+from sklearn.base import BaseEstimator, TransformerMixin
+from tsfresh import defaults
+from tsfresh.feature_extraction.settings import from_columns
+from tsfresh.transformers.feature_augmenter import FeatureAugmenter
+from tsfresh.transformers.feature_selector import FeatureSelector
+from tsfresh.utilities.dataframe_functions import impute_dataframe_range, get_range_values_per_column
+
+
+# Pro: It offers more control
+# Contra: The Transformer is more than an Augmenter
+class RelevantFeatureAugmenter(BaseEstimator, TransformerMixin):
+    """
+    Sklearn-compatible estimator to calculate relevant features out of a time series and add them to a data sample.
+
+    As many other sklearn estimators, this estimator works in two steps:
+
+    In the fit phase, all possible time series features are calculated using the time series, that is set by the
+    set_timeseries_container function (if the features are not manually changed by handing in a
+    feature_extraction_settings object). Then, their significance and relevance to the target is computed using
+    statistical methods and only the relevant ones are selected using the Benjamini Hochberg procedure. These features
+    are stored internally.
+
+    In the transform step, the information on which features are relevant from the fit step is used and those features
+    are extracted from the time series. These extracted features are then added to the input data sample.
+
+    This estimator is a wrapper around most of the functionality in the tsfresh package. For more information on the
+    subtasks, please refer to the single modules and functions, which are:
+
+    * Settings for the feature extraction: :class:`~tsfresh.feature_extraction.settings.ComprehensiveFCParameters`
+    * Feature extraction method: :func:`~tsfresh.feature_extraction.extraction.extract_features`
+    * Extracted features: :mod:`~tsfresh.feature_extraction.feature_calculators`
+    * Feature selection: :func:`~tsfresh.feature_selection.feature_selector.check_fs_sig_bh`
+
+    This estimator works analogue to the :class:`~tsfresh.transformers.feature_augmenter.FeatureAugmenter` with
+    the difference that this estimator does only output and calculate the relevant features,
+    whereas the other outputs all features.
+
+    Also for this estimator, two datasets play a crucial role:
+
+    1. the time series container with the timeseries data. This container (for the format see
+       :mod:`~tsfresh.feature_extraction.extraction`) contains the data which is used for calculating the
+       features. It must be groupable by ids which are used to identify which feature should be attached to which row
+       in the second dataframe:
+
+    2. the input data, where the features will be added to.
+
+    Imagine the following situation: You want to classify 10 different financial shares and you have their development
+    in the last year as a time series. You would then start by creating features from the metainformation of the
+    shares, e.g. how long they were on the market etc. and filling up a table - the features of one stock in one row.
+
+    >>> # Fill in the information of the stocks and the target
+    >>> X_train, X_test, y_train = pd.DataFrame(), pd.DataFrame(), pd.Series()
+
+    You can then extract all the relevant features from the time development of the shares, by using this estimator:
+
+    >>> train_time_series, test_time_series = read_in_timeseries() # get the development of the shares
+    >>> from tsfresh.transformers import RelevantFeatureAugmenter
+    >>> augmenter = RelevantFeatureAugmenter()
+    >>> augmenter.set_timeseries_container(train_time_series)
+    >>> augmenter.fit(X_train, y_train)
+    >>> augmenter.set_timeseries_container(test_time_series)
+    >>> X_test_with_features = augmenter.transform(X_test)
+
+    X_test_with_features will then contain the same information as X_test (with all the meta information you have
+    probably added) plus some relevant time series features calculated on the time series you handed in.
+
+    Please keep in mind that the time series you hand in before fit or transform must contain data for the rows that are
+    present in X.
+
+    If your set filter_only_tsfresh_features to True, your manually-created features that were present in X_train (or
+    X_test) before using this estimator are not touched. Otherwise, also those features are evaluated and may be
+    rejected from the data sample, because they are irrelevant.
+
+    For a description what the parameters column_id, column_sort, column_kind and column_value mean, please see
+    :mod:`~tsfresh.feature_extraction.extraction`.
+
+    You can control the feature extraction in the fit step (the feature extraction in the transform step is done
+    automatically) as well as the feature selection in the fit step by handing in settings.
+    However, the default settings which are used if you pass no flags are often quite sensible.
+    """
+
+    def __init__(self,
+                 filter_only_tsfresh_features=True,
+                 default_fc_parameters=None,
+                 kind_to_fc_parameters=None,
+                 column_id=None, column_sort=None, column_kind=None, column_value=None,
+                 timeseries_container=None,
+                 chunksize=defaults.CHUNKSIZE,
+                 n_jobs=defaults.N_PROCESSES,
+                 show_warnings=defaults.SHOW_WARNINGS,
+                 disable_progressbar=defaults.DISABLE_PROGRESSBAR,
+                 profile=defaults.PROFILING,
+                 profiling_filename=defaults.PROFILING_FILENAME,
+                 profiling_sorting=defaults.PROFILING_SORTING,
+                 test_for_binary_target_binary_feature=defaults.TEST_FOR_BINARY_TARGET_BINARY_FEATURE,
+                 test_for_binary_target_real_feature=defaults.TEST_FOR_BINARY_TARGET_REAL_FEATURE,
+                 test_for_real_target_binary_feature=defaults.TEST_FOR_REAL_TARGET_BINARY_FEATURE,
+                 test_for_real_target_real_feature=defaults.TEST_FOR_REAL_TARGET_REAL_FEATURE,
+                 fdr_level=defaults.FDR_LEVEL,
+                 hypotheses_independent=defaults.HYPOTHESES_INDEPENDENT,
+                 ml_task='auto'):
+
+        """
+        Create a new RelevantFeatureAugmenter instance.
+
+        :param settings: The extraction settings to use. Leave empty to use the default ones.
+        :type settings: tsfresh.feature_extraction.settings.ExtendedFCParameters
+
+        :param filter_only_tsfresh_features: Whether to touch the manually-created features during feature selection or
+                                             not.
+        :type filter_only_tsfresh_features: bool
+        :param feature_selection_settings: The feature selection settings.
+        :type feature_selection_settings: tsfresh.feature_selection.settings.FeatureSelectionSettings
+        :param feature_extraction_settings: The feature extraction settings.
+        :type feature_selection_settings: tsfresh.feature_extraction.settings.ComprehensiveFCParameters
+        :param column_id: The column with the id. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_id: basestring
+        :param column_sort: The column with the sort data. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_sort: basestring
+        :param column_kind: The column with the kind data. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_kind: basestring
+        :param column_value: The column with the values. See :mod:`~tsfresh.feature_extraction.extraction`.
+        :type column_value: basestring
+
+        :param chunksize: The size of one chunk for the parallelisation
+        :type chunksize: None or int
+
+        :param n_jobs: The number of processes to use for parallelization. If zero, no parallelization is used.
+        :type n_jobs: int
+
+        :param: show_warnings: Show warnings during the feature extraction (needed for debugging of calculators).
+        :type show_warnings: bool
+
+        :param disable_progressbar: Do not show a progressbar while doing the calculation.
+        :type disable_progressbar: bool
+
+        :param profile: Turn on profiling during feature extraction
+        :type profile: bool
+
+        :param profiling_sorting: How to sort the profiling results (see the documentation of the profiling package for
+               more information)
+        :type profiling_sorting: basestring
+
+        :param profiling_filename: Where to save the profiling results.
+        :type profiling_filename: basestring
+
+        :param test_for_binary_target_binary_feature: Which test to be used for binary target, binary feature (currently unused)
+        :type test_for_binary_target_binary_feature: str
+
+        :param test_for_binary_target_real_feature: Which test to be used for binary target, real feature
+        :type test_for_binary_target_real_feature: str
+
+        :param test_for_real_target_binary_feature: Which test to be used for real target, binary feature (currently unused)
+        :type test_for_real_target_binary_feature: str
+
+        :param test_for_real_target_real_feature: Which test to be used for real target, real feature (currently unused)
+        :type test_for_real_target_real_feature: str
+
+        :param fdr_level: The FDR level that should be respected, this is the theoretical expected percentage of irrelevant
+                          features among all created features.
+        :type fdr_level: float
+
+        :param hypotheses_independent: Can the significance of the features be assumed to be independent?
+                                       Normally, this should be set to False as the features are never
+                                       independent (e.g. mean and median)
+        :type hypotheses_independent: bool
+
+        :param ml_task: The intended machine learning task. Either `'classification'`, `'regression'` or `'auto'`.
+                    Defaults to `'auto'`, meaning the intended task is inferred from `y`.
+                    If `y` has a boolean, integer or object dtype, the task is assumend to be classification,
+                    else regression.
+        :type ml_task: str
+        """
+
+        self.feature_extractor = FeatureAugmenter(column_id=column_id, column_sort=column_sort, column_kind=column_kind,
+                                                  column_value=column_value,
+                                                  default_fc_parameters=default_fc_parameters,
+                                                  kind_to_fc_parameters=kind_to_fc_parameters,
+                                                  chunksize=chunksize,
+                                                  n_jobs=n_jobs, show_warnings=show_warnings,
+                                                  disable_progressbar=disable_progressbar,
+                                                  profile=profile,
+                                                  profiling_filename=profiling_filename,
+                                                  profiling_sorting=profiling_sorting
+                                                  )
+
+        self.feature_selector = FeatureSelector(
+            test_for_binary_target_binary_feature=test_for_binary_target_binary_feature,
+            test_for_binary_target_real_feature=test_for_binary_target_real_feature,
+            test_for_real_target_binary_feature=test_for_real_target_binary_feature,
+            test_for_real_target_real_feature=test_for_real_target_real_feature,
+            fdr_level=fdr_level, hypotheses_independent=hypotheses_independent,
+            n_jobs=n_jobs, chunksize=chunksize, ml_task=ml_task
+        )
+
+        self.filter_only_tsfresh_features = filter_only_tsfresh_features
+        self.timeseries_container = timeseries_container
+
+    def set_timeseries_container(self, timeseries_container):
+        """
+        Set the timeseries, with which the features will be calculated. For a format of the time series container,
+        please refer to :mod:`~tsfresh.feature_extraction.extraction`. The timeseries must contain the same indices
+        as the later DataFrame, to which the features will be added (the one you will pass to :func:`~transform` or
+        :func:`~fit`). You can call this function as often as you like, to change the timeseries later
+        (e.g. if you want to extract for different ids).
+
+        :param timeseries_container: The timeseries as a pandas.DataFrame or a dict. See
+            :mod:`~tsfresh.feature_extraction.extraction` for the format.
+        :type timeseries_container: pandas.DataFrame or dict
+        :return: None
+        :rtype: None
+        """
+        self.timeseries_container = timeseries_container
+
+    def fit(self, X, y):
+        """
+        Use the given timeseries from :func:`~set_timeseries_container` and calculate features from it and add them
+        to the data sample X (which can contain other manually-designed features).
+
+        Then determine which of the features of X are relevant for the given target y.
+        Store those relevant features internally to only extract them in the transform step.
+
+        If filter_only_tsfresh_features is True, only reject newly, automatically added features. If it is False,
+        also look at the features that are already present in the DataFrame.
+
+        :param X: The data frame without the time series features. The index rows should be present in the timeseries
+           and in the target vector.
+        :type X: pandas.DataFrame or numpy.array
+
+        :param y: The target vector to define, which features are relevant.
+        :type y: pandas.Series or numpy.array
+
+        :return: the fitted estimator with the information, which features are relevant.
+        :rtype: RelevantFeatureAugmenter
+        """
+        if self.timeseries_container is None:
+            raise RuntimeError("You have to provide a time series using the set_timeseries_container function before.")
+
+        self.feature_extractor.set_timeseries_container(self.timeseries_container)
+
+        if self.filter_only_tsfresh_features:
+            # Do not merge the time series features to the old features
+            X_tmp = pd.DataFrame(index=X.index)
+        else:
+            X_tmp = X
+
+        X_augmented = self.feature_extractor.transform(X_tmp)
+
+        self.col_to_max, self.col_to_min, self.col_to_median = get_range_values_per_column(X_augmented)
+        X_augmented = impute_dataframe_range(X_augmented, col_to_max=self.col_to_max, col_to_median=self.col_to_median,
+                                             col_to_min=self.col_to_min)
+
+        self.feature_selector.fit(X_augmented, y)
+
+        return self
+
+    def transform(self, X):
+        """
+        After the fit step, it is known which features are relevant, Only extract those from the time series handed in
+        with the function :func:`~set_timeseries_container`.
+
+        If filter_only_tsfresh_features is False, also delete the irrelevant, already present features in the data frame.
+
+        :param X: the data sample to add the relevant (and delete the irrelevant) features to.
+        :type X: pandas.DataFrame or numpy.array
+
+        :return: a data sample with the same information as X, but with added relevant time series features and
+            deleted irrelevant information (only if filter_only_tsfresh_features is False).
+        :rtype: pandas.DataFrame
+        """
+        if self.feature_selector.relevant_features is None:
+            raise RuntimeError("You have to call fit before.")
+
+        if self.timeseries_container is None:
+            raise RuntimeError("You have to provide a time series using the set_timeseries_container function before.")
+
+        self.feature_extractor.set_timeseries_container(self.timeseries_container)
+
+        relevant_time_series_features = set(self.feature_selector.relevant_features) - set(pd.DataFrame(X).columns)
+        relevant_extraction_settings = from_columns(relevant_time_series_features)
+
+        # Set imputing strategy
+        impute_function = partial(impute_dataframe_range, col_to_max=self.col_to_max,
+                                  col_to_min=self.col_to_min, col_to_median=self.col_to_median)
+
+        relevant_feature_extractor = FeatureAugmenter(kind_to_fc_parameters=relevant_extraction_settings,
+                                                      default_fc_parameters={},
+                                                      column_id=self.feature_extractor.column_id,
+                                                      column_sort=self.feature_extractor.column_sort,
+                                                      column_kind=self.feature_extractor.column_kind,
+                                                      column_value=self.feature_extractor.column_value,
+                                                      chunksize=self.feature_extractor.chunksize,
+                                                      n_jobs=self.feature_extractor.n_jobs,
+                                                      show_warnings=self.feature_extractor.show_warnings,
+                                                      disable_progressbar=self.feature_extractor.disable_progressbar,
+                                                      impute_function=impute_function,
+                                                      profile=self.feature_extractor.profile,
+                                                      profiling_filename=self.feature_extractor.profiling_filename,
+                                                      profiling_sorting=self.feature_extractor.profiling_sorting)
+
+        relevant_feature_extractor.set_timeseries_container(self.feature_extractor.timeseries_container)
+
+        X_augmented = relevant_feature_extractor.transform(X)
+
+        if self.filter_only_tsfresh_features:
+            return X_augmented.copy().loc[:, self.feature_selector.relevant_features + X.columns.tolist()]
+        else:
+            return X_augmented.copy().loc[:, self.feature_selector.relevant_features]
```

### Comparing `tsfresh-0.8.1/tsfresh/utilities/profiling.py` & `tsfresh-0.9.0/tsfresh/utilities/profiling.py`

 * *Files identical despite different names*

### Comparing `tsfresh-0.8.1/tsfresh.egg-info/PKG-INFO` & `tsfresh-0.9.0/tsfresh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tsfresh
-Version: 0.8.1
+Version: 0.9.0
 Summary: tsfresh extracts relevant characteristics from time series
 Home-page: https://github.com/blue-yonder/tsfresh
 Author: Maximilian Christ, Nils Braun, Julius Neuffer
 Author-email: max.christ@me.com
 License: MIT
 Description: |Documentation Status| |Build Status| |Coverage Status| |license|
         |Gitter chat| |py27 status| |py352 status|
```

### Comparing `tsfresh-0.8.1/tsfresh.egg-info/SOURCES.txt` & `tsfresh-0.9.0/tsfresh.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .coveragerc
 .travis.yml
 AUTHORS.rst
 CHANGES.rst
 LICENSE.txt
 README.md
 README.rst
-notebooks-requirements.txt
 pypi_index.zip
 rdocs-requirements.txt
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 .github/ISSUE_TEMPLATE.md
@@ -28,54 +27,64 @@
 docs/api/tsfresh.feature_selection.rst
 docs/api/tsfresh.rst
 docs/api/tsfresh.transformers.rst
 docs/api/tsfresh.utilities.rst
 docs/images/feature_extraction_process_20160815_mc_1.png
 docs/images/introduction_ts_exa.png
 docs/images/introduction_ts_exa_features.png
+docs/images/rolling_mechanism_1.png
+docs/images/rolling_mechanism_2.png
+docs/images/rolling_mechanism_drawio_template.xml
 docs/images/ts_example_robot_failures_fail.png
 docs/images/ts_example_robot_failures_nofail.png
 docs/text/data_formats.rst
 docs/text/faq.rst
 docs/text/feature_calculation.rst
 docs/text/feature_extraction_settings.rst
 docs/text/feature_filtering.rst
+docs/text/forecasting.rst
 docs/text/how_to_add_custom_feature.rst
 docs/text/how_to_contribute.rst
 docs/text/introduction.rst
 docs/text/parallelization.rst
 docs/text/quick_start.rst
-docs/text/rolling.rst
 docs/text/sklearn_transformers.rst
 notebooks/basic_pipeline_example.ipynb
 notebooks/compare-runtimes-of-feature-calculators.ipynb
 notebooks/friedrich_coefficients.ipynb
 notebooks/human_activity_recognition_multi_class_example.ipynb
+notebooks/inspect_dft_features.ipynb
 notebooks/pipeline_with_two_datasets.ipynb
 notebooks/robot_failure_example.ipynb
 notebooks/the-fc_parameters-extraction-dictionary.ipynb
+notebooks/timeseries_forecasting_basic_example.ipynb
+notebooks/timeseries_forecasting_google_stock.ipynb
 tests/__init__.py
 tests/fixtures.py
 tests/test_feature_significance.py
+tests/test_notebooks.py
 tests/test_relevant_feature_extraction.py
 tests/examples/test_driftbif_simulation.py
 tests/examples/test_har_dataset.py
 tests/examples/test_robot_execution_failures.py
 tests/feature_extraction/test_extraction.py
 tests/feature_extraction/test_feature_calculations.py
 tests/feature_extraction/test_settings.py
-tests/feature_selection/test_feature_selectors.py
+tests/feature_selection/test_checks.py
+tests/feature_selection/test_relevance.py
 tests/feature_selection/test_selection.py
+tests/feature_selection/test_significance_tests.py
 tests/scripts/test_run_tsfresh.py
 tests/transformers/test_feature_augmenter.py
 tests/transformers/test_feature_selector.py
 tests/transformers/test_full_pipeline.py
 tests/transformers/test_per_column_imputer.py
-tests/transformers/test_relevant_feature_extractor.py
+tests/transformers/test_relevant_feature_augmenter.py
 tests/utilities/test_dataframe_functions.py
+tests/utilities/test_string_manipilations.py
 tsfresh/__init__.py
 tsfresh/defaults.py
 tsfresh.egg-info/PKG-INFO
 tsfresh.egg-info/SOURCES.txt
 tsfresh.egg-info/dependency_links.txt
 tsfresh.egg-info/entry_points.txt
 tsfresh.egg-info/not-zip-safe
@@ -89,21 +98,24 @@
 tsfresh/examples/robot_execution_failures.py
 tsfresh/examples/test_tsfresh_baseline_dataset.py
 tsfresh/feature_extraction/__init__.py
 tsfresh/feature_extraction/extraction.py
 tsfresh/feature_extraction/feature_calculators.py
 tsfresh/feature_extraction/settings.py
 tsfresh/feature_selection/__init__.py
-tsfresh/feature_selection/feature_selector.py
+tsfresh/feature_selection/benjamini_hochberg_test.py
+tsfresh/feature_selection/relevance.py
 tsfresh/feature_selection/selection.py
 tsfresh/feature_selection/significance_tests.py
 tsfresh/scripts/__init__.py
 tsfresh/scripts/data.txt
 tsfresh/scripts/run_tsfresh.py
+tsfresh/scripts/test_timing.py
 tsfresh/transformers/__init__.py
 tsfresh/transformers/feature_augmenter.py
 tsfresh/transformers/feature_selector.py
 tsfresh/transformers/per_column_imputer.py
 tsfresh/transformers/relevant_feature_augmenter.py
 tsfresh/utilities/__init__.py
 tsfresh/utilities/dataframe_functions.py
-tsfresh/utilities/profiling.py
+tsfresh/utilities/profiling.py
+tsfresh/utilities/string_manipulation.py
```

