# Comparing `tmp/cgcsdk-0.9.0.tar.gz` & `tmp/cgcsdk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.9.0.tar", last modified: Tue Jun 13 11:20:52 2023, max compression
+gzip compressed data, was "cgcsdk-0.9.1.tar", last modified: Wed Jun 14 08:46:44 2023, max compression
```

## Comparing `cgcsdk-0.9.0.tar` & `cgcsdk-0.9.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.490730 cgcsdk-0.9.0/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-06-13 11:20:52.488733 cgcsdk-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.208077 cgcsdk-0.9.0/cgc/
--rw-rw-rw-   0        0        0      209 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/cgc/.env
--rw-rw-rw-   0        0        0     4450 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.9.0/cgc/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.9.0/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.223500 cgcsdk-0.9.0/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.236364 cgcsdk-0.9.0/cgc/commands/auth/
--rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.9.0/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.9.0/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.9.0/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.9.0/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.248292 cgcsdk-0.9.0/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     4061 2023-05-23 09:09:29.000000 cgcsdk-0.9.0/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.9.0/cgc/commands/cgc_cmd_responses.py
--rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.9.0/cgc/commands/cgc_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.265104 cgcsdk-0.9.0/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.9.0/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.9.0/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      959 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.9.0/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.272104 cgcsdk-0.9.0/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.9.0/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.282326 cgcsdk-0.9.0/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.9.0/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.9.0/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.9.0/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.293409 cgcsdk-0.9.0/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.9.0/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.319365 cgcsdk-0.9.0/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.9.0/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.9.0/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.9.0/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.9.0/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.9.0/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/config.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.342605 cgcsdk-0.9.0/cgc/sdk/
--rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.9.0/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.9.0/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.9.0/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.9.0/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     2840 2023-05-29 15:06:35.000000 cgcsdk-0.9.0/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-0.9.0/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.348615 cgcsdk-0.9.0/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.9.0/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.359226 cgcsdk-0.9.0/cgc/tests/
--rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.9.0/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.403474 cgcsdk-0.9.0/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.9.0/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.9.0/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.449836 cgcsdk-0.9.0/cgc/utils/
--rw-rw-rw-   0        0        0     3405 2023-05-19 13:08:19.000000 cgcsdk-0.9.0/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.9.0/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-0.9.0/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.457687 cgcsdk-0.9.0/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-0.9.0/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.467907 cgcsdk-0.9.0/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.9.0/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.9.0/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1773 2023-05-23 09:05:26.000000 cgcsdk-0.9.0/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2488 2023-05-23 09:03:57.000000 cgcsdk-0.9.0/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     2050 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.9.0/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.9.0/cgc/utils/update.py
--rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:20:52.484735 cgcsdk-0.9.0/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-06-13 11:20:52.000000 cgcsdk-0.9.0/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2023-06-13 11:20:52.000000 cgcsdk-0.9.0/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 11:20:52.000000 cgcsdk-0.9.0/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-13 11:20:52.000000 cgcsdk-0.9.0/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-06-13 11:20:52.000000 cgcsdk-0.9.0/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 11:20:52.000000 cgcsdk-0.9.0/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 11:20:52.490730 cgcsdk-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2096 2023-06-13 11:20:10.000000 cgcsdk-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.238045 cgcsdk-0.9.1/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-06-14 08:46:44.237157 cgcsdk-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:43.972209 cgcsdk-0.9.1/cgc/
+-rw-rw-rw-   0        0        0      209 2023-06-14 08:41:05.000000 cgcsdk-0.9.1/cgc/.env
+-rw-rw-rw-   0        0        0     4687 2023-06-14 08:43:44.000000 cgcsdk-0.9.1/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.9.1/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:43.987927 cgcsdk-0.9.1/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.004788 cgcsdk-0.9.1/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.9.1/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.9.1/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.9.1/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.9.1/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.030461 cgcsdk-0.9.1/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4711 2023-06-14 08:36:45.000000 cgcsdk-0.9.1/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     4061 2023-05-23 09:09:29.000000 cgcsdk-0.9.1/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.9.1/cgc/commands/cgc_cmd_responses.py
+-rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.9.1/cgc/commands/cgc_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.057307 cgcsdk-0.9.1/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      959 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.064932 cgcsdk-0.9.1/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.9.1/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.071689 cgcsdk-0.9.1/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.9.1/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.077743 cgcsdk-0.9.1/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.094389 cgcsdk-0.9.1/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.9.1/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.9.1/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.110643 cgcsdk-0.9.1/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.9.1/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.9.1/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     2840 2023-05-29 15:06:35.000000 cgcsdk-0.9.1/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-0.9.1/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.116837 cgcsdk-0.9.1/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.9.1/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.123399 cgcsdk-0.9.1/cgc/tests/
+-rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.9.1/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.156525 cgcsdk-0.9.1/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.189977 cgcsdk-0.9.1/cgc/utils/
+-rw-rw-rw-   0        0        0     3466 2023-06-13 12:13:50.000000 cgcsdk-0.9.1/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.9.1/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-0.9.1/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.199734 cgcsdk-0.9.1/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-0.9.1/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.212955 cgcsdk-0.9.1/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.9.1/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1773 2023-05-23 09:05:26.000000 cgcsdk-0.9.1/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2488 2023-05-23 09:03:57.000000 cgcsdk-0.9.1/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     2050 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.9.1/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.9.1/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.233230 cgcsdk-0.9.1/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:46:44.239027 cgcsdk-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     2096 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/setup.py
```

### Comparing `cgcsdk-0.9.0/PKG-INFO` & `cgcsdk-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.9.0
+Version: 0.9.1
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.9.0/cgc/CHANGELOG.md` & `cgcsdk-0.9.1/cgc/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Change Log
 
+## 0.9.1
+
+Release on June 14,2023
+
+* cgc billing - updated which values from response are taken to show
+  * cost_total in billing was shown correctly - no changes
+  * start, end, time: updated with correct key:value pairs from response
+
 ## 0.9.0
 
 Release on June 13, 2023.
 
 * APP TLS update - DNS for API endpoint
 * removed self signed certificate, server got signed certificate for cgc-api.comtegra.cloud
 * added new compose template: label-studio
```

### Comparing `cgcsdk-0.9.0/cgc/cgc.py` & `cgcsdk-0.9.1/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.9.1/cgc/commands/auth/auth_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.9.1/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.9.1/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/billing/__init__.py` & `cgcsdk-0.9.1/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.9.1/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.9.1/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.9.1/cgc/commands/billing/billing_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     :type costs_list: list
     :return: formatted list of costs and total cost for user
     :rtype: user_costs_list_to_print: list, total_user_cost: float
     """
     user_costs_list_to_print = []
     total_user_cost = 0
     for cost in costs_list:
-        rent_start = cost["rent_start"]
-        rent_end = cost["rent_end"]
-        rent_time = f"{int(cost['rent_time'])} s"
+        rent_start = cost["rent_start_cost"]
+        rent_end = cost["rent_end_cost"]
+        rent_time = f"{int(cost['rent_time_cost'])} s"
         rent_cost = f"{float(cost['cost_total']):.2f} pln"
         resources = cost["resources"]
         name = resources["name"]
         rent_type = cost["type"]
         if rent_type == "events_resource":
             entity = resources["entity"]
         elif rent_type == "events_volume":
```

### Comparing `cgcsdk-0.9.0/cgc/commands/cgc_cmd.py` & `cgcsdk-0.9.1/cgc/commands/cgc_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.9.1/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/cgc_helpers.py` & `cgcsdk-0.9.1/cgc/commands/cgc_helpers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.9.1/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/compute/compute_models.py` & `cgcsdk-0.9.1/cgc/commands/compute/compute_models.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.9.1/cgc/commands/compute/compute_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.9.1/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/db/db_cmd.py` & `cgcsdk-0.9.1/cgc/commands/db/db_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/resource/resource_cmd.py` & `cgcsdk-0.9.1/cgc/commands/resource/resource_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/volume/data_model.py` & `cgcsdk-0.9.1/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.9.1/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.9.1/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.9.1/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/sdk/handlers.py` & `cgcsdk-0.9.1/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/sdk/mongodb.py` & `cgcsdk-0.9.1/cgc/sdk/mongodb.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/sdk/postgresql.py` & `cgcsdk-0.9.1/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/sdk/redis.py` & `cgcsdk-0.9.1/cgc/sdk/redis.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/server.crt` & `cgcsdk-0.9.1/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/telemetry/basic.py` & `cgcsdk-0.9.1/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/tests/__init__.py` & `cgcsdk-0.9.1/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.9.1/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.9.1/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/tests/responses_tests.py` & `cgcsdk-0.9.1/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/__init__.py` & `cgcsdk-0.9.1/cgc/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,18 @@
         read_from_cfg(None, filename)
     except NoConfigFileFound:
         return False
     return True
 
 
 def list_all_config_files() -> List[str]:
-    only_files = [f for f in listdir(config_path) if isfile(join(config_path, f))]
+    try:
+        only_files = [f for f in listdir(config_path) if isfile(join(config_path, f))]
+    except FileNotFoundError:
+        return []
 
     def only_json_file(filename: str):
         return filename if filename.endswith(".json") else None
 
     def cgc_config_file(filename: str):
         filename_prefix = filename.split(".")[0]
         try:
```

### Comparing `cgcsdk-0.9.0/cgc/utils/click_group.py` & `cgcsdk-0.9.1/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/config_utils.py` & `cgcsdk-0.9.1/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/consts/env_consts.py` & `cgcsdk-0.9.1/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/consts/message_consts.py` & `cgcsdk-0.9.1/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.9.1/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.9.1/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.9.1/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/custom_exceptions.py` & `cgcsdk-0.9.1/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/message_utils.py` & `cgcsdk-0.9.1/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/prepare_headers.py` & `cgcsdk-0.9.1/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/requests_helper.py` & `cgcsdk-0.9.1/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/response_utils.py` & `cgcsdk-0.9.1/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgc/utils/version_control.py` & `cgcsdk-0.9.1/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.9.1/cgcsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.9.0
+Version: 0.9.1
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.9.0/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.9.1/cgcsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.0/setup.py` & `cgcsdk-0.9.1/setup.py`

 * *Files identical despite different names*

