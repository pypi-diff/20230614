# Comparing `tmp/evolved5g-1.0.5.tar.gz` & `tmp/evolved5g-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evolved5g-1.0.5.tar", last modified: Wed May 24 13:46:16 2023, max compression
+gzip compressed data, was "evolved5g-1.0.6.tar", last modified: Wed Jun 14 20:09:47 2023, max compression
```

## Comparing `evolved5g-1.0.5.tar` & `evolved5g-1.0.6.tar`

### file list

```diff
@@ -1,123 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.501783 evolved5g-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-24 13:45:36.000000 evolved5g-1.0.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-24 13:45:36.000000 evolved5g-1.0.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-24 13:45:36.000000 evolved5g-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 13:45:36.000000 evolved5g-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-24 13:46:16.501783 evolved5g-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-24 13:45:36.000000 evolved5g-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.489782 evolved5g-1.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.489782 evolved5g-1.0.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/dummy_html_example.png
--rw-r--r--   0 runner    (1001) docker     (123)   416176 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/generate.gif
--rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/generate_execution.png
--rw-r--r--   0 runner    (1001) docker     (123)    31097 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/repo_creation.png
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/repo_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/ssh_gpg.png
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/ssh_key.png
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/ssh_key_button.png
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/token1.png
--rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/token2.png
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/token3.png
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/information.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/libraries.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/pre_requisites.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/evolved5g/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    17764 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/cli_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/nef_and_tsn_api_service_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    88921 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/evolved5g/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.497782 evolved5g-1.0.5/evolved5g/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/cells_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/g_n_bs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/location_frontend_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/login_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/monitoring_event_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/paths_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/qo_s_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/u_es_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/ui_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/utils_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.501783 evolved5g-1.0.5/evolved5g/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/accumulated_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_u_es_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_create_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_update_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/cell_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/cell_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/location_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report_received.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/path_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/path_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/qo_s_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/qos_monitoring_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/reporting_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/snssai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/u_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/ue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/ue_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/ue_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/usage_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_notification_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/evolved5g.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:46:12.000000 evolved5g-1.0.5/evolved5g.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 13:45:36.000000 evolved5g-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 13:46:16.505783 evolved5g-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-24 13:45:36.000000 evolved5g-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.689367 evolved5g-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-14 20:09:05.000000 evolved5g-1.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-06-14 20:09:05.000000 evolved5g-1.0.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-14 20:09:05.000000 evolved5g-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 20:09:05.000000 evolved5g-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-14 20:09:47.689367 evolved5g-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-14 20:09:05.000000 evolved5g-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.677366 evolved5g-1.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.677366 evolved5g-1.0.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.681366 evolved5g-1.0.6/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/dummy_html_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/generate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/generate_execution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54245 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/netapp_creation.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   347578 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/netapp_repo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    55213 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/repo_creation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56898 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/repo_structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/ssh_gpg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/ssh_key.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/ssh_key_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/token1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/token2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/images/token3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/information.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/libraries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-14 20:09:05.000000 evolved5g-1.0.6/docs/source/pre_requisites.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.681366 evolved5g-1.0.6/evolved5g/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/cli_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/nef_and_tsn_api_service_validation_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91551 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.681366 evolved5g-1.0.6/evolved5g/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.685366 evolved5g-1.0.6/evolved5g/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/cells_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/g_n_bs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/location_frontend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/login_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/monitoring_event_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/paths_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/qo_s_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/u_es_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/ui_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api/utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.689367 evolved5g-1.0.6/evolved5g/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/accumulated_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_u_es_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_ue_create_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_ue_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_ue_update_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/cell_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/cell_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/gnb_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/gnb_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/location_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_report_received.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/path_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/path_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/qo_s_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/qos_monitoring_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/reporting_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/snssai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/u_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/ue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/ue_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/ue_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/usage_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/user_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/user_plane_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/user_plane_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/user_plane_notification_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/user_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-14 20:09:05.000000 evolved5g-1.0.6/evolved5g/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:09:47.681366 evolved5g-1.0.6/evolved5g.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-14 20:09:47.000000 evolved5g-1.0.6/evolved5g.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-14 20:09:47.000000 evolved5g-1.0.6/evolved5g.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:09:47.000000 evolved5g-1.0.6/evolved5g.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 20:09:47.000000 evolved5g-1.0.6/evolved5g.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:09:43.000000 evolved5g-1.0.6/evolved5g.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 20:09:47.000000 evolved5g-1.0.6/evolved5g.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 20:09:47.000000 evolved5g-1.0.6/evolved5g.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 20:09:05.000000 evolved5g-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 20:09:47.693367 evolved5g-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-14 20:09:05.000000 evolved5g-1.0.6/setup.py
```

### Comparing `evolved5g-1.0.5/CONTRIBUTING.rst` & `evolved5g-1.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/HISTORY.rst` & `evolved5g-1.0.6/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 =======
 History
 =======
 
 -------------------
+1.0.6 (2023-06-14)
+-------------------
+
+* The CLI command run-verification-tests now required three inputs (capif registration file, certificates folder and verification file) to launch NEF and TSN verification pipelines.
+* CAPIFProviderConnector has a new method offboard_and_deregister_netapp() that allows a network app to be offboarded and deregistered from CAPIF.
+* The SDK classes LocationSubscriber,ConnectionMonitor,QosAwareness don't accept the parameter 'nef_bearer_access_token' any more.
+* The CLI method register_and_onboard_to_capif now accepts a second parameter --environment that takes values "production" or "development".
+If this parameter is set to production then validation tests are running in the background, just after the registration and onboarding of the network app finishes.
+
+-------------------
 1.0.5 (2023-05-24)
 -------------------
 * Bug fix on CAPIFProviderConnector. When storing the capif_cert_server.pem the port was hardcoded.
 * Improvement on verification pipelines. Required user and password.
 * TSN verification pipeline added.
 * Validation pipeline included.
- 
+
 -------------------
 1.0.4 (2023-04-27)
 -------------------
 * Bug fix on ServiceDiscoverer: When creating the security context we now pass OAUTH as prefSecurityMethod
 
 -------------------
 1.0.3 (2023-04-25)
```

### Comparing `evolved5g-1.0.5/LICENSE` & `evolved5g-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/PKG-INFO` & `evolved5g-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.5
+Version: 1.0.6
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,21 +54,31 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.6 (2023-06-14)
+        -------------------
+        
+        * The CLI command run-verification-tests now required three inputs (capif registration file, certificates folder and verification file) to launch NEF and TSN verification pipelines.
+        * CAPIFProviderConnector has a new method offboard_and_deregister_netapp() that allows a network app to be offboarded and deregistered from CAPIF.
+        * The SDK classes LocationSubscriber,ConnectionMonitor,QosAwareness don't accept the parameter 'nef_bearer_access_token' any more.
+        * The CLI method register_and_onboard_to_capif now accepts a second parameter --environment that takes values "production" or "development".
+        If this parameter is set to production then validation tests are running in the background, just after the registration and onboarding of the network app finishes.
+        
+        -------------------
         1.0.5 (2023-05-24)
         -------------------
         * Bug fix on CAPIFProviderConnector. When storing the capif_cert_server.pem the port was hardcoded.
         * Improvement on verification pipelines. Required user and password.
         * TSN verification pipeline added.
         * Validation pipeline included.
-         
+        
         -------------------
         1.0.4 (2023-04-27)
         -------------------
         * Bug fix on ServiceDiscoverer: When creating the security context we now pass OAUTH as prefSecurityMethod
         
         -------------------
         1.0.3 (2023-04-25)
```

### Comparing `evolved5g-1.0.5/README.rst` & `evolved5g-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/Makefile` & `evolved5g-1.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/make.bat` & `evolved5g-1.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/cli.rst` & `evolved5g-1.0.6/docs/source/cli.rst`

 * *Files 9% similar despite different names*

```diff
@@ -56,19 +56,21 @@
 
 Now, you can execute ``evolved5g generate --config-file <path-to-your-config.yaml>`` providing the path of your yaml file.
 
 .. only:: html
 
    .. figure:: images/generate.gif
 
-If you access GitHub once you have seen that output in your terminal, you will see that the repository has been successfully created:
+Then the repository is created in your local computer as well as remotely in GitHub.
 
-   .. image:: images/repo_creation.png
+   .. figure:: images/netapp_creation.gif
 
-It will create a specific branch (evolved5g) which will be used by the CI/CD for verification purposes. A dummy example will be created in both branches (master and evolved5g) which allow to directly run a pipeline using such branch. You will see a Dockerfile and inside the src folder a dummy html file as an example. Below can see the file structure created.
+If you go to https://github.com/EVOLVED-5G you will see that the repository has been successfully created:
 
-   .. image:: images/repo_structure.png
+   .. image:: images/repo_creation.png
 
+It will create a specific branch (evolved5g) which will be used by the CI/CD for verification and validation purposes. An example is provided in master branch. You will see the src folder with a docker compose and a script (run.sh) to launch the Network App.
+It is important to remind that in order to have a fully functional example, it is mandatory to have NEF and CAPIF already up and running in your machine/container. Below can see the file structure created.
 
-   .. image:: images/dummy_html_example.png
+   .. image:: images/repo_structure.png
 
-When the repository is created you will be at branch evolved5g, so the push must be done there, in case you want to work with master (branch) you have to execute git checkout master and then do the push ``git push -u origin master``, to know in which branch you are, just execute git branch.
+   .. figure:: images/netapp_repo.gif
```

### Comparing `evolved5g-1.0.5/docs/source/conf.py` & `evolved5g-1.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/dummy_html_example.png` & `evolved5g-1.0.6/docs/source/images/dummy_html_example.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/generate_execution.png` & `evolved5g-1.0.6/docs/source/images/generate_execution.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/ssh_gpg.png` & `evolved5g-1.0.6/docs/source/images/ssh_gpg.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/ssh_key.png` & `evolved5g-1.0.6/docs/source/images/ssh_key.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/ssh_key_button.png` & `evolved5g-1.0.6/docs/source/images/ssh_key_button.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/token1.png` & `evolved5g-1.0.6/docs/source/images/token1.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/token2.png` & `evolved5g-1.0.6/docs/source/images/token2.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/images/token3.png` & `evolved5g-1.0.6/docs/source/images/token3.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/index.rst` & `evolved5g-1.0.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/information.rst` & `evolved5g-1.0.6/docs/source/information.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/installation.rst` & `evolved5g-1.0.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/docs/source/pre_requisites.rst` & `evolved5g-1.0.6/docs/source/pre_requisites.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/cli.py` & `evolved5g-1.0.6/evolved5g/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,49 +11,67 @@
     """Console interface for EVOLVED-5G H2020 project"""
     ctx.ensure_object(dict)
     ctx.obj["helper"] = CLI_helper()
 
 
 @cli.command()
 @click.option(
-    "--config-file", type=str, help="Provide User config location for custom package"
+    "--config-file", required=True, type=str, help="Provide User config location for custom package"
 )
 @click.pass_context
 def generate(ctx, config_file):
     """Generate EVOLVED-5G compliant NetApp from template"""
     ctx.obj["helper"].generate(config_file)
 
 
 @cli.command()
 @click.option(
     "--mode",
     type=click.Choice(
-        ["build", "deploy", "destroy", "capif_nef", "capif_tsn", "code_analysis", "security_scan", "validation"],
+        ["build", "deploy", "destroy", "capif_nef", "capif_tsn", "code_analysis", "security_scan"],
         case_sensitive=False,
     ),
+
 )
-@click.option("--repo", type=str, help="Enter repo name")
-@click.option("--user", type=str, help="Enter your username for pipelines")
-@click.option("--passwd", type=str, help="Enter repo password for pipelines")
+@click.option("--repo", required=True, type=str, help="Enter repo name")
+@click.option("--user", required=True, type=str, help="Enter your username for pipelines")
+@click.option("--passwd", required=True, type=str, help="Enter repo password for pipelines")
+@click.option("--capifpath", required=False, default=None, show_default=True, type=str, help="(Only for NEF and CAPIF) Path where to find the CAPIF registration configuration file (json)")
+@click.option("--certpath", required=False, default=None, show_default=True, type=str, help="(Only for NEF and CAPIF) Folder path where to store the certification files")
+@click.option("--verfpath", required=False, default=None, show_default=True, type=str, help="(Only for NEF and CAPIF) Path for the python file to verify")
+@click.option("--version", required=False, default=4.0, show_default=True, type=str, help="Network App version")
 
 @click.pass_context
-def run_verification_tests(ctx, mode, repo, user, passwd):
+def run_verification_tests(ctx, mode, repo, user, passwd, capifpath, certpath, verfpath, version):
     """Launch different verification tests"""
-    ctx.obj["helper"].run_verification_tests(mode, repo, user, passwd)
-
+    ctx.obj["helper"].run_verification_tests(mode, repo, user, passwd, capifpath, certpath, verfpath, version)
 
 @cli.command()
-@click.option("--id", type=int, help="Enter pipeline id")
-@click.option("--user", type=str, help="Enter your username for pipelines")
-@click.option("--passwd", type=str, help="Enter repo password for pipelines")
+@click.option("--id", required=True, type=int, help="Enter pipeline id")
+@click.option("--user", required=True, type=str, help="Enter your username for pipelines")
+@click.option("--passwd", required=True, type=str, help="Enter repo password for pipelines")
+
 @click.pass_context
 def check_job(ctx, id, user, passwd):
     """Check the status of a pipeline"""
     ctx.obj["helper"].check_job(id, user, passwd)
 
+@cli.command()
+@click.option("--repo", required=True, type=str, help="Enter repo name")
+@click.option("--user", required=True, type=str, help="Enter your username for pipelines")
+@click.option("--passwd", required=True, type=str, help="Enter repo password for pipelines")
+@click.option("--environment", required=False, show_default=True, default="openshift", type=str, help="Enter the environment to deploy the NetApp (openshift, kubernetes-athens, kubernetes-uma)")
+@click.option("--deploy", required=False, type=str, help="Network App deployment name")
+@click.option("--email", required=False, default=False, type=str, help="Developer email to receive the report")
+@click.option("--version", required=False, default=4.0, show_default=True, type=str, help="Network App version")
+
+@click.pass_context
+def validation(ctx, repo, user, passwd, environment, deploy, email, version):
+    """Launch the validation tests"""
+    ctx.obj["helper"].validation(repo, user, passwd, environment, deploy, email, version)
 
 @cli.command()
 @click.option(
     "--config_file_full_path",
     type=str,
     help="""The configuration file used to register and onboard the NetApp to CAPIF
                 --folder_to_store_certificates: The folder where certificates and authorization files will be stored
```

### Comparing `evolved5g-1.0.5/evolved5g/cli_helper.py` & `evolved5g-1.0.6/evolved5g/cli_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def generate(self, config_file):
         """Generate EVOLVED-5G compliant NetApp from template"""
         location = "gh:EVOLVED-5G/NetApp-template"
         directory = "template"
         cookiecutter_generate(location, config_file, directory, no_input=True)
 
-    def run_verification_tests(self, mode, repo, user, passwd):
+    def run_verification_tests(self, mode, repo, user, passwd, capifpath, certpath, verfpath, version):
         """Run the build pipeline for the EVOLVED-5G NetApp"""
 
         if repo is None:
             echo(
                 "'None' value provided.\nPlease enter the correct command: evolved5g run-verification-tests --mode "
                 "build --repo REPOSITORY_NAME "
             )
@@ -51,81 +51,85 @@
                         }
 
                         data = (
                                 '{ "action": "'
                                 + mode
                                 + '", "parameters": { "GIT_NETAPP_URL": "https://github.com/EVOLVED-5G/'
                                 + repo
+                                + '", "VERSION_NETAPP": "'
+                                + version
                                 + '","GIT_NETAPP_BRANCH": "'
                                 + self.netapp_branch
                                 + '"} }'
                         )
 
                         resp = requests.post(
                             self.url_curl, headers=self.header, data=data
                         )
 
-                        if (len(resp.json()) > 3): #List
-                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has been finished.")
-                        else: #It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']} and the actual status is: {resp.json()[0]['status']}.")
+                        if (resp.json()['status'] == 403):
+                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has finished.")
+                        else:
+                            echo(
+                                f"Your pipeline ID is: {resp.json()['job_id']} and the actual status is: {resp.json()['status']}.")
 
                     elif mode == "deploy":
                         self.header = {
                             "content-Type": "application/json",
                             "accept": "application/json",
                             "username": user,
                             "password": passwd,
                         }
 
+                        foldernetapp = repo.lower()
                         data = (
                                 '{ "action": "'
                                 + mode
-                                + '", "parameters": { "GIT_NETAPP_URL": "https://github.com/EVOLVED-5G/'
+                                + '", "parameters": { "FOLDER_NETWORK_APP": "'
+                                + foldernetapp
+                                + '","RELEASE_NAME": "'
                                 + repo
-                                + '","GIT_NETAPP_BRANCH": "'
-                                + self.netapp_branch
                                 + '"} }'
                         )
 
                         resp = requests.post(
                             self.url_curl, headers=self.header, data=data
                         )
-
-                        if (len(resp.json()) > 3): #List
-                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has been finished.")
-                        else: #It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']} and the actual status is: {resp.json()[0]['status']}.")
+                        
+                        if (resp.json()['status'] == 403):
+                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has finished.")
+                        else:
+                            echo(
+                                f"Your pipeline ID is: {resp.json()['job_id']} and the actual status is: {resp.json()['status']}.")
 
                     elif mode == "destroy":
                         self.header = {
                             "content-Type": "application/json",
                             "accept": "application/json",
                             "username": user,
                             "password": passwd,
                         }
 
                         data = (
                                 '{ "action": "'
                                 + mode
-                                + '", "parameters": { "GIT_NETAPP_URL": "https://github.com/EVOLVED-5G/'
+                                + '", "parameters": { "RELEASE_NAME": "'
                                 + repo
-                                + '","GIT_NETAPP_BRANCH": "'
-                                + self.netapp_branch
                                 + '"} }'
                         )
 
                         resp = requests.post(
                             self.url_curl, headers=self.header, data=data
                         )
 
-                        if (len(resp.json()) > 3): #List
-                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has been finished.")
-                        else: #It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']} and the actual status is: {resp.json()[0]['status']}.")
+                        if (resp.json()['status'] == 403):
+                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has finished.")
+                        else:
+                            echo(
+                                f"Your pipeline ID is: {resp.json()['job_id']} and the actual status is: {resp.json()['status']}.")
 
 
                     elif mode == "code_analysis":
                         self.header = {
                             "content-Type": "application/json",
                             "accept": "application/json",
                             "username": user,
@@ -142,18 +146,18 @@
                                 + '"} }'
                         )
 
                         resp = requests.post(
                             self.url_curl, headers=self.header, data=data
                         )
 
-                        if (len(resp.json()) > 3): #List
-                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has been finished.")
-                        else: #It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']} and the actual status is: {resp.json()[0]['status']}.")
+                        if (resp.json()['status'] == 403):
+                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has finished.")
+                        else:
+                            echo(f"Your pipeline ID is: {resp.json()['job_id']} and the actual status is: {resp.json()['status']}.")
 
 
                     elif mode == "security_scan":
                         self.header = {
                             "content-Type": "application/json",
                             "accept": "application/json",
                             "username": user,
@@ -168,140 +172,205 @@
                                 + self.netapp_branch
                                 + '"} }'
                         )
                         resp = requests.post(
                             self.url_curl, headers=self.header, data=data
                         )
 
-                        if (len(resp.json()) > 3): #List
+                        if (len(resp.json()) > 3):  # List
                             echo(f"{resp.json()['detail']} Please wait until your previous pipeline has been finished.")
-                        else: #It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']}, {resp.json()[1]['job_id']} and {resp.json()[2]['job_id']} and the actual status for each is: {resp.json()[0]['status']}, "
-                                 f"{resp.json()[1]['status']} and {resp.json()[2]['status']}.")
+                        else:  # It is a List treated as Dictionary
+                            echo(
+                                f"Your pipeline ID is: {resp.json()[0]['job_id']}, {resp.json()[1]['job_id']} and {resp.json()[2]['job_id']} and the actual status for each is: {resp.json()[0]['status']}, "
+                                f"{resp.json()[1]['status']} and {resp.json()[2]['status']}.")
 
                     elif mode == "capif_nef":
-                        self.header = {
-                            "content-Type": "application/json",
-                            "accept": "application/json",
-                            "username": user,
-                            "password": passwd,
-                        }
-                        data = (
-                                '{ "action": "'
-                                + mode
-                                + '", "parameters": { "GIT_NETAPP_URL": "https://github.com/EVOLVED-5G/'
-                                + repo
-                                + '","GIT_NETAPP_BRANCH": "'
-                                + self.netapp_branch
-                                + '"} }'
-                        )
-                        resp = requests.post(
-                            self.url_curl, headers=self.header, data=data
-                        )
 
-                        if (len(resp.json()) > 3): #List
-                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has been finished.")
-                        else: #It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']} and the actual status is: {resp.json()[0]['status']}.")
+                        if (not capifpath or  not certpath or not verfpath):
+                            print (f"Please provide all the files and folder required to launch the NEF pipeline.\n"
+                                   f"You must provide the path for capif registration file, the path where to store the certification files"
+                                   f"and the path of the file to be verified. You have actually provided:\n"
+                                   f"Path for CAPIF registration file (json): {capifpath}\nPath for certification files: {certpath}\nPath for verification file: {verfpath}")
+                        else:
+                            self.header = {
+                                "content-Type": "application/json",
+                                "accept": "application/json",
+                                "username": user,
+                                "password": passwd,
+                            }
+
+                            data = (
+                                    '{ "action": "'
+                                    + mode
+                                    + '", "parameters": { "NetApp_repo": "'
+                                    + repo
+                                    + '","CAPIF_REGISTRATION_CONFIG_PATH": "'
+                                    + capifpath
+                                    + '","CERTIFICATES_FOLDER_PATH": "'
+                                    + certpath
+                                    + '","VERIFICATION_FILE": "'
+                                    + verfpath
+                                    + '","NetApp_repo_branch": "'
+                                    + self.netapp_branch
+                                    + '"} }'
+                            )
+
+                            resp = requests.post(
+                                self.url_curl, headers=self.header, data=data
+                            )
+
+                            if (resp.json()['status'] == 403):
+                                echo(f"{resp.json()['detail']} Please wait until your previous pipeline has finished.")
+                            else:
+                                echo(
+                                    f"Your pipeline ID is: {resp.json()['job_id']} and the actual status is: {resp.json()['status']}.")
 
                     elif mode == "capif_tsn":
-                        self.header = {
-                            "content-Type": "application/json",
-                            "accept": "application/json",
-                            "username": user,
-                            "password": passwd,
-                        }
-                        data = (
-                                '{ "action": "'
-                                + mode
-                                + '", "parameters": { "GIT_NETAPP_URL": "https://github.com/EVOLVED-5G/'
-                                + repo
-                                + '","GIT_NETAPP_BRANCH": "'
-                                + self.netapp_branch
-                                + '"} }'
-                        )
-                        echo (data)
-                        resp = requests.post(
-                            self.url_curl, headers=self.header, data=data
+                        if (not capifpath or  not certpath or not verfpath):
+                            print (f"Please provide all the files and folder required to launch the NEF pipeline.\n"
+                                   f"You must provide the path for capif registration file, the path where to store the certification files"
+                                   f"and the path of the file to be verified. You have actually provided:\n"
+                                   f"Path for CAPIF registration file (json): {capifpath}\nPath for certification files: {certpath}\nPath for verification file: {verfpath}")
+                        else:
+                            self.header = {
+                                "content-Type": "application/json",
+                                "accept": "application/json",
+                                "username": user,
+                                "password": passwd,
+                            }
+
+                            data = (
+                                    '{ "action": "'
+                                    + mode
+                                    + '", "parameters": { "NetApp_repo": "'
+                                    + repo
+                                    + '","CAPIF_REGISTRATION_CONFIG_PATH": "'
+                                    + capifpath
+                                    + '","CERTIFICATES_FOLDER_PATH": "'
+                                    + certpath
+                                    + '","VERIFICATION_FILE": "'
+                                    + verfpath
+                                    + '","NetApp_repo_branch": "'
+                                    + self.netapp_branch
+                                    + '"} }'
+                            )
+
+                            #echo (data)
+
+                            resp = requests.post(
+                                self.url_curl, headers=self.header, data=data
+                            )
+                            print (resp.json())
+
+                            if (resp.json()['status'] == 403):
+                                echo(f"{resp.json()['detail']} Please wait until your previous pipeline has finished.")
+                            else:
+                                echo(
+                                    f"Your pipeline ID is: {resp.json()['job_id']} and the actual status is: {resp.json()['status']}.")
+                            
+                    else:
+                        echo(
+                            f"The {mode} you have chosen does not exist, please check the modes and try again"
                         )
 
-                        if (len(resp.json()) > 3): #List
-                            echo(f"{resp.json()['detail']} Please wait until your previous pipeline has been finished.")
-                        else: #It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']} and the actual status is: {resp.json()[0]['status']}.")
+                except ValueError as e:
+                    echo(
+                        "Please enter the correct command: evolved5g run-verification-tests --mode build --repo <your_REPOSITORY_NAME>, --user <yourUSERNAME>, --passwd <yourPASSWORD>"
+                    )
+            else:
+                echo(
+                    f"The {repo} repository you have chosen does not exist, please check the name you typed and try again."
+                )
 
-                    elif mode == "validation":
+    def validation(self, repo, user, passwd, environment, deploy, email, version):
+        """Run the build pipeline for the EVOLVED-5G NetApp"""
 
-                        self.header = {
-                            "content-Type": "application/json",
-                            "accept": "application/json",
-                            "username": user,
-                            "password": passwd,
-                        }
+        if deploy is None: deploy = repo
 
-                        data = (
-                                '{ "action": "'
-                                + mode
-                                + '", "parameters": { "GIT_NETAPP_URL": "https://github.com/EVOLVED-5G/'
-                                + repo
-                                + '","GIT_NETAPP_BRANCH": "'
-                                + self.netapp_branch
-                                + '"} }'
-                        )
+        if repo is None:
+            echo(
+                "'None' value provided.\nPlease enter the correct command: evolved5g run-verification-tests --repo REPOSITORY_NAME ")
+        else:
+            r = requests.get(f"{self.repository}/{repo}")
+            repo_exist = r.json()
 
-                        resp = requests.post(
-                            self.url_curl, headers=self.header, data=data
-                        )
+            if "message" not in repo_exist:
+                try:
+                    self.header = {
+                        "content-Type": "application/json",
+                        "accept": "application/json",
+                        "username": user,
+                        "password": passwd,
+                    }
+
+                    data = (
+                            '{ "action": "validation", "parameters": { "GIT_NETAPP_URL": "https://github.com/EVOLVED-5G/'
+                            + repo
+                            + '", "ENVIRONMENT": "'
+                            + environment
+                            + '", "SEND_DEV_EMAIL": "'
+                            + email
+                            + '", "VERSION_NETAPP": "'
+                            + version
+                            + '", "DEPLOY_NAME": "'
+                            + deploy
+                            + '","GIT_NETAPP_BRANCH": "'
+                            + self.netapp_branch
+                            + '"} }'
+                    )
 
-                        if (len(resp.json()) > 3): #List
-                            echo(f"{resp.json()['detail']}. Please wait until you received your result by email.")
-                        else:  # It is a List treated as Dictionary
-                            echo(f"Your pipeline ID is: {resp.json()[0]['job_id']} and the actual status is: {resp.json()[0]['status']}.")
+                    #print(data)
 
+                    resp = requests.post(
+                        self.url_curl, headers=self.header, data=data
+                    )
+
+                    #echo(f"{resp.json()}")
+
+                    if (resp.json()['status'] == 403):
+                        echo(f"{resp.json()['detail']} Please wait until your previous pipeline has finished.")
                     else:
-                        echo(
-                            f"The {mode} you have chosen does not exist, please check the modes and try again"
-                        )
+                        echo(f"Your pipeline ID is: {resp.json()['job_id']} and the actual status is: {resp.json()['status']}.")
+
 
                 except ValueError as e:
                     echo(
-                        "Please enter the correct command: evolved5g run-verification-tests --mode build --repo <your_REPOSITORY_NAME>, --user <yourUSERNAME>, --passwd <yourPASSWORD>"
-                    )
+                        "Please enter the correct command: evolved5g run-verification-tests --mode build --repo <your_REPOSITORY_NAME>, --user <yourUSERNAME>, --passwd <yourPASSWORD>")
             else:
                 echo(
-                    f"The {repo} repository you have chosen does not exist, please check the name you typed and try again."
-                )
+                    f"The {repo} repository you have chosen does not exist, please check the name you typed and try again.")
 
     def check_job(self, id, user, passwd):
 
         """Check the status of the pipeline for the EVOLVED-5G NetApp"""
 
         try:
             self.header = {
                 "content-Type": "application/json",
                 "accept": "application/json",
                 "username": user,
                 "password": passwd,
             }
             resp = requests.get(f"{self.url_curl_job}/{id}/status", headers=self.header)
             result = resp.json()
-            echo (result["status"])
 
-            '''if result["status"] == "QUEUED":
-                echo(result)
+            if result["status"] == "QUEUED":
+                # echo(result)
+                echo(f"Your pipeline {id} status is {result['status']}, please {result['status'].split(',')[1]}")
             else:
-                console = json.dumps(result["console_log"]).split("\\n")
+                console = json.dumps(result["log"]).split("\\n")
 
                 for element in console:
                     if "] { (" in element:
                         echo(element)
                     elif "[Pipeline]" not in element:
                         echo(element)
                     elif "] stage" in element:
-                        echo(element)'''
+                        echo(element)
+                echo(result["status"])
 
         except ValueError as e:
             echo("Please add the ID: evolved5g check-job --id <yourID>, --user <yourUSERNAME>, --passwd <yourPASSWORD>")
 
     def register_and_onboard_to_capif(self, config_file_full_path: str) -> None:
         with open(config_file_full_path, "r") as openfile:
             config = json.load(openfile)
@@ -380,11 +449,11 @@
         profile = matched_profiles[0]
         clearance_token = tsn.apply_tsn_profile_to_netapp(netapp_tsn_id, profile)
         echo(
             f'The TSN profile "{profile_name}" has been successfully applied to your netapp "{netapp_name}".'
             f'\nStore the token "{clearance_token}" to clear the profile if you wish in the future.'
         )
 
-    def test_capif_and_nef_published_to_capif_endpoints(self, config_file_full_path: str)->None:
+    def test_capif_and_nef_published_to_capif_endpoints(self, config_file_full_path: str) -> None:
         test_capif_and_nef_published_to_capif_endpoints(config_file_full_path)
```

### Comparing `evolved5g-1.0.5/evolved5g/nef_and_tsn_api_service_tests.py` & `evolved5g-1.0.6/evolved5g/nef_and_tsn_api_service_validation_pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,70 @@
 import json
 import json.decoder
-from evolved5g.sdk import TSNManager, LocationSubscriber, ConnectionMonitor, QosAwareness
+from evolved5g.sdk import TSNManager, LocationSubscriber, ConnectionMonitor, QosAwareness, ServiceDiscoverer
 from evolved5g.swagger_client.rest import ApiException
 from evolved5g import swagger_client
 from evolved5g.swagger_client import LoginApi, User, UsageThreshold
 from evolved5g.swagger_client.models import Token
 import datetime
 
 
-def test_capif_and_nef_published_to_capif_endpoints(config_file_full_path: str) -> None:
-    with open(config_file_full_path, "r") as openfile:
-        config = json.load(openfile)
-
-    test_nef_service_api(config)
-    test_tsn_service_api(config)
-
-
-def test_nef_service_api(config):
+def validate_all_endpoints_returned_by_service_discoverer(config_file_full_path: str) -> bool:
     """
-    Test
-    :param config:
-    :return:
+    This method finds all the released APIs in CAPIF (via ServiceDiscovery) and performs tests to make sure that they work as expected
+    :param config_file_full_path:
+    :return: True if the endpoints work as expected. Else an exception is raised
     """
-    __test_location_subscriber(config)
-    __test_connection_monitor(config)
-    __test_qos_awereness(config)
-
+    with open(config_file_full_path, "r") as openfile:
+        config = json.load(openfile)
 
-def test_tsn_service_api(config):
-    __test_tsn_manager(config)
+    service_discoverer = ServiceDiscoverer(folder_path_for_certificates_and_api_key=config["folder_to_store_certificates"],
+                                           capif_host=config["capif_host"],
+                                           capif_https_port=config["capif_https_port"]
+                                           )
+    service_apis = service_discoverer.discover_service_apis()
+
+    # We iterate to all of the available published services.
+    # Notice that if a new api is published and we dont have tests for it, an exception is raised
+    for api_description in service_apis["serviceAPIDescriptions"]:
+        print("Starting testing endpoints for ApiName: " + api_description["apiName"] )
+        host_info = api_description["aefProfiles"][0]['interfaceDescriptions'][0]
+        if api_description["apiName"] == "/nef/api/v1/3gpp-monitoring-event/":
+
+            # nef_url=  "https://localhost:4443"
+            nef_url = "https://{host}:{port}".format(host=host_info["ipv4Addr"], port=host_info["port"])
+            __test_location_subscriber(config,nef_url)
+            __test_connection_monitor(config,nef_url)
+        elif api_description["apiName"] == "/nef/api/v1/3gpp-as-session-with-qos/":
+            # nef_url=  "https://localhost:4443"
+            nef_url = "https://{host}:{port}".format(host=host_info["ipv4Addr"], port=host_info["port"])
+            __test_qos_awereness(config,nef_url)
+        elif api_description["apiName"] == "/tsn/api/":
+            #tsn_host = "localhost"  # TSN server hostname
+            #tsn_port = 8899  # TSN server port
+            __test_tsn_manager(config,host_info["ipv4Addr"],host_info["port"])
+        else:
+            raise NotImplementedError("Could not find Validation tests for ApiName" + api_description["apiName"])
 
+    print("All endpoints work as expected")
+    return True
 
-def __test_location_subscriber(config) -> None:
+def __test_location_subscriber(config,url_of_the_nef_emulator) -> None:
     """
     Tests the NEF api name /nef/api/v1/3gpp-monitoring-event/ with dummy data
     :param config:
     """
 
     # Create a subscription, that will notify us 1000 times, for the next 1 day starting from now
     expire_time = (datetime.datetime.utcnow() + datetime.timedelta(days=1)).isoformat() + "Z"
     netapp_id = "myNetapp"
-    token = get_token_for_nef_emulator()
-    location_subscriber = LocationSubscriber(nef_url=get_url_of_the_nef_emulator(),
-                                             nef_bearer_access_token=token.access_token,
-                                             folder_path_for_certificates_and_capif_api_key=get_folder_path_for_netapp_certificates_and_capif_api_key(),
-                                             capif_host=get_capif_host(),
-                                             capif_https_port=get_capif_https_port())
+    location_subscriber = LocationSubscriber(nef_url=url_of_the_nef_emulator,
+                                             folder_path_for_certificates_and_capif_api_key=config["folder_to_store_certificates"],
+                                             capif_host=config["capif_host"],
+                                             capif_https_port=config["capif_https_port"])
     # The following external identifier was copy pasted by the NEF emulator. Go to the Map and click on a User icon. There you can retrieve the id
     external_id = "10003@domain.com"
 
     subscription = location_subscriber.create_subscription(
         netapp_id=netapp_id,
         external_id=external_id,
         notification_destination="http://172.17.0.1:5000/monitoring/callback",
@@ -71,29 +86,27 @@
         if ex.status == 404:
             print("No active transcriptions found")
         else:
             # something else happened, test failed! Re-throw the exception
             raise
 
 
-def __test_connection_monitor(config):
+def __test_connection_monitor(config,url_of_the_nef_emulator):
     """
      Tests the NEF api name /nef/api/v1/3gpp-monitoring-event/ with dummy data
      :param config:
    """
 
     # Create a subscription, that will notify us 1000 times, for the next 1 day starting from now
     expire_time = (datetime.datetime.utcnow() + datetime.timedelta(days=1)).isoformat() + "Z"
     netapp_id = "myNetapp"
-    token = get_token_for_nef_emulator()
-    connection_monitor = ConnectionMonitor(nef_url=get_url_of_the_nef_emulator(),
-                                           nef_bearer_access_token=token.access_token,
-                                           folder_path_for_certificates_and_capif_api_key=get_folder_path_for_netapp_certificates_and_capif_api_key(),
-                                           capif_host=get_capif_host(),
-                                           capif_https_port=get_capif_https_port())
+    connection_monitor = ConnectionMonitor(nef_url=url_of_the_nef_emulator,
+                                           folder_path_for_certificates_and_capif_api_key=config["folder_to_store_certificates"],
+                                           capif_host=config["capif_host"],
+                                           capif_https_port=config["capif_https_port"])
     # The following external identifier was copy pasted by the NEF emulator. Go to the Map and click on a User icon. There you can retrieve the id
     external_id = "10003@domain.com"
 
     subscription_when_not_connected = connection_monitor.create_subscription(
         netapp_id=netapp_id,
         external_id=external_id,
         notification_destination="http://172.17.0.1:5000/monitoring/callback",
@@ -115,27 +128,25 @@
     except ApiException as ex:
         if ex.status == 404:
             print("No active transcriptions found")
         else:  # something else happened, re-throw the exception
             raise
 
 
-def __test_qos_awereness(config):
+def __test_qos_awereness(config,url_of_the_nef_emulator):
     """
      Tests the NEF api name  /nef/api/v1/3gpp-as-session-with-qos/  with dummy data
      :param config:
    """
     netapp_id = "myNetapp"
 
-    token = get_token_for_nef_emulator()
-    qos_awereness = QosAwareness(nef_url=get_url_of_the_nef_emulator(),
-                                 nef_bearer_access_token=token.access_token,
-                                 folder_path_for_certificates_and_capif_api_key=get_folder_path_for_netapp_certificates_and_capif_api_key(),
-                                 capif_host=get_capif_host(),
-                                 capif_https_port=get_capif_https_port())
+    qos_awereness = QosAwareness(nef_url=url_of_the_nef_emulator,
+                                 folder_path_for_certificates_and_capif_api_key=config["folder_to_store_certificates"],
+                                 capif_host=config["capif_host"],
+                                 capif_https_port=config["capif_https_port"])
     # The following external identifier was copy pasted by the NEF emulator.
     # Go to the Map and hover over a User icon.There you can retrieve the id address.
     # Notice that the NEF emulator is able to establish a guaranteed bit rate only if one and only one user is connected to a shell
     # This is done in purpose in the NEF emulator, to allow testing the lost of guaranteed connectivity to your code
     # in the NEF if a user "10.0.0.3" is connected to Cell only by her self (she is the only connection within range)
     # the NEF guarantees the connection. If another user walks by, within the same Cell range then the connection is no
     # more guaranteed and a callback notification will be retrieved.
@@ -193,27 +204,26 @@
     except ApiException as ex:
         if ex.status == 404:
             print("No active transcriptions found")
         else:  # something else happened, re-throw the exception
             raise
 
 
-def __test_tsn_manager(config):
+def __test_tsn_manager(config,tsn_host,tsn_port):
     """
       Tests the TSN api name  with dummy data
      :param config:
    """
-    tsn_host = "localhost"  # TSN server hostname
-    tsn_port = 8899  # TSN server port
+
 
     netapp_name = "MyNetapp1"  # The name of our NetApp
     tsn = TSNManager(  # Initialization of the TNSManager
-        folder_path_for_certificates_and_capif_api_key=get_folder_path_for_netapp_certificates_and_capif_api_key(),
-        capif_host=get_capif_host(),
-        capif_https_port=get_capif_https_port(),
+        folder_path_for_certificates_and_capif_api_key=config["folder_to_store_certificates"],
+        capif_host=config["capif_host"],
+        capif_https_port=config["capif_https_port"],
         https=False,
         tsn_host=tsn_host,
         tsn_port=tsn_port
     )
 
     # Retrieve information on all the available TSN profiles
     profiles = tsn.get_tsn_profiles()
@@ -235,52 +245,13 @@
     )
 
     tsn.clear_profile_for_tsn_netapp_identifier(tsn_netapp_identifier, clearance_token)
 
     # If we reached this point with no exceptions, then we tested all the endpoints of TSN
 
 
-def get_token_for_nef_emulator() -> Token:
-    username = "admin@my-email.com"
-    password = "pass"
-    # User name and pass matches are set in the .env of the docker of NEF_EMULATOR. See
-    # https://github.com/EVOLVED-5G/NEF_emulator
-    configuration = swagger_client.Configuration()
-    # The host of the 5G API (emulator)
-    configuration.host = get_url_of_the_nef_emulator()
-    configuration.verify_ssl = False
-    api_client = swagger_client.ApiClient(configuration=configuration)
-    api_client.select_header_content_type(["application/x-www-form-urlencoded"])
-    api = LoginApi(api_client)
-    token = api.login_access_token_api_v1_login_access_token_post("", username, password, "", "", "")
-    return token
 
 
-def get_url_of_the_nef_emulator() -> str:
-    return "https://localhost:4443"
+if __name__ == "__main__":
+    config_file_path= "/home/alex/Projects/maggioli/evolved-5g/SDK-CLI/examples/netapp_capif_config/netapp_capif_connector_config_file.json"
+    validate_all_endpoints_returned_by_service_discoverer(config_file_path)
 
-
-def get_folder_path_for_netapp_certificates_and_capif_api_key() -> str:
-    """
-    This is the folder that is provided when you registered the NetApp to CAPIF.
-    It contains the certificates and the api.key needed to communicate with the CAPIF server.
-    Make sure to change this path name to match your environment!
-    :return:
-    """
-    return "/home/alex/Projects/test_certificate_folder"
-
-
-def get_capif_host() -> str:
-    """
-    When running CAPIF via docker (by running ./run.sh) you should have at your /etc/hosts the following record
-    127.0.0.1       capifcore
-    :return:
-    """
-    return "capifcore"
-
-
-def get_capif_https_port() -> int:
-    """
-    This is the default https port when running CAPIF via docker
-    :return:
-    """
-    return 443
```

### Comparing `evolved5g-1.0.5/evolved5g/sdk.py` & `evolved5g-1.0.6/evolved5g/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,39 +40,39 @@
 import warnings
 
 
 class MonitoringSubscriber(ABC):
     def __init__(
             self,
             host: str,
-            nef_bearer_access_token: str,
             folder_path_for_certificates_and_capif_api_key: str,
             capif_host: str,
             capif_https_port: int,
     ):
         configuration = swagger_client.Configuration()
         configuration.verify_ssl = False
         configuration.host = host
         service_discoverer = ServiceDiscoverer(folder_path_for_certificates_and_capif_api_key, capif_host,
                                                capif_https_port)
         api_name = "/nef/api/v1/3gpp-monitoring-event/"
         configuration.available_endpoints = {
             "MONITORING_SUBSCRIPTIONS": service_discoverer.retrieve_specific_resource_name(api_name,
-                                                                                           "MONITORING_SUBSCRIPTIONS"),
+                                                                                   "MONITORING_SUBSCRIPTIONS"),
             "MONITORING_SUBSCRIPTION_SINGLE": service_discoverer.retrieve_specific_resource_name(api_name,
-                                                                                                 "MONITORING_SUBSCRIPTION_SINGLE"),
+                                                                                     "MONITORING_SUBSCRIPTION_SINGLE"),
         }
         api_resource_description = service_discoverer.retrieve_api_description_by_name(api_name)
-        configuration.access_token = nef_bearer_access_token + "," + service_discoverer.get_access_token(api_name,
-                                                                                                         api_resource_description[
-                                                                                                             "apiId"],
-                                                                                                         api_resource_description[
-                                                                                                             "aefProfiles"][
-                                                                                                             0][
-                                                                                                             "aefId"])
+
+        configuration.access_token =  service_discoverer.get_access_token(api_name,
+                                                                         api_resource_description[
+                                                                             "apiId"],
+                                                                         api_resource_description[
+                                                                             "aefProfiles"][
+                                                                             0][
+                                                                             "aefId"])
         api_client = swagger_client.ApiClient(configuration=configuration)
         self.monitoring_event_api = MonitoringEventAPIApi(api_client)
         self.cell_api = CellsApi(api_client)
 
     def create_subscription_request(
             self,
             monitoring_type,
@@ -131,30 +131,28 @@
         )
 
 
 class LocationSubscriber(MonitoringSubscriber):
     def __init__(
             self,
             nef_url: str,
-            nef_bearer_access_token: str,
             folder_path_for_certificates_and_capif_api_key: str,
             capif_host: str,
             capif_https_port: int,
     ):
         """
         Initializes class LocationSubscriber.
         This SKD class allows you to track devices and retrieve updates about their location.
         You can create subscriptions where each one of them can be used to track a device.
         A notification is sent to a callback url you will provide, everytime the user device changes Cell
 
          :param str nef_url: The url of the 5G-API
         """
         super().__init__(
             nef_url,
-            nef_bearer_access_token,
             folder_path_for_certificates_and_capif_api_key,
             capif_host,
             capif_https_port,
         )
 
     def __get_monitoring_type(self):
         return "LOCATION_REPORTING"
@@ -274,15 +272,14 @@
 
         INFORM_WHEN_CONNECTED = 1
         INFORM_WHEN_NOT_CONNECTED = 2
 
     def __init__(
             self,
             nef_url: str,
-            nef_bearer_access_token: str,
             folder_path_for_certificates_and_capif_api_key: str,
             capif_host: str,
             capif_https_port: int,
     ):
         """
         Initializes class ConnectionMonitor.
         Consider a scenario where a NetApp wants to monitor 100 devices in the 5G Network.
@@ -296,15 +293,14 @@
         :param folder_path_for_certificates_and_capif_api_key: The folder that contains the NetApp certificates and
          CAPIF API Key. These are created  while registering and onboarding the NetApp to the CAPIF Server
         :param capif_host: The host of the CAPIF Server (ex. "capifcore")
         :param capif_https_port: The https_port of the  CAPIF Server
         """
         super().__init__(
             nef_url,
-            nef_bearer_access_token,
             folder_path_for_certificates_and_capif_api_key,
             capif_host,
             capif_https_port,
         )
 
     def __get_monitoring_type(self, monitoring_type: MonitoringType):
         if monitoring_type == self.MonitoringType.INFORM_WHEN_CONNECTED:
@@ -503,15 +499,14 @@
 
         def get_reporting_configuration(self):
             return self.repetition_period_in_seconds
 
     def __init__(
             self,
             nef_url: str,
-            nef_bearer_access_token: str,
             folder_path_for_certificates_and_capif_api_key: str,
             capif_host: str,
             capif_https_port: int,
     ):
         """
         Initializes class QosAwareness.
         This SKD class allows you to request QoS from a set of standardized values for better service experience.
@@ -541,15 +536,15 @@
                 api_name, "QOS_SUBSCRIPTIONS"
             ),
             "QOS_SUBSCRIPTION_SINGLE": service_discoverer.retrieve_specific_resource_name(
                 api_name, "QOS_SUBSCRIPTION_SINGLE"
             ),
         }
         api_resource_description = service_discoverer.retrieve_api_description_by_name(api_name)
-        configuration.access_token = nef_bearer_access_token + "," + service_discoverer.get_access_token(api_name,
+        configuration.access_token = service_discoverer.get_access_token(api_name,
                                                                                                          api_resource_description[
                                                                                                              "apiId"],
                                                                                                          api_resource_description[
                                                                                                              "aefProfiles"][
                                                                                                              0][
                                                                                                              "aefId"])
         api_client = swagger_client.ApiClient(configuration=configuration)
@@ -950,26 +945,27 @@
         self.csr_common_name = "invoker_" + csr_common_name
         self.csr_organizational_unit = csr_organizational_unit
         self.csr_organization = csr_organization
         self.crs_locality = crs_locality
         self.csr_state_or_province_name = csr_state_or_province_name
         self.csr_country_name = csr_country_name
         self.csr_email_address = csr_email_address
+        self.capif_api_details_filename = "capif_api_security_context_details.json"
 
     def __add_trailing_slash_to_url_if_missing(self, url):
         if url[len(url) - 1] != "/":
             url = url + "/"
         return url
 
     def register_and_onboard_netapp(self) -> None:
         """
         Using this method a NetApp can get onboarded to CAPIF.
         After calling this method the following should happen:
          a) A signed certificate should exist in folder folder_to_store_certificates
-         b) A json file 'capif_api_details.json' should exist with the api_invoker_id and the api discovery url
+         b) A json file 'capif_api_security_context_details_.json' should exist with the api_invoker_id and the api discovery url
 
         These will be used  ServiceDiscoverer class in order to communicate with CAPIF and discover services
 
         """
         public_key = self.__create_private_and_public_keys()
         role = "invoker"
         registration_result = self.__register_to_capif(role)
@@ -979,14 +975,35 @@
         api_invoker_id = (
             self.__onboard_netapp_to_capif_and_create_the_signed_certificate(
                 public_key, capif_onboarding_url, capif_access_token
             )
         )
         self.__write_to_file(self.csr_common_name, api_invoker_id, capif_discover_url)
 
+    def __load_netapp_api_details(self):
+        with open(
+                self.folder_to_store_certificates + self.capif_api_details_filename,
+                "r",
+        ) as openfile:
+            return json.load(openfile)
+    def offboard_netapp(self) ->None:
+        capif_api_details = self.__load_netapp_api_details()
+        url = self.capif_https_url + "api-invoker-management/v1/onboardedInvokers/" +capif_api_details["api_invoker_id"]
+        requests.request(
+            "DELETE",
+            url,
+            verify=self.folder_to_store_certificates + "ca.crt"
+        )
+
+
+    def offboard_and_deregister_netapp(self)->None:
+        self.offboard_netapp()
+        role = "invoker"
+        self.de_register_from_capif(role)
+
     def __create_private_and_public_keys(self) -> str:
         """
         Creates 2 keys in folder folder_to_store_certificates. A private.key and a cert_req.csr.
         :return: The contents of the public key
         """
 
         private_key_path = self.folder_to_store_certificates + "private.key"
@@ -1033,14 +1050,33 @@
             data=json.dumps(payload),
         )
         response.raise_for_status()
 
         response_payload = json.loads(response.text)
         return response_payload
 
+    def de_register_from_capif(self,role):
+
+        url = self.capif_http_url + "remove"
+        payload = dict()
+        payload["username"] = self.capif_netapp_username
+        payload["password"] = self.capif_netapp_password
+        payload["role"] = role
+
+        response = requests.request(
+            "DELETE",
+            url,
+            headers={"Content-Type": "application/json"},
+            data=json.dumps(payload)
+        )
+        response.raise_for_status()
+
+        response_payload = json.loads(response.text)
+        return response_payload
+
     def __save_capif_ca_root_file_and_get_auth_token(self, role):
 
         url = self.capif_http_url + "getauth"
 
         payload = dict()
         payload["username"] = self.capif_netapp_username
         payload["password"] = self.capif_netapp_password
@@ -1061,15 +1097,14 @@
     def __onboard_netapp_to_capif_and_create_the_signed_certificate(
             self, public_key, capif_onboarding_url, capif_access_token
     ):
         url = self.capif_https_url + capif_onboarding_url
         payload_dict = {
             "notificationDestination": self.capif_callback_url,
             "supportedFeatures": "fffffff",
-            # TODO: This works fine.  But what about CapifProviderConnector class where we onboard a Provider/Exposer. On onboarding there we dont pass the username. Is this a mistake in the flow? Or a different flow is implemented there
             "apiInvokerInformation": self.csr_common_name,
             "websockNotifConfig": {
                 "requestWebsocketUri": True,
                 "websocketUri": "websocketUri",
             },
             "onboardingInformation": {"apiInvokerPublicKey": str(public_key, "utf-8")},
             "requestTestNotification": True,
@@ -1098,15 +1133,15 @@
             )
         )
         certification_file.close()
         return response_payload["apiInvokerId"]
 
     def __write_to_file(self, csr_common_name, api_invoker_id, discover_services_url):
         with open(
-                self.folder_to_store_certificates + "capif_api_details.json", "w"
+                self.folder_to_store_certificates + self.capif_api_details_filename, "w"
         ) as outfile:
             json.dump(
                 {
                     "csr_common_name": csr_common_name,
                     "api_invoker_id": api_invoker_id,
                     "discover_services_url": discover_services_url,
                 },
@@ -1453,15 +1488,15 @@
         self.ca_root_path = self.folder_to_store_certificates_and_api_key + "ca.crt"
 
     def get_api_invoker_id(self):
         return self.capif_api_details["api_invoker_id"]
 
     def __load_netapp_api_details(self):
         with open(
-                self.folder_to_store_certificates_and_api_key + "capif_api_details.json",
+                self.folder_to_store_certificates_and_api_key + "capif_api_security_context_details.json",
                 "r",
         ) as openfile:
             return json.load(openfile)
 
     def _add_trailing_slash_to_url_if_missing(self, url):
         if url[len(url) - 1] != "/":
             url = url + "/"
@@ -1470,35 +1505,86 @@
     def get_access_token(self, api_name, api_id, aef_id):
         """
         :param api_name: The api id name is returned by discover services
          :param api_id: The api id that is returned by discover services
         :param aef_id: The relevant aef_id that is returned by discover services
          :return: The access token (jwt)
         """
-        if not self.__aef_id_already_registered(aef_id):
+
+        # if we dont have a security contenxt created before, create one
+        if self.__security_context_does_not_exist():
+            self.capif_api_details["registered_security_contexes"] = []
+            self.capif_api_details["registered_security_contexes"].append({ "api_id": api_id, "aef_id": aef_id})
             self.__register_security_service(api_id, aef_id)
-            self.__save_aef_id_to_already_registered_cached_list(aef_id)
+            self.__cache_security_context()
+        elif  self.__security_context_for_given_api_id_and_aef_id_does_not_exist(api_id,aef_id):
+            self.capif_api_details["registered_security_contexes"].append({ "api_id": api_id, "aef_id": aef_id})
+            self.__update_security_service(api_id,aef_id)
+            self.__cache_security_context()
+
+
 
         token_dic = self.__get_security_token(api_name, aef_id)
         return token_dic["access_token"]
 
-    def __aef_id_already_registered(self, aef_id):
-        return "registered_aef_ids" in self.capif_api_details and \
-            aef_id in self.capif_api_details["registered_aef_ids"]
-
-    def __save_aef_id_to_already_registered_cached_list(self, aef_id):
-        if "registered_aef_ids" not in self.capif_api_details:
-            self.capif_api_details["registered_aef_ids"] = []
+    def __security_context_does_not_exist(self):
+        return "registered_security_contexes" not in self.capif_api_details
+
+
+    def __security_context_for_given_api_id_and_aef_id_does_not_exist(self,api_id,aef_id):
+        contexes = self.capif_api_details["registered_security_contexes"]
+        results = list(filter(lambda c: c['api_id']== api_id and c["aef_id"]==aef_id, contexes))
+        return len(results) == 0
+
 
-        self.capif_api_details["registered_aef_ids"].append(aef_id)
+    def __cache_security_context(self):
         with open(
-                self.folder_to_store_certificates_and_api_key + "capif_api_details.json", "w"
+                self.folder_to_store_certificates_and_api_key + "capif_api_security_context_details.json", "w"
         ) as outfile:
             json.dump(self.capif_api_details, outfile)
 
+
+    def __update_security_service(self, api_id, aef_id):
+        """
+
+        :param api_id: The api id that is returned by discover services
+        :param aef_id: The aef_id that is returned by discover services
+        :return: None
+        """
+        url = "https://{}/capif-security/v1/trustedInvokers/{}/update".format(self.capif_host,
+                                                                       self.capif_api_details["api_invoker_id"])
+
+        payload = {
+            "securityInfo": [],
+            "notificationDestination": "https://mynotificationdest.com",
+            "requestTestNotification": True,
+            "websockNotifConfig": {
+                "websocketUri": "string",
+                "requestWebsocketUri": True
+            },
+            "supportedFeatures": "fff"
+        }
+
+        for security_info in self.capif_api_details["registered_security_contexes"]:
+            payload["securityInfo"].append({
+                "prefSecurityMethods": ["OAUTH"],
+                "aefId": security_info["aef_id"],
+                "apiId": security_info["api_id"]
+            })
+
+        response = requests.post(url,
+                                json=payload,
+                                cert=(self.signed_key_crt_path, self.private_key_path),
+                                verify=self.ca_root_path
+                                )
+
+        response.raise_for_status()
+        response.json()
+
+
     def __register_security_service(self, api_id, aef_id):
         """
 
         :param api_id: The api id that is returned by discover services
         :param aef_id: The aef_id that is returned by discover services
         :return: None
         """
@@ -1726,16 +1812,15 @@
         """
         Returns the names of supported time-sensitive networking (TSN) profiles.
 
         :return: a list of TSN profiles. Each TSN profile is a TSNProfile class.
 
         """
         url = self.url_prefix + self.service_discoverer. \
-            retrieve_specific_resource_name(self.api_name, "TSN_LIST_PROFILES"). \
-            format(scsAsId=self.api_invoker_id)
+            retrieve_specific_resource_name(self.api_name, "TSN_LIST_PROFILES")
 
         response = requests.get(url=url, headers=self.headers_auth)
         response.raise_for_status()
         response_dict = json.loads(response.text)
         return [
             self.TSNProfile(tsn_manager=self, profile_name=name)
             for name in response_dict["profiles"]
```

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/__init__.py` & `evolved5g-1.0.6/evolved5g/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/__init__.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/cells_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/cells_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/default_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/g_n_bs_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/g_n_bs_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/location_frontend_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/location_frontend_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/login_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/login_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/monitoring_event_api_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/monitoring_event_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/paths_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/paths_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/qo_s_information_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/qo_s_information_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/session_with_qo_s_api_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/session_with_qo_s_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/u_es_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/u_es_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/ui_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/ui_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/users_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api/utils_api.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/api_client.py` & `evolved5g-1.0.6/evolved5g/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/configuration.py` & `evolved5g-1.0.6/evolved5g/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/__init__.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/accumulated_usage.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/accumulated_usage.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_u_es_speed.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_u_es_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_create_speed.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_ue_create_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_speed.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_ue_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_update_speed.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_ue_update_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/cell.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/cell.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/cell_create.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/cell_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/cell_update.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/cell_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/gnb.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/gnb.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_create.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/gnb_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_update.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/gnb_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/http_validation_error.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/location_info.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/location_info.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report_received.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_report_received.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription_create.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_event_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_notification.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_notification.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_type.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/monitoring_type.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/msg.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/msg.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/path.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/path.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/path_create.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/path_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/path_update.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/path_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/paths.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/paths.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/point.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/point.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/qo_s_monitoring_report.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/qo_s_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/qos_monitoring_information.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/qos_monitoring_information.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/reporting_frequency.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/reporting_frequency.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/snssai.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/snssai.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/speed.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/token.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/u_es.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/u_es.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/ue.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/ue.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/ue_create.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/ue_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/ue_update.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/ue_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/usage_threshold.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/usage_threshold.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/user.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/user_create.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/user_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/user_plane_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event_report.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/user_plane_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_notification_data.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/user_plane_notification_data.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/user_update.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/user_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/models/validation_error.py` & `evolved5g-1.0.6/evolved5g/swagger_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g/swagger_client/rest.py` & `evolved5g-1.0.6/evolved5g/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.5/evolved5g.egg-info/PKG-INFO` & `evolved5g-1.0.6/evolved5g.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.5
+Version: 1.0.6
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,21 +54,31 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.6 (2023-06-14)
+        -------------------
+        
+        * The CLI command run-verification-tests now required three inputs (capif registration file, certificates folder and verification file) to launch NEF and TSN verification pipelines.
+        * CAPIFProviderConnector has a new method offboard_and_deregister_netapp() that allows a network app to be offboarded and deregistered from CAPIF.
+        * The SDK classes LocationSubscriber,ConnectionMonitor,QosAwareness don't accept the parameter 'nef_bearer_access_token' any more.
+        * The CLI method register_and_onboard_to_capif now accepts a second parameter --environment that takes values "production" or "development".
+        If this parameter is set to production then validation tests are running in the background, just after the registration and onboarding of the network app finishes.
+        
+        -------------------
         1.0.5 (2023-05-24)
         -------------------
         * Bug fix on CAPIFProviderConnector. When storing the capif_cert_server.pem the port was hardcoded.
         * Improvement on verification pipelines. Required user and password.
         * TSN verification pipeline added.
         * Validation pipeline included.
-         
+        
         -------------------
         1.0.4 (2023-04-27)
         -------------------
         * Bug fix on ServiceDiscoverer: When creating the security context we now pass OAUTH as prefSecurityMethod
         
         -------------------
         1.0.3 (2023-04-25)
```

### Comparing `evolved5g-1.0.5/evolved5g.egg-info/SOURCES.txt` & `evolved5g-1.0.6/evolved5g.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 docs/source/installation.rst
 docs/source/libraries.rst
 docs/source/pipelines.rst
 docs/source/pre_requisites.rst
 docs/source/images/dummy_html_example.png
 docs/source/images/generate.gif
 docs/source/images/generate_execution.png
+docs/source/images/netapp_creation.gif
+docs/source/images/netapp_repo.gif
 docs/source/images/repo_creation.png
 docs/source/images/repo_structure.png
 docs/source/images/ssh_gpg.png
 docs/source/images/ssh_key.png
 docs/source/images/ssh_key_button.png
 docs/source/images/token1.png
 docs/source/images/token2.png
 docs/source/images/token3.png
 evolved5g/__init__.py
 evolved5g/cli.py
 evolved5g/cli_helper.py
-evolved5g/nef_and_tsn_api_service_tests.py
+evolved5g/nef_and_tsn_api_service_validation_pipeline.py
 evolved5g/sdk.py
 evolved5g/utils.py
 evolved5g.egg-info/PKG-INFO
 evolved5g.egg-info/SOURCES.txt
 evolved5g.egg-info/dependency_links.txt
 evolved5g.egg-info/entry_points.txt
 evolved5g.egg-info/not-zip-safe
```

### Comparing `evolved5g-1.0.5/setup.py` & `evolved5g-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords="evolved5g",
     name="evolved5g",
     packages=find_packages(include=["evolved5g", "evolved5g.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/EVOLVED-5G/SDK-CLI",
-    version="1.0.5",
+    version="1.0.6",
     zip_safe=False,
 )
```

