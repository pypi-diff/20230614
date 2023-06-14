# Comparing `tmp/lolpop-0.1.0a5.tar.gz` & `tmp/lolpop-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolpop-0.1.0a5.tar", max compression
+gzip compressed data, was "lolpop-0.1.0a6.tar", max compression
```

## Comparing `lolpop-0.1.0a5.tar` & `lolpop-0.1.0a6.tar`

### file list

```diff
@@ -1,157 +1,165 @@
--rw-r--r--   0        0        0    11357 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/LICENSE
--rw-r--r--   0        0        0      220 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/__init__.py
--rw-r--r--   0        0        0     2552 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/cli.py
--rw-r--r--   0        0        0    12841 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/create.py
--rw-r--r--   0        0        0     3464 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/datagen.py
--rw-r--r--   0        0        0      432 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/package.py
--rw-r--r--   0        0        0     1928 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/run.py
--rw-r--r--   0        0        0     2037 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/seed.py
--rw-r--r--   0        0        0      451 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/test.py
--rw-r--r--   0        0        0     1311 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/__init__.py
--rw-r--r--   0        0        0     3744 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/base_component.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/__init__.py
--rw-r--r--   0        0        0      164 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/base_data_checker.py
--rw-r--r--   0        0        0     2160 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/deepchecks_data_checker.py
--rw-r--r--   0        0        0     1813 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/evidentlyai_data_checker.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/__init__.py
--rw-r--r--   0        0        0      233 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/base_data_connector.py
--rw-r--r--   0        0        0     6265 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/bigquery_data_connector.py
--rw-r--r--   0        0        0     5431 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/databricks_sql_data_connector.py
--rw-r--r--   0        0        0     4122 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/duckdb_data_connector.py
--rw-r--r--   0        0        0     4275 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/gcs_data_connector.py
--rw-r--r--   0        0        0     1299 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/local_data_connector.py
--rw-r--r--   0        0        0     5453 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/postgres_data_connector.py
--rw-r--r--   0        0        0      637 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/redshift_data_connector.py
--rw-r--r--   0        0        0     3352 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_connector/s3_data_connector.py
--rw-r--r--   0        0        0     6484 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_connector/snowflake_data_connector.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/__init__.py
--rw-r--r--   0        0        0      243 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/base_data_profiler.py
--rw-r--r--   0        0        0     1462 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/continual_data_profiler.py
--rw-r--r--   0        0        0     2314 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/evidentlyai_data_profiler.py
--rw-r--r--   0        0        0     2162 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/sweetviz_data_profiler.py
--rw-r--r--   0        0        0     1912 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_splitter/__init__.py
--rw-r--r--   0        0        0      163 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_splitter/base_data_splitter.py
--rw-r--r--   0        0        0     8542 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_splitter/local_data_splitter.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_synthesizer/__init__.py
--rw-r--r--   0        0        0      396 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_synthesizer/base_data_synthesizer.py
--rw-r--r--   0        0        0     5878 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_synthesizer/svd_data_synthesizer.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/__init__.py
--rw-r--r--   0        0        0      301 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/base_data_transformer.py
--rw-r--r--   0        0        0      712 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/bigquery_data_transformer.py
--rw-r--r--   0        0        0      870 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/databricks_sql_data_transformer.py
--rw-r--r--   0        0        0     4525 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/dbt_data_transformer.py
--rw-r--r--   0        0        0      613 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/duckdb_data_transformer.py
--rw-r--r--   0        0        0     2472 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/local_data_transformer.py
--rw-r--r--   0        0        0      838 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/postrgres_data_transformer.py
--rw-r--r--   0        0        0      962 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/redshift_data_transformer.py
--rw-r--r--   0        0        0      855 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/snowflake_data_transformer.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/genai_chatbot/__init__.py
--rw-r--r--   0        0        0      228 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/genai_chatbot/base_genai_chatbot.py
--rw-r--r--   0        0        0      940 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/genai_chatbot/openai_chatbot.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/__init__.py
--rw-r--r--   0        0        0     2346 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
--rw-r--r--   0        0        0     2755 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
--rw-r--r--   0        0        0     9180 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/__init__.py
--rw-r--r--   0        0        0      139 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/base_logger.py
--rw-r--r--   0        0        0     1699 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/file_logger.py
--rw-r--r--   0        0        0     2017 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/stdout_logger.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/__init__.py
--rw-r--r--   0        0        0     2073 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/base_metadata_tracker.py
--rw-r--r--   0        0        0    15598 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/continual_metadata_tracker.py
--rw-r--r--   0        0        0    12388 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/__init__.py
--rw-r--r--   0        0        0      460 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/base_metrics_tracker.py
--rw-r--r--   0        0        0     5843 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/continual_metrics_tracker.py
--rw-r--r--   0        0        0     4804 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_bias_checker/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
--rw-r--r--   0        0        0      240 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_bias_checker/base_model_bias_checker.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/__init__.py
--rw-r--r--   0        0        0     5574 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/base_model_checker.py
--rw-r--r--   0        0        0     2848 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/deepchecks_model_checker.py
--rw-r--r--   0        0        0     3408 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/evidentlyai_model_checker.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_deployer/__init__.py
--rw-r--r--   0        0        0      371 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_deployer/base_model_deployer.py
--rw-r--r--   0        0        0      574 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_deployer/seldon_model_deployer.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_explainer/__init__.py
--rw-r--r--   0        0        0     8917 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_explainer/alibi_model_explainer.py
--rw-r--r--   0        0        0      244 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_explainer/base_model_explainer.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/__init__.py
--rw-r--r--   0        0        0      309 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/base_model_repository.py
--rw-r--r--   0        0        0     2993 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/continual_model_repository.py
--rw-r--r--   0        0        0     4521 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/mlflow_model_repository.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_trainer/__init__.py
--rw-r--r--   0        0        0     7260 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_trainer/base_model_trainer.py
--rw-r--r--   0        0        0     2407 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_trainer/xgboost_model_trainer.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_visualizer/__init__.py
--rw-r--r--   0        0        0      169 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_visualizer/base_model_visualizer.py
--rw-r--r--   0        0        0     3881 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/__init__.py
--rw-r--r--   0        0        0      156 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/base_notifier.py
--rw-r--r--   0        0        0     2904 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/gmail_notifier.py
--rw-r--r--   0        0        0      880 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/slack_notifier.py
--rw-r--r--   0        0        0     1272 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/smtp_notifier.py
--rw-r--r--   0        0        0      322 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/stdout_notifier.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/__init__.py
--rw-r--r--   0        0        0      376 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/base_resource_version_control.py
--rw-r--r--   0        0        0     3221 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/continual_version_control.py
--rw-r--r--   0        0        0     5828 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/dvc_version_control.py
--rw-r--r--   0        0        0     2346 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/extension/__init__.py
--rw-r--r--   0        0        0     1299 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/__init__.py
--rw-r--r--   0        0        0     4967 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/base_pipeline.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/__init__.py
--rw-r--r--   0        0        0      454 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/base_deploy.py
--rw-r--r--   0        0        0     3849 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/metaflow_offline_deploy.py
--rw-r--r--   0        0        0     1660 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/offline_deploy.py
--rw-r--r--   0        0        0       42 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/__init__.py
--rw-r--r--   0        0        0      227 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/base_predict.py
--rw-r--r--   0        0        0     7182 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/metaflow_offline_predict.py
--rw-r--r--   0        0        0     4137 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/offline_predict.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/__init__.py
--rw-r--r--   0        0        0      452 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/base_process.py
--rw-r--r--   0        0        0     5459 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/metaflow_offline_process.py
--rw-r--r--   0        0        0     3267 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/offline_process.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/__init__.py
--rw-r--r--   0        0        0      645 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/base_train.py
--rw-r--r--   0        0        0     7474 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/metaflow_offline_train.py
--rw-r--r--   0        0        0     4499 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/offline_train.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/wrapper/__init__.py
--rw-r--r--   0        0        0      275 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/wrapper/base_wrapper.py
--rw-r--r--   0        0        0      789 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
--rw-r--r--   0        0        0     1285 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/__init__.py
--rw-r--r--   0        0        0     7121 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/base_runner.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/classification_runner/__init__.py
--rw-r--r--   0        0        0     7686 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/classification_runner/classification_runner.py
--rw-r--r--   0        0        0     6130 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/classification_runner/metaflow_classification.py
--rw-r--r--   0        0        0      175 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/templates/component_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
--rw-r--r--   0        0        0      802 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
--rw-r--r--   0        0        0     1122 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
--rw-r--r--   0        0        0      167 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
--rw-r--r--   0        0        0      803 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
--rw-r--r--   0        0        0     1096 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
--rw-r--r--   0        0        0       66 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0       32 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0     1418 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
--rw-r--r--   0        0        0     1408 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
--rw-r--r--   0        0        0     1363 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
--rw-r--r--   0        0        0      310 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      151 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
--rw-r--r--   0        0        0      795 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
--rw-r--r--   0        0        0     1054 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
--rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/__init__.py
--rw-r--r--   0        0        0    16250 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/common_utils.py
--rw-r--r--   0        0        0     1566 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/continual_utils.py
--rw-r--r--   0        0        0     2452 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/metaflow_utils.py
--rw-r--r--   0        0        0     3298 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/mlflow_utils.py
--rw-r--r--   0        0        0     2261 2023-05-20 04:33:29.454445 lolpop-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 lolpop-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 04:39:46.158228 lolpop-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0      373 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/__init__.py
+-rw-r--r--   0        0        0     2552 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/cli.py
+-rw-r--r--   0        0        0    12841 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/create.py
+-rw-r--r--   0        0        0     3464 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/datagen.py
+-rw-r--r--   0        0        0      432 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/package.py
+-rw-r--r--   0        0        0     1928 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/run.py
+-rw-r--r--   0        0        0     2037 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/seed.py
+-rw-r--r--   0        0        0      451 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/cli/test.py
+-rw-r--r--   0        0        0     1311 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/__init__.py
+-rw-r--r--   0        0        0     3752 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/base_component.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_checker/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_checker/base_data_checker.py
+-rw-r--r--   0        0        0     2160 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_checker/deepchecks_data_checker.py
+-rw-r--r--   0        0        0     1813 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_checker/evidentlyai_data_checker.py
+-rw-r--r--   0        0        0     2650 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_checker/stumpy_matrix_profiler.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/base_data_connector.py
+-rw-r--r--   0        0        0     6265 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/bigquery_data_connector.py
+-rw-r--r--   0        0        0     5431 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/databricks_sql_data_connector.py
+-rw-r--r--   0        0        0     4188 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/duckdb_data_connector.py
+-rw-r--r--   0        0        0     4275 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/gcs_data_connector.py
+-rw-r--r--   0        0        0     1299 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/local_data_connector.py
+-rw-r--r--   0        0        0     5453 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/postgres_data_connector.py
+-rw-r--r--   0        0        0      637 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/redshift_data_connector.py
+-rw-r--r--   0        0        0     3352 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/s3_data_connector.py
+-rw-r--r--   0        0        0     6484 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_connector/snowflake_data_connector.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_profiler/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_profiler/base_data_profiler.py
+-rw-r--r--   0        0        0     1462 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_profiler/continual_data_profiler.py
+-rw-r--r--   0        0        0     2314 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_profiler/evidentlyai_data_profiler.py
+-rw-r--r--   0        0        0     2162 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_profiler/sweetviz_data_profiler.py
+-rw-r--r--   0        0        0     1087 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_profiler/tslumen_data_profiler.py
+-rw-r--r--   0        0        0     2164 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_splitter/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_splitter/base_data_splitter.py
+-rw-r--r--   0        0        0     9612 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_splitter/local_data_splitter.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_synthesizer/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_synthesizer/base_data_synthesizer.py
+-rw-r--r--   0        0        0     5878 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_synthesizer/svd_data_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/base_data_transformer.py
+-rw-r--r--   0        0        0      712 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/bigquery_data_transformer.py
+-rw-r--r--   0        0        0      870 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/databricks_sql_data_transformer.py
+-rw-r--r--   0        0        0     4525 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/dbt_data_transformer.py
+-rw-r--r--   0        0        0      613 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/duckdb_data_transformer.py
+-rw-r--r--   0        0        0     2472 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/local_data_transformer.py
+-rw-r--r--   0        0        0      838 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/postrgres_data_transformer.py
+-rw-r--r--   0        0        0      962 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/redshift_data_transformer.py
+-rw-r--r--   0        0        0      855 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/data_transformer/snowflake_data_transformer.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/genai_chatbot/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/genai_chatbot/base_genai_chatbot.py
+-rw-r--r--   0        0        0      940 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/genai_chatbot/openai_chatbot.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/hyperparameter_tuner/__init__.py
+-rw-r--r--   0        0        0     2705 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     2755 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     9416 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/logger/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/logger/base_logger.py
+-rw-r--r--   0        0        0     1699 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/logger/file_logger.py
+-rw-r--r--   0        0        0     2017 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/logger/stdout_logger.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metadata_tracker/__init__.py
+-rw-r--r--   0        0        0     2073 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metadata_tracker/base_metadata_tracker.py
+-rw-r--r--   0        0        0    15598 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metadata_tracker/continual_metadata_tracker.py
+-rw-r--r--   0        0        0    12571 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metrics_tracker/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metrics_tracker/base_metrics_tracker.py
+-rw-r--r--   0        0        0     5843 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metrics_tracker/continual_metrics_tracker.py
+-rw-r--r--   0        0        0     4804 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/model_bias_checker/__init__.py
+-rw-r--r--   0        0        0     3960 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
+-rw-r--r--   0        0        0      240 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/model_bias_checker/base_model_bias_checker.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/model_checker/__init__.py
+-rw-r--r--   0        0        0     9228 2023-05-29 04:39:46.162229 lolpop-0.1.0a6/lolpop/component/model_checker/base_model_checker.py
+-rw-r--r--   0        0        0     2846 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_checker/deepchecks_model_checker.py
+-rw-r--r--   0        0        0     3404 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_checker/evidentlyai_model_checker.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_deployer/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_deployer/base_model_deployer.py
+-rw-r--r--   0        0        0      574 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_deployer/seldon_model_deployer.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_explainer/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_explainer/alibi_model_explainer.py
+-rw-r--r--   0        0        0      244 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_explainer/base_model_explainer.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_repository/__init__.py
+-rw-r--r--   0        0        0      309 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_repository/base_model_repository.py
+-rw-r--r--   0        0        0     2993 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_repository/continual_model_repository.py
+-rw-r--r--   0        0        0     4521 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_repository/mlflow_model_repository.py
+-rw-r--r--   0        0        0     5064 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_trainer/ProphetModelTrainer.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_trainer/__init__.py
+-rw-r--r--   0        0        0    12025 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_trainer/base_model_trainer.py
+-rw-r--r--   0        0        0     2405 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_trainer/xgboost_model_trainer.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_visualizer/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_visualizer/base_model_visualizer.py
+-rw-r--r--   0        0        0     2504 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_visualizer/prophet_visualizer.py
+-rw-r--r--   0        0        0     3881 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/notifier/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/notifier/base_notifier.py
+-rw-r--r--   0        0        0     2904 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/notifier/gmail_notifier.py
+-rw-r--r--   0        0        0      880 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/notifier/slack_notifier.py
+-rw-r--r--   0        0        0     1272 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/notifier/smtp_notifier.py
+-rw-r--r--   0        0        0      322 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/notifier/stdout_notifier.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/resource_version_control/__init__.py
+-rw-r--r--   0        0        0      376 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/resource_version_control/base_resource_version_control.py
+-rw-r--r--   0        0        0     3221 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/resource_version_control/continual_version_control.py
+-rw-r--r--   0        0        0     5828 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/component/resource_version_control/dvc_version_control.py
+-rw-r--r--   0        0        0     2661 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/__init__.py
+-rw-r--r--   0        0        0     4971 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/deploy/__init__.py
+-rw-r--r--   0        0        0      454 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/deploy/base_deploy.py
+-rw-r--r--   0        0        0     3849 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/deploy/metaflow_offline_deploy.py
+-rw-r--r--   0        0        0     1660 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/deploy/offline_deploy.py
+-rw-r--r--   0        0        0       42 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/predict/__init__.py
+-rw-r--r--   0        0        0      227 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/predict/base_predict.py
+-rw-r--r--   0        0        0     7180 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/predict/metaflow_offline_predict.py
+-rw-r--r--   0        0        0     4172 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/predict/offline_predict.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/process/__init__.py
+-rw-r--r--   0        0        0      452 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/process/base_process.py
+-rw-r--r--   0        0        0     5660 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/process/metaflow_offline_process.py
+-rw-r--r--   0        0        0     3267 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/process/offline_process.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/train/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/train/base_train.py
+-rw-r--r--   0        0        0     7331 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/train/metaflow_offline_train.py
+-rw-r--r--   0        0        0     4499 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/train/offline_train.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/wrapper/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/wrapper/base_wrapper.py
+-rw-r--r--   0        0        0      793 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
+-rw-r--r--   0        0        0     1285 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/runner/__init__.py
+-rw-r--r--   0        0        0     7121 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/runner/base_runner.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/runner/classification_runner/__init__.py
+-rw-r--r--   0        0        0     7705 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/runner/classification_runner/classification_runner.py
+-rw-r--r--   0        0        0     6167 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/runner/classification_runner/metaflow_classification.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/runner/timeseries_runner/__init__.py
+-rw-r--r--   0        0        0     8835 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/runner/timeseries_runner/timeseries_runner.py
+-rw-r--r--   0        0        0      175 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/component_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
+-rw-r--r--   0        0        0      802 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
+-rw-r--r--   0        0        0     1122 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
+-rw-r--r--   0        0        0      167 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/pipeline_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
+-rw-r--r--   0        0        0      803 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
+-rw-r--r--   0        0        0     1096 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
+-rw-r--r--   0        0        0       66 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0       32 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
+-rw-r--r--   0        0        0      152 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/__int__.py
+-rw-r--r--   0        0        0      152 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
+-rw-r--r--   0        0        0      310 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/runner_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
+-rw-r--r--   0        0        0      795 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
+-rw-r--r--   0        0        0     1054 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:39:46.166229 lolpop-0.1.0a6/lolpop/utils/__init__.py
+-rw-r--r--   0        0        0    15753 2023-05-29 04:39:46.170229 lolpop-0.1.0a6/lolpop/utils/common_utils.py
+-rw-r--r--   0        0        0     1566 2023-05-29 04:39:46.170229 lolpop-0.1.0a6/lolpop/utils/continual_utils.py
+-rw-r--r--   0        0        0     2452 2023-05-29 04:39:46.170229 lolpop-0.1.0a6/lolpop/utils/metaflow_utils.py
+-rw-r--r--   0        0        0     3298 2023-05-29 04:39:46.170229 lolpop-0.1.0a6/lolpop/utils/mlflow_utils.py
+-rw-r--r--   0        0        0     2381 2023-05-29 04:40:09.079594 lolpop-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 lolpop-0.1.0a6/PKG-INFO
```

### Comparing `lolpop-0.1.0a5/LICENSE` & `lolpop-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/cli/cli.py` & `lolpop-0.1.0a6/lolpop/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/cli/create.py` & `lolpop-0.1.0a6/lolpop/cli/create.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/cli/datagen.py` & `lolpop-0.1.0a6/lolpop/cli/datagen.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/cli/run.py` & `lolpop-0.1.0a6/lolpop/cli/run.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/cli/seed.py` & `lolpop-0.1.0a6/lolpop/cli/seed.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/__init__.py` & `lolpop-0.1.0a6/lolpop/component/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/base_component.py` & `lolpop-0.1.0a6/lolpop/component/base_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
             self.notifier.notify(msg, level)
             self.log("Notification Sent: %s" %msg, level)
 
     #helper function to lookup config key in component, pipeline or runner conf
     def _get_config(self, key, default_value=None):
         key = key.lower()
         value = utils.lower_conf(self.config).get(key, None)
-        if not value: 
+        if value is None: 
             value = utils.lower_conf(self.pipeline_conf).get(key, None)
-            if not value: 
+            if value is None: 
                 value = utils.lower_conf(self.runner_conf).get(key, default_value)
         return value
 
     def _set_config(self, key, value): 
         key = key.lower()
         self.config[key]=value
```

### Comparing `lolpop-0.1.0a5/lolpop/component/data_checker/deepchecks_data_checker.py` & `lolpop-0.1.0a6/lolpop/component/data_checker/deepchecks_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_checker/evidentlyai_data_checker.py` & `lolpop-0.1.0a6/lolpop/component/data_checker/evidentlyai_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/bigquery_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/bigquery_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/databricks_sql_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/databricks_sql_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/duckdb_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/duckdb_data_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,20 @@
         result = pd.DataFrame()
         with duckdb.connect(database = path) as con: 
             res = con.sql(sql)
             result = res.df() 
         return result
 
     def _save_data(self, data, table_name, path, table_exists):
-        with duckdb.connect(database = path) as con: 
-            if not table_exists: 
-                con.sql("CREATE TABLE %s as SELECT * from data" %table_name)
-            else: 
-                con.sql("INSERT INTO %s as SELECT * from data" % table_name)
+        if data is not None and len(data)>0: 
+            with duckdb.connect(database = path) as con: 
+                if not table_exists: 
+                    con.sql("CREATE TABLE %s as SELECT * from data" %table_name)
+                else: 
+                    con.sql("INSERT INTO %s as SELECT * from data" % table_name)
 
 
     def _map_pandas_col_type_to_duckdb_type(self, col_type):
         """_summary_
 
         Args:
             col_type (_type_): _description_
```

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/gcs_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/gcs_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/local_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/local_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/postgres_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/postgres_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/redshift_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/redshift_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/s3_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/s3_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_connector/snowflake_data_connector.py` & `lolpop-0.1.0a6/lolpop/component/data_connector/snowflake_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_profiler/continual_data_profiler.py` & `lolpop-0.1.0a6/lolpop/component/data_profiler/continual_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_profiler/evidentlyai_data_profiler.py` & `lolpop-0.1.0a6/lolpop/component/data_profiler/evidentlyai_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_profiler/sweetviz_data_profiler.py` & `lolpop-0.1.0a6/lolpop/component/data_profiler/sweetviz_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_splitter/local_data_splitter.py` & `lolpop-0.1.0a6/lolpop/component/data_splitter/local_data_splitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,60 @@
                     X_valid = Features of the validation dataset
                     y_valid = Labels of the validation dataset
                     X_test = Features of the test/holdout dataset
                     y_test = Labels of the validation dataset
 
         """
         data_out = data.drop(self._get_config("DROP_COLUMNS",[]),axis=1, errors="ignore")
-        data_out = self._split_data(
-            data_out, 
-            self._get_config("MODEL_TARGET"), 
-            split_column = self._get_config("SPLIT_COLUMN", None),
-            split_classes = self._get_config("SPLIT_CLASSES", {}),  
-            split_ratio = self._get_config("SPLIT_RATIO", [0.8, 0.2]), 
-            sample_num = self._get_config("SAMPLE_NUM", 100000), 
-            use_startified = self._get_config("USE_STRATIFIED", False),
-            include_test = self._get_config("INCLUDE_TEST", False),
+
+        if self.problem_type == "timeseries": 
+            data_out = self._split_timeseries_data(
+                data_out, 
+                self._get_config("time_index"), 
+                self._get_config("model_target"),
+                self._get_config("test_size"), 
+                self._get_config("validation_size"),
             )
+        else: 
+            data_out = self._split_data(
+                data_out, 
+                self._get_config("MODEL_TARGET"), 
+                split_column = self._get_config("SPLIT_COLUMN", None),
+                split_classes = self._get_config("SPLIT_CLASSES", {}),  
+                split_ratio = self._get_config("SPLIT_RATIO", [0.8, 0.2]), 
+                sample_num = self._get_config("SAMPLE_NUM", 100000), 
+                use_startified = self._get_config("USE_STRATIFIED", False),
+                include_test = self._get_config("INCLUDE_TEST", False),
+                )
         for key in data_out.keys():
             self.log("Created %s dataset with %s rows" %(key, data_out.get(key).shape[0]))
 
         return data_out
 
+    def _split_timeseries_data(self, data, time_index, target, test_size=0, validation_size=0,): 
+        #make sure data is ordered 
+        data_out = {}
+
+        data = data.sort_values(time_index).reset_index(drop=True)
+
+        test = None 
+        valid = None
+        train = data  
+        if test_size > 0: 
+            test = train[-test_size:].reset_index(drop=True)
+            train = train[:-test_size]
+        if validation_size > 0: 
+            valid = train[-validation_size:].reset_index(drop=True)
+            train = train[:-validation_size]
+        
+        data_out = self._build_split_dfs(train, valid, target, test=test)
+
+        return data_out 
+
+
     def _split_data(self, data, target,  split_column=None, split_classes={},  split_ratio=[0.8,0.2], sample_num=100000, use_startified=False, include_test=False): 
         """ Function to split data. 
             Supports random splitting, manual splitting, and stratified. 
             Can also include test set. 
 
         Args:
             data (pd.DataFrame): Dataframe to split
```

### Comparing `lolpop-0.1.0a5/lolpop/component/data_synthesizer/svd_data_synthesizer.py` & `lolpop-0.1.0a6/lolpop/component/data_synthesizer/svd_data_synthesizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/bigquery_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/bigquery_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/databricks_sql_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/databricks_sql_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/dbt_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/dbt_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/duckdb_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/duckdb_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/local_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/local_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/postrgres_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/postrgres_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/redshift_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/redshift_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/data_transformer/snowflake_data_transformer.py` & `lolpop-0.1.0a6/lolpop/component/data_transformer/snowflake_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/genai_chatbot/openai_chatbot.py` & `lolpop-0.1.0a6/lolpop/component/genai_chatbot/openai_chatbot.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py` & `lolpop-0.1.0a6/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     __REQUIRED_CONF__ = {
         "config" : ["training_params", "metrics", "perf_metric"]
     }
     
     def run_experiment(self, data, *args, **kwargs): 
         pass 
 
-    def build_model(self, data, model_version, algo, params): 
+    def build_model(self, data, model_version, algo, params, trainer_config={}): 
         #create experiment and log params
         experiment = self.metadata_tracker.create_resource(id=None, type="experiment", parent=model_version)
 
         #load model trainer and build model
         model_cl = utils.load_class(algo)
         dependent_components = {"logger" : self.logger, "notifier" : self.notifier,  "metadata_tracker" :self.metadata_tracker, "metrics_tracker": self.metrics_tracker, "resource_version_control": self.resource_version_control}
-        model = model_cl(conf=self.config, pipeline_conf=self.pipeline_conf, runner_conf=self.runner_conf, 
+        model = model_cl(conf=trainer_config, pipeline_conf=self.pipeline_conf, runner_conf=self.runner_conf, 
                          parent_process = self.name, problem_type = self.problem_type, params=params, components=dependent_components) 
         model_obj = model.fit(data)
 
         return model, experiment 
 
     def save_model(self, model, experiment, params, algo, **kwargs):
         model_obj = model._get_model()
@@ -30,20 +30,25 @@
         vc_info = self.resource_version_control.version_model(experiment, model_obj, algo=algo)
         experiment_metadata = {
             "training_params" : params,
             "model_trainer" : algo, 
         }
         self.metadata_tracker.register_vc_resource(experiment, vc_info, additional_metadata = experiment_metadata)
 
+        experiment_id = self.metadata_tracker.get_resource_id(experiment, type="experiment")
+        model_artifacts = model.get_artifacts(experiment_id) or {}
+        for k,v in model_artifacts.items(): 
+            self.metadata_tracker.log_artifact(experiment, k, v)
 
     #builds a grid of all possible parameter combinations gives a params item with a list of values for each param
     def _build_training_grid(self, params): 
         keys, values = zip(*params.items())
         values = [v if isinstance(v, ListConfig) else str(v).split(",") for v in values]
         grid = [dict(zip(keys,v)) for v in itertools.product(*values)]
 
         return grid
 
     #determines the winning experiment from the experiment list 
     def _get_winning_experiment(self, exp_list, perf_metric, reverse): 
-        new_list = sorted(exp_list.items(), key=lambda x: x[1], reverse=reverse) # sort list by values
+        # sort list by values. reverse=True is descending, False is ascending (Default)
+        new_list = sorted(exp_list.items(), key=lambda x: x[1], reverse=reverse) 
         return new_list[0][0]
```

### Comparing `lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py` & `lolpop-0.1.0a6/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py` & `lolpop-0.1.0a6/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,43 +3,48 @@
 import optuna
 from datetime import datetime
 import os
 
 @utils.decorate_all_methods([utils.error_handler,utils.log_execution()])
 class OptunaHyperparameterTuner(BaseHyperparameterTuner): 
 
-    def run_experiment(self, data, model_version, n_trials=100, timeout=600, *args, **kwargs): 
+    def run_experiment(self, data, model_version, n_trials=100, *args, **kwargs): 
         #set up params
         training_params = self._get_config("training_params")
+        trainer_configs = self._get_config("trainer_configs", {})
         param_type = self._get_config("param_type", "fixed")
         metrics = self._get_config("metrics")
         perf_metric = self._get_config("perf_metric")
+        # default to 1 hr timeout
+        timeout = self._get_config("optuna_timeout", 3600)
+        n_jobs = self._get_config("num_jobs", 1)
 
         #understand if we want to minimize or maximum objective for optuna
         reverse = utils.get_metric_direction(perf_metric)
         direction = "maximize"
-        if reverse: 
+        if not reverse: 
             direction = "minimize"
-            
+ 
         exp_list = {} 
         model_list = {}
         for algo in training_params: 
             #need to create study w/ sampler so that the results are reproducible later on
             sampler = optuna.samplers.TPESampler(seed=42) 
             study_name = self.metadata_tracker.get_resource_id(model_version)
             study = optuna.create_study(direction=direction, sampler=sampler, study_name=study_name)
             if param_type == "fixed":
                 grid = self._build_training_grid(training_params[algo])
+                #only run n_trials = len(grid) to only run enqued params
+                n_trials = len(grid)
+                self.log("Found %s parameter combinations. Proceeding to enqueue all combinations..." %n_trials)
                 #enqueue all fixed params
                 for params in grid: 
                     study.enqueue_trial(params)   
-                #only run n_trials = len(grid) to only run enqued params
-                n_trials = len(grid)
             #run study
-            study.optimize(lambda trial: self._optuna_objective(trial, param_type, data, model_version, algo, training_params[algo], metrics, perf_metric, exp_list, model_list), n_trials=n_trials, timeout=timeout)
+            study.optimize(lambda trial: self._optuna_objective(trial, param_type, data, model_version, algo, training_params[algo], trainer_configs.get(algo,{}), metrics, perf_metric, exp_list, model_list), n_trials=n_trials, timeout=timeout, n_jobs=n_jobs)
             #log study
             #study.set_user_attr("perf_metric_name", perf_metric)
             #study.set_user_attr("perf_metric_val", study.best_value)
             self._log_study(study, model_version, algo) #returns best exp id 
             #get best experiment in study
             #best_experiment = study.best_trial.user_attrs.get("experiment_id")
             #exp_model = study.best_trial.user_attrs.get("model")
@@ -48,35 +53,33 @@
 
         #save data splits
         for k,v in data.items(): 
             vc_info = self.resource_version_control.version_data(model_version, v, key=k)
             self.metadata_tracker.register_vc_resource(model_version, vc_info, key=k, file_type="csv")
 
         #now, we determine overall best experiment and save into model_version
-        winning_exp_id = self._get_winning_experiment(exp_list, perf_metric, reverse=utils.get_metric_direction(perf_metric))
+        winning_exp_id = self._get_winning_experiment(exp_list, perf_metric, reverse=reverse)
         winning_exp = self.metadata_tracker.get_resource(winning_exp_id, parent=model_version, type="experiment")
         winning_exp_model_trainer = self.metadata_tracker.get_metadata(winning_exp, id="model_trainer")
         best_model = model_list.get(winning_exp_id)
 
         #log important stuff to model version
         self.metrics_tracker.copy_metrics(winning_exp, model_version)
         self.metadata_tracker.log_metadata(model_version, id="winning_experiment_id", data=winning_exp_id)
         self.metadata_tracker.log_metadata(model_version, id="winning_experiment_model_trainer", data=winning_exp_model_trainer)
       
         return best_model
 
-    def _optuna_objective(self, trial, param_type, data, model_version, algo, params, metrics, perf_metric, experiment_list, model_list): 
-        #if we are dynamic we just need to modify the paramst to use suggest_x to dynamically create values 
-
+    def _optuna_objective(self, trial, param_type, data, model_version, algo, params, trainer_config, metrics, perf_metric, experiment_list, model_list): 
         if param_type == "dynamic": 
             model_params = self._get_dynamic_params(trial, params)
         else: #param_type=="fixed"
             model_params = self._get_fixed_params(trial, params)
         #build model
-        model, experiment = self.build_model(data, model_version, algo, model_params)
+        model, experiment = self.build_model(data, model_version, algo, model_params, trainer_config)
         #make predictions
         predictions = model.predict(data)
         #calculate metrics
         metrics_val = model.calculate_metrics(data, predictions, metrics)
         perf_metric_value = metrics_val["valid"][perf_metric]
 
         #need to save exp model now because optuna doesn't provide access to models objects later on.
```

### Comparing `lolpop-0.1.0a5/lolpop/component/logger/file_logger.py` & `lolpop-0.1.0a6/lolpop/component/logger/file_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/logger/stdout_logger.py` & `lolpop-0.1.0a6/lolpop/component/logger/stdout_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/metadata_tracker/base_metadata_tracker.py` & `lolpop-0.1.0a6/lolpop/component/metadata_tracker/base_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/metadata_tracker/continual_metadata_tracker.py` & `lolpop-0.1.0a6/lolpop/component/metadata_tracker/continual_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py` & `lolpop-0.1.0a6/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,29 +248,33 @@
         id = id + "_data_comparison"
         self.log_artifact(resource, id, file_path)
 
     def stop(self):
         mlflow_utils.stop_run(self.run.info.run_id, self.run.info.experiment_id)
 
     #should this live in model_repository?
-    def load_model(self, model_obj, model_version, ref_model, *args, **kwargs):
-        model_trainer = self.get_metadata(
-            model_version, "winning_experiment_model_trainer")
+    def load_model(self, model_obj, model_version, ref_model, pipeline_config={}, *args, **kwargs):
+        model_trainer = self.get_metadata(model_version, "winning_experiment_model_trainer")
         model_cl = utils.load_class(model_trainer)
         dependent_components = {"logger": self.logger, "notifier": self.notifier,  "metadata_tracker": self.metadata_tracker,
                                 "metrics_tracker": self.metrics_tracker, "resource_version_control": self.resource_version_control}
         #might want to find a better way to do this next step.
         #it would be nice if you could reconstruct a model trainer class only w/ a model version object
         if ref_model is not None:
             config = ref_model.config
             parent_process = ref_model.parent_process
             params = ref_model.params
+            pipeline_conf = ref_model.pipeline_conf
         else:
             config = {}
             parent_process = self.parent_process
             params = {}
-        model = model_cl(conf=config, pipeline_conf=self.config, runner_conf=self.runner_conf, parent_process=parent_process,
+            pipeline_conf = {}
+        if len(pipeline_config) > 0:
+            pipeline_conf = pipeline_config 
+        
+        model = model_cl(conf=config, pipeline_conf=pipeline_conf, runner_conf=self.runner_conf, parent_process=parent_process,
                          problem_type=self.problem_type, params=params, components=dependent_components)
         #if you passed in a model_obj, we assume you have a pre-trained model object you wish to use
         if model_obj is not None:
             model._set_model(model_obj)
         return model
```

### Comparing `lolpop-0.1.0a5/lolpop/component/metrics_tracker/continual_metrics_tracker.py` & `lolpop-0.1.0a6/lolpop/component/metrics_tracker/continual_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py` & `lolpop-0.1.0a6/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py` & `lolpop-0.1.0a6/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/model_checker/deepchecks_model_checker.py` & `lolpop-0.1.0a6/lolpop/component/model_checker/deepchecks_model_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         model_target = self._get_config("MODEL_TARGET")
         model_index = self._get_config("MODEL_INDEX")
         model_time_index = self._get_config("MODEL_TIME_INDEX")
         model_cat_features = self._get_config("MODEL_CAT_FEATURES")
 
         df_current = data["X_test"].copy() 
         df_deployed = df_current.copy()
-        df_current["prediction"] = current_model._predict_df(df_current)
-        df_deployed["prediction"] = deployed_model._predict_df(df_deployed)
+        df_current["prediction"] = current_model.predict_df(df_current)
+        df_deployed["prediction"] = deployed_model.predict_df(df_deployed)
 
         ds_current = Dataset(df_current, label = "prediction", index_name=model_index, cat_features=model_cat_features, datetime_name=model_time_index)
         ds_deployed = Dataset(df_deployed, label = "prediction", index_name=model_index, cat_features=model_cat_features, datetime_name=model_time_index)
       
         check = TrainTestLabelDrift()
         model_report = check.run(train_dataset=ds_deployed, test_dataset=ds_current)
```

### Comparing `lolpop-0.1.0a5/lolpop/component/model_checker/evidentlyai_model_checker.py` & `lolpop-0.1.0a6/lolpop/component/model_checker/evidentlyai_model_checker.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         column_mapping = ColumnMapping()
         model_target = self._get_config("MODEL_TARGET")
         column_mapping.target = model_target
         column_mapping.prediction = "prediction"
 
         #set up data + predictions for train/test drift
         df_train, df_test = self.data_splitter.get_train_test_dfs(data_dict) 
-        df_train["prediction"] = model._predict_df(df_train.drop([model_target], axis=1))
-        df_test["prediction"] = model._predict_df(df_test.drop([model_target], axis=1))
+        df_train["prediction"] = model.predict_df(df_train.drop([model_target], axis=1))
+        df_test["prediction"] = model.predict_df(df_test.drop([model_target], axis=1))
 
         if self.problem_type == "classification": 
             if classification_type == "multiclass": 
                 model_report = TestSuite(tests=[MulticlassClassificationTestPreset(), NoTargetPerformanceTestPreset(), TestColumnDrift(column_name=model_target)])
             else: 
                 model_report = TestSuite(tests=[BinaryClassificationTestPreset(), NoTargetPerformanceTestPreset(), TestColumnDrift(column_name=model_target)])
             model_report.run(current_data=df_test, reference_data=df_train, column_mapping=column_mapping)
@@ -52,16 +52,16 @@
         df_current = data["X_test"].copy() 
         df_deployed = df_current.copy()
 
         #create column mapping
         column_mapping = ColumnMapping()
         column_mapping.target=self._get_config("model_target")
         column_mapping.target="prediction"
-        df_current["prediction"] = current_model._predict_df(df_current)
-        df_deployed["prediction"] = deployed_model._predict_df(df_deployed)
+        df_current["prediction"] = current_model.predict_df(df_current)
+        df_deployed["prediction"] = deployed_model.predict_df(df_deployed)
 
         #drift_report = TestSuite(tests=[TestColumnDrift(column_name="prediction")])
         drift_report = Report(metrics = [TargetDriftPreset()])
 
         drift_report.run(current_data=df_current, reference_data=df_deployed, column_mapping=column_mapping)
         file_path = "%s/EVIDENTLY_MODEL_DRIFT_REPORT.HTML" %self._get_config("local_dir")
         drift_report.save_html(file_path)
```

### Comparing `lolpop-0.1.0a5/lolpop/component/model_deployer/seldon_model_deployer.py` & `lolpop-0.1.0a6/lolpop/component/model_deployer/seldon_model_deployer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/model_explainer/alibi_model_explainer.py` & `lolpop-0.1.0a6/lolpop/component/model_explainer/alibi_model_explainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/model_repository/continual_model_repository.py` & `lolpop-0.1.0a6/lolpop/component/model_repository/continual_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/model_repository/mlflow_model_repository.py` & `lolpop-0.1.0a6/lolpop/component/model_repository/mlflow_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/model_trainer/xgboost_model_trainer.py` & `lolpop-0.1.0a6/lolpop/component/model_trainer/xgboost_model_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         #self.predictions = predictions
 
         return predictions 
 
     #def save(self, experiment, *args, **kwargs): 
     #    pass
 
-    def _predict_df(self,df): 
+    def predict_df(self,df): 
         return self.model.predict(df)
 
-    def _predict_proba_df(self,df, to_list=False): 
+    def predict_proba_df(self,df, to_list=False): 
         predictions = self.model.predict_proba(df)
         if to_list: 
             predictions = predictions.tolist()
         return predictions
```

### Comparing `lolpop-0.1.0a5/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py` & `lolpop-0.1.0a6/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/notifier/gmail_notifier.py` & `lolpop-0.1.0a6/lolpop/component/notifier/gmail_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/notifier/slack_notifier.py` & `lolpop-0.1.0a6/lolpop/component/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/notifier/smtp_notifier.py` & `lolpop-0.1.0a6/lolpop/component/notifier/smtp_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/resource_version_control/continual_version_control.py` & `lolpop-0.1.0a6/lolpop/component/resource_version_control/continual_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/component/resource_version_control/dvc_version_control.py` & `lolpop-0.1.0a6/lolpop/component/resource_version_control/dvc_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/extension/__init__.py` & `lolpop-0.1.0a6/lolpop/extension/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,51 @@
+from pkgutil import extend_path
+
+#allows extensions to work when doing local dev
+__path__ = extend_path(__path__, __name__)
+
 def __map_extensions__():
     from pathlib import Path
     import os
     from importlib import import_module
     from inspect import isclass
     from lolpop.component.base_component import BaseComponent
     from lolpop.pipeline.base_pipeline import BasePipeline
     from lolpop.runner.base_runner import BaseRunner
     import warnings
 
     warnings.filterwarnings("ignore")
     #get current directory and all subdirectors. These represent the extensions 
     # resource types
-    path = Path(__file__).parent.resolve() #lolpop/extension
-    extensions = ["%s/%s" % (path, x) for x in os.listdir(path)
-                  if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
-    #iterate through extensions and add each top level 
-    for extension in extensions: #lolpop/extension/my_extension
-        resources = ["%s/%s" % (extension, x) for x in os.listdir(extension)
-                     if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
-        for resource in resources: #lolpop/extension/my_extension/{component,pipeline,runner}
-            subdirs = ["%s/%s" % (resource, x) for x in os.listdir(resource)
-                       if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
-        #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
-        for subdir in subdirs:
-            files = [x for x in os.listdir(subdir) if (
-                (".py" in x) and ("__" not in x) and (x[0] != "."))]
-            #from each file, import all classes and register them in the global namespace.
-            for file in files:
-                subdir_arr = subdir.split("/")
-                module = import_module("lolpop.extension.%s.%s.%s.%s" % (
-                    subdir_arr[-3], subdir_arr[-2], subdir_arr[-1], file[:-3]))
-                classes = [x for x in dir(module) if isclass(getattr(module, x))]
-                components = [x for x in classes if (
-                    issubclass(getattr(module, x), BaseComponent)
-                    or issubclass(getattr(module, x), BasePipeline)
-                    or issubclass(getattr(module, x), BaseRunner)
-                    )]
-                globals().update({name: getattr(module, name)
-                                for name in components})
+    #path = Path(__file__).parent.resolve() #lolpop/extension
+    for path in __path__: 
+        extensions = ["%s/%s" % (path, x) for x in os.listdir(path)
+                    if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
+        #iterate through extensions and add each top level 
+        for extension in extensions: #lolpop/extension/my_extension
+            resources = ["%s/%s" % (extension, x) for x in os.listdir(extension)
+                        if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
+            for resource in resources: #lolpop/extension/my_extension/{component,pipeline,runner}
+                subdirs = ["%s/%s" % (resource, x) for x in os.listdir(resource)
+                        if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
+                #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
+                for subdir in subdirs:
+                    files = [x for x in os.listdir(subdir) if (
+                        (".py" in x) and ("__" not in x) and (x[0] != "."))]
+                    #from each file, import all classes and register them in the global namespace.
+                    for file in files:
+                        subdir_arr = subdir.split("/")
+                        module = import_module("lolpop.extension.%s.%s.%s.%s" % (
+                            subdir_arr[-3], subdir_arr[-2], subdir_arr[-1], file[:-3]))
+                        classes = [x for x in dir(module) if isclass(getattr(module, x))]
+                        components = [x for x in classes if (
+                            issubclass(getattr(module, x), BaseComponent)
+                            or issubclass(getattr(module, x), BasePipeline)
+                            or issubclass(getattr(module, x), BaseRunner)
+                            )]
+                        globals().update({name: getattr(module, name)
+                                        for name in components})
 
-        warnings.resetwarnings()
+    warnings.resetwarnings()
 
 
 __map_extensions__()
```

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/__init__.py` & `lolpop-0.1.0a6/lolpop/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/base_pipeline.py` & `lolpop-0.1.0a6/lolpop/pipeline/base_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,14 @@
             self.notifier.notify(msg, level)
             self.log("Notification Sent: %s" %msg, level)
 
     #helper function for lookup up config key in pipeline or runner conf
     def _get_config(self, key, default_value=None): 
         key = key.lower()
         value = utils.lower_conf(self.config).get(key, None)
-        if not value: 
+        if value is None: 
             value = utils.lower_conf(self.runner_conf).get(key, default_value)
         return value 
 
     def _set_config(self, key, value): 
         key = key.lower()
         self.config[key]=value
```

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/deploy/metaflow_offline_deploy.py` & `lolpop-0.1.0a6/lolpop/pipeline/deploy/metaflow_offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/deploy/offline_deploy.py` & `lolpop-0.1.0a6/lolpop/pipeline/deploy/offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/predict/metaflow_offline_predict.py` & `lolpop-0.1.0a6/lolpop/pipeline/predict/metaflow_offline_predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,17 +95,17 @@
 
         data = self.data
         #drop any metadata columns
         df = data.drop(self.lolpop._get_config("DROP_COLUMNS", []),
                        axis=1, errors="ignore")
 
         #make predictions
-        data["predictions"] = self.model._predict_df(df)
+        data["predictions"] = self.model.predict_df(df)
         if self.lolpop.problem_type == "classification":
-            data["predictions_proba"] = self.model._predict_proba_df(
+            data["predictions_proba"] = self.model.predict_proba_df(
                 df, to_list=True)
 
         #get explanations
         data["explanations"] = self.lolpop.model_explainer.get_explanations(
             df, self.model, self.model_version, "predictions", to_list=True)
 
         #log predictions
```

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/predict/offline_predict.py` & `lolpop-0.1.0a6/lolpop/pipeline/predict/offline_predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         prediction_id = "%s_predictions" %self.metadata_tracker.get_resource_id(model_version)
         prediction_job = self.metadata_tracker.create_resource(id=prediction_id, type="prediction_job", parent=model_version, prediction_count=data.shape[0])
 
         #drop any metadata columns
         df = data.drop(self._get_config("DROP_COLUMNS", []), axis=1, errors="ignore")
 
         #make predictions
-        data["predictions"] = model._predict_df(df)
+        data["predictions"] = model.predict_df(df)
         if self.problem_type == "classification": 
-            data["predictions_proba"] = model._predict_proba_df(df, to_list=True)
+            data["predictions_proba"] = model.predict_proba_df(df, to_list=True)
 
         #get explanations
-        if not self._get_config("skip_prediction_explanations"):
+        if self.problem_type !="timeseries" and not self._get_config("skip_prediction_explanations"):
             data["explanations"] = self.model_explainer.get_explanations(df, model, model_version, "predictions", to_list=True)
 
         #log predictions
         self.metrics_tracker.log_prediction_metrics(prediction_job, data["predictions"])
 
         return data, prediction_job
```

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/process/offline_process.py` & `lolpop-0.1.0a6/lolpop/pipeline/process/offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/train/base_train.py` & `lolpop-0.1.0a6/lolpop/pipeline/train/base_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/train/metaflow_offline_train.py` & `lolpop-0.1.0a6/lolpop/pipeline/train/metaflow_offline_train.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,18 +67,14 @@
         self.next(self.train_model)
 
     @step
     def train_model(self):
         #create model_version
         id = self.lolpop._get_config("model_name")
         model_version = self.lolpop.metadata_tracker.create_resource(id, type="model_version")
-        print(model_version)
-        print(model_version[1])
-        print(model_version[1].info.run_id)
-        print(type(model_version[1]))
 
         #if we are using hyperparameter tuner, use that, otherwise just use the model trainer provided
         if hasattr(self.lolpop, "hyperparameter_tuner"):
             model = self.lolpop.hyperparameter_tuner.run_experiment(
                 self.data_dict, model_version)
         else:
             model = self.lolpop.model_trainer.build_model(self.data_dict, model_version)
```

### Comparing `lolpop-0.1.0a5/lolpop/pipeline/train/offline_train.py` & `lolpop-0.1.0a6/lolpop/pipeline/train/offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/runner/__init__.py` & `lolpop-0.1.0a6/lolpop/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/runner/base_runner.py` & `lolpop-0.1.0a6/lolpop/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/runner/classification_runner/classification_runner.py` & `lolpop-0.1.0a6/lolpop/runner/classification_runner/classification_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,19 @@
         "components": ["metadata_tracker", "metrics_tracker", "resource_version_control"],
         "config": ["train_data", "eval_data", "prediction_data", "model_target", "drop_columns"]
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(problem_type="classification", *args, **kwargs)
 
-    def process_data(self, source_data = "train"):
+    def process_data(self, source = "train"):
         #run data transformations and encodings
-        source_data_name = self._get_config("%s_data" % source_data)
-        data = self.process.transform_data(source_data_name)  # maybe better called get_training_data?
+        source_data_name = "%s_data" % source
+        source_data = self._get_config(source_data_name)
+        data = self.process.transform_data(source_data)  # maybe better called get_training_data?
 
         #track & version data
         dataset_version = self.process.track_data(data, source_data_name)
 
         #profile data
         self.process.profile_data(data, dataset_version)
 
@@ -161,11 +162,11 @@
         pass
 
     def build_all(self):
         data, dataset_version = self.process_data()
         model_version, model, is_new_model_better = self.train_model(data, dataset_version)
         if is_new_model_better: 
             deployment = self.deploy_model(model_version)
-        eval_data, eval_dataset_version = self.process_data(source_data="eval")
+        eval_data, eval_dataset_version = self.process_data(source="eval")
         data, prediction_job = self.predict_data(model_version,model, eval_data, eval_dataset_version)
         self.evaluate_ground_truth(prediction_job)
```

### Comparing `lolpop-0.1.0a5/lolpop/runner/classification_runner/metaflow_classification.py` & `lolpop-0.1.0a6/lolpop/runner/classification_runner/metaflow_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
         "components": ["metadata_tracker", "metrics_tracker", "resource_version_control"],
         "config": ["train_data", "eval_data", "prediction_data", "model_target", "drop_columns"]
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(problem_type="classification", *args, **kwargs)
 
-    def process_data(self, source_data = "train"):
+    def process_data(self, source = "train"):
         #run the metaflow process pipeline
-        source_data_name = self._get_config("%s_data" % source_data)
-        self.process.run(source_data_name)
+        source_data_name = "%s_data" % source
+        source_data = self._get_config(source_data_name)
+        self.process.run(source_data_name, source_data)
 
         #retrieve artifacts from metaflow pipeline
         data, dataset_version = self.process.get_artifacts(["data", "dataset_version"])
 
         #return data
         return data, dataset_version
 
@@ -116,11 +117,11 @@
         pass
 
     def build_all(self):
         data, dataset_version = self.process_data()
         model_version, model, is_new_model_better = self.train_model(data, dataset_version)
         if is_new_model_better: 
             deployment = self.deploy_model(model_version)
-        eval_data, eval_dataset_version = self.process_data(source_data="eval")
+        eval_data, eval_dataset_version = self.process_data(source="eval")
         data, prediction_job = self.predict_data(model_version,model, eval_data, eval_dataset_version)
         self.evaluate_ground_truth(prediction_job)
```

### Comparing `lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py` & `lolpop-0.1.0a6/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py` & `lolpop-0.1.0a6/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py` & `lolpop-0.1.0a6/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py` & `lolpop-0.1.0a6/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py` & `lolpop-0.1.0a6/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py` & `lolpop-0.1.0a6/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/utils/common_utils.py` & `lolpop-0.1.0a6/lolpop/utils/common_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,26 +73,49 @@
     if obj: 
         plugin_paths = obj._get_config("plugin_paths",[]) 
         plugin_paths.append(plugin_dir)
         obj._set_config("plugin_paths", plugin_paths)
     return mod
 
 #load class object
-def load_class(class_name, class_type="component", parent="lolpop"): 
+def load_class_obj(class_name, class_type="component", parent="lolpop"): 
     module = import_module("%s.%s" %(parent, class_type))
     cl = getattr(module, class_name)
     return cl
 
+def load_class(class_name, class_type="component", plugin_mods = [], self_obj=None): 
+    try:
+        cl = load_class_obj(class_name, class_type)
+    except: 
+        try: 
+            if self_obj: 
+                self_obj.log("Unable to find class %s in build-in resources. Searching extensions..." %class_name)
+            cl = load_class_obj(class_name, class_type="extension")
+            if self_obj:
+                self_obj.log("Found class %s in extensions!" %class_name)
+        except: 
+            if self_obj:
+                self_obj.log(
+                    "Unable to find class %s in extensions. Searching plugins modules in %s..." %(class_name, str(plugin_mods)))
+            cl = load_class_from_plugin(class_name, plugin_mods, class_type)
+            if cl is not None: 
+                if self_obj: 
+                    self_obj.log("Found class %s in plugins!" % class_name)
+            else: 
+                if self_obj:
+                    self_obj.log("Unable to find class %s in plugins!" %class_name)
+    return cl 
+
 #load class object from plugins
 def load_class_from_plugin(class_name, plugin_mods, class_type="component"):
     #try to load from each plugin
     cl = None 
     for plugin in plugin_mods: 
         try: 
-            cl = load_class(class_name, class_type=class_type, parent=plugin)
+            cl = load_class_obj(class_name, class_type=class_type, parent=plugin)
             break 
         except Exception as e: 
             #if multiple plugins are used, the one we are looking for will not be in most of them, so just ignore any errors
             continue 
     return cl
 
 #loads a module from a file
@@ -106,58 +129,29 @@
 #register component class as an attribute of the provided object
 def register_component_class(self_obj, conf, component_type, default_class_name=None, 
                              pipeline_conf = {}, runner_conf = {}, parent_process = "runner", 
                              problem_type = None, dependent_components = {}, plugin_mods=[], *args, **kwargs): 
     obj = None
     component_class_name = conf.components.get(component_type, default_class_name)
     if component_class_name is not None:
-        try: 
-            cl = load_class(component_class_name) 
-        except: 
-            try: 
-                self_obj.log("Unable to find component in build-in components. Searching extensions...")
-                cl = load_class(component_class_name, class_type="extension")
-                self_obj.log("Found class %s in extensions!" %component_class_name)
-            except: 
-                self_obj.log(
-                    "Unable to find class %s in extensions. Searching plugins modules in %s..." %(component_class_name, str(plugin_mods)))
-                cl = load_class_from_plugin(component_class_name, plugin_mods)
-                if cl is not None: 
-                    self_obj.log("Found class %s in plugins!" % component_class_name)
-                else: 
-                    self_obj.log("Unable to find class %s in plugins!" %component_class_name)
+        cl = load_class(component_class_name) 
         if cl is not None: 
             obj = cl(conf=conf.get(component_type, {}), pipeline_conf=pipeline_conf, runner_conf=runner_conf,
                      parent_process=parent_process, problem_type=problem_type, components=dependent_components, *args, **kwargs)
             setattr(self_obj, component_type, obj)
     return obj 
 
 #registers pipeline as an attribute of the provided object
 def register_pipeline_class(self_obj, conf, pipeline_type, default_class_name=None, runner_conf = {}, 
                             parent_process = "runner", problem_type = None, dependent_components = {}, 
                             plugin_mods=[], *args, **kwargs): 
     obj = None 
     pipeline_class_name = conf.pipelines.get(pipeline_type, default_class_name)
     if pipeline_class_name is not None: 
-        try: 
-            cl = load_class(pipeline_class_name, class_type="pipeline")
-        except: 
-            try: 
-                self_obj.log(
-                    "Unable to find component in build-in components. Searching extensions...")
-                cl = load_class(pipeline_class_name, class_type="extension")
-                self_obj.log("Found class %s in extensions!" %
-                             pipeline_class_name)
-            except: 
-                self_obj.log(
-                    "Unable to find pipeline %s in built-in pipelines. Searching plugins..." % pipeline_class_name)
-                cl = load_class_from_plugin(
-                    pipeline_class_name, plugin_mods, class_type="pipeline")
-                self_obj.log(
-                    "Found class %s in plugins!" % pipeline_class_name)
+        cl = load_class(pipeline_class_name, class_type="pipeline")
         if cl is not None: 
             obj = cl(conf=conf.get(pipeline_type, {}), runner_conf=runner_conf, parent_process=parent_process,
                      problem_type=problem_type, components=dependent_components, plugin_mods=plugin_mods, *args, **kwargs)
             setattr(self_obj, pipeline_type, obj)
     return obj
 
 def lower_conf(conf): 
@@ -354,30 +348,30 @@
         ok = False
         try: 
             data = convert_col_types(data, prev_data)
             ok = True
         except Exception as e: 
             obj.notify("Data Comparison failed. New and old dataframes do not have compatible column types. Error: %s" %str(e), "ERROR")
             raise 
-    return data, prev_data, True
+    return data, prev_data, ok
 
 def convert_col_types(data, prev_data):
     df_a = data.copy()
     df_b = prev_data.copy()
     for col in df_a.columns:
         if col in df_b.columns: #if col is net new, we can skip
             if df_a[col].dtype != df_b[col].dtype:
                 df_a[col] = df_a[col].astype(df_b[col].dtype)
     return df_a
 
-#True = lower is better
+#True = higher is better (descending)
 def get_metric_direction(perf_metric): 
-    reverse = False 
-    if perf_metric in ["mse", "rmse", "mae", "mape", "smape"]: 
-        reverse = True 
+    reverse = True 
+    if perf_metric in ["mse", "rmse", "mae", "mdae", "mape", "smape", "rmsle", "msle"]: 
+        reverse = False 
     return reverse
 
 #labels should be something like data["y_train"].unique()
 def get_multiclass(labels): 
     classification_type = "binary"
     num_classes = len(labels)
     if num_classes > 2:
```

### Comparing `lolpop-0.1.0a5/lolpop/utils/continual_utils.py` & `lolpop-0.1.0a6/lolpop/utils/continual_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/utils/metaflow_utils.py` & `lolpop-0.1.0a6/lolpop/utils/metaflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/lolpop/utils/mlflow_utils.py` & `lolpop-0.1.0a6/lolpop/utils/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a5/pyproject.toml` & `lolpop-0.1.0a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lolpop"
-version = "v0.1.0-alpha.5"
+version = "v0.1.0-alpha.6"
 description = "A software engineering framework for machine learning workflows"
 authors = ["jordanvolz <jordan.volz@gmail.com>"]
 repository = "https://github.com/jordanvolz/lolpop"
 #hompage = 
 #documentation = 
 keywords = ["machine learning", "data science", "mlops"]
 license = "Apache-2.0"
@@ -58,22 +58,25 @@
 duckdb={version="^0.7.1", optional=true}
 databricks-sql-connector={version="^2.5.2", optional=true}
 boto3={version="^1.26.89", optional=true}
 db-dtypes={version="^1.1.1", optional=true}
 psychopg2={version="^2.9.6", optional=true}
 openai="^0.27.6"
 cookiecutter={version="^2.1.1", optional=true}
+tslumen={version="^0.0.1", optional=true}
+prophet={version="^1.1.3", optional=true}
 
 [tool.poetry.extras]
 duckdb = ["duckdb"]
 databricks = ["databricks-sql-connector"]
 cli = ["sdv", "openai", "cookiecutter"]
 aws = ["boto3"]
 google = ["google-cloud-bigquery", "google-cloud-storage", "db-dtypes"]
 redshift = ["psychopg2"]
+timeseries = ["tslumen", "prophet"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 faker = "^14.0"
 
 [tool.poetry.scripts]
 lolpop = "lolpop.cli.cli:app"
```

### Comparing `lolpop-0.1.0a5/PKG-INFO` & `lolpop-0.1.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolpop
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: A software engineering framework for machine learning workflows
 Home-page: https://github.com/jordanvolz/lolpop
 License: Apache-2.0
 Keywords: machine learning,data science,mlops
 Author: jordanvolz
 Author-email: jordan.volz@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: aws
 Provides-Extra: cli
 Provides-Extra: databricks
 Provides-Extra: duckdb
 Provides-Extra: google
 Provides-Extra: redshift
+Provides-Extra: timeseries
 Requires-Dist: SQLAlchemy (>=1.4.37,<2.0.0)
 Requires-Dist: aif360 (>=0.5.0,<0.6.0)
 Requires-Dist: alibi[shap] (>=0.8.0,<0.9.0)
 Requires-Dist: boto3 (>=1.26.89,<2.0.0) ; extra == "aws"
 Requires-Dist: continual (>=2.0.0a51,<3.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "cli"
 Requires-Dist: databricks-sql-connector (>=2.5.2,<3.0.0) ; extra == "databricks"
@@ -45,18 +46,20 @@
 Requires-Dist: mlflow (>=2.2.2,<3.0.0)
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
 Requires-Dist: omegaconf (==2.2.3)
 Requires-Dist: openai (>=0.27.6,<0.28.0) ; extra == "cli"
 Requires-Dist: optuna (>=3.0.4,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: prefect (>=2.6.6,<3.0.0)
+Requires-Dist: prophet (>=1.1.3,<2.0.0) ; extra == "timeseries"
 Requires-Dist: psychopg2 (>=2.9.6,<3.0.0) ; extra == "redshift"
 Requires-Dist: pyarrow (>=6.0.1,<7.0.0)
 Requires-Dist: scikit_learn (==1.2.2)
 Requires-Dist: sdv (>=1.0.1,<2.0.0) ; extra == "cli"
 Requires-Dist: snowflake-sqlalchemy (>=1.4.6,<2.0.0)
 Requires-Dist: sweetviz (>=2.1.4,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: tslumen (>=0.0.1,<0.0.2) ; extra == "timeseries"
 Requires-Dist: xgboost (>=1.6.1,<2.0.0)
 Requires-Dist: ydata-profiling (>=4.0.0,<5.0.0)
 Requires-Dist: yellowbrick (>=1.4,<2.0)
 Project-URL: Repository, https://github.com/jordanvolz/lolpop
```

