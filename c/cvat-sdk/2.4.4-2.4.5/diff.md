# Comparing `tmp/cvat_sdk-2.4.4.tar.gz` & `tmp/cvat_sdk-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk-2.4.4.tar", last modified: Fri May 19 11:29:16 2023, max compression
+gzip compressed data, was "cvat_sdk-2.4.5.tar", last modified: Wed Jun 14 19:50:01 2023, max compression
```

## Comparing `cvat_sdk-2.4.4.tar` & `cvat_sdk-2.4.5.tar`

### file list

```diff
@@ -1,217 +1,218 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.4/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.4/README.md
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.051894 cvat_sdk-2.4.4/cvat_sdk/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.061894 cvat_sdk-2.4.4/cvat_sdk/api_client/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.061894 cvat_sdk-2.4.4/cvat_sdk/api_client/api/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    51130 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/auth_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    59211 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/cloudstorages_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33454 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/comments_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15480 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/events_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    32769 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/invitations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33944 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/issues_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    86553 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/jobs_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    28832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/labels_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    36609 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/lambda_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    27089 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/memberships_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33378 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/organizations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    78780 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/projects_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11305 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/schema_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    24041 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/server_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)   140016 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/tasks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    32999 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/users_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    72493 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/webhooks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45222 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api_client.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.061894 cvat_sdk-2.4.4/cvat_sdk/api_client/apis/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1711 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/apis/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/configuration.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/exceptions.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.071894 cvat_sdk-2.4.4/cvat_sdk/api_client/model/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/about.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotation_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotations_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/backup_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12787 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/chunk_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comments_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13414 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/credentials_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15261 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/data_meta_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    28377 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_format.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_formats.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/event.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/event_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15575 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/events_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12705 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/frame_meta.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12971 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/input_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/issues_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    20943 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read_assignee.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12873 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_stage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12871 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/jobs_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/label.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labels_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12769 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/location_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/login_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14906 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/membership_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/meta_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/online_function_call_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12955 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/operation_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_comment_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_invitation_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_issue_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_job_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_label_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_membership_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_meta_user_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_organization_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_project_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_task_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_change_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_confirm_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_data_meta_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_label_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_membership_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/plugins.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13163 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/provider_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/rest_auth_detail.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12920 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/role_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12937 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status_state_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13253 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/signing_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12994 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sorting_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12760 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12839 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/tasks_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/token.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12550 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_content_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16363 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_delivery_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12771 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model_utils.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.071894 cvat_sdk-2.4.4/cvat_sdk/api_client/models/
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13505 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/models/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/rest.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk/core/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/client.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/downloading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/git.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/helpers.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/progress.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk/core/proxies/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/annotations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/issues.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/jobs.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/model_proxy.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/organizations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/projects.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14224 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/tasks.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/users.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13947 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/uploading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/utils.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/models.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk/pytorch/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/caching.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/common.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/project_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/task_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/transforms.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     9179 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/top_level.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.4/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-05-19 11:27:39.000000 cvat_sdk-2.4.4/requirements/api_client.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.4/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-05-19 11:27:39.000000 cvat_sdk-2.4.4/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.5/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.5/README.md
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/api_client/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/api_client/api/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45482 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/auth_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    60847 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/cloudstorages_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31362 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/comments_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15007 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/events_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30677 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/invitations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31852 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/issues_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    78813 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/jobs_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    26714 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/labels_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33079 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/lambda_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24997 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/memberships_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    29848 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/organizations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    73158 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/projects_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    10673 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/schema_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21217 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/server_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)   128040 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/tasks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30201 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/users_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    66165 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/webhooks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45222 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api_client.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/api_client/apis/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1711 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/apis/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/configuration.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/exceptions.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.166667 cvat_sdk-2.4.5/cvat_sdk/api_client/model/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/about.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotation_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotations_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/backup_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13023 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/chunk_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13139 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_content.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comments_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14282 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/credentials_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15330 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_meta_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31709 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_format.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_formats.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/event.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/event_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18731 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/events_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12821 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/frame_meta.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13367 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/input_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/issues_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21389 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read_assignee.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_stage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13203 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/jobs_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/label.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labels_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12981 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/location_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/login_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14975 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/membership_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/meta_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/online_function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13335 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/operation_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_comment_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_invitation_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_issue_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_job_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_label_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_membership_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_meta_user_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_organization_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_project_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_task_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_change_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_confirm_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_data_meta_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_label_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_membership_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/plugins.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13747 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/provider_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/rest_auth_detail.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13300 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/role_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13285 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status_state_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13953 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/signing_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13430 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sorting_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12956 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13123 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/tasks_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/token.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12666 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_content_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16432 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_delivery_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12991 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model_utils.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.166667 cvat_sdk-2.4.5/cvat_sdk/api_client/models/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13607 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/models/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/rest.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.166667 cvat_sdk-2.4.5/cvat_sdk/core/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/client.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/downloading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/git.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/helpers.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/progress.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/cvat_sdk/core/proxies/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/annotations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/issues.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/jobs.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/model_proxy.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/organizations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/projects.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14268 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/tasks.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/users.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13947 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/uploading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/utils.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/models.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/cvat_sdk/pytorch/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/caching.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/common.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/project_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/task_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/transforms.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/cvat_sdk.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     9232 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/top_level.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.5/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-06-14 19:49:19.000000 cvat_sdk-2.4.5/requirements/api_client.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.5/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-06-14 19:49:19.000000 cvat_sdk-2.4.5/setup.py
```

### Comparing `cvat_sdk-2.4.4/PKG-INFO` & `cvat_sdk-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat_sdk
-Version: 2.4.4
+Version: 2.4.5
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.4/README.md` & `cvat_sdk-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/__init__.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
-__version__ = "2.4.4"
+__version__ = "2.4.5"
 
 from cvat_sdk.api_client.api_client import ApiClient
 
 from cvat_sdk.api_client.configuration import Configuration
 
 from cvat_sdk.api_client.exceptions import OpenApiException
 from cvat_sdk.api_client.exceptions import ApiAttributeError
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/auth_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/cloudstorages_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -21,614 +21,735 @@
 from cvat_sdk.api_client.api_client import ApiClient, Endpoint as _Endpoint
 from cvat_sdk.api_client.model_utils import (  # noqa: F401
     date,
     datetime,
     file_type,
     none_type,
 )
-from cvat_sdk.api_client.model.login_serializer_ex_request import LoginSerializerExRequest
-from cvat_sdk.api_client.model.password_change_request import PasswordChangeRequest
-from cvat_sdk.api_client.model.password_reset_confirm_request import PasswordResetConfirmRequest
-from cvat_sdk.api_client.model.password_reset_serializer_ex_request import PasswordResetSerializerExRequest
-from cvat_sdk.api_client.model.register_serializer_ex import RegisterSerializerEx
-from cvat_sdk.api_client.model.register_serializer_ex_request import RegisterSerializerExRequest
-from cvat_sdk.api_client.model.rest_auth_detail import RestAuthDetail
-from cvat_sdk.api_client.model.signing_request import SigningRequest
-from cvat_sdk.api_client.model.token import Token
+from cvat_sdk.api_client.model.cloud_storage_content import CloudStorageContent
+from cvat_sdk.api_client.model.cloud_storage_read import CloudStorageRead
+from cvat_sdk.api_client.model.cloud_storage_write_request import CloudStorageWriteRequest
+from cvat_sdk.api_client.model.paginated_cloud_storage_read_list import PaginatedCloudStorageReadList
+from cvat_sdk.api_client.model.patched_cloud_storage_write_request import PatchedCloudStorageWriteRequest
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-class AuthApi(object):
+class CloudstoragesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_login_endpoint = _Endpoint(
+        self.create_endpoint = _Endpoint(
             settings={
-                'response_schema': (Token,),
+                'response_schema': (CloudStorageRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/auth/login',
-                'operation_id': 'create_login',
+                'endpoint_path': '/api/cloudstorages',
+                'operation_id': 'create',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'login_serializer_ex_request',
+                    'cloud_storage_write_request',
                     'x_organization',
                     'org',
                     'org_id',
                 ],
                 'required': [
-                    'login_serializer_ex_request',
+                    'cloud_storage_write_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'login_serializer_ex_request':
-                        (LoginSerializerExRequest,),
+                    'cloud_storage_write_request':
+                        (CloudStorageWriteRequest,),
                     'x_organization':
                         (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'org': 'org',
                     'org_id': 'org_id',
                 },
                 'location_map': {
-                    'login_serializer_ex_request': 'body',
+                    'cloud_storage_write_request': 'body',
                     'x_organization': 'header',
                     'org': 'query',
                     'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json'
+                    'application/json',
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
-        self.create_logout_endpoint = _Endpoint(
+        self.destroy_endpoint = _Endpoint(
             settings={
-                'response_schema': (RestAuthDetail,),
+                'response_schema': None,
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/auth/logout',
-                'operation_id': 'create_logout',
-                'http_method': 'POST',
+                'endpoint_path': '/api/cloudstorages/{id}',
+                'operation_id': 'destroy',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (int,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.list_endpoint = _Endpoint(
+            settings={
+                'response_schema': (PaginatedCloudStorageReadList,),
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/cloudstorages',
+                'operation_id': 'list',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'x_organization',
+                    'credentials_type',
+                    'filter',
+                    'name',
                     'org',
                     'org_id',
+                    'owner',
+                    'page',
+                    'page_size',
+                    'provider_type',
+                    'resource',
+                    'search',
+                    'sort',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
+                    'credentials_type',
+                    'provider_type',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('credentials_type',): {
+
+                        "KEY_SECRET_KEY_PAIR": "KEY_SECRET_KEY_PAIR",
+                        "ACCOUNT_NAME_TOKEN_PAIR": "ACCOUNT_NAME_TOKEN_PAIR",
+                        "KEY_FILE_PATH": "KEY_FILE_PATH",
+                        "ANONYMOUS_ACCESS": "ANONYMOUS_ACCESS",
+                        "CONNECTION_STRING": "CONNECTION_STRING"
+                    },
+                    ('provider_type',): {
+
+                        "AWS_S3_BUCKET": "AWS_S3_BUCKET",
+                        "AZURE_CONTAINER": "AZURE_CONTAINER",
+                        "GOOGLE_DRIVE": "GOOGLE_DRIVE",
+                        "GOOGLE_CLOUD_STORAGE": "GOOGLE_CLOUD_STORAGE"
+                    },
                 },
                 'openapi_types': {
                     'x_organization':
                         (str,),
+                    'credentials_type':
+                        (str,),
+                    'filter':
+                        (str,),
+                    'name':
+                        (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
+                    'owner':
+                        (str,),
+                    'page':
+                        (int,),
+                    'page_size':
+                        (int,),
+                    'provider_type':
+                        (str,),
+                    'resource':
+                        (str,),
+                    'search':
+                        (str,),
+                    'sort':
+                        (str,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
+                    'credentials_type': 'credentials_type',
+                    'filter': 'filter',
+                    'name': 'name',
                     'org': 'org',
                     'org_id': 'org_id',
+                    'owner': 'owner',
+                    'page': 'page',
+                    'page_size': 'page_size',
+                    'provider_type': 'provider_type',
+                    'resource': 'resource',
+                    'search': 'search',
+                    'sort': 'sort',
                 },
                 'location_map': {
                     'x_organization': 'header',
+                    'credentials_type': 'query',
+                    'filter': 'query',
+                    'name': 'query',
                     'org': 'query',
                     'org_id': 'query',
+                    'owner': 'query',
+                    'page': 'query',
+                    'page_size': 'query',
+                    'provider_type': 'query',
+                    'resource': 'query',
+                    'search': 'query',
+                    'sort': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.create_password_change_endpoint = _Endpoint(
+        self.partial_update_endpoint = _Endpoint(
             settings={
-                'response_schema': (RestAuthDetail,),
+                'response_schema': (CloudStorageRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/auth/password/change',
-                'operation_id': 'create_password_change',
-                'http_method': 'POST',
+                'endpoint_path': '/api/cloudstorages/{id}',
+                'operation_id': 'partial_update',
+                'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'password_change_request',
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'id',
+                    'patched_cloud_storage_write_request',
                 ],
                 'required': [
-                    'password_change_request',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'password_change_request':
-                        (PasswordChangeRequest,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
+                    'id':
                         (int,),
+                    'patched_cloud_storage_write_request':
+                        (PatchedCloudStorageWriteRequest,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'id': 'id',
                 },
                 'location_map': {
-                    'password_change_request': 'body',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'id': 'path',
+                    'patched_cloud_storage_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json'
+                    'application/json',
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
-        self.create_password_reset_endpoint = _Endpoint(
+        self.retrieve_endpoint = _Endpoint(
             settings={
-                'response_schema': (RestAuthDetail,),
+                'response_schema': (CloudStorageRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/auth/password/reset',
-                'operation_id': 'create_password_reset',
-                'http_method': 'POST',
+                'endpoint_path': '/api/cloudstorages/{id}',
+                'operation_id': 'retrieve',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'password_reset_serializer_ex_request',
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'id',
                 ],
                 'required': [
-                    'password_reset_serializer_ex_request',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'password_reset_serializer_ex_request':
-                        (PasswordResetSerializerExRequest,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
+                    'id':
                         (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'id': 'id',
                 },
                 'location_map': {
-                    'password_reset_serializer_ex_request': 'body',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.create_password_reset_confirm_endpoint = _Endpoint(
+        self.retrieve_actions_endpoint = _Endpoint(
             settings={
-                'response_schema': (RestAuthDetail,),
+                'response_schema': (str,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/auth/password/reset/confirm',
-                'operation_id': 'create_password_reset_confirm',
-                'http_method': 'POST',
+                'endpoint_path': '/api/cloudstorages/{id}/actions',
+                'operation_id': 'retrieve_actions',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'password_reset_confirm_request',
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'id',
                 ],
                 'required': [
-                    'password_reset_confirm_request',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'password_reset_confirm_request':
-                        (PasswordResetConfirmRequest,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
+                    'id':
                         (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'id': 'id',
                 },
                 'location_map': {
-                    'password_reset_confirm_request': 'body',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.create_register_endpoint = _Endpoint(
+        self.retrieve_content_endpoint = _Endpoint(
             settings={
-                'response_schema': (RegisterSerializerEx,),
+                'response_schema': ([str],),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/auth/register',
-                'operation_id': 'create_register',
-                'http_method': 'POST',
+                'endpoint_path': '/api/cloudstorages/{id}/content',
+                'operation_id': 'retrieve_content',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'register_serializer_ex_request',
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'id',
+                    'manifest_path',
                 ],
                 'required': [
-                    'register_serializer_ex_request',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'register_serializer_ex_request':
-                        (RegisterSerializerExRequest,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
+                    'id':
                         (int,),
+                    'manifest_path':
+                        (str,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'id': 'id',
+                    'manifest_path': 'manifest_path',
                 },
                 'location_map': {
-                    'register_serializer_ex_request': 'body',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'id': 'path',
+                    'manifest_path': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.create_signing_endpoint = _Endpoint(
+        self.retrieve_content_v2_endpoint = _Endpoint(
             settings={
-                'response_schema': (str,),
+                'response_schema': (CloudStorageContent,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/auth/signing',
-                'operation_id': 'create_signing',
-                'http_method': 'POST',
+                'endpoint_path': '/api/cloudstorages/{id}/content-v2',
+                'operation_id': 'retrieve_content_v2',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'signing_request',
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'id',
+                    'manifest_path',
+                    'next_token',
+                    'page_size',
+                    'prefix',
                 ],
                 'required': [
-                    'signing_request',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'signing_request':
-                        (SigningRequest,),
-                    'x_organization':
+                    'id':
+                        (int,),
+                    'manifest_path':
                         (str,),
-                    'org':
+                    'next_token':
                         (str,),
-                    'org_id':
+                    'page_size':
                         (int,),
+                    'prefix':
+                        (str,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'id': 'id',
+                    'manifest_path': 'manifest_path',
+                    'next_token': 'next_token',
+                    'page_size': 'page_size',
+                    'prefix': 'prefix',
                 },
                 'location_map': {
-                    'signing_request': 'body',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'id': 'path',
+                    'manifest_path': 'query',
+                    'next_token': 'query',
+                    'page_size': 'query',
+                    'prefix': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.retrieve_rules_endpoint = _Endpoint(
+        self.retrieve_preview_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
-                'auth': [],
-                'endpoint_path': '/api/auth/rules',
-                'operation_id': 'retrieve_rules',
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/cloudstorages/{id}/preview',
+                'operation_id': 'retrieve_preview',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'id',
+                ],
+                'required': [
+                    'id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
+                    'id':
                         (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'id': 'id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.retrieve_status_endpoint = _Endpoint(
+            settings={
+                'response_schema': (str,),
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/cloudstorages/{id}/status',
+                'operation_id': 'retrieve_status',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (int,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
 
-    def create_login(
+    def create(
         self,
-        login_serializer_ex_request: LoginSerializerExRequest,
+        cloud_storage_write_request: CloudStorageWriteRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[Token], urllib3.HTTPResponse]:
-        """create_login  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[CloudStorageRead], urllib3.HTTPResponse]:
+        """Method creates a cloud storage with a specified characteristics  # noqa: E501
 
-        Check the credentials and return the REST Token if the credentials are valid and authenticated. If email verification is enabled and the user has the unverified email, an email with a confirmation link will be sent. Calls Django Auth login method to register User ID in Django session framework.  Accept the following POST parameters: username, email, password Return the REST Framework Token Object's key.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_login(login_serializer_ex_request, _async_call=True)
+        >>> thread = api.create(cloud_storage_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            login_serializer_ex_request (LoginSerializerExRequest):
+            cloud_storage_write_request (CloudStorageWriteRequest):
 
         Keyword Args:
             x_organization (str): [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
@@ -659,60 +780,147 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (Token, HTTPResponse)
+            (CloudStorageRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['login_serializer_ex_request'] = login_serializer_ex_request
-        return self.create_login_endpoint.call_with_http_info(**kwargs)
+        kwargs['cloud_storage_write_request'] = cloud_storage_write_request
+        return self.create_endpoint.call_with_http_info(**kwargs)
 
-    def create_logout(
+    def destroy(
         self,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[RestAuthDetail], urllib3.HTTPResponse]:
-        """create_logout  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+        """Method deletes a specific cloud storage  # noqa: E501
 
-        Calls Django logout method and delete the Token object assigned to the current User object.  Accepts/Returns nothing.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_logout(_async_call=True)
+        >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
+        Args:
+            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
+            _parse_response (bool): if False, the response data will not be parsed,
+                None is returned for data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _validate_inputs (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _validate_outputs (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _check_status (bool): whether to check response status
+                for being positive or not.
+                Default is True
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            _async_call (bool): execute request asynchronously
+
+        Returns:
+            (None, HTTPResponse)
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['_async_call'] = _async_call
+        kwargs['_parse_response'] = _parse_response
+        kwargs['_request_timeout'] = _request_timeout
+        kwargs['_validate_inputs'] = _validate_inputs
+        kwargs['_validate_outputs'] = _validate_outputs
+        kwargs['_check_status'] = _check_status
+        kwargs['_spec_property_naming'] = _spec_property_naming
+        kwargs['_content_type'] = _content_type
+        kwargs['_host_index'] = _host_index
+        kwargs['_request_auths'] = _request_auths
+        kwargs['id'] = id
+        return self.destroy_endpoint.call_with_http_info(**kwargs)
+
+    def list(
+        self,
+        *,
+        _parse_response: bool = True,
+        _request_timeout: typing.Union[int, float, tuple] = None,
+        _validate_inputs: bool = True,
+        _validate_outputs: bool = True,
+        _check_status: bool = True,
+        _spec_property_naming: bool = False,
+        _content_type: typing.Optional[str] = None,
+        _host_index: typing.Optional[int] = None,
+        _request_auths: typing.Optional[typing.List] = None,
+        _async_call: bool = False,
+        **kwargs,
+    ) -> typing.Tuple[typing.Optional[PaginatedCloudStorageReadList], urllib3.HTTPResponse]:
+        """Returns a paginated list of storages  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass _async_call=True
+
+        >>> thread = api.list(_async_call=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            x_organization (str): Organization unique slug. [optional]
+            credentials_type (str): A simple equality filter for the credentials_type field. [optional]
+            filter (str): A filter term. Available filter_fields: ['provider_type', 'name', 'resource', 'credentials_type', 'owner', 'description', 'id']. [optional]
+            name (str): A simple equality filter for the name field. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
+            owner (str): A simple equality filter for the owner field. [optional]
+            page (int): A page number within the paginated result set.. [optional]
+            page_size (int): Number of results to return per page.. [optional]
+            provider_type (str): A simple equality filter for the provider_type field. [optional]
+            resource (str): A simple equality filter for the resource field. [optional]
+            search (str): A search term. Available search_fields: ('provider_type', 'name', 'resource', 'credentials_type', 'owner', 'description'). [optional]
+            sort (str): Which field to use when ordering the results. Available ordering_fields: ['provider_type', 'name', 'resource', 'credentials_type', 'owner', 'description', 'id']. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -738,62 +946,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (RestAuthDetail, HTTPResponse)
+            (PaginatedCloudStorageReadList, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        return self.create_logout_endpoint.call_with_http_info(**kwargs)
+        return self.list_endpoint.call_with_http_info(**kwargs)
 
-    def create_password_change(
+    def partial_update(
         self,
-        password_change_request: PasswordChangeRequest,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[RestAuthDetail], urllib3.HTTPResponse]:
-        """create_password_change  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[CloudStorageRead], urllib3.HTTPResponse]:
+        """Methods does a partial update of chosen fields in a cloud storage instance  # noqa: E501
 
-        Calls Django Auth SetPasswordForm save method.  Accepts the following POST parameters: new_password1, new_password2 Returns the success/fail message.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_password_change(password_change_request, _async_call=True)
+        >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            password_change_request (PasswordChangeRequest):
+            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
+            patched_cloud_storage_write_request (PatchedCloudStorageWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -819,63 +1024,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (RestAuthDetail, HTTPResponse)
+            (CloudStorageRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['password_change_request'] = password_change_request
-        return self.create_password_change_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.partial_update_endpoint.call_with_http_info(**kwargs)
 
-    def create_password_reset(
+    def retrieve(
         self,
-        password_reset_serializer_ex_request: PasswordResetSerializerExRequest,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[RestAuthDetail], urllib3.HTTPResponse]:
-        """create_password_reset  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[CloudStorageRead], urllib3.HTTPResponse]:
+        """Method returns details of a specific cloud storage  # noqa: E501
 
-        Calls Django Auth PasswordResetForm save method.  Accepts the following POST parameters: email Returns the success/fail message.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_password_reset(password_reset_serializer_ex_request, _async_call=True)
+        >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            password_reset_serializer_ex_request (PasswordResetSerializerExRequest):
+            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -901,63 +1102,60 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (RestAuthDetail, HTTPResponse)
+            (CloudStorageRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['password_reset_serializer_ex_request'] = password_reset_serializer_ex_request
-        return self.create_password_reset_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.retrieve_endpoint.call_with_http_info(**kwargs)
 
-    def create_password_reset_confirm(
+    def retrieve_actions(
         self,
-        password_reset_confirm_request: PasswordResetConfirmRequest,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[RestAuthDetail], urllib3.HTTPResponse]:
-        """create_password_reset_confirm  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[str], urllib3.HTTPResponse]:
+        """Method returns allowed actions for the cloud storage  # noqa: E501
 
-        Password reset e-mail link is confirmed, therefore this resets the user's password.  Accepts the following POST parameters: token, uid,     new_password1, new_password2 Returns the success/fail message.  # noqa: E501
+        Method return allowed actions for cloud storage. It's required for reading/writing  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_password_reset_confirm(password_reset_confirm_request, _async_call=True)
+        >>> thread = api.retrieve_actions(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            password_reset_confirm_request (PasswordResetConfirmRequest):
+            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -983,62 +1181,61 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (RestAuthDetail, HTTPResponse)
+            (str, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['password_reset_confirm_request'] = password_reset_confirm_request
-        return self.create_password_reset_confirm_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.retrieve_actions_endpoint.call_with_http_info(**kwargs)
 
-    def create_register(
+    def retrieve_content(
         self,
-        register_serializer_ex_request: RegisterSerializerExRequest,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[RegisterSerializerEx], urllib3.HTTPResponse]:
-        """create_register  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[typing.List[str]], urllib3.HTTPResponse]:
+        """Method returns a manifest content  # noqa: E501
 
+        This method is deprecated and will be removed in version 2.6.0. Please use the new version of API: /cloudstorages/id/content-v2/  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_register(register_serializer_ex_request, _async_call=True)
+        >>> thread = api.retrieve_content(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            register_serializer_ex_request (RegisterSerializerExRequest):
+            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
+            manifest_path (str): Path to the manifest file in a cloud storage. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1064,63 +1261,63 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (RegisterSerializerEx, HTTPResponse)
+            ([str], HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['register_serializer_ex_request'] = register_serializer_ex_request
-        return self.create_register_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.retrieve_content_endpoint.call_with_http_info(**kwargs)
 
-    def create_signing(
+    def retrieve_content_v2(
         self,
-        signing_request: SigningRequest,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[str], urllib3.HTTPResponse]:
-        """This method signs URL for access to the server  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[CloudStorageContent], urllib3.HTTPResponse]:
+        """Method returns the content of the cloud storage  # noqa: E501
 
-        Signed URL contains a token which authenticates a user on the server.Signed URL is valid during 30 seconds since signing.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_signing(signing_request, _async_call=True)
+        >>> thread = api.retrieve_content_v2(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            signing_request (SigningRequest):
+            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
+            manifest_path (str): Path to the manifest file in a cloud storage. [optional]
+            next_token (str): Used to continue listing files in the bucket. [optional]
+            page_size (int): [optional]
+            prefix (str): Prefix to filter data. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1146,59 +1343,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (str, HTTPResponse)
+            (CloudStorageContent, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['signing_request'] = signing_request
-        return self.create_signing_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.retrieve_content_v2_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve_rules(
+    def retrieve_preview(
         self,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """retrieve_rules  # noqa: E501
+        """Method returns a preview image from a cloud storage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve_rules(_async_call=True)
+        >>> thread = api.retrieve_preview(id, _async_call=True)
         >>> result = thread.get()
 
+        Args:
+            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1238,9 +1435,88 @@
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        return self.retrieve_rules_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.retrieve_preview_endpoint.call_with_http_info(**kwargs)
+
+    def retrieve_status(
+        self,
+        id: int,
+        *,
+        _parse_response: bool = True,
+        _request_timeout: typing.Union[int, float, tuple] = None,
+        _validate_inputs: bool = True,
+        _validate_outputs: bool = True,
+        _check_status: bool = True,
+        _spec_property_naming: bool = False,
+        _content_type: typing.Optional[str] = None,
+        _host_index: typing.Optional[int] = None,
+        _request_auths: typing.Optional[typing.List] = None,
+        _async_call: bool = False,
+        **kwargs,
+    ) -> typing.Tuple[typing.Optional[str], urllib3.HTTPResponse]:
+        """Method returns a cloud storage status  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass _async_call=True
+
+        >>> thread = api.retrieve_status(id, _async_call=True)
+        >>> result = thread.get()
+
+        Args:
+            id (int): A unique integer value identifying this cloud storage.
+
+        Keyword Args:
+            _parse_response (bool): if False, the response data will not be parsed,
+                None is returned for data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _validate_inputs (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _validate_outputs (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _check_status (bool): whether to check response status
+                for being positive or not.
+                Default is True
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            _async_call (bool): execute request asynchronously
+
+        Returns:
+            (str, HTTPResponse)
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['_async_call'] = _async_call
+        kwargs['_parse_response'] = _parse_response
+        kwargs['_request_timeout'] = _request_timeout
+        kwargs['_validate_inputs'] = _validate_inputs
+        kwargs['_validate_outputs'] = _validate_outputs
+        kwargs['_check_status'] = _check_status
+        kwargs['_spec_property_naming'] = _spec_property_naming
+        kwargs['_content_type'] = _content_type
+        kwargs['_host_index'] = _host_index
+        kwargs['_request_auths'] = _request_auths
+        kwargs['id'] = id
+        return self.retrieve_status_endpoint.call_with_http_info(**kwargs)
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/cloudstorages_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/webhooks_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -21,130 +21,250 @@
 from cvat_sdk.api_client.api_client import ApiClient, Endpoint as _Endpoint
 from cvat_sdk.api_client.model_utils import (  # noqa: F401
     date,
     datetime,
     file_type,
     none_type,
 )
-from cvat_sdk.api_client.model.cloud_storage_read import CloudStorageRead
-from cvat_sdk.api_client.model.cloud_storage_write_request import CloudStorageWriteRequest
-from cvat_sdk.api_client.model.paginated_cloud_storage_read_list import PaginatedCloudStorageReadList
-from cvat_sdk.api_client.model.patched_cloud_storage_write_request import PatchedCloudStorageWriteRequest
+from cvat_sdk.api_client.model.events import Events
+from cvat_sdk.api_client.model.paginated_webhook_delivery_read_list import PaginatedWebhookDeliveryReadList
+from cvat_sdk.api_client.model.paginated_webhook_read_list import PaginatedWebhookReadList
+from cvat_sdk.api_client.model.patched_webhook_write_request import PatchedWebhookWriteRequest
+from cvat_sdk.api_client.model.webhook_delivery_read import WebhookDeliveryRead
+from cvat_sdk.api_client.model.webhook_read import WebhookRead
+from cvat_sdk.api_client.model.webhook_write_request import WebhookWriteRequest
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-class CloudstoragesApi(object):
+class WebhooksApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.create_endpoint = _Endpoint(
             settings={
-                'response_schema': (CloudStorageRead,),
+                'response_schema': (WebhookRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages',
+                'endpoint_path': '/api/webhooks',
                 'operation_id': 'create',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'cloud_storage_write_request',
+                    'webhook_write_request',
                     'x_organization',
                     'org',
                     'org_id',
                 ],
                 'required': [
-                    'cloud_storage_write_request',
+                    'webhook_write_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'cloud_storage_write_request':
-                        (CloudStorageWriteRequest,),
+                    'webhook_write_request':
+                        (WebhookWriteRequest,),
                     'x_organization':
                         (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'org': 'org',
                     'org_id': 'org_id',
                 },
                 'location_map': {
-                    'cloud_storage_write_request': 'body',
+                    'webhook_write_request': 'body',
                     'x_organization': 'header',
                     'org': 'query',
                     'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'multipart/form-data'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.create_deliveries_redelivery_endpoint = _Endpoint(
+            settings={
+                'response_schema': None,
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/webhooks/{id}/deliveries/{delivery_id}/redelivery',
+                'operation_id': 'create_deliveries_redelivery',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'delivery_id',
+                    'id',
+                ],
+                'required': [
+                    'delivery_id',
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'delivery_id',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('delivery_id',): {
+
+                        'regex': {
+                            'pattern': r'^\d+$',  # noqa: E501
+                        },
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'delivery_id':
+                        (str,),
+                    'id':
+                        (int,),
+                },
+                'attribute_map': {
+                    'delivery_id': 'delivery_id',
+                    'id': 'id',
+                },
+                'location_map': {
+                    'delivery_id': 'path',
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.create_ping_endpoint = _Endpoint(
+            settings={
+                'response_schema': (WebhookDeliveryRead,),
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/webhooks/{id}/ping',
+                'operation_id': 'create_ping',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (int,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages/{id}',
+                'endpoint_path': '/api/webhooks/{id}',
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -156,194 +276,167 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.list_endpoint = _Endpoint(
             settings={
-                'response_schema': (PaginatedCloudStorageReadList,),
+                'response_schema': (PaginatedWebhookReadList,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages',
+                'endpoint_path': '/api/webhooks',
                 'operation_id': 'list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'x_organization',
-                    'credentials_type',
                     'filter',
-                    'name',
                     'org',
                     'org_id',
                     'owner',
                     'page',
                     'page_size',
-                    'provider_type',
-                    'resource',
+                    'project_id',
                     'search',
                     'sort',
+                    'target_url',
+                    'type',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
-                    'credentials_type',
-                    'provider_type',
+                    'type',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('credentials_type',): {
-
-                        "KEY_SECRET_KEY_PAIR": "KEY_SECRET_KEY_PAIR",
-                        "ACCOUNT_NAME_TOKEN_PAIR": "ACCOUNT_NAME_TOKEN_PAIR",
-                        "KEY_FILE_PATH": "KEY_FILE_PATH",
-                        "ANONYMOUS_ACCESS": "ANONYMOUS_ACCESS",
-                        "CONNECTION_STRING": "CONNECTION_STRING"
-                    },
-                    ('provider_type',): {
+                    ('type',): {
 
-                        "AWS_S3_BUCKET": "AWS_S3_BUCKET",
-                        "AZURE_CONTAINER": "AZURE_CONTAINER",
-                        "GOOGLE_DRIVE": "GOOGLE_DRIVE",
-                        "GOOGLE_CLOUD_STORAGE": "GOOGLE_CLOUD_STORAGE"
+                        "ORGANIZATION": "organization",
+                        "PROJECT": "project"
                     },
                 },
                 'openapi_types': {
                     'x_organization':
                         (str,),
-                    'credentials_type':
-                        (str,),
                     'filter':
                         (str,),
-                    'name':
-                        (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
                     'owner':
                         (str,),
                     'page':
                         (int,),
                     'page_size':
                         (int,),
-                    'provider_type':
-                        (str,),
-                    'resource':
-                        (str,),
+                    'project_id':
+                        (int,),
                     'search':
                         (str,),
                     'sort':
                         (str,),
+                    'target_url':
+                        (str,),
+                    'type':
+                        (str,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
-                    'credentials_type': 'credentials_type',
                     'filter': 'filter',
-                    'name': 'name',
                     'org': 'org',
                     'org_id': 'org_id',
                     'owner': 'owner',
                     'page': 'page',
                     'page_size': 'page_size',
-                    'provider_type': 'provider_type',
-                    'resource': 'resource',
+                    'project_id': 'project_id',
                     'search': 'search',
                     'sort': 'sort',
+                    'target_url': 'target_url',
+                    'type': 'type',
                 },
                 'location_map': {
                     'x_organization': 'header',
-                    'credentials_type': 'query',
                     'filter': 'query',
-                    'name': 'query',
                     'org': 'query',
                     'org_id': 'query',
                     'owner': 'query',
                     'page': 'query',
                     'page_size': 'query',
-                    'provider_type': 'query',
-                    'resource': 'query',
+                    'project_id': 'query',
                     'search': 'query',
                     'sort': 'query',
+                    'target_url': 'query',
+                    'type': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.partial_update_endpoint = _Endpoint(
+        self.list_deliveries_endpoint = _Endpoint(
             settings={
-                'response_schema': (CloudStorageRead,),
+                'response_schema': (PaginatedWebhookDeliveryReadList,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages/{id}',
-                'operation_id': 'partial_update',
-                'http_method': 'PATCH',
+                'endpoint_path': '/api/webhooks/{id}/deliveries',
+                'operation_id': 'list_deliveries',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'patched_cloud_storage_write_request',
+                    'filter',
+                    'page',
+                    'page_size',
+                    'search',
+                    'sort',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -355,71 +448,71 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
+                    'filter':
                         (str,),
-                    'org_id':
+                    'page':
+                        (int,),
+                    'page_size':
                         (int,),
-                    'patched_cloud_storage_write_request':
-                        (PatchedCloudStorageWriteRequest,),
+                    'search':
+                        (str,),
+                    'sort':
+                        (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'filter': 'filter',
+                    'page': 'page',
+                    'page_size': 'page_size',
+                    'search': 'search',
+                    'sort': 'sort',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'patched_cloud_storage_write_request': 'body',
+                    'filter': 'query',
+                    'page': 'query',
+                    'page_size': 'query',
+                    'search': 'query',
+                    'sort': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
-                'content_type': [
-                    'application/json',
-                    'multipart/form-data'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.retrieve_endpoint = _Endpoint(
+        self.partial_update_endpoint = _Endpoint(
             settings={
-                'response_schema': (CloudStorageRead,),
+                'response_schema': (WebhookRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages/{id}',
-                'operation_id': 'retrieve',
-                'http_method': 'GET',
+                'endpoint_path': '/api/webhooks/{id}',
+                'operation_id': 'partial_update',
+                'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'patched_webhook_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -431,65 +524,55 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
+                    'patched_webhook_write_request':
+                        (PatchedWebhookWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'patched_webhook_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.retrieve_actions_endpoint = _Endpoint(
+        self.retrieve_endpoint = _Endpoint(
             settings={
-                'response_schema': (str,),
+                'response_schema': (WebhookRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages/{id}/actions',
-                'operation_id': 'retrieve_actions',
+                'endpoint_path': '/api/webhooks/{id}',
+                'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -501,211 +584,176 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.retrieve_content_endpoint = _Endpoint(
+        self.retrieve_deliveries_endpoint = _Endpoint(
             settings={
-                'response_schema': ([str],),
+                'response_schema': (WebhookDeliveryRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages/{id}/content',
-                'operation_id': 'retrieve_content',
+                'endpoint_path': '/api/webhooks/{id}/deliveries/{delivery_id}',
+                'operation_id': 'retrieve_deliveries',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'delivery_id',
                     'id',
-                    'x_organization',
-                    'manifest_path',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
+                    'delivery_id',
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
+                    'delivery_id',
                 ]
             },
             root_map={
                 'validations': {
+                    ('delivery_id',): {
+
+                        'regex': {
+                            'pattern': r'^\d+$',  # noqa: E501
+                        },
+                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id':
-                        (int,),
-                    'x_organization':
+                    'delivery_id':
                         (str,),
-                    'manifest_path':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
+                    'id':
                         (int,),
                 },
                 'attribute_map': {
+                    'delivery_id': 'delivery_id',
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'manifest_path': 'manifest_path',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
+                    'delivery_id': 'path',
                     'id': 'path',
-                    'x_organization': 'header',
-                    'manifest_path': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.retrieve_preview_endpoint = _Endpoint(
+        self.retrieve_events_endpoint = _Endpoint(
             settings={
-                'response_schema': None,
+                'response_schema': (Events,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages/{id}/preview',
-                'operation_id': 'retrieve_preview',
+                'endpoint_path': '/api/webhooks/events',
+                'operation_id': 'retrieve_events',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                ],
-                'required': [
-                    'id',
+                    'type',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id':
-                        (int,),
-                    'x_organization':
+                    'type':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
-                    'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'type': 'type',
                 },
                 'location_map': {
-                    'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'type': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.retrieve_status_endpoint = _Endpoint(
+        self.update_endpoint = _Endpoint(
             settings={
-                'response_schema': (str,),
+                'response_schema': (WebhookRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/cloudstorages/{id}/status',
-                'operation_id': 'retrieve_status',
-                'http_method': 'GET',
+                'endpoint_path': '/api/webhooks/{id}',
+                'operation_id': 'update',
+                'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
+                    'webhook_write_request',
                 ],
                 'required': [
                     'id',
+                    'webhook_write_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -714,71 +762,64 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
+                    'webhook_write_request':
+                        (WebhookWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'webhook_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
 
     def create(
         self,
-        cloud_storage_write_request: CloudStorageWriteRequest,
+        webhook_write_request: WebhookWriteRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[CloudStorageRead], urllib3.HTTPResponse]:
-        """Method creates a cloud storage with a specified characteristics  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[WebhookRead], urllib3.HTTPResponse]:
+        """Method creates a webhook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create(cloud_storage_write_request, _async_call=True)
+        >>> thread = api.create(webhook_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            cloud_storage_write_request (CloudStorageWriteRequest):
+            webhook_write_request (WebhookWriteRequest):
 
         Keyword Args:
             x_organization (str): [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
@@ -809,31 +850,190 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (CloudStorageRead, HTTPResponse)
+            (WebhookRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['cloud_storage_write_request'] = cloud_storage_write_request
+        kwargs['webhook_write_request'] = webhook_write_request
         return self.create_endpoint.call_with_http_info(**kwargs)
 
+    def create_deliveries_redelivery(
+        self,
+        delivery_id: str,
+        id: int,
+        *,
+        _parse_response: bool = True,
+        _request_timeout: typing.Union[int, float, tuple] = None,
+        _validate_inputs: bool = True,
+        _validate_outputs: bool = True,
+        _check_status: bool = True,
+        _spec_property_naming: bool = False,
+        _content_type: typing.Optional[str] = None,
+        _host_index: typing.Optional[int] = None,
+        _request_auths: typing.Optional[typing.List] = None,
+        _async_call: bool = False,
+        **kwargs,
+    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+        """Method redeliver a specific webhook delivery  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass _async_call=True
+
+        >>> thread = api.create_deliveries_redelivery(delivery_id, id, _async_call=True)
+        >>> result = thread.get()
+
+        Args:
+            delivery_id (str):
+            id (int): A unique integer value identifying this webhook.
+
+        Keyword Args:
+            _parse_response (bool): if False, the response data will not be parsed,
+                None is returned for data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _validate_inputs (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _validate_outputs (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _check_status (bool): whether to check response status
+                for being positive or not.
+                Default is True
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            _async_call (bool): execute request asynchronously
+
+        Returns:
+            (None, HTTPResponse)
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['_async_call'] = _async_call
+        kwargs['_parse_response'] = _parse_response
+        kwargs['_request_timeout'] = _request_timeout
+        kwargs['_validate_inputs'] = _validate_inputs
+        kwargs['_validate_outputs'] = _validate_outputs
+        kwargs['_check_status'] = _check_status
+        kwargs['_spec_property_naming'] = _spec_property_naming
+        kwargs['_content_type'] = _content_type
+        kwargs['_host_index'] = _host_index
+        kwargs['_request_auths'] = _request_auths
+        kwargs['delivery_id'] = delivery_id
+        kwargs['id'] = id
+        return self.create_deliveries_redelivery_endpoint.call_with_http_info(**kwargs)
+
+    def create_ping(
+        self,
+        id: int,
+        *,
+        _parse_response: bool = True,
+        _request_timeout: typing.Union[int, float, tuple] = None,
+        _validate_inputs: bool = True,
+        _validate_outputs: bool = True,
+        _check_status: bool = True,
+        _spec_property_naming: bool = False,
+        _content_type: typing.Optional[str] = None,
+        _host_index: typing.Optional[int] = None,
+        _request_auths: typing.Optional[typing.List] = None,
+        _async_call: bool = False,
+        **kwargs,
+    ) -> typing.Tuple[typing.Optional[WebhookDeliveryRead], urllib3.HTTPResponse]:
+        """Method send ping webhook  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass _async_call=True
+
+        >>> thread = api.create_ping(id, _async_call=True)
+        >>> result = thread.get()
+
+        Args:
+            id (int): A unique integer value identifying this webhook.
+
+        Keyword Args:
+            _parse_response (bool): if False, the response data will not be parsed,
+                None is returned for data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _validate_inputs (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _validate_outputs (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _check_status (bool): whether to check response status
+                for being positive or not.
+                Default is True
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            _async_call (bool): execute request asynchronously
+
+        Returns:
+            (WebhookDeliveryRead, HTTPResponse)
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['_async_call'] = _async_call
+        kwargs['_parse_response'] = _parse_response
+        kwargs['_request_timeout'] = _request_timeout
+        kwargs['_validate_inputs'] = _validate_inputs
+        kwargs['_validate_outputs'] = _validate_outputs
+        kwargs['_check_status'] = _check_status
+        kwargs['_spec_property_naming'] = _spec_property_naming
+        kwargs['_content_type'] = _content_type
+        kwargs['_host_index'] = _host_index
+        kwargs['_request_auths'] = _request_auths
+        kwargs['id'] = id
+        return self.create_ping_endpoint.call_with_http_info(**kwargs)
+
     def destroy(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
@@ -842,29 +1042,26 @@
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method deletes a specific cloud storage  # noqa: E501
+        """Method deletes a webhook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this cloud storage.
+            id (int): A unique integer value identifying this webhook.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -921,38 +1118,37 @@
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[PaginatedCloudStorageReadList], urllib3.HTTPResponse]:
-        """Returns a paginated list of storages  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[PaginatedWebhookReadList], urllib3.HTTPResponse]:
+        """Method returns a paginated list of webhook according to query parameters  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
-            credentials_type (str): A simple equality filter for the credentials_type field. [optional]
-            filter (str): A filter term. Available filter_fields: ['provider_type', 'name', 'resource', 'credentials_type', 'owner', 'description', 'id']. [optional]
-            name (str): A simple equality filter for the name field. [optional]
+            x_organization (str): Organization unique slug. [optional]
+            filter (str): A filter term. Available filter_fields: ['target_url', 'owner', 'type', 'description', 'id', 'project_id', 'updated_date']. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             owner (str): A simple equality filter for the owner field. [optional]
             page (int): A page number within the paginated result set.. [optional]
             page_size (int): Number of results to return per page.. [optional]
-            provider_type (str): A simple equality filter for the provider_type field. [optional]
-            resource (str): A simple equality filter for the resource field. [optional]
-            search (str): A search term. Available search_fields: ('provider_type', 'name', 'resource', 'credentials_type', 'owner', 'description'). [optional]
-            sort (str): Which field to use when ordering the results. Available ordering_fields: ['provider_type', 'name', 'resource', 'credentials_type', 'owner', 'description', 'id']. [optional]
+            project_id (int): A simple equality filter for the project_id field. [optional]
+            search (str): A search term. Available search_fields: ('target_url', 'owner', 'type', 'description'). [optional]
+            sort (str): Which field to use when ordering the results. Available ordering_fields: ['target_url', 'owner', 'type', 'description', 'id', 'project_id', 'updated_date']. [optional]
+            target_url (str): A simple equality filter for the target_url field. [optional]
+            type (str): A simple equality filter for the type field. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -978,15 +1174,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (PaginatedCloudStorageReadList, HTTPResponse)
+            (PaginatedWebhookReadList, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
@@ -994,46 +1190,47 @@
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         return self.list_endpoint.call_with_http_info(**kwargs)
 
-    def partial_update(
+    def list_deliveries(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[CloudStorageRead], urllib3.HTTPResponse]:
-        """Methods does a partial update of chosen fields in a cloud storage instance  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[PaginatedWebhookDeliveryReadList], urllib3.HTTPResponse]:
+        """Method return a list of deliveries for a specific webhook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.partial_update(id, _async_call=True)
+        >>> thread = api.list_deliveries(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this cloud storage.
+            id (int): A unique integer value identifying this webhook.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            patched_cloud_storage_write_request (PatchedCloudStorageWriteRequest): [optional]
+            filter (str): A filter term. Available filter_fields: None. [optional]
+            page (int): A page number within the paginated result set.. [optional]
+            page_size (int): Number of results to return per page.. [optional]
+            search (str): A search term. Available search_fields: None. [optional]
+            sort (str): Which field to use when ordering the results. Available ordering_fields: None. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1059,62 +1256,60 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (CloudStorageRead, HTTPResponse)
+            (PaginatedWebhookDeliveryReadList, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        return self.partial_update_endpoint.call_with_http_info(**kwargs)
+        return self.list_deliveries_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve(
+    def partial_update(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[CloudStorageRead], urllib3.HTTPResponse]:
-        """Method returns details of a specific cloud storage  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[WebhookRead], urllib3.HTTPResponse]:
+        """Methods does a partial update of chosen fields in a webhook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve(id, _async_call=True)
+        >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this cloud storage.
+            id (int): A unique integer value identifying this webhook.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
+            patched_webhook_write_request (PatchedWebhookWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1140,63 +1335,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (CloudStorageRead, HTTPResponse)
+            (WebhookRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        return self.retrieve_endpoint.call_with_http_info(**kwargs)
+        return self.partial_update_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve_actions(
+    def retrieve(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[str], urllib3.HTTPResponse]:
-        """Method returns allowed actions for the cloud storage  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[WebhookRead], urllib3.HTTPResponse]:
+        """Method returns details of a webhook  # noqa: E501
 
-        Method return allowed actions for cloud storage. It's required for reading/writing  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve_actions(id, _async_call=True)
+        >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this cloud storage.
+            id (int): A unique integer value identifying this webhook.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1222,63 +1413,61 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (str, HTTPResponse)
+            (WebhookRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        return self.retrieve_actions_endpoint.call_with_http_info(**kwargs)
+        return self.retrieve_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve_content(
+    def retrieve_deliveries(
         self,
+        delivery_id: str,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[typing.List[str]], urllib3.HTTPResponse]:
-        """Method returns a manifest content  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[WebhookDeliveryRead], urllib3.HTTPResponse]:
+        """Method return a specific delivery for a specific webhook  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve_content(id, _async_call=True)
+        >>> thread = api.retrieve_deliveries(delivery_id, id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this cloud storage.
+            delivery_id (str):
+            id (int): A unique integer value identifying this webhook.
 
         Keyword Args:
-            x_organization (str): [optional]
-            manifest_path (str): Path to the manifest file in a cloud storage. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1304,62 +1493,58 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            ([str], HTTPResponse)
+            (WebhookDeliveryRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
+        kwargs['delivery_id'] = delivery_id
         kwargs['id'] = id
-        return self.retrieve_content_endpoint.call_with_http_info(**kwargs)
+        return self.retrieve_deliveries_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve_preview(
+    def retrieve_events(
         self,
-        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method returns a preview image from a cloud storage  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[Events], urllib3.HTTPResponse]:
+        """Method return a list of available webhook events  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve_preview(id, _async_call=True)
+        >>> thread = api.retrieve_events(_async_call=True)
         >>> result = thread.get()
 
-        Args:
-            id (int): A unique integer value identifying this cloud storage.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
+            type (str): Type of webhook. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1385,62 +1570,60 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (None, HTTPResponse)
+            (Events, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['id'] = id
-        return self.retrieve_preview_endpoint.call_with_http_info(**kwargs)
+        return self.retrieve_events_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve_status(
+    def update(
         self,
         id: int,
+        webhook_write_request: WebhookWriteRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[str], urllib3.HTTPResponse]:
-        """Method returns a cloud storage status  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[WebhookRead], urllib3.HTTPResponse]:
+        """Method updates a webhook by id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve_status(id, _async_call=True)
+        >>> thread = api.update(id, webhook_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this cloud storage.
+            id (int): A unique integer value identifying this webhook.
+            webhook_write_request (WebhookWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1466,24 +1649,25 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (str, HTTPResponse)
+            (WebhookRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        return self.retrieve_status_endpoint.call_with_http_info(**kwargs)
+        kwargs['webhook_write_request'] = webhook_write_request
+        return self.update_endpoint.call_with_http_info(**kwargs)
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/comments_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/comments_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -133,17 +133,14 @@
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -155,32 +152,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -309,17 +294,14 @@
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_comment_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -332,34 +314,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_comment_write_request':
                         (PatchedCommentWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_comment_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -385,17 +355,14 @@
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -407,32 +374,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -547,17 +502,14 @@
         >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this comment.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -625,15 +577,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             filter (str): A filter term. Available filter_fields: ['owner', 'id', 'issue_id', 'frame_id', 'job_id']. [optional]
             frame_id (int): A simple equality filter for the frame_id field. [optional]
             issue_id (int): A simple equality filter for the issue_id field. [optional]
             job_id (int): A simple equality filter for the job_id field. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             owner (str): A simple equality filter for the owner field. [optional]
@@ -714,17 +666,14 @@
         >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this comment.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_comment_write_request (PatchedCommentWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -796,17 +745,14 @@
         >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this comment.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/events_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/events_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -130,20 +130,18 @@
                 'endpoint_path': '/api/events',
                 'operation_id': 'list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
                     'action',
                     'filename',
                     '_from',
                     'job_id',
-                    'org',
                     'org_id',
                     'project_id',
                     'query_id',
                     'task_id',
                     'to',
                     'user_id',
                 ],
@@ -162,60 +160,52 @@
                 'allowed_values': {
                     ('action',): {
 
                         "DOWNLOAD": "download"
                     },
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'filename':
                         (str,),
                     '_from':
                         (datetime,),
                     'job_id':
                         (int,),
-                    'org':
-                        (str,),
                     'org_id':
                         (int,),
                     'project_id':
                         (int,),
                     'query_id':
                         (str,),
                     'task_id':
                         (int,),
                     'to':
                         (datetime,),
                     'user_id':
                         (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'filename': 'filename',
                     '_from': 'from',
                     'job_id': 'job_id',
-                    'org': 'org',
                     'org_id': 'org_id',
                     'project_id': 'project_id',
                     'query_id': 'query_id',
                     'task_id': 'task_id',
                     'to': 'to',
                     'user_id': 'user_id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
                     'action': 'query',
                     'filename': 'query',
                     '_from': 'query',
                     'job_id': 'query',
-                    'org': 'query',
                     'org_id': 'query',
                     'project_id': 'query',
                     'query_id': 'query',
                     'task_id': 'query',
                     'to': 'query',
                     'user_id': 'query',
                 },
@@ -333,20 +323,18 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after annotation file had been created. [optional] if omitted the server will use the default value of "download"
             filename (str): Desired output file name. [optional]
             _from (datetime): Filter events after the datetime. If no 'from' or 'to' parameters are passed, the last 30 days will be set.. [optional]
             job_id (int): Filter events by job ID. [optional]
-            org (str): Organization unique slug. [optional]
             org_id (int): Filter events by organization ID. [optional]
             project_id (int): Filter events by project ID. [optional]
             query_id (str): ID of query request that need to check or download. [optional]
             task_id (int): Filter events by task ID. [optional]
             to (datetime): Filter events before the datetime. If no 'from' or 'to' parameters are passed, the last 30 days will be set.. [optional]
             user_id (int): Filter events by user ID. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/invitations_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/invitations_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -133,17 +133,14 @@
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'key',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'key',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -155,32 +152,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'key':
                         (str,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'key': 'key',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'key': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -294,17 +279,14 @@
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'key',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_invitation_write_request',
                 ],
                 'required': [
                     'key',
                 ],
                 'nullable': [
                 ],
@@ -317,34 +299,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'key':
                         (str,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_invitation_write_request':
                         (PatchedInvitationWriteRequest,),
                 },
                 'attribute_map': {
                     'key': 'key',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'key': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_invitation_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -370,17 +340,14 @@
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'key',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'key',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -392,32 +359,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'key':
                         (str,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'key': 'key',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'key': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -532,17 +487,14 @@
         >>> thread = api.destroy(key, _async_call=True)
         >>> result = thread.get()
 
         Args:
             key (str): A unique value identifying this invitation.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -610,15 +562,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             filter (str): A filter term. Available filter_fields: ['owner']. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             owner (str): A simple equality filter for the owner field. [optional]
             page (int): A page number within the paginated result set.. [optional]
             page_size (int): Number of results to return per page.. [optional]
             search (str): A search term. Available search_fields: ('owner',). [optional]
@@ -696,17 +648,14 @@
         >>> thread = api.partial_update(key, _async_call=True)
         >>> result = thread.get()
 
         Args:
             key (str): A unique value identifying this invitation.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_invitation_write_request (PatchedInvitationWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -778,17 +727,14 @@
         >>> thread = api.retrieve(key, _async_call=True)
         >>> result = thread.get()
 
         Args:
             key (str): A unique value identifying this invitation.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/issues_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/users_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -21,129 +21,54 @@
 from cvat_sdk.api_client.api_client import ApiClient, Endpoint as _Endpoint
 from cvat_sdk.api_client.model_utils import (  # noqa: F401
     date,
     datetime,
     file_type,
     none_type,
 )
-from cvat_sdk.api_client.model.issue_read import IssueRead
-from cvat_sdk.api_client.model.issue_write_request import IssueWriteRequest
-from cvat_sdk.api_client.model.paginated_issue_read_list import PaginatedIssueReadList
-from cvat_sdk.api_client.model.patched_issue_write_request import PatchedIssueWriteRequest
+from cvat_sdk.api_client.model.meta_user import MetaUser
+from cvat_sdk.api_client.model.paginated_meta_user_list import PaginatedMetaUserList
+from cvat_sdk.api_client.model.patched_user_request import PatchedUserRequest
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-class IssuesApi(object):
+class UsersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_endpoint = _Endpoint(
-            settings={
-                'response_schema': (IssueRead,),
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/issues',
-                'operation_id': 'create',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'issue_write_request',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                ],
-                'required': [
-                    'issue_write_request',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'issue_write_request':
-                        (IssueWriteRequest,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'issue_write_request': 'body',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/vnd.cvat+json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/issues/{id}',
+                'endpoint_path': '/api/users/{id}',
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -155,73 +80,59 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.list_endpoint = _Endpoint(
             settings={
-                'response_schema': (PaginatedIssueReadList,),
+                'response_schema': (PaginatedMetaUserList,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/issues',
+                'endpoint_path': '/api/users',
                 'operation_id': 'list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'x_organization',
-                    'assignee',
                     'filter',
-                    'frame_id',
-                    'job_id',
+                    'first_name',
+                    'is_active',
+                    'last_name',
                     'org',
                     'org_id',
-                    'owner',
                     'page',
                     'page_size',
-                    'resolved',
                     'search',
                     'sort',
-                    'task_id',
+                    'username',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -231,106 +142,95 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'x_organization':
                         (str,),
-                    'assignee':
-                        (str,),
                     'filter':
                         (str,),
-                    'frame_id':
-                        (int,),
-                    'job_id':
-                        (int,),
+                    'first_name':
+                        (str,),
+                    'is_active':
+                        (bool,),
+                    'last_name':
+                        (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
-                    'owner':
-                        (str,),
                     'page':
                         (int,),
                     'page_size':
                         (int,),
-                    'resolved':
-                        (bool,),
                     'search':
                         (str,),
                     'sort':
                         (str,),
-                    'task_id':
-                        (int,),
+                    'username':
+                        (str,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
-                    'assignee': 'assignee',
                     'filter': 'filter',
-                    'frame_id': 'frame_id',
-                    'job_id': 'job_id',
+                    'first_name': 'first_name',
+                    'is_active': 'is_active',
+                    'last_name': 'last_name',
                     'org': 'org',
                     'org_id': 'org_id',
-                    'owner': 'owner',
                     'page': 'page',
                     'page_size': 'page_size',
-                    'resolved': 'resolved',
                     'search': 'search',
                     'sort': 'sort',
-                    'task_id': 'task_id',
+                    'username': 'username',
                 },
                 'location_map': {
                     'x_organization': 'header',
-                    'assignee': 'query',
                     'filter': 'query',
-                    'frame_id': 'query',
-                    'job_id': 'query',
+                    'first_name': 'query',
+                    'is_active': 'query',
+                    'last_name': 'query',
                     'org': 'query',
                     'org_id': 'query',
-                    'owner': 'query',
                     'page': 'query',
                     'page_size': 'query',
-                    'resolved': 'query',
                     'search': 'query',
                     'sort': 'query',
-                    'task_id': 'query',
+                    'username': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.partial_update_endpoint = _Endpoint(
             settings={
-                'response_schema': (IssueRead,),
+                'response_schema': (MetaUser,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/issues/{id}',
+                'endpoint_path': '/api/users/{id}',
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'patched_issue_write_request',
+                    'patched_user_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -342,35 +242,23 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'patched_issue_write_request':
-                        (PatchedIssueWriteRequest,),
+                    'patched_user_request':
+                        (PatchedUserRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'patched_issue_write_request': 'body',
+                    'patched_user_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -379,33 +267,30 @@
                     'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
-                'response_schema': (IssueRead,),
+                'response_schema': (MetaUser,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/issues/{id}',
+                'endpoint_path': '/api/users/{id}',
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -417,76 +302,109 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.retrieve_self_endpoint = _Endpoint(
+            settings={
+                'response_schema': (MetaUser,),
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/users/self',
+                'operation_id': 'retrieve_self',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def create(
+    def destroy(
         self,
-        issue_write_request: IssueWriteRequest,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[IssueRead], urllib3.HTTPResponse]:
-        """Method creates an issue  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+        """Method deletes a specific user from the server  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create(issue_write_request, _async_call=True)
+        >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            issue_write_request (IssueWriteRequest):
+            id (int): A unique integer value identifying this user.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -512,62 +430,68 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (IssueRead, HTTPResponse)
+            (None, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['issue_write_request'] = issue_write_request
-        return self.create_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.destroy_endpoint.call_with_http_info(**kwargs)
 
-    def destroy(
+    def list(
         self,
-        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method deletes an issue  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[PaginatedMetaUserList], urllib3.HTTPResponse]:
+        """Method returns a paginated list of users  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.destroy(id, _async_call=True)
+        >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
-        Args:
-            id (int): A unique integer value identifying this issue.
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
+            filter (str): A filter term. Available filter_fields: ['username', 'first_name', 'last_name', 'id', 'is_active']. [optional]
+            first_name (str): A simple equality filter for the first_name field. [optional]
+            is_active (bool): A simple equality filter for the is_active field. [optional]
+            last_name (str): A simple equality filter for the last_name field. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
+            page (int): A page number within the paginated result set.. [optional]
+            page_size (int): Number of results to return per page.. [optional]
+            search (str): A search term. Available search_fields: ('username', 'first_name', 'last_name'). [optional]
+            sort (str): Which field to use when ordering the results. Available ordering_fields: ['username', 'first_name', 'last_name', 'id', 'is_active']. [optional]
+            username (str): A simple equality filter for the username field. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -593,70 +517,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (None, HTTPResponse)
+            (PaginatedMetaUserList, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['id'] = id
-        return self.destroy_endpoint.call_with_http_info(**kwargs)
+        return self.list_endpoint.call_with_http_info(**kwargs)
 
-    def list(
+    def partial_update(
         self,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[PaginatedIssueReadList], urllib3.HTTPResponse]:
-        """Method returns a paginated list of issues  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[MetaUser], urllib3.HTTPResponse]:
+        """Method updates chosen fields of a user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.list(_async_call=True)
+        >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
+        Args:
+            id (int): A unique integer value identifying this user.
 
         Keyword Args:
-            x_organization (str): [optional]
-            assignee (str): A simple equality filter for the assignee field. [optional]
-            filter (str): A filter term. Available filter_fields: ['owner', 'assignee', 'id', 'job_id', 'task_id', 'resolved', 'frame_id']. [optional]
-            frame_id (int): A simple equality filter for the frame_id field. [optional]
-            job_id (int): A simple equality filter for the job_id field. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            owner (str): A simple equality filter for the owner field. [optional]
-            page (int): A page number within the paginated result set.. [optional]
-            page_size (int): Number of results to return per page.. [optional]
-            resolved (bool): A simple equality filter for the resolved field. [optional]
-            search (str): A search term. Available search_fields: ('owner', 'assignee'). [optional]
-            sort (str): Which field to use when ordering the results. Available ordering_fields: ['owner', 'assignee', 'id', 'job_id', 'task_id', 'resolved', 'frame_id']. [optional]
-            task_id (int): A simple equality filter for the task_id field. [optional]
+            patched_user_request (PatchedUserRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -682,62 +595,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (PaginatedIssueReadList, HTTPResponse)
+            (MetaUser, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        return self.list_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.partial_update_endpoint.call_with_http_info(**kwargs)
 
-    def partial_update(
+    def retrieve(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[IssueRead], urllib3.HTTPResponse]:
-        """Methods does a partial update of chosen fields in an issue  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[MetaUser], urllib3.HTTPResponse]:
+        """Method provides information of a specific user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.partial_update(id, _async_call=True)
+        >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this issue.
+            id (int): A unique integer value identifying this user.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            patched_issue_write_request (PatchedIssueWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -763,62 +673,57 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (IssueRead, HTTPResponse)
+            (MetaUser, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        return self.partial_update_endpoint.call_with_http_info(**kwargs)
+        return self.retrieve_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve(
+    def retrieve_self(
         self,
-        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[IssueRead], urllib3.HTTPResponse]:
-        """Method returns details of an issue  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[MetaUser], urllib3.HTTPResponse]:
+        """Method returns an instance of a user who is currently authorized  # noqa: E501
 
+        Method returns an instance of a user who is currently authorized  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve(id, _async_call=True)
+        >>> thread = api.retrieve_self(_async_call=True)
         >>> result = thread.get()
 
-        Args:
-            id (int): A unique integer value identifying this issue.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -844,24 +749,23 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (IssueRead, HTTPResponse)
+            (MetaUser, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['id'] = id
-        return self.retrieve_endpoint.call_with_http_info(**kwargs)
+        return self.retrieve_self_endpoint.call_with_http_info(**kwargs)
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/jobs_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/jobs_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -67,21 +67,18 @@
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                     'annotation_file_request',
-                    'x_organization',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'id',
                     'annotation_file_request',
                 ],
                 'nullable': [
@@ -103,52 +100,40 @@
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
                     'annotation_file_request':
                         (AnnotationFileRequest,),
-                    'x_organization':
-                        (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
                     'annotation_file_request': 'body',
-                    'x_organization': 'header',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -173,17 +158,14 @@
                 'operation_id': 'destroy_annotations',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -195,32 +177,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -390,17 +360,14 @@
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_job_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -413,34 +380,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_job_write_request':
                         (PatchedJobWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_job_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -467,17 +422,14 @@
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'action',
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_labeled_data_request',
                 ],
                 'required': [
                     'action',
                     'id',
                 ],
                 'nullable': [
@@ -500,36 +452,24 @@
                     },
                 },
                 'openapi_types': {
                     'action':
                         (str,),
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_labeled_data_request':
                         (PatchedLabeledDataRequest,),
                 },
                 'attribute_map': {
                     'action': 'action',
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'action': 'query',
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_labeled_data_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -554,17 +494,14 @@
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -576,32 +513,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -624,22 +549,19 @@
                 'operation_id': 'retrieve_annotations',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -663,55 +585,43 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -735,18 +645,15 @@
                 'operation_id': 'retrieve_data',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'number',
-                    'org',
-                    'org_id',
                     'quality',
                     'type',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
@@ -773,42 +680,30 @@
                         "CONTEXT_IMAGE": "context_image",
                         "FRAME": "frame"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'number':
                         (int,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'quality':
                         (str,),
                     'type':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'number': 'number',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'quality': 'quality',
                     'type': 'type',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'number': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'quality': 'query',
                     'type': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -833,17 +728,14 @@
                 'operation_id': 'retrieve_data_meta',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -855,32 +747,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -904,21 +784,18 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'format',
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'format',
                     'id',
                 ],
                 'nullable': [
@@ -945,53 +822,41 @@
                     },
                 },
                 'openapi_types': {
                     'format':
                         (str,),
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'format': 'format',
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'format': 'query',
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -1015,17 +880,14 @@
                 'operation_id': 'retrieve_preview',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -1037,32 +899,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -1083,18 +933,15 @@
                 'operation_id': 'update_annotations',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'format',
-                    'org',
-                    'org_id',
                     'job_annotations_update_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -1107,38 +954,26 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'format':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'job_annotations_update_request':
                         (JobAnnotationsUpdateRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'format': 'format',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'format': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'job_annotations_update_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -1176,21 +1011,18 @@
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
             annotation_file_request (AnnotationFileRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Annotation file name. [optional]
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): where to import the annotation from. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in the task to import annotation. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1263,17 +1095,14 @@
         >>> thread = api.destroy_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1341,15 +1170,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             assignee (str): A simple equality filter for the assignee field. [optional]
             dimension (str): A simple equality filter for the dimension field. [optional]
             filter (str): A filter term. Available filter_fields: ['task_name', 'project_name', 'assignee', 'state', 'stage', 'id', 'task_id', 'project_id', 'updated_date', 'dimension']. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             page (int): A page number within the paginated result set.. [optional]
             page_size (int): Number of results to return per page.. [optional]
@@ -1434,17 +1263,14 @@
         >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_job_write_request (PatchedJobWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1518,17 +1344,14 @@
         >>> result = thread.get()
 
         Args:
             action (str):
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_labeled_data_request (PatchedLabeledDataRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1601,17 +1424,14 @@
         >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1682,22 +1502,19 @@
         >>> thread = api.retrieve_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after annotation file had been created. [optional] if omitted the server will use the default value of "download"
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Desired output file name. [optional]
             format (str): Desired output format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): Where need to save downloaded annotation. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in the task to export annotation. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1769,18 +1586,15 @@
         >>> thread = api.retrieve_data(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
             number (int): A unique number value identifying chunk or frame. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             quality (str): Specifies the quality level of the requested data. [optional]
             type (str): Specifies the type of the requested data. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1853,17 +1667,14 @@
         >>> thread = api.retrieve_data_meta(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1936,21 +1747,18 @@
         >>> result = thread.get()
 
         Args:
             format (str): Desired output format name You can get the list of supported formats at: /server/annotation/formats
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after annotation file had been created. [optional] if omitted the server will use the default value of "download"
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Desired output file name. [optional]
             location (str): Where need to save downloaded dataset. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in the task to export dataset. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -2023,17 +1831,14 @@
         >>> thread = api.retrieve_preview(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -2104,18 +1909,15 @@
         >>> thread = api.update_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             job_annotations_update_request (JobAnnotationsUpdateRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/labels_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/labels_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -61,17 +61,14 @@
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -83,32 +80,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -271,17 +256,14 @@
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_label_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -294,34 +276,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_label_request':
                         (PatchedLabelRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_label_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -347,17 +317,14 @@
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -369,32 +336,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -428,17 +383,14 @@
         >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this label.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -599,17 +551,14 @@
         >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this label.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_label_request (PatchedLabelRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -681,17 +630,14 @@
         >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this label.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/lambda_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/lambda_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -59,17 +59,14 @@
                 'operation_id': 'create_functions',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'func_id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'online_function_call_request',
                 ],
                 'required': [
                     'func_id',
                 ],
                 'nullable': [
                 ],
@@ -89,34 +86,22 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'func_id':
                         (str,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'online_function_call_request':
                         (OnlineFunctionCallRequest,),
                 },
                 'attribute_map': {
                     'func_id': 'func_id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'func_id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'online_function_call_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -200,17 +185,14 @@
                 'endpoint_path': '/api/lambda/functions',
                 'operation_id': 'list_functions',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -218,30 +200,18 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -261,17 +231,14 @@
                 'endpoint_path': '/api/lambda/requests',
                 'operation_id': 'list_requests',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -279,30 +246,18 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -323,17 +278,14 @@
                 'operation_id': 'retrieve_functions',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'func_id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'func_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -352,32 +304,20 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'func_id':
                         (str,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'func_id': 'func_id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'func_id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -400,17 +340,14 @@
                 'operation_id': 'retrieve_requests',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -422,32 +359,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -480,17 +405,14 @@
         >>> thread = api.create_functions(func_id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             func_id (str):
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             online_function_call_request (OnlineFunctionCallRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -636,17 +558,14 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list_functions(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -713,17 +632,14 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list_requests(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -793,17 +709,14 @@
         >>> thread = api.retrieve_functions(func_id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             func_id (str):
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -874,17 +787,14 @@
         >>> thread = api.retrieve_requests(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): Request id
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/memberships_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/memberships_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -61,17 +61,14 @@
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -83,32 +80,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -235,17 +220,14 @@
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_membership_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -258,34 +240,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_membership_write_request':
                         (PatchedMembershipWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_membership_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -311,17 +281,14 @@
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -333,32 +300,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -392,17 +347,14 @@
         >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this membership.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -470,15 +422,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             filter (str): A filter term. Available filter_fields: ['user', 'role', 'id']. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             page (int): A page number within the paginated result set.. [optional]
             page_size (int): Number of results to return per page.. [optional]
             role (str): A simple equality filter for the role field. [optional]
             search (str): A search term. Available search_fields: ('user', 'role'). [optional]
@@ -557,17 +509,14 @@
         >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this membership.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_membership_write_request (PatchedMembershipWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -639,17 +588,14 @@
         >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this membership.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/organizations_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/issues_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -21,91 +21,91 @@
 from cvat_sdk.api_client.api_client import ApiClient, Endpoint as _Endpoint
 from cvat_sdk.api_client.model_utils import (  # noqa: F401
     date,
     datetime,
     file_type,
     none_type,
 )
-from cvat_sdk.api_client.model.organization_read import OrganizationRead
-from cvat_sdk.api_client.model.organization_write_request import OrganizationWriteRequest
-from cvat_sdk.api_client.model.paginated_organization_read_list import PaginatedOrganizationReadList
-from cvat_sdk.api_client.model.patched_organization_write_request import PatchedOrganizationWriteRequest
+from cvat_sdk.api_client.model.issue_read import IssueRead
+from cvat_sdk.api_client.model.issue_write_request import IssueWriteRequest
+from cvat_sdk.api_client.model.paginated_issue_read_list import PaginatedIssueReadList
+from cvat_sdk.api_client.model.patched_issue_write_request import PatchedIssueWriteRequest
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-class OrganizationsApi(object):
+class IssuesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.create_endpoint = _Endpoint(
             settings={
-                'response_schema': (OrganizationRead,),
+                'response_schema': (IssueRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/organizations',
+                'endpoint_path': '/api/issues',
                 'operation_id': 'create',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization_write_request',
+                    'issue_write_request',
                     'x_organization',
                     'org',
                     'org_id',
                 ],
                 'required': [
-                    'organization_write_request',
+                    'issue_write_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization_write_request':
-                        (OrganizationWriteRequest,),
+                    'issue_write_request':
+                        (IssueWriteRequest,),
                     'x_organization':
                         (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'org': 'org',
                     'org_id': 'org_id',
                 },
                 'location_map': {
-                    'organization_write_request': 'body',
+                    'issue_write_request': 'body',
                     'x_organization': 'header',
                     'org': 'query',
                     'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
@@ -125,25 +125,22 @@
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/organizations/{id}',
+                'endpoint_path': '/api/issues/{id}',
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -155,70 +152,61 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.list_endpoint = _Endpoint(
             settings={
-                'response_schema': (PaginatedOrganizationReadList,),
+                'response_schema': (PaginatedIssueReadList,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/organizations',
+                'endpoint_path': '/api/issues',
                 'operation_id': 'list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'x_organization',
+                    'assignee',
                     'filter',
-                    'name',
+                    'frame_id',
+                    'job_id',
                     'org',
                     'org_id',
                     'owner',
                     'page',
                     'page_size',
+                    'resolved',
                     'search',
-                    'slug',
                     'sort',
+                    'task_id',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -228,94 +216,103 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'x_organization':
                         (str,),
-                    'filter':
+                    'assignee':
                         (str,),
-                    'name':
+                    'filter':
                         (str,),
+                    'frame_id':
+                        (int,),
+                    'job_id':
+                        (int,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
                     'owner':
                         (str,),
                     'page':
                         (int,),
                     'page_size':
                         (int,),
+                    'resolved':
+                        (bool,),
                     'search':
                         (str,),
-                    'slug':
-                        (str,),
                     'sort':
                         (str,),
+                    'task_id':
+                        (int,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
+                    'assignee': 'assignee',
                     'filter': 'filter',
-                    'name': 'name',
+                    'frame_id': 'frame_id',
+                    'job_id': 'job_id',
                     'org': 'org',
                     'org_id': 'org_id',
                     'owner': 'owner',
                     'page': 'page',
                     'page_size': 'page_size',
+                    'resolved': 'resolved',
                     'search': 'search',
-                    'slug': 'slug',
                     'sort': 'sort',
+                    'task_id': 'task_id',
                 },
                 'location_map': {
                     'x_organization': 'header',
+                    'assignee': 'query',
                     'filter': 'query',
-                    'name': 'query',
+                    'frame_id': 'query',
+                    'job_id': 'query',
                     'org': 'query',
                     'org_id': 'query',
                     'owner': 'query',
                     'page': 'query',
                     'page_size': 'query',
+                    'resolved': 'query',
                     'search': 'query',
-                    'slug': 'query',
                     'sort': 'query',
+                    'task_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.partial_update_endpoint = _Endpoint(
             settings={
-                'response_schema': (OrganizationRead,),
+                'response_schema': (IssueRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/organizations/{id}',
+                'endpoint_path': '/api/issues/{id}',
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'patched_organization_write_request',
+                    'patched_issue_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -327,35 +324,23 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'patched_organization_write_request':
-                        (PatchedOrganizationWriteRequest,),
+                    'patched_issue_write_request':
+                        (PatchedIssueWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'patched_organization_write_request': 'body',
+                    'patched_issue_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -364,33 +349,30 @@
                     'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
-                'response_schema': (OrganizationRead,),
+                'response_schema': (IssueRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/organizations/{id}',
+                'endpoint_path': '/api/issues/{id}',
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -402,32 +384,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -435,38 +405,38 @@
                 'content_type': [],
             },
             api_client=api_client
         )
 
     def create(
         self,
-        organization_write_request: OrganizationWriteRequest,
+        issue_write_request: IssueWriteRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[OrganizationRead], urllib3.HTTPResponse]:
-        """Method creates an organization  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[IssueRead], urllib3.HTTPResponse]:
+        """Method creates an issue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create(organization_write_request, _async_call=True)
+        >>> thread = api.create(issue_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            organization_write_request (OrganizationWriteRequest):
+            issue_write_request (IssueWriteRequest):
 
         Keyword Args:
             x_organization (str): [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
@@ -497,29 +467,29 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (OrganizationRead, HTTPResponse)
+            (IssueRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['organization_write_request'] = organization_write_request
+        kwargs['issue_write_request'] = issue_write_request
         return self.create_endpoint.call_with_http_info(**kwargs)
 
     def destroy(
         self,
         id: int,
         *,
         _parse_response: bool = True,
@@ -530,29 +500,26 @@
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method deletes an organization  # noqa: E501
+        """Method deletes an issue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this organization.
+            id (int): A unique integer value identifying this issue.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -609,36 +576,39 @@
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[PaginatedOrganizationReadList], urllib3.HTTPResponse]:
-        """Method returns a paginated list of organizations  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[PaginatedIssueReadList], urllib3.HTTPResponse]:
+        """Method returns a paginated list of issues  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
-            filter (str): A filter term. Available filter_fields: ['name', 'owner', 'id', 'slug']. [optional]
-            name (str): A simple equality filter for the name field. [optional]
+            x_organization (str): Organization unique slug. [optional]
+            assignee (str): A simple equality filter for the assignee field. [optional]
+            filter (str): A filter term. Available filter_fields: ['owner', 'assignee', 'id', 'job_id', 'task_id', 'resolved', 'frame_id']. [optional]
+            frame_id (int): A simple equality filter for the frame_id field. [optional]
+            job_id (int): A simple equality filter for the job_id field. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             owner (str): A simple equality filter for the owner field. [optional]
             page (int): A page number within the paginated result set.. [optional]
             page_size (int): Number of results to return per page.. [optional]
-            search (str): A search term. Available search_fields: ('name', 'owner'). [optional]
-            slug (str): A simple equality filter for the slug field. [optional]
-            sort (str): Which field to use when ordering the results. Available ordering_fields: ['name', 'owner', 'id', 'slug']. [optional]
+            resolved (bool): A simple equality filter for the resolved field. [optional]
+            search (str): A search term. Available search_fields: ('owner', 'assignee'). [optional]
+            sort (str): Which field to use when ordering the results. Available ordering_fields: ['owner', 'assignee', 'id', 'job_id', 'task_id', 'resolved', 'frame_id']. [optional]
+            task_id (int): A simple equality filter for the task_id field. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -664,15 +634,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (PaginatedOrganizationReadList, HTTPResponse)
+            (PaginatedIssueReadList, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
@@ -695,31 +665,28 @@
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[OrganizationRead], urllib3.HTTPResponse]:
-        """Methods does a partial update of chosen fields in an organization  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[IssueRead], urllib3.HTTPResponse]:
+        """Methods does a partial update of chosen fields in an issue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this organization.
+            id (int): A unique integer value identifying this issue.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            patched_organization_write_request (PatchedOrganizationWriteRequest): [optional]
+            patched_issue_write_request (PatchedIssueWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -745,15 +712,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (OrganizationRead, HTTPResponse)
+            (IssueRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
@@ -777,30 +744,27 @@
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[OrganizationRead], urllib3.HTTPResponse]:
-        """Method returns details of an organization  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[IssueRead], urllib3.HTTPResponse]:
+        """Method returns details of an issue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this organization.
+            id (int): A unique integer value identifying this issue.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -826,15 +790,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (OrganizationRead, HTTPResponse)
+            (IssueRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/projects_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/projects_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -226,21 +226,18 @@
                 'operation_id': 'create_dataset',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                     'dataset_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
@@ -261,53 +258,41 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                     'dataset_write_request':
                         (DatasetWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                     'dataset_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -333,17 +318,14 @@
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -355,32 +337,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -516,17 +486,14 @@
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_project_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -539,34 +506,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_project_write_request':
                         (PatchedProjectWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_project_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -592,17 +547,14 @@
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -614,32 +566,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -663,21 +603,18 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'format',
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'format',
                     'id',
                 ],
                 'nullable': [
@@ -704,53 +641,41 @@
                     },
                 },
                 'openapi_types': {
                     'format':
                         (str,),
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'format': 'format',
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'format': 'query',
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -774,21 +699,18 @@
                 'operation_id': 'retrieve_backup',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -812,51 +734,39 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -878,22 +788,19 @@
                 'operation_id': 'retrieve_dataset',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -918,55 +825,43 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -990,17 +885,14 @@
                 'operation_id': 'retrieve_preview',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -1012,32 +904,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -1231,21 +1111,18 @@
         >>> thread = api.create_dataset(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Dataset file name. [optional]
             format (str): Desired dataset format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): Where to import the dataset from. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in the project to import annotations. [optional] if omitted the server will use the default value of True
             dataset_write_request (DatasetWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1318,17 +1195,14 @@
         >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1396,15 +1270,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             assignee (str): A simple equality filter for the assignee field. [optional]
             filter (str): A filter term. Available filter_fields: ['name', 'owner', 'assignee', 'status', 'id', 'updated_date']. [optional]
             name (str): A simple equality filter for the name field. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             owner (str): A simple equality filter for the owner field. [optional]
             page (int): A page number within the paginated result set.. [optional]
@@ -1485,17 +1359,14 @@
         >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_project_write_request (PatchedProjectWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1567,17 +1438,14 @@
         >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1650,21 +1518,18 @@
         >>> result = thread.get()
 
         Args:
             format (str): Desired output format name You can get the list of supported formats at: /server/annotation/formats
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after annotation file had been created. [optional] if omitted the server will use the default value of "download"
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Desired output file name. [optional]
             location (str): Where need to save downloaded dataset. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in project to export annotation. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1737,21 +1602,18 @@
         >>> thread = api.retrieve_backup(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after backup file had been created. [optional] if omitted the server will use the default value of "download"
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Backup file name. [optional]
             location (str): Where need to save downloaded backup. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in project to export backup. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1823,22 +1685,19 @@
         >>> thread = api.retrieve_dataset(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after annotation file had been created. [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Desired output file name. [optional]
             format (str): Desired output format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): Where need to save downloaded dataset. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in project to import dataset. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1910,17 +1769,14 @@
         >>> thread = api.retrieve_preview(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this project.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/schema_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/schema_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -57,18 +57,15 @@
                 'endpoint_path': '/api/schema/',
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
                     'lang',
-                    'org',
-                    'org_id',
                     'scheme',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                     'lang',
@@ -90,14 +87,15 @@
                         "AZ": "az",
                         "BE": "be",
                         "BG": "bg",
                         "BN": "bn",
                         "BR": "br",
                         "BS": "bs",
                         "CA": "ca",
+                        "CKB": "ckb",
                         "CS": "cs",
                         "CY": "cy",
                         "DA": "da",
                         "DE": "de",
                         "DSB": "dsb",
                         "EL": "el",
                         "EN": "en",
@@ -142,14 +140,15 @@
                         "LB": "lb",
                         "LT": "lt",
                         "LV": "lv",
                         "MK": "mk",
                         "ML": "ml",
                         "MN": "mn",
                         "MR": "mr",
+                        "MS": "ms",
                         "MY": "my",
                         "NB": "nb",
                         "NE": "ne",
                         "NL": "nl",
                         "NN": "nn",
                         "OS": "os",
                         "PA": "pa",
@@ -183,37 +182,25 @@
                     ('scheme',): {
 
                         "JSON": "json",
                         "YAML": "yaml"
                     },
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
                     'lang':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'scheme':
                         (str,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
                     'lang': 'lang',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'scheme': 'scheme',
                 },
                 'location_map': {
-                    'x_organization': 'header',
                     'lang': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'scheme': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -249,18 +236,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.retrieve(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
             lang (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             scheme (str): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/server_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/server_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -61,18 +61,15 @@
                 'endpoint_path': '/api/server/share',
                 'operation_id': 'list_share',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
                     'directory',
-                    'org',
-                    'org_id',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -80,34 +77,22 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
                     'directory':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
                     'directory': 'directory',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
                     'directory': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -129,17 +114,14 @@
                 'endpoint_path': '/api/server/about',
                 'operation_id': 'retrieve_about',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -147,30 +129,18 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -192,17 +162,14 @@
                 'endpoint_path': '/api/server/annotation/formats',
                 'operation_id': 'retrieve_annotation_formats',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -210,30 +177,18 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -255,17 +210,14 @@
                 'endpoint_path': '/api/server/plugins',
                 'operation_id': 'retrieve_plugins',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -273,30 +225,18 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -327,18 +267,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list_share(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
             directory (str): Directory to browse. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -405,17 +342,14 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.retrieve_about(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -482,17 +416,14 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.retrieve_annotation_formats(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -559,17 +490,14 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.retrieve_plugins(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/tasks_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/tasks_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -72,17 +72,14 @@
                 'operation_id': 'jobs_partial_update_data_meta',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_data_meta_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -95,34 +92,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_data_meta_write_request':
                         (PatchedDataMetaWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_data_meta_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -219,21 +204,18 @@
                 'operation_id': 'create_annotations',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                     'task_annotations_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
@@ -254,53 +236,41 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                     'task_annotations_write_request':
                         (TaskAnnotationsWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                     'task_annotations_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -421,17 +391,14 @@
             params_map={
                 'all': [
                     'id',
                     'data_request',
                     'upload_finish',
                     'upload_multiple',
                     'upload_start',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                     'data_request',
                 ],
                 'nullable': [
                 ],
@@ -452,39 +419,27 @@
                         (DataRequest,),
                     'upload_finish':
                         (bool,),
                     'upload_multiple':
                         (bool,),
                     'upload_start':
                         (bool,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'upload_finish': 'Upload-Finish',
                     'upload_multiple': 'Upload-Multiple',
                     'upload_start': 'Upload-Start',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
                     'data_request': 'body',
                     'upload_finish': 'header',
                     'upload_multiple': 'header',
                     'upload_start': 'header',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
@@ -508,17 +463,14 @@
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -530,32 +482,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -576,17 +516,14 @@
                 'operation_id': 'destroy_annotations',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -598,32 +535,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -795,17 +720,14 @@
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_task_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -818,34 +740,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_task_write_request':
                         (PatchedTaskWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_task_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -872,17 +782,14 @@
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'action',
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_labeled_data_request',
                 ],
                 'required': [
                     'action',
                     'id',
                 ],
                 'nullable': [
@@ -905,36 +812,24 @@
                     },
                 },
                 'openapi_types': {
                     'action':
                         (str,),
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_labeled_data_request':
                         (PatchedLabeledDataRequest,),
                 },
                 'attribute_map': {
                     'action': 'action',
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'action': 'query',
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_labeled_data_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -961,17 +856,14 @@
                 'operation_id': 'partial_update_data_meta',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                     'patched_data_meta_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -984,34 +876,22 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'patched_data_meta_write_request':
                         (PatchedDataMetaWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                     'patched_data_meta_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -1037,17 +917,14 @@
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -1059,32 +936,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -1107,22 +972,19 @@
                 'operation_id': 'retrieve_annotations',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -1146,55 +1008,43 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -1218,21 +1068,18 @@
                 'operation_id': 'retrieve_backup',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -1256,51 +1103,39 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -1322,18 +1157,15 @@
                 'operation_id': 'retrieve_data',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'number',
-                    'org',
-                    'org_id',
                     'quality',
                     'type',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
@@ -1360,42 +1192,30 @@
                         "CONTEXT_IMAGE": "context_image",
                         "FRAME": "frame"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'number':
                         (int,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'quality':
                         (str,),
                     'type':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'number': 'number',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'quality': 'quality',
                     'type': 'type',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'number': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'quality': 'query',
                     'type': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -1418,17 +1238,14 @@
                 'operation_id': 'retrieve_data_meta',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -1440,32 +1257,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -1489,21 +1294,18 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'format',
                     'id',
-                    'x_organization',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'location',
-                    'org',
-                    'org_id',
                     'use_default_location',
                 ],
                 'required': [
                     'format',
                     'id',
                 ],
                 'nullable': [
@@ -1530,53 +1332,41 @@
                     },
                 },
                 'openapi_types': {
                     'format':
                         (str,),
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'action':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'location':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'format': 'format',
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
-                    'org': 'org',
-                    'org_id': 'org_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'format': 'query',
                     'id': 'path',
-                    'x_organization': 'header',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -1600,17 +1390,14 @@
                 'operation_id': 'retrieve_preview',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -1622,32 +1409,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
@@ -1668,17 +1443,14 @@
                 'operation_id': 'retrieve_status',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -1690,32 +1462,20 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -1738,18 +1498,15 @@
                 'operation_id': 'update_annotations',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
                     'format',
-                    'org',
-                    'org_id',
                     'task_annotations_update_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                     'task_annotations_update_request',
@@ -1763,38 +1520,26 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
                     'format':
                         (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                     'task_annotations_update_request':
                         (TaskAnnotationsUpdateRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
                     'format': 'format',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
                     'format': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
                     'task_annotations_update_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -1830,17 +1575,14 @@
         >>> thread = api.jobs_partial_update_data_meta(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_data_meta_write_request (PatchedDataMetaWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1993,21 +1735,18 @@
         >>> thread = api.create_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Annotation file name. [optional]
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): where to import the annotation from. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in task to import annotations. [optional] if omitted the server will use the default value of True
             task_annotations_write_request (TaskAnnotationsWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2169,17 +1908,14 @@
             id (int): A unique integer value identifying this task.
             data_request (DataRequest):
 
         Keyword Args:
             upload_finish (bool): Finishes data upload. Can be combined with Upload-Start header to create task data with one request. [optional]
             upload_multiple (bool): Indicates that data with this request are single or multiple files that should be attached to a task. [optional]
             upload_start (bool): Initializes data upload. No data should be sent with this header. [optional]
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -2251,17 +1987,14 @@
         >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -2332,17 +2065,14 @@
         >>> thread = api.destroy_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -2410,15 +2140,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             assignee (str): A simple equality filter for the assignee field. [optional]
             dimension (str): A simple equality filter for the dimension field. [optional]
             filter (str): A filter term. Available filter_fields: ['project_name', 'name', 'owner', 'status', 'assignee', 'subset', 'mode', 'dimension', 'tracker_link', 'id', 'project_id', 'updated_date']. [optional]
             mode (str): A simple equality filter for the mode field. [optional]
             name (str): A simple equality filter for the name field. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
@@ -2505,17 +2235,14 @@
         >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_task_write_request (PatchedTaskWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -2589,17 +2316,14 @@
         >>> result = thread.get()
 
         Args:
             action (str):
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_labeled_data_request (PatchedLabeledDataRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -2672,17 +2396,14 @@
         >>> thread = api.partial_update_data_meta(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             patched_data_meta_write_request (PatchedDataMetaWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -2754,17 +2475,14 @@
         >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -2835,22 +2553,19 @@
         >>> thread = api.retrieve_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after annotation file had been created. [optional] if omitted the server will use the default value of "download"
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Desired output file name. [optional]
             format (str): Desired output format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): Where need to save downloaded dataset. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in the task to export annotation. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -2922,21 +2637,18 @@
         >>> thread = api.retrieve_backup(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after backup file had been created. [optional] if omitted the server will use the default value of "download"
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Backup file name. [optional]
             location (str): Where need to save downloaded backup. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in the task to export backup. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -3008,18 +2720,15 @@
         >>> thread = api.retrieve_data(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
             number (int): A unique number value identifying chunk or frame. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             quality (str): Specifies the quality level of the requested data. [optional]
             type (str): Specifies the type of the requested data. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -3092,17 +2801,14 @@
         >>> thread = api.retrieve_data_meta(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -3175,21 +2881,18 @@
         >>> result = thread.get()
 
         Args:
             format (str): Desired output format name You can get the list of supported formats at: /server/annotation/formats
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
             action (str): Used to start downloading process after annotation file had been created. [optional] if omitted the server will use the default value of "download"
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Desired output file name. [optional]
             location (str): Where need to save downloaded dataset. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             use_default_location (bool): Use the location that was configured in task to export annotations. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -3262,17 +2965,14 @@
         >>> thread = api.retrieve_preview(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -3343,17 +3043,14 @@
         >>> thread = api.retrieve_status(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -3424,18 +3121,15 @@
         >>> thread = api.update_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
-            x_organization (str): [optional]
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             task_annotations_update_request (TaskAnnotationsUpdateRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api/users_api.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api/organizations_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -21,57 +21,111 @@
 from cvat_sdk.api_client.api_client import ApiClient, Endpoint as _Endpoint
 from cvat_sdk.api_client.model_utils import (  # noqa: F401
     date,
     datetime,
     file_type,
     none_type,
 )
-from cvat_sdk.api_client.model.meta_user import MetaUser
-from cvat_sdk.api_client.model.paginated_meta_user_list import PaginatedMetaUserList
-from cvat_sdk.api_client.model.patched_user_request import PatchedUserRequest
+from cvat_sdk.api_client.model.organization_read import OrganizationRead
+from cvat_sdk.api_client.model.organization_write_request import OrganizationWriteRequest
+from cvat_sdk.api_client.model.paginated_organization_read_list import PaginatedOrganizationReadList
+from cvat_sdk.api_client.model.patched_organization_write_request import PatchedOrganizationWriteRequest
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-class UsersApi(object):
+class OrganizationsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.create_endpoint = _Endpoint(
+            settings={
+                'response_schema': (OrganizationRead,),
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/organizations',
+                'operation_id': 'create',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_write_request',
+                ],
+                'required': [
+                    'organization_write_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_write_request':
+                        (OrganizationWriteRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'organization_write_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/users/{id}',
+                'endpoint_path': '/api/organizations/{id}',
                 'operation_id': 'destroy',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -83,71 +137,55 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.list_endpoint = _Endpoint(
             settings={
-                'response_schema': (PaginatedMetaUserList,),
+                'response_schema': (PaginatedOrganizationReadList,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/users',
+                'endpoint_path': '/api/organizations',
                 'operation_id': 'list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'x_organization',
                     'filter',
-                    'first_name',
-                    'is_active',
-                    'last_name',
-                    'org',
-                    'org_id',
+                    'name',
+                    'owner',
                     'page',
                     'page_size',
                     'search',
+                    'slug',
                     'sort',
-                    'username',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -155,100 +193,81 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'x_organization':
-                        (str,),
                     'filter':
                         (str,),
-                    'first_name':
-                        (str,),
-                    'is_active':
-                        (bool,),
-                    'last_name':
+                    'name':
                         (str,),
-                    'org':
+                    'owner':
                         (str,),
-                    'org_id':
-                        (int,),
                     'page':
                         (int,),
                     'page_size':
                         (int,),
                     'search':
                         (str,),
-                    'sort':
+                    'slug':
                         (str,),
-                    'username':
+                    'sort':
                         (str,),
                 },
                 'attribute_map': {
-                    'x_organization': 'X-Organization',
                     'filter': 'filter',
-                    'first_name': 'first_name',
-                    'is_active': 'is_active',
-                    'last_name': 'last_name',
-                    'org': 'org',
-                    'org_id': 'org_id',
+                    'name': 'name',
+                    'owner': 'owner',
                     'page': 'page',
                     'page_size': 'page_size',
                     'search': 'search',
+                    'slug': 'slug',
                     'sort': 'sort',
-                    'username': 'username',
                 },
                 'location_map': {
-                    'x_organization': 'header',
                     'filter': 'query',
-                    'first_name': 'query',
-                    'is_active': 'query',
-                    'last_name': 'query',
-                    'org': 'query',
-                    'org_id': 'query',
+                    'name': 'query',
+                    'owner': 'query',
                     'page': 'query',
                     'page_size': 'query',
                     'search': 'query',
+                    'slug': 'query',
                     'sort': 'query',
-                    'username': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.partial_update_endpoint = _Endpoint(
             settings={
-                'response_schema': (MetaUser,),
+                'response_schema': (OrganizationRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/users/{id}',
+                'endpoint_path': '/api/organizations/{id}',
                 'operation_id': 'partial_update',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'patched_user_request',
+                    'patched_organization_write_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -260,35 +279,23 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'patched_user_request':
-                        (PatchedUserRequest,),
+                    'patched_organization_write_request':
+                        (PatchedOrganizationWriteRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'patched_user_request': 'body',
+                    'patched_organization_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -297,33 +304,30 @@
                     'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
-                'response_schema': (MetaUser,),
+                'response_schema': (OrganizationRead,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
-                'endpoint_path': '/api/users/{id}',
+                'endpoint_path': '/api/organizations/{id}',
                 'operation_id': 'retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -335,139 +339,61 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
                 },
                 'location_map': {
                     'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/vnd.cvat+json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.retrieve_self_endpoint = _Endpoint(
-            settings={
-                'response_schema': (MetaUser,),
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/users/self',
-                'operation_id': 'retrieve_self',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'x_organization',
-                    'org',
-                    'org_id',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def destroy(
+    def create(
         self,
-        id: int,
+        organization_write_request: OrganizationWriteRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method deletes a specific user from the server  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[OrganizationRead], urllib3.HTTPResponse]:
+        """Method creates an organization  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.destroy(id, _async_call=True)
+        >>> thread = api.create(organization_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this user.
+            organization_write_request (OrganizationWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -493,68 +419,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (None, HTTPResponse)
+            (OrganizationRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['id'] = id
-        return self.destroy_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_write_request'] = organization_write_request
+        return self.create_endpoint.call_with_http_info(**kwargs)
 
-    def list(
+    def destroy(
         self,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[PaginatedMetaUserList], urllib3.HTTPResponse]:
-        """Method returns a paginated list of users  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+        """Method deletes an organization  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.list(_async_call=True)
+        >>> thread = api.destroy(id, _async_call=True)
         >>> result = thread.get()
 
+        Args:
+            id (int): A unique integer value identifying this organization.
 
         Keyword Args:
-            x_organization (str): [optional]
-            filter (str): A filter term. Available filter_fields: ['username', 'first_name', 'last_name', 'id', 'is_active']. [optional]
-            first_name (str): A simple equality filter for the first_name field. [optional]
-            is_active (bool): A simple equality filter for the is_active field. [optional]
-            last_name (str): A simple equality filter for the last_name field. [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            page (int): A page number within the paginated result set.. [optional]
-            page_size (int): Number of results to return per page.. [optional]
-            search (str): A search term. Available search_fields: ('username', 'first_name', 'last_name'). [optional]
-            sort (str): Which field to use when ordering the results. Available ordering_fields: ['username', 'first_name', 'last_name', 'id', 'is_active']. [optional]
-            username (str): A simple equality filter for the username field. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -580,62 +497,64 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (PaginatedMetaUserList, HTTPResponse)
+            (None, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        return self.list_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.destroy_endpoint.call_with_http_info(**kwargs)
 
-    def partial_update(
+    def list(
         self,
-        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[MetaUser], urllib3.HTTPResponse]:
-        """Method updates chosen fields of a user  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[PaginatedOrganizationReadList], urllib3.HTTPResponse]:
+        """Method returns a paginated list of organizations  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.partial_update(id, _async_call=True)
+        >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
-        Args:
-            id (int): A unique integer value identifying this user.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            patched_user_request (PatchedUserRequest): [optional]
+            filter (str): A filter term. Available filter_fields: ['name', 'owner', 'id', 'slug']. [optional]
+            name (str): A simple equality filter for the name field. [optional]
+            owner (str): A simple equality filter for the owner field. [optional]
+            page (int): A page number within the paginated result set.. [optional]
+            page_size (int): Number of results to return per page.. [optional]
+            search (str): A search term. Available search_fields: ('name', 'owner'). [optional]
+            slug (str): A simple equality filter for the slug field. [optional]
+            sort (str): Which field to use when ordering the results. Available ordering_fields: ['name', 'owner', 'id', 'slug']. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -661,62 +580,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (MetaUser, HTTPResponse)
+            (PaginatedOrganizationReadList, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['id'] = id
-        return self.partial_update_endpoint.call_with_http_info(**kwargs)
+        return self.list_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve(
+    def partial_update(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[MetaUser], urllib3.HTTPResponse]:
-        """Method provides information of a specific user  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[OrganizationRead], urllib3.HTTPResponse]:
+        """Methods does a partial update of chosen fields in an organization  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve(id, _async_call=True)
+        >>> thread = api.partial_update(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): A unique integer value identifying this user.
+            id (int): A unique integer value identifying this organization.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
+            patched_organization_write_request (PatchedOrganizationWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -742,60 +658,59 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (MetaUser, HTTPResponse)
+            (OrganizationRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        return self.retrieve_endpoint.call_with_http_info(**kwargs)
+        return self.partial_update_endpoint.call_with_http_info(**kwargs)
 
-    def retrieve_self(
+    def retrieve(
         self,
+        id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[MetaUser], urllib3.HTTPResponse]:
-        """Method returns an instance of a user who is currently authorized  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[OrganizationRead], urllib3.HTTPResponse]:
+        """Method returns details of an organization  # noqa: E501
 
-        Method returns an instance of a user who is currently authorized  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.retrieve_self(_async_call=True)
+        >>> thread = api.retrieve(id, _async_call=True)
         >>> result = thread.get()
 
+        Args:
+            id (int): A unique integer value identifying this organization.
 
         Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -821,23 +736,24 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (MetaUser, HTTPResponse)
+            (OrganizationRead, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        return self.retrieve_self_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = id
+        return self.retrieve_endpoint.call_with_http_info(**kwargs)
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/api_client.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import json
@@ -110,15 +110,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers: typing.Dict[str, str] = headers or {}
         self.cookies = SimpleCookie()
         if cookies:
             self.cookies.update(cookies)
         # Set default User-Agent.
-        self.user_agent = 'cvat_sdk/2.4.4'
+        self.user_agent = 'cvat_sdk/2.4.5'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/apis/__init__.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/apis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/configuration.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import copy
 import logging
 import multiprocessing
@@ -484,16 +484,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.4.4\n"\
-               "SDK Package Version: 2.4.4".\
+               "Version of the API: 2.4.5\n"\
+               "SDK Package Version: 2.4.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/exceptions.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/about.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/about.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotation_file_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotation_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotations_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotations_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/backup_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/backup_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/chunk_type.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IChunkType(IModelData):
+class IWebhookType(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "video", "imageset", "list"  # noqa: E501
+    One of: "organization", "project"  # noqa: E501
     """
 
-class ChunkType(ModelSimple, IChunkType):
+class WebhookType(ModelSimple, IWebhookType):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,17 +78,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'VIDEO': "video",
-            'IMAGESET': "imageset",
-            'LIST': "list",
+            'ORGANIZATION': "organization",
+            'PROJECT': "project",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -128,23 +127,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ChunkType - a model defined in OpenAPI
+        """WebhookType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["video", "imageset", "list", ]  # noqa: E501
+            args[0] (str): * `organization` - ORGANIZATION * `project` - PROJECT., must be one of ["organization", "project", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["video", "imageset", "list", ]  # noqa: E501
+            value (str): * `organization` - ORGANIZATION * `project` - PROJECT., must be one of ["organization", "project", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -224,23 +223,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """ChunkType - a model defined in OpenAPI
+        """WebhookType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["video", "imageset", "list", ]  # noqa: E501
+            args[0] (str): * `organization` - ORGANIZATION * `project` - PROJECT., must be one of ["organization", "project", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["video", "imageset", "list", ]  # noqa: E501
+            value (str): * `organization` - ORGANIZATION * `project` - PROJECT., must be one of ["organization", "project", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read_owner.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comments_summary.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comments_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/credentials_type_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_stage.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class ICredentialsTypeEnum(IModelData):
+class IJobStage(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING"  # noqa: E501
+    One of: "annotation", "validation", "acceptance"  # noqa: E501
     """
 
-class CredentialsTypeEnum(ModelSimple, ICredentialsTypeEnum):
+class JobStage(ModelSimple, IJobStage):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,19 +78,17 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'KEY_SECRET_KEY_PAIR': "KEY_SECRET_KEY_PAIR",
-            'ACCOUNT_NAME_TOKEN_PAIR': "ACCOUNT_NAME_TOKEN_PAIR",
-            'KEY_FILE_PATH': "KEY_FILE_PATH",
-            'ANONYMOUS_ACCESS': "ANONYMOUS_ACCESS",
-            'CONNECTION_STRING': "CONNECTION_STRING",
+            'ANNOTATION': "annotation",
+            'VALIDATION': "validation",
+            'ACCEPTANCE': "acceptance",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -130,23 +128,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CredentialsTypeEnum - a model defined in OpenAPI
+        """JobStage - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
+            args[0] (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `acceptance` - ACCEPTANCE., must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
+            value (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `acceptance` - ACCEPTANCE., must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -226,23 +224,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """CredentialsTypeEnum - a model defined in OpenAPI
+        """JobStage - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
+            args[0] (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `acceptance` - ACCEPTANCE., must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
+            value (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `acceptance` - ACCEPTANCE., must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/data_meta_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_meta_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -54,15 +54,15 @@
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    chunk_size: int # noqa: E501
+    chunk_size: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
     size: int # noqa: E501
     """
     [optional]
@@ -108,15 +108,15 @@
     Attributes:
       image_quality (int):
 
       frames ([FrameMeta], none_type):
 
       deleted_frames ([int]):
 
-      chunk_size (int): [optional]  # noqa: E501
+      chunk_size (int, none_type): [optional]  # noqa: E501
 
       size (int): [optional]  # noqa: E501
 
       start_frame (int): [optional]  # noqa: E501
 
       stop_frame (int): [optional]  # noqa: E501
 
@@ -173,15 +173,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'image_quality': (int,),  # noqa: E501
             'frames': ([FrameMeta], none_type,),  # noqa: E501
             'deleted_frames': ([int],),  # noqa: E501
-            'chunk_size': (int,),  # noqa: E501
+            'chunk_size': (int, none_type,),  # noqa: E501
             'size': (int,),  # noqa: E501
             'start_frame': (int,),  # noqa: E501
             'stop_frame': (int,),  # noqa: E501
             'frame_filter': (str,),  # noqa: E501
         }
 
     @cached_property
@@ -218,15 +218,15 @@
 
         Args:
             image_quality (int):
             frames ([FrameMeta], none_type):
             deleted_frames ([int]):
 
         Keyword Args:
-            chunk_size (int): [optional]  # noqa: E501
+            chunk_size (int, none_type): [optional]  # noqa: E501
 
             size (int): [optional]  # noqa: E501
 
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
 
@@ -322,15 +322,15 @@
 
         Args:
             image_quality (int):
             frames ([FrameMeta], none_type):
             deleted_frames ([int]):
 
         Keyword Args:
-            chunk_size (int): [optional]  # noqa: E501
+            chunk_size (int, none_type): [optional]  # noqa: E501
 
             size (int): [optional]  # noqa: E501
 
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/data_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -119,14 +119,21 @@
     server_files: typing.List[str] # noqa: E501
     """
     [optional, default: []]
     [str]
     Paths to files from a file share mounted on the server, or from a cloud storage.
     """
 
+    server_files_exclude: typing.List[str] # noqa: E501
+    """
+    [optional, default: []]
+    [str]
+    Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] .
+    """
+
     remote_files: typing.List[str] # noqa: E501
     """
     [optional, default: []]
     [str]
     Direct download URLs for files.
     """
 
@@ -207,14 +214,16 @@
 
       original_chunk_type (ChunkType): [optional]  # noqa: E501
 
       client_files ([file_type]): Uploaded files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
       server_files ([str]): Paths to files from a file share mounted on the server, or from a cloud storage. [optional] if omitted the server will use the default value of []  # noqa: E501
 
+      server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
+
       remote_files ([str]): Direct download URLs for files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
       use_zip_chunks (bool): When true, video chunks will be represented as zip archives with decoded video frames. When false, video chunks are represented as video segments . [optional] if omitted the server will use the default value of False  # noqa: E501
 
       cloud_storage_id (int, none_type): If not null, the files referenced by server_files will be retrieved from the cloud storage with the specified ID. The cloud storages applicable depend on the context. In the user sandbox, only the user sandbox cloud storages can be used. In an organization, only the organization cloud storages can be used. . [optional]  # noqa: E501
 
       use_cache (bool): Enable or disable task data chunk caching for the task. Read more: https://opencv.github.io/cvat/docs/manual/advanced/data_on_fly/ . [optional] if omitted the server will use the default value of False  # noqa: E501
@@ -311,14 +320,15 @@
             'start_frame': (int,),  # noqa: E501
             'stop_frame': (int,),  # noqa: E501
             'frame_filter': (str,),  # noqa: E501
             'compressed_chunk_type': (ChunkType,),  # noqa: E501
             'original_chunk_type': (ChunkType,),  # noqa: E501
             'client_files': ([file_type],),  # noqa: E501
             'server_files': ([str],),  # noqa: E501
+            'server_files_exclude': ([str],),  # noqa: E501
             'remote_files': ([str],),  # noqa: E501
             'use_zip_chunks': (bool,),  # noqa: E501
             'cloud_storage_id': (int, none_type,),  # noqa: E501
             'use_cache': (bool,),  # noqa: E501
             'copy_data': (bool,),  # noqa: E501
             'storage_method': (StorageMethod,),  # noqa: E501
             'storage': (StorageType,),  # noqa: E501
@@ -340,14 +350,15 @@
         'start_frame': 'start_frame',  # noqa: E501
         'stop_frame': 'stop_frame',  # noqa: E501
         'frame_filter': 'frame_filter',  # noqa: E501
         'compressed_chunk_type': 'compressed_chunk_type',  # noqa: E501
         'original_chunk_type': 'original_chunk_type',  # noqa: E501
         'client_files': 'client_files',  # noqa: E501
         'server_files': 'server_files',  # noqa: E501
+        'server_files_exclude': 'server_files_exclude',  # noqa: E501
         'remote_files': 'remote_files',  # noqa: E501
         'use_zip_chunks': 'use_zip_chunks',  # noqa: E501
         'cloud_storage_id': 'cloud_storage_id',  # noqa: E501
         'use_cache': 'use_cache',  # noqa: E501
         'copy_data': 'copy_data',  # noqa: E501
         'storage_method': 'storage_method',  # noqa: E501
         'storage': 'storage',  # noqa: E501
@@ -384,14 +395,16 @@
 
             original_chunk_type (ChunkType): [optional]  # noqa: E501
 
             client_files ([file_type]): Uploaded files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             server_files ([str]): Paths to files from a file share mounted on the server, or from a cloud storage. [optional] if omitted the server will use the default value of []  # noqa: E501
 
+            server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
+
             remote_files ([str]): Direct download URLs for files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             use_zip_chunks (bool): When true, video chunks will be represented as zip archives with decoded video frames. When false, video chunks are represented as video segments . [optional] if omitted the server will use the default value of False  # noqa: E501
 
             cloud_storage_id (int, none_type): If not null, the files referenced by server_files will be retrieved from the cloud storage with the specified ID. The cloud storages applicable depend on the context. In the user sandbox, only the user sandbox cloud storages can be used. In an organization, only the organization cloud storages can be used. . [optional]  # noqa: E501
 
             use_cache (bool): Enable or disable task data chunk caching for the task. Read more: https://opencv.github.io/cvat/docs/manual/advanced/data_on_fly/ . [optional] if omitted the server will use the default value of False  # noqa: E501
@@ -512,14 +525,16 @@
 
             original_chunk_type (ChunkType): [optional]  # noqa: E501
 
             client_files ([file_type]): Uploaded files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             server_files ([str]): Paths to files from a file share mounted on the server, or from a cloud storage. [optional] if omitted the server will use the default value of []  # noqa: E501
 
+            server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
+
             remote_files ([str]): Direct download URLs for files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             use_zip_chunks (bool): When true, video chunks will be represented as zip archives with decoded video frames. When false, video chunks are represented as video segments . [optional] if omitted the server will use the default value of False  # noqa: E501
 
             cloud_storage_id (int, none_type): If not null, the files referenced by server_files will be retrieved from the cloud storage with the specified ID. The cloud storages applicable depend on the context. In the user sandbox, only the user sandbox cloud storages can be used. In an organization, only the organization cloud storages can be used. . [optional]  # noqa: E501
 
             use_cache (bool): Enable or disable task data chunk caching for the task. Read more: https://opencv.github.io/cvat/docs/manual/advanced/data_on_fly/ . [optional] if omitted the server will use the default value of False  # noqa: E501
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_file_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_format.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_formats.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/event.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/event_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/events.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/events_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/frame_meta.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,129 +41,153 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IEventsEnum(IModelData):
+class IFrameMeta(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-    value: str
+    # member type declarations
+    width: int # noqa: E501
+    """
+    """
+
+    height: int # noqa: E501
+    """
     """
-    [optional]
 
-    One of: "create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task"  # noqa: E501
+    name: str # noqa: E501
+    """
     """
 
-class EventsEnum(ModelSimple, IEventsEnum):
-    """NOTE: This class is auto generated by OpenAPI Generator.
+    related_files: int # noqa: E501
+    """
+    """
+
+    has_related_context: bool # noqa: E501
+    """
+    [optional]
+    """
+
+
+class FrameMeta(ModelNormal, IFrameMeta):
+    """
+    NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
+      width (int):
+
+      height (int):
+
+      name (str):
+
+      related_files (int):
+
+      has_related_context (bool): [optional]  # noqa: E501
+
+
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
+
     """
 
     allowed_values = {
-        ('value',): {
-            'CREATE:COMMENT': "create:comment",
-            'CREATE:INVITATION': "create:invitation",
-            'CREATE:ISSUE': "create:issue",
-            'CREATE:JOB': "create:job",
-            'CREATE:MEMBERSHIP': "create:membership",
-            'CREATE:PROJECT': "create:project",
-            'CREATE:TASK': "create:task",
-            'DELETE:COMMENT': "delete:comment",
-            'DELETE:INVITATION': "delete:invitation",
-            'DELETE:ISSUE': "delete:issue",
-            'DELETE:JOB': "delete:job",
-            'DELETE:MEMBERSHIP': "delete:membership",
-            'DELETE:ORGANIZATION': "delete:organization",
-            'DELETE:PROJECT': "delete:project",
-            'DELETE:TASK': "delete:task",
-            'UPDATE:COMMENT': "update:comment",
-            'UPDATE:ISSUE': "update:issue",
-            'UPDATE:JOB': "update:job",
-            'UPDATE:MEMBERSHIP': "update:membership",
-            'UPDATE:ORGANIZATION': "update:organization",
-            'UPDATE:PROJECT': "update:project",
-            'UPDATE:TASK': "update:task",
-        },
     }
 
     validations = {
+        ('name',): {
+            'max_length': 1024,
+        },
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'width': (int,),  # noqa: E501
+            'height': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'related_files': (int,),  # noqa: E501
+            'has_related_context': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
-    attribute_map = {}
+    attribute_map = {
+        'width': 'width',  # noqa: E501
+        'height': 'height',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'related_files': 'related_files',  # noqa: E501
+        'has_related_context': 'has_related_context',  # noqa: E501
+    }
 
-    read_only_vars = set()
+    read_only_vars = {
+        'has_related_context',  # noqa: E501
+    }
 
-    _composed_schemas = None
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """EventsEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, width, height, name, related_files, *args, **kwargs):  # noqa: E501
+        """FrameMeta - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            width (int):
+            height (int):
+            name (str):
+            related_files (int):
 
         Keyword Args:
-            value (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            has_related_context (bool): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -186,37 +210,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-        """
+"""
         from cvat_sdk.api_client.configuration import Configuration
 
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -229,37 +241,51 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """EventsEnum - a model defined in OpenAPI
+        self.width = width
+        self.height = height
+        self.name = name
+        self.related_files = related_files
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, width, height, name, related_files, *args, **kwargs):  # noqa: E501
+        """FrameMeta - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            width (int):
+            height (int):
+            name (str):
+            related_files (int):
 
         Keyword Args:
-            value (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            has_related_context (bool): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -282,36 +308,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-        """
+"""
         from cvat_sdk.api_client.configuration import Configuration
 
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -327,19 +337,24 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.width = width
+        self.height = height
+        self.name = name
+        self.related_files = related_files
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
+
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info_type_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info_type_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -132,18 +132,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """FileInfoTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["REG", "DIR", ]  # noqa: E501
+            args[0] (str): * `REG` - REG * `DIR` - DIR., must be one of ["REG", "DIR", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["REG", "DIR", ]  # noqa: E501
+            value (str): * `REG` - REG * `DIR` - DIR., must be one of ["REG", "DIR", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -228,18 +228,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """FileInfoTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["REG", "DIR", ]  # noqa: E501
+            args[0] (str): * `REG` - REG * `DIR` - DIR., must be one of ["REG", "DIR", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["REG", "DIR", ]  # noqa: E501
+            value (str): * `REG` - REG * `DIR` - DIR., must be one of ["REG", "DIR", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/frame_meta.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_comment_write_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,62 +41,38 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IFrameMeta(IModelData):
+class IPatchedCommentWriteRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    width: int # noqa: E501
-    """
-    """
-
-    height: int # noqa: E501
-    """
-    """
-
-    name: str # noqa: E501
-    """
-    """
-
-    related_files: int # noqa: E501
-    """
-    """
-
-    has_related_context: bool # noqa: E501
+    message: str # noqa: E501
     """
     [optional]
     """
 
 
-class FrameMeta(ModelNormal, IFrameMeta):
+class PatchedCommentWriteRequest(ModelNormal, IPatchedCommentWriteRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      width (int):
-
-      height (int):
-
-      name (str):
-
-      related_files (int):
-
-      has_related_context (bool): [optional]  # noqa: E501
+      message (str): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -113,16 +89,16 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 1024,
+        ('message',): {
+            'min_length': 1,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
@@ -139,54 +115,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'width': (int,),  # noqa: E501
-            'height': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'related_files': (int,),  # noqa: E501
-            'has_related_context': (bool,),  # noqa: E501
+            'message': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'width': 'width',  # noqa: E501
-        'height': 'height',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'related_files': 'related_files',  # noqa: E501
-        'has_related_context': 'has_related_context',  # noqa: E501
+        'message': 'message',  # noqa: E501
     }
 
     read_only_vars = {
-        'has_related_context',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, width, height, name, related_files, *args, **kwargs):  # noqa: E501
-        """FrameMeta - a model defined in OpenAPI
-
-        Args:
-            width (int):
-            height (int):
-            name (str):
-            related_files (int):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """PatchedCommentWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            has_related_context (bool): [optional]  # noqa: E501
+            message (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -242,18 +203,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.width = width
-        self.height = height
-        self.name = name
-        self.related_files = related_files
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -266,25 +223,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, width, height, name, related_files, *args, **kwargs):  # noqa: E501
-        """FrameMeta - a model defined in OpenAPI
-
-        Args:
-            width (int):
-            height (int):
-            name (str):
-            related_files (int):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """PatchedCommentWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            has_related_context (bool): [optional]  # noqa: E501
+            message (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -338,18 +289,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.width = width
-        self.height = height
-        self.name = name
-        self.related_files = related_files
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/input_type_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/chunk_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IInputTypeEnum(IModelData):
+class IChunkType(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "checkbox", "radio", "number", "text", "select"  # noqa: E501
+    One of: "video", "imageset", "list"  # noqa: E501
     """
 
-class InputTypeEnum(ModelSimple, IInputTypeEnum):
+class ChunkType(ModelSimple, IChunkType):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,19 +78,17 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CHECKBOX': "checkbox",
-            'RADIO': "radio",
-            'NUMBER': "number",
-            'TEXT': "text",
-            'SELECT': "select",
+            'VIDEO': "video",
+            'IMAGESET': "imageset",
+            'LIST': "list",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -130,23 +128,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """InputTypeEnum - a model defined in OpenAPI
+        """ChunkType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
+            args[0] (str): * `video` - VIDEO * `imageset` - IMAGESET * `list` - LIST., must be one of ["video", "imageset", "list", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
+            value (str): * `video` - VIDEO * `imageset` - IMAGESET * `list` - LIST., must be one of ["video", "imageset", "list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -226,23 +224,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """InputTypeEnum - a model defined in OpenAPI
+        """ChunkType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
+            args[0] (str): * `video` - VIDEO * `imageset` - IMAGESET * `list` - LIST., must be one of ["video", "imageset", "list", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
+            value (str): * `video` - VIDEO * `imageset` - IMAGESET * `list` - LIST., must be one of ["video", "imageset", "list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/issues_summary.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/issues_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_annotations_update_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_annotations_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -136,14 +136,19 @@
     """
 
     data_chunk_size: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
+    organization: typing.Union[int, none_type] # noqa: E501
+    """
+    [optional]
+    """
+
     data_compressed_chunk_type: typing.Union[typing.Any, none_type] # noqa: E501
     """
     [optional]
     """
 
     updated_date: datetime # noqa: E501
     """
@@ -195,14 +200,16 @@
 
       start_frame (int): [optional]  # noqa: E501
 
       stop_frame (int): [optional]  # noqa: E501
 
       data_chunk_size (int, none_type): [optional]  # noqa: E501
 
+      organization (int, none_type): [optional]  # noqa: E501
+
       data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       updated_date (datetime): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
@@ -281,14 +288,15 @@
             'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'stage': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'state': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'mode': (str,),  # noqa: E501
             'start_frame': (int,),  # noqa: E501
             'stop_frame': (int,),  # noqa: E501
             'data_chunk_size': (int, none_type,),  # noqa: E501
+            'organization': (int, none_type,),  # noqa: E501
             'data_compressed_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -308,14 +316,15 @@
         'status': 'status',  # noqa: E501
         'stage': 'stage',  # noqa: E501
         'state': 'state',  # noqa: E501
         'mode': 'mode',  # noqa: E501
         'start_frame': 'start_frame',  # noqa: E501
         'stop_frame': 'stop_frame',  # noqa: E501
         'data_chunk_size': 'data_chunk_size',  # noqa: E501
+        'organization': 'organization',  # noqa: E501
         'data_compressed_chunk_type': 'data_compressed_chunk_type',  # noqa: E501
         'updated_date': 'updated_date',  # noqa: E501
     }
 
     read_only_vars = {
         'url',  # noqa: E501
         'id',  # noqa: E501
@@ -326,14 +335,15 @@
         'status',  # noqa: E501
         'stage',  # noqa: E501
         'state',  # noqa: E501
         'mode',  # noqa: E501
         'start_frame',  # noqa: E501
         'stop_frame',  # noqa: E501
         'data_chunk_size',  # noqa: E501
+        'organization',  # noqa: E501
         'data_compressed_chunk_type',  # noqa: E501
         'updated_date',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
@@ -370,14 +380,16 @@
 
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
 
             data_chunk_size (int, none_type): [optional]  # noqa: E501
 
+            organization (int, none_type): [optional]  # noqa: E501
+
             data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -494,14 +506,16 @@
 
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
 
             data_chunk_size (int, none_type): [optional]  # noqa: E501
 
+            organization (int, none_type): [optional]  # noqa: E501
+
             data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read_assignee.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read_assignee.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_stage.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/location_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IJobStage(IModelData):
+class ILocationEnum(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "annotation", "validation", "acceptance"  # noqa: E501
+    One of: "cloud_storage", "local"  # noqa: E501
     """
 
-class JobStage(ModelSimple, IJobStage):
+class LocationEnum(ModelSimple, ILocationEnum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,17 +78,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'ANNOTATION': "annotation",
-            'VALIDATION': "validation",
-            'ACCEPTANCE': "acceptance",
+            'CLOUD_STORAGE': "cloud_storage",
+            'LOCAL': "local",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -128,23 +127,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """JobStage - a model defined in OpenAPI
+        """LocationEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
+            args[0] (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL., must be one of ["cloud_storage", "local", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
+            value (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL., must be one of ["cloud_storage", "local", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -224,23 +223,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """JobStage - a model defined in OpenAPI
+        """LocationEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
+            args[0] (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL., must be one of ["cloud_storage", "local", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["annotation", "validation", "acceptance", ]  # noqa: E501
+            value (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL., must be one of ["cloud_storage", "local", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_status.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -133,18 +133,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """JobStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["annotation", "validation", "completed", ]  # noqa: E501
+            args[0] (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `completed` - COMPLETED., must be one of ["annotation", "validation", "completed", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["annotation", "validation", "completed", ]  # noqa: E501
+            value (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `completed` - COMPLETED., must be one of ["annotation", "validation", "completed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -229,18 +229,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """JobStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["annotation", "validation", "completed", ]  # noqa: E501
+            args[0] (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `completed` - COMPLETED., must be one of ["annotation", "validation", "completed", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["annotation", "validation", "completed", ]  # noqa: E501
+            value (str): * `annotation` - ANNOTATION * `validation` - VALIDATION * `completed` - COMPLETED., must be one of ["annotation", "validation", "completed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/jobs_summary.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/jobs_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/label.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labels_summary.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labels_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/location_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_content_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class ILocationEnum(IModelData):
+class IWebhookContentType(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
-    [optional]
+    [optional, default: "application/json"]
 
-    One of: "cloud_storage", "local"  # noqa: E501
+    One of: "application/json"  # noqa: E501
     """
 
-class LocationEnum(ModelSimple, ILocationEnum):
+class WebhookContentType(ModelSimple, IWebhookContentType):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,16 +78,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CLOUD_STORAGE': "cloud_storage",
-            'LOCAL': "local",
+            'APPLICATION/JSON': "application/json",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -127,23 +126,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """LocationEnum - a model defined in OpenAPI
+        """WebhookContentType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["cloud_storage", "local", ]  # noqa: E501
+            args[0] (str): * `application/json` - JSON. if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["cloud_storage", "local", ]  # noqa: E501
+            value (str): * `application/json` - JSON. if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -178,19 +177,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
+            value = "application/json"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -223,23 +218,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """LocationEnum - a model defined in OpenAPI
+        """WebhookContentType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["cloud_storage", "local", ]  # noqa: E501
+            args[0] (str): * `application/json` - JSON. if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["cloud_storage", "local", ]  # noqa: E501
+            value (str): * `application/json` - JSON. if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -276,19 +271,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
+            value = "application/json"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/login_serializer_ex_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/login_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/membership_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/membership_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -75,15 +75,15 @@
     """
 
     is_active: bool # noqa: E501
     """
     [optional]
     """
 
-    joined_date: datetime # noqa: E501
+    joined_date: typing.Union[datetime, none_type] # noqa: E501
     """
     [optional]
     """
 
     role: typing.Union[typing.Any, none_type] # noqa: E501
     """
     [optional]
@@ -107,15 +107,15 @@
 
       id (int): [optional]  # noqa: E501
 
       organization (int): [optional]  # noqa: E501
 
       is_active (bool): [optional]  # noqa: E501
 
-      joined_date (datetime): [optional]  # noqa: E501
+      joined_date (datetime, none_type): [optional]  # noqa: E501
 
       role (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       invitation (str): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
@@ -165,15 +165,15 @@
         """
         lazy_import()
         return {
             'user': (BasicUser,),  # noqa: E501
             'id': (int,),  # noqa: E501
             'organization': (int,),  # noqa: E501
             'is_active': (bool,),  # noqa: E501
-            'joined_date': (datetime,),  # noqa: E501
+            'joined_date': (datetime, none_type,),  # noqa: E501
             'role': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'invitation': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -212,15 +212,15 @@
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             organization (int): [optional]  # noqa: E501
 
             is_active (bool): [optional]  # noqa: E501
 
-            joined_date (datetime): [optional]  # noqa: E501
+            joined_date (datetime, none_type): [optional]  # noqa: E501
 
             role (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             invitation (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -314,15 +314,15 @@
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             organization (int): [optional]  # noqa: E501
 
             is_active (bool): [optional]  # noqa: E501
 
-            joined_date (datetime): [optional]  # noqa: E501
+            joined_date (datetime, none_type): [optional]  # noqa: E501
 
             role (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             invitation (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/meta_user.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/meta_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/online_function_call_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/online_function_call_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/operation_status.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_method.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IOperationStatus(IModelData):
+class IStorageMethod(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "new", "in progress", "completed", "rejected"  # noqa: E501
+    One of: "cache", "file_system"  # noqa: E501
     """
 
-class OperationStatus(ModelSimple, IOperationStatus):
+class StorageMethod(ModelSimple, IStorageMethod):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,18 +78,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'NEW': "new",
-            'IN_PROGRESS': "in progress",
-            'COMPLETED': "completed",
-            'REJECTED': "rejected",
+            'CACHE': "cache",
+            'FILE_SYSTEM': "file_system",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -129,23 +127,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """OperationStatus - a model defined in OpenAPI
+        """StorageMethod - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
+            args[0] (str): * `cache` - CACHE * `file_system` - FILE_SYSTEM., must be one of ["cache", "file_system", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
+            value (str): * `cache` - CACHE * `file_system` - FILE_SYSTEM., must be one of ["cache", "file_system", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -225,23 +223,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """OperationStatus - a model defined in OpenAPI
+        """StorageMethod - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
+            args[0] (str): * `cache` - CACHE * `file_system` - FILE_SYSTEM., must be one of ["cache", "file_system", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
+            value (str): * `cache` - CACHE * `file_system` - FILE_SYSTEM., must be one of ["cache", "file_system", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_comment_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_comment_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_invitation_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_invitation_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_issue_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_issue_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_job_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_job_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_label_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_label_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_membership_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_membership_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_meta_user_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_meta_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_organization_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_organization_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_project_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_project_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_task_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_task_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_read_list.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_change_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_change_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_confirm_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_comment_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_membership_write_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,40 +39,44 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
+def lazy_import():
+    from cvat_sdk.api_client.model.role_enum import RoleEnum
+    globals()['RoleEnum'] = RoleEnum
 
 
-class IPatchedCommentWriteRequest(IModelData):
+
+class IPatchedMembershipWriteRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    message: str # noqa: E501
+    role: RoleEnum # noqa: E501
     """
     [optional]
     """
 
 
-class PatchedCommentWriteRequest(ModelNormal, IPatchedCommentWriteRequest):
+class PatchedMembershipWriteRequest(ModelNormal, IPatchedMembershipWriteRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      message (str): [optional]  # noqa: E501
+      role (RoleEnum): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -89,65 +93,64 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('message',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'message': (str,),  # noqa: E501
+            'role': (RoleEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'message': 'message',  # noqa: E501
+        'role': 'role',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchedCommentWriteRequest - a model defined in OpenAPI
+        """PatchedMembershipWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            message (str): [optional]  # noqa: E501
+            role (RoleEnum): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -224,18 +227,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchedCommentWriteRequest - a model defined in OpenAPI
+        """PatchedMembershipWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            message (str): [optional]  # noqa: E501
+            role (RoleEnum): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_data_meta_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_data_meta_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_invitation_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_issue_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_job_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_label_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_label_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_labeled_data_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_membership_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/signing_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,44 +39,39 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-def lazy_import():
-    from cvat_sdk.api_client.model.role_enum import RoleEnum
-    globals()['RoleEnum'] = RoleEnum
 
 
-
-class IPatchedMembershipWriteRequest(IModelData):
+class ISigningRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    role: RoleEnum # noqa: E501
+    url: str # noqa: E501
     """
-    [optional]
     """
 
 
-class PatchedMembershipWriteRequest(ModelNormal, IPatchedMembershipWriteRequest):
+class SigningRequest(ModelNormal, ISigningRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      role (RoleEnum): [optional]  # noqa: E501
+      url (str):
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -93,65 +88,67 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('url',): {
+            'min_length': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'role': (RoleEnum,),  # noqa: E501
+            'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'role': 'role',  # noqa: E501
+        'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchedMembershipWriteRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, url, *args, **kwargs):  # noqa: E501
+        """SigningRequest - a model defined in OpenAPI
 
-        Keyword Args:
-            role (RoleEnum): [optional]  # noqa: E501
+        Args:
+            url (str):
 
+        Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -206,14 +203,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -226,20 +224,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchedMembershipWriteRequest - a model defined in OpenAPI
+    def __init__(self, url, *args, **kwargs):  # noqa: E501
+        """SigningRequest - a model defined in OpenAPI
 
-        Keyword Args:
-            role (RoleEnum): [optional]  # noqa: E501
+        Args:
+            url (str):
 
+        Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -292,14 +291,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_organization_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_user_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_webhook_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/plugins.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_file_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_owner.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_owner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_target_storage.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/provider_type_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/role_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IProviderTypeEnum(IModelData):
+class IRoleEnum(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE"  # noqa: E501
+    One of: "worker", "supervisor", "maintainer", "owner"  # noqa: E501
     """
 
-class ProviderTypeEnum(ModelSimple, IProviderTypeEnum):
+class RoleEnum(ModelSimple, IRoleEnum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,18 +78,18 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'AWS_S3_BUCKET': "AWS_S3_BUCKET",
-            'AZURE_CONTAINER': "AZURE_CONTAINER",
-            'GOOGLE_DRIVE': "GOOGLE_DRIVE",
-            'GOOGLE_CLOUD_STORAGE': "GOOGLE_CLOUD_STORAGE",
+            'WORKER': "worker",
+            'SUPERVISOR': "supervisor",
+            'MAINTAINER': "maintainer",
+            'OWNER': "owner",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -129,23 +129,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ProviderTypeEnum - a model defined in OpenAPI
+        """RoleEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
+            args[0] (str): * `worker` - Worker * `supervisor` - Supervisor * `maintainer` - Maintainer * `owner` - Owner., must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
+            value (str): * `worker` - Worker * `supervisor` - Supervisor * `maintainer` - Maintainer * `owner` - Owner., must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -225,23 +225,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """ProviderTypeEnum - a model defined in OpenAPI
+        """RoleEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
+            args[0] (str): * `worker` - Worker * `supervisor` - Supervisor * `maintainer` - Maintainer * `owner` - Owner., must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
+            value (str): * `worker` - Worker * `supervisor` - Supervisor * `maintainer` - Maintainer * `owner` - Owner., must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/rest_auth_detail.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/role_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,111 +41,114 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IRoleEnum(IModelData):
+class IToken(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-    value: str
+    # member type declarations
+    key: str # noqa: E501
     """
-    [optional]
-
-    One of: "worker", "supervisor", "maintainer", "owner"  # noqa: E501
     """
 
-class RoleEnum(ModelSimple, IRoleEnum):
-    """NOTE: This class is auto generated by OpenAPI Generator.
+
+class Token(ModelNormal, IToken):
+    """
+    NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
+      key (str):
+
+
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
+
     """
 
     allowed_values = {
-        ('value',): {
-            'WORKER': "worker",
-            'SUPERVISOR': "supervisor",
-            'MAINTAINER': "maintainer",
-            'OWNER': "owner",
-        },
     }
 
     validations = {
+        ('key',): {
+            'max_length': 40,
+        },
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'key': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'key': 'key',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """RoleEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, key, *args, **kwargs):  # noqa: E501
+        """Token - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
+            key (str):
 
         Keyword Args:
-            value (str):, must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -168,37 +171,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-        """
+"""
         from cvat_sdk.api_client.configuration import Configuration
 
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -211,37 +202,43 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """RoleEnum - a model defined in OpenAPI
+        self.key = key
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    @convert_js_args_to_python_args
+    def __init__(self, key, *args, **kwargs):  # noqa: E501
+        """Token - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
+            key (str):
 
         Keyword Args:
-            value (str):, must be one of ["worker", "supervisor", "maintainer", "owner", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -264,36 +261,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-        """
+"""
         from cvat_sdk.api_client.configuration import Configuration
 
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -309,19 +290,21 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.key = key
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
+
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status_state_enum.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_file_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,111 +41,111 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IRqStatusStateEnum(IModelData):
+class ITaskFileRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-    value: str
+    # member type declarations
+    task_file: file_type # noqa: E501
     """
-    [optional]
-
-    One of: "Queued", "Started", "Finished", "Failed"  # noqa: E501
     """
 
-class RqStatusStateEnum(ModelSimple, IRqStatusStateEnum):
-    """NOTE: This class is auto generated by OpenAPI Generator.
+
+class TaskFileRequest(ModelNormal, ITaskFileRequest):
+    """
+    NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
+      task_file (file_type):
+
+
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
+
     """
 
     allowed_values = {
-        ('value',): {
-            'QUEUED': "Queued",
-            'STARTED': "Started",
-            'FINISHED': "Finished",
-            'FAILED': "Failed",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'task_file': (file_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'task_file': 'task_file',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """RqStatusStateEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, task_file, *args, **kwargs):  # noqa: E501
+        """TaskFileRequest - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
+            task_file (file_type):
 
         Keyword Args:
-            value (str):, must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -168,37 +168,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-        """
+"""
         from cvat_sdk.api_client.configuration import Configuration
 
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -211,37 +199,43 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """RqStatusStateEnum - a model defined in OpenAPI
+        self.task_file = task_file
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, task_file, *args, **kwargs):  # noqa: E501
+        """TaskFileRequest - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
+            task_file (file_type):
 
         Keyword Args:
-            value (str):, must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -264,36 +258,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-        """
+"""
         from cvat_sdk.api_client.configuration import Configuration
 
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -309,19 +287,21 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.task_file = task_file
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
+
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/shape_type.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/shape_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -138,18 +138,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """ShapeType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
+            args[0] (str): * `rectangle` - RECTANGLE * `polygon` - POLYGON * `polyline` - POLYLINE * `points` - POINTS * `ellipse` - ELLIPSE * `cuboid` - CUBOID * `mask` - MASK * `skeleton` - SKELETON., must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
+            value (str): * `rectangle` - RECTANGLE * `polygon` - POLYGON * `polyline` - POLYLINE * `points` - POINTS * `ellipse` - ELLIPSE * `cuboid` - CUBOID * `mask` - MASK * `skeleton` - SKELETON., must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -234,18 +234,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """ShapeType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
+            args[0] (str): * `rectangle` - RECTANGLE * `polygon` - POLYGON * `polyline` - POLYLINE * `points` - POINTS * `ellipse` - ELLIPSE * `cuboid` - CUBOID * `mask` - MASK * `skeleton` - SKELETON., must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
+            value (str): * `rectangle` - RECTANGLE * `polygon` - POLYGON * `polyline` - POLYLINE * `points` - POINTS * `ellipse` - ELLIPSE * `cuboid` - CUBOID * `mask` - MASK * `skeleton` - SKELETON., must be one of ["rectangle", "polygon", "polyline", "points", "ellipse", "cuboid", "mask", "skeleton", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/signing_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/tasks_summary.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,37 +41,45 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class ISigningRequest(IModelData):
+class ITasksSummary(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
+    count: int # noqa: E501
+    """
+    [optional, default: 0]
+    """
+
     url: str # noqa: E501
     """
+    [optional]
     """
 
 
-class SigningRequest(ModelNormal, ISigningRequest):
+class TasksSummary(ModelNormal, ITasksSummary):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      url (str):
+      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+
+      url (str): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -88,17 +96,14 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('url',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -114,41 +119,45 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'count': (int,),  # noqa: E501
             'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
+        'count': 'count',  # noqa: E501
         'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
+        'url',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, url, *args, **kwargs):  # noqa: E501
-        """SigningRequest - a model defined in OpenAPI
-
-        Args:
-            url (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TasksSummary - a model defined in OpenAPI
 
         Keyword Args:
+            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+
+            url (str): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -203,15 +212,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -224,21 +232,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, url, *args, **kwargs):  # noqa: E501
-        """SigningRequest - a model defined in OpenAPI
-
-        Args:
-            url (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TasksSummary - a model defined in OpenAPI
 
         Keyword Args:
+            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+
+            url (str): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -291,15 +300,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sorting_method.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sorting_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -134,18 +134,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """SortingMethod - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
+            args[0] (str): * `lexicographical` - LEXICOGRAPHICAL * `natural` - NATURAL * `predefined` - PREDEFINED * `random` - RANDOM., must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
+            value (str): * `lexicographical` - LEXICOGRAPHICAL * `natural` - NATURAL * `predefined` - PREDEFINED * `random` - RANDOM., must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -230,18 +230,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """SortingMethod - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
+            args[0] (str): * `lexicographical` - LEXICOGRAPHICAL * `natural` - NATURAL * `predefined` - PREDEFINED * `random` - RANDOM., must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
+            value (str): * `lexicographical` - LEXICOGRAPHICAL * `natural` - NATURAL * `predefined` - PREDEFINED * `random` - RANDOM., must be one of ["lexicographical", "natural", "predefined", "random", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_method.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IStorageMethod(IModelData):
+class IStorageType(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "cache", "file_system"  # noqa: E501
+    One of: "cloud_storage", "local", "share"  # noqa: E501
     """
 
-class StorageMethod(ModelSimple, IStorageMethod):
+class StorageType(ModelSimple, IStorageType):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,16 +78,17 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CACHE': "cache",
-            'FILE_SYSTEM': "file_system",
+            'CLOUD_STORAGE': "cloud_storage",
+            'LOCAL': "local",
+            'SHARE': "share",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -127,23 +128,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """StorageMethod - a model defined in OpenAPI
+        """StorageType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["cache", "file_system", ]  # noqa: E501
+            args[0] (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL * `share` - SHARE., must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["cache", "file_system", ]  # noqa: E501
+            value (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL * `share` - SHARE., must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -223,23 +224,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """StorageMethod - a model defined in OpenAPI
+        """StorageType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["cache", "file_system", ]  # noqa: E501
+            args[0] (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL * `share` - SHARE., must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["cache", "file_system", ]  # noqa: E501
+            value (str): * `cloud_storage` - CLOUD_STORAGE * `local` - LOCAL * `share` - SHARE., must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_type.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/credentials_type_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IStorageType(IModelData):
+class ICredentialsTypeEnum(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "cloud_storage", "local", "share"  # noqa: E501
+    One of: "KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING"  # noqa: E501
     """
 
-class StorageType(ModelSimple, IStorageType):
+class CredentialsTypeEnum(ModelSimple, ICredentialsTypeEnum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,17 +78,19 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CLOUD_STORAGE': "cloud_storage",
-            'LOCAL': "local",
-            'SHARE': "share",
+            'KEY_SECRET_KEY_PAIR': "KEY_SECRET_KEY_PAIR",
+            'ACCOUNT_NAME_TOKEN_PAIR': "ACCOUNT_NAME_TOKEN_PAIR",
+            'KEY_FILE_PATH': "KEY_FILE_PATH",
+            'ANONYMOUS_ACCESS': "ANONYMOUS_ACCESS",
+            'CONNECTION_STRING': "CONNECTION_STRING",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -128,23 +130,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """StorageType - a model defined in OpenAPI
+        """CredentialsTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
+            args[0] (str): * `KEY_SECRET_KEY_PAIR` - KEY_SECRET_KEY_PAIR * `ACCOUNT_NAME_TOKEN_PAIR` - ACCOUNT_NAME_TOKEN_PAIR * `KEY_FILE_PATH` - KEY_FILE_PATH * `ANONYMOUS_ACCESS` - ANONYMOUS_ACCESS * `CONNECTION_STRING` - CONNECTION_STRING., must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
+            value (str): * `KEY_SECRET_KEY_PAIR` - KEY_SECRET_KEY_PAIR * `ACCOUNT_NAME_TOKEN_PAIR` - ACCOUNT_NAME_TOKEN_PAIR * `KEY_FILE_PATH` - KEY_FILE_PATH * `ANONYMOUS_ACCESS` - ANONYMOUS_ACCESS * `CONNECTION_STRING` - CONNECTION_STRING., must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -224,23 +226,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """StorageType - a model defined in OpenAPI
+        """CredentialsTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
+            args[0] (str): * `KEY_SECRET_KEY_PAIR` - KEY_SECRET_KEY_PAIR * `ACCOUNT_NAME_TOKEN_PAIR` - ACCOUNT_NAME_TOKEN_PAIR * `KEY_FILE_PATH` - KEY_FILE_PATH * `ANONYMOUS_ACCESS` - ANONYMOUS_ACCESS * `CONNECTION_STRING` - CONNECTION_STRING., must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["cloud_storage", "local", "share", ]  # noqa: E501
+            value (str): * `KEY_SECRET_KEY_PAIR` - KEY_SECRET_KEY_PAIR * `ACCOUNT_NAME_TOKEN_PAIR` - ACCOUNT_NAME_TOKEN_PAIR * `KEY_FILE_PATH` - KEY_FILE_PATH * `ANONYMOUS_ACCESS` - ANONYMOUS_ACCESS * `CONNECTION_STRING` - CONNECTION_STRING., must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_update_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_file_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,39 +39,52 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
+def lazy_import():
+    from cvat_sdk.api_client.model.file_info import FileInfo
+    globals()['FileInfo'] = FileInfo
 
 
-class ITaskFileRequest(IModelData):
+
+class ICloudStorageContent(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    task_file: file_type # noqa: E501
+    next: typing.Union[str, none_type] # noqa: E501
+    """
+    [optional]
+    This token is used to continue listing files in the bucket..
+    """
+
+    content: typing.List[FileInfo] # noqa: E501
     """
+    [FileInfo]
     """
 
 
-class TaskFileRequest(ModelNormal, ITaskFileRequest):
+class CloudStorageContent(ModelNormal, ICloudStorageContent):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      task_file (file_type):
+      content ([FileInfo]):
+
+      next (str, none_type): This token is used to continue listing files in the bucket.. [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -96,56 +109,62 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'task_file': (file_type,),  # noqa: E501
+            'content': ([FileInfo],),  # noqa: E501
+            'next': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'task_file': 'task_file',  # noqa: E501
+        'content': 'content',  # noqa: E501
+        'next': 'next',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, task_file, *args, **kwargs):  # noqa: E501
-        """TaskFileRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, content, *args, **kwargs):  # noqa: E501
+        """CloudStorageContent - a model defined in OpenAPI
 
         Args:
-            task_file (file_type):
+            content ([FileInfo]):
 
         Keyword Args:
+            next (str, none_type): This token is used to continue listing files in the bucket.. [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -200,15 +219,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.task_file = task_file
+        self.content = content
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -221,21 +240,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, task_file, *args, **kwargs):  # noqa: E501
-        """TaskFileRequest - a model defined in OpenAPI
+    def __init__(self, content, *args, **kwargs):  # noqa: E501
+        """CloudStorageContent - a model defined in OpenAPI
 
         Args:
-            task_file (file_type):
+            content ([FileInfo]):
 
         Keyword Args:
+            next (str, none_type): This token is used to continue listing files in the bucket.. [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -288,15 +309,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.task_file = task_file
+        self.content = content
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read_target_storage.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/tasks_summary.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/operation_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,123 +41,111 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class ITasksSummary(IModelData):
+class IOperationStatus(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-    # member type declarations
-    count: int # noqa: E501
-    """
-    [optional, default: 0]
-    """
-
-    url: str # noqa: E501
+    value: str
     """
     [optional]
-    """
 
-
-class TasksSummary(ModelNormal, ITasksSummary):
+    One of: "new", "in progress", "completed", "rejected"  # noqa: E501
     """
-    NOTE: This class is auto generated by OpenAPI Generator.
+
+class OperationStatus(ModelSimple, IOperationStatus):
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
-      url (str): [optional]  # noqa: E501
-
-
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
-
     """
 
     allowed_values = {
+        ('value',): {
+            'NEW': "new",
+            'IN_PROGRESS': "in progress",
+            'COMPLETED': "completed",
+            'REJECTED': "rejected",
+        },
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'count': (int,),  # noqa: E501
-            'url': (str,),  # noqa: E501
+            'value': (str,),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
-    attribute_map = {
-        'count': 'count',  # noqa: E501
-        'url': 'url',  # noqa: E501
-    }
+    attribute_map = {}
 
-    read_only_vars = {
-        'url',  # noqa: E501
-    }
+    read_only_vars = set()
 
-    _composed_schemas = {}
+    _composed_schemas = None
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-    @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TasksSummary - a model defined in OpenAPI
+    def __init__(self, *args, **kwargs):
+        """OperationStatus - a model defined in OpenAPI
 
-        Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+        Note that value can be passed either in args or in kwargs, but not in both.
 
-            url (str): [optional]  # noqa: E501
+        Args:
+            args[0] (str): * `new` - NEW * `in progress` - IN_PROGRESS * `completed` - COMPLETED * `rejected` - REJECTED., must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
 
+        Keyword Args:
+            value (str): * `new` - NEW * `in progress` - IN_PROGRESS * `completed` - COMPLETED * `rejected` - REJECTED., must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -180,25 +168,37 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-"""
+        """
         from cvat_sdk.api_client.configuration import Configuration
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        # required up here when default value is not given
         _path_to_item = kwargs.pop('_path_to_item', ())
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
-        self = super(OpenApiModel, cls).__new__(cls)
-
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -211,43 +211,37 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """TasksSummary - a model defined in OpenAPI
+    def _from_openapi_data(cls, *args, **kwargs):
+        """OperationStatus - a model defined in OpenAPI
 
-        Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+        Note that value can be passed either in args or in kwargs, but not in both.
 
-            url (str): [optional]  # noqa: E501
+        Args:
+            args[0] (str): * `new` - NEW * `in progress` - IN_PROGRESS * `completed` - COMPLETED * `rejected` - REJECTED., must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
 
+        Keyword Args:
+            value (str): * `new` - NEW * `in progress` - IN_PROGRESS * `completed` - COMPLETED * `rejected` - REJECTED., must be one of ["new", "in progress", "completed", "rejected", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -270,20 +264,36 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-"""
+        """
         from cvat_sdk.api_client.configuration import Configuration
 
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
+
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -299,20 +309,19 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
-
+        return self
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/token.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status_state_enum.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,114 +41,111 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IToken(IModelData):
+class IRqStatusStateEnum(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-    # member type declarations
-    key: str # noqa: E501
+    value: str
     """
-    """
-
+    [optional]
 
-class Token(ModelNormal, IToken):
+    One of: "Queued", "Started", "Finished", "Failed"  # noqa: E501
     """
-    NOTE: This class is auto generated by OpenAPI Generator.
+
+class RqStatusStateEnum(ModelSimple, IRqStatusStateEnum):
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      key (str):
-
-
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
-
     """
 
     allowed_values = {
+        ('value',): {
+            'QUEUED': "Queued",
+            'STARTED': "Started",
+            'FINISHED': "Finished",
+            'FAILED': "Failed",
+        },
     }
 
     validations = {
-        ('key',): {
-            'max_length': 40,
-        },
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'key': (str,),  # noqa: E501
+            'value': (str,),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
-    attribute_map = {
-        'key': 'key',  # noqa: E501
-    }
+    attribute_map = {}
 
-    read_only_vars = {
-    }
+    read_only_vars = set()
 
-    _composed_schemas = {}
+    _composed_schemas = None
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-    @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, key, *args, **kwargs):  # noqa: E501
-        """Token - a model defined in OpenAPI
+    def __init__(self, *args, **kwargs):
+        """RqStatusStateEnum - a model defined in OpenAPI
+
+        Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            key (str):
+            args[0] (str): * `Queued` - Queued * `Started` - Started * `Finished` - Finished * `Failed` - Failed., must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
 
         Keyword Args:
+            value (str): * `Queued` - Queued * `Started` - Started * `Finished` - Finished * `Failed` - Failed., must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -171,25 +168,37 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-"""
+        """
         from cvat_sdk.api_client.configuration import Configuration
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        # required up here when default value is not given
         _path_to_item = kwargs.pop('_path_to_item', ())
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
-        self = super(OpenApiModel, cls).__new__(cls)
-
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -202,43 +211,37 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
-        self.key = key
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, key, *args, **kwargs):  # noqa: E501
-        """Token - a model defined in OpenAPI
+    def _from_openapi_data(cls, *args, **kwargs):
+        """RqStatusStateEnum - a model defined in OpenAPI
+
+        Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            key (str):
+            args[0] (str): * `Queued` - Queued * `Started` - Started * `Finished` - Finished * `Failed` - Failed., must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
 
         Keyword Args:
+            value (str): * `Queued` - Queued * `Started` - Started * `Finished` - Finished * `Failed` - Failed., must be one of ["Queued", "Started", "Finished", "Failed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -261,20 +264,36 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-"""
+        """
         from cvat_sdk.api_client.configuration import Configuration
 
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
+
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -290,21 +309,19 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
-        self.key = key
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
-
+        return self
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/user.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_content_type.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/input_type_enum.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IWebhookContentType(IModelData):
+class IInputTypeEnum(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
-    [optional, default: "application/json"]
+    [optional]
 
-    One of: "application/json"  # noqa: E501
+    One of: "checkbox", "radio", "number", "text", "select"  # noqa: E501
     """
 
-class WebhookContentType(ModelSimple, IWebhookContentType):
+class InputTypeEnum(ModelSimple, IInputTypeEnum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,15 +78,19 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'APPLICATION/JSON': "application/json",
+            'CHECKBOX': "checkbox",
+            'RADIO': "radio",
+            'NUMBER': "number",
+            'TEXT': "text",
+            'SELECT': "select",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -126,23 +130,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """WebhookContentType - a model defined in OpenAPI
+        """InputTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
+            args[0] (str): * `checkbox` - CHECKBOX * `radio` - RADIO * `number` - NUMBER * `text` - TEXT * `select` - SELECT., must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
+            value (str): * `checkbox` - CHECKBOX * `radio` - RADIO * `number` - NUMBER * `text` - TEXT * `select` - SELECT., must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -177,15 +181,19 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "application/json"
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -218,23 +226,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """WebhookContentType - a model defined in OpenAPI
+        """InputTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
+            args[0] (str): * `checkbox` - CHECKBOX * `radio` - RADIO * `number` - NUMBER * `text` - TEXT * `select` - SELECT., must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "application/json", must be one of ["application/json", ]  # noqa: E501
+            value (str): * `checkbox` - CHECKBOX * `radio` - RADIO * `number` - NUMBER * `text` - TEXT * `select` - SELECT., must be one of ["checkbox", "radio", "number", "text", "select", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -271,15 +279,19 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "application/json"
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_delivery_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_delivery_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -65,15 +65,15 @@
     """
 
     event: str # noqa: E501
     """
     [optional]
     """
 
-    status_code: int # noqa: E501
+    status_code: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
     redelivery: bool # noqa: E501
     """
     [optional]
@@ -117,15 +117,15 @@
     Attributes:
       id (int): [optional]  # noqa: E501
 
       webhook_id (int): [optional]  # noqa: E501
 
       event (str): [optional]  # noqa: E501
 
-      status_code (int): [optional]  # noqa: E501
+      status_code (int, none_type): [optional]  # noqa: E501
 
       redelivery (bool): [optional]  # noqa: E501
 
       created_date (datetime): [optional]  # noqa: E501
 
       updated_date (datetime): [optional]  # noqa: E501
 
@@ -180,15 +180,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (int,),  # noqa: E501
             'webhook_id': (int,),  # noqa: E501
             'event': (str,),  # noqa: E501
-            'status_code': (int,),  # noqa: E501
+            'status_code': (int, none_type,),  # noqa: E501
             'redelivery': (bool,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
             'changed_fields': (str,),  # noqa: E501
             'request': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'response': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
@@ -235,15 +235,15 @@
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             webhook_id (int): [optional]  # noqa: E501
 
             event (str): [optional]  # noqa: E501
 
-            status_code (int): [optional]  # noqa: E501
+            status_code (int, none_type): [optional]  # noqa: E501
 
             redelivery (bool): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
@@ -341,15 +341,15 @@
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             webhook_id (int): [optional]  # noqa: E501
 
             event (str): [optional]  # noqa: E501
 
-            status_code (int): [optional]  # noqa: E501
+            status_code (int, none_type): [optional]  # noqa: E501
 
             redelivery (bool): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_read.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_type.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/provider_type_enum.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,30 +41,30 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IWebhookType(IModelData):
+class IProviderTypeEnum(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "organization", "project"  # noqa: E501
+    One of: "AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE"  # noqa: E501
     """
 
-class WebhookType(ModelSimple, IWebhookType):
+class ProviderTypeEnum(ModelSimple, IProviderTypeEnum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,16 +78,18 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'ORGANIZATION': "organization",
-            'PROJECT': "project",
+            'AWS_S3_BUCKET': "AWS_S3_BUCKET",
+            'AZURE_CONTAINER': "AZURE_CONTAINER",
+            'GOOGLE_DRIVE': "GOOGLE_DRIVE",
+            'GOOGLE_CLOUD_STORAGE': "GOOGLE_CLOUD_STORAGE",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -127,23 +129,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """WebhookType - a model defined in OpenAPI
+        """ProviderTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["organization", "project", ]  # noqa: E501
+            args[0] (str): * `AWS_S3_BUCKET` - AWS_S3 * `AZURE_CONTAINER` - AZURE_CONTAINER * `GOOGLE_DRIVE` - GOOGLE_DRIVE * `GOOGLE_CLOUD_STORAGE` - GOOGLE_CLOUD_STORAGE., must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["organization", "project", ]  # noqa: E501
+            value (str): * `AWS_S3_BUCKET` - AWS_S3 * `AZURE_CONTAINER` - AZURE_CONTAINER * `GOOGLE_DRIVE` - GOOGLE_DRIVE * `GOOGLE_CLOUD_STORAGE` - GOOGLE_CLOUD_STORAGE., must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -223,23 +225,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """WebhookType - a model defined in OpenAPI
+        """ProviderTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["organization", "project", ]  # noqa: E501
+            args[0] (str): * `AWS_S3_BUCKET` - AWS_S3 * `AZURE_CONTAINER` - AZURE_CONTAINER * `GOOGLE_DRIVE` - GOOGLE_DRIVE * `GOOGLE_CLOUD_STORAGE` - GOOGLE_CLOUD_STORAGE., must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["organization", "project", ]  # noqa: E501
+            value (str): * `AWS_S3_BUCKET` - AWS_S3 * `AZURE_CONTAINER` - AZURE_CONTAINER * `GOOGLE_DRIVE` - GOOGLE_DRIVE * `GOOGLE_CLOUD_STORAGE` - GOOGLE_CLOUD_STORAGE., must be one of ["AWS_S3_BUCKET", "AZURE_CONTAINER", "GOOGLE_DRIVE", "GOOGLE_CLOUD_STORAGE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_write_request.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/model_utils.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/models/__init__.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
@@ -29,14 +29,15 @@
 from cvat_sdk.api_client.model.attribute_val_request import AttributeValRequest, IAttributeValRequest
 from cvat_sdk.api_client.model.backup_write_request import BackupWriteRequest
 from cvat_sdk.api_client.model.basic_user import BasicUser, IBasicUser
 from cvat_sdk.api_client.model.basic_user_request import BasicUserRequest, IBasicUserRequest
 from cvat_sdk.api_client.model.chunk_type import ChunkType, IChunkType
 from cvat_sdk.api_client.model.client_events import ClientEvents, IClientEvents
 from cvat_sdk.api_client.model.client_events_request import ClientEventsRequest, IClientEventsRequest
+from cvat_sdk.api_client.model.cloud_storage_content import CloudStorageContent, ICloudStorageContent
 from cvat_sdk.api_client.model.cloud_storage_read import CloudStorageRead, ICloudStorageRead
 from cvat_sdk.api_client.model.cloud_storage_write_request import CloudStorageWriteRequest, ICloudStorageWriteRequest
 from cvat_sdk.api_client.model.comment_read import CommentRead, ICommentRead
 from cvat_sdk.api_client.model.comment_read_owner import CommentReadOwner
 from cvat_sdk.api_client.model.comment_write_request import CommentWriteRequest, ICommentWriteRequest
 from cvat_sdk.api_client.model.comments_summary import CommentsSummary, ICommentsSummary
 from cvat_sdk.api_client.model.credentials_type_enum import CredentialsTypeEnum, ICredentialsTypeEnum
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/api_client/rest.py` & `cvat_sdk-2.4.5/cvat_sdk/api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import io
 import json
 import logging
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/client.py` & `cvat_sdk-2.4.5/cvat_sdk/core/client.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/downloading.py` & `cvat_sdk-2.4.5/cvat_sdk/core/downloading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/git.py` & `cvat_sdk-2.4.5/cvat_sdk/core/git.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/helpers.py` & `cvat_sdk-2.4.5/cvat_sdk/core/helpers.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/progress.py` & `cvat_sdk-2.4.5/cvat_sdk/core/progress.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/annotations.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/annotations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/issues.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/issues.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/jobs.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/jobs.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/model_proxy.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/model_proxy.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/organizations.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/organizations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/projects.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/projects.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/tasks.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
                     "start_frame",
                     "stop_frame",
                     "use_cache",
                     "use_zip_chunks",
                     "job_file_mapping",
                     "filename_pattern",
                     "cloud_storage_id",
+                    "server_files_exclude",
                 ],
             )
         )
         if params.get("frame_step") is not None:
             data["frame_filter"] = f"step={params.get('frame_step')}"
 
         if resource_type in [ResourceType.REMOTE, ResourceType.SHARE]:
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/proxies/users.py` & `cvat_sdk-2.4.5/cvat_sdk/core/proxies/users.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/uploading.py` & `cvat_sdk-2.4.5/cvat_sdk/core/uploading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/core/utils.py` & `cvat_sdk-2.4.5/cvat_sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/pytorch/caching.py` & `cvat_sdk-2.4.5/cvat_sdk/pytorch/caching.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/pytorch/common.py` & `cvat_sdk-2.4.5/cvat_sdk/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/pytorch/project_dataset.py` & `cvat_sdk-2.4.5/cvat_sdk/pytorch/project_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/pytorch/task_dataset.py` & `cvat_sdk-2.4.5/cvat_sdk/pytorch/task_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk/pytorch/transforms.py` & `cvat_sdk-2.4.5/cvat_sdk/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.4/cvat_sdk.egg-info/PKG-INFO` & `cvat_sdk-2.4.5/cvat_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-sdk
-Version: 2.4.4
+Version: 2.4.5
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.4/cvat_sdk.egg-info/SOURCES.txt` & `cvat_sdk-2.4.5/cvat_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 ./cvat_sdk/api_client/model/attribute_val_request.py
 ./cvat_sdk/api_client/model/backup_write_request.py
 ./cvat_sdk/api_client/model/basic_user.py
 ./cvat_sdk/api_client/model/basic_user_request.py
 ./cvat_sdk/api_client/model/chunk_type.py
 ./cvat_sdk/api_client/model/client_events.py
 ./cvat_sdk/api_client/model/client_events_request.py
+./cvat_sdk/api_client/model/cloud_storage_content.py
 ./cvat_sdk/api_client/model/cloud_storage_read.py
 ./cvat_sdk/api_client/model/cloud_storage_write_request.py
 ./cvat_sdk/api_client/model/comment_read.py
 ./cvat_sdk/api_client/model/comment_read_owner.py
 ./cvat_sdk/api_client/model/comment_write_request.py
 ./cvat_sdk/api_client/model/comments_summary.py
 ./cvat_sdk/api_client/model/credentials_type_enum.py
```

### Comparing `cvat_sdk-2.4.4/setup.py` & `cvat_sdk-2.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.4
+# The version of the OpenAPI document: 2.4.5
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import os.path as osp
 import re
 from setuptools import find_packages, setup
```

