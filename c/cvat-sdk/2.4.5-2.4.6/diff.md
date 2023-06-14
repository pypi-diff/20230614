# Comparing `tmp/cvat_sdk-2.4.5.tar.gz` & `tmp/cvat_sdk-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk-2.4.5.tar", last modified: Wed Jun 14 19:50:01 2023, max compression
+gzip compressed data, was "cvat_sdk-2.4.6.tar", last modified: Wed Jun 14 19:55:23 2023, max compression
```

## Comparing `cvat_sdk-2.4.5.tar` & `cvat_sdk-2.4.6.tar`

### file list

```diff
@@ -1,218 +1,219 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.5/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.5/README.md
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/api_client/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/api_client/api/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45482 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/auth_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    60847 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/cloudstorages_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31362 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/comments_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15007 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/events_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30677 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/invitations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31852 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/issues_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    78813 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/jobs_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    26714 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/labels_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33079 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/lambda_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    24997 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/memberships_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    29848 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/organizations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    73158 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/projects_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    10673 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/schema_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21217 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/server_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)   128040 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/tasks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30201 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/users_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    66165 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api/webhooks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45222 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/api_client.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.126666 cvat_sdk-2.4.5/cvat_sdk/api_client/apis/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1711 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/apis/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/configuration.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/exceptions.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.166667 cvat_sdk-2.4.5/cvat_sdk/api_client/model/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/about.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotation_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotations_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/backup_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13023 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/chunk_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13139 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_content.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/comments_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14282 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/credentials_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15330 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_meta_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31709 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_format.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_formats.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/event.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/event_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18731 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/events_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12821 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/frame_meta.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13367 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/input_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/issues_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21389 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read_assignee.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_stage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13203 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/jobs_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/label.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/labels_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12981 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/location_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/login_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14975 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/membership_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/meta_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/online_function_call_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13335 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/operation_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_comment_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_invitation_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_issue_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_job_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_label_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_membership_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_meta_user_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_organization_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_project_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_task_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_change_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_confirm_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_data_meta_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_label_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_membership_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/plugins.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13747 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/provider_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/rest_auth_detail.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13300 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/role_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13285 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status_state_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13953 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/signing_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13430 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sorting_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12956 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13123 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/tasks_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/token.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12666 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_content_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16432 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_delivery_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12991 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/model_utils.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.166667 cvat_sdk-2.4.5/cvat_sdk/api_client/models/
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13607 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/models/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/api_client/rest.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.166667 cvat_sdk-2.4.5/cvat_sdk/core/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/client.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/downloading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/git.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/helpers.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/progress.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/cvat_sdk/core/proxies/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/annotations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/issues.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/jobs.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/model_proxy.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/organizations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/projects.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14268 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/tasks.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/proxies/users.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13947 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/uploading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/core/utils.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/models.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/cvat_sdk/pytorch/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/caching.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/common.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/project_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/task_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/pytorch/transforms.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-14 19:49:20.000000 cvat_sdk-2.4.5/cvat_sdk/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/cvat_sdk.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     9232 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-14 19:50:01.000000 cvat_sdk-2.4.5/cvat_sdk.egg-info/top_level.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.5/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-06-14 19:49:19.000000 cvat_sdk-2.4.5/requirements/api_client.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.5/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-14 19:50:01.176667 cvat_sdk-2.4.5/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-06-14 19:49:19.000000 cvat_sdk-2.4.5/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.6/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.6/README.md
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/api_client/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/api_client/api/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45482 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/auth_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    60873 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/cloudstorages_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31388 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/comments_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15033 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/events_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30703 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/invitations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31878 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/issues_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    79891 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/jobs_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    26740 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/labels_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33105 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/lambda_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24997 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/memberships_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    29848 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/organizations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    75123 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/projects_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    10673 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/schema_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21217 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/server_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)   131955 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/tasks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30201 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/users_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    66191 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/webhooks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45222 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api_client.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/api_client/apis/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1711 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/apis/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/configuration.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/exceptions.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/api_client/model/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/about.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotation_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotations_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/backup_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13023 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/chunk_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13139 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_content.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comments_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14282 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/credentials_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15330 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_meta_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33482 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_format.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_formats.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/event.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/event_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18731 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/events_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12821 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/frame_meta.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13367 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/input_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/issues_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21389 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read_assignee.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_stage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13203 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/jobs_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/label.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labels_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12981 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/location_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/login_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14975 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/membership_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/meta_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/online_function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13335 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/operation_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_comment_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_invitation_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_issue_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_job_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_label_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_membership_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_meta_user_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_organization_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_project_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_task_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_change_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_confirm_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_data_meta_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_label_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_membership_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/plugins.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13747 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/provider_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rest_auth_detail.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13300 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/role_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12215 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_id.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13285 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status_state_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13953 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/signing_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13430 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sorting_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12956 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13123 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/tasks_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/token.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12666 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_content_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16432 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_delivery_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12991 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model_utils.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/api_client/models/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13663 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/models/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/rest.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/core/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/client.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/downloading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/git.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/helpers.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/progress.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/core/proxies/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/annotations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/issues.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/jobs.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/model_proxy.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/organizations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/projects.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14269 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/tasks.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/users.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14651 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/uploading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/utils.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/models.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/cvat_sdk/pytorch/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/caching.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/common.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/project_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/task_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/transforms.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/cvat_sdk.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     9269 2023-06-14 19:55:23.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/top_level.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.6/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-06-14 19:54:47.000000 cvat_sdk-2.4.6/requirements/api_client.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.6/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-06-14 19:54:47.000000 cvat_sdk-2.4.6/setup.py
```

### Comparing `cvat_sdk-2.4.5/PKG-INFO` & `cvat_sdk-2.4.6/cvat_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cvat_sdk
-Version: 2.4.5
+Name: cvat-sdk
+Version: 2.4.6
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.5/README.md` & `cvat_sdk-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/__init__.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
-__version__ = "2.4.5"
+__version__ = "2.4.6"
 
 from cvat_sdk.api_client.api_client import ApiClient
 
 from cvat_sdk.api_client.configuration import Configuration
 
 from cvat_sdk.api_client.exceptions import OpenApiException
 from cvat_sdk.api_client.exceptions import ApiAttributeError
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/auth_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/auth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/cloudstorages_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/cloudstorages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -744,15 +744,15 @@
         >>> thread = api.create(cloud_storage_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             cloud_storage_write_request (CloudStorageWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/comments_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/comments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -421,15 +421,15 @@
         >>> thread = api.create(comment_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             comment_write_request (CommentWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/events_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/events_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -244,15 +244,15 @@
         >>> thread = api.create(client_events_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             client_events_request (ClientEventsRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/invitations_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/invitations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -406,15 +406,15 @@
         >>> thread = api.create(invitation_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             invitation_write_request (InvitationWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/issues_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/issues_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -431,15 +431,15 @@
         >>> thread = api.create(issue_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             issue_write_request (IssueWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/jobs_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/jobs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -29,14 +29,15 @@
 from cvat_sdk.api_client.model.annotations_read import AnnotationsRead
 from cvat_sdk.api_client.model.data_meta_read import DataMetaRead
 from cvat_sdk.api_client.model.job_annotations_update_request import JobAnnotationsUpdateRequest
 from cvat_sdk.api_client.model.job_read import JobRead
 from cvat_sdk.api_client.model.paginated_job_read_list import PaginatedJobReadList
 from cvat_sdk.api_client.model.patched_job_write_request import PatchedJobWriteRequest
 from cvat_sdk.api_client.model.patched_labeled_data_request import PatchedLabeledDataRequest
+from cvat_sdk.api_client.model.rq_id import RqId
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
@@ -132,15 +133,17 @@
                     'location': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
@@ -934,14 +937,15 @@
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                     'format',
+                    'rq_id',
                     'job_annotations_update_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -956,24 +960,28 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
                     'format':
                         (str,),
+                    'rq_id':
+                        (str,),
                     'job_annotations_update_request':
                         (JobAnnotationsUpdateRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'format': 'format',
+                    'rq_id': 'rq_id',
                 },
                 'location_map': {
                     'id': 'path',
                     'format': 'query',
+                    'rq_id': 'query',
                     'job_annotations_update_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -998,16 +1006,17 @@
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method allows to upload job annotations  # noqa: E501
+        """Method allows to initialize the process of the job annotation upload from a local file or a cloud storage  # noqa: E501
 
+         The request POST /api/jobs/id/annotations will initiate file upload and will create the rq job on the server in which the process of annotations uploading from file will be carried out. Please, use the PUT /api/jobs/id/annotations endpoint for checking status of the process.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.create_annotations(id, annotation_file_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
@@ -1897,27 +1906,29 @@
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method performs an update of all annotations in a specific job  # noqa: E501
+        """Method performs an update of all annotations in a specific job or used for uploading annotations from a file  # noqa: E501
 
+         To check the status of the process of uploading a job annotations from a file:  After initiating the annotations upload, you will receive an rq_id parameter. Make sure to include this parameter as a query parameter in your subsequent PUT /api/jobs/id/annotations requests to track the status of the annotations upload.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.update_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
+            rq_id (str): rq id. [optional]
             job_annotations_update_request (JobAnnotationsUpdateRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/labels_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/labels_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -458,15 +458,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             color (str): A simple equality filter for the color field. [optional]
             filter (str): A filter term. Available filter_fields: ['name', 'parent', 'id', 'type', 'color', 'parent_id']. [optional]
             job_id (int): A simple equality filter for job id. [optional]
             name (str): A simple equality filter for the name field. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             page (int): A page number within the paginated result set.. [optional]
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/lambda_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/lambda_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -481,15 +481,15 @@
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.create_requests(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/memberships_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/organizations_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/projects_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/projects_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -28,14 +28,15 @@
 from cvat_sdk.api_client.model.annotations_read import AnnotationsRead
 from cvat_sdk.api_client.model.backup_write_request import BackupWriteRequest
 from cvat_sdk.api_client.model.dataset_write_request import DatasetWriteRequest
 from cvat_sdk.api_client.model.paginated_project_read_list import PaginatedProjectReadList
 from cvat_sdk.api_client.model.patched_project_write_request import PatchedProjectWriteRequest
 from cvat_sdk.api_client.model.project_read import ProjectRead
 from cvat_sdk.api_client.model.project_write_request import ProjectWriteRequest
+from cvat_sdk.api_client.model.rq_id import RqId
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
@@ -141,14 +142,15 @@
                 'all': [
                     'x_organization',
                     'cloud_storage_id',
                     'filename',
                     'location',
                     'org',
                     'org_id',
+                    'rq_id',
                     'backup_write_request',
                 ],
                 'required': [],
                 'nullable': [
                     'backup_write_request',
                 ],
                 'enum': [
@@ -176,49 +178,55 @@
                         (str,),
                     'location':
                         (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
+                    'rq_id':
+                        (str,),
                     'backup_write_request':
                         (BackupWriteRequest,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
                     'org': 'org',
                     'org_id': 'org_id',
+                    'rq_id': 'rq_id',
                 },
                 'location_map': {
                     'x_organization': 'header',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
                     'org': 'query',
                     'org_id': 'query',
+                    'rq_id': 'query',
                     'backup_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.create_dataset_endpoint = _Endpoint(
             settings={
-                'response_schema': None,
+                'response_schema': (RqId,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
@@ -292,15 +300,17 @@
                     'use_default_location': 'query',
                     'dataset_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
@@ -793,14 +803,15 @@
                 'all': [
                     'id',
                     'action',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
+                    'rq_id',
                     'use_default_location',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -835,33 +846,37 @@
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
+                    'rq_id':
+                        (str,),
                     'use_default_location':
                         (bool,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'action': 'action',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
+                    'rq_id': 'rq_id',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
                     'action': 'query',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
+                    'rq_id': 'query',
                     'use_default_location': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -949,15 +964,15 @@
         >>> thread = api.create(project_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             project_write_request (ProjectWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1019,28 +1034,30 @@
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
         """Methods create a project from a backup  # noqa: E501
 
+         The backup import process is as follows:  The first request POST /api/projects/backup will initiate file upload and will create the rq job on the server in which the process of a project creating from an uploaded backup will be carried out.  After initiating the backup upload, you will receive an rq_id parameter. Make sure to include this parameter as a query parameter in your subsequent requests to track the status of the project creation. Once the project has been successfully created, the server will return the id of the newly created project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.create_backup(_async_call=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Backup file name. [optional]
             location (str): Where to import the backup file from. [optional] if omitted the server will use the default value of "local"
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
+            rq_id (str): rq id. [optional]
             backup_write_request (BackupWriteRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -1098,17 +1115,18 @@
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Import dataset in specific format as a project  # noqa: E501
+    ) -> typing.Tuple[typing.Optional[RqId], urllib3.HTTPResponse]:
+        """Import dataset in specific format as a project or check status of dataset import process  # noqa: E501
 
+         The request POST /api/projects/id/dataset will initiate file upload and will create the rq job on the server in which the process of dataset import from a file will be carried out. Please, use the GET /api/projects/id/dataset endpoint for checking status of the process.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.create_dataset(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
@@ -1150,15 +1168,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (None, HTTPResponse)
+            (RqId, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
@@ -1675,14 +1693,15 @@
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[file_type], urllib3.HTTPResponse]:
         """Export project as a dataset in a specific format  # noqa: E501
 
+         To check the status of the process of importing a project dataset from a file:  After initiating the dataset upload, you will receive an rq_id parameter. Make sure to include this parameter as a query parameter in your subsequent GET /api/projects/id/dataset requests to track the status of the dataset import. Also you should specify action parameter: action=import_status.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.retrieve_dataset(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
@@ -1690,14 +1709,15 @@
 
         Keyword Args:
             action (str): Used to start downloading process after annotation file had been created. [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Desired output file name. [optional]
             format (str): Desired output format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): Where need to save downloaded dataset. [optional]
+            rq_id (str): rq id. [optional]
             use_default_location (bool): Use the location that was configured in project to import dataset. [optional] if omitted the server will use the default value of True
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/schema_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/server_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/tasks_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/tasks_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -29,14 +29,15 @@
 from cvat_sdk.api_client.model.data_meta_read import DataMetaRead
 from cvat_sdk.api_client.model.data_request import DataRequest
 from cvat_sdk.api_client.model.labeled_data import LabeledData
 from cvat_sdk.api_client.model.paginated_task_read_list import PaginatedTaskReadList
 from cvat_sdk.api_client.model.patched_data_meta_write_request import PatchedDataMetaWriteRequest
 from cvat_sdk.api_client.model.patched_labeled_data_request import PatchedLabeledDataRequest
 from cvat_sdk.api_client.model.patched_task_write_request import PatchedTaskWriteRequest
+from cvat_sdk.api_client.model.rq_id import RqId
 from cvat_sdk.api_client.model.rq_status import RqStatus
 from cvat_sdk.api_client.model.task_annotations_update_request import TaskAnnotationsUpdateRequest
 from cvat_sdk.api_client.model.task_annotations_write_request import TaskAnnotationsWriteRequest
 from cvat_sdk.api_client.model.task_file_request import TaskFileRequest
 from cvat_sdk.api_client.model.task_read import TaskRead
 from cvat_sdk.api_client.model.task_write_request import TaskWriteRequest
 
@@ -270,15 +271,17 @@
                     'use_default_location': 'query',
                     'task_annotations_write_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
@@ -302,14 +305,15 @@
                     'task_file_request',
                     'x_organization',
                     'cloud_storage_id',
                     'filename',
                     'location',
                     'org',
                     'org_id',
+                    'rq_id',
                 ],
                 'required': [
                     'task_file_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -339,37 +343,43 @@
                         (str,),
                     'location':
                         (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
+                    'rq_id':
+                        (str,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
                     'org': 'org',
                     'org_id': 'org_id',
+                    'rq_id': 'rq_id',
                 },
                 'location_map': {
                     'task_file_request': 'body',
                     'x_organization': 'header',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
                     'org': 'query',
                     'org_id': 'query',
+                    'rq_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
@@ -1499,14 +1509,15 @@
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                     'format',
+                    'rq_id',
                     'task_annotations_update_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                     'task_annotations_update_request',
@@ -1522,24 +1533,28 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
                     'format':
                         (str,),
+                    'rq_id':
+                        (str,),
                     'task_annotations_update_request':
                         (TaskAnnotationsUpdateRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'format': 'format',
+                    'rq_id': 'rq_id',
                 },
                 'location_map': {
                     'id': 'path',
                     'format': 'query',
+                    'rq_id': 'query',
                     'task_annotations_update_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -1654,15 +1669,15 @@
         >>> thread = api.create(task_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             task_write_request (TaskWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1723,16 +1738,17 @@
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method allows to upload task annotations from a local file or a cloud storage  # noqa: E501
+        """Method allows to initialize the  process of upload task annotations from a local or a cloud storage file  # noqa: E501
 
+         The request POST /api/tasks/id/annotations will initiate file upload and will create the rq job on the server in which the process of annotations uploading from file will be carried out. Please, use the PUT /api/tasks/id/annotations endpoint for checking status of the process.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.create_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
@@ -1809,30 +1825,32 @@
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
         """Method recreates a task from an attached task backup file  # noqa: E501
 
+         The backup import process is as follows:  The first request POST /api/tasks/backup will initiate file upload and will create the rq job on the server in which the process of a task creating from an uploaded backup will be carried out.  After initiating the backup upload, you will receive an rq_id parameter. Make sure to include this parameter as a query parameter in your subsequent requests to track the status of the task creation. Once the task has been successfully created, the server will return the id of the newly created task.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.create_backup(task_file_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             task_file_request (TaskFileRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Backup file name. [optional]
             location (str): Where to import the backup file from. [optional] if omitted the server will use the default value of "local"
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
+            rq_id (str): rq id. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1892,30 +1910,31 @@
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method permanently attaches images or video to a task. Supports tus uploads, see more https://tus.io/  # noqa: E501
+        """Method permanently attaches data (images, video, etc.) to a task  # noqa: E501
 
+        Allows to upload data to a task. Supports the TUS open file uploading protocol (https://tus.io/).  Supports the following protocols:  1. A single Data request  and  2.1. An Upload-Start request 2.2.a. Regular TUS protocol requests (Upload-Length + Chunks) 2.2.b. Upload-Multiple requests 2.3. An Upload-Finish request  Requests: - Data - POST, no extra headers or 'Upload-Start' + 'Upload-Finish' headers.   Contains data in the body. - Upload-Start - POST, has an 'Upload-Start' header. No body is expected. - Upload-Length - POST, has an 'Upload-Length' header (see the TUS specification) - Chunk - HEAD/PATCH (see the TUS specification). Sent to /data/<file id> endpoints. - Upload-Finish - POST, has an 'Upload-Finish' header. Can contain data in the body. - Upload-Multiple - POST, has an 'Upload-Multiple' header. Contains data in the body.  The 'Upload-Finish' request allows to specify the uploaded files should be ordered. This may be needed if the files can be sent unordered. To state that the input files are sent ordered, pass an empty list of files in the 'upload_file_order' field. If the files are sent unordered, the ordered file list is expected in the 'upload_file_order' field. It must be a list of string file paths, relative to the dataset root.  Example: files = [     \"cats/cat_1.jpg\",     \"dogs/dog2.jpg\",     \"image_3.png\",     ... ]  Independently of the file declaration field used ('client_files', 'server_files', etc.), when the 'predefined' sorting method is selected, the uploaded files will be ordered according to the '.jsonl' manifest file, if it is found in the list of files. For archives (e.g. '.zip'), a manifest file ('*.jsonl') is required when using the 'predefined' file ordering. Such file must be provided next to the archive in the list of files. Read more about manifest files here: https://opencv.github.io/cvat/docs/manual/advanced/dataset_manifest/  After all data is sent, the operation status can be retrieved via the /status endpoint.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.create_data(id, data_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
             data_request (DataRequest):
 
         Keyword Args:
             upload_finish (bool): Finishes data upload. Can be combined with Upload-Start header to create task data with one request. [optional]
             upload_multiple (bool): Indicates that data with this request are single or multiple files that should be attached to a task. [optional]
-            upload_start (bool): Initializes data upload. No data should be sent with this header. [optional]
+            upload_start (bool): Initializes data upload. Optionally, can include upload metadata in the request body.. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -3109,27 +3128,29 @@
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Method allows to upload task annotations  # noqa: E501
+        """Method allows to upload task annotations or edit existing annotations  # noqa: E501
 
+         To check the status of the process of uploading a task annotations from a file:  After initiating the annotations upload, you will receive an rq_id parameter. Make sure to include this parameter as a query parameter in your subsequent PUT /api/tasks/id/annotations requests to track the status of the annotations upload.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.update_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
 
         Keyword Args:
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
+            rq_id (str): rq id. [optional]
             task_annotations_update_request (TaskAnnotationsUpdateRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/users_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api/webhooks_api.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api/webhooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -814,15 +814,15 @@
         >>> thread = api.create(webhook_write_request, _async_call=True)
         >>> result = thread.get()
 
         Args:
             webhook_write_request (WebhookWriteRequest):
 
         Keyword Args:
-            x_organization (str): [optional]
+            x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/api_client.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
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
-        self.user_agent = 'cvat_sdk/2.4.5'
+        self.user_agent = 'cvat_sdk/2.4.6'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/apis/__init__.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/apis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/configuration.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
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
-               "Version of the API: 2.4.5\n"\
-               "SDK Package Version: 2.4.5".\
+               "Version of the API: 2.4.6\n"\
+               "SDK Package Version: 2.4.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/exceptions.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/about.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotation_file_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotation_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/annotations_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotations_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/attribute_val_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/backup_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/backup_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/basic_user_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/chunk_type.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/chunk_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/client_events_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_content.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/cloud_storage_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_read_owner.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comment_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/comments_summary.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comments_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/credentials_type_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/credentials_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_meta_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_meta_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/data_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -119,34 +119,34 @@
     server_files: typing.List[str] # noqa: E501
     """
     [optional, default: []]
     [str]
     Paths to files from a file share mounted on the server, or from a cloud storage.
     """
 
-    server_files_exclude: typing.List[str] # noqa: E501
-    """
-    [optional, default: []]
-    [str]
-    Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] .
-    """
-
     remote_files: typing.List[str] # noqa: E501
     """
     [optional, default: []]
     [str]
     Direct download URLs for files.
     """
 
     use_zip_chunks: bool # noqa: E501
     """
     [optional, default: False]
     When true, video chunks will be represented as zip archives with decoded video frames. When false, video chunks are represented as video segments .
     """
 
+    server_files_exclude: typing.List[str] # noqa: E501
+    """
+    [optional, default: []]
+    [str]
+    Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] .
+    """
+
     cloud_storage_id: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     If not null, the files referenced by server_files will be retrieved from the cloud storage with the specified ID. The cloud storages applicable depend on the context. In the user sandbox, only the user sandbox cloud storages can be used. In an organization, only the organization cloud storages can be used. .
     """
 
     use_cache: bool # noqa: E501
@@ -185,14 +185,21 @@
     job_file_mapping: typing.List[typing.List[str]] # noqa: E501
     """
     [optional]
     [[str]]
      Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options. Files in the jobs must not overlap or repeat.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ] .
     """
 
+    upload_file_order: typing.List[str] # noqa: E501
+    """
+    [optional]
+    [str]
+    Allows to specify file order for client_file uploads. Only valid with the \"predefined\" sorting method selected.  To state that the input files are sent in the correct order, pass an empty list.  If you want to send files in an arbitrary order and reorder them afterwards on the server, pass the list of file names in the required order. .
+    """
+
 
 class DataRequest(ModelNormal, IDataRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -214,20 +221,20 @@
 
       original_chunk_type (ChunkType): [optional]  # noqa: E501
 
       client_files ([file_type]): Uploaded files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
       server_files ([str]): Paths to files from a file share mounted on the server, or from a cloud storage. [optional] if omitted the server will use the default value of []  # noqa: E501
 
-      server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
-
       remote_files ([str]): Direct download URLs for files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
       use_zip_chunks (bool): When true, video chunks will be represented as zip archives with decoded video frames. When false, video chunks are represented as video segments . [optional] if omitted the server will use the default value of False  # noqa: E501
 
+      server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
+
       cloud_storage_id (int, none_type): If not null, the files referenced by server_files will be retrieved from the cloud storage with the specified ID. The cloud storages applicable depend on the context. In the user sandbox, only the user sandbox cloud storages can be used. In an organization, only the organization cloud storages can be used. . [optional]  # noqa: E501
 
       use_cache (bool): Enable or disable task data chunk caching for the task. Read more: https://opencv.github.io/cvat/docs/manual/advanced/data_on_fly/ . [optional] if omitted the server will use the default value of False  # noqa: E501
 
       copy_data (bool): Copy data from the server file share to CVAT during the task creation. This will create a copy of the data, making the server independent from the file share availability . [optional] if omitted the server will use the default value of False  # noqa: E501
 
       storage_method (StorageMethod): [optional]  # noqa: E501
@@ -236,14 +243,16 @@
 
       sorting_method (SortingMethod): [optional]  # noqa: E501
 
       filename_pattern (str, none_type): A filename filter for cloud storage files listed in the manifest. Supports fnmatch wildcards. Read more: https://docs.python.org/3/library/fnmatch.html . [optional]  # noqa: E501
 
       job_file_mapping ([[str]]):  Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options. Files in the jobs must not overlap or repeat.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ] . [optional]  # noqa: E501
 
+      upload_file_order ([str]): Allows to specify file order for client_file uploads. Only valid with the \"predefined\" sorting method selected.  To state that the input files are sent in the correct order, pass an empty list.  If you want to send files in an arbitrary order and reorder them afterwards on the server, pass the list of file names in the required order. . [optional]  # noqa: E501
+
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
@@ -320,25 +329,26 @@
             'start_frame': (int,),  # noqa: E501
             'stop_frame': (int,),  # noqa: E501
             'frame_filter': (str,),  # noqa: E501
             'compressed_chunk_type': (ChunkType,),  # noqa: E501
             'original_chunk_type': (ChunkType,),  # noqa: E501
             'client_files': ([file_type],),  # noqa: E501
             'server_files': ([str],),  # noqa: E501
-            'server_files_exclude': ([str],),  # noqa: E501
             'remote_files': ([str],),  # noqa: E501
             'use_zip_chunks': (bool,),  # noqa: E501
+            'server_files_exclude': ([str],),  # noqa: E501
             'cloud_storage_id': (int, none_type,),  # noqa: E501
             'use_cache': (bool,),  # noqa: E501
             'copy_data': (bool,),  # noqa: E501
             'storage_method': (StorageMethod,),  # noqa: E501
             'storage': (StorageType,),  # noqa: E501
             'sorting_method': (SortingMethod,),  # noqa: E501
             'filename_pattern': (str, none_type,),  # noqa: E501
             'job_file_mapping': ([[str]],),  # noqa: E501
+            'upload_file_order': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -350,25 +360,26 @@
         'start_frame': 'start_frame',  # noqa: E501
         'stop_frame': 'stop_frame',  # noqa: E501
         'frame_filter': 'frame_filter',  # noqa: E501
         'compressed_chunk_type': 'compressed_chunk_type',  # noqa: E501
         'original_chunk_type': 'original_chunk_type',  # noqa: E501
         'client_files': 'client_files',  # noqa: E501
         'server_files': 'server_files',  # noqa: E501
-        'server_files_exclude': 'server_files_exclude',  # noqa: E501
         'remote_files': 'remote_files',  # noqa: E501
         'use_zip_chunks': 'use_zip_chunks',  # noqa: E501
+        'server_files_exclude': 'server_files_exclude',  # noqa: E501
         'cloud_storage_id': 'cloud_storage_id',  # noqa: E501
         'use_cache': 'use_cache',  # noqa: E501
         'copy_data': 'copy_data',  # noqa: E501
         'storage_method': 'storage_method',  # noqa: E501
         'storage': 'storage',  # noqa: E501
         'sorting_method': 'sorting_method',  # noqa: E501
         'filename_pattern': 'filename_pattern',  # noqa: E501
         'job_file_mapping': 'job_file_mapping',  # noqa: E501
+        'upload_file_order': 'upload_file_order',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -395,20 +406,20 @@
 
             original_chunk_type (ChunkType): [optional]  # noqa: E501
 
             client_files ([file_type]): Uploaded files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             server_files ([str]): Paths to files from a file share mounted on the server, or from a cloud storage. [optional] if omitted the server will use the default value of []  # noqa: E501
 
-            server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
-
             remote_files ([str]): Direct download URLs for files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             use_zip_chunks (bool): When true, video chunks will be represented as zip archives with decoded video frames. When false, video chunks are represented as video segments . [optional] if omitted the server will use the default value of False  # noqa: E501
 
+            server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
+
             cloud_storage_id (int, none_type): If not null, the files referenced by server_files will be retrieved from the cloud storage with the specified ID. The cloud storages applicable depend on the context. In the user sandbox, only the user sandbox cloud storages can be used. In an organization, only the organization cloud storages can be used. . [optional]  # noqa: E501
 
             use_cache (bool): Enable or disable task data chunk caching for the task. Read more: https://opencv.github.io/cvat/docs/manual/advanced/data_on_fly/ . [optional] if omitted the server will use the default value of False  # noqa: E501
 
             copy_data (bool): Copy data from the server file share to CVAT during the task creation. This will create a copy of the data, making the server independent from the file share availability . [optional] if omitted the server will use the default value of False  # noqa: E501
 
             storage_method (StorageMethod): [optional]  # noqa: E501
@@ -417,14 +428,16 @@
 
             sorting_method (SortingMethod): [optional]  # noqa: E501
 
             filename_pattern (str, none_type): A filename filter for cloud storage files listed in the manifest. Supports fnmatch wildcards. Read more: https://docs.python.org/3/library/fnmatch.html . [optional]  # noqa: E501
 
             job_file_mapping ([[str]]):  Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options. Files in the jobs must not overlap or repeat.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ] . [optional]  # noqa: E501
 
+            upload_file_order ([str]): Allows to specify file order for client_file uploads. Only valid with the \"predefined\" sorting method selected.  To state that the input files are sent in the correct order, pass an empty list.  If you want to send files in an arbitrary order and reorder them afterwards on the server, pass the list of file names in the required order. . [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -525,20 +538,20 @@
 
             original_chunk_type (ChunkType): [optional]  # noqa: E501
 
             client_files ([file_type]): Uploaded files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             server_files ([str]): Paths to files from a file share mounted on the server, or from a cloud storage. [optional] if omitted the server will use the default value of []  # noqa: E501
 
-            server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
-
             remote_files ([str]): Direct download URLs for files. [optional] if omitted the server will use the default value of []  # noqa: E501
 
             use_zip_chunks (bool): When true, video chunks will be represented as zip archives with decoded video frames. When false, video chunks are represented as video segments . [optional] if omitted the server will use the default value of False  # noqa: E501
 
+            server_files_exclude ([str]): Paths to files and directories from a file share mounted on the server, or from a cloud storage that should be excluded from the directories specified in server_files. This option cannot be used together with filename_pattern. The server_files_exclude parameter cannot be used to exclude a part of dataset from an archive.  Examples:  Exclude all files from subfolder 'sub/sub_1/sub_2'and single file 'sub/image.jpg' from specified folder: server_files = ['sub/'], server_files_exclude = ['sub/sub_1/sub_2/', 'sub/image.jpg']  Exclude all cloud storage files with prefix 'sub' from the content of manifest file: server_files = ['manifest.jsonl'], server_files_exclude = ['sub/'] . [optional] if omitted the server will use the default value of []  # noqa: E501
+
             cloud_storage_id (int, none_type): If not null, the files referenced by server_files will be retrieved from the cloud storage with the specified ID. The cloud storages applicable depend on the context. In the user sandbox, only the user sandbox cloud storages can be used. In an organization, only the organization cloud storages can be used. . [optional]  # noqa: E501
 
             use_cache (bool): Enable or disable task data chunk caching for the task. Read more: https://opencv.github.io/cvat/docs/manual/advanced/data_on_fly/ . [optional] if omitted the server will use the default value of False  # noqa: E501
 
             copy_data (bool): Copy data from the server file share to CVAT during the task creation. This will create a copy of the data, making the server independent from the file share availability . [optional] if omitted the server will use the default value of False  # noqa: E501
 
             storage_method (StorageMethod): [optional]  # noqa: E501
@@ -547,14 +560,16 @@
 
             sorting_method (SortingMethod): [optional]  # noqa: E501
 
             filename_pattern (str, none_type): A filename filter for cloud storage files listed in the manifest. Supports fnmatch wildcards. Read more: https://docs.python.org/3/library/fnmatch.html . [optional]  # noqa: E501
 
             job_file_mapping ([[str]]):  Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options. Files in the jobs must not overlap or repeat.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ] . [optional]  # noqa: E501
 
+            upload_file_order ([str]): Allows to specify file order for client_file uploads. Only valid with the \"predefined\" sorting method selected.  To state that the input files are sent in the correct order, pass an empty list.  If you want to send files in an arbitrary order and reorder them afterwards on the server, pass the list of file names in the required order. . [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_file_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_format.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_formats.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/dataset_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/event.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/event_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/events.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/events_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/events_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/file_info_type_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info_type_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/frame_meta.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/frame_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/input_type_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/input_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/invitation_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/issue_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/issues_summary.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/issues_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_annotations_update_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_annotations_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_read_assignee.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read_assignee.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_stage.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/job_status.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/jobs_summary.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/jobs_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/label.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_data_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_image_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_shape_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labeled_track_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/labels_summary.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labels_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/location_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/location_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/login_serializer_ex_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/login_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/membership_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/membership_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/meta_user.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/meta_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/online_function_call_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/online_function_call_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/operation_status.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/organization_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_comment_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_comment_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_invitation_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_invitation_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_issue_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_issue_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_job_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_job_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_label_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_label_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_membership_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_membership_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_meta_user_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_meta_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_organization_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_organization_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_project_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_project_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_task_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_task_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/paginated_webhook_read_list.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_change_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_change_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_confirm_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_comment_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_comment_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_data_meta_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_data_meta_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_invitation_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_issue_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_job_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_label_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_label_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_labeled_data_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_membership_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_membership_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_organization_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_user_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/patched_webhook_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/plugins.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_file_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_owner.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_read_target_storage.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/project_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/provider_type_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/provider_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/register_serializer_ex_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/rest_auth_detail.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/role_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/role_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/rq_status_state_enum.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status_state_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/shape_type.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/shape_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/signing_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/signing_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sorting_method.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sorting_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_method.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/storage_type.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_shape_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sub_labeled_track_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/sublabel_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_update_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_annotations_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_file_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_read_target_storage.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/task_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/tasks_summary.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/tasks_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/token.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/tracked_shape_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/user.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_content_type.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_content_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_delivery_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_delivery_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_read.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_type.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model/webhook_write_request.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/model_utils.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/models/__init__.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
@@ -123,14 +123,15 @@
 from cvat_sdk.api_client.model.project_read_target_storage import ProjectReadTargetStorage
 from cvat_sdk.api_client.model.project_write_request import ProjectWriteRequest, IProjectWriteRequest
 from cvat_sdk.api_client.model.provider_type_enum import ProviderTypeEnum, IProviderTypeEnum
 from cvat_sdk.api_client.model.register_serializer_ex import RegisterSerializerEx, IRegisterSerializerEx
 from cvat_sdk.api_client.model.register_serializer_ex_request import RegisterSerializerExRequest, IRegisterSerializerExRequest
 from cvat_sdk.api_client.model.rest_auth_detail import RestAuthDetail, IRestAuthDetail
 from cvat_sdk.api_client.model.role_enum import RoleEnum, IRoleEnum
+from cvat_sdk.api_client.model.rq_id import RqId, IRqId
 from cvat_sdk.api_client.model.rq_status import RqStatus, IRqStatus
 from cvat_sdk.api_client.model.rq_status_state_enum import RqStatusStateEnum, IRqStatusStateEnum
 from cvat_sdk.api_client.model.shape_type import ShapeType, IShapeType
 from cvat_sdk.api_client.model.signing_request import SigningRequest, ISigningRequest
 from cvat_sdk.api_client.model.sorting_method import SortingMethod, ISortingMethod
 from cvat_sdk.api_client.model.storage import Storage, IStorage
 from cvat_sdk.api_client.model.storage_method import StorageMethod, IStorageMethod
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/api_client/rest.py` & `cvat_sdk-2.4.6/cvat_sdk/api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import io
 import json
 import logging
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/client.py` & `cvat_sdk-2.4.6/cvat_sdk/core/client.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/downloading.py` & `cvat_sdk-2.4.6/cvat_sdk/core/downloading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/git.py` & `cvat_sdk-2.4.6/cvat_sdk/core/git.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/helpers.py` & `cvat_sdk-2.4.6/cvat_sdk/core/helpers.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/progress.py` & `cvat_sdk-2.4.6/cvat_sdk/core/progress.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/annotations.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/annotations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/issues.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/issues.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/jobs.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/jobs.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/model_proxy.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/model_proxy.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/organizations.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/organizations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/projects.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/projects.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/tasks.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,10 +446,10 @@
             success_status=201,
             positive_statuses=[202],
             post_params={"rq_id": rq_id},
             status_check_period=status_check_period,
         )
 
         task_id = json.loads(response.data)["id"]
-        self._client.logger.info(f"Task has been imported sucessfully. Task ID: {task_id}")
+        self._client.logger.info(f"Task has been imported successfully. Task ID: {task_id}")
 
         return self.retrieve(task_id)
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/proxies/users.py` & `cvat_sdk-2.4.6/cvat_sdk/core/proxies/users.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/uploading.py` & `cvat_sdk-2.4.6/cvat_sdk/core/uploading.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Copyright (C) 2022 CVAT.ai Corporation
+# Copyright (C) 2022-2023 CVAT.ai Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
+import json
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple
 
 import requests
 import urllib3
 
@@ -85,14 +86,15 @@
 
         Makes request to tus server to create a new upload url for the required file upload.
         """
         headers = self.headers
         headers["upload-length"] = str(self.file_size)
         headers["upload-metadata"] = ",".join(self.encode_metadata())
         resp = self._api_client.rest_client.POST(self.client.url, headers=headers)
+        self.real_filename = resp.headers.get("Upload-Filename")
         url = resp.headers.get("location")
         if url is None:
             msg = "Attempt to retrieve create file url with status {}".format(resp.status_code)
             raise tus_uploader.TusCommunicationError(msg, resp.status_code, resp.content)
         return tus_uploader.urljoin(self.client.url, url)
 
     @tus_uploader._catch_requests_error
@@ -175,17 +177,18 @@
             response of the last request (the "Upload-Finished" one)
         """
         # "CVAT-TUS" protocol has 2 extra messages
         # query params are used only in the extra messages
         assert meta["filename"]
 
         self._tus_start_upload(url, query_params=query_params)
-        self._upload_file_data_with_tus(
+        real_filename = self._upload_file_data_with_tus(
             url=url, filename=filename, meta=meta, pbar=pbar, logger=logger
         )
+        query_params["filename"] = real_filename
         return self._tus_finish_upload(url, query_params=query_params, fields=fields)
 
     def _wait_for_completion(
         self,
         url: str,
         *,
         success_status: int,
@@ -212,15 +215,17 @@
         headers["Origin"] = api_client.configuration.host
         headers.update(api_client.get_common_headers())
 
         client = _TusClient(url, headers=headers)
 
         return _MyTusUploader(client=client, api_client=api_client, **kwargs)
 
-    def _upload_file_data_with_tus(self, url, filename, *, meta=None, pbar=None, logger=None):
+    def _upload_file_data_with_tus(
+        self, url, filename, *, meta=None, pbar=None, logger=None
+    ) -> str:
         file_size = filename.stat().st_size
         if pbar is None:
             pbar = NullProgressReporter()
 
         with open(filename, "rb") as input_file, StreamWithProgress(
             input_file, pbar, length=file_size
         ) as input_file_with_progress:
@@ -229,14 +234,15 @@
                 url=url.rstrip("/") + "/",
                 metadata=meta,
                 file_stream=input_file_with_progress,
                 chunk_size=Uploader._CHUNK_SIZE,
                 log_func=logger,
             )
             tus_uploader.upload()
+            return tus_uploader.real_filename
 
     def _tus_start_upload(self, url, *, query_params=None):
         response = self._client.api_client.rest_client.POST(
             url,
             query_params=query_params,
             headers={
                 "Upload-Start": "",
@@ -269,25 +275,29 @@
         *,
         url_params: Optional[Dict[str, Any]] = None,
         pbar: Optional[ProgressReporter] = None,
         status_check_period: Optional[int] = None,
     ):
         url = self._client.api_map.make_endpoint_url(endpoint.path, kwsub=url_params)
         params = {"format": format_name, "filename": filename.name}
-        self.upload_file(
+        response = self.upload_file(
             url, filename, pbar=pbar, query_params=params, meta={"filename": params["filename"]}
         )
 
+        rq_id = json.loads(response.data).get("rq_id")
+        assert rq_id, "The rq_id was not found in the response"
+        params["rq_id"] = rq_id
+
         self._wait_for_completion(
             url,
             success_status=201,
             positive_statuses=[202],
             status_check_period=status_check_period,
             query_params=params,
-            method="POST",
+            method="PUT",
         )
 
 
 class DatasetUploader(Uploader):
     def upload_file_and_wait(
         self,
         upload_endpoint: Endpoint,
@@ -297,20 +307,25 @@
         *,
         url_params: Optional[Dict[str, Any]] = None,
         pbar: Optional[ProgressReporter] = None,
         status_check_period: Optional[int] = None,
     ):
         url = self._client.api_map.make_endpoint_url(upload_endpoint.path, kwsub=url_params)
         params = {"format": format_name, "filename": filename.name}
-        self.upload_file(
+        response = self.upload_file(
             url, filename, pbar=pbar, query_params=params, meta={"filename": params["filename"]}
         )
+        rq_id = json.loads(response.data).get("rq_id")
+        assert rq_id, "The rq_id was not found in the response"
 
         url = self._client.api_map.make_endpoint_url(retrieve_endpoint.path, kwsub=url_params)
-        params = {"action": "import_status"}
+        params = {
+            "action": "import_status",
+            "rq_id": rq_id,
+        }
         self._wait_for_completion(
             url,
             success_status=201,
             positive_statuses=[202],
             status_check_period=status_check_period,
             query_params=params,
             method="GET",
@@ -331,14 +346,18 @@
         **kwargs,
     ):
         bulk_file_groups, separate_files, total_size = self._split_files_by_requests(resources)
 
         if pbar is not None:
             pbar.start(total_size, desc="Uploading data")
 
+        if str(kwargs.get("sorting_method")).lower() == "predefined":
+            # Request file ordering, because we reorder files to send more efficiently
+            kwargs.setdefault("upload_file_order", [p.name for p in resources])
+
         self._tus_start_upload(url)
 
         for group, group_size in bulk_file_groups:
             files = {}
             for i, filename in enumerate(group):
                 files[f"client_files[{i}]"] = (
                     os.fspath(filename),
@@ -355,15 +374,14 @@
             )
             expect_status(200, response)
 
             if pbar is not None:
                 pbar.advance(group_size)
 
         for filename in separate_files:
-            # TODO: check if basename produces invalid paths here, can lead to overwriting
             self._upload_file_data_with_tus(
                 url,
                 filename,
                 meta={"filename": filename.name},
                 pbar=pbar,
                 logger=self._client.logger.debug,
             )
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk/core/utils.py` & `cvat_sdk-2.4.6/cvat_sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/pytorch/caching.py` & `cvat_sdk-2.4.6/cvat_sdk/pytorch/caching.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/pytorch/common.py` & `cvat_sdk-2.4.6/cvat_sdk/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/pytorch/project_dataset.py` & `cvat_sdk-2.4.6/cvat_sdk/pytorch/project_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/pytorch/task_dataset.py` & `cvat_sdk-2.4.6/cvat_sdk/pytorch/task_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk/pytorch/transforms.py` & `cvat_sdk-2.4.6/cvat_sdk/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.5/cvat_sdk.egg-info/PKG-INFO` & `cvat_sdk-2.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cvat-sdk
-Version: 2.4.5
+Name: cvat_sdk
+Version: 2.4.6
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.5/cvat_sdk.egg-info/SOURCES.txt` & `cvat_sdk-2.4.6/cvat_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 ./cvat_sdk/api_client/model/project_read_target_storage.py
 ./cvat_sdk/api_client/model/project_write_request.py
 ./cvat_sdk/api_client/model/provider_type_enum.py
 ./cvat_sdk/api_client/model/register_serializer_ex.py
 ./cvat_sdk/api_client/model/register_serializer_ex_request.py
 ./cvat_sdk/api_client/model/rest_auth_detail.py
 ./cvat_sdk/api_client/model/role_enum.py
+./cvat_sdk/api_client/model/rq_id.py
 ./cvat_sdk/api_client/model/rq_status.py
 ./cvat_sdk/api_client/model/rq_status_state_enum.py
 ./cvat_sdk/api_client/model/shape_type.py
 ./cvat_sdk/api_client/model/signing_request.py
 ./cvat_sdk/api_client/model/sorting_method.py
 ./cvat_sdk/api_client/model/storage.py
 ./cvat_sdk/api_client/model/storage_method.py
```

### Comparing `cvat_sdk-2.4.5/setup.py` & `cvat_sdk-2.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.5
+# The version of the OpenAPI document: 2.4.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import os.path as osp
 import re
 from setuptools import find_packages, setup
```

