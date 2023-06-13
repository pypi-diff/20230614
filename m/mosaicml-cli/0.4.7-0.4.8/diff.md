# Comparing `tmp/mosaicml-cli-0.4.7.tar.gz` & `tmp/mosaicml-cli-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.7.tar", last modified: Thu Jun  8 20:36:22 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.8.tar", last modified: Tue Jun 13 23:02:45 2023, max compression
```

## Comparing `mosaicml-cli-0.4.7.tar` & `mosaicml-cli-0.4.8.tar`

### file list

```diff
@@ -1,200 +1,202 @@
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.787793 mosaicml-cli-0.4.7/
--rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-08 20:36:22.787561 mosaicml-cli-0.4.7/PKG-INFO
--rw-r--r--   0 margaretqian   (501) staff       (20)     7089 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/README.md
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.760093 mosaicml-cli-0.4.7/mcli/
--rw-r--r--   0 margaretqian   (501) staff       (20)     2092 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.760685 mosaicml-cli-0.4.7/mcli/api/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.760963 mosaicml-cli-0.4.7/mcli/api/cluster/
--rw-r--r--   0 margaretqian   (501) staff       (20)      134 2022-10-27 18:49:21.000000 mosaicml-cli-0.4.7/mcli/api/cluster/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4237 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.761223 mosaicml-cli-0.4.7/mcli/api/engine/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/engine/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    26003 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/api/engine/engine.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10685 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/exceptions.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.762380 mosaicml-cli-0.4.7/mcli/api/inference_deployments/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1521 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3297 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5105 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3603 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     8450 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2053 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2356 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6483 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.762753 mosaicml-cli-0.4.7/mcli/api/mint/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.7/mcli/api/mint/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     7849 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/api/mint/shell.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2676 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/mint/tty.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.763281 mosaicml-cli-0.4.7/mcli/api/model/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1114 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6322 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/cluster_details.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4583 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/inference_deployment.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10439 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/run.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.764573 mosaicml-cli-0.4.7/mcli/api/runs/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1199 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/api/runs/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2804 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_create_run.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4211 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     8906 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10933 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5213 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_start_run.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5405 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3937 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10619 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.764836 mosaicml-cli-0.4.7/mcli/api/schema/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/schema/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      636 2022-08-23 17:34:43.000000 mosaicml-cli-0.4.7/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.765387 mosaicml-cli-0.4.7/mcli/api/secrets/
--rw-r--r--   0 margaretqian   (501) staff       (20)      309 2022-09-22 23:36:49.000000 mosaicml-cli-0.4.7/mcli/api/secrets/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2386 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3019 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2354 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/typing_future.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.765659 mosaicml-cli-0.4.7/mcli/api/users/
--rw-r--r--   0 margaretqian   (501) staff       (20)      139 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.7/mcli/api/users/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2715 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/users/api_get_users.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1091 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/api/utils.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.765895 mosaicml-cli-0.4.7/mcli/cli/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/__init__.py
--rwxr-xr-x   0 margaretqian   (501) staff       (20)     6387 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/cli.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.766290 mosaicml-cli-0.4.7/mcli/cli/common/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.7/mcli/cli/common/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2560 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6922 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.766531 mosaicml-cli-0.4.7/mcli/cli/m_connect/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.7/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1935 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.766910 mosaicml-cli-0.4.7/mcli/cli/m_create/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_create/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2385 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_create/m_create.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    16900 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.767327 mosaicml-cli-0.4.7/mcli/cli/m_delete/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6448 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_delete/delete.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5805 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.767585 mosaicml-cli-0.4.7/mcli/cli/m_deploy/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.768141 mosaicml-cli-0.4.7/mcli/cli/m_describe/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3929 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     9988 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2002 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.769225 mosaicml-cli-0.4.7/mcli/cli/m_get/
--rw-r--r--   0 margaretqian   (501) staff       (20)      467 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6226 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/clusters.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6447 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/display.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5669 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4803 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/m_get.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     9800 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2189 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/secrets.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1580 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/users.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.769476 mosaicml-cli-0.4.7/mcli/cli/m_init/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_init/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4115 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.770112 mosaicml-cli-0.4.7/mcli/cli/m_interactive/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10916 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    44284 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     9493 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.770777 mosaicml-cli-0.4.7/mcli/cli/m_kube/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5523 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1398 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2050 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6946 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.771027 mosaicml-cli-0.4.7/mcli/cli/m_log/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_log/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    11398 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.775512 mosaicml-cli-0.4.7/mcli/cli/m_ping/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.775854 mosaicml-cli-0.4.7/mcli/cli/m_predict/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1661 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.776142 mosaicml-cli-0.4.7/mcli/cli/m_root/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_root/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      536 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.776582 mosaicml-cli-0.4.7/mcli/cli/m_run/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_run/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     8267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.777468 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-10-11 22:54:49.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2973 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1802 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1940 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1421 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      881 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.777751 mosaicml-cli-0.4.7/mcli/cli/m_stop/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.7/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4066 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.778152 mosaicml-cli-0.4.7/mcli/cli/m_util/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-07-14 21:04:39.000000 mosaicml-cli-0.4.7/mcli/cli/m_util/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      797 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_util/m_util.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6837 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_util/util.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    12876 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/config.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.779133 mosaicml-cli-0.4.7/mcli/models/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1047 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/gpu_type.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10374 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/models/inference_deployment_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      427 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/mcli_cluster.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      456 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/mcli_envvar.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6724 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/mcli_secret.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    19547 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/run_config.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.779293 mosaicml-cli-0.4.7/mcli/objects/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/objects/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.780555 mosaicml-cli-0.4.7/mcli/objects/secrets/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1090 2022-12-07 22:00:09.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.782249 mosaicml-cli-0.4.7/mcli/objects/secrets/create/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1646 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/base.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2244 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2408 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6377 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3858 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5342 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      783 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1017 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/env_var.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      556 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/gcp.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/mounted.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      967 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/oci.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      961 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/s3.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.782580 mosaicml-cli-0.4.7/mcli/proto/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/proto/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1477 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.783027 mosaicml-cli-0.4.7/mcli/sdk/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1976 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/sdk/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.785760 mosaicml-cli-0.4.7/mcli/utils/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/utils/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5306 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/utils/utils_cli.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6073 2023-04-13 22:08:13.000000 mosaicml-cli-0.4.7/mcli/utils/utils_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      740 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.7/mcli/utils/utils_date.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10749 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_docker.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2225 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_epilog.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10774 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_interactive.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4527 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_logging.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2160 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6614 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/utils/utils_pypi.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3115 2022-08-31 05:37:31.000000 mosaicml-cli-0.4.7/mcli/utils/utils_rich.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5033 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/utils/utils_run_status.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4350 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/utils/utils_spinner.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10751 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_string_functions.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1677 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_types.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1001 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/utils/utils_yaml.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3885 2023-06-08 20:35:56.000000 mosaicml-cli-0.4.7/mcli/version.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.786816 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/
--rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 margaretqian   (501) staff       (20)     4886 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)        1 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)       75 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)     1655 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)        5 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)    31087 2023-05-16 20:27:59.000000 mosaicml-cli-0.4.7/pyproject.toml
--rw-r--r--   0 margaretqian   (501) staff       (20)       38 2023-06-08 20:36:22.787870 mosaicml-cli-0.4.7/setup.cfg
--rw-r--r--   0 margaretqian   (501) staff       (20)     3057 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/setup.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.787302 mosaicml-cli-0.4.7/tests/
--rw-r--r--   0 margaretqian   (501) staff       (20)     5991 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/tests/test_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)       62 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/tests/test_simple.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6116 2023-04-11 21:00:01.000000 mosaicml-cli-0.4.7/tests/test_upgrade.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.943381 mosaicml-cli-0.4.8/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-13 23:02:45.943082 mosaicml-cli-0.4.8/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7089 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.8/README.md
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.898764 mosaicml-cli-0.4.8/mcli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2092 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.899802 mosaicml-cli-0.4.8/mcli/api/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/api/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.900548 mosaicml-cli-0.4.8/mcli/api/cluster/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.8/mcli/api/cluster/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4228 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.900943 mosaicml-cli-0.4.8/mcli/api/engine/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/api/engine/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    26219 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/engine/engine.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10784 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/exceptions.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.903414 mosaicml-cli-0.4.8/mcli/api/inference_deployments/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1521 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3297 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5096 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3603 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8441 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2053 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2347 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6474 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.903921 mosaicml-cli-0.4.8/mcli/api/mint/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.8/mcli/api/mint/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7840 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/mint/shell.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2676 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/api/mint/tty.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.905161 mosaicml-cli-0.4.8/mcli/api/model/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/model/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6322 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/model/cluster_details.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4583 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10439 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/model/run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.907663 mosaicml-cli-0.4.8/mcli/api/runs/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/api/runs/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2804 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4202 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8888 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10924 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5204 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5396 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3928 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.909013 mosaicml-cli-0.4.8/mcli/api/schema/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/api/schema/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.8/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.909947 mosaicml-cli-0.4.8/mcli/api/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.8/mcli/api/secrets/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2386 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3010 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3709 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.8/mcli/api/typing_future.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.910287 mosaicml-cli-0.4.8/mcli/api/users/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.8/mcli/api/users/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2715 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/users/api_get_users.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      920 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/utils.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.910685 mosaicml-cli-0.4.8/mcli/cli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.8/mcli/cli/__init__.py
+-rwxr-xr-x   0 tylerlee   (502) staff       (20)     6378 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/cli.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.911353 mosaicml-cli-0.4.8/mcli/cli/common/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.8/mcli/cli/common/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2560 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6922 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.911677 mosaicml-cli-0.4.8/mcli/cli/m_connect/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.8/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.912173 mosaicml-cli-0.4.8/mcli/cli/m_create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    16900 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.912824 mosaicml-cli-0.4.8/mcli/cli/m_delete/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6448 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5805 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.913138 mosaicml-cli-0.4.8/mcli/cli/m_deploy/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4001 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.914056 mosaicml-cli-0.4.8/mcli/cli/m_describe/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3929 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9988 2023-06-13 22:57:06.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2002 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.915910 mosaicml-cli-0.4.8/mcli/cli/m_get/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6226 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6447 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/display.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5669 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4803 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9800 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/users.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.916311 mosaicml-cli-0.4.8/mcli/cli/m_init/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3908 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.917343 mosaicml-cli-0.4.8/mcli/cli/m_interactive/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9484 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.918609 mosaicml-cli-0.4.8/mcli/cli/m_kube/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5523 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1398 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2050 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6946 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.918965 mosaicml-cli-0.4.8/mcli/cli/m_log/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    11253 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.919389 mosaicml-cli-0.4.8/mcli/cli/m_ping/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.919870 mosaicml-cli-0.4.8/mcli/cli/m_predict/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1661 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.920308 mosaicml-cli-0.4.8/mcli/cli/m_root/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.920696 mosaicml-cli-0.4.8/mcli/cli/m_run/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8258 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.922013 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2964 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      745 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.922285 mosaicml-cli-0.4.8/mcli/cli/m_stop/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.8/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4066 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.923083 mosaicml-cli-0.4.8/mcli/cli/m_util/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.8/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-06-13 22:57:06.000000 mosaicml-cli-0.4.8/mcli/cli/m_util/util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    12143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.925382 mosaicml-cli-0.4.8/mcli/models/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/gpu_type.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10374 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.8/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/mcli_cluster.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      456 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/mcli_envvar.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6724 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/mcli_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    19538 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/models/run_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.925915 mosaicml-cli-0.4.8/mcli/objects/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/objects/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.927874 mosaicml-cli-0.4.8/mcli/objects/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.929494 mosaicml-cli-0.4.8/mcli/objects/secrets/create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.929805 mosaicml-cli-0.4.8/mcli/proto/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/proto/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.930082 mosaicml-cli-0.4.8/mcli/sdk/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1976 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/sdk/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.934542 mosaicml-cli-0.4.8/mcli/utils/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.8/mcli/utils/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5306 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/utils/utils_cli.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/utils/utils_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.8/mcli/utils/utils_date.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10749 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_docker.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_epilog.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4527 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_logging.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6605 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/utils/utils_pypi.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.8/mcli/utils/utils_rich.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5033 2023-06-06 15:18:59.000000 mosaicml-cli-0.4.8/mcli/utils/utils_run_status.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.8/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/utils/utils_spinner.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_types.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/utils/utils_yaml.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3876 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/version.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.938033 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4922 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1655 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/pyproject.toml
+-rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-06-13 23:02:45.943565 mosaicml-cli-0.4.8/setup.cfg
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3057 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.8/setup.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.941898 mosaicml-cli-0.4.8/tests/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.8/tests/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/tests/conftest.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7127 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/tests/test_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.8/tests/test_simple.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.7/PKG-INFO` & `mosaicml-cli-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.7
+Version: 0.4.8
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.7/README.md` & `mosaicml-cli-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/__init__.py` & `mosaicml-cli-0.4.8/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.8/mcli/api/cluster/api_get_clusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters
         },
     }
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {'userIds': [cfg.user_id]}
 
     response = run_plural_mapi_request(
         query=QUERY_UTILIZATION if include_utilization else QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=ClusterDetails,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.8/mcli/api/engine/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,26 +18,36 @@
 from gql.client import Client, ReconnectingAsyncClientSession
 from gql.transport import AsyncTransport
 from gql.transport.exceptions import TransportQueryError
 from gql.transport.websockets import WebsocketsTransport
 from graphql import DocumentNode
 from websockets.exceptions import ConnectionClosed, PayloadTooBig, WebSocketException
 
-from mcli.api.exceptions import MAPIException, MCLIConfigError, MultiMAPIException
+from mcli.api.exceptions import ERROR_API_KEY_MISSING, MAPIException, MCLIConfigError, MultiMAPIException
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.api.utils import check_python_certificates
-from mcli.config import MESSAGE, get_timeout
+from mcli.config import get_timeout
+from mcli.version import __version__
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable-next=invalid-name
 THREADPOOL_WORKERS = 10
 THREADPOOL: Optional[ThreadPoolExecutor] = None
 
 
+def get_common_header(header: Dict[str, str]) -> Dict[str, str]:
+    return {
+        **header,
+        'Content-Type': 'application/json',
+        'x-mosaicml-client': 'mcli',
+        'x-mosaicml-client-version': __version__,
+    }
+
+
 def _create_threadpool() -> ThreadPoolExecutor:
     """Create a global threadpool for requests
     """
     logger.debug("Creating default threadpool")
     global THREADPOOL
     THREADPOOL = ThreadPoolExecutor(max_workers=THREADPOOL_WORKERS, thread_name_prefix='mosaicml-api')
     return THREADPOOL
@@ -90,15 +100,15 @@
         self._session: Optional[ReconnectingAsyncClientSession] = None
         self._loop = asyncio.new_event_loop()
         self._terminate = Event()
 
     def _load_from_environment(self, api_key: Optional[str] = None, endpoint: Optional[str] = None) -> None:
         # pylint: disable-next=import-outside-toplevel
         from mcli import config
-        conf = config.MCLIConfig.load_config(safe=True)
+        conf = config.MCLIConfig.load_config()
         if api_key is None:
             api_key = conf.api_key
 
         if not api_key:
             api_key = ''
 
         self.api_key = api_key
@@ -153,15 +163,15 @@
 
     @property
     def client(self) -> Client:
         return self.create_websocket_connection()
 
     async def _create_gql_client(self) -> Client:
         ws_endpoint = self.endpoint.replace("http://", "ws://").replace("https://", "wss://")
-        headers = {'Authorization': self.api_key, 'Content-Type': 'application/json'}
+        headers = get_common_header({'Authorization': self.api_key})
         logger.debug(f"Connecting to websocket server at endpoint {ws_endpoint}")
         transport = WebsocketsTransport(url=ws_endpoint, init_payload=headers)
         return Client(transport=transport, fetch_schema_from_transport=False)
 
     def subscribe(
         self,
         query: DocumentNode,
@@ -468,15 +478,15 @@
     variables: Optional[Dict[str, Any]],
     query_function: str,
     model_type: Optional[Type[ModelT]],
 ) -> List[ModelT]:
     """Run a graphql request in a thread and return a list of items
     """
     if not api_key:
-        raise MCLIConfigError(MESSAGE.API_KEY_MISSING)
+        raise MCLIConfigError(ERROR_API_KEY_MISSING)
     try:
         response = _run_graphql_request(api_key, endpoint, query, variables)
     except requests.exceptions.ConnectionError as e:
         mapi_error = MAPIException.from_requests_error(e)
         raise mapi_error from e
 
     return _deserialize_response(response, query_function, model_type, paginated=True)
@@ -489,15 +499,15 @@
     variables: Optional[Dict[str, Any]],
     query_function: str,
     model_type: Optional[Type[ModelT]],
 ) -> List[ModelT]:
     """Run a graphql request in a thread and return a list of items
     """
     if not api_key:
-        raise MCLIConfigError(MESSAGE.API_KEY_MISSING)
+        raise MCLIConfigError(ERROR_API_KEY_MISSING)
     try:
         response = _run_graphql_request(api_key, endpoint, query, variables)
     except requests.exceptions.ConnectionError as e:
         mapi_error = MAPIException.from_requests_error(e)
         raise mapi_error from e
 
     return _deserialize_response(response, query_function, model_type)
@@ -602,18 +612,15 @@
     variables: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, Any]:
 
     if variables is None:
         variables = {}
     variables = {key.replace('$', ''): value for key, value in variables.items()}
 
-    headers = {
-        'Content-Type': 'application/json',
-        'authorization': api_key,
-    }
+    headers = get_common_header({'authorization': api_key})
     payload = json.dumps({'query': query, 'variables': variables})
 
     # Don't want timeout since this will be run in a background thread
     # pylint: disable-next=missing-timeout
     response = requests.request(
         'POST',
         endpoint,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/exceptions.py` & `mosaicml-cli-0.4.8/mcli/api/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from websockets.exceptions import ConnectionClosedError, InvalidStatusCode
 
 from mcli.utils.utils_logging import FAIL
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_MESSAGE = 'Unknown Error'
+ERROR_API_KEY_MISSING = 'No API key found. Please create one and set it using `mcli set api-key`.'
 
 
 class MCLIException(Exception):
     """Base custom exception that MCLI will raise
 
     All errors should inherit this base so that expected errors can be properly caught
     """
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
     filters = {}
     if deployment_names:
         filters['name'] = {'in': deployment_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     response = run_plural_mapi_request(
         query=QUERY,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters,
             'includeDeleted': False,
         },
     }
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {'userIds': [cfg.user_id]}
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=InferenceDeployment,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     validate_url = cast(Callable[[str], bool], validators.url)
     if isinstance(deployment, str) and not validate_url(deployment):
         # if a string is passed in that is not a url then lookup the deployment and get the name
         deployment_objs = get_inference_deployments(deployments=[deployment])
         if len(deployment_objs) == 0:
             raise MAPIException(HTTPStatus.NOT_FOUND, f'No inference deployment found with name {deployment}.')
         deployment = deployment_objs[0]
-    conf = config.MCLIConfig.load_config(safe=True)
+    conf = config.MCLIConfig.load_config()
     api_key = conf.api_key
     headers = {
         'authorization': api_key,
     }
     base_url = deployment
     if isinstance(deployment, InferenceDeployment):
         base_url = f'https://{deployment.public_dns}'
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                     'in': [d.name if isinstance(d, InferenceDeployment) else d for d in deployments]
                 },
             }
         },
         VARIABLE_DATA_UPDATE_DEPLOYMENTS: updates,
     }
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_GET_DEPLOYMENTS]['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     response = run_plural_mapi_request(
         query=QUERY,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.8/mcli/api/mint/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
         # Start the async event loop
         self._loop = asyncio.get_event_loop_policy().get_event_loop()
 
     def _load_from_environment(self, api_key: Optional[str] = None, endpoint: Optional[str] = None) -> None:
         # pylint: disable-next=import-outside-toplevel
         from mcli import config
-        conf = config.MCLIConfig.load_config(safe=True)
+        conf = config.MCLIConfig.load_config()
         if api_key is None:
             api_key = conf.api_key
 
         if not api_key:
             api_key = ''
 
         self.api_key = api_key
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.8/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.8/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.8/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.8/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/model/run.py` & `mosaicml-cli-0.4.8/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.8/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_delete_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
     filters = {}
     if run_names:
         filters['name'] = {'in': run_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     response = run_plural_mapi_request(
         query=QUERY,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_get_run_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     filters: Dict[str, Any] = {'name': run_name, 'follow': False, 'failed': failed}
     if rank is not None:
         filters['nodeRank'] = rank
 
     if attempt is not None:
         filters['attemptIndex'] = attempt
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     variables = {VARIABLE_DATA_NAME: filters}
     for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
@@ -180,15 +180,15 @@
     filters: Dict[str, Any] = {'name': run_name, 'follow': True}
     if rank is not None:
         filters['nodeRank'] = rank
 
     if attempt is not None:
         filters['attemptIndex'] = attempt
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     variables = {VARIABLE_DATA_NAME: filters}
     for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_get_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     variables = {
         variable_name: {
             'filters': filters,
             'includeDeleted': False,
         },
     }
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[variable_name]['entity'] = {'userIds': [cfg.user_id]}
     if user_emails:
         if variables[variable_name].get('entity'):
             variables[variable_name]['entity']['emails'] = user_emails
         else:
             variables[variable_name]['entity'] = {'emails': user_emails}
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_start_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     filters = {}
     if run_names:
         filters['name'] = {'in': run_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     response = run_plural_mapi_request(
         query=QUERY,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_stop_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     filters = {}
     if run_names:
         filters['name'] = {'in': run_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     response = run_plural_mapi_request(
         query=QUERY,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_update_run_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             }
         },
         VARIABLE_DATA_UPDATE_RUN_METADATA: {
             'metadata': metadata
         },
     }
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_GET_RUNS]['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     response = run_singular_mapi_request(
         query=QUERY,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.8/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.8/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.8/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.8/mcli/api/secrets/api_delete_secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters,
         },
     }
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     response = run_plural_mapi_request(
         query=QUERY,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.8/mcli/api/secrets/api_get_secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters,
         },
     }
 
-    cfg = MCLIConfig.load_config(safe=True)
+    cfg = MCLIConfig.load_config()
     if cfg.user_id:
         variables[VARIABLE_DATA_NAME]['entity'] = {'userIds': [cfg.user_id]}
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Secret,
```

### Comparing `mosaicml-cli-0.4.7/mcli/api/typing_future.py` & `mosaicml-cli-0.4.8/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.8/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/api/utils.py` & `mosaicml-cli-0.4.8/mcli/api/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Utils for all api folders
 """
 
 import logging
 import os
 import ssl
+import sys
 
 from mcli.utils.utils_logging import WARN, FormatString, format_string
 
 logger = logging.getLogger(__name__)
 
-LINK = 'https://stackoverflow.com/questions/52805115/certificate-verify-failed-unable-to-get-local-issuer-certificate'
-
 
 def check_python_certificates():
+    # Only support macOS checks for now
+    if sys.platform != 'darwin':
+        return
+
     certificates_exist = os.path.exists(ssl.get_default_verify_paths().openssl_cafile)
     if not certificates_exist:
         command = 'bash /Applications/Python*/Install\\ Certificates.command'
         command = format_string(command, FormatString.BLUE)
         message = ('Python SSL Certificates are not installed. '
                    'These are required to make HTTPs requests against MosaicML services.')
         message = format_string(message, FormatString.RED)
-        link = format_string(LINK, FormatString.BLUE)
-        logger.error(f'{message}\n\n{WARN}If you are on macOS, please run the '
-                     f'following command to install them: \n{command}\n\n'
-                     f'For other operating systems, please see: \n{link}')
+        logger.error(f'{message}\n\n{WARN}Please run the '
+                     f'following command to install them: \n{command}\n')
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/cli.py` & `mosaicml-cli-0.4.8/mcli/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     add_root_commands(subparser=subparser)
     return parser, subparser
 
 
 def get_parser(is_admin: bool = False) -> argparse.ArgumentParser:
     parser, subparser = get_mcli_root('mcli' if not is_admin else 'mcli-admin')
 
-    conf = MCLIConfig.load_config(safe=True)
+    conf = MCLIConfig.load_config()
 
     if conf.feature_enabled(FeatureFlag.MCLOUD_INTERACTIVE):
         add_connect_argparser(subparser=subparser)
         add_interactive_argparser(subparser=subparser)
     elif conf.allow_interactive:
         kube_interactive_argparser(subparser=subparser)
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.8/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.8/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_set.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,51 @@
-""" mcli connect Entrypoint """
+""" mcli set Entrypoint """
 import argparse
 
-from mcli.cli.m_interactive.interactive import connect_entrypoint
-
-
-def configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.add_argument(
-        'name',
-        metavar='RUN',
-        default=None,
-        nargs='?',
-        help='Run name',
+from mcli.cli.m_set_unset.api_key import configure_api_key_argparser, modify_api_key
+from mcli.cli.m_set_unset.feature_flag import use_feature_flag
+from mcli.cli.m_set_unset.user import configure_user_argparser, modify_user
+
+
+def set_entrypoint(**kwargs):
+    del kwargs
+    mock_parser = configure_argparser(parser=argparse.ArgumentParser())
+    mock_parser.print_help()
+    return 0
+
+
+def configure_argparser(parser: argparse.ArgumentParser, is_admin: bool = False) -> argparse.ArgumentParser:
+    subparsers = parser.add_subparsers()
+    parser.set_defaults(func=set_entrypoint)
+
+    feature_parser = subparsers.add_parser('feature', help='Activate a feature flag')
+    feature_parser.add_argument('feature', nargs='?', help='The name of the feature flag')
+    feature_parser.set_defaults(func=use_feature_flag, activate=True)
+
+    api_key_parser = subparsers.add_parser(
+        'api-key',
+        help='Set a MosaicML platform API key that will be used in all of your subsequent workloads',
+        description='Set a MosaicML platform API key that will be used in all of your subsequent workloads',
     )
+    configure_api_key_argparser(api_key_parser)
+    api_key_parser.set_defaults(func=modify_api_key)
 
-    parser.add_argument('--rank',
-                        metavar='N',
-                        default=0,
-                        type=int,
-                        help='Connect to the specified node rank within the run')
-
-    parser.add_argument(
-        '-l',
-        '--latest',
-        action='store_true',
-        dest='latest',
-        default=False,
-        help='Connect to the latest run',
-    )
-    command_grp = parser.add_mutually_exclusive_group()
-    command_grp.add_argument(
-        '--command',
-        help='The command to execute in the run. By default you will be dropped into a bash shell',
-    )
-    command_grp.add_argument(
-        '--tmux',
-        action='store_true',
-        help='Use tmux as the entrypoint for your run so your session is robust to disconnects',
-    )
+    if is_admin:
+        user_parser = subparsers.add_parser('user', help='Set the user id to use')
+        configure_user_argparser(user_parser)
+        user_parser.set_defaults(func=modify_user)
 
-    parser.set_defaults(func=connect_entrypoint)
     return parser
 
 
-def add_connect_argparser(subparser: argparse._SubParsersAction,) -> argparse.ArgumentParser:
-    """Adds the get parser to a subparser
+def add_set_argparser(subparser: argparse._SubParsersAction, is_admin: bool = False) -> argparse.ArgumentParser:
+    """Adds the set parser to a subparser
 
     Args:
-        subparser: the Subparser to add the Get parser to
+        subparser: the Subparser to add the Use parser to
     """
-    examples = """
-
-Examples:
-
-# Connect to an existing run
-> mcli connect my-run-1234
-
-# Connect to the rank 1 node from my-run-1234
-> mcli connect my-run-1234 --rank 1
-    """
-
-    connect_parser: argparse.ArgumentParser = subparser.add_parser(
-        'connect',
-        help='Create an interactive session that\'s connected to a run',
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-        epilog=examples,
+    set_parser: argparse.ArgumentParser = subparser.add_parser(
+        'set',
+        help='Set local configuration variables',
     )
-
-    get_parser = configure_argparser(parser=connect_parser)
-    return get_parser
+    set_parser = configure_argparser(parser=set_parser, is_admin=is_admin)
+    return set_parser
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.8/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.8/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.8/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.8/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.8/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.8/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.8/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.8/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.8/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.8/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.8/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.8/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.8/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.8/mcli/cli/m_init/m_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ m init Entrypoint"""
 import logging
 import textwrap
 import webbrowser
 from typing import Optional
 
 from mcli import config
-from mcli.api.exceptions import MCLIConfigError
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import MCLIConfig
 from mcli.utils.utils_interactive import secret_prompt
 from mcli.utils.utils_logging import OK
 from mcli.utils.utils_string_functions import validate_api_plaintext
 
 logger = logging.getLogger(__name__)
@@ -24,20 +23,15 @@
     Returns:
         True if MCLI needed to be initialized. False if initialization was already done.
     """
 
     if not config.MCLI_CONFIG_DIR.exists():
         config.MCLI_CONFIG_DIR.mkdir(parents=True, exist_ok=True)
 
-    # Generate MCLI Config if not existing
-    try:
-        mcli_config = MCLIConfig.load_config()
-    except MCLIConfigError:
-        mcli_config = MCLIConfig.empty()
-        mcli_config.save_config()
+    mcli_config = MCLIConfig.load_config()
 
     return mcli_config
 
 
 def no_input_init(has_api_key: bool) -> int:
     logger.info(f'{OK} MCLI successfully initialized')
     logger.info('')
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.8/mcli/cli/m_log/m_log.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,340 +1,275 @@
-"""
-mcloud interactive
-"""
+"""mcli logs entrypoint"""
+from __future__ import annotations
 
 import argparse
 import logging
-from typing import Optional
-
-from mcli.api.cluster import get_clusters
-from mcli.api.exceptions import MintException
-from mcli.api.mint import shell
-from mcli.api.model.run import Run, RunConfig, RunStatus
-from mcli.api.runs.api_create_run import create_run
-from mcli.api.runs.api_get_runs import get_runs
+import os
+import sys
+from functools import partial
+from http import HTTPStatus
+from typing import List, Optional, Tuple, Union
+
+from mcli.api.exceptions import MAPIException
+from mcli.api.inference_deployments.api_get_inference_deployment_logs import get_inference_deployment_logs
+from mcli.api.model.inference_deployment import InferenceDeployment
+from mcli.api.model.run import Run
+from mcli.api.runs.api_get_run_logs import follow_run_logs, get_run_logs
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
-from mcli.cli.m_get.display import format_timestamp
+from mcli.cli.common.deployment_filters import get_deployments_with_filters
+from mcli.cli.common.run_filters import get_runs_with_filters
+from mcli.utils.utils_cli import SubmissionType
 from mcli.utils.utils_epilog import CommonLog
-from mcli.utils.utils_interactive import choose_one
-from mcli.utils.utils_logging import FAIL
-from mcli.utils.utils_types import get_hours_type
+from mcli.utils.utils_logging import FAIL, INFO, err_console
+from mcli.utils.utils_run_status import RunStatus
 
 logger = logging.getLogger(__name__)
 
+# pylint: disable-next=invalid-name
+RUN_LOG_EXAMPLES = """
 
-def wait_for_run(run: Run) -> bool:
-    last_status: Optional[RunStatus] = None
-    with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
-        run = watcher.follow()
-        last_status = run.status
-
-    common_log = CommonLog(logger)
-    if last_status is None:
-        common_log.log_timeout()
-        return False
-    elif last_status == RunStatus.RUNNING:
-        common_log.log_run_interactive_starting(run.name)
-        return True
-    elif last_status == RunStatus.FAILED:
-        if run.reason == "FailedImagePull":
-            common_log.log_pod_failed_pull(run.name, run.config.image)
-        else:
-            common_log.log_pod_failed(run.name)
-        return False
-    elif last_status.after(RunStatus.RUNNING):
-        common_log.log_connect_run_terminating(last_status.display_name)
-        return False
-
-    common_log.log_unknown_did_not_start()
-    logger.debug(last_status)
-    return False
-
-
-def interactive(
-    name: Optional[str] = None,
-    cluster: Optional[str] = None,
-    gpu_type: Optional[str] = None,
-    gpus: Optional[int] = None,
-    hours: Optional[float] = None,
-    image: str = 'mosaicml/pytorch',
-    rank: int = 0,
-    connect: bool = True,
-    command: Optional[str] = None,
-    **kwargs,
-) -> int:
-    del kwargs
+Examples:
 
-    if not cluster:
-        clusters = get_clusters()
-        if not clusters:
-            raise RuntimeError('No clusters available. Contact your administrators to set one up')
-        elif len(clusters) == 1:
-            cluster = clusters[0].name
-        else:
-            values = ", ".join([c.name for c in clusters])
-            raise RuntimeError('Multiple clusters available. Please use the --cluster argument to set the '
-                               f'cluster to use for interactive. Available clusters: {values}')
-
-    run_config = RunConfig(
-        name=name or f'interactive-{(gpu_type or "none").replace("_", "-")}-{gpus or 0}'.lower(),
-        image=image,
-        command=f'sleep {int(3600 * (hours or 1))}',
-        gpu_num=gpus,
-        gpu_type=gpu_type,
-        cluster=cluster,
-        optimization_level=0,
-    )
+# View the current logs of an ongoing run
+> mcli logs run-1234
 
-    run = create_run(run_config)
-    ready = wait_for_run(run)
-    if not ready:
-        return 1
+# By default, if you don't specify the run name the logs for the latest run will be retrieved
+> mcli logs
 
-    if not connect:
-        return 0
+# View the logs of a specific node in a multi-node run
+> mcli logs multinode-run-1234 --rank 1
 
-    try:
-        mint_shell = shell.MintShell(run.name, rank=rank)
-        mint_shell.connect(command=command)
-    except MintException as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    return 0
+# Follow the logs for an ongoing run
+> mcli logs run-1234 --follow
 
+# View the logs for a failed run
+> mcli logs run-1234 --failed
 
-def connect_entrypoint(
-    name: Optional[str] = None,
-    rank: int = 0,
-    latest: bool = False,
-    command: Optional[str] = None,
-    tmux: Optional[bool] = None,
-    **kwargs,
-):
-    del kwargs
+# View the logs for the run's first attempt
+> mcli logs run-1234 --attempt-index 0
+"""
 
-    if name:
-        runs = get_runs([name])
-        if not runs:
-            # TODO: could have nice suggestions or latest defaults
-            logger.error(f'{FAIL} Unknown run {name}')
-            return 1
-        run = runs[0]
-    else:
-        available_runs = get_runs(statuses=[RunStatus.STARTING, RunStatus.RUNNING])
-        if not available_runs:
-            logger.error(f'{FAIL} No running runs available to connect to')
-            return 1
-        elif len(available_runs) == 1:
-            run = available_runs[0]
-        else:
-            sorted_runs = sorted(available_runs, key=lambda x: x.created_at, reverse=True)
+# pylint: disable-next=invalid-name
+DEPLOYMENT_LOG_EXAMPLES = """
 
-            if len(available_runs) > 10:
-                available_runs = sorted(available_runs, key=lambda x: x.created_at, reverse=True)[:10]
+Examples:
 
-            if latest:
-                run = sorted_runs[0]
-            else:
+# View the current logs of an ongoing deployment
+> mcli get deployment logs deploy-1234
 
-                def get_name(r: Run):
-                    if r.started_at:
-                        details = f'Started at {format_timestamp(r.started_at)}'
-                    else:
-                        details = 'Not yet started'
-                    return f'{r.name} ({details})'
-
-                run = choose_one(
-                    'What run would you like to connect to?',
-                    options=available_runs,
-                    formatter=get_name,
-                )
+# By default, the logs for the latest deployment will be retrieved
+> mcli get deployment logs
 
-    ready = wait_for_run(run)
-    if not ready:
-        return 1
+# View the logs of a specific restart in a deployment
+> mcli get deployment logs deploy-1234 --restart 5
+"""
 
-    if tmux:
-        command = get_tmux_command()
 
-    try:
-        mint_shell = shell.MintShell(run.name, rank=rank)
-        mint_shell.connect(command=command)
-    except MintException as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    return 0
+def _get_run_logs(run: Run, follow: bool, rank: Optional[int], failed: bool,
+                  attempt: Optional[int]) -> Tuple[Optional[str], int]:
+
+    if run.status == RunStatus.FAILED and not failed and rank is None:
+        if run.reason and run.reason == "FailedImagePull":
+            suggestion = 'Try `mcli describe run {run.name}` and double-check that your image name is correct.'
+            logger.info(
+                f'{INFO} Run {run.name} has failed during image pull, so there are likely no logs. {suggestion}')
+        else:
+            err_message = f'({run.reason})' if run.reason else ''
+            logger.info(
+                f'{INFO} Run {run.name} has failed. {err_message} Defaulting to show the first failed node rank.')
+        failed = True
+
+    if follow and run.status.before(RunStatus.RUNNING):
+        with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
+            run = watcher.follow()
+
+    if run.status == RunStatus.FAILED_PULL:
+        CommonLog(logger).log_pod_failed_pull(run.name, run.config.image)
+        return '', 1
+    elif run.status.before(RunStatus.QUEUED, inclusive=True):
+        # Pod still waiting to be scheduled. Return
+        logger.error(f'{FAIL} Run {run.name} has not been scheduled')
+        return '', 1
+    elif run.status.before(RunStatus.RUNNING):
+        # Pod still not running, probably because follow==False
+        logger.error(f'{FAIL} Run has not yet started. You can check the status with `mcli get runs` '
+                     'and try again later.')
+        return '', 1
+
+    last_line: Optional[str] = None
+    end: str = ''
+    if follow:
+        for line in follow_run_logs(run, rank=rank, attempt=attempt):
+            print(line, end=end)
+            if line:
+                last_line = line
+        return last_line, int(0)
+    else:
+        log_lines = get_run_logs(run, rank=rank, failed=failed, attempt=attempt)
+        for line in log_lines:
+            # When using progress bars we randomly get newlines added. By default,
+            # kubernetes does not return empty lines when streaming, which is
+            # replicated in `follow_run_logs`. We'll do that here for parity
+            if line:
+                last_line = line
+                print(line, end='')
+        return last_line, int(0)
+
+
+def _get_deployment_logs(deploy: InferenceDeployment, restart) -> Tuple[Optional[str], int]:
+    log_lines = get_inference_deployment_logs(deploy, restart=restart)
+    last_line: Optional[str] = None
+    for line in log_lines:
+        # When using progress bars we randomly get newlines added. By default,
+        # kubernetes does not return empty lines when streaming, which is
+        # replicated in `follow_run_logs`. We'll do that here for parity
+        if line:
+            last_line = line
+            print(line, end='')
+    return last_line, 0
+
+
+def get_with_filters(submission_type: SubmissionType,
+                     name: Optional[str] = None,
+                     latest: bool = False) -> Union[List[Run], List[InferenceDeployment]]:
+    name_filter = [name] if name else None
+    if submission_type == SubmissionType.RUN:
+        return get_runs_with_filters(name_filter=name_filter, latest=latest)
+    else:
+        return get_deployments_with_filters(name_filter=name_filter)
 
 
-def get_tmux_command() -> str:
-    # set the command to a tmux entrypoint
-    # Check if tmux already exists
-    # command -v tmux >/dev/null 2>&1: Check if tmux already exists
-    # apt update && apt install -yq tmux: If not, quietly install. Assumes debian-based systems with apt
-    install_command = 'command -v tmux >/dev/null 2>&1 || (apt update && apt install -yq tmux)'
-
-    # new-session: Create a session
-    # -A: Attach if one exists (for auto-reconnect)
-    # -s main: Name the session ("main") for clarity
-    # -D: Disconnect other clients (from previous connections)
-    session_command = 'tmux new-session -A -s main -D'
-    return f'/bin/bash -c "({install_command}) && {session_command}"'
-
-
-def interactive_entrypoint(
-    name: Optional[str] = None,
-    cluster: Optional[str] = None,
-    gpu_type: Optional[str] = None,
-    gpus: Optional[int] = None,
-    hrs: Optional[float] = None,
-    hours: Optional[float] = None,
-    image: str = 'mosaicml/pytorch',
-    connect: bool = True,
-    rank: int = 0,
-    command: Optional[str] = None,
-    tmux: Optional[bool] = None,
+# pylint: disable-next=too-many-statements
+def get_logs(
+    submission_type: SubmissionType,
+    submission_name: Optional[str] = None,
+    rank: Optional[int] = None,
+    restart: Optional[int] = None,
+    follow: bool = False,
+    failed: bool = False,
+    attempt: Optional[int] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
-    # Hours can be specified as a positional argument (hrs) or named argument (hours)
-    if hours and hrs:
-        logger.error(f'{FAIL} The duration of your interactive session was specified twice. '
-                     'Please use only the positional argument or --hours. '
-                     'See mcli interactive --help for more details.')
-
-    hours = hrs or hours
-    if hours is None:
-        logger.error(f'{FAIL} Please specify the duration of your interactive session. '
-                     'See mcli interactive --help for details.')
-        return 1
-
-    if tmux:
-        command = get_tmux_command()
-
-    return interactive(
-        name=name,
-        cluster=cluster,
-        gpu_type=gpu_type,
-        gpus=gpus,
-        hours=hours,
-        image=image,
-        rank=rank,
-        connect=connect,
-        command=command,
-    )
-
-
-# TODO: Move into mcli/cli/m_interactive/m_interactive.py once kube mcli deprecated
-def configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-
-    hrs_grp = parser.add_mutually_exclusive_group()
-    hrs_grp.add_argument(
-        'hrs',
-        metavar='HOURS',
-        nargs='?',
-        type=get_hours_type(),
-        help='Number of hours the interactive session should run',
-    )
-    hrs_grp.add_argument(
-        '--hours',
-        nargs='?',
-        type=get_hours_type(),
-        help='Number of hours the interactive session should run',
-    )
+    try:
+        submission_type_str = submission_type.value.lower()
+        with err_console.status(f'Getting {submission_type_str} details...') as spinner:
+            if submission_name is None:
+                spinner.update(f'No {submission_type_str} name provided. Finding latest {submission_type_str}'
+                               f'...')
+                submissions = get_with_filters(submission_type, submission_name, latest=True)
+                if not submissions:
+                    raise MAPIException(status=HTTPStatus.NOT_FOUND, message=f'No {submission_type_str} found')
+                logger.info(
+                    f'{INFO} No {submission_type_str} name provided. Displaying log of latest {submission_type_str}: '
+                    f'[cyan]{submissions[0].name}[/]')
+            else:
+                submissions = get_with_filters(submission_type, submission_name, latest=True)
+                if not submissions:
+                    raise MAPIException(status=HTTPStatus.NOT_FOUND,
+                                        message=f'Could not find {submission_type_str}: [red]{submission_name}[/]')
+
+        last_line: Optional[str] = None
+        #Have to check type to satisfy pyright
+        if isinstance(submissions[0], Run):
+            last_line, err = _get_run_logs(submissions[0], follow, rank, failed, attempt)
+            if err == 1:
+                return 1
+        elif isinstance(submissions[0], InferenceDeployment):
+            last_line, err = _get_deployment_logs(submissions[0], restart)
+            if err == 1:
+                return 1
+
+        # Progress bars are weird. Let's add a final newline so that if the printing
+        # ends on an incompleted progress bar, it isn't erased
+        if last_line:
+            print('', file=sys.stderr)
 
-    parser.add_argument(
-        '--name',
-        default=None,
-        metavar='NAME',
-        type=str,
-        help='Name for the interactive session. '
-        'Default: "interactive-<gpu type>-<gpu num>"',
-    )
+    except MAPIException as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
+    except RuntimeError as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
+    except BrokenPipeError:
+        # This is raised when output is piped to programs like `head`
+        # Error handling taken from this example in the python docs:
+        # https://docs.python.org/3/library/signal.html#note-on-sigpipe
+        devnull = os.open(os.devnull, os.O_WRONLY)
+        os.dup2(devnull, sys.stdout.fileno())
 
-    cluster_arguments = parser.add_argument_group('Instance settings')
-    cluster_arguments.add_argument('--cluster',
-                                   default=None,
-                                   metavar='CLUSTER',
-                                   help='Cluster where your interactive session should run. If you '
-                                   'only have one available, that one will be selected by default. '
-                                   'Depending on your cluster, you\'ll have access to different GPU types and counts. '
-                                   'See the available combinations above. ')
-
-    cluster_arguments.add_argument(
-        '--gpu-type',
-        metavar='TYPE',
-        help='Type of GPU to use. Valid GPU types depend on the cluster and GPU numbers requested',
-    )
-    cluster_arguments.add_argument(
-        '--gpus',
-        type=int,
-        metavar='NGPUs',
-        help='Number of GPUs to run interactively. Valid GPU numbers depend on the cluster and GPU type',
-    )
+        return 1
 
-    parser.add_argument(
-        '--image',
-        default='mosaicml/pytorch',
-        help='Docker image to use',
-    )
+    return 0
 
-    command_grp = parser.add_mutually_exclusive_group()
-    command_grp.add_argument(
-        '--command',
-        help='The command you\'d like to execute on entry into your run. Defaults to /bin/bash',
-    )
-    command_grp.add_argument(
-        '--tmux',
-        action='store_true',
-        help='Use tmux as the entrypoint for your run so your session is robust to disconnects',
-    )
 
-    parser.add_argument(
-        '--no-connect',
-        dest='connect',
-        action='store_false',
-        help='Do not connect to the interactive session immediately',
-    )
+def configure_deployments_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.set_defaults(func=partial(get_logs, SubmissionType.DEPLOYMENT))
 
-    parser.add_argument('--rank',
-                        metavar='N',
-                        default=0,
+    parser.add_argument('submission_name',
+                        metavar='DEPLOYMENT',
+                        help='The name of the inference deployment to fetch logs for.')
+    parser.add_argument('--restart',
                         type=int,
-                        help='Connect to the specified node rank within the run')
-    parser.set_defaults(func=interactive_entrypoint)
-    return parser
-
+                        default=None,
+                        help='Which restart to fetch logs for. If not provided, will fetch logs of most recent restart')
 
-def add_interactive_argparser(subparser: argparse._SubParsersAction,) -> argparse.ArgumentParser:
-    """Adds the get parser to a subparser
-
-    Args:
-        subparser: the Subparser to add the Get parser to
-    """
-    examples = """
+    return parser
 
-Examples:
 
-# Create a 1 hour run to be used for interactive
-> mcli interactive --hours 1
+def configure_runs_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.set_defaults(func=partial(get_logs, SubmissionType.RUN))
+    parser.add_argument('submission_name',
+                        metavar='RUN',
+                        nargs='?',
+                        help='The name of the run. If not provided, will return the logs of the latest run')
+    parser.add_argument('--attempt',
+                        type=int,
+                        default=None,
+                        metavar='N',
+                        dest='attempt',
+                        help="Attempt (0-indexed) of the run whose logs you'd like to view.")
+    rank_grp = parser.add_mutually_exclusive_group()
+    rank_grp.add_argument('--rank',
+                          type=int,
+                          default=None,
+                          metavar='N',
+                          help='Rank of the node in a multi-node run whose logs you\'d like to view')
+    rank_grp.add_argument('--failed',
+                          action='store_true',
+                          dest='failed',
+                          default=False,
+                          help='Get the logs of the first failed node rank in a multinode run.')
+    follow_grp = parser.add_mutually_exclusive_group()
+    follow_grp.add_argument('--no-follow',
+                            action='store_false',
+                            dest='follow',
+                            default=False,
+                            help='Do not follow the logs of an in-progress run. '
+                            'Simply print any existing logs and exit. This is the default behavior.')
+    follow_grp.add_argument('-f',
+                            '--follow',
+                            action='store_true',
+                            dest='follow',
+                            default=False,
+                            help='Follow the logs of an in-progress run.')
 
-# Create a 1 hour run to be used for interactive with custom name and docker image
-> mcli interactive --hours 1 --image my-image --name my-run
+    return parser
 
-# Connect to the latest run
-> mcli connect
 
-# Connect to the rank 1 node from interactive session my-run-1234
-> mcli interactive -r my-run-1234 --rank 1
+def add_log_parser(subparser: argparse._SubParsersAction, submission_type: SubmissionType):
+    """Add the parser for retrieving submission logs
     """
 
-    interactive_parser: argparse.ArgumentParser = subparser.add_parser(
-        'interactive',
-        help='Create an interactive session',
-        description=('Create an interactive session. '
-                     'Once created, you can attach to the session. '),
+    log_parser: argparse.ArgumentParser = subparser.add_parser(
+        'logs',
+        aliases=['log'],
+        help=f'View the logs from a specific {submission_type.value.lower()}',
+        description=f'View the logs of an ongoing, completed or failed {submission_type.value.lower()}',
+        epilog=RUN_LOG_EXAMPLES if submission_type == SubmissionType.RUN else DEPLOYMENT_LOG_EXAMPLES,
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        epilog=examples,
     )
-    get_parser = configure_argparser(parser=interactive_parser)
-    return get_parser
+    log_parser = configure_runs_argparser(
+        log_parser) if submission_type == SubmissionType.RUN else configure_deployments_argparser(log_parser)
+
+    return log_parser
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.8/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.8/mcli/cli/m_interactive/m_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         default_namespace = ''
         for c in kube_config.list_kube_config_contexts()[0]:
             if c.get('name') == context:  # type: ignore
                 default_namespace = c.get('context', {}).get('namespace', '')  # type: ignore
                 break
 
-        if MCLIConfig.load_config(safe=True).internal:
+        if MCLIConfig.load_config().internal:
             default_namespace = 'mosaicml-orchestration'
 
         namespace = simple_prompt(
             f'Which kube namespace should be used to connect to the interactive run? [{default_namespace}]',
             default=default_namespace,
             mandatory=False,
         )
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.4.8/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.4.8/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.4.8/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.4.8/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.8/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.8/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.8/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.8/mcli/cli/m_run/m_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
     parser.add_argument(
         '--instance',
         dest='override_instance',
         help='Optional override for instance type',
     )
 
-    conf = MCLIConfig.load_config(safe=True)
+    conf = MCLIConfig.load_config()
     if conf.internal:
         parser.add_argument(
             '-o',
             '--optimization_level',
             dest='override_optimization_level',
             choices=VALID_OPTIMIZATION_LEVELS,
             type=int,
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             if api_key_value is None:
                 api_key_value = secret_prompt('What value would you like to set?', validate=validate_api_plaintext)
         except InputDisabledError:
             logger.error(INPUT_DISABLED_MESSAGE)
             return 1
 
     # Get the current api key
-    conf = MCLIConfig.load_config(safe=True)
+    conf = MCLIConfig.load_config()
 
     current_api_key = conf.get_api_key(env_override=False)
     if current_api_key == api_key_value:
         logger.info(f"{OK} The API key has already been set with this value")
         return 0
 
     # Don't override existing values without confirmation
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/feature_flag.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from mcli.utils.utils_logging import FAIL, OK
 
 logger = logging.getLogger(__name__)
 
 
 def use_feature_flag(feature: Optional[str], activate: bool = True, **kwargs) -> int:
     del kwargs
-    conf = config.MCLIConfig.load_config(safe=True)
+    conf = config.MCLIConfig.load_config()
     available_features = conf.mcli_mode.available_feature_flags()
     available_features_str = [x.value for x in available_features]
     feature_flag: Optional[config.FeatureFlag] = None
     if feature:
         feature = feature.upper()
         if feature not in available_features_str:
             if not available_features_str:
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ mcli modify user functions """
 import argparse
 import logging
 from typing import Optional
 
-from mcli.config import MESSAGE, MCLIConfig, MCLIConfigError
+from mcli.config import MCLIConfig
 from mcli.utils.utils_logging import OK
 
 logger = logging.getLogger(__name__)
 
 
 def modify_user(
     user_id: Optional[str] = None,
@@ -17,20 +17,15 @@
 
     Returns:
         0 if succeeded, else 1
     """
     del kwargs
 
     # Get the current user
-    try:
-        conf = MCLIConfig.load_config()
-    except MCLIConfigError:
-        logger.error(MESSAGE.MCLI_NOT_INITIALIZED)
-        return 1
-
+    conf = MCLIConfig.load_config()
     conf.user_id = user_id
     conf.save_config()
 
     if user_id:
         logger.info(f"{OK} Updated User to {user_id}")
     else:
         logger.info(f"{OK} Removed User")
```

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.8/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.8/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.8/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/config.py` & `mosaicml-cli-0.4.8/mcli/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Global Singleton Config Store"""
 from __future__ import annotations
 
 import logging
 import os
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set
 
 import ruamel.yaml
 import yaml
 from ruamel.yaml import YAML
 from ruamel.yaml.comments import CommentedMap
 
-from mcli.api.exceptions import MCLIConfigError
-from mcli.models import Cluster
-from mcli.utils.utils_serializable_dataclass import SerializableDataclass
 from mcli.utils.utils_yaml import StringDumpYAML
 
+logging.getLogger('urllib3.connectionpool').disabled = True
 logger = logging.getLogger(__name__)
 
 
 def env_path_override_config(config_value: str):
     if config_value in os.environ:
         globals()[config_value] = Path(os.environ[config_value])
 
@@ -31,17 +29,14 @@
     if config_value in os.environ:
         globals()[config_value] = os.environ[config_value]
 
 
 MCLI_CONFIG_DIR: Path = Path(os.path.expanduser('~/.mosaic'))
 env_path_override_config('MCLI_CONFIG_DIR')
 
-MCLI_BACKUP_CONFIG_DIR: Path = Path(os.path.expanduser('~/.mosaic.bak'))
-env_path_override_config('MCLI_BACKUP_CONFIG_DIR')
-
 MOSAICML_API_ENDPOINT: str = 'https://api.mosaicml.com/graphql'
 MOSAICML_API_ENDPOINT_STAGING: str = 'https://staging.api.mosaicml.com/graphql'
 MOSAICML_API_ENDPOINT_DEV: str = 'https://dev.api.mosaicml.com/graphql'
 MOSAICML_API_ENDPOINT_LOCAL: str = 'http://localhost:3001/graphql'
 MOSAICML_API_ENDPOINT_ENV: str = 'MOSAICML_API_ENDPOINT'
 env_str_override_config(MOSAICML_API_ENDPOINT_ENV)
 
@@ -51,17 +46,14 @@
 MOSAICML_MINT_ENDPOINT_LOCAL: str = 'ws://localhost:3004/v1/shell'
 MOSAICML_MINT_ENDPOINT_ENV: str = 'MOSAICML_MINT_ENDPOINT'
 env_str_override_config(MOSAICML_MINT_ENDPOINT_ENV)
 
 MCLI_CONFIG_PATH: Path = MCLI_CONFIG_DIR / 'mcli_config'
 env_path_override_config('MCLI_CONFIG_PATH')
 
-MCLI_KUBECONFIG: Path = MCLI_CONFIG_DIR / 'kube_config'
-env_path_override_config('MCLI_KUBECONFIG')
-
 UPDATE_CHECK_FREQUENCY_DAYS: float = 2
 
 MCLI_MODE_ENV: str = 'MCLI_MODE'
 env_str_override_config(MCLI_MODE_ENV)
 
 MCLI_INTERACTIVE_ENV: str = 'MCLI_INTERACTIVE'
 env_str_override_config(MCLI_INTERACTIVE_ENV)
@@ -71,18 +63,14 @@
 
 MCLI_DISABLE_UPGRADE_CHECK_ENV: str = 'MCLI_DISABLE_UPGRADE_CHECK'
 env_str_override_config(MCLI_DISABLE_UPGRADE_CHECK_ENV)
 
 # Used for local dev and testing
 MOSAICML_API_KEY_ENV: str = 'MOSAICML_API_KEY'
 
-logging.getLogger('urllib3.connectionpool').disabled = True
-
-logger = logging.getLogger(__name__)
-
 ADMIN_MODE = False
 
 
 def get_timeout(default_timeout: Optional[float] = None) -> Optional[float]:
     timeout_env = os.environ.get(MCLI_TIMEOUT_ENV)
 
     if timeout_env:
@@ -168,26 +156,22 @@
         """True if the mode is a valid alternate mcloud environment
         """
         alternate_env_modes = {MCLIMode.DEV, MCLIMode.LOCAL, MCLIMode.STAGING}
         return self in alternate_env_modes
 
 
 @dataclass
-class MCLIConfig(SerializableDataclass):
+class MCLIConfig:
     """Global Config Store persisted on local disk"""
 
-    # set to default for now to not break existing users' configs
     MOSAICML_API_KEY: str = ''  # pylint: disable=invalid-name Global Stored within Singleton
 
     feature_flags: Dict[str, bool] = field(default_factory=dict)
     last_update_check: datetime = field(default_factory=datetime.now)
 
-    # Registered Clusters
-    clusters: List[Cluster] = field(default_factory=list)
-
     # MCloud environments w/ API keys
     # Most users will be in PROD, so this will likely only be touched internally
     mcloud_envs: Dict[str, str] = field(default_factory=dict)
 
     _user_id: Optional[str] = None
 
     @property
@@ -226,23 +210,21 @@
         return disable_env == 'true'
 
     @property
     def endpoint(self) -> str:
         """The user's MAPI endpoint
         """
         env_endpoint = os.environ.get(MOSAICML_API_ENDPOINT_ENV, None)
-
         return env_endpoint or self.mcli_mode.endpoint
 
     @property
     def mint_endpoint(self) -> str:
         """The user's MINT endpoint
         """
         env_endpoint = os.environ.get(MOSAICML_MINT_ENDPOINT_ENV, None)
-
         return env_endpoint or self.mcli_mode.mint_endpoint
 
     @property
     def api_key(self):
         """The user's configured MCloud API key
         """
         return self.get_api_key(env_override=True)
@@ -271,89 +253,94 @@
             return api_key_env
         elif self.mcli_mode.is_alternate():
             return self.mcloud_envs.get(self.mcli_mode.value, '')
         elif self.MOSAICML_API_KEY:
             return self.MOSAICML_API_KEY
         return ''
 
-    @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> MCLIConfig:
-        # TODO: Remove after full deprecation transition
-        if 'dev_mode' in data:
-            del data['dev_mode']
-        if 'internal' in data:
-            del data['internal']
-        # TODO(END): Remove after full deprecation transition
-
-        # Backwards compatibility: platforms should be synonymous with clusters
-        if 'platforms' in data:
-            data['clusters'] = data['platforms']
-            del data['platforms']
+    def to_dict(self) -> Dict[str, Any]:
+        """Converts the config to a dictionary
 
-        if 'environment_variables' in data:
-            del data['environment_variables']
+        Returns:
+            Dict[str, Any]: The dictionary representation of the config
+        """
+        res: Dict[str, Any] = {
+            'last_update_check': self.last_update_check,
+        }
 
-        data['clusters'] = []
+        # Only add configs if they are filled
+        if self.MOSAICML_API_KEY:
+            res['MOSAICML_API_KEY'] = self.MOSAICML_API_KEY
 
-        # Remove any unknown feature flags
-        known_feature_flags = {f.value for f in FeatureFlag}
-        data['feature_flags'] = {k: v for k, v in data.get('feature_flags', {}).items() if k in known_feature_flags}
+        if self.feature_flags:
+            res['feature_flags'] = self.feature_flags
+
+        if self.mcloud_envs:
+            res['mcloud_envs'] = self.mcloud_envs
 
-        return super().from_dict(data)
+        if self._user_id:
+            res['_user_id'] = self._user_id
+
+        return res
 
     @classmethod
-    def load_config(cls, safe: bool = False) -> MCLIConfig:
-        """Loads the MCLIConfig from local disk
+    def from_dict(cls, data: Dict[str, Any]) -> MCLIConfig:
+        # Remove any unknown or false feature flags
+        known_feature_flags = {f.value for f in FeatureFlag}
+        feature_flags = {k: v for k, v in data.get('feature_flags', {}).items() if k in known_feature_flags and v}
 
+        if isinstance(data.get('last_update_check'), str):
+            last_update_check = datetime.fromisoformat(data['last_update_check'])
+        elif isinstance(data.get('last_update_check'), datetime):
+            last_update_check = data['last_update_check']
+        else:
+            last_update_check = datetime.now()
 
-        Args:
-            safe (bool): If safe is true, if the config fails to load it will return
-                an empty generated config
+        return MCLIConfig(
+            MOSAICML_API_KEY=data.get('MOSAICML_API_KEY', ''),
+            feature_flags=feature_flags,
+            last_update_check=last_update_check,
+            mcloud_envs=data.get('mcloud_envs', {}),
+            _user_id=data.get('_user_id', None),
+        )
+
+    @classmethod
+    def load_config(cls) -> MCLIConfig:
+        """Loads the MCLIConfig from local disk
 
         Return:
-            Returns the MCLIConfig if successful, otherwise raises MCLIConfigError
+            Returns the MCLIConfig, if not found, returns a new empty config
         """
         try:
             with open(MCLI_CONFIG_PATH, 'r', encoding='utf8') as f:
                 data: Dict[str, Any] = yaml.full_load(f)
-            conf: MCLIConfig = cls.from_dict(data)
-        except FileNotFoundError as e:
-            if safe:
-                return MCLIConfig.empty()
-            raise MCLIConfigError(Messages.MCLI_NOT_INITIALIZED) from e
-
-        # Optional values can get filled in over time. If a new optional value is not
-        # present in the config, let it be filled in by the default, if one was set.
-        if set(asdict(conf)) != set(data):
-            # TODO: Bug on over-saving HEK-452
-            conf.save_config()  # pylint: disable=no-member
+            conf = cls.from_dict(data)
+        except FileNotFoundError:
+            conf = MCLIConfig.empty()
 
         return conf
 
     def save_config(self) -> bool:
         """Saves the MCLIConfig to local disk
 
         Return:
             Returns true if successful
         """
+        logger.debug(f'Saving config to {MCLI_CONFIG_PATH}')
         data = self._get_formatted_dump()
         y = YAML()
         y.explicit_start = True  # type: ignore
         with open(MCLI_CONFIG_PATH, 'w', encoding='utf8') as f:
             y.dump(data, f)
         return True
 
     def _get_formatted_dump(self) -> CommentedMap:
         """Gets the ruamel yaml formatted dump of the config
         """
-        raw_data = self.to_disk()
-
-        # Remove clusters
-        del raw_data['clusters']
-
+        raw_data = self.to_dict()
         data: CommentedMap = ruamel.yaml.load(
             yaml.dump(raw_data),
             ruamel.yaml.RoundTripLoader,
         )
         return data
 
     def feature_enabled(self, feature: FeatureFlag) -> bool:
@@ -382,17 +369,9 @@
     def __str__(self) -> str:
         data = self._get_formatted_dump()
         y = StringDumpYAML()
         return y.dump(data)
 
 
 def feature_enabled(feature: FeatureFlag) -> bool:
-    conf = MCLIConfig.load_config(safe=True)
+    conf = MCLIConfig.load_config()
     return conf.feature_enabled(feature=feature)
-
-
-class Messages():
-    MCLI_NOT_INITIALIZED = 'MCLI not yet initialized. Please run `mcli init` first.'
-    API_KEY_MISSING = 'No API key found. Please create one and set it using `mcli set api-key`.'
-
-
-MESSAGE = Messages()
```

### Comparing `mosaicml-cli-0.4.7/mcli/models/__init__.py` & `mosaicml-cli-0.4.8/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.8/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.8/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.8/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/models/run_config.py` & `mosaicml-cli-0.4.8/mcli/models/run_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
         Raises:
             :class:`~mcli.api.exceptions.MCLIConfigError`: If MCLI config is not present or is missing information
             :class:`~mcli.api.exceptions.MCLIRunConfigValidationError`: If run_config is not valid
         """
         # pylint: disable-next=import-outside-toplevel
         from mcli.config import MCLIConfig
-        conf = MCLIConfig.load_config(safe=True)
+        conf = MCLIConfig.load_config()
 
         if run_config.cpus is None:
             run_config.cpus = 0
 
         # MosaicML Agent is disabled for all external users
         if not conf.internal or run_config.optimization_level is None:
             # TODO: not all docker images will support adding the MosaicML Agent
```

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.8/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.8/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.8/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_pypi.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     Raises:
         NeedsUpdateError: Raised if the user is too far behind on updates
     """
     if current_version is None:
         # Lazy sets current_version for monkeypatched tests
         current_version = _current_version
 
-    conf = MCLIConfig.load_config(safe=True)
+    conf = MCLIConfig.load_config()
 
     # Don't check if user is on dev/local mode
     if conf.mcli_mode.is_alternate():
         return
 
     if conf.disable_upgrade:
         return
```

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.8/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/mcli/version.py` & `mosaicml-cli-0.4.8/mcli/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 def get_formatted_version() -> str:
     """ Return version number as a string """
     # pylint: disable=import-outside-toplevel
     from mcli.config import FeatureFlag, MCLIConfig
     from mcli.utils.utils_pypi import get_latest_alpha_package_version, get_latest_package_version
 
     latest_version = current_version = Version.from_string(__version__)
-    conf = MCLIConfig.load_config(safe=True)
+    conf = MCLIConfig.load_config()
     is_alpha = current_version.is_alpha or conf.feature_enabled(FeatureFlag.ALPHA_TESTER)
     version_output = ''
     try:
         if is_alpha:
             latest_version = get_latest_alpha_package_version()
         else:
             latest_version = get_latest_package_version()
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.4.7'
+__version__ = '0.4.8'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.7/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.8/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.7
+Version: 0.4.8
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.7/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.8/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -149,10 +149,12 @@
 mcli/utils/utils_yaml.py
 mosaicml_cli.egg-info/PKG-INFO
 mosaicml_cli.egg-info/SOURCES.txt
 mosaicml_cli.egg-info/dependency_links.txt
 mosaicml_cli.egg-info/entry_points.txt
 mosaicml_cli.egg-info/requires.txt
 mosaicml_cli.egg-info/top_level.txt
+tests/__init__.py
+tests/conftest.py
 tests/test_config.py
 tests/test_simple.py
 tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.7/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.8/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-yapf>=0.33.0
-sphinxcontrib-applehelp>=1.0.2
+sphinx-panels==0.6.0
+sphinx-argparse==0.4.0
 sphinxcontrib-images>=0.9.4
-myst-parser>=0.16.1
 pre-commit>=2.17.0
-sphinx-markdown-tables==0.0.17
-sphinx_external_toc==0.3.0
-sphinx-panels==0.6.0
 sphinxemoji==0.2.0
-sphinx-argparse==0.4.0
 radon>=5.1.0
-docutils>=0.17.0
-sphinx-design
 isort>=5.9.3
+pytest>=6.2.5
 sphinxcontrib-katex==0.9.4
-furo==2022.9.29
+sphinxext-opengraph==0.8.2
+pyright==1.1.256
+sphinxcontrib-jsmath>=1.0.1
 pylint>=2.12.2
-pytest-mock>=3.7.0
+pytest-cov>=4.0.0
+sphinx-rtd-theme==1.0.0
+sphinxcontrib-applehelp>=1.0.2
+sphinx_external_toc==0.3.0
 sphinx-copybutton==0.5.2
-sphinxcontrib-qthelp>=1.0.3
-sphinxcontrib-devhelp>=1.0.2
-sphinxcontrib-jsmath>=1.0.1
-sphinx==4.4.0
 sphinxcontrib-htmlhelp>=2.0.0
-sphinx-rtd-theme==1.0.0
-twine>=4.0.2
+sphinxcontrib-qthelp>=1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-pytest>=6.2.5
-sphinxext-opengraph==0.8.2
-toml>=0.10.2
+twine>=4.0.2
+myst-parser>=0.16.1
+docutils>=0.17.0
+yapf>=0.33.0
+sphinx-design
+furo==2022.9.29
 build>=0.10.0
-pyright==1.1.256
-pytest-cov>=4.0.0
+sphinx==4.4.0
+sphinx-markdown-tables==0.0.17
+sphinxcontrib-devhelp>=1.0.2
+toml>=0.10.2
+pytest-mock>=3.7.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.4.7/pyproject.toml` & `mosaicml-cli-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/setup.py` & `mosaicml-cli-0.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.7/tests/test_config.py` & `mosaicml-cli-0.4.8/tests/test_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from contextlib import contextmanager
 
 import pytest
 
 from mcli.config import (MCLI_INTERACTIVE_ENV, MCLI_MODE_ENV, MOSAICML_API_ENDPOINT, MOSAICML_API_ENDPOINT_DEV,
                          MOSAICML_API_ENDPOINT_ENV, MOSAICML_API_ENDPOINT_LOCAL, MOSAICML_API_KEY_ENV, FeatureFlag,
-                         MCLIConfig, MCLIConfigError, MCLIMode)
+                         MCLIConfig, MCLIMode)
 
 
 @contextmanager
 def clear_envs(*envs):
     values = {}
     for k in envs:
         values[k] = os.environ.pop(k, None)
@@ -31,38 +31,43 @@
         },
         cluster_key: [
             {
                 'kubernetes_context': 'microk8s',
                 'name': 'microk8s',
                 'namespace': 'microk8s',
             },
-            # these should be ignored
             {
                 'kubernetes_context': 'unknown',
                 'name': 'unknown',
                 'namespace': 'unknown',
             },
             {
                 'kubernetes_context': 'aws-research-01',
             },
         ],
-        # these should be removed
         'dev_mode': True,
         'internal': True,
     }
     mcli_config = MCLIConfig.from_dict(data)
     assert mcli_config.feature_flags
     assert mcli_config.feature_enabled(FeatureFlag.ALPHA_TESTER)
 
+    conf = mcli_config.to_dict()
+    assert set(conf.keys()) == {'feature_flags', 'last_update_check'}
+
 
 def test_uninitialized(new_mcli_setup):
     """Test MCLIConfig fails to load for a new setup, raising a custom exception
     """
-    with pytest.raises(MCLIConfigError):
-        MCLIConfig.load_config()
+    conf = MCLIConfig.load_config()
+
+    assert conf.MOSAICML_API_KEY == ''
+    assert not conf.internal
+    assert conf.mcli_mode == MCLIMode.PROD
+    assert conf.endpoint == MOSAICML_API_ENDPOINT
 
 
 def test_initialized(base_mcli_setup):
     """Test MCLIConfig successfully loads
     """
     config = MCLIConfig.load_config()
 
@@ -72,20 +77,41 @@
     assert config.endpoint == MOSAICML_API_ENDPOINT
 
 
 def test_config_save_load(new_mcli_setup):
     """Test basic save and load
     """
     conf = MCLIConfig.empty()
+    conf._user_id = '123'
     conf.save_config()
 
     conf2 = MCLIConfig.load_config()
+    assert conf2._user_id == '123'
     assert conf.to_dict() == conf2.to_dict()
 
 
+def test_feature_flags(new_mcli_setup, mocker):
+    mocker.patch('mcli.config.MCLIConfig.internal', new_callable=mocker.PropertyMock, return_value=True)
+
+    conf = MCLIConfig.from_dict({"feature_flags": {"UNKNOWN": True}})
+    assert conf.feature_flags == {}
+    assert not conf.feature_enabled(FeatureFlag.ALPHA_TESTER)
+    assert not conf.to_dict().get("feature_flags")
+
+    conf2 = MCLIConfig.from_dict({"feature_flags": {FeatureFlag.ALPHA_TESTER.value: True}})
+    assert conf2.feature_flags == {FeatureFlag.ALPHA_TESTER.value: True}
+    assert conf2.feature_enabled(FeatureFlag.ALPHA_TESTER)
+    assert conf2.to_dict().get("feature_flags") == {FeatureFlag.ALPHA_TESTER.value: True}
+
+    conf3 = MCLIConfig.from_dict({"feature_flags": {FeatureFlag.ALPHA_TESTER.value: False}})
+    assert conf3.feature_flags == {}
+    assert not conf3.feature_enabled(FeatureFlag.ALPHA_TESTER)
+    assert not conf3.to_dict().get("feature_flags")
+
+
 def test_mcli_mode(new_mcli_setup):
     with clear_envs(MCLI_MODE_ENV, 'DOGEMODE'):
         conf = MCLIConfig.empty()
         assert conf.mcli_mode == MCLIMode.PROD
 
         os.environ[MCLI_MODE_ENV] = MCLIMode.DEV.value
         assert conf.mcli_mode == MCLIMode.DEV
```

### Comparing `mosaicml-cli-0.4.7/tests/test_upgrade.py` & `mosaicml-cli-0.4.8/tests/test_upgrade.py`

 * *Files identical despite different names*

