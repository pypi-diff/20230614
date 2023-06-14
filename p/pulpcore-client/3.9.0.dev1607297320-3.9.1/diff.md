# Comparing `tmp/pulpcore-client-3.9.0.dev1607297320.tar.gz` & `tmp/pulpcore-client-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulpcore-client-3.9.0.dev1607297320.tar", last modified: Sun Dec  6 23:28:46 2020, max compression
+gzip compressed data, was "dist/pulpcore-client-3.9.1.tar", last modified: Thu Jan 21 19:35:15 2021, max compression
```

## Comparing `pulpcore-client-3.9.0.dev1607297320.tar` & `pulpcore-client-3.9.1.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/
--rw-r--r--   0 runner    (1001) docker     (116)      366 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    14780 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (116)     7294 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/
--rw-r--r--   0 runner    (1001) docker     (116)     1489 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    25714 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/access_policies_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    33439 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/artifacts_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    25101 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/exporters_core_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    35914 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/exporters_pulp_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    35210 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    13928 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_model_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    25128 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_object_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    18783 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_users_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    24919 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/importers_core_imports_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    35818 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/importers_pulp_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5228 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/orphans_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5296 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/repair_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    13286 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/signing_services_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5382 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/status_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    17286 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/task_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    37853 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    35638 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    18713 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    20587 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/workers_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    26289 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)    13967 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     3769 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/
--rw-r--r--   0 runner    (1001) docker     (116)     5371 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6080 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/access_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)     7791 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/access_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     8237 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/artifact.py
--rw-r--r--   0 runner    (1001) docker     (116)    10073 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/artifact_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3572 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4444 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/content_app_status_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3778 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/database_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3641 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group.py
--rw-r--r--   0 runner    (1001) docker     (116)     6707 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_progress_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4927 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3901 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_user.py
--rw-r--r--   0 runner    (1001) docker     (116)     4662 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6015 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/import_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5560 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_access_policy_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5468 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_artifact_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5399 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_group_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5491 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_group_user_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5422 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_import_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5514 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_permission_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5514 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_pulp_export_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5560 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_pulp_exporter_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5560 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_pulp_importer_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5606 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_signing_service_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5491 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_task_group_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5376 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_task_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5422 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_upload_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5376 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_user_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5422 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_worker_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5698 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)     3543 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_group.py
--rw-r--r--   0 runner    (1001) docker     (116)     5799 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_pulp_exporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     4636 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_pulp_importer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3474 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_task_cancel.py
--rw-r--r--   0 runner    (1001) docker     (116)     5337 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/permission_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     7560 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/progress_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     7593 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_export.py
--rw-r--r--   0 runner    (1001) docker     (116)     8684 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_export_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6129 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_exporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     7872 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_exporter_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4137 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     4706 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_importer.py
--rw-r--r--   0 runner    (1001) docker     (116)     6385 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_importer_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3740 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/redis_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6212 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/signing_service_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     9552 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5946 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/storage_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11411 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/task_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    15715 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/task_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3466 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (116)     4221 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_chunk.py
--rw-r--r--   0 runner    (1001) docker     (116)     3951 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_chunk_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3576 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_commit.py
--rw-r--r--   0 runner    (1001) docker     (116)     6716 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5881 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4436 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/user_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11435 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4579 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5859 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/worker_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12311 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      366 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7437 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/pulpcore_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1114 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 23:28:46.000000 pulpcore-client-3.9.0.dev1607297320/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_access_policies_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1793 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)     2027 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_access_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1620 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (116)     1832 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_artifact_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1254 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_artifacts_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1655 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_content_app_status_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1603 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_database_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1333 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_exporters_core_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_exporters_pulp_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1356 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_group.py
--rw-r--r--   0 runner    (1001) docker     (116)     1696 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_group_progress_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1506 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1410 2020-12-06 23:28:44.000000 pulpcore-client-3.9.0.dev1607297320/test/test_group_user.py
--rw-r--r--   0 runner    (1001) docker     (116)     1534 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_group_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1483 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1088 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_groups_model_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1347 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_groups_object_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_groups_users_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1664 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_import_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1333 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_importers_core_imports_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_importers_pulp_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      868 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_orphans_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     2386 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_access_policy_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2368 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_artifact_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     1980 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_group_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2005 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_group_user_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_import_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2088 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_permission_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2529 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_pulp_export_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2344 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_pulp_exporter_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2259 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_pulp_importer_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2223 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_signing_service_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2731 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_task_group_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     3450 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_task_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2191 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_upload_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2558 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_user_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2197 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_paginated_worker_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     1666 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_patched_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1407 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_patched_group.py
--rw-r--r--   0 runner    (1001) docker     (116)     1632 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_patched_pulp_exporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1524 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_patched_pulp_importer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1465 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_patched_task_cancel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1568 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_permission_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1669 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_progress_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1643 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_pulp_export.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_pulp_export_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1689 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_pulp_exporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1923 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_pulp_exporter_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1413 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_pulp_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     1473 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_pulp_importer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1762 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_pulp_importer_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_redis_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      867 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_repair_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1752 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_signing_service_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1051 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_signing_services_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      880 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_status_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     3624 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_storage_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_task_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1011 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_task_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     2805 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_task_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1223 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1365 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (116)     1477 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_upload_chunk.py
--rw-r--r--   0 runner    (1001) docker     (116)     1515 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_upload_chunk_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1439 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_upload_commit.py
--rw-r--r--   0 runner    (1001) docker     (116)     1995 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_upload_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1706 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1487 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1526 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_user_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2098 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1541 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_version_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1685 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_worker_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      983 2020-12-06 23:28:45.000000 pulpcore-client-3.9.0.dev1607297320/test/test_workers_api.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)      352 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    14765 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (116)       75 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (116)       75 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (116)     7279 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/
+-rw-r--r--   0 runner    (1001) docker     (116)     1489 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25714 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/access_policies_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    33439 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/artifacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25101 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/exporters_core_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35914 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/exporters_pulp_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35210 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13928 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_model_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25128 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_object_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18783 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24919 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/importers_core_imports_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35818 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/importers_pulp_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5228 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/orphans_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5296 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/repair_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13286 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/signing_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5382 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/status_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17286 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/task_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37853 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35638 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18713 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20587 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/workers_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26274 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13952 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3769 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/
+-rw-r--r--   0 runner    (1001) docker     (116)     5371 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6080 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7791 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/access_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8237 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10073 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/artifact_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3572 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4444 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/content_app_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3778 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/database_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3641 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6707 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_progress_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4927 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3901 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_user.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4662 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6015 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/import_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5560 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_access_policy_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5468 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_artifact_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5399 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_group_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5491 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_group_user_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5422 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_import_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5514 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_permission_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5514 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_pulp_export_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5560 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_pulp_exporter_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5560 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_pulp_importer_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5606 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_signing_service_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5491 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_task_group_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5376 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_task_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5422 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_upload_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5376 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_user_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5422 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_worker_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5698 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3543 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5799 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_pulp_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4636 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_pulp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3474 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_task_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5337 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/permission_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7560 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/progress_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7593 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_export.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8684 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6129 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7872 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_exporter_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4137 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_import.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4706 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6385 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_importer_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3740 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/redis_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6212 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/signing_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9552 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5946 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/storage_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11411 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/task_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15715 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/task_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3466 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4221 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3951 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_chunk_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3576 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_commit.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6716 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5881 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4436 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/user_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11435 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4579 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5859 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/worker_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12311 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore/client/pulpcore/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      352 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     7437 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       48 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/pulpcore_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       69 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1099 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     1322 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_access_policies_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1793 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2027 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_access_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1620 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1832 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_artifact_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1254 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_artifacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1547 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1655 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_content_app_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1603 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_database_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1333 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_exporters_core_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1575 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_exporters_pulp_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1356 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1696 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_group_progress_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1506 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1410 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_group_user.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1534 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_group_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1483 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1088 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_groups_model_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1347 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_groups_object_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1132 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_groups_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1664 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_import_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1333 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_importers_core_imports_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1575 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_importers_pulp_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      868 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_orphans_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2386 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_access_policy_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2368 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_artifact_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1980 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_group_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2005 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_group_user_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2160 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_import_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2088 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_permission_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2529 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_pulp_export_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2344 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_pulp_exporter_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2259 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_pulp_importer_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2223 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_signing_service_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2731 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_task_group_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3450 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_task_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2191 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_upload_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2558 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_user_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2197 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_paginated_worker_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1666 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_patched_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1407 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_patched_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1632 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_patched_pulp_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1524 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_patched_pulp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1465 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_patched_task_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1568 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_permission_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1669 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_progress_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1643 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_pulp_export.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_pulp_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1689 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_pulp_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1923 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_pulp_exporter_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1413 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_pulp_import.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1473 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_pulp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1762 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_pulp_importer_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1570 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_redis_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      867 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_repair_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1752 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_signing_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1051 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_signing_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      880 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3624 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1572 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_storage_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2188 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_task_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1011 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_task_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2805 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1223 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1365 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1477 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_upload_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1515 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_upload_chunk_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1439 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_upload_commit.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1995 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_upload_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1706 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1487 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1526 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_user_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2098 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1541 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1685 2021-01-21 19:35:14.000000 pulpcore-client-3.9.1/test/test_worker_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      983 2021-01-21 19:35:15.000000 pulpcore-client-3.9.1/test/test_workers_api.py
```

### Comparing `pulpcore-client-3.9.0.dev1607297320/README.md` & `pulpcore-client-3.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulpcore-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 3.9.0.dev01607297320
+- Package version: 3.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/__init__.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "3.9.0.dev01607297320"
+__version__ = "3.9.1"
 
 # import apis into sdk package
 from pulpcore.client.pulpcore.api.access_policies_api import AccessPoliciesApi
 from pulpcore.client.pulpcore.api.artifacts_api import ArtifactsApi
 from pulpcore.client.pulpcore.api.exporters_core_exports_api import ExportersCoreExportsApi
 from pulpcore.client.pulpcore.api.exporters_pulp_api import ExportersPulpApi
 from pulpcore.client.pulpcore.api.groups_api import GroupsApi
```

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/__init__.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/access_policies_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/access_policies_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/artifacts_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/artifacts_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/exporters_core_exports_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/exporters_core_exports_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/exporters_pulp_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/exporters_pulp_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_model_permissions_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_model_permissions_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_object_permissions_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_object_permissions_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/groups_users_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/groups_users_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/importers_core_imports_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/importers_core_imports_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/importers_pulp_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/importers_pulp_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/orphans_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/orphans_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/repair_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/repair_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/signing_services_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/signing_services_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/status_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/status_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/task_groups_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/task_groups_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/tasks_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/uploads_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/uploads_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/users_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/users_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api/workers_api.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api/workers_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/api_client.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.9.0.dev01607297320/python'
+        self.user_agent = 'OpenAPI-Generator/3.9.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/configuration.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 3.9.0.dev01607297320".\
+               "SDK Package Version: 3.9.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/exceptions.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/__init__.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/access_policy.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/access_policy.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/access_policy_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/access_policy_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/artifact.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/artifact_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/artifact_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/async_operation_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/content_app_status_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/content_app_status_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/database_connection_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/database_connection_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_progress_report_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_progress_report_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_user.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_user.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/group_user_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/group_user_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/import_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/import_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_access_policy_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_access_policy_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_artifact_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_artifact_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_group_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_group_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_group_user_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_group_user_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_import_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_import_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_permission_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_permission_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_pulp_export_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_pulp_export_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_pulp_exporter_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_pulp_exporter_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_pulp_importer_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_pulp_importer_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_signing_service_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_signing_service_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_task_group_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_task_group_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_task_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_task_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_upload_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_upload_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_user_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_user_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/paginated_worker_response_list.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/paginated_worker_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_access_policy.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_access_policy.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_group.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_group.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_pulp_exporter.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_pulp_exporter.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_pulp_importer.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_pulp_importer.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/patched_task_cancel.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/patched_task_cancel.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/permission_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/permission_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/progress_report_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/progress_report_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_export.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_export.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_export_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_export_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_exporter.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_exporter.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_exporter_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_exporter_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_import.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_import.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_importer.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_importer.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/pulp_importer_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/pulp_importer_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/redis_connection_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/redis_connection_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/signing_service_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/signing_service_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/status_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/status_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/storage_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/storage_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/task_group_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/task_group_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/task_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/task_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_chunk.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_chunk.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_chunk_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_chunk_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_commit.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_commit.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_detail_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_detail_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/upload_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/upload_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/user_group_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/user_group_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/user_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/user_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/version_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/version_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/models/worker_response.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/models/worker_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore/client/pulpcore/rest.py` & `pulpcore-client-3.9.1/pulpcore/client/pulpcore/rest.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/pulpcore_client.egg-info/SOURCES.txt` & `pulpcore-client-3.9.1/pulpcore_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/setup.py` & `pulpcore-client-3.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulpcore-client"
-VERSION = "3.9.0.dev01607297320"
+VERSION = "3.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_access_policies_api.py` & `pulpcore-client-3.9.1/test/test_access_policies_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_access_policy.py` & `pulpcore-client-3.9.1/test/test_access_policy.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_access_policy_response.py` & `pulpcore-client-3.9.1/test/test_access_policy_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_artifact.py` & `pulpcore-client-3.9.1/test/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_artifact_response.py` & `pulpcore-client-3.9.1/test/test_artifact_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_artifacts_api.py` & `pulpcore-client-3.9.1/test/test_artifacts_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_async_operation_response.py` & `pulpcore-client-3.9.1/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_content_app_status_response.py` & `pulpcore-client-3.9.1/test/test_content_app_status_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_database_connection_response.py` & `pulpcore-client-3.9.1/test/test_database_connection_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_exporters_core_exports_api.py` & `pulpcore-client-3.9.1/test/test_exporters_core_exports_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_exporters_pulp_api.py` & `pulpcore-client-3.9.1/test/test_exporters_pulp_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_group.py` & `pulpcore-client-3.9.1/test/test_group.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_group_progress_report_response.py` & `pulpcore-client-3.9.1/test/test_group_progress_report_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_group_response.py` & `pulpcore-client-3.9.1/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_group_user.py` & `pulpcore-client-3.9.1/test/test_group_user.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_group_user_response.py` & `pulpcore-client-3.9.1/test/test_group_user_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_groups_api.py` & `pulpcore-client-3.9.1/test/test_groups_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_groups_model_permissions_api.py` & `pulpcore-client-3.9.1/test/test_groups_model_permissions_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_groups_object_permissions_api.py` & `pulpcore-client-3.9.1/test/test_groups_object_permissions_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_groups_users_api.py` & `pulpcore-client-3.9.1/test/test_groups_users_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_import_response.py` & `pulpcore-client-3.9.1/test/test_import_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_importers_core_imports_api.py` & `pulpcore-client-3.9.1/test/test_importers_core_imports_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_importers_pulp_api.py` & `pulpcore-client-3.9.1/test/test_importers_pulp_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_orphans_api.py` & `pulpcore-client-3.9.1/test/test_orphans_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_access_policy_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_access_policy_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_artifact_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_artifact_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_group_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_group_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_group_user_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_group_user_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_import_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_import_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_permission_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_permission_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_pulp_export_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_pulp_export_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_pulp_exporter_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_pulp_exporter_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_pulp_importer_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_pulp_importer_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_signing_service_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_signing_service_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_task_group_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_task_group_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_task_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_task_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_upload_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_upload_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_user_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_user_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_paginated_worker_response_list.py` & `pulpcore-client-3.9.1/test/test_paginated_worker_response_list.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_patched_access_policy.py` & `pulpcore-client-3.9.1/test/test_patched_access_policy.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_patched_group.py` & `pulpcore-client-3.9.1/test/test_patched_group.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_patched_pulp_exporter.py` & `pulpcore-client-3.9.1/test/test_patched_pulp_exporter.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_patched_pulp_importer.py` & `pulpcore-client-3.9.1/test/test_patched_pulp_importer.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_patched_task_cancel.py` & `pulpcore-client-3.9.1/test/test_patched_task_cancel.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_permission_response.py` & `pulpcore-client-3.9.1/test/test_permission_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_progress_report_response.py` & `pulpcore-client-3.9.1/test/test_progress_report_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_pulp_export.py` & `pulpcore-client-3.9.1/test/test_pulp_export.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_pulp_export_response.py` & `pulpcore-client-3.9.1/test/test_pulp_export_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_pulp_exporter.py` & `pulpcore-client-3.9.1/test/test_pulp_exporter.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_pulp_exporter_response.py` & `pulpcore-client-3.9.1/test/test_pulp_exporter_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_pulp_import.py` & `pulpcore-client-3.9.1/test/test_pulp_import.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_pulp_importer.py` & `pulpcore-client-3.9.1/test/test_pulp_importer.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_pulp_importer_response.py` & `pulpcore-client-3.9.1/test/test_pulp_importer_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_redis_connection_response.py` & `pulpcore-client-3.9.1/test/test_redis_connection_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_repair_api.py` & `pulpcore-client-3.9.1/test/test_repair_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_signing_service_response.py` & `pulpcore-client-3.9.1/test/test_signing_service_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_signing_services_api.py` & `pulpcore-client-3.9.1/test/test_signing_services_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_status_api.py` & `pulpcore-client-3.9.1/test/test_status_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_status_response.py` & `pulpcore-client-3.9.1/test/test_status_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_storage_response.py` & `pulpcore-client-3.9.1/test/test_storage_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_task_group_response.py` & `pulpcore-client-3.9.1/test/test_task_group_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_task_groups_api.py` & `pulpcore-client-3.9.1/test/test_task_groups_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_task_response.py` & `pulpcore-client-3.9.1/test/test_task_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_tasks_api.py` & `pulpcore-client-3.9.1/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_upload.py` & `pulpcore-client-3.9.1/test/test_upload.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_upload_chunk.py` & `pulpcore-client-3.9.1/test/test_upload_chunk.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_upload_chunk_response.py` & `pulpcore-client-3.9.1/test/test_upload_chunk_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_upload_commit.py` & `pulpcore-client-3.9.1/test/test_upload_commit.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_upload_detail_response.py` & `pulpcore-client-3.9.1/test/test_upload_detail_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_upload_response.py` & `pulpcore-client-3.9.1/test/test_upload_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_uploads_api.py` & `pulpcore-client-3.9.1/test/test_uploads_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_user_group_response.py` & `pulpcore-client-3.9.1/test/test_user_group_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_user_response.py` & `pulpcore-client-3.9.1/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_users_api.py` & `pulpcore-client-3.9.1/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_version_response.py` & `pulpcore-client-3.9.1/test/test_version_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_worker_response.py` & `pulpcore-client-3.9.1/test/test_worker_response.py`

 * *Files identical despite different names*

### Comparing `pulpcore-client-3.9.0.dev1607297320/test/test_workers_api.py` & `pulpcore-client-3.9.1/test/test_workers_api.py`

 * *Files identical despite different names*

