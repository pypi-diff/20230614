# Comparing `tmp/dataquality-0.8.8a0.tar.gz` & `tmp/dataquality-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.8.8a0.tar", last modified: Thu Dec 15 23:16:54 2022, max compression
+gzip compressed data, was "dataquality-0.8.9.tar", last modified: Thu Dec 15 23:41:39 2022, max compression
```

## Comparing `dataquality-0.8.8a0.tar` & `dataquality-0.8.9.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0       99 2022-10-11 23:00:09.655956 dataquality-0.8.8a0/.coveragerc
--rw-r--r--   0        0        0      131 2022-10-11 23:00:09.656126 dataquality-0.8.8a0/.editorconfig
--rw-r--r--   0        0        0      181 2022-10-11 23:00:09.656277 dataquality-0.8.8a0/.flake8
--rw-r--r--   0        0        0       75 2022-10-11 23:00:09.656495 dataquality-0.8.8a0/.github/CODEOWNERS
--rw-r--r--   0        0        0      924 2022-10-11 23:00:09.656756 dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      590 2022-10-11 23:00:09.656922 dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/doc.md
--rw-r--r--   0        0        0      700 2022-10-11 23:00:09.657078 dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      542 2022-10-11 23:00:09.657221 dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1169 2022-10-11 23:00:09.657374 dataquality-0.8.8a0/.github/pull_request_template.md
--rw-r--r--   0        0        0      525 2022-10-11 23:00:09.657583 dataquality-0.8.8a0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      740 2022-10-11 23:00:09.657729 dataquality-0.8.8a0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2292 2022-12-09 01:34:41.687656 dataquality-0.8.8a0/.gitignore
--rw-r--r--   0        0        0        6 2022-10-11 23:00:09.658013 dataquality-0.8.8a0/.python-version
--rw-r--r--   0        0        0     8078 2022-10-11 23:00:09.658217 dataquality-0.8.8a0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1066 2022-10-11 23:00:09.658384 dataquality-0.8.8a0/LICENSE
--rw-r--r--   0        0        0      548 2022-10-11 23:00:09.658550 dataquality-0.8.8a0/README.md
--rw-r--r--   0        0        0     4487 2022-12-15 23:16:53.525653 dataquality-0.8.8a0/dataquality/__init__.py
--rw-r--r--   0        0        0     8443 2022-12-15 22:55:49.705515 dataquality-0.8.8a0/dataquality/analytics.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/clients/__init__.py
--rw-r--r--   0        0        0    31697 2022-12-15 22:55:49.723354 dataquality-0.8.8a0/dataquality/clients/api.py
--rw-r--r--   0        0        0     4125 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/clients/objectstore.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/core/__init__.py
--rw-r--r--   0        0        0     8371 2022-12-15 22:55:49.880493 dataquality-0.8.8a0/dataquality/core/_config.py
--rw-r--r--   0        0        0     3104 2022-12-15 22:55:49.857121 dataquality-0.8.8a0/dataquality/core/auth.py
--rw-r--r--   0        0        0     6108 2022-12-15 22:55:49.892040 dataquality-0.8.8a0/dataquality/core/finish.py
--rw-r--r--   0        0        0     9768 2022-12-15 22:55:49.873353 dataquality-0.8.8a0/dataquality/core/init.py
--rw-r--r--   0        0        0    15137 2022-12-15 22:55:49.865162 dataquality-0.8.8a0/dataquality/core/log.py
--rw-r--r--   0        0        0     7039 2022-12-15 22:55:49.885835 dataquality-0.8.8a0/dataquality/core/report.py
--rw-r--r--   0        0        0        0 2022-11-28 17:23:58.644880 dataquality-0.8.8a0/dataquality/dq_auto/__init__.py
--rw-r--r--   0        0        0     9405 2022-12-15 22:55:50.192113 dataquality-0.8.8a0/dataquality/dq_auto/auto.py
--rw-r--r--   0        0        0     4098 2022-12-15 22:55:50.165562 dataquality-0.8.8a0/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0        0        0     7262 2022-12-15 22:55:50.180450 dataquality-0.8.8a0/dataquality/dq_auto/ner.py
--rw-r--r--   0        0        0     3768 2022-12-15 22:55:50.161639 dataquality-0.8.8a0/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0        0        0     3070 2022-12-15 22:55:50.184016 dataquality-0.8.8a0/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0        0        0    11287 2022-12-15 22:55:50.174932 dataquality-0.8.8a0/dataquality/dq_auto/text_classification.py
--rw-r--r--   0        0        0      293 2022-10-31 17:31:56.991517 dataquality-0.8.8a0/dataquality/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/integrations/__init__.py
--rw-r--r--   0        0        0    15422 2022-12-15 22:55:50.153586 dataquality-0.8.8a0/dataquality/integrations/experimental/keras.py
--rw-r--r--   0        0        0     9603 2022-12-15 22:55:50.141797 dataquality-0.8.8a0/dataquality/integrations/hf.py
--rw-r--r--   0        0        0     4418 2022-12-15 22:55:50.099188 dataquality-0.8.8a0/dataquality/integrations/keras.py
--rw-r--r--   0        0        0    25573 2022-12-15 22:55:50.127805 dataquality-0.8.8a0/dataquality/integrations/spacy.py
--rw-r--r--   0        0        0     5701 2022-12-15 22:55:50.133612 dataquality-0.8.8a0/dataquality/integrations/torch.py
--rw-r--r--   0        0        0     8344 2022-12-15 22:55:50.110231 dataquality-0.8.8a0/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0        0        0       95 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/loggers/__init__.py
--rw-r--r--   0        0        0    10577 2022-12-15 22:55:49.742526 dataquality-0.8.8a0/dataquality/loggers/base_logger.py
--rw-r--r--   0        0        0      357 2022-12-15 22:55:49.797420 dataquality-0.8.8a0/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0        0        0    21618 2022-12-15 22:55:49.833504 dataquality-0.8.8a0/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0        0        0     1935 2022-12-15 22:55:49.795136 dataquality-0.8.8a0/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0        0        0    19534 2022-12-15 23:16:18.640854 dataquality-0.8.8a0/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0        0        0    14796 2022-12-15 22:55:49.810658 dataquality-0.8.8a0/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0        0        0    31289 2022-12-15 22:55:49.822605 dataquality-0.8.8a0/dataquality/loggers/data_logger/text_ner.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0        0        0     1702 2022-12-15 22:55:49.849791 dataquality-0.8.8a0/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0        0        0      260 2022-12-09 01:34:41.691356 dataquality-0.8.8a0/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0        0        0      958 2022-12-15 22:55:49.841534 dataquality-0.8.8a0/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0        0        0     1510 2022-12-15 22:55:49.844092 dataquality-0.8.8a0/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0        0        0     1608 2022-12-15 22:55:49.846923 dataquality-0.8.8a0/dataquality/loggers/logger_config/text_ner.py
--rw-r--r--   0        0        0      362 2022-12-15 22:55:49.752683 dataquality-0.8.8a0/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0        0        0     8218 2022-12-15 22:55:49.787356 dataquality-0.8.8a0/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0        0        0     1015 2022-12-15 22:55:49.748942 dataquality-0.8.8a0/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0        0        0     7838 2022-12-15 22:55:49.758139 dataquality-0.8.8a0/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0        0        0     9058 2022-12-15 22:55:49.765076 dataquality-0.8.8a0/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0        0        0    33524 2022-12-15 22:55:49.778826 dataquality-0.8.8a0/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0        0        0    27895 2022-12-15 22:55:49.682962 dataquality-0.8.8a0/dataquality/metrics.py
--rw-r--r--   0        0        0      165 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/schemas/__init__.py
--rw-r--r--   0        0        0     8363 2022-12-15 22:55:50.070930 dataquality-0.8.8a0/dataquality/schemas/condition.py
--rw-r--r--   0        0        0      570 2022-12-15 22:55:50.042509 dataquality-0.8.8a0/dataquality/schemas/dataframe.py
--rw-r--r--   0        0        0     4382 2022-12-15 22:55:50.066364 dataquality-0.8.8a0/dataquality/schemas/edit.py
--rw-r--r--   0        0        0      662 2022-11-28 17:23:58.658371 dataquality-0.8.8a0/dataquality/schemas/hf.py
--rw-r--r--   0        0        0      118 2022-12-15 22:55:50.045596 dataquality-0.8.8a0/dataquality/schemas/job.py
--rw-r--r--   0        0        0     5254 2022-12-15 22:55:50.039905 dataquality-0.8.8a0/dataquality/schemas/metrics.py
--rw-r--r--   0        0        0      992 2022-12-15 22:55:50.075199 dataquality-0.8.8a0/dataquality/schemas/ner.py
--rw-r--r--   0        0        0      617 2022-12-15 22:55:50.087265 dataquality-0.8.8a0/dataquality/schemas/report.py
--rw-r--r--   0        0        0      287 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/schemas/request_type.py
--rw-r--r--   0        0        0     1397 2022-12-15 22:55:50.051404 dataquality-0.8.8a0/dataquality/schemas/route.py
--rw-r--r--   0        0        0      928 2022-12-15 22:55:50.078365 dataquality-0.8.8a0/dataquality/schemas/split.py
--rw-r--r--   0        0        0      770 2022-12-15 22:55:50.081648 dataquality-0.8.8a0/dataquality/schemas/task_type.py
--rw-r--r--   0        0        0      244 2022-12-15 22:55:50.084718 dataquality-0.8.8a0/dataquality/schemas/torch.py
--rw-r--r--   0        0        0      222 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/utils/__init__.py
--rw-r--r--   0        0        0      674 2022-11-02 20:22:30.684530 dataquality-0.8.8a0/dataquality/utils/ampli.py
--rw-r--r--   0        0        0      401 2022-12-15 22:55:49.897812 dataquality-0.8.8a0/dataquality/utils/auth.py
--rw-r--r--   0        0        0     5784 2022-12-15 22:55:50.032304 dataquality-0.8.8a0/dataquality/utils/auto.py
--rw-r--r--   0        0        0      865 2022-12-15 21:23:01.762336 dataquality-0.8.8a0/dataquality/utils/auto_trainer.py
--rw-r--r--   0        0        0      154 2022-12-15 22:55:49.911595 dataquality-0.8.8a0/dataquality/utils/cloud.py
--rw-r--r--   0        0        0      651 2022-12-09 01:34:41.693535 dataquality-0.8.8a0/dataquality/utils/cv.py
--rw-r--r--   0        0        0     3381 2022-12-15 22:55:49.959886 dataquality-0.8.8a0/dataquality/utils/dq_logger.py
--rw-r--r--   0        0        0      129 2022-10-11 23:00:09.000000 dataquality-0.8.8a0/dataquality/utils/file.py
--rw-r--r--   0        0        0     1672 2022-12-15 22:55:49.935030 dataquality-0.8.8a0/dataquality/utils/hdf5_store.py
--rw-r--r--   0        0        0     3047 2022-12-15 22:55:50.000060 dataquality-0.8.8a0/dataquality/utils/helpers.py
--rw-r--r--   0        0        0     9962 2022-12-15 22:55:49.903455 dataquality-0.8.8a0/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0        0        0      429 2022-11-28 17:23:58.665769 dataquality-0.8.8a0/dataquality/utils/imports.py
--rw-r--r--   0        0        0     7977 2022-12-15 22:55:49.918540 dataquality-0.8.8a0/dataquality/utils/keras.py
--rw-r--r--   0        0        0     2408 2022-12-15 22:55:49.946816 dataquality-0.8.8a0/dataquality/utils/ml.py
--rw-r--r--   0        0        0    23873 2022-11-02 20:22:30.685786 dataquality-0.8.8a0/dataquality/utils/name.py
--rw-r--r--   0        0        0     5923 2022-12-15 22:55:49.984237 dataquality-0.8.8a0/dataquality/utils/profiler.py
--rw-r--r--   0        0        0     4070 2022-12-15 22:55:49.932303 dataquality-0.8.8a0/dataquality/utils/spacy_integration.py
--rw-r--r--   0        0        0      260 2022-11-28 17:23:58.668908 dataquality-0.8.8a0/dataquality/utils/tf.py
--rw-r--r--   0        0        0     1912 2022-12-15 22:55:49.921000 dataquality-0.8.8a0/dataquality/utils/thread_pool.py
--rw-r--r--   0        0        0     9488 2022-12-15 22:55:49.993538 dataquality-0.8.8a0/dataquality/utils/torch.py
--rw-r--r--   0        0        0     2739 2022-12-15 22:55:49.914032 dataquality-0.8.8a0/dataquality/utils/transformers.py
--rw-r--r--   0        0        0     9149 2022-12-15 22:55:49.940824 dataquality-0.8.8a0/dataquality/utils/vaex.py
--rw-r--r--   0        0        0     1440 2022-11-02 20:22:30.688040 dataquality-0.8.8a0/dataquality/utils/version.py
--rw-r--r--   0        0        0    18832 2022-10-11 23:00:09.671318 dataquality-0.8.8a0/docs/Dataquality-Client-Demo.ipynb
--rw-r--r--   0        0        0    10352 2022-12-06 23:24:23.704737 dataquality-0.8.8a0/docs/End to End runs per task type.ipynb
--rw-r--r--   0        0        0    12031 2022-10-11 23:00:09.671739 dataquality-0.8.8a0/docs/Inference-Demo.ipynb
--rw-r--r--   0        0        0     6893 2022-10-11 23:00:09.671910 dataquality-0.8.8a0/docs/NER Inference.ipynb
--rw-r--r--   0        0        0      172 2022-12-09 01:34:41.694895 dataquality-0.8.8a0/docs/cv/README.md
--rw-r--r--   0        0        0     4245 2022-12-09 01:34:41.695431 dataquality-0.8.8a0/docs/cv/cv-demo-hf.py
--rw-r--r--   0        0        0     1893 2022-12-09 01:34:41.695867 dataquality-0.8.8a0/docs/cv/cv-testing-benchmark.py
--rw-r--r--   0        0        0      154 2022-10-11 23:00:09.672060 dataquality-0.8.8a0/docs/index.md
--rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672196 dataquality-0.8.8a0/mkdocs.yml
--rw-r--r--   0        0        0       66 2022-10-11 23:00:09.672321 dataquality-0.8.8a0/mypy.ini
--rw-r--r--   0        0        0     1571 2022-12-15 21:23:01.763974 dataquality-0.8.8a0/pyproject.toml
--rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672594 dataquality-0.8.8a0/pytest.ini
--rwxr-xr-x   0        0        0      247 2022-10-11 23:00:09.672835 dataquality-0.8.8a0/scripts/bump-version.sh
--rwxr-xr-x   0        0        0      100 2022-10-11 23:00:09.672960 dataquality-0.8.8a0/scripts/clean.sh
--rwxr-xr-x   0        0        0       60 2022-10-11 23:00:09.673077 dataquality-0.8.8a0/scripts/docs-build.sh
--rwxr-xr-x   0        0        0       55 2022-10-11 23:00:09.673199 dataquality-0.8.8a0/scripts/docs-serve.sh
--rwxr-xr-x   0        0        0      320 2022-10-11 23:00:09.673322 dataquality-0.8.8a0/scripts/format.sh
--rwxr-xr-x   0        0        0      106 2022-10-11 23:00:09.673446 dataquality-0.8.8a0/scripts/install.sh
--rwxr-xr-x   0        0        0      126 2022-10-11 23:00:09.673573 dataquality-0.8.8a0/scripts/lint.sh
--rwxr-xr-x   0        0        0       29 2022-10-11 23:00:09.673690 dataquality-0.8.8a0/scripts/publish.sh
--rwxr-xr-x   0        0        0       66 2022-10-11 23:00:09.673820 dataquality-0.8.8a0/scripts/set-local-env.sh
--rwxr-xr-x   0        0        0       56 2022-10-11 23:00:09.673948 dataquality-0.8.8a0/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      216 2022-10-11 23:00:09.674078 dataquality-0.8.8a0/scripts/test.sh
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.674219 dataquality-0.8.8a0/tests/__init__.py
--rw-r--r--   0        0        0     3479 2022-12-15 22:55:50.337694 dataquality-0.8.8a0/tests/auto/test_ner_auto.py
--rw-r--r--   0        0        0    16171 2022-12-15 22:55:50.332451 dataquality-0.8.8a0/tests/auto/test_tc_auto.py
--rw-r--r--   0        0        0    10549 2022-12-15 22:55:50.250383 dataquality-0.8.8a0/tests/clients/test_api.py
--rw-r--r--   0        0        0     5852 2022-12-15 22:55:50.218271 dataquality-0.8.8a0/tests/conftest.py
--rw-r--r--   0        0        0     1409 2022-12-15 22:55:50.291882 dataquality-0.8.8a0/tests/core/test_auth.py
--rw-r--r--   0        0        0      418 2022-11-02 20:22:30.689801 dataquality-0.8.8a0/tests/core/test_cloud.py
--rw-r--r--   0        0        0     6719 2022-12-15 22:55:50.310038 dataquality-0.8.8a0/tests/core/test_config.py
--rw-r--r--   0        0        0     6122 2022-12-15 22:55:50.303943 dataquality-0.8.8a0/tests/core/test_finish.py
--rw-r--r--   0        0        0    15940 2022-12-15 22:55:50.321348 dataquality-0.8.8a0/tests/core/test_init.py
--rw-r--r--   0        0        0     6907 2022-12-15 22:55:50.298561 dataquality-0.8.8a0/tests/core/test_report.py
--rw-r--r--   0        0        0       40 2022-10-11 23:00:09.674520 dataquality-0.8.8a0/tests/exceptions.py
--rw-r--r--   0        0        0     4990 2022-12-15 22:55:50.551753 dataquality-0.8.8a0/tests/inference/test_inference.py
--rw-r--r--   0        0        0     3234 2022-11-02 20:22:30.691277 dataquality-0.8.8a0/tests/inference/test_text_classification_inf.py
--rw-r--r--   0        0        0     3792 2022-11-02 20:22:30.691419 dataquality-0.8.8a0/tests/inference/test_text_ner_inf.py
--rw-r--r--   0        0        0     3862 2022-10-11 23:00:09.675468 dataquality-0.8.8a0/tests/integration/mock_training_run.py
--rw-r--r--   0        0        0     3954 2022-12-15 22:55:50.518748 dataquality-0.8.8a0/tests/integrations/hf/test_cv_hf.py
--rw-r--r--   0        0        0    10897 2022-12-15 22:55:50.511915 dataquality-0.8.8a0/tests/integrations/hf/test_hf_integration.py
--rw-r--r--   0        0        0    10123 2022-12-15 22:55:50.500976 dataquality-0.8.8a0/tests/integrations/hf/test_text_classification_hf.py
--rw-r--r--   0        0        0     9263 2022-12-15 22:55:50.474496 dataquality-0.8.8a0/tests/integrations/keras/test_experimental.py
--rw-r--r--   0        0        0      514 2022-12-15 21:23:01.768632 dataquality-0.8.8a0/tests/integrations/keras/test_utils.py
--rw-r--r--   0        0        0     1346 2022-12-15 22:55:50.529433 dataquality-0.8.8a0/tests/integrations/spacy/conftest.py
--rw-r--r--   0        0        0      760 2022-11-02 20:22:30.692338 dataquality-0.8.8a0/tests/integrations/spacy/test_spacy_integration.py
--rw-r--r--   0        0        0    16355 2022-12-15 22:55:50.540102 dataquality-0.8.8a0/tests/integrations/spacy/test_spacy_ner.py
--rw-r--r--   0        0        0      904 2022-12-15 22:55:50.480165 dataquality-0.8.8a0/tests/integrations/torch/test_pt_utils.py
--rw-r--r--   0        0        0     7367 2022-12-15 22:55:50.489505 dataquality-0.8.8a0/tests/integrations/torch/test_text_classification_pt.py
--rw-r--r--   0        0        0    11728 2022-12-15 22:55:50.261645 dataquality-0.8.8a0/tests/loggers/test_multi_label.py
--rw-r--r--   0        0        0    23385 2022-12-15 22:55:50.285697 dataquality-0.8.8a0/tests/loggers/test_ner.py
--rw-r--r--   0        0        0    13108 2022-12-15 22:56:24.494601 dataquality-0.8.8a0/tests/loggers/test_text_classification.py
--rw-r--r--   0        0        0     7226 2022-12-15 22:55:50.453144 dataquality-0.8.8a0/tests/schemas/test_conditions.py
--rw-r--r--   0        0        0      402 2022-11-02 20:22:30.695867 dataquality-0.8.8a0/tests/schemas/test_metrics.py
--rw-r--r--   0        0        0    29166 2022-12-15 22:55:50.237796 dataquality-0.8.8a0/tests/test_dataquality.py
--rw-r--r--   0        0        0     1783 2022-11-28 17:23:58.686840 dataquality-0.8.8a0/tests/test_telemetrics.py
--rw-r--r--   0        0        0        0 2022-11-02 20:22:30.697603 dataquality-0.8.8a0/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     5900 2022-12-15 22:55:50.384518 dataquality-0.8.8a0/tests/test_utils/data_utils.py
--rw-r--r--   0        0        0     3808 2022-12-15 22:55:50.346268 dataquality-0.8.8a0/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0        0        0    11378 2022-11-02 20:22:30.698317 dataquality-0.8.8a0/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0        0        0     8122 2022-11-28 17:23:58.687297 dataquality-0.8.8a0/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0        0        0     3695 2022-11-02 20:22:30.698590 dataquality-0.8.8a0/tests/test_utils/lightning_model.py
--rw-r--r--   0        0        0     4908 2022-12-15 22:55:50.362495 dataquality-0.8.8a0/tests/test_utils/mock_request.py
--rw-r--r--   0        0        0     2840 2022-11-02 20:22:30.699379 dataquality-0.8.8a0/tests/test_utils/ner_constants.py
--rw-r--r--   0        0        0     4239 2022-12-15 22:55:50.370141 dataquality-0.8.8a0/tests/test_utils/spacy_integration.py
--rw-r--r--   0        0        0    22487 2022-12-06 23:24:23.709042 dataquality-0.8.8a0/tests/test_utils/spacy_integration_constants.py
--rw-r--r--   0        0        0    23021 2022-12-06 23:24:23.709498 dataquality-0.8.8a0/tests/test_utils/spacy_integration_constants_inference.py
--rw-r--r--   0        0        0     4614 2022-12-15 22:55:50.432733 dataquality-0.8.8a0/tests/utils/test_auto.py
--rw-r--r--   0        0        0     1623 2022-11-02 20:22:30.700412 dataquality-0.8.8a0/tests/utils/test_dq_logger.py
--rw-r--r--   0        0        0      224 2022-12-15 22:55:50.438763 dataquality-0.8.8a0/tests/utils/test_name.py
--rw-r--r--   0        0        0      288 2022-11-28 17:23:58.689269 dataquality-0.8.8a0/tests/utils/test_tf_version.py
--rw-r--r--   0        0        0      601 2022-11-02 20:22:30.701010 dataquality-0.8.8a0/tests/utils/test_vaex_utils.py
--rw-r--r--   0        0        0     1316 2022-12-15 22:55:50.419074 dataquality-0.8.8a0/tests/utils/test_version.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 dataquality-0.8.8a0/PKG-INFO
+-rw-r--r--   0        0        0       99 2022-10-11 23:00:09.655956 dataquality-0.8.9/.coveragerc
+-rw-r--r--   0        0        0      131 2022-10-11 23:00:09.656126 dataquality-0.8.9/.editorconfig
+-rw-r--r--   0        0        0      181 2022-10-11 23:00:09.656277 dataquality-0.8.9/.flake8
+-rw-r--r--   0        0        0       75 2022-10-11 23:00:09.656495 dataquality-0.8.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      924 2022-10-11 23:00:09.656756 dataquality-0.8.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      590 2022-10-11 23:00:09.656922 dataquality-0.8.9/.github/ISSUE_TEMPLATE/doc.md
+-rw-r--r--   0        0        0      700 2022-10-11 23:00:09.657078 dataquality-0.8.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0        0        0      542 2022-10-11 23:00:09.657221 dataquality-0.8.9/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1169 2022-10-11 23:00:09.657374 dataquality-0.8.9/.github/pull_request_template.md
+-rw-r--r--   0        0        0      525 2022-10-11 23:00:09.657583 dataquality-0.8.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      740 2022-10-11 23:00:09.657729 dataquality-0.8.9/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     2292 2022-12-09 01:34:41.687656 dataquality-0.8.9/.gitignore
+-rw-r--r--   0        0        0        6 2022-10-11 23:00:09.658013 dataquality-0.8.9/.python-version
+-rw-r--r--   0        0        0     8078 2022-10-11 23:00:09.658217 dataquality-0.8.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1066 2022-10-11 23:00:09.658384 dataquality-0.8.9/LICENSE
+-rw-r--r--   0        0        0      548 2022-10-11 23:00:09.658550 dataquality-0.8.9/README.md
+-rw-r--r--   0        0        0     4485 2022-12-15 23:41:37.187563 dataquality-0.8.9/dataquality/__init__.py
+-rw-r--r--   0        0        0     8443 2022-12-15 23:31:05.910410 dataquality-0.8.9/dataquality/analytics.py
+-rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/clients/__init__.py
+-rw-r--r--   0        0        0    31697 2022-12-15 23:31:05.927629 dataquality-0.8.9/dataquality/clients/api.py
+-rw-r--r--   0        0        0     4125 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/clients/objectstore.py
+-rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/core/__init__.py
+-rw-r--r--   0        0        0     8371 2022-12-15 23:31:06.069608 dataquality-0.8.9/dataquality/core/_config.py
+-rw-r--r--   0        0        0     3104 2022-12-15 23:31:06.045893 dataquality-0.8.9/dataquality/core/auth.py
+-rw-r--r--   0        0        0     6108 2022-12-15 23:31:06.082327 dataquality-0.8.9/dataquality/core/finish.py
+-rw-r--r--   0        0        0     9768 2022-12-15 23:31:06.062587 dataquality-0.8.9/dataquality/core/init.py
+-rw-r--r--   0        0        0    15137 2022-12-15 23:31:06.053808 dataquality-0.8.9/dataquality/core/log.py
+-rw-r--r--   0        0        0     7039 2022-12-15 23:31:06.076104 dataquality-0.8.9/dataquality/core/report.py
+-rw-r--r--   0        0        0        0 2022-11-28 17:23:58.644880 dataquality-0.8.9/dataquality/dq_auto/__init__.py
+-rw-r--r--   0        0        0     9405 2022-12-15 23:31:06.393084 dataquality-0.8.9/dataquality/dq_auto/auto.py
+-rw-r--r--   0        0        0     4098 2022-12-15 23:31:06.333955 dataquality-0.8.9/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0        0        0     7262 2022-12-15 23:31:06.379759 dataquality-0.8.9/dataquality/dq_auto/ner.py
+-rw-r--r--   0        0        0     3768 2022-12-15 23:31:06.310402 dataquality-0.8.9/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0        0        0     3070 2022-12-15 23:31:06.384090 dataquality-0.8.9/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0        0        0    11287 2022-12-15 23:31:06.373912 dataquality-0.8.9/dataquality/dq_auto/text_classification.py
+-rw-r--r--   0        0        0      293 2022-10-31 17:31:56.991517 dataquality-0.8.9/dataquality/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/integrations/__init__.py
+-rw-r--r--   0        0        0    15422 2022-12-15 23:31:06.300508 dataquality-0.8.9/dataquality/integrations/experimental/keras.py
+-rw-r--r--   0        0        0     9603 2022-12-15 23:31:06.289374 dataquality-0.8.9/dataquality/integrations/hf.py
+-rw-r--r--   0        0        0     4418 2022-12-15 23:31:06.250210 dataquality-0.8.9/dataquality/integrations/keras.py
+-rw-r--r--   0        0        0    25573 2022-12-15 23:31:06.275830 dataquality-0.8.9/dataquality/integrations/spacy.py
+-rw-r--r--   0        0        0     5701 2022-12-15 23:31:06.281061 dataquality-0.8.9/dataquality/integrations/torch.py
+-rw-r--r--   0        0        0     8344 2022-12-15 23:31:06.259439 dataquality-0.8.9/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0        0        0       95 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/loggers/__init__.py
+-rw-r--r--   0        0        0    10577 2022-12-15 23:31:05.945221 dataquality-0.8.9/dataquality/loggers/base_logger.py
+-rw-r--r--   0        0        0      357 2022-12-15 23:31:05.989196 dataquality-0.8.9/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0        0        0    21618 2022-12-15 23:31:06.020215 dataquality-0.8.9/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0        0        0     1935 2022-12-15 23:31:05.986971 dataquality-0.8.9/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0        0        0    19532 2022-12-15 23:31:05.994896 dataquality-0.8.9/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0        0        0    14796 2022-12-15 23:31:06.000577 dataquality-0.8.9/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0        0        0    31289 2022-12-15 23:31:06.009806 dataquality-0.8.9/dataquality/loggers/data_logger/text_ner.py
+-rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0        0        0     1702 2022-12-15 23:31:06.039210 dataquality-0.8.9/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0        0        0      260 2022-12-09 01:34:41.691356 dataquality-0.8.9/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0        0        0      958 2022-12-15 23:31:06.029388 dataquality-0.8.9/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0        0        0     1510 2022-12-15 23:31:06.032713 dataquality-0.8.9/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0        0        0     1608 2022-12-15 23:31:06.036035 dataquality-0.8.9/dataquality/loggers/logger_config/text_ner.py
+-rw-r--r--   0        0        0      362 2022-12-15 23:31:05.953592 dataquality-0.8.9/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0        0        0     8218 2022-12-15 23:31:05.979653 dataquality-0.8.9/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0        0        0     1015 2022-12-15 23:31:05.950221 dataquality-0.8.9/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0        0        0     7838 2022-12-15 23:31:05.958149 dataquality-0.8.9/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0        0        0     9058 2022-12-15 23:31:05.963261 dataquality-0.8.9/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0        0        0    33524 2022-12-15 23:31:05.972893 dataquality-0.8.9/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0        0        0    27895 2022-12-15 23:31:05.890944 dataquality-0.8.9/dataquality/metrics.py
+-rw-r--r--   0        0        0      165 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/schemas/__init__.py
+-rw-r--r--   0        0        0     8363 2022-12-15 23:31:06.224815 dataquality-0.8.9/dataquality/schemas/condition.py
+-rw-r--r--   0        0        0      570 2022-12-15 23:31:06.204166 dataquality-0.8.9/dataquality/schemas/dataframe.py
+-rw-r--r--   0        0        0     4382 2022-12-15 23:31:06.220218 dataquality-0.8.9/dataquality/schemas/edit.py
+-rw-r--r--   0        0        0      662 2022-11-28 17:23:58.658371 dataquality-0.8.9/dataquality/schemas/hf.py
+-rw-r--r--   0        0        0      118 2022-12-15 23:31:06.206491 dataquality-0.8.9/dataquality/schemas/job.py
+-rw-r--r--   0        0        0     5254 2022-12-15 23:31:06.201016 dataquality-0.8.9/dataquality/schemas/metrics.py
+-rw-r--r--   0        0        0      992 2022-12-15 23:31:06.228257 dataquality-0.8.9/dataquality/schemas/ner.py
+-rw-r--r--   0        0        0      617 2022-12-15 23:31:06.239527 dataquality-0.8.9/dataquality/schemas/report.py
+-rw-r--r--   0        0        0      287 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/schemas/request_type.py
+-rw-r--r--   0        0        0     1397 2022-12-15 23:31:06.209696 dataquality-0.8.9/dataquality/schemas/route.py
+-rw-r--r--   0        0        0      928 2022-12-15 23:31:06.231109 dataquality-0.8.9/dataquality/schemas/split.py
+-rw-r--r--   0        0        0      770 2022-12-15 23:31:06.234039 dataquality-0.8.9/dataquality/schemas/task_type.py
+-rw-r--r--   0        0        0      244 2022-12-15 23:31:06.236970 dataquality-0.8.9/dataquality/schemas/torch.py
+-rw-r--r--   0        0        0      222 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/utils/__init__.py
+-rw-r--r--   0        0        0      674 2022-11-02 20:22:30.684530 dataquality-0.8.9/dataquality/utils/ampli.py
+-rw-r--r--   0        0        0      401 2022-12-15 23:31:06.089109 dataquality-0.8.9/dataquality/utils/auth.py
+-rw-r--r--   0        0        0     5784 2022-12-15 23:31:06.193967 dataquality-0.8.9/dataquality/utils/auto.py
+-rw-r--r--   0        0        0      865 2022-12-15 21:23:01.762336 dataquality-0.8.9/dataquality/utils/auto_trainer.py
+-rw-r--r--   0        0        0      154 2022-12-15 23:31:06.103700 dataquality-0.8.9/dataquality/utils/cloud.py
+-rw-r--r--   0        0        0      651 2022-12-09 01:34:41.693535 dataquality-0.8.9/dataquality/utils/cv.py
+-rw-r--r--   0        0        0     3381 2022-12-15 23:31:06.154205 dataquality-0.8.9/dataquality/utils/dq_logger.py
+-rw-r--r--   0        0        0      129 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/utils/file.py
+-rw-r--r--   0        0        0     1672 2022-12-15 23:31:06.129311 dataquality-0.8.9/dataquality/utils/hdf5_store.py
+-rw-r--r--   0        0        0     3039 2022-12-15 23:31:06.189283 dataquality-0.8.9/dataquality/utils/helpers.py
+-rw-r--r--   0        0        0     9962 2022-12-15 23:31:06.095391 dataquality-0.8.9/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0        0        0      429 2022-11-28 17:23:58.665769 dataquality-0.8.9/dataquality/utils/imports.py
+-rw-r--r--   0        0        0     7977 2022-12-15 23:31:06.111254 dataquality-0.8.9/dataquality/utils/keras.py
+-rw-r--r--   0        0        0     2408 2022-12-15 23:31:06.142227 dataquality-0.8.9/dataquality/utils/ml.py
+-rw-r--r--   0        0        0    23873 2022-11-02 20:22:30.685786 dataquality-0.8.9/dataquality/utils/name.py
+-rw-r--r--   0        0        0     5923 2022-12-15 23:31:06.177280 dataquality-0.8.9/dataquality/utils/profiler.py
+-rw-r--r--   0        0        0     4070 2022-12-15 23:31:06.125979 dataquality-0.8.9/dataquality/utils/spacy_integration.py
+-rw-r--r--   0        0        0      260 2022-11-28 17:23:58.668908 dataquality-0.8.9/dataquality/utils/tf.py
+-rw-r--r--   0        0        0     1912 2022-12-15 23:31:06.114129 dataquality-0.8.9/dataquality/utils/thread_pool.py
+-rw-r--r--   0        0        0     9488 2022-12-15 23:31:06.185769 dataquality-0.8.9/dataquality/utils/torch.py
+-rw-r--r--   0        0        0     2739 2022-12-15 23:31:06.106465 dataquality-0.8.9/dataquality/utils/transformers.py
+-rw-r--r--   0        0        0     9149 2022-12-15 23:31:06.136612 dataquality-0.8.9/dataquality/utils/vaex.py
+-rw-r--r--   0        0        0     1440 2022-11-02 20:22:30.688040 dataquality-0.8.9/dataquality/utils/version.py
+-rw-r--r--   0        0        0    18832 2022-10-11 23:00:09.671318 dataquality-0.8.9/docs/Dataquality-Client-Demo.ipynb
+-rw-r--r--   0        0        0    10352 2022-12-06 23:24:23.704737 dataquality-0.8.9/docs/End to End runs per task type.ipynb
+-rw-r--r--   0        0        0    12031 2022-10-11 23:00:09.671739 dataquality-0.8.9/docs/Inference-Demo.ipynb
+-rw-r--r--   0        0        0     6893 2022-10-11 23:00:09.671910 dataquality-0.8.9/docs/NER Inference.ipynb
+-rw-r--r--   0        0        0      172 2022-12-09 01:34:41.694895 dataquality-0.8.9/docs/cv/README.md
+-rw-r--r--   0        0        0     4245 2022-12-09 01:34:41.695431 dataquality-0.8.9/docs/cv/cv-demo-hf.py
+-rw-r--r--   0        0        0     1893 2022-12-09 01:34:41.695867 dataquality-0.8.9/docs/cv/cv-testing-benchmark.py
+-rw-r--r--   0        0        0      154 2022-10-11 23:00:09.672060 dataquality-0.8.9/docs/index.md
+-rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672196 dataquality-0.8.9/mkdocs.yml
+-rw-r--r--   0        0        0       66 2022-10-11 23:00:09.672321 dataquality-0.8.9/mypy.ini
+-rw-r--r--   0        0        0     1571 2022-12-15 21:23:01.763974 dataquality-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672594 dataquality-0.8.9/pytest.ini
+-rwxr-xr-x   0        0        0      247 2022-10-11 23:00:09.672835 dataquality-0.8.9/scripts/bump-version.sh
+-rwxr-xr-x   0        0        0      100 2022-10-11 23:00:09.672960 dataquality-0.8.9/scripts/clean.sh
+-rwxr-xr-x   0        0        0       60 2022-10-11 23:00:09.673077 dataquality-0.8.9/scripts/docs-build.sh
+-rwxr-xr-x   0        0        0       55 2022-10-11 23:00:09.673199 dataquality-0.8.9/scripts/docs-serve.sh
+-rwxr-xr-x   0        0        0      320 2022-10-11 23:00:09.673322 dataquality-0.8.9/scripts/format.sh
+-rwxr-xr-x   0        0        0      106 2022-10-11 23:00:09.673446 dataquality-0.8.9/scripts/install.sh
+-rwxr-xr-x   0        0        0      126 2022-10-11 23:00:09.673573 dataquality-0.8.9/scripts/lint.sh
+-rwxr-xr-x   0        0        0       29 2022-10-11 23:00:09.673690 dataquality-0.8.9/scripts/publish.sh
+-rwxr-xr-x   0        0        0       66 2022-10-11 23:00:09.673820 dataquality-0.8.9/scripts/set-local-env.sh
+-rwxr-xr-x   0        0        0       56 2022-10-11 23:00:09.673948 dataquality-0.8.9/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      216 2022-10-11 23:00:09.674078 dataquality-0.8.9/scripts/test.sh
+-rw-r--r--   0        0        0        0 2022-10-11 23:00:09.674219 dataquality-0.8.9/tests/__init__.py
+-rw-r--r--   0        0        0     3479 2022-12-15 23:31:06.527876 dataquality-0.8.9/tests/auto/test_ner_auto.py
+-rw-r--r--   0        0        0    16171 2022-12-15 23:31:06.523820 dataquality-0.8.9/tests/auto/test_tc_auto.py
+-rw-r--r--   0        0        0    10549 2022-12-15 23:31:06.444129 dataquality-0.8.9/tests/clients/test_api.py
+-rw-r--r--   0        0        0     5852 2022-12-15 23:31:06.418269 dataquality-0.8.9/tests/conftest.py
+-rw-r--r--   0        0        0     1409 2022-12-15 23:31:06.481108 dataquality-0.8.9/tests/core/test_auth.py
+-rw-r--r--   0        0        0      418 2022-11-02 20:22:30.689801 dataquality-0.8.9/tests/core/test_cloud.py
+-rw-r--r--   0        0        0     6719 2022-12-15 23:31:06.497841 dataquality-0.8.9/tests/core/test_config.py
+-rw-r--r--   0        0        0     6122 2022-12-15 23:31:06.492412 dataquality-0.8.9/tests/core/test_finish.py
+-rw-r--r--   0        0        0    15940 2022-12-15 23:31:06.511453 dataquality-0.8.9/tests/core/test_init.py
+-rw-r--r--   0        0        0     6907 2022-12-15 23:31:06.487171 dataquality-0.8.9/tests/core/test_report.py
+-rw-r--r--   0        0        0       40 2022-10-11 23:00:09.674520 dataquality-0.8.9/tests/exceptions.py
+-rw-r--r--   0        0        0     4990 2022-12-15 23:31:06.709420 dataquality-0.8.9/tests/inference/test_inference.py
+-rw-r--r--   0        0        0     3234 2022-11-02 20:22:30.691277 dataquality-0.8.9/tests/inference/test_text_classification_inf.py
+-rw-r--r--   0        0        0     3792 2022-11-02 20:22:30.691419 dataquality-0.8.9/tests/inference/test_text_ner_inf.py
+-rw-r--r--   0        0        0     3862 2022-10-11 23:00:09.675468 dataquality-0.8.9/tests/integration/mock_training_run.py
+-rw-r--r--   0        0        0     3954 2022-12-15 23:31:06.679834 dataquality-0.8.9/tests/integrations/hf/test_cv_hf.py
+-rw-r--r--   0        0        0    10897 2022-12-15 23:31:06.673447 dataquality-0.8.9/tests/integrations/hf/test_hf_integration.py
+-rw-r--r--   0        0        0    10123 2022-12-15 23:31:06.662649 dataquality-0.8.9/tests/integrations/hf/test_text_classification_hf.py
+-rw-r--r--   0        0        0     9263 2022-12-15 23:31:06.640380 dataquality-0.8.9/tests/integrations/keras/test_experimental.py
+-rw-r--r--   0        0        0      514 2022-12-15 21:23:01.768632 dataquality-0.8.9/tests/integrations/keras/test_utils.py
+-rw-r--r--   0        0        0     1346 2022-12-15 23:31:06.689001 dataquality-0.8.9/tests/integrations/spacy/conftest.py
+-rw-r--r--   0        0        0      760 2022-11-02 20:22:30.692338 dataquality-0.8.9/tests/integrations/spacy/test_spacy_integration.py
+-rw-r--r--   0        0        0    16355 2022-12-15 23:31:06.699854 dataquality-0.8.9/tests/integrations/spacy/test_spacy_ner.py
+-rw-r--r--   0        0        0      904 2022-12-15 23:31:06.645632 dataquality-0.8.9/tests/integrations/torch/test_pt_utils.py
+-rw-r--r--   0        0        0     7367 2022-12-15 23:31:06.653430 dataquality-0.8.9/tests/integrations/torch/test_text_classification_pt.py
+-rw-r--r--   0        0        0    11728 2022-12-15 23:31:06.453921 dataquality-0.8.9/tests/loggers/test_multi_label.py
+-rw-r--r--   0        0        0    23385 2022-12-15 23:31:06.475658 dataquality-0.8.9/tests/loggers/test_ner.py
+-rw-r--r--   0        0        0    13108 2022-12-15 23:31:06.460897 dataquality-0.8.9/tests/loggers/test_text_classification.py
+-rw-r--r--   0        0        0     7226 2022-12-15 23:31:06.622782 dataquality-0.8.9/tests/schemas/test_conditions.py
+-rw-r--r--   0        0        0      402 2022-11-02 20:22:30.695867 dataquality-0.8.9/tests/schemas/test_metrics.py
+-rw-r--r--   0        0        0    29166 2022-12-15 23:31:06.434729 dataquality-0.8.9/tests/test_dataquality.py
+-rw-r--r--   0        0        0     1783 2022-11-28 17:23:58.686840 dataquality-0.8.9/tests/test_telemetrics.py
+-rw-r--r--   0        0        0        0 2022-11-02 20:22:30.697603 dataquality-0.8.9/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     5900 2022-12-15 23:31:06.565806 dataquality-0.8.9/tests/test_utils/data_utils.py
+-rw-r--r--   0        0        0     3808 2022-12-15 23:31:06.536970 dataquality-0.8.9/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0        0        0    11378 2022-11-02 20:22:30.698317 dataquality-0.8.9/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0        0        0     8122 2022-11-28 17:23:58.687297 dataquality-0.8.9/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0        0        0     3695 2022-11-02 20:22:30.698590 dataquality-0.8.9/tests/test_utils/lightning_model.py
+-rw-r--r--   0        0        0     4908 2022-12-15 23:31:06.548195 dataquality-0.8.9/tests/test_utils/mock_request.py
+-rw-r--r--   0        0        0     2840 2022-11-02 20:22:30.699379 dataquality-0.8.9/tests/test_utils/ner_constants.py
+-rw-r--r--   0        0        0     4239 2022-12-15 23:31:06.553629 dataquality-0.8.9/tests/test_utils/spacy_integration.py
+-rw-r--r--   0        0        0    22487 2022-12-06 23:24:23.709042 dataquality-0.8.9/tests/test_utils/spacy_integration_constants.py
+-rw-r--r--   0        0        0    23021 2022-12-06 23:24:23.709498 dataquality-0.8.9/tests/test_utils/spacy_integration_constants_inference.py
+-rw-r--r--   0        0        0     4614 2022-12-15 23:31:06.607721 dataquality-0.8.9/tests/utils/test_auto.py
+-rw-r--r--   0        0        0     1623 2022-11-02 20:22:30.700412 dataquality-0.8.9/tests/utils/test_dq_logger.py
+-rw-r--r--   0        0        0      224 2022-12-15 23:31:06.612161 dataquality-0.8.9/tests/utils/test_name.py
+-rw-r--r--   0        0        0      288 2022-11-28 17:23:58.689269 dataquality-0.8.9/tests/utils/test_tf_version.py
+-rw-r--r--   0        0        0      601 2022-11-02 20:22:30.701010 dataquality-0.8.9/tests/utils/test_vaex_utils.py
+-rw-r--r--   0        0        0     1316 2022-12-15 23:31:06.599087 dataquality-0.8.9/tests/utils/test_version.py
+-rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 dataquality-0.8.9/PKG-INFO
```

### Comparing `dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/bug.md` & `dataquality-0.8.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/doc.md` & `dataquality-0.8.9/.github/ISSUE_TEMPLATE/doc.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/feature.md` & `dataquality-0.8.9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/.github/ISSUE_TEMPLATE/question.md` & `dataquality-0.8.9/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/.github/pull_request_template.md` & `dataquality-0.8.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/.github/workflows/publish.yaml` & `dataquality-0.8.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/.github/workflows/test.yaml` & `dataquality-0.8.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/.gitignore` & `dataquality-0.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/CONTRIBUTING.md` & `dataquality-0.8.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/LICENSE` & `dataquality-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/README.md` & `dataquality-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/__init__.py` & `dataquality-0.8.9/dataquality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 "dataquality"
 
-__version__ = "v0.8.8a0"
+__version__ = "v0.8.9"
 
 import os
 
 import dataquality.core._config
 import dataquality.integrations
 
 # We try/catch this in case the user installed dq inside of jupyter. You need to
```

### Comparing `dataquality-0.8.8a0/dataquality/analytics.py` & `dataquality-0.8.9/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/clients/api.py` & `dataquality-0.8.9/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/clients/objectstore.py` & `dataquality-0.8.9/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/core/_config.py` & `dataquality-0.8.9/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/core/auth.py` & `dataquality-0.8.9/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/core/finish.py` & `dataquality-0.8.9/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/core/init.py` & `dataquality-0.8.9/dataquality/core/init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/core/log.py` & `dataquality-0.8.9/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/core/report.py` & `dataquality-0.8.9/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/dq_auto/auto.py` & `dataquality-0.8.9/dataquality/dq_auto/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.8.9/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/dq_auto/ner.py` & `dataquality-0.8.9/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.8.9/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.8.9/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/dq_auto/text_classification.py` & `dataquality-0.8.9/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/integrations/experimental/keras.py` & `dataquality-0.8.9/dataquality/integrations/experimental/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/integrations/hf.py` & `dataquality-0.8.9/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/integrations/keras.py` & `dataquality-0.8.9/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/integrations/spacy.py` & `dataquality-0.8.9/dataquality/integrations/spacy.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/integrations/torch.py` & `dataquality-0.8.9/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/integrations/transformers_trainer.py` & `dataquality-0.8.9/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/base_logger.py` & `dataquality-0.8.9/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.8.9/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/data_logger/image_classification.py` & `dataquality-0.8.9/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.8.9/dataquality/loggers/data_logger/text_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         super().validate()
         label_len = len(self.labels)
         text_len = len(self.texts)
         id_len = len(self.ids)
 
         set_labels_are_ints = self.logger_config.int_labels
 
-        if self.split != Split.inference and (isinstance(self.labels[0], int)):
+        if self.split != Split.inference and str(self.labels[0]).isnumeric():
             # labels must be set if numeric
             assert self.logger_config.labels is not None, (
                 "You must set labels before logging input data,"
                 " when label column is numeric"
             )
 
         if label_len and isinstance(self.labels[0], int) and not set_labels_are_ints:
```

### Comparing `dataquality-0.8.8a0/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.8.9/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.8.9/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.8.9/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.8.9/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.8.9/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.8.9/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.8.9/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/model_logger/image_classification.py` & `dataquality-0.8.9/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.8.9/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.8.9/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.8.9/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/metrics.py` & `dataquality-0.8.9/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/condition.py` & `dataquality-0.8.9/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/dataframe.py` & `dataquality-0.8.9/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/edit.py` & `dataquality-0.8.9/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/hf.py` & `dataquality-0.8.9/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/metrics.py` & `dataquality-0.8.9/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/ner.py` & `dataquality-0.8.9/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/report.py` & `dataquality-0.8.9/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/route.py` & `dataquality-0.8.9/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/split.py` & `dataquality-0.8.9/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/schemas/task_type.py` & `dataquality-0.8.9/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/ampli.py` & `dataquality-0.8.9/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/auto.py` & `dataquality-0.8.9/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/auto_trainer.py` & `dataquality-0.8.9/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/cv.py` & `dataquality-0.8.9/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/dq_logger.py` & `dataquality-0.8.9/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/hdf5_store.py` & `dataquality-0.8.9/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/helpers.py` & `dataquality-0.8.9/dataquality/utils/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import webbrowser
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar
 
 from typing_extensions import ParamSpec
 
 T = TypeVar("T")
 P = ParamSpec("P")
@@ -94,15 +95,14 @@
     work in colab (because colab is running on a server, so there's no "browser" to
     interact with). This also prints out the link for users to click so even in those
     environments they still have something to interact with.
     """
     if not link:
         return
     try:
-        import webbrowser
 
         webbrowser.open(link)
     # In some environments, webbrowser will raise. Other times it fails silently (colab)
     except Exception:
         pass
     finally:
         print(f"Click here to see your run! {link}")
```

### Comparing `dataquality-0.8.8a0/dataquality/utils/hf_tokenizer.py` & `dataquality-0.8.9/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/keras.py` & `dataquality-0.8.9/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/ml.py` & `dataquality-0.8.9/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/name.py` & `dataquality-0.8.9/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/profiler.py` & `dataquality-0.8.9/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/spacy_integration.py` & `dataquality-0.8.9/dataquality/utils/spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/thread_pool.py` & `dataquality-0.8.9/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/torch.py` & `dataquality-0.8.9/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/transformers.py` & `dataquality-0.8.9/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/vaex.py` & `dataquality-0.8.9/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/dataquality/utils/version.py` & `dataquality-0.8.9/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/docs/Dataquality-Client-Demo.ipynb` & `dataquality-0.8.9/docs/Dataquality-Client-Demo.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/docs/End to End runs per task type.ipynb` & `dataquality-0.8.9/docs/End to End runs per task type.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/docs/Inference-Demo.ipynb` & `dataquality-0.8.9/docs/Inference-Demo.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/docs/NER Inference.ipynb` & `dataquality-0.8.9/docs/NER Inference.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/docs/cv/cv-demo-hf.py` & `dataquality-0.8.9/docs/cv/cv-demo-hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/docs/cv/cv-testing-benchmark.py` & `dataquality-0.8.9/docs/cv/cv-testing-benchmark.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/pyproject.toml` & `dataquality-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/auto/test_ner_auto.py` & `dataquality-0.8.9/tests/auto/test_ner_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/auto/test_tc_auto.py` & `dataquality-0.8.9/tests/auto/test_tc_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/clients/test_api.py` & `dataquality-0.8.9/tests/clients/test_api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/conftest.py` & `dataquality-0.8.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/core/test_auth.py` & `dataquality-0.8.9/tests/core/test_auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/core/test_config.py` & `dataquality-0.8.9/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/core/test_finish.py` & `dataquality-0.8.9/tests/core/test_finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/core/test_init.py` & `dataquality-0.8.9/tests/core/test_init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/core/test_report.py` & `dataquality-0.8.9/tests/core/test_report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/inference/test_inference.py` & `dataquality-0.8.9/tests/inference/test_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/inference/test_text_classification_inf.py` & `dataquality-0.8.9/tests/inference/test_text_classification_inf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/inference/test_text_ner_inf.py` & `dataquality-0.8.9/tests/inference/test_text_ner_inf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integration/mock_training_run.py` & `dataquality-0.8.9/tests/integration/mock_training_run.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/hf/test_cv_hf.py` & `dataquality-0.8.9/tests/integrations/hf/test_cv_hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/hf/test_hf_integration.py` & `dataquality-0.8.9/tests/integrations/hf/test_hf_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/hf/test_text_classification_hf.py` & `dataquality-0.8.9/tests/integrations/hf/test_text_classification_hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/keras/test_experimental.py` & `dataquality-0.8.9/tests/integrations/keras/test_experimental.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/keras/test_utils.py` & `dataquality-0.8.9/tests/integrations/keras/test_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/spacy/conftest.py` & `dataquality-0.8.9/tests/integrations/spacy/conftest.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/spacy/test_spacy_integration.py` & `dataquality-0.8.9/tests/integrations/spacy/test_spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/spacy/test_spacy_ner.py` & `dataquality-0.8.9/tests/integrations/spacy/test_spacy_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/torch/test_pt_utils.py` & `dataquality-0.8.9/tests/integrations/torch/test_pt_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/integrations/torch/test_text_classification_pt.py` & `dataquality-0.8.9/tests/integrations/torch/test_text_classification_pt.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/loggers/test_multi_label.py` & `dataquality-0.8.9/tests/loggers/test_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/loggers/test_ner.py` & `dataquality-0.8.9/tests/loggers/test_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/loggers/test_text_classification.py` & `dataquality-0.8.9/tests/loggers/test_text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/schemas/test_conditions.py` & `dataquality-0.8.9/tests/schemas/test_conditions.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_dataquality.py` & `dataquality-0.8.9/tests/test_dataquality.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_telemetrics.py` & `dataquality-0.8.9/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/data_utils.py` & `dataquality-0.8.9/tests/test_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/hf_datasets_mock.py` & `dataquality-0.8.9/tests/test_utils/hf_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/hf_integration_constants.py` & `dataquality-0.8.9/tests/test_utils/hf_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.8.9/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/lightning_model.py` & `dataquality-0.8.9/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/mock_request.py` & `dataquality-0.8.9/tests/test_utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/ner_constants.py` & `dataquality-0.8.9/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/spacy_integration.py` & `dataquality-0.8.9/tests/test_utils/spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/spacy_integration_constants.py` & `dataquality-0.8.9/tests/test_utils/spacy_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/test_utils/spacy_integration_constants_inference.py` & `dataquality-0.8.9/tests/test_utils/spacy_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/utils/test_auto.py` & `dataquality-0.8.9/tests/utils/test_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/utils/test_dq_logger.py` & `dataquality-0.8.9/tests/utils/test_dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/utils/test_vaex_utils.py` & `dataquality-0.8.9/tests/utils/test_vaex_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/tests/utils/test_version.py` & `dataquality-0.8.9/tests/utils/test_version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.8a0/PKG-INFO` & `dataquality-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.8.8a0
+Version: 0.8.9
 Summary: dataquality
 Home-page: https://www.github.com/rungalileo/dataquality
 Author: Galileo Technologies, Inc
 Author-email: team@rungalileo.io
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.8.2
```

