# Comparing `tmp/femr-0.1.7.tar.gz` & `tmp/femr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femr-0.1.7.tar", last modified: Fri Apr 28 19:27:40 2023, max compression
+gzip compressed data, was "femr-0.1.8.tar", last modified: Tue May  2 01:40:14 2023, max compression
```

## Comparing `femr-0.1.7.tar` & `femr-0.1.8.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.112164 femr-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 19:27:29.000000 femr-0.1.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.072163 femr-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.076163 femr-0.1.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 19:27:29.000000 femr-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 19:27:29.000000 femr-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.080164 femr-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-28 19:27:29.000000 femr-0.1.7/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-28 19:27:29.000000 femr-0.1.7/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 19:27:29.000000 femr-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 19:27:29.000000 femr-0.1.7/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 19:27:29.000000 femr-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-28 19:27:29.000000 femr-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-28 19:27:40.112164 femr-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-28 19:27:29.000000 femr-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 19:27:29.000000 femr-0.1.7/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.092164 femr-0.1.7/native/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-28 19:27:29.000000 femr-0.1.7/native/.bazelrc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 19:27:29.000000 femr-0.1.7/native/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 19:27:29.000000 femr-0.1.7/native/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-28 19:27:29.000000 femr-0.1.7/native/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-28 19:27:29.000000 femr-0.1.7/native/WORKSPACE
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-28 19:27:29.000000 femr-0.1.7/native/backupbazelrc
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-28 19:27:29.000000 femr-0.1.7/native/civil_day_caster.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-28 19:27:29.000000 femr-0.1.7/native/clmbr_dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 19:27:29.000000 femr-0.1.7/native/compute_statistics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-28 19:27:29.000000 femr-0.1.7/native/constdb.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 19:27:29.000000 femr-0.1.7/native/constdb.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-28 19:27:29.000000 femr-0.1.7/native/convert_dictionary_formats.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-28 19:27:29.000000 femr-0.1.7/native/count_codes_and_values.cc
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 19:27:29.000000 femr-0.1.7/native/count_codes_and_values.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-28 19:27:29.000000 femr-0.1.7/native/count_codes_and_values_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-28 19:27:29.000000 femr-0.1.7/native/cpu_jax_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-28 19:27:29.000000 femr-0.1.7/native/create_dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-28 19:27:29.000000 femr-0.1.7/native/create_dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-04-28 19:27:29.000000 femr-0.1.7/native/create_survival_dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 19:27:29.000000 femr-0.1.7/native/create_survival_dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-28 19:27:29.000000 femr-0.1.7/native/csv.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-28 19:27:29.000000 femr-0.1.7/native/csv.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-28 19:27:29.000000 femr-0.1.7/native/csv_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    44062 2023-04-28 19:27:29.000000 femr-0.1.7/native/database.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-04-28 19:27:29.000000 femr-0.1.7/native/database.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-28 19:27:29.000000 femr-0.1.7/native/database_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-28 19:27:29.000000 femr-0.1.7/native/database_test_helper.cc
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-28 19:27:29.000000 femr-0.1.7/native/database_test_helper.hh
--rw-r--r--   0 runner    (1001) docker     (123)    50034 2023-04-28 19:27:29.000000 femr-0.1.7/native/dataloader_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 19:27:29.000000 femr-0.1.7/native/dataloader_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-04-28 19:27:29.000000 femr-0.1.7/native/datasets_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 19:27:29.000000 femr-0.1.7/native/datasets_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-28 19:27:29.000000 femr-0.1.7/native/dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-28 19:27:29.000000 femr-0.1.7/native/dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-28 19:27:29.000000 femr-0.1.7/native/dictionary_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-28 19:27:29.000000 femr-0.1.7/native/embedding_dot.cu
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-28 19:27:29.000000 femr-0.1.7/native/embedding_dot.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-28 19:27:29.000000 femr-0.1.7/native/exp_mean.cu
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-28 19:27:29.000000 femr-0.1.7/native/exp_mean.hh
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 19:27:29.000000 femr-0.1.7/native/extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-28 19:27:29.000000 femr-0.1.7/native/extension_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-28 19:27:29.000000 femr-0.1.7/native/filesystem_caster.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-28 19:27:29.000000 femr-0.1.7/native/flatmap.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-28 19:27:29.000000 femr-0.1.7/native/gather_scatter.cu
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-28 19:27:29.000000 femr-0.1.7/native/gather_scatter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 19:27:29.000000 femr-0.1.7/native/jax_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 19:27:29.000000 femr-0.1.7/native/jax_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-28 19:27:29.000000 femr-0.1.7/native/join_csvs.cc
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 19:27:29.000000 femr-0.1.7/native/join_csvs.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-28 19:27:29.000000 femr-0.1.7/native/join_csvs_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    33436 2023-04-28 19:27:29.000000 femr-0.1.7/native/local_attention.cu
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-28 19:27:29.000000 femr-0.1.7/native/local_attention.hh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 19:27:29.000000 femr-0.1.7/native/malloc_trim.hh
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 19:27:29.000000 femr-0.1.7/native/metrics_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 19:27:29.000000 femr-0.1.7/native/metrics_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-28 19:27:29.000000 femr-0.1.7/native/npy.hh
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 19:27:29.000000 femr-0.1.7/native/parse_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 19:27:29.000000 femr-0.1.7/native/parse_utils.hh
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-28 19:27:29.000000 femr-0.1.7/native/prepare_all.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-28 19:27:29.000000 femr-0.1.7/native/prepare_notes_for_tokenization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-28 19:27:29.000000 femr-0.1.7/native/register_iterable.hh
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 19:27:29.000000 femr-0.1.7/native/simple_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-28 19:27:29.000000 femr-0.1.7/native/stat_utils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-04-28 19:27:29.000000 femr-0.1.7/native/survival.hh
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-04-28 19:27:29.000000 femr-0.1.7/native/survival_metrics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 19:27:29.000000 femr-0.1.7/native/survival_metrics.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-28 19:27:29.000000 femr-0.1.7/native/survival_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 19:27:29.000000 femr-0.1.7/native/thread_utils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-28 19:27:29.000000 femr-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:27:40.112164 femr-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-28 19:27:29.000000 femr-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.072163 femr-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.092164 femr-0.1.7/src/femr/
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.096164 femr-0.1.7/src/femr/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/datasets/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/datasets/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.096164 femr-0.1.7/src/femr/etl_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/etl_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/etl_pipelines/omop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/etl_pipelines/sickkids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/etl_pipelines/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/etl_pipelines/stanford.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.096164 femr-0.1.7/src/femr/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/extension/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/extension/datasets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/extension/jax.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.100164 femr-0.1.7/src/femr/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/extractors/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/extractors/omop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.100164 femr-0.1.7/src/femr/featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/featurizers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/featurizers/featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/featurizers/featurizers_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.100164 femr-0.1.7/src/femr/labelers/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/labelers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/labelers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/labelers/omop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/labelers/omop_inpatient_admissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/labelers/omop_lab_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.100164 femr-0.1.7/src/femr/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.104164 femr-0.1.7/src/femr/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/models/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/models/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/models/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.104164 femr-0.1.7/src/femr/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/transforms/notes.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/transforms/sickkids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-04-28 19:27:29.000000 femr-0.1.7/src/femr/transforms/stanford.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.096164 femr-0.1.7/src/femr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-28 19:27:40.000000 femr-0.1.7/src/femr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-28 19:27:40.000000 femr-0.1.7/src/femr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:27:40.000000 femr-0.1.7/src/femr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 19:27:40.000000 femr-0.1.7/src/femr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:27:39.000000 femr-0.1.7/src/femr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 19:27:40.000000 femr-0.1.7/src/femr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 19:27:40.000000 femr-0.1.7/src/femr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.104164 femr-0.1.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.104164 femr-0.1.7/tests/featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-28 19:27:29.000000 femr-0.1.7/tests/featurizers/test_OnlineStatistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-04-28 19:27:29.000000 femr-0.1.7/tests/featurizers/test_featurizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.108164 femr-0.1.7/tests/labelers/
--rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-04-28 19:27:29.000000 femr-0.1.7/tests/labelers/test_CodeLabelers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-04-28 19:27:29.000000 femr-0.1.7/tests/labelers/test_InpatientAdmissionLabelers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-28 19:27:29.000000 femr-0.1.7/tests/labelers/test_LabValueLabelers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-28 19:27:29.000000 femr-0.1.7/tests/labelers/test_LabeledPatients.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 19:27:29.000000 femr-0.1.7/tests/labelers/test_NLabelerPerPatient.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 19:27:29.000000 femr-0.1.7/tests/labelers/test_OpioidOverdoseLabeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-28 19:27:29.000000 femr-0.1.7/tests/labelers/test_TimeHorizonEventLabeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 19:27:29.000000 femr-0.1.7/tests/test_csvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-28 19:27:29.000000 femr-0.1.7/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-28 19:27:29.000000 femr-0.1.7/tests/test_jax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-28 19:27:29.000000 femr-0.1.7/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-28 19:27:29.000000 femr-0.1.7/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-28 19:27:29.000000 femr-0.1.7/tests/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.076163 femr-0.1.7/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.108164 femr-0.1.7/tools/omop/
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-28 19:27:29.000000 femr-0.1.7/tools/omop/normalize_visit_detail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.108164 femr-0.1.7/tools/stanford/
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-28 19:27:29.000000 femr-0.1.7/tools/stanford/download_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-28 19:27:29.000000 femr-0.1.7/tools/stanford/flowsheet_cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:27:40.112164 femr-0.1.7/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-04-28 19:27:29.000000 femr-0.1.7/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-28 19:27:29.000000 femr-0.1.7/tutorials/1_run_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-28 19:27:29.000000 femr-0.1.7/tutorials/2_train_baseline_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-28 19:27:29.000000 femr-0.1.7/tutorials/3_run_text_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-28 19:27:29.000000 femr-0.1.7/tutorials/4_train_clmbr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-28 19:27:29.000000 femr-0.1.7/tutorials/Simple FEMR Format.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-28 19:27:29.000000 femr-0.1.7/tutorials/mimic_etl_tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.133796 femr-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 01:40:04.000000 femr-0.1.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.105795 femr-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.109796 femr-0.1.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-02 01:40:04.000000 femr-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-02 01:40:04.000000 femr-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.109796 femr-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-02 01:40:04.000000 femr-0.1.8/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-02 01:40:04.000000 femr-0.1.8/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 01:40:04.000000 femr-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-02 01:40:04.000000 femr-0.1.8/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-02 01:40:04.000000 femr-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-02 01:40:04.000000 femr-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-05-02 01:40:14.133796 femr-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-05-02 01:40:04.000000 femr-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 01:40:04.000000 femr-0.1.8/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.121796 femr-0.1.8/native/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-02 01:40:04.000000 femr-0.1.8/native/.bazelrc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 01:40:04.000000 femr-0.1.8/native/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 01:40:04.000000 femr-0.1.8/native/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-02 01:40:04.000000 femr-0.1.8/native/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-02 01:40:04.000000 femr-0.1.8/native/WORKSPACE
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-02 01:40:04.000000 femr-0.1.8/native/backupbazelrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-02 01:40:04.000000 femr-0.1.8/native/civil_day_caster.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-02 01:40:04.000000 femr-0.1.8/native/clmbr_dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-02 01:40:04.000000 femr-0.1.8/native/compute_statistics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-05-02 01:40:04.000000 femr-0.1.8/native/constdb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-02 01:40:04.000000 femr-0.1.8/native/constdb.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-02 01:40:04.000000 femr-0.1.8/native/convert_dictionary_formats.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-02 01:40:04.000000 femr-0.1.8/native/count_codes_and_values.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 01:40:04.000000 femr-0.1.8/native/count_codes_and_values.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-02 01:40:04.000000 femr-0.1.8/native/count_codes_and_values_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-02 01:40:04.000000 femr-0.1.8/native/cpu_jax_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-02 01:40:04.000000 femr-0.1.8/native/create_dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 01:40:04.000000 femr-0.1.8/native/create_dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-02 01:40:04.000000 femr-0.1.8/native/create_survival_dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 01:40:04.000000 femr-0.1.8/native/create_survival_dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-02 01:40:04.000000 femr-0.1.8/native/csv.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-02 01:40:04.000000 femr-0.1.8/native/csv.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-02 01:40:04.000000 femr-0.1.8/native/csv_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    44062 2023-05-02 01:40:04.000000 femr-0.1.8/native/database.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-05-02 01:40:04.000000 femr-0.1.8/native/database.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-02 01:40:04.000000 femr-0.1.8/native/database_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-02 01:40:04.000000 femr-0.1.8/native/database_test_helper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-02 01:40:04.000000 femr-0.1.8/native/database_test_helper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    50034 2023-05-02 01:40:04.000000 femr-0.1.8/native/dataloader_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 01:40:04.000000 femr-0.1.8/native/dataloader_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-02 01:40:04.000000 femr-0.1.8/native/datasets_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 01:40:04.000000 femr-0.1.8/native/datasets_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-02 01:40:04.000000 femr-0.1.8/native/dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-02 01:40:04.000000 femr-0.1.8/native/dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-02 01:40:04.000000 femr-0.1.8/native/dictionary_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-02 01:40:04.000000 femr-0.1.8/native/embedding_dot.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-02 01:40:04.000000 femr-0.1.8/native/embedding_dot.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-02 01:40:04.000000 femr-0.1.8/native/exp_mean.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-02 01:40:04.000000 femr-0.1.8/native/exp_mean.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-02 01:40:04.000000 femr-0.1.8/native/extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-02 01:40:04.000000 femr-0.1.8/native/extension_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-02 01:40:04.000000 femr-0.1.8/native/filesystem_caster.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-02 01:40:04.000000 femr-0.1.8/native/flatmap.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-02 01:40:04.000000 femr-0.1.8/native/gather_scatter.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 01:40:04.000000 femr-0.1.8/native/gather_scatter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-02 01:40:04.000000 femr-0.1.8/native/jax_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 01:40:04.000000 femr-0.1.8/native/jax_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-02 01:40:04.000000 femr-0.1.8/native/join_csvs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-02 01:40:04.000000 femr-0.1.8/native/join_csvs.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-02 01:40:04.000000 femr-0.1.8/native/join_csvs_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    33436 2023-05-02 01:40:04.000000 femr-0.1.8/native/local_attention.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 01:40:04.000000 femr-0.1.8/native/local_attention.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 01:40:04.000000 femr-0.1.8/native/malloc_trim.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-02 01:40:04.000000 femr-0.1.8/native/metrics_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 01:40:04.000000 femr-0.1.8/native/metrics_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-05-02 01:40:04.000000 femr-0.1.8/native/npy.hh
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 01:40:04.000000 femr-0.1.8/native/parse_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-02 01:40:04.000000 femr-0.1.8/native/parse_utils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-02 01:40:04.000000 femr-0.1.8/native/prepare_all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-02 01:40:04.000000 femr-0.1.8/native/prepare_notes_for_tokenization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-02 01:40:04.000000 femr-0.1.8/native/register_iterable.hh
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 01:40:04.000000 femr-0.1.8/native/simple_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-02 01:40:04.000000 femr-0.1.8/native/stat_utils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-02 01:40:04.000000 femr-0.1.8/native/survival.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-05-02 01:40:04.000000 femr-0.1.8/native/survival_metrics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 01:40:04.000000 femr-0.1.8/native/survival_metrics.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-02 01:40:04.000000 femr-0.1.8/native/survival_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-02 01:40:04.000000 femr-0.1.8/native/thread_utils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-02 01:40:04.000000 femr-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 01:40:14.133796 femr-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-02 01:40:04.000000 femr-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.105795 femr-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.121796 femr-0.1.8/src/femr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.121796 femr-0.1.8/src/femr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/datasets/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/datasets/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.125796 femr-0.1.8/src/femr/etl_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/etl_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/etl_pipelines/omop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/etl_pipelines/sickkids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/etl_pipelines/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/etl_pipelines/stanford.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.125796 femr-0.1.8/src/femr/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/extension/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/extension/datasets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/extension/jax.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.125796 femr-0.1.8/src/femr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/extractors/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/extractors/omop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.125796 femr-0.1.8/src/femr/featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/featurizers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/featurizers/featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/featurizers/featurizers_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.125796 femr-0.1.8/src/femr/labelers/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/labelers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/labelers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/labelers/omop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/labelers/omop_inpatient_admissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/labelers/omop_lab_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.125796 femr-0.1.8/src/femr/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.129796 femr-0.1.8/src/femr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/models/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/models/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/models/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.129796 femr-0.1.8/src/femr/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/transforms/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/transforms/sickkids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-02 01:40:04.000000 femr-0.1.8/src/femr/transforms/stanford.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.121796 femr-0.1.8/src/femr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-05-02 01:40:14.000000 femr-0.1.8/src/femr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-02 01:40:14.000000 femr-0.1.8/src/femr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:40:14.000000 femr-0.1.8/src/femr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 01:40:14.000000 femr-0.1.8/src/femr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:40:13.000000 femr-0.1.8/src/femr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 01:40:14.000000 femr-0.1.8/src/femr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 01:40:14.000000 femr-0.1.8/src/femr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.129796 femr-0.1.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.129796 femr-0.1.8/tests/featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-02 01:40:04.000000 femr-0.1.8/tests/featurizers/test_OnlineStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-05-02 01:40:04.000000 femr-0.1.8/tests/featurizers/test_featurizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.133796 femr-0.1.8/tests/labelers/
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-05-02 01:40:04.000000 femr-0.1.8/tests/labelers/test_CodeLabelers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-05-02 01:40:04.000000 femr-0.1.8/tests/labelers/test_InpatientAdmissionLabelers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-05-02 01:40:04.000000 femr-0.1.8/tests/labelers/test_LabValueLabelers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-02 01:40:04.000000 femr-0.1.8/tests/labelers/test_LabeledPatients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-02 01:40:04.000000 femr-0.1.8/tests/labelers/test_NLabelerPerPatient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-02 01:40:04.000000 femr-0.1.8/tests/labelers/test_OpioidOverdoseLabeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-05-02 01:40:04.000000 femr-0.1.8/tests/labelers/test_TimeHorizonEventLabeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-02 01:40:04.000000 femr-0.1.8/tests/test_csvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-02 01:40:04.000000 femr-0.1.8/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-02 01:40:04.000000 femr-0.1.8/tests/test_jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-02 01:40:04.000000 femr-0.1.8/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-02 01:40:04.000000 femr-0.1.8/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-02 01:40:04.000000 femr-0.1.8/tests/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.105795 femr-0.1.8/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.133796 femr-0.1.8/tools/omop/
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-05-02 01:40:04.000000 femr-0.1.8/tools/omop/normalize_visit_detail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.133796 femr-0.1.8/tools/stanford/
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-02 01:40:04.000000 femr-0.1.8/tools/stanford/download_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-05-02 01:40:04.000000 femr-0.1.8/tools/stanford/flowsheet_cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:40:14.133796 femr-0.1.8/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-02 01:40:04.000000 femr-0.1.8/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-02 01:40:04.000000 femr-0.1.8/tutorials/1_run_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-02 01:40:04.000000 femr-0.1.8/tutorials/2_train_baseline_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-05-02 01:40:04.000000 femr-0.1.8/tutorials/3_run_text_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-02 01:40:04.000000 femr-0.1.8/tutorials/4_train_clmbr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-02 01:40:04.000000 femr-0.1.8/tutorials/Simple FEMR Format.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-05-02 01:40:04.000000 femr-0.1.8/tutorials/mimic_etl_tutorial.py
```

### Comparing `femr-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md` & `femr-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `femr-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/.github/workflows/build.yaml` & `femr-0.1.8/.github/workflows/build.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   build_wheels:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: true
       matrix:
         os: ["ubuntu-latest", "macos-12"]
         python-version: ["3.10"]
-        version: ["cpu", "cuda"]
+        version: ["cpu", "cuda", "old_cpu"]
         exclude:
           - os: macos-12
             version: cuda
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
@@ -28,14 +28,23 @@
       uses: pypa/cibuildwheel@v2.12.2
       if: matrix.version == 'cpu' && matrix.os == 'ubuntu-latest'
       env:
         CIBW_BEFORE_ALL_LINUX: bash build/linux_setup.sh
         CIBW_ARCHS_LINUX: x86_64
         CIBW_SKIP: '*-musllinux_*'
 
+    - name: Build wheels old cpu linux
+      uses: pypa/cibuildwheel@v2.12.2
+      if: matrix.version == 'old_cpu' && matrix.os == 'ubuntu-latest'
+      env:
+        CIBW_ENVIRONMENT: DISABLE_CPU_ARCH=1
+        CIBW_BEFORE_ALL_LINUX: bash build/linux_setup_old.sh
+        CIBW_ARCHS_LINUX: x86_64
+        CIBW_SKIP: '*-musllinux_*'
+
     - name: Build wheels cpu mac
       uses: pypa/cibuildwheel@v2.12.2
       if: matrix.version == 'cpu' && matrix.os == 'macos-12'
       env:
         CIBW_ENVIRONMENT: MACOSX_DEPLOYMENT_TARGET=10.14
         CIBW_ARCHS_MACOS: x86_64 arm64
```

### Comparing `femr-0.1.7/.github/workflows/tests.yaml` & `femr-0.1.8/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/.mypy.ini` & `femr-0.1.8/.mypy.ini`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/.pre-commit-config.yaml` & `femr-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/LICENSE` & `femr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/PKG-INFO` & `femr-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Framework for Electronic Medical Records. A python package for building models using EHR data.
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: models
 License-File: LICENSE
```

### Comparing `femr-0.1.7/README.md` & `femr-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/.bazelrc` & `femr-0.1.8/native/.bazelrc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/BUILD` & `femr-0.1.8/native/BUILD`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/WORKSPACE` & `femr-0.1.8/native/WORKSPACE`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/backupbazelrc` & `femr-0.1.8/native/backupbazelrc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/civil_day_caster.hh` & `femr-0.1.8/native/civil_day_caster.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/clmbr_dictionary.hh` & `femr-0.1.8/native/clmbr_dictionary.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/compute_statistics.cc` & `femr-0.1.8/native/compute_statistics.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/constdb.cc` & `femr-0.1.8/native/constdb.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/constdb.hh` & `femr-0.1.8/native/constdb.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/convert_dictionary_formats.cc` & `femr-0.1.8/native/convert_dictionary_formats.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/count_codes_and_values.cc` & `femr-0.1.8/native/count_codes_and_values.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/count_codes_and_values_test.cc` & `femr-0.1.8/native/count_codes_and_values_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/create_dictionary.cc` & `femr-0.1.8/native/create_dictionary.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/create_survival_dictionary.cc` & `femr-0.1.8/native/create_survival_dictionary.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/csv.cc` & `femr-0.1.8/native/csv.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/csv.hh` & `femr-0.1.8/native/csv.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/csv_test.cc` & `femr-0.1.8/native/csv_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/database.cc` & `femr-0.1.8/native/database.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/database.hh` & `femr-0.1.8/native/database.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/database_test.cc` & `femr-0.1.8/native/database_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/database_test_helper.cc` & `femr-0.1.8/native/database_test_helper.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/dataloader_extension.cc` & `femr-0.1.8/native/dataloader_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/datasets_extension.cc` & `femr-0.1.8/native/datasets_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/dictionary.cc` & `femr-0.1.8/native/dictionary.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/dictionary.hh` & `femr-0.1.8/native/dictionary.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/dictionary_test.cc` & `femr-0.1.8/native/dictionary_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/embedding_dot.cu` & `femr-0.1.8/native/embedding_dot.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/embedding_dot.hh` & `femr-0.1.8/native/embedding_dot.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/exp_mean.cu` & `femr-0.1.8/native/exp_mean.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/extension_test.py` & `femr-0.1.8/native/extension_test.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/filesystem_caster.hh` & `femr-0.1.8/native/filesystem_caster.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/flatmap.hh` & `femr-0.1.8/native/flatmap.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/gather_scatter.cu` & `femr-0.1.8/native/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/jax_extension.cc` & `femr-0.1.8/native/jax_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/join_csvs.cc` & `femr-0.1.8/native/join_csvs.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/join_csvs.hh` & `femr-0.1.8/native/join_csvs.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/join_csvs_test.cc` & `femr-0.1.8/native/join_csvs_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/local_attention.cu` & `femr-0.1.8/native/local_attention.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/local_attention.hh` & `femr-0.1.8/native/local_attention.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/metrics_extension.cc` & `femr-0.1.8/native/metrics_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/npy.hh` & `femr-0.1.8/native/npy.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/parse_utils.hh` & `femr-0.1.8/native/parse_utils.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/prepare_all.sh` & `femr-0.1.8/native/prepare_all.sh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/prepare_notes_for_tokenization.cc` & `femr-0.1.8/native/prepare_notes_for_tokenization.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/register_iterable.hh` & `femr-0.1.8/native/register_iterable.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/stat_utils.hh` & `femr-0.1.8/native/stat_utils.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/survival.hh` & `femr-0.1.8/native/survival.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/survival_metrics.cc` & `femr-0.1.8/native/survival_metrics.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/survival_metrics.hh` & `femr-0.1.8/native/survival_metrics.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/survival_test.cc` & `femr-0.1.8/native/survival_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/native/thread_utils.hh` & `femr-0.1.8/native/thread_utils.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/pyproject.toml` & `femr-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "tqdm >= 4.60.0",
     "zstandard >= 0.18",
     "icecream == 2.1.3",
     "nptyping == 2.4.1",
     "msgpack >= 1.0.5",
 ]
 requires-python=">3.9"
-version = "0.1.7"
+version = "0.1.8"
 
 [project.scripts]
 
 etl_stanford_omop = "femr.etl_pipelines.stanford:etl_starr_omop_program"
 etl_generic_omop = "femr.etl_pipelines.omop:etl_generic_omop_program"
 etl_simple_femr = "femr.etl_pipelines.simple:etl_simple_femr_program"
 etl_sickkids_omop = "femr.etl_pipelines.sickkids:etl_sk_omop_program"
```

### Comparing `femr-0.1.7/setup.py` & `femr-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,20 @@
 
             if has_nvcc():
                 extra_args.extend(["--//:cuda=enabled"])
 
             if source_env.get("MACOSX_DEPLOYMENT_TARGET"):
                 extra_args.extend(["--macos_minimum_os", source_env["MACOSX_DEPLOYMENT_TARGET"]])
 
-            if not can_build_simple(sourcedir=ext.sourcedir, env=env, bazel_extra_args=bazel_extra_args):
+            if source_env.get("DISABLE_CPU_ARCH") or not can_build_simple(sourcedir=ext.sourcedir, env=env, bazel_extra_args=bazel_extra_args):
                 bazel_extra_args.extend(["--noworkspace_rc", "--bazelrc=backupbazelrc"])
                 assert can_build_simple(
                     sourcedir=ext.sourcedir, env=env, bazel_extra_args=bazel_extra_args
                 ), "Cannot build C++ extension"
-            
+
             subprocess.run(
                 args=["bazel", "clean", "--expunge"],
                 cwd=ext.sourcedir,
                 env=env,
                 check=True,
             )
```

### Comparing `femr-0.1.7/src/femr/__init__.py` & `femr-0.1.8/src/femr/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/datasets/__init__.py` & `femr-0.1.8/src/femr/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/datasets/fileio.py` & `femr-0.1.8/src/femr/datasets/fileio.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/datasets/types.py` & `femr-0.1.8/src/femr/datasets/types.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/etl_pipelines/omop.py` & `femr-0.1.8/src/femr/etl_pipelines/omop.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/etl_pipelines/sickkids.py` & `femr-0.1.8/src/femr/etl_pipelines/sickkids.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/etl_pipelines/simple.py` & `femr-0.1.8/src/femr/etl_pipelines/simple.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,14 +55,19 @@
             event = RawEvent(
                 start=datetime.datetime.fromisoformat(row["start"]),
                 concept_id=concept_map[row["code"]],
                 value=row["value"],
             )
             for k, v in row.items():
                 if k not in ("start", "code", "value", "patient_id"):
+                    if v == "":
+                        v = None
+                    elif k == "end":
+                        v = datetime.datetime.fromisoformat(v)
+
                     setattr(event, k, v)
 
             writer.add_event(int(row["patient_id"]), event)
 
 
 def etl_simple_femr_program() -> None:
     """Extract data from an generic OMOP source to create a femr PatientDatabase."""
@@ -90,14 +95,21 @@
     parser.add_argument(
         "--num_threads",
         type=int,
         help="The number of threads to use",
         default=1,
     )
 
+    parser.add_argument(
+        "--athena_download",
+        type=str,
+        help="An optional athena download to use for ontologies",
+        default=None,
+    )
+
     args = parser.parse_args()
 
     soft, hard = resource.getrlimit(resource.RLIMIT_NOFILE)
     resource.setrlimit(resource.RLIMIT_NOFILE, (hard, hard))
 
     args.target_location = os.path.abspath(args.target_location)
     args.temp_location = os.path.abspath(args.temp_location)
@@ -137,37 +149,61 @@
 
             concept_ids = set()
             with multiprocessing.Pool(args.num_threads) as pool:
                 for f_concepts in pool.imap_unordered(get_concept_ids_from_file, input_files):
                     concept_ids |= f_concepts
 
             os.mkdir(omop_dir)
-            concept_id_map = {}
             with open(os.path.join(omop_dir, "concept.csv"), "w") as f:
+                concept_id_map = {}
                 writer = csv.DictWriter(
                     f, ["concept_id", "concept_name", "vocabulary_id", "standard_concept", "concept_code"]
                 )
+
                 writer.writeheader()
+                if args.athena_download:
+                    with open(os.path.join(args.athena_download, "CONCEPT.csv"), "r") as f:
+                        reader = csv.DictReader(f, delimiter="\t")
+                        for row in reader:
+                            del row["invalid_reason"]
+                            del row["domain_id"]
+                            del row["valid_end_date"]
+                            del row["concept_class_id"]
+                            del row["valid_start_date"]
+                            writer.writerow(row)
+                            concept_id_map[f'{row["vocabulary_id"]}/{row["concept_code"]}'] = row["concept_id"]
+
                 for i, concept_id in enumerate(concept_ids):
-                    index = i + 1
+                    if concept_id in concept_id_map:
+                        continue
+                    index = i + 11_000_000_000
                     prefix_index = concept_id.index("/")
                     vocab = concept_id[:prefix_index]
                     code = concept_id[prefix_index + 1 :]
                     writer.writerow(
                         {
                             "concept_id": index,
                             "concept_name": concept_id,
                             "vocabulary_id": vocab,
                             "standard_concept": "",
                             "concept_code": code,
                         }
                     )
                     concept_id_map[concept_id] = index
 
-            os.mkdir(os.path.join(omop_dir, "concept_relationship"))
+            if args.athena_download:
+                with open(os.path.join(args.athena_download, "CONCEPT_RELATIONSHIP.csv"), "r") as f:
+                    with open(os.path.join(omop_dir, "concept_relationship.csv"), "w") as wf:
+                        reader = csv.DictReader(f, delimiter="\t")
+                        writer = csv.DictWriter(wf, fieldnames=reader.fieldnames)
+                        writer.writeheader()
+                        for row in reader:
+                            writer.writerow(row)
+            else:
+                os.mkdir(os.path.join(omop_dir, "concept_relationship"))
 
             event_collection = EventCollection(event_dir)
             with multiprocessing.Pool(args.num_threads) as pool:
                 tasks = [(fname, concept_id_map, event_collection) for fname in input_files]
                 for _ in pool.imap_unordered(convert_file_to_event_file, tasks):
                     pass
         else:
```

### Comparing `femr-0.1.7/src/femr/etl_pipelines/stanford.py` & `femr-0.1.8/src/femr/etl_pipelines/stanford.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/extension/datasets.pyi` & `femr-0.1.8/src/femr/extension/datasets.pyi`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/extractors/csv.py` & `femr-0.1.8/src/femr/extractors/csv.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/extractors/omop.py` & `femr-0.1.8/src/femr/extractors/omop.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/featurizers/__init__.py` & `femr-0.1.8/src/femr/featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/featurizers/core.py` & `femr-0.1.8/src/femr/featurizers/core.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/featurizers/featurizers.py` & `femr-0.1.8/src/femr/featurizers/featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/featurizers/featurizers_notes.py` & `femr-0.1.8/src/femr/featurizers/featurizers_notes.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/jax.py` & `femr-0.1.8/src/femr/jax.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/labelers/core.py` & `femr-0.1.8/src/femr/labelers/core.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/labelers/omop.py` & `femr-0.1.8/src/femr/labelers/omop.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/labelers/omop_inpatient_admissions.py` & `femr-0.1.8/src/femr/labelers/omop_inpatient_admissions.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/labelers/omop_lab_values.py` & `femr-0.1.8/src/femr/labelers/omop_lab_values.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/models/dataloader.py` & `femr-0.1.8/src/femr/models/dataloader.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/models/scripts.py` & `femr-0.1.8/src/femr/models/scripts.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/models/transformer.py` & `femr-0.1.8/src/femr/models/transformer.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/transforms/__init__.py` & `femr-0.1.8/src/femr/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/transforms/notes.py` & `femr-0.1.8/src/femr/transforms/notes.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/transforms/sickkids.py` & `femr-0.1.8/src/femr/transforms/sickkids.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr/transforms/stanford.py` & `femr-0.1.8/src/femr/transforms/stanford.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr.egg-info/PKG-INFO` & `femr-0.1.8/src/femr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Framework for Electronic Medical Records. A python package for building models using EHR data.
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: models
 License-File: LICENSE
```

### Comparing `femr-0.1.7/src/femr.egg-info/SOURCES.txt` & `femr-0.1.8/src/femr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/src/femr.egg-info/entry_points.txt` & `femr-0.1.8/src/femr.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/featurizers/test_OnlineStatistics.py` & `femr-0.1.8/tests/featurizers/test_OnlineStatistics.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/featurizers/test_featurizers.py` & `femr-0.1.8/tests/featurizers/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/labelers/test_CodeLabelers.py` & `femr-0.1.8/tests/labelers/test_CodeLabelers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/labelers/test_InpatientAdmissionLabelers.py` & `femr-0.1.8/tests/labelers/test_InpatientAdmissionLabelers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/labelers/test_LabValueLabelers.py` & `femr-0.1.8/tests/labelers/test_LabValueLabelers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/labelers/test_LabeledPatients.py` & `femr-0.1.8/tests/labelers/test_LabeledPatients.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/labelers/test_NLabelerPerPatient.py` & `femr-0.1.8/tests/labelers/test_NLabelerPerPatient.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/labelers/test_OpioidOverdoseLabeler.py` & `femr-0.1.8/tests/labelers/test_OpioidOverdoseLabeler.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/labelers/test_TimeHorizonEventLabeler.py` & `femr-0.1.8/tests/labelers/test_TimeHorizonEventLabeler.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/test_csvs.py` & `femr-0.1.8/tests/test_csvs.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/test_datasets.py` & `femr-0.1.8/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/test_jax.py` & `femr-0.1.8/tests/test_jax.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/test_metrics.py` & `femr-0.1.8/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/test_transforms.py` & `femr-0.1.8/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tests/tools.py` & `femr-0.1.8/tests/tools.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tools/omop/normalize_visit_detail.py` & `femr-0.1.8/tools/omop/normalize_visit_detail.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tools/stanford/download_bigquery.py` & `femr-0.1.8/tools/stanford/download_bigquery.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tools/stanford/flowsheet_cleaner.py` & `femr-0.1.8/tools/stanford/flowsheet_cleaner.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb` & `femr-0.1.8/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tutorials/1_run_featurizers.py` & `femr-0.1.8/tutorials/1_run_featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tutorials/2_train_baseline_models.py` & `femr-0.1.8/tutorials/2_train_baseline_models.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tutorials/3_run_text_featurizer.py` & `femr-0.1.8/tutorials/3_run_text_featurizer.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tutorials/4_train_clmbr_model.py` & `femr-0.1.8/tutorials/4_train_clmbr_model.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.7/tutorials/Simple FEMR Format.ipynb` & `femr-0.1.8/tutorials/Simple FEMR Format.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994354194223986%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(10, '    "*

 * *            'f.write("2,1994-02-03,ICD10/E11.4,,,,,some_table\\\\n")  # Note how events can be out '*

 * *            "of order\\n')], delete: [10]}}, 6: {'execution_count': None, 'outputs': {0: {'text': "*

 * *            '["2023-04-28 01:39:46,957 [MainThread  ] [INFO ]  Extracting from OMOP with arguments '*

 * *            "Namespace(simple_source='trash/simple_femr/simple_input', "*

 * *            "target_location='/local-scratch/nigam/projects/ethanid/femr_develop/femr/t […]*

```diff
@@ -89,15 +89,15 @@
                 "\n",
                 "with open(os.path.join(INPUT_DIR, \"example.csv\"), \"w\") as f:\n",
                 "    f.write(\"patient_id,start,code,value,dosage,visit_id,lab_unit,clarity_table\\n\")\n",
                 "    f.write(\"2,1994-01-03,Birth/Birth,,,,,\\n\")  # First event is always birth\n",
                 "\n",
                 "    f.write(\"2,1994-03-06,Drug/Atorvastatin,,50mg,,,\\n\")  # Example usage of dosage\n",
                 "\n",
-                "    f.write(\"2,1994-02-03,ICD10CM/E11.4,,,,,some_table\\n\")  # Note how events can be out of order\n",
+                "    f.write(\"2,1994-02-03,ICD10/E11.4,,,,,some_table\\n\")  # Note how events can be out of order\n",
                 "\n",
                 "    f.write(\"2,1994-07-09,Vitals/Blood Pressure,150,,2,mmhg,\\n\")  # Example use of a numeric value"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
@@ -128,79 +128,42 @@
                 "        for patient_id in range(file_no * 100, (file_no + 1) * 100):\n",
                 "            add_random_patient(patient_id, f)\n",
                 "        "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "id": "fb41a735-7d03-4b5b-b07d-5e442dd71a19",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-04-12 23:05:34,784 [MainThread  ] [INFO ]  Extracting from OMOP with arguments Namespace(simple_source='trash/simple_femr/simple_input', target_location='/local-scratch/nigam/projects/ethanid/femr_develop/femr/tutorials/trash/simple_femr/extract', temp_location='/local-scratch/nigam/projects/ethanid/femr_develop/femr/tutorials/trash/simple_femr/logs', num_threads=2)\n",
-                        "2023-04-12 23:05:34,784 [MainThread  ] [INFO ]  Converting to events\n",
-                        "2023-04-12 23:05:34,899 [MainThread  ] [INFO ]  Converting to patients\n",
-                        "2023-04-12 23:05:34,936 [MainThread  ] [INFO ]  Converting to extract\n"
+                        "2023-04-28 01:39:46,957 [MainThread  ] [INFO ]  Extracting from OMOP with arguments Namespace(simple_source='trash/simple_femr/simple_input', target_location='/local-scratch/nigam/projects/ethanid/femr_develop/femr/tutorials/trash/simple_femr/extract', temp_location='/local-scratch/nigam/projects/ethanid/femr_develop/femr/tutorials/trash/simple_femr/logs', num_threads=2, athena_download='/home/ethanid/vocab')\n",
+                        "2023-04-28 01:39:46,957 [MainThread  ] [INFO ]  Converting to events\n"
                     ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Done with main 2023-04-12T23:05:34.983625759+00:00\n",
-                        "Done with meta 2023-04-12T23:05:34.983845773+00:00\n",
-                        "Converting to extract 2023-04-12 23:05:34.936232\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/plain": [
-                            "0"
-                        ]
-                    },
-                    "execution_count": 4,
-                    "metadata": {},
-                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Convert the directory to an extract\n",
                 "\n",
                 "LOG_DIR = os.path.join(TARGET_DIR, \"logs\")\n",
                 "EXTRACT_DIR = os.path.join(TARGET_DIR, \"extract\")\n",
                 "\n",
-                "os.system(f\"etl_simple_femr {INPUT_DIR} {EXTRACT_DIR} {LOG_DIR} --num_threads 2\")\n"
+                "os.system(f\"etl_simple_femr {INPUT_DIR} {EXTRACT_DIR} {LOG_DIR} --num_threads 2 --athena_download ~/vocab\")\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "id": "a322d997-fa51-4fec-89ee-b87ef0f8f2a0",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Num patients 1001\n",
-                        "8\n",
-                        "Patient(patient_id=8, events=(Event(start=1994-01-03 00:00:00, code=0, dosage=, visit_id=, lab_unit=, clarity_table=), Event(start=1994-02-03 00:00:00, code=3019, dosage=, visit_id=, lab_unit=, clarity_table=some_table), Event(start=1994-03-06 00:00:00, code=4287, dosage=50mg, visit_id=, lab_unit=, clarity_table=), Event(start=1994-07-09 00:00:00, code=3362, value=150.0, dosage=, visit_id=2, lab_unit=mmhg, clarity_table=)))\n",
-                        "2\n",
-                        "What the first code means: Birth/Birth\n",
-                        "Event(start=1994-01-03 00:00:00, code=0, dosage=, visit_id=, lab_unit=, clarity_table=)  Birth/Birth\n",
-                        "Event(start=1994-02-03 00:00:00, code=3019, dosage=, visit_id=, lab_unit=, clarity_table=some_table)  ICD10CM/E11.4\n",
-                        "Event(start=1994-03-06 00:00:00, code=4287, dosage=50mg, visit_id=, lab_unit=, clarity_table=) 50mg Drug/Atorvastatin\n",
-                        "Event(start=1994-07-09 00:00:00, code=3362, value=150.0, dosage=, visit_id=2, lab_unit=mmhg, clarity_table=)  Vitals/Blood Pressure\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# Open and look at the data.\n",
                 "\n",
                 "\n",
                 "import femr.datasets\n",
                 "\n",
                 "database = femr.datasets.PatientDatabase(EXTRACT_DIR)\n",
@@ -211,20 +174,17 @@
                 "# Note that FEMR remaps patient ids, we have to use a mapping to get back our original patient 2\n",
                 "\n",
                 "# Print out that patient\n",
                 "patient = database[2]\n",
                 "print(patient)\n",
                 "\n",
                 "\n",
-                "# Also note that concepts have been mapped to integers\n",
-                "print(\"What the first code means:\", database.get_code_dictionary()[patient.events[0].code])\n",
-                "\n",
                 "# You can pull things like dosage by looking at the event\n",
                 "for event in patient.events:\n",
-                "    print(event, event.dosage, database.get_code_dictionary()[event.code])\n",
+                "    print(event, event.dosage, database.get_ontology().get_all_parents(event.code))\n",
                 "  \n",
                 "all_patient_ids = list(database)\n",
                 "print(len(all_patient_ids))"
             ]
         }
     ],
     "metadata": {
```

### Comparing `femr-0.1.7/tutorials/mimic_etl_tutorial.py` & `femr-0.1.8/tutorials/mimic_etl_tutorial.py`

 * *Files identical despite different names*

