# Comparing `tmp/ucam-identitylib-1.6.0.tar.gz` & `tmp/ucam-identitylib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam-identitylib-1.6.0.tar", last modified: Fri May 12 10:19:27 2023, max compression
+gzip compressed data, was "ucam-identitylib-2.0.0.tar", last modified: Wed Jun 14 14:27:08 2023, max compression
```

## Comparing `ucam-identitylib-1.6.0.tar` & `ucam-identitylib-2.0.0.tar`

### file list

```diff
@@ -1,269 +1,265 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.814756 ucam-identitylib-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2699 2023-05-12 10:19:27.814756 ucam-identitylib-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2002 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.686756 ucam-identitylib-1.6.0/identitylib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2517 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/api_client_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.686756 ucam-identitylib-1.6.0/identitylib/card_client/
--rw-r--r--   0 root         (0) root         (0)     8516 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.690756 ucam-identitylib-1.6.0/identitylib/card_client/api/
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13392 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/permissions_api.py
--rw-r--r--   0 root         (0) root         (0)   217877 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/v1beta1_api.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/versions_api.py
--rw-r--r--   0 root         (0) root         (0)    46930 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.690756 ucam-identitylib-1.6.0/identitylib/card_client/apis/
--rw-r--r--   0 root         (0) root         (0)      643 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24525 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)    12776 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.714756 ucam-identitylib-1.6.0/identitylib/card_client/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19212 2023-05-12 10:18:48.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/api_exception.py
--rw-r--r--   0 root         (0) root         (0)    19855 2023-05-12 10:18:48.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode.py
--rw-r--r--   0 root         (0) root         (0)    19301 2023-05-12 10:18:48.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19607 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19919 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py
--rw-r--r--   0 root         (0) root         (0)    19449 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py
--rw-r--r--   0 root         (0) root         (0)    19216 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    25221 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card.py
--rw-r--r--   0 root         (0) root         (0)    22299 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19875 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_response_type.py
--rw-r--r--   0 root         (0) root         (0)    24195 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier.py
--rw-r--r--   0 root         (0) root         (0)    19670 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19747 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
--rw-r--r--   0 root         (0) root         (0)    19680 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19600 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
--rw-r--r--   0 root         (0) root         (0)    19209 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_destroy_response_type.py
--rw-r--r--   0 root         (0) root         (0)    21322 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_summary.py
--rw-r--r--   0 root         (0) root         (0)    19477 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19206 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    21069 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_logo.py
--rw-r--r--   0 root         (0) root         (0)    20492 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note.py
--rw-r--r--   0 root         (0) root         (0)    19441 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19208 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19191 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_response_type.py
--rw-r--r--   0 root         (0) root         (0)    30424 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request.py
--rw-r--r--   0 root         (0) root         (0)    19640 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    21306 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py
--rw-r--r--   0 root         (0) root         (0)    20037 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py
--rw-r--r--   0 root         (0) root         (0)    19489 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py
--rw-r--r--   0 root         (0) root         (0)    19671 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19284 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19213 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_distinct_values.py
--rw-r--r--   0 root         (0) root         (0)    27953 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_summary.py
--rw-r--r--   0 root         (0) root         (0)    21042 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19197 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19721 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19708 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py
--rw-r--r--   0 root         (0) root         (0)    23503 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_summary.py
--rw-r--r--   0 root         (0) root         (0)    19521 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19176 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19276 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/college_institution_ids_list_response_type.py
--rw-r--r--   0 root         (0) root         (0)    20114 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_available_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)    20165 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_identifier_summary_type.py
--rw-r--r--   0 root         (0) root         (0)    19851 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_logo_type.py
--rw-r--r--   0 root         (0) root         (0)    19851 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_note_type.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_request_summary_type.py
--rw-r--r--   0 root         (0) root         (0)    20064 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_summary_type.py
--rw-r--r--   0 root         (0) root         (0)    19382 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/permissions_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19244 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    19608 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/version_response_type.py
--rw-r--r--   0 root         (0) root         (0)    90312 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.714756 ucam-identitylib-1.6.0/identitylib/card_client/models/
--rw-r--r--   0 root         (0) root         (0)     5572 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21989 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/card_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.718756 ucam-identitylib-1.6.0/identitylib/hr_client/
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.718756 ucam-identitylib-1.6.0/identitylib/hr_client/api/
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15246 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/api/staff_members_api.py
--rw-r--r--   0 root         (0) root         (0)    41199 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.718756 ucam-identitylib-1.6.0/identitylib/hr_client/apis/
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18527 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6932 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.726756 ucam-identitylib-1.6.0/identitylib/hr_client/model/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15386 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation.py
--rw-r--r--   0 root         (0) root         (0)    14942 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13339 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/http_exception.py
--rw-r--r--   0 root         (0) root         (0)    13537 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)    13824 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    14333 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13097 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/location_inner.py
--rw-r--r--   0 root         (0) root         (0)    14276 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/paginated_results_staff_member.py
--rw-r--r--   0 root         (0) root         (0)    16189 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/staff_member.py
--rw-r--r--   0 root         (0) root         (0)    13901 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    84466 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.726756 ucam-identitylib-1.6.0/identitylib/hr_client/models/
--rw-r--r--   0 root         (0) root         (0)     1113 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16143 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     9961 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/identifiers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.734756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.734756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/
--rw-r--r--   0 root         (0) root         (0)      238 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6469 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    40103 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.734756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/apis/
--rw-r--r--   0 root         (0) root         (0)      521 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17693 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5929 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.742756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12946 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_datum.py
--rw-r--r--   0 root         (0) root         (0)    12728 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_response.py
--rw-r--r--   0 root         (0) root         (0)    83476 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.742756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/models/
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15153 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.746756 ucam-identitylib-1.6.0/identitylib/lookup_client/
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.750756 ucam-identitylib-1.6.0/identitylib/lookup_client/api/
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58215 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/group_api.py
--rw-r--r--   0 root         (0) root         (0)    10948 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/ibis_api.py
--rw-r--r--   0 root         (0) root         (0)    76192 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/institution_api.py
--rw-r--r--   0 root         (0) root         (0)   101034 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/person_api.py
--rw-r--r--   0 root         (0) root         (0)    39272 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.750756 ucam-identitylib-1.6.0/identitylib/lookup_client/apis/
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16967 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5116 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.778756 ucam-identitylib-1.6.0/identitylib/lookup_client/model/
--rw-r--r--   0 root         (0) root         (0)      359 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14574 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute.py
--rw-r--r--   0 root         (0) root         (0)    14850 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute_scheme.py
--rw-r--r--   0 root         (0) root         (0)    12076 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_phone_number.py
--rw-r--r--   0 root         (0) root         (0)    14778 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_row.py
--rw-r--r--   0 root         (0) root         (0)    11774 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_web_page.py
--rw-r--r--   0 root         (0) root         (0)    12447 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/error.py
--rw-r--r--   0 root         (0) root         (0)    21254 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response.py
--rw-r--r--   0 root         (0) root         (0)    11698 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11901 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response.py
--rw-r--r--   0 root         (0) root         (0)    11699 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11961 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py
--rw-r--r--   0 root         (0) root         (0)    11735 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11850 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response.py
--rw-r--r--   0 root         (0) root         (0)    11684 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    20692 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_members_of_inst.py
--rw-r--r--   0 root         (0) root         (0)    11880 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response.py
--rw-r--r--   0 root         (0) root         (0)    11532 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11962 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    18567 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py
--rw-r--r--   0 root         (0) root         (0)    11871 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11910 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response.py
--rw-r--r--   0 root         (0) root         (0)    11785 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11950 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response.py
--rw-r--r--   0 root         (0) root         (0)    11762 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11960 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response.py
--rw-r--r--   0 root         (0) root         (0)    11776 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11971 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py
--rw-r--r--   0 root         (0) root         (0)    11856 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11900 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response.py
--rw-r--r--   0 root         (0) root         (0)    11771 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    18657 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person.py
--rw-r--r--   0 root         (0) root         (0)    11870 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response.py
--rw-r--r--   0 root         (0) root         (0)    11702 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    14062 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_identifier.py
--rw-r--r--   0 root         (0) root         (0)    11932 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py
--rw-r--r--   0 root         (0) root         (0)    11550 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    82654 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.778756 ucam-identitylib-1.6.0/identitylib/lookup_client/models/
--rw-r--r--   0 root         (0) root         (0)     4751 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14331 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/lookup_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.778756 ucam-identitylib-1.6.0/identitylib/photo_client/
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.782756 ucam-identitylib-1.6.0/identitylib/photo_client/api/
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11772 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/all_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    10203 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/api_versions_api.py
--rw-r--r--   0 root         (0) root         (0)    43722 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/approved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    10164 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/permissions_api.py
--rw-r--r--   0 root         (0) root         (0)    11335 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifier_api.py
--rw-r--r--   0 root         (0) root         (0)    27918 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifiers_api.py
--rw-r--r--   0 root         (0) root         (0)    11127 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    61774 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/unapproved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    43706 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.782756 ucam-identitylib-1.6.0/identitylib/photo_client/apis/
--rw-r--r--   0 root         (0) root         (0)     1216 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21352 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     9560 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.794757 ucam-identitylib-1.6.0/identitylib/photo_client/model/
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17123 2023-05-12 10:19:04.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/action_enum.py
--rw-r--r--   0 root         (0) root         (0)    16212 2023-05-12 10:19:04.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/api_versions.py
--rw-r--r--   0 root         (0) root         (0)    15964 2023-05-12 10:19:04.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/bad_request.py
--rw-r--r--   0 root         (0) root         (0)    15961 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/forbidden.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/internal_server_error.py
--rw-r--r--   0 root         (0) root         (0)    15958 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/not_found.py
--rw-r--r--   0 root         (0) root         (0)    16791 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py
--rw-r--r--   0 root         (0) root         (0)    16619 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py
--rw-r--r--   0 root         (0) root         (0)    16028 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/permissions.py
--rw-r--r--   0 root         (0) root         (0)    18732 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier.py
--rw-r--r--   0 root         (0) root         (0)    16464 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py
--rw-r--r--   0 root         (0) root         (0)    16412 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py
--rw-r--r--   0 root         (0) root         (0)    19295 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/scheme_enum.py
--rw-r--r--   0 root         (0) root         (0)    16889 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/status_enum.py
--rw-r--r--   0 root         (0) root         (0)    16252 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/transient_image_url.py
--rw-r--r--   0 root         (0) root         (0)    15970 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/unauthorized.py
--rw-r--r--   0 root         (0) root         (0)    22401 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo.py
--rw-r--r--   0 root         (0) root         (0)    16599 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
--rw-r--r--   0 root         (0) root         (0)    16547 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py
--rw-r--r--   0 root         (0) root         (0)    87097 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.794757 ucam-identitylib-1.6.0/identitylib/photo_client/models/
--rw-r--r--   0 root         (0) root         (0)     2004 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18774 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/photo_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.798756 ucam-identitylib-1.6.0/identitylib/student_client/
--rw-r--r--   0 root         (0) root         (0)     2582 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.798756 ucam-identitylib-1.6.0/identitylib/student_client/api/
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21826 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/api/students_api.py
--rw-r--r--   0 root         (0) root         (0)    41093 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.798756 ucam-identitylib-1.6.0/identitylib/student_client/apis/
--rw-r--r--   0 root         (0) root         (0)      509 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18407 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6818 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.806756 ucam-identitylib-1.6.0/identitylib/student_client/model/
--rw-r--r--   0 root         (0) root         (0)      360 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15305 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation.py
--rw-r--r--   0 root         (0) root         (0)    14466 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13235 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/http_exception.py
--rw-r--r--   0 root         (0) root         (0)    13438 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)    13725 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    14035 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/identifier_scheme.py
--rw-r--r--   0 root         (0) root         (0)    12993 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/location_inner.py
--rw-r--r--   0 root         (0) root         (0)    14202 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/paginated_results_student.py
--rw-r--r--   0 root         (0) root         (0)    16439 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/student.py
--rw-r--r--   0 root         (0) root         (0)    13802 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    84357 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.806756 ucam-identitylib-1.6.0/identitylib/student_client/models/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16034 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/university_hr_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/university_student_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 10:19:27.814756 ucam-identitylib-1.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-05-11 16:18:48.000000 ucam-identitylib-1.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.810757 ucam-identitylib-1.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 10:18:27.000000 ucam-identitylib-1.6.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5517 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/tests/test_api_client_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/tests/test_identifiers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.810757 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2699 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12396 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.628632 ucam-identitylib-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-06-14 14:27:08.628632 ucam-identitylib-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.512632 ucam-identitylib-2.0.0/identitylib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/api_client_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.516631 ucam-identitylib-2.0.0/identitylib/card_client/
+-rw-r--r--   0 root         (0) root         (0)     8516 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.516631 ucam-identitylib-2.0.0/identitylib/card_client/api/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13392 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/api/permissions_api.py
+-rw-r--r--   0 root         (0) root         (0)   226616 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/api/v1beta1_api.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/api/versions_api.py
+-rw-r--r--   0 root         (0) root         (0)    46930 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.520632 ucam-identitylib-2.0.0/identitylib/card_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      643 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24525 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)    12776 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.548632 ucam-identitylib-2.0.0/identitylib/card_client/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19212 2023-06-14 14:26:33.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)    19855 2023-06-14 14:26:33.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode.py
+-rw-r--r--   0 root         (0) root         (0)    19301 2023-06-14 14:26:33.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19607 2023-06-14 14:26:33.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19919 2023-06-14 14:26:33.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py
+-rw-r--r--   0 root         (0) root         (0)    19449 2023-06-14 14:26:33.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19216 2023-06-14 14:26:33.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    25572 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card.py
+-rw-r--r--   0 root         (0) root         (0)    19569 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_bulk_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_bulk_update_request_type_updates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19650 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_bulk_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    22299 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_filter_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19875 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_filter_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    24195 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    19670 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19737 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19680 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19600 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19209 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_destroy_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    21322 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_summary.py
+-rw-r--r--   0 root         (0) root         (0)    19463 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19206 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    21069 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_logo.py
+-rw-r--r--   0 root         (0) root         (0)    20492 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_note.py
+-rw-r--r--   0 root         (0) root         (0)    19441 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_note_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19208 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_note_destroy_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19191 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_note_destroy_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    30424 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request.py
+-rw-r--r--   0 root         (0) root         (0)    19640 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    21310 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    20037 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py
+-rw-r--r--   0 root         (0) root         (0)    19489 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19671 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19213 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_distinct_values.py
+-rw-r--r--   0 root         (0) root         (0)    27953 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_summary.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19197 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19721 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19708 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py
+-rw-r--r--   0 root         (0) root         (0)    23854 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_summary.py
+-rw-r--r--   0 root         (0) root         (0)    19521 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19176 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/card_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19276 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/college_institution_ids_list_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    20114 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_available_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)    20165 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_identifier_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    19851 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_logo_type.py
+-rw-r--r--   0 root         (0) root         (0)    19851 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_note_type.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_request_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    20064 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/permissions_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    19608 2023-06-14 14:26:34.000000 ucam-identitylib-2.0.0/identitylib/card_client/model/version_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    90312 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.548632 ucam-identitylib-2.0.0/identitylib/card_client/models/
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21989 2023-06-14 14:26:35.000000 ucam-identitylib-2.0.0/identitylib/card_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/card_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.552632 ucam-identitylib-2.0.0/identitylib/hr_client/
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.552632 ucam-identitylib-2.0.0/identitylib/hr_client/api/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15246 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/api/staff_members_api.py
+-rw-r--r--   0 root         (0) root         (0)    41199 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.552632 ucam-identitylib-2.0.0/identitylib/hr_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      517 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18527 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6932 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.556632 ucam-identitylib-2.0.0/identitylib/hr_client/model/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15386 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/affiliation.py
+-rw-r--r--   0 root         (0) root         (0)    14942 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/affiliation_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13339 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/http_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13537 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    14333 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/identifier_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13097 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/location_inner.py
+-rw-r--r--   0 root         (0) root         (0)    14276 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/paginated_results_staff_member.py
+-rw-r--r--   0 root         (0) root         (0)    16189 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/staff_member.py
+-rw-r--r--   0 root         (0) root         (0)    13901 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    84466 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.556632 ucam-identitylib-2.0.0/identitylib/hr_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16143 2023-06-14 14:26:39.000000 ucam-identitylib-2.0.0/identitylib/hr_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    10094 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/identifiers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.560632 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.564632 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/api/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6469 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    40103 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.564632 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      521 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17693 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.564632 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12946 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model/mapping_datum.py
+-rw-r--r--   0 root         (0) root         (0)    12728 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model/mapping_response.py
+-rw-r--r--   0 root         (0) root         (0)    83476 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.564632 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/models/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15153 2023-06-14 14:26:53.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/inst_identifier_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.568632 ucam-identitylib-2.0.0/identitylib/lookup_client/
+-rw-r--r--   0 root         (0) root         (0)      872 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.572632 ucam-identitylib-2.0.0/identitylib/lookup_client/api/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58215 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/api/group_api.py
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/api/ibis_api.py
+-rw-r--r--   0 root         (0) root         (0)    76192 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/api/institution_api.py
+-rw-r--r--   0 root         (0) root         (0)   101034 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/api/person_api.py
+-rw-r--r--   0 root         (0) root         (0)    39272 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.572632 ucam-identitylib-2.0.0/identitylib/lookup_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16967 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5116 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.592632 ucam-identitylib-2.0.0/identitylib/lookup_client/model/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14574 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/attribute.py
+-rw-r--r--   0 root         (0) root         (0)    14850 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/attribute_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    12076 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/contact_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)    14778 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/contact_row.py
+-rw-r--r--   0 root         (0) root         (0)    11774 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/contact_web_page.py
+-rw-r--r--   0 root         (0) root         (0)    12447 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/error.py
+-rw-r--r--   0 root         (0) root         (0)    21254 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11698 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11901 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups_default_response.py
+-rw-r--r--   0 root         (0) root         (0)    11699 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11961 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11735 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11850 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_group200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11684 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_group200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    20692 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_members_of_inst.py
+-rw-r--r--   0 root         (0) root         (0)    11880 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_search_count200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11532 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_search_count200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11962 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    18567 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11871 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_insts200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11785 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11950 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attribute200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11960 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attributes200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11776 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11971 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11856 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11900 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_inst200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11771 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    18657 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/person.py
+-rw-r--r--   0 root         (0) root         (0)    11870 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_get_person200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11702 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_get_person200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    14062 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-06-14 14:26:43.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    82654 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.592632 ucam-identitylib-2.0.0/identitylib/lookup_client/models/
+-rw-r--r--   0 root         (0) root         (0)     4751 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14331 2023-06-14 14:26:44.000000 ucam-identitylib-2.0.0/identitylib/lookup_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/lookup_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.592632 ucam-identitylib-2.0.0/identitylib/photo_client/
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.596632 ucam-identitylib-2.0.0/identitylib/photo_client/api/
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10203 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/api/api_versions_api.py
+-rw-r--r--   0 root         (0) root         (0)    10164 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/api/permissions_api.py
+-rw-r--r--   0 root         (0) root         (0)   144241 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/api/v1beta1_api.py
+-rw-r--r--   0 root         (0) root         (0)    43706 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.596632 ucam-identitylib-2.0.0/identitylib/photo_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      655 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21352 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     9560 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.600632 ucam-identitylib-2.0.0/identitylib/photo_client/model/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17041 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/action_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16212 2023-06-14 14:26:46.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/api_versions.py
+-rw-r--r--   0 root         (0) root         (0)    15964 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/bad_request.py
+-rw-r--r--   0 root         (0) root         (0)    15961 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/forbidden.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/internal_server_error.py
+-rw-r--r--   0 root         (0) root         (0)    15958 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/not_found.py
+-rw-r--r--   0 root         (0) root         (0)    16791 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py
+-rw-r--r--   0 root         (0) root         (0)    16619 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py
+-rw-r--r--   0 root         (0) root         (0)    16028 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    18732 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/photo_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    16464 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py
+-rw-r--r--   0 root         (0) root         (0)    16412 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    19295 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/scheme_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16889 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16271 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/transient_image_url.py
+-rw-r--r--   0 root         (0) root         (0)    15970 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/unauthorized.py
+-rw-r--r--   0 root         (0) root         (0)    22401 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/v1_beta1_photo.py
+-rw-r--r--   0 root         (0) root         (0)    16599 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
+-rw-r--r--   0 root         (0) root         (0)    87097 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.600632 ucam-identitylib-2.0.0/identitylib/photo_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18774 2023-06-14 14:26:47.000000 ucam-identitylib-2.0.0/identitylib/photo_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/photo_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.604632 ucam-identitylib-2.0.0/identitylib/student_client/
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.608632 ucam-identitylib-2.0.0/identitylib/student_client/api/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21826 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/api/students_api.py
+-rw-r--r--   0 root         (0) root         (0)    41093 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.608632 ucam-identitylib-2.0.0/identitylib/student_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      509 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18407 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.620632 ucam-identitylib-2.0.0/identitylib/student_client/model/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15305 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/affiliation.py
+-rw-r--r--   0 root         (0) root         (0)    14466 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/affiliation_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13235 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/http_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13438 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    13725 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    14035 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/identifier_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    12993 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/location_inner.py
+-rw-r--r--   0 root         (0) root         (0)    14202 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/paginated_results_student.py
+-rw-r--r--   0 root         (0) root         (0)    16439 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/student.py
+-rw-r--r--   0 root         (0) root         (0)    13802 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    84357 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.624632 ucam-identitylib-2.0.0/identitylib/student_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16034 2023-06-14 14:26:50.000000 ucam-identitylib-2.0.0/identitylib/student_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/university_hr_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/identitylib/university_student_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 14:27:08.628632 ucam-identitylib-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-06-14 14:22:26.000000 ucam-identitylib-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.624632 ucam-identitylib-2.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 14:26:12.000000 ucam-identitylib-2.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5517 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/tests/test_api_client_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-06-14 12:42:08.000000 ucam-identitylib-2.0.0/tests/test_identifiers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:27:08.628632 ucam-identitylib-2.0.0/ucam_identitylib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-06-14 14:27:08.000000 ucam-identitylib-2.0.0/ucam_identitylib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12166 2023-06-14 14:27:08.000000 ucam-identitylib-2.0.0/ucam_identitylib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 14:27:08.000000 ucam-identitylib-2.0.0/ucam_identitylib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-14 14:27:08.000000 ucam-identitylib-2.0.0/ucam_identitylib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-14 14:27:08.000000 ucam-identitylib-2.0.0/ucam_identitylib.egg-info/top_level.txt
```

### Comparing `ucam-identitylib-1.6.0/PKG-INFO` & `ucam-identitylib-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-identitylib
-Version: 1.6.0
+Version: 2.0.0
 Summary: A module containing helpers and shared code related to identity systems within UIS, University of Cambridge.
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib
 Author: University of Cambridge Information Services
 Author-email: devops+ucam-identitylib@uis.cam.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ucam-identitylib-1.6.0/README.md` & `ucam-identitylib-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/api_client_mixin.py` & `ucam-identitylib-2.0.0/identitylib/api_client_mixin.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/__init__.py` & `ucam-identitylib-2.0.0/identitylib/card_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/api/permissions_api.py` & `ucam-identitylib-2.0.0/identitylib/card_client/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/api/v1beta1_api.py` & `ucam-identitylib-2.0.0/identitylib/card_client/api/v1beta1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 )
 from identitylib.card_client.model.api_exception import APIException
 from identitylib.card_client.model.available_barcode import AvailableBarcode
 from identitylib.card_client.model.available_barcode_batch_request_type import AvailableBarcodeBatchRequestType
 from identitylib.card_client.model.available_barcode_batch_response_type import AvailableBarcodeBatchResponseType
 from identitylib.card_client.model.available_barcode_create_request_type import AvailableBarcodeCreateRequestType
 from identitylib.card_client.model.card import Card
+from identitylib.card_client.model.card_bulk_update_request_type import CardBulkUpdateRequestType
+from identitylib.card_client.model.card_bulk_update_response_type import CardBulkUpdateResponseType
 from identitylib.card_client.model.card_filter_request_type import CardFilterRequestType
 from identitylib.card_client.model.card_filter_response_type import CardFilterResponseType
 from identitylib.card_client.model.card_identifier import CardIdentifier
 from identitylib.card_client.model.card_identifier_bulk_update_request_type import CardIdentifierBulkUpdateRequestType
 from identitylib.card_client.model.card_identifier_bulk_update_response_type import CardIdentifierBulkUpdateResponseType
 from identitylib.card_client.model.card_identifier_destroy_response_type import CardIdentifierDestroyResponseType
 from identitylib.card_client.model.card_identifier_update_request_type import CardIdentifierUpdateRequestType
@@ -1697,14 +1699,67 @@
                     'image/bmp',
                     'image/svg+xml'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.v1beta1_cards_bulk_update_endpoint = _Endpoint(
+            settings={
+                'response_type': (CardBulkUpdateResponseType,),
+                'auth': [
+                    'API Service OAuth2 Client Credentials',
+                    'API Service OAuth2 Access Code'
+                ],
+                'endpoint_path': '/v1beta1/cards/update',
+                'operation_id': 'v1beta1_cards_bulk_update',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data',
+                ],
+                'required': [
+                    'data',
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
+                    'data':
+                        (CardBulkUpdateRequestType,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.v1beta1_cards_filter_endpoint = _Endpoint(
             settings={
                 'response_type': (CardFilterResponseType,),
                 'auth': [
                     'API Service OAuth2 Client Credentials',
                     'API Service OAuth2 Access Code'
                 ],
@@ -1857,18 +1912,26 @@
             params_map={
                 'all': [
                     'search',
                     'updated_at__lte',
                     'updated_at__gte',
                     'expires_at__lte',
                     'expires_at__gte',
+                    'expires_at__isnull',
+                    'created_at__lte',
+                    'created_at__gte',
+                    'issued_at__lte',
+                    'issued_at__gte',
+                    'issued_at__isnull',
                     'identifier',
                     'status',
                     'card_type',
                     'institution',
+                    'originating_card_request__isnull',
+                    'originating_card_request',
                     'cursor',
                     'page_size',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
@@ -1896,57 +1959,89 @@
                         "TEMPORARY": "MIFARE_TEMPORARY"
                     },
                 },
                 'openapi_types': {
                     'search':
                         (str,),
                     'updated_at__lte':
-                        (str,),
+                        (datetime,),
                     'updated_at__gte':
-                        (str,),
+                        (datetime,),
                     'expires_at__lte':
-                        (str,),
+                        (datetime,),
                     'expires_at__gte':
-                        (str,),
+                        (datetime,),
+                    'expires_at__isnull':
+                        (bool,),
+                    'created_at__lte':
+                        (datetime,),
+                    'created_at__gte':
+                        (datetime,),
+                    'issued_at__lte':
+                        (datetime,),
+                    'issued_at__gte':
+                        (datetime,),
+                    'issued_at__isnull':
+                        (bool,),
                     'identifier':
                         (str,),
                     'status':
                         (str,),
                     'card_type':
                         (str,),
                     'institution':
                         (str,),
+                    'originating_card_request__isnull':
+                        (bool,),
+                    'originating_card_request':
+                        (str,),
                     'cursor':
                         (str,),
                     'page_size':
                         (int,),
                 },
                 'attribute_map': {
                     'search': 'search',
                     'updated_at__lte': 'updated_at__lte',
                     'updated_at__gte': 'updated_at__gte',
                     'expires_at__lte': 'expires_at__lte',
                     'expires_at__gte': 'expires_at__gte',
+                    'expires_at__isnull': 'expires_at__isnull',
+                    'created_at__lte': 'created_at__lte',
+                    'created_at__gte': 'created_at__gte',
+                    'issued_at__lte': 'issued_at__lte',
+                    'issued_at__gte': 'issued_at__gte',
+                    'issued_at__isnull': 'issued_at__isnull',
                     'identifier': 'identifier',
                     'status': 'status',
                     'card_type': 'card_type',
                     'institution': 'institution',
+                    'originating_card_request__isnull': 'originating_card_request__isnull',
+                    'originating_card_request': 'originating_card_request',
                     'cursor': 'cursor',
                     'page_size': 'page_size',
                 },
                 'location_map': {
                     'search': 'query',
                     'updated_at__lte': 'query',
                     'updated_at__gte': 'query',
                     'expires_at__lte': 'query',
                     'expires_at__gte': 'query',
+                    'expires_at__isnull': 'query',
+                    'created_at__lte': 'query',
+                    'created_at__gte': 'query',
+                    'issued_at__lte': 'query',
+                    'issued_at__gte': 'query',
+                    'issued_at__isnull': 'query',
                     'identifier': 'query',
                     'status': 'query',
                     'card_type': 'query',
                     'institution': 'query',
+                    'originating_card_request__isnull': 'query',
+                    'originating_card_request': 'query',
                     'cursor': 'query',
                     'page_size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -2786,15 +2881,15 @@
         self,
         id,
         data,
         **kwargs
     ):
         """Update the card identifier  # noqa: E501
 
-         ## Update the card identifier  This method allows a client to submit an action in the request body for a given card identifier. The allowed actions are `set_retention`, `restore`, `soft_delete` and `hard_delete`.  ### Permissions  Principals with the `CARD_ADMIN` permission will be able to affect this endpoint.     # noqa: E501
+         ## Update the card identifier  This method allows a client to submit an action in the request body for a given card identifier. The allowed actions are `repair`, `restore`, `soft_delete` and `hard_delete`.  ### Permissions  Principals with the `CARD_ADMIN` permission will be able to affect this endpoint.     # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1beta1_card_identifiers_update(id, data, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4434,14 +4529,97 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.v1beta1_cards_back_visualization_endpoint.call_with_http_info(**kwargs)
 
+    def v1beta1_cards_bulk_update(
+        self,
+        data,
+        **kwargs
+    ):
+        """Update multiple cards  # noqa: E501
+
+         ## Update multiple cards  Allows multiple cards to be updated in one call. For large number of cards, this endpoint will be faster than PUT-ing each update.  Updates are processed in the order they are received. The response includes the detail of the operation, the UUID of the card that was updated, and HTTP status code which would have been returned from separate PUTs. If the status code is 404, the `id` property is omitted.  ### Permissions  Principals with the `CARD_UPDATER` permission will be able to affect this endpoint.    # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1beta1_cards_bulk_update(data, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data (CardBulkUpdateRequestType):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
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
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            CardBulkUpdateResponseType
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['data'] = \
+            data
+        return self.v1beta1_cards_bulk_update_endpoint.call_with_http_info(**kwargs)
+
     def v1beta1_cards_filter(
         self,
         data,
         **kwargs
     ):
         """Filter cards by identifiers  # noqa: E501
 
@@ -4621,22 +4799,30 @@
 
         >>> thread = api.v1beta1_cards_list(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             search (str): A search term.. [optional]
-            updated_at__lte (str): [optional]
-            updated_at__gte (str): [optional]
-            expires_at__lte (str): [optional]
-            expires_at__gte (str): [optional]
+            updated_at__lte (datetime): Filter updatedAt by IsoDateTime less than. [optional]
+            updated_at__gte (datetime): Filter updatedAt by IsoDateTime greater than. [optional]
+            expires_at__lte (datetime): Filter expiresAt by IsoDateTime less than. [optional]
+            expires_at__gte (datetime): Filter expiresAt by IsoDateTime greater than. [optional]
+            expires_at__isnull (bool): Filter expiresAt by IsoDateTime is Null. [optional]
+            created_at__lte (datetime): Filter createdAt by IsoDateTime less than. [optional]
+            created_at__gte (datetime): Filter createdAt by IsoDateTime greater than. [optional]
+            issued_at__lte (datetime): Filter issuedAt by IsoDateTime less than. [optional]
+            issued_at__gte (datetime): Filter issuedAt by IsoDateTime greater than. [optional]
+            issued_at__isnull (bool): Filter issuedAt by IsoDateTime is Null. [optional]
             identifier (str): Filter cards by an identifier in the format {value}@{scheme}. [optional]
             status (str): Filter cards by their current status. [optional]
             card_type (str): Filter by the type of card. [optional]
             institution (str): Filter by an institution id in the format {value}@{scheme}. The scheme must be the Lookup institution scheme: `insts.lookup.cam.ac.uk`, if the @{scheme} is omitted this value is assumed.. [optional]
+            originating_card_request__isnull (bool): Filter originating_card_request by CardRequest UUID isNull. [optional]
+            originating_card_request (str): Filter originating_card_request by CardRequest UUID. [optional]
             cursor (str): The pagination cursor value.. [optional]
             page_size (int): Number of results to return per page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/api/versions_api.py` & `ucam-identitylib-2.0.0/identitylib/card_client/api/versions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/api_client.py` & `ucam-identitylib-2.0.0/identitylib/card_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/apis/__init__.py` & `ucam-identitylib-2.0.0/identitylib/card_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/configuration.py` & `ucam-identitylib-2.0.0/identitylib/card_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/exceptions.py` & `ucam-identitylib-2.0.0/identitylib/card_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/api_exception.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/api_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_create_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/available_barcode_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
             'can_update': (bool,),  # noqa: E501
             'identifiers': ([CardIdentifierSummary],),  # noqa: E501
             'notes': ([CardNote],),  # noqa: E501
             'status': (str,),  # noqa: E501
             'attributes': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'back_visualization_link': (str,),  # noqa: E501
             'card_type': (str,),  # noqa: E501
+            'created_at': (datetime, none_type,),  # noqa: E501
             'expires_at': (datetime, none_type,),  # noqa: E501
             'front_visualization_link': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'issue_number': (int, none_type,),  # noqa: E501
             'issued_at': (datetime, none_type,),  # noqa: E501
             'returned_at': (datetime, none_type,),  # noqa: E501
             'revoked_at': (datetime, none_type,),  # noqa: E501
@@ -132,27 +133,29 @@
         'can_update': 'canUpdate',  # noqa: E501
         'identifiers': 'identifiers',  # noqa: E501
         'notes': 'notes',  # noqa: E501
         'status': 'status',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
         'back_visualization_link': 'backVisualizationLink',  # noqa: E501
         'card_type': 'cardType',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
         'expires_at': 'expiresAt',  # noqa: E501
         'front_visualization_link': 'frontVisualizationLink',  # noqa: E501
         'id': 'id',  # noqa: E501
         'issue_number': 'issueNumber',  # noqa: E501
         'issued_at': 'issuedAt',  # noqa: E501
         'returned_at': 'returnedAt',  # noqa: E501
         'revoked_at': 'revokedAt',  # noqa: E501
         'self_link': 'selfLink',  # noqa: E501
         'updated_at': 'updatedAt',  # noqa: E501
     }
 
     read_only_vars = {
         'back_visualization_link',  # noqa: E501
+        'created_at',  # noqa: E501
         'front_visualization_link',  # noqa: E501
         'id',  # noqa: E501
         'self_link',  # noqa: E501
         'updated_at',  # noqa: E501
     }
 
     _composed_schemas = {}
@@ -198,14 +201,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             attributes (bool, date, datetime, dict, float, int, list, str, none_type): The attributes of the card - describing what is present on the physical version of the card. This is an untyped block of JSON and the structure may change between card types, as different card types will allow different data to be printed on them. The attributes of temporary cards will not be populated as data relating to what has been printed on temporary cards has not been recorded.. [optional]  # noqa: E501
             back_visualization_link (str): [optional]  # noqa: E501
             card_type (str): The type of the card. [optional]  # noqa: E501
+            created_at (datetime, none_type): When this record was created. [optional]  # noqa: E501
             expires_at (datetime, none_type): If non-NULL, when the card expires. [optional]  # noqa: E501
             front_visualization_link (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             issue_number (int, none_type): The issue number of the card. [optional]  # noqa: E501
             issued_at (datetime, none_type): If non-NULL, when the card was issued. [optional]  # noqa: E501
             returned_at (datetime, none_type): If non-NULL, when the card was returned. [optional]  # noqa: E501
             revoked_at (datetime, none_type): If non-NULL, when the card was revoked. [optional]  # noqa: E501
@@ -305,14 +309,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             attributes (bool, date, datetime, dict, float, int, list, str, none_type): The attributes of the card - describing what is present on the physical version of the card. This is an untyped block of JSON and the structure may change between card types, as different card types will allow different data to be printed on them. The attributes of temporary cards will not be populated as data relating to what has been printed on temporary cards has not been recorded.. [optional]  # noqa: E501
             back_visualization_link (str): [optional]  # noqa: E501
             card_type (str): The type of the card. [optional]  # noqa: E501
+            created_at (datetime, none_type): When this record was created. [optional]  # noqa: E501
             expires_at (datetime, none_type): If non-NULL, when the card expires. [optional]  # noqa: E501
             front_visualization_link (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             issue_number (int, none_type): The issue number of the card. [optional]  # noqa: E501
             issued_at (datetime, none_type): If non-NULL, when the card was issued. [optional]  # noqa: E501
             returned_at (datetime, none_type): If non-NULL, when the card was returned. [optional]  # noqa: E501
             revoked_at (datetime, none_type): If non-NULL, when the card was revoked. [optional]  # noqa: E501
```

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_filter_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_filter_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('action',): {
-            'SET_RETENTION': "set_retention",
             'RESTORE': "restore",
+            'REPAIR': "repair",
             'SOFT_DELETE': "soft_delete",
             'HARD_DELETE': "hard_delete",
         },
     }
 
     validations = {
     }
@@ -140,15 +140,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             action (str): The action to apply to this card identifier.. [optional]  # noqa: E501
-            id (str): id of the card identifier. [optional]  # noqa: E501
+            id (str): UUID of the card identifier. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -227,15 +227,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             action (str): The action to apply to this card identifier.. [optional]  # noqa: E501
-            id (str): id of the card identifier. [optional]  # noqa: E501
+            id (str): UUID of the card identifier. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_destroy_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_destroy_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_summary.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_summary.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_update_request_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('action',): {
-            'SET_RETENTION': "set_retention",
             'RESTORE': "restore",
+            'REPAIR': "repair",
             'SOFT_DELETE': "soft_delete",
             'HARD_DELETE': "hard_delete",
         },
     }
 
     validations = {
     }
```

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_identifier_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_logo.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_logo.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_note.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_create_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_note_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_note_destroy_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_note_destroy_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             action (str): The action to apply to this card request.. [optional]  # noqa: E501
             fields (CardRequestBulkUpdateRequestTypeUpdatesInnerFields): [optional]  # noqa: E501
-            id (str): id of the card request. [optional]  # noqa: E501
+            id (str): UUID of the card request. [optional]  # noqa: E501
             identifiers ([CardRequestBulkUpdateRequestTypeUpdatesInnerIdentifiersInner]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -249,15 +249,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             action (str): The action to apply to this card request.. [optional]  # noqa: E501
             fields (CardRequestBulkUpdateRequestTypeUpdatesInnerFields): [optional]  # noqa: E501
-            id (str): id of the card request. [optional]  # noqa: E501
+            id (str): UUID of the card request. [optional]  # noqa: E501
             identifiers ([CardRequestBulkUpdateRequestTypeUpdatesInnerIdentifiersInner]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_bulk_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_create_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_distinct_values.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_distinct_values.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_summary.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_summary.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_request_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_summary.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
         """
         lazy_import()
         return {
             'identifiers': ([CardIdentifierSummary],),  # noqa: E501
             'status': (str,),  # noqa: E501
             'back_visualization_link': (str,),  # noqa: E501
             'card_type': (str,),  # noqa: E501
+            'created_at': (datetime, none_type,),  # noqa: E501
             'expires_at': (datetime, none_type,),  # noqa: E501
             'front_visualization_link': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'issue_number': (int, none_type,),  # noqa: E501
             'issued_at': (datetime, none_type,),  # noqa: E501
             'returned_at': (datetime, none_type,),  # noqa: E501
             'revoked_at': (datetime, none_type,),  # noqa: E501
@@ -124,27 +125,29 @@
 
 
     attribute_map = {
         'identifiers': 'identifiers',  # noqa: E501
         'status': 'status',  # noqa: E501
         'back_visualization_link': 'backVisualizationLink',  # noqa: E501
         'card_type': 'cardType',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
         'expires_at': 'expiresAt',  # noqa: E501
         'front_visualization_link': 'frontVisualizationLink',  # noqa: E501
         'id': 'id',  # noqa: E501
         'issue_number': 'issueNumber',  # noqa: E501
         'issued_at': 'issuedAt',  # noqa: E501
         'returned_at': 'returnedAt',  # noqa: E501
         'revoked_at': 'revokedAt',  # noqa: E501
         'self_link': 'selfLink',  # noqa: E501
         'updated_at': 'updatedAt',  # noqa: E501
     }
 
     read_only_vars = {
         'back_visualization_link',  # noqa: E501
+        'created_at',  # noqa: E501
         'front_visualization_link',  # noqa: E501
         'id',  # noqa: E501
         'self_link',  # noqa: E501
         'updated_at',  # noqa: E501
     }
 
     _composed_schemas = {}
@@ -187,14 +190,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             back_visualization_link (str): [optional]  # noqa: E501
             card_type (str): The type of the card. [optional]  # noqa: E501
+            created_at (datetime, none_type): When this record was created. [optional]  # noqa: E501
             expires_at (datetime, none_type): If non-NULL, when the card expires. [optional]  # noqa: E501
             front_visualization_link (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             issue_number (int, none_type): The issue number of the card. [optional]  # noqa: E501
             issued_at (datetime, none_type): If non-NULL, when the card was issued. [optional]  # noqa: E501
             returned_at (datetime, none_type): If non-NULL, when the card was returned. [optional]  # noqa: E501
             revoked_at (datetime, none_type): If non-NULL, when the card was revoked. [optional]  # noqa: E501
@@ -289,14 +293,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             back_visualization_link (str): [optional]  # noqa: E501
             card_type (str): The type of the card. [optional]  # noqa: E501
+            created_at (datetime, none_type): When this record was created. [optional]  # noqa: E501
             expires_at (datetime, none_type): If non-NULL, when the card expires. [optional]  # noqa: E501
             front_visualization_link (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             issue_number (int, none_type): The issue number of the card. [optional]  # noqa: E501
             issued_at (datetime, none_type): If non-NULL, when the card was issued. [optional]  # noqa: E501
             returned_at (datetime, none_type): If non-NULL, when the card was returned. [optional]  # noqa: E501
             revoked_at (datetime, none_type): If non-NULL, when the card was revoked. [optional]  # noqa: E501
```

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_request_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/card_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/college_institution_ids_list_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/college_institution_ids_list_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_available_barcode_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_available_barcode_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_identifier_summary_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_identifier_summary_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_logo_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_logo_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_note_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_note_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_request_summary_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_request_summary_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_summary_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/paginated_card_summary_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/permissions_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/permissions_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/validation_error.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model/version_response_type.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model/version_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/model_utils.py` & `ucam-identitylib-2.0.0/identitylib/card_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/models/__init__.py` & `ucam-identitylib-2.0.0/identitylib/card_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from identitylib.card_client.model.available_barcode import AvailableBarcode
 from identitylib.card_client.model.available_barcode_batch_request_type import AvailableBarcodeBatchRequestType
 from identitylib.card_client.model.available_barcode_batch_response_type import AvailableBarcodeBatchResponseType
 from identitylib.card_client.model.available_barcode_batch_response_type_details import AvailableBarcodeBatchResponseTypeDetails
 from identitylib.card_client.model.available_barcode_batch_response_type_details_invalid_inner import AvailableBarcodeBatchResponseTypeDetailsInvalidInner
 from identitylib.card_client.model.available_barcode_create_request_type import AvailableBarcodeCreateRequestType
 from identitylib.card_client.model.card import Card
+from identitylib.card_client.model.card_bulk_update_request_type import CardBulkUpdateRequestType
+from identitylib.card_client.model.card_bulk_update_request_type_updates_inner import CardBulkUpdateRequestTypeUpdatesInner
+from identitylib.card_client.model.card_bulk_update_response_type import CardBulkUpdateResponseType
 from identitylib.card_client.model.card_filter_request_type import CardFilterRequestType
 from identitylib.card_client.model.card_filter_response_type import CardFilterResponseType
 from identitylib.card_client.model.card_identifier import CardIdentifier
 from identitylib.card_client.model.card_identifier_bulk_update_request_type import CardIdentifierBulkUpdateRequestType
 from identitylib.card_client.model.card_identifier_bulk_update_request_type_updates_inner import CardIdentifierBulkUpdateRequestTypeUpdatesInner
 from identitylib.card_client.model.card_identifier_bulk_update_response_type import CardIdentifierBulkUpdateResponseType
 from identitylib.card_client.model.card_identifier_bulk_update_response_type_details_inner import CardIdentifierBulkUpdateResponseTypeDetailsInner
```

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client/rest.py` & `ucam-identitylib-2.0.0/identitylib/card_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/card_client_configuration.py` & `ucam-identitylib-2.0.0/identitylib/card_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/__init__.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/api/staff_members_api.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/api/staff_members_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/api_client.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/apis/__init__.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/configuration.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/exceptions.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/affiliation.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation_scheme.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/affiliation_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/http_exception.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/http_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/http_validation_error.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier_scheme.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/identifier_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/location_inner.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/location_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/paginated_results_staff_member.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/paginated_results_staff_member.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/staff_member.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/staff_member.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model/validation_error.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/model_utils.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/models/__init__.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/hr_client/rest.py` & `ucam-identitylib-2.0.0/identitylib/hr_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/identifiers.py` & `ucam-identitylib-2.0.0/identitylib/identifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,14 +321,17 @@
         elif len(parts) == 1 and fallback_scheme is not None:
             parsed_value = value
             scheme = fallback_scheme
         else:
             raise ValueError(f"Invalid identifier {value}")
 
         parsed_value = scheme.value_parser(parsed_value) if scheme.value_parser else parsed_value
+
+        if str(scheme).lower() == str(IdentifierSchemes.CRSID).lower():
+            return Identifier(parsed_value.lower(), scheme)
         return Identifier(parsed_value, scheme)
 
     def __str__(self):
         """
         Parse an identifier back to string form.
 
         """
```

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/__init__.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/default_api.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api_client.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/apis/__init__.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/configuration.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/exceptions.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_datum.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model/mapping_datum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_response.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model/mapping_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model_utils.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/models/__init__.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/rest.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/inst_identifier_configuration.py` & `ucam-identitylib-2.0.0/identitylib/inst_identifier_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/__init__.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/api/group_api.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/api/group_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/api/ibis_api.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/api/ibis_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/api/institution_api.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/api/institution_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/api/person_api.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/api/person_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/api_client.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/apis/__init__.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/configuration.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/exceptions.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/attribute.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute_scheme.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/attribute_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_phone_number.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/contact_phone_number.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_row.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/contact_row.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_web_page.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/contact_web_page.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/error.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups_default_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_group200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_get_group200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_members_of_inst.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_members_of_inst.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_search_count200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/group_search_count200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_version200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/identifier.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_insts200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attribute200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attributes200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_inst200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/person.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_get_person200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_get_person200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_identifier.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/model_utils.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/models/__init__.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client/rest.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/lookup_client_configuration.py` & `ucam-identitylib-2.0.0/identitylib/lookup_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/__init__.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/api/all_photos_api.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/api/permissions_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,48 +18,42 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from identitylib.photo_client.model.bad_request import BadRequest
-from identitylib.photo_client.model.forbidden import Forbidden
-from identitylib.photo_client.model.internal_server_error import InternalServerError
-from identitylib.photo_client.model.paginated_v1_beta1_photo_list import PaginatedV1Beta1PhotoList
-from identitylib.photo_client.model.unauthorized import Unauthorized
+from identitylib.photo_client.model.permissions import Permissions
 
 
-class AllPhotosApi(object):
+class PermissionsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.v1beta1_all_photos_list_endpoint = _Endpoint(
+        self.permissions_retrieve_endpoint = _Endpoint(
             settings={
-                'response_type': (PaginatedV1Beta1PhotoList,),
+                'response_type': (Permissions,),
                 'auth': [
                     'apiGatewayAuthorizationCodeSecurityScheme',
                     'apiGatewayClientCredentialsSecurityScheme'
                 ],
-                'endpoint_path': '/v1beta1/all-photos',
-                'operation_id': 'v1beta1_all_photos_list',
+                'endpoint_path': '/permissions',
+                'operation_id': 'permissions_retrieve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'cursor',
-                    'page_size',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -67,56 +61,46 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'cursor':
-                        (str,),
-                    'page_size':
-                        (int,),
                 },
                 'attribute_map': {
-                    'cursor': 'cursor',
-                    'page_size': 'pageSize',
                 },
                 'location_map': {
-                    'cursor': 'query',
-                    'page_size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def v1beta1_all_photos_list(
+    def permissions_retrieve(
         self,
         **kwargs
     ):
-        """List all photos  # noqa: E501
+        """List permissions  # noqa: E501
 
-         # List all Photos  This endpoint allows information and metadata about all Photos to be fetched.  Results are ordered by `createdAt` ascending, and may be split over multiple 'pages'. Where more results exist a `next` URL will be provided which can be used to fetch the next page of results. The `previous` URL can be used to navigate backwards through the result pages. The `pageSize` query parameter can be used to request a specific amount of results per page. If not provided the `pageSize` is set to `200`. The amount of results per page is limited to `500`, if a number greater than `500` is specified in the `pageSize` parameter no error is returned but the number of results will be capped at 500 per page.  Only principals with the `PHOTO_ADMIN` permission can list all photos.    # noqa: E501
+        List the permissions of the current principal  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1beta1_all_photos_list(async_req=True)
+        >>> thread = api.permissions_retrieve(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            cursor (str): The pagination cursor value.. [optional]
-            page_size (int): Number of results to return per page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -141,15 +125,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            PaginatedV1Beta1PhotoList
+            Permissions
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -170,9 +154,9 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.v1beta1_all_photos_list_endpoint.call_with_http_info(**kwargs)
+        return self.permissions_retrieve_endpoint.call_with_http_info(**kwargs)
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/api/api_versions_api.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/api/api_versions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/api/approved_photos_api.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/api_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,866 +5,895 @@
 
     The version of the OpenAPI document: v1beta1
     Contact: devops+photoapi@uis.cam.ac.uk
     Generated by: https://openapi-generator.tech
 """
 
 
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from identitylib.photo_client.api_client import ApiClient, Endpoint as _Endpoint
-from identitylib.photo_client.model_utils import (  # noqa: F401
+import json
+import atexit
+import mimetypes
+from multiprocessing.pool import ThreadPool
+import io
+import os
+import re
+import typing
+from urllib.parse import quote
+from urllib3.fields import RequestField
+
+
+from identitylib.photo_client import rest
+from identitylib.photo_client.configuration import Configuration
+from identitylib.photo_client.exceptions import ApiTypeError, ApiValueError, ApiException
+from identitylib.photo_client.model_utils import (
+    ModelNormal,
+    ModelSimple,
+    ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
+    deserialize_file,
     file_type,
+    model_to_dict,
     none_type,
     validate_and_convert_types
 )
-from identitylib.photo_client.model.bad_request import BadRequest
-from identitylib.photo_client.model.forbidden import Forbidden
-from identitylib.photo_client.model.internal_server_error import InternalServerError
-from identitylib.photo_client.model.not_found import NotFound
-from identitylib.photo_client.model.paginated_v1_beta1_photo_list import PaginatedV1Beta1PhotoList
-from identitylib.photo_client.model.transient_image_url import TransientImageUrl
-from identitylib.photo_client.model.unauthorized import Unauthorized
-from identitylib.photo_client.model.v1_beta1_photo import V1Beta1Photo
-
-
-class ApprovedPhotosApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
-    """
 
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.v1beta1_approved_photos_content_retrieve_endpoint = _Endpoint(
-            settings={
-                'response_type': None,
-                'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
-                ],
-                'endpoint_path': '/v1beta1/approved-photos/{identifier}/content',
-                'operation_id': 'v1beta1_approved_photos_content_retrieve',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'identifier',
-                ],
-                'required': [
-                    'identifier',
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
-                    'identifier':
-                        (str,),
-                },
-                'attribute_map': {
-                    'identifier': 'identifier',
-                },
-                'location_map': {
-                    'identifier': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'image/*',
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.v1beta1_approved_photos_content_transient_url_retrieve_endpoint = _Endpoint(
-            settings={
-                'response_type': (TransientImageUrl,),
-                'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
-                ],
-                'endpoint_path': '/v1beta1/approved-photos/{identifier}/content/transient-url',
-                'operation_id': 'v1beta1_approved_photos_content_transient_url_retrieve',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'identifier',
-                ],
-                'required': [
-                    'identifier',
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
-                    'identifier':
-                        (str,),
-                },
-                'attribute_map': {
-                    'identifier': 'identifier',
-                },
-                'location_map': {
-                    'identifier': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.v1beta1_approved_photos_list_endpoint = _Endpoint(
-            settings={
-                'response_type': (PaginatedV1Beta1PhotoList,),
-                'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
-                ],
-                'endpoint_path': '/v1beta1/approved-photos',
-                'operation_id': 'v1beta1_approved_photos_list',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'approved_since',
-                    'cursor',
-                    'page_size',
-                ],
-                'required': [
-                    'approved_since',
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
-                    'approved_since':
-                        (str,),
-                    'cursor':
-                        (str,),
-                    'page_size':
-                        (int,),
-                },
-                'attribute_map': {
-                    'approved_since': 'approvedSince',
-                    'cursor': 'cursor',
-                    'page_size': 'pageSize',
-                },
-                'location_map': {
-                    'approved_since': 'query',
-                    'cursor': 'query',
-                    'page_size': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.v1beta1_approved_photos_retrieve_endpoint = _Endpoint(
-            settings={
-                'response_type': (V1Beta1Photo,),
-                'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
-                ],
-                'endpoint_path': '/v1beta1/approved-photos/{identifier}',
-                'operation_id': 'v1beta1_approved_photos_retrieve',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'identifier',
-                ],
-                'required': [
-                    'identifier',
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
-                    'identifier':
-                        (str,),
-                },
-                'attribute_map': {
-                    'identifier': 'identifier',
-                },
-                'location_map': {
-                    'identifier': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.v1beta1_approved_photos_thumbnail_retrieve_endpoint = _Endpoint(
-            settings={
-                'response_type': None,
-                'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
-                ],
-                'endpoint_path': '/v1beta1/approved-photos/{identifier}/thumbnail',
-                'operation_id': 'v1beta1_approved_photos_thumbnail_retrieve',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'identifier',
-                ],
-                'required': [
-                    'identifier',
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
-                    'identifier':
-                        (str,),
-                },
-                'attribute_map': {
-                    'identifier': 'identifier',
-                },
-                'location_map': {
-                    'identifier': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'image/*',
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.v1beta1_approved_photos_thumbnail_transient_url_retrieve_endpoint = _Endpoint(
-            settings={
-                'response_type': (TransientImageUrl,),
-                'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
-                ],
-                'endpoint_path': '/v1beta1/approved-photos/{identifier}/thumbnail/transient-url',
-                'operation_id': 'v1beta1_approved_photos_thumbnail_transient_url_retrieve',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'identifier',
-                ],
-                'required': [
-                    'identifier',
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
-                    'identifier':
-                        (str,),
-                },
-                'attribute_map': {
-                    'identifier': 'identifier',
-                },
-                'location_map': {
-                    'identifier': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
+class ApiClient(object):
+    """Generic API client for OpenAPI client library builds.
 
-    def v1beta1_approved_photos_content_retrieve(
-        self,
-        identifier,
-        **kwargs
-    ):
-        """Get the image content of an approved photo using a person identifier  # noqa: E501
+    OpenAPI generic API client. This client handles the client-
+    server communication, and is invariant across implementations. Specifics of
+    the methods and models for each application are generated from the OpenAPI
+    templates.
 
-         # Get image content of an approved Photo  This endpoint redirects to the image content of the single, most recently approved, Photo for the given PhotoIdentifier.  The PhotoIdentifier should be included in the URL params in the format `<value>@<scheme>` - see the introduction to this API for a list of supported schemes. If the scheme is not provided it is assumed to be a CRSid (v1.person.identifiers.cam.ac.uk).  A given PhotoIdentifier may link to many approved Photos, in which case the most recently approved Photo is returned here. If a PhotoIdentifier does not link to an approved Photo a `404` response will be returned.  The Photo returned may change over time if a new Photo is approved for a given PhotoIdentifier. If you want to keep a reference to an exact Photo you can use the Photo's `id` (the UUID), or `contentLink` of the Photo returned from the `Get approved Photo` endpoint above, which is guaranteed to always give back the same Photo, regardless of whether a new Photo is approved for a given PhotoIdentifier.  This endpoint redirects to a temporary URL provided by the storage service used by this API. This temporary URL will expire after a short period of time and therefore should not be recorded or used as a permanent reference to this Photo.    # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
+    NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+    Do not edit the class manually.
 
-        >>> thread = api.v1beta1_approved_photos_content_retrieve(identifier, async_req=True)
-        >>> result = thread.get()
+    :param configuration: .Configuration object for this client
+    :param header_name: a header to pass when making calls to the API.
+    :param header_value: a header value to pass when making calls to
+        the API.
+    :param cookie: a cookie to include in the header when making calls
+        to the API
+    :param pool_threads: The number of threads to use for async requests
+        to the API. More threads means more concurrent API requests.
+    """
 
-        Args:
-            identifier (str): The PhotoIdentifier to get an approved photo for in the format `<value>@<scheme>`
+    _pool = None
 
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            None
-                If the method is called asynchronously, returns the request
-                thread.
+    def __init__(self, configuration=None, header_name=None, header_value=None,
+                 cookie=None, pool_threads=1):
+        if configuration is None:
+            configuration = Configuration.get_default_copy()
+        self.configuration = configuration
+        self.pool_threads = pool_threads
+
+        self.rest_client = rest.RESTClientObject(configuration)
+        self.default_headers = {}
+        if header_name is not None:
+            self.default_headers[header_name] = header_value
+        self.cookie = cookie
+        # Set default User-Agent.
+        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+
+    def close(self):
+        if self._pool:
+            self._pool.close()
+            self._pool.join()
+            self._pool = None
+            if hasattr(atexit, 'unregister'):
+                atexit.unregister(self.close)
+
+    @property
+    def pool(self):
+        """Create thread pool on first request
+         avoids instantiating unused threadpool for blocking clients.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['identifier'] = \
-            identifier
-        return self.v1beta1_approved_photos_content_retrieve_endpoint.call_with_http_info(**kwargs)
+        if self._pool is None:
+            atexit.register(self.close)
+            self._pool = ThreadPool(self.pool_threads)
+        return self._pool
+
+    @property
+    def user_agent(self):
+        """User agent for this API client"""
+        return self.default_headers['User-Agent']
+
+    @user_agent.setter
+    def user_agent(self, value):
+        self.default_headers['User-Agent'] = value
+
+    def set_default_header(self, header_name, header_value):
+        self.default_headers[header_name] = header_value
 
-    def v1beta1_approved_photos_content_transient_url_retrieve(
+    def __call_api(
         self,
-        identifier,
-        **kwargs
+        resource_path: str,
+        method: str,
+        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        body: typing.Optional[typing.Any] = None,
+        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
+        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
+        auth_settings: typing.Optional[typing.List[str]] = None,
+        _return_http_data_only: typing.Optional[bool] = None,
+        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
+        _preload_content: bool = True,
+        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
+        _host: typing.Optional[str] = None,
+        _check_type: typing.Optional[bool] = None,
+        _content_type: typing.Optional[str] = None,
+        _request_auths: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
     ):
-        """Get the transient url of the content of this approved photo  # noqa: E501
-
-         # Get transient URL of the content of an approved Photo  This endpoint returns a transient URL which can be used to fetch the most recently approved Photo's content for a PhotoIdentifier.  The PhotoIdentifier should be included in the URL params in the format `<value>@<scheme>` - see the introduction to this API for a list of supported schemes. If the scheme is not provided it is assumed to be a CRSid (v1.person.identifiers.cam.ac.uk).  A given PhotoIdentifier may link to many approved Photos, in which case the most recently approved Photo is returned here. If a PhotoIdentifier does not link to an approved Photo a `404` response will be returned.  The Photo returned may change over time if a new Photo is approved for a given PhotoIdentifier. If you want to keep a reference to an exact Photo you can use the Photo's `id` (the UUID), or `contentLink` of the Photo returned from the `Get approved Photo` endpoint above, which is guaranteed to always give back the same Photo, regardless of whether a new Photo is approved for a given PhotoIdentifier.  This endpoint returns both a publicly accessible URL and the expiry time of that URL in seconds.    # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1beta1_approved_photos_content_transient_url_retrieve(identifier, async_req=True)
-        >>> result = thread.get()
+        config = self.configuration
 
-        Args:
-            identifier (str): The PhotoIdentifier to get an approved photo for in the format `<value>@<scheme>`
+        # header parameters
+        header_params = header_params or {}
+        header_params.update(self.default_headers)
+        if self.cookie:
+            header_params['Cookie'] = self.cookie
+        if header_params:
+            header_params = self.sanitize_for_serialization(header_params)
+            header_params = dict(self.parameters_to_tuples(header_params,
+                                                           collection_formats))
+
+        # path parameters
+        if path_params:
+            path_params = self.sanitize_for_serialization(path_params)
+            path_params = self.parameters_to_tuples(path_params,
+                                                    collection_formats)
+            for k, v in path_params:
+                # specified safe chars, encode everything
+                resource_path = resource_path.replace(
+                    '{%s}' % k,
+                    quote(str(v), safe=config.safe_chars_for_path_param)
+                )
+
+        # query parameters
+        if query_params:
+            query_params = self.sanitize_for_serialization(query_params)
+            query_params = self.parameters_to_tuples(query_params,
+                                                     collection_formats)
+
+        # post parameters
+        if post_params or files:
+            post_params = post_params if post_params else []
+            post_params = self.sanitize_for_serialization(post_params)
+            post_params = self.parameters_to_tuples(post_params,
+                                                    collection_formats)
+            post_params.extend(self.files_parameters(files))
+            if header_params['Content-Type'].startswith("multipart"):
+                post_params = self.parameters_to_multipart(post_params,
+                                                           (dict))
+
+        # body
+        if body:
+            body = self.sanitize_for_serialization(body)
+
+        # auth setting
+        self.update_params_for_auth(header_params, query_params,
+                                    auth_settings, resource_path, method, body,
+                                    request_auths=_request_auths)
+
+        # request url
+        if _host is None:
+            url = self.configuration.host + resource_path
+        else:
+            # use server/host defined in path or operation instead
+            url = _host + resource_path
+
+        try:
+            # perform request and return response
+            response_data = self.request(
+                method, url, query_params=query_params, headers=header_params,
+                post_params=post_params, body=body,
+                _preload_content=_preload_content,
+                _request_timeout=_request_timeout)
+        except ApiException as e:
+            e.body = e.body.decode('utf-8')
+            raise e
+
+        self.last_response = response_data
+
+        return_data = response_data
+
+        if not _preload_content:
+            return (return_data)
+            return return_data
+
+        # deserialize response data
+        if response_type:
+            if response_type != (file_type,):
+                encoding = "utf-8"
+                content_type = response_data.getheader('content-type')
+                if content_type is not None:
+                    match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
+                    if match:
+                        encoding = match.group(1)
+                response_data.data = response_data.data.decode(encoding)
+
+            return_data = self.deserialize(
+                response_data,
+                response_type,
+                _check_type
+            )
+        else:
+            return_data = None
+
+        if _return_http_data_only:
+            return (return_data)
+        else:
+            return (return_data, response_data.status,
+                    response_data.getheaders())
+
+    def parameters_to_multipart(self, params, collection_types):
+        """Get parameters as list of tuples, formatting as json if value is collection_types
+
+        :param params: Parameters as list of two-tuples
+        :param dict collection_types: Parameter collection types
+        :return: Parameters as list of tuple or urllib3.fields.RequestField
+        """
+        new_params = []
+        if collection_types is None:
+            collection_types = (dict)
+        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
+            if isinstance(
+                     v, collection_types): # v is instance of collection_type, formatting as application/json
+                v = json.dumps(v, ensure_ascii=False).encode("utf-8")
+                field = RequestField(k, v)
+                field.make_multipart(content_type="application/json; charset=utf-8")
+                new_params.append(field)
+            else:
+                new_params.append((k, v))
+        return new_params
+
+    @classmethod
+    def sanitize_for_serialization(cls, obj):
+        """Prepares data for transmission before it is sent with the rest client
+        If obj is None, return None.
+        If obj is str, int, long, float, bool, return directly.
+        If obj is datetime.datetime, datetime.date
+            convert to string in iso8601 format.
+        If obj is list, sanitize each element in the list.
+        If obj is dict, return the dict.
+        If obj is OpenAPI model, return the properties dict.
+        If obj is io.IOBase, return the bytes
+        :param obj: The data to serialize.
+        :return: The serialized form of data.
+        """
+        if isinstance(obj, (ModelNormal, ModelComposed)):
+            return {
+                key: cls.sanitize_for_serialization(val) for key,
+                val in model_to_dict(
+                    obj,
+                    serialize=True).items()}
+        elif isinstance(obj, io.IOBase):
+            return cls.get_file_data_and_close_file(obj)
+        elif isinstance(obj, (str, int, float, none_type, bool)):
+            return obj
+        elif isinstance(obj, (datetime, date)):
+            return obj.isoformat()
+        elif isinstance(obj, ModelSimple):
+            return cls.sanitize_for_serialization(obj.value)
+        elif isinstance(obj, list):
+            return [cls.sanitize_for_serialization(item) for item in obj]
+        elif isinstance(obj, tuple):
+            return tuple(cls.sanitize_for_serialization(item) for item in obj)
+        if isinstance(obj, dict):
+            return {key: cls.sanitize_for_serialization(val) for key, val in obj.items()}
+        raise ApiValueError(
+            'Unable to prepare type {} for serialization'.format(
+                obj.__class__.__name__))
+
+    def deserialize(self, response, response_type, _check_type):
+        """Deserializes response into an object.
+
+        :param response: RESTResponse object to be deserialized.
+        :param response_type: For the response, a tuple containing:
+            valid classes
+            a list containing valid classes (for list schemas)
+            a dict containing a tuple of valid classes as the value
+            Example values:
+            (str,)
+            (Pet,)
+            (float, none_type)
+            ([int, none_type],)
+            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
+        :param _check_type: boolean, whether to check the types of the data
+            received from the server
+        :type _check_type: bool
 
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            TransientImageUrl
-                If the method is called asynchronously, returns the request
-                thread.
+        :return: deserialized object.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
+        # handle file downloading
+        # save response body into a tmp file and return the instance
+        if response_type == (file_type,):
+            content_disposition = response.getheader("Content-Disposition")
+            return deserialize_file(response.data, self.configuration,
+                                    content_disposition=content_disposition)
+
+        # fetch data from response object
+        try:
+            received_data = json.loads(response.data)
+        except ValueError:
+            received_data = response.data
+
+        # store our data under the key of 'received_data' so users have some
+        # context if they are deserializing a string and the data type is wrong
+        deserialized_data = validate_and_convert_types(
+            received_data,
+            response_type,
+            ['received_data'],
+            True,
+            _check_type,
+            configuration=self.configuration
         )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['identifier'] = \
-            identifier
-        return self.v1beta1_approved_photos_content_transient_url_retrieve_endpoint.call_with_http_info(**kwargs)
+        return deserialized_data
 
-    def v1beta1_approved_photos_list(
+    def call_api(
         self,
-        approved_since,
-        **kwargs
+        resource_path: str,
+        method: str,
+        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        body: typing.Optional[typing.Any] = None,
+        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
+        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
+        auth_settings: typing.Optional[typing.List[str]] = None,
+        async_req: typing.Optional[bool] = None,
+        _return_http_data_only: typing.Optional[bool] = None,
+        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
+        _preload_content: bool = True,
+        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
+        _host: typing.Optional[str] = None,
+        _check_type: typing.Optional[bool] = None,
+        _request_auths: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
     ):
-        """List approved photos  # noqa: E501
-
-         # List approved Photos  Return list of approved photos.  This endpoint allows information and metadata about approved Photos to be fetched. Approved photos must be filtered by approvedSince - which returns only photos which have been approved after a given point in time. This is to allow for incremental export of data, where the approvedSince can be specified as the point of the last export and only an increment of approved photo data queried.  Results are ordered by `approvedAt` ascending and may be split over multiple 'pages'. Where more results exist a `next` URL will be provided which can be used to fetch the next page of results. The `previous` URL can be used to navigate backwards through the result pages. The `pageSize` query parameter can be used to request a specific amount of results per page. If not provided the `pageSize` is set to `200`. The amount of results per page is limited to `500`, if a number greater than `500` is specified in the `pageSize` parameter no error is returned but the number of results will be capped at 500 per page.    # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
+        """Makes the HTTP request (synchronous) and returns deserialized data.
 
-        >>> thread = api.v1beta1_approved_photos_list(approved_since, async_req=True)
-        >>> result = thread.get()
+        To make an async_req request, set the async_req parameter.
 
-        Args:
-            approved_since (str): Specify the earliest datetime at which approved photos should be returned in ISO datetime format.
-
-        Keyword Args:
-            cursor (str): The pagination cursor value.. [optional]
-            page_size (int): Number of results to return per page.. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            PaginatedV1Beta1PhotoList
-                If the method is called asynchronously, returns the request
-                thread.
+        :param resource_path: Path to method endpoint.
+        :param method: Method to call.
+        :param path_params: Path parameters in the url.
+        :param query_params: Query parameters in the url.
+        :param header_params: Header parameters to be
+            placed in the request header.
+        :param body: Request body.
+        :param post_params dict: Request post form parameters,
+            for `application/x-www-form-urlencoded`, `multipart/form-data`.
+        :param auth_settings list: Auth Settings names for the request.
+        :param response_type: For the response, a tuple containing:
+            valid classes
+            a list containing valid classes (for list schemas)
+            a dict containing a tuple of valid classes as the value
+            Example values:
+            (str,)
+            (Pet,)
+            (float, none_type)
+            ([int, none_type],)
+            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
+        :param files: key -> field name, value -> a list of open file
+            objects for `multipart/form-data`.
+        :type files: dict
+        :param async_req bool: execute request asynchronously
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param collection_formats: dict of collection formats for path, query,
+            header, and post parameters.
+        :type collection_formats: dict, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _check_type: boolean describing if the data back from the server
+            should have its type checked.
+        :type _check_type: bool, optional
+        :param _request_auths: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auths: list, optional
+        :return:
+            If async_req parameter is True,
+            the request will be called asynchronously.
+            The method will return the request thread.
+            If parameter async_req is False or missing,
+            then the method will return the response directly.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['approved_since'] = \
-            approved_since
-        return self.v1beta1_approved_photos_list_endpoint.call_with_http_info(**kwargs)
-
-    def v1beta1_approved_photos_retrieve(
-        self,
-        identifier,
-        **kwargs
-    ):
-        """Get an approved photo of a person using a person identifier  # noqa: E501
+        if not async_req:
+            return self.__call_api(resource_path, method,
+                                   path_params, query_params, header_params,
+                                   body, post_params, files,
+                                   response_type, auth_settings,
+                                   _return_http_data_only, collection_formats,
+                                   _preload_content, _request_timeout, _host,
+                                   _check_type, _request_auths=_request_auths)
+
+        return self.pool.apply_async(self.__call_api, (resource_path,
+                                                       method, path_params,
+                                                       query_params,
+                                                       header_params, body,
+                                                       post_params, files,
+                                                       response_type,
+                                                       auth_settings,
+                                                       _return_http_data_only,
+                                                       collection_formats,
+                                                       _preload_content,
+                                                       _request_timeout,
+                                                       _host, _check_type, None, _request_auths))
+
+    def request(self, method, url, query_params=None, headers=None,
+                post_params=None, body=None, _preload_content=True,
+                _request_timeout=None):
+        """Makes the HTTP request using RESTClient."""
+        if method == "GET":
+            return self.rest_client.GET(url,
+                                        query_params=query_params,
+                                        _preload_content=_preload_content,
+                                        _request_timeout=_request_timeout,
+                                        headers=headers)
+        elif method == "HEAD":
+            return self.rest_client.HEAD(url,
+                                         query_params=query_params,
+                                         _preload_content=_preload_content,
+                                         _request_timeout=_request_timeout,
+                                         headers=headers)
+        elif method == "OPTIONS":
+            return self.rest_client.OPTIONS(url,
+                                            query_params=query_params,
+                                            headers=headers,
+                                            post_params=post_params,
+                                            _preload_content=_preload_content,
+                                            _request_timeout=_request_timeout,
+                                            body=body)
+        elif method == "POST":
+            return self.rest_client.POST(url,
+                                         query_params=query_params,
+                                         headers=headers,
+                                         post_params=post_params,
+                                         _preload_content=_preload_content,
+                                         _request_timeout=_request_timeout,
+                                         body=body)
+        elif method == "PUT":
+            return self.rest_client.PUT(url,
+                                        query_params=query_params,
+                                        headers=headers,
+                                        post_params=post_params,
+                                        _preload_content=_preload_content,
+                                        _request_timeout=_request_timeout,
+                                        body=body)
+        elif method == "PATCH":
+            return self.rest_client.PATCH(url,
+                                          query_params=query_params,
+                                          headers=headers,
+                                          post_params=post_params,
+                                          _preload_content=_preload_content,
+                                          _request_timeout=_request_timeout,
+                                          body=body)
+        elif method == "DELETE":
+            return self.rest_client.DELETE(url,
+                                           query_params=query_params,
+                                           headers=headers,
+                                           _preload_content=_preload_content,
+                                           _request_timeout=_request_timeout,
+                                           body=body)
+        else:
+            raise ApiValueError(
+                "http method must be `GET`, `HEAD`, `OPTIONS`,"
+                " `POST`, `PATCH`, `PUT` or `DELETE`."
+            )
+
+    def parameters_to_tuples(self, params, collection_formats):
+        """Get parameters as list of tuples, formatting collections.
+
+        :param params: Parameters as dict or list of two-tuples
+        :param dict collection_formats: Parameter collection formats
+        :return: Parameters as list of tuples, collections formatted
+        """
+        new_params = []
+        if collection_formats is None:
+            collection_formats = {}
+        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
+            if k in collection_formats:
+                collection_format = collection_formats[k]
+                if collection_format == 'multi':
+                    new_params.extend((k, value) for value in v)
+                else:
+                    if collection_format == 'ssv':
+                        delimiter = ' '
+                    elif collection_format == 'tsv':
+                        delimiter = '\t'
+                    elif collection_format == 'pipes':
+                        delimiter = '|'
+                    else:  # csv is the default
+                        delimiter = ','
+                    new_params.append(
+                        (k, delimiter.join(str(value) for value in v)))
+            else:
+                new_params.append((k, v))
+        return new_params
+
+    @staticmethod
+    def get_file_data_and_close_file(file_instance: io.IOBase) -> bytes:
+        file_data = file_instance.read()
+        file_instance.close()
+        return file_data
+
+    def files_parameters(self,
+                         files: typing.Optional[typing.Dict[str,
+                                                            typing.List[io.IOBase]]] = None):
+        """Builds form parameters.
+
+        :param files: None or a dict with key=param_name and
+            value is a list of open file objects
+        :return: List of tuples of form parameters with file data
+        """
+        if files is None:
+            return []
 
-         # Get approved Photo  Return the single, most recently approved, photo for a given PhotoIdentifier.  This endpoint allows information and metadata about an approved Photo to be fetched using a PhotoIdentifier. The PhotoIdentifier should be included in the URL params in the format `<value>@<scheme>` - see the introduction to this API for a list of supported schemes. If the scheme is not provided it is assumed to be a CRSid (v1.person.identifiers.cam.ac.uk).  A given PhotoIdentifier may link to many approved Photos, in which case the most recently approved Photo is returned here. If a PhotoIdentifier does not link to an approved Photo a `404` response is returned.  The Photo returned may change over time if a new Photo is approved for a given PhotoIdentifier. If you want to keep a reference to an exact Photo, you can use the Photo's `id` (the UUID), or `selfLink` returned to directly reference an instance of an immutable Photo.    # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
+        params = []
+        for param_name, file_instances in files.items():
+            if file_instances is None:
+                # if the file field is nullable, skip None values
+                continue
+            for file_instance in file_instances:
+                if file_instance is None:
+                    # if the file field is nullable, skip None values
+                    continue
+                if file_instance.closed is True:
+                    raise ApiValueError(
+                        "Cannot read a closed file. The passed in file_type "
+                        "for %s must be open." % param_name
+                    )
+                filename = os.path.basename(file_instance.name)
+                filedata = self.get_file_data_and_close_file(file_instance)
+                mimetype = (mimetypes.guess_type(filename)[0] or
+                            'application/octet-stream')
+                params.append(
+                    tuple([param_name, tuple([filename, filedata, mimetype])]))
 
-        >>> thread = api.v1beta1_approved_photos_retrieve(identifier, async_req=True)
-        >>> result = thread.get()
+        return params
 
-        Args:
-            identifier (str): The PhotoIdentifier to get an approved photo for in the format `<value>@<scheme>`
+    def select_header_accept(self, accepts):
+        """Returns `Accept` based on an array of accepts provided.
 
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            V1Beta1Photo
-                If the method is called asynchronously, returns the request
-                thread.
+        :param accepts: List of headers.
+        :return: Accept (e.g. application/json).
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['identifier'] = \
-            identifier
-        return self.v1beta1_approved_photos_retrieve_endpoint.call_with_http_info(**kwargs)
+        if not accepts:
+            return
 
-    def v1beta1_approved_photos_thumbnail_retrieve(
-        self,
-        identifier,
-        **kwargs
-    ):
-        """Get the thumbnail of an approved photo using a person identifier  # noqa: E501
-
-         # Get thumbnail of an approved Photo  This endpoint redirects to the thumbnail of the most recently approved Photo for the given PhotoIdentifier.  This thumbnail is guaranteed to be smaller than 128x128 pixels and will be in png format.  The documentation for the `Get image content of an approved Photo` additionally applies to this endpoint, as all constraints are the same between the two endpoints.    # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.v1beta1_approved_photos_thumbnail_retrieve(identifier, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            identifier (str): The PhotoIdentifier to get an approved photo for in the format `<value>@<scheme>`
+        accepts = [x.lower() for x in accepts]
 
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            None
-                If the method is called asynchronously, returns the request
-                thread.
+        if 'application/json' in accepts:
+            return 'application/json'
+        else:
+            return ', '.join(accepts)
+
+    def select_header_content_type(self, content_types, method=None, body=None):
+        """Returns `Content-Type` based on an array of content_types provided.
+
+        :param content_types: List of content-types.
+        :param method: http method (e.g. POST, PATCH).
+        :param body: http body to send.
+        :return: Content-Type (e.g. application/json).
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['identifier'] = \
-            identifier
-        return self.v1beta1_approved_photos_thumbnail_retrieve_endpoint.call_with_http_info(**kwargs)
+        if not content_types:
+            return None
 
-    def v1beta1_approved_photos_thumbnail_transient_url_retrieve(
-        self,
-        identifier,
-        **kwargs
-    ):
-        """Get the transient url of an the thumbnail of an approved photo using a person identifier  # noqa: E501
+        content_types = [x.lower() for x in content_types]
 
-         # Get transient URL of the thumbnail of an approved Photo  This endpoint returns a transient URL which can be used to fetch the most recently approved Photo's thumbnail for a given PhotoIdentifier.  This endpoint returns both a publically accessible URL and the expiry time of that URL in seconds.    # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
+        if (method == 'PATCH' and
+                'application/json-patch+json' in content_types and
+                isinstance(body, list)):
+            return 'application/json-patch+json'
+
+        if 'application/json' in content_types or '*/*' in content_types:
+            return 'application/json'
+        else:
+            return content_types[0]
+
+    def update_params_for_auth(self, headers, queries, auth_settings,
+                               resource_path, method, body, request_auths=None):
+        """Updates header and query params based on authentication setting.
+
+        :param headers: Header parameters dict to be updated.
+        :param queries: Query parameters tuple list to be updated.
+        :param auth_settings: Authentication setting identifiers list.
+        :param resource_path: A string representation of the HTTP request resource path.
+        :param method: A string representation of the HTTP request method.
+        :param body: A object representing the body of the HTTP request.
+            The object type is the return value of _encoder.default().
+        :param request_auths: if set, the provided settings will
+            override the token in the configuration.
+        """
+        if not auth_settings:
+            return
 
-        >>> thread = api.v1beta1_approved_photos_thumbnail_transient_url_retrieve(identifier, async_req=True)
-        >>> result = thread.get()
+        if request_auths:
+            for auth_setting in request_auths:
+                self._apply_auth_params(
+                    headers, queries, resource_path, method, body, auth_setting)
+            return
+
+        for auth in auth_settings:
+            auth_setting = self.configuration.auth_settings().get(auth)
+            if auth_setting:
+                self._apply_auth_params(
+                    headers, queries, resource_path, method, body, auth_setting)
+
+    def _apply_auth_params(self, headers, queries, resource_path, method, body, auth_setting):
+        if auth_setting['in'] == 'cookie':
+            headers['Cookie'] = auth_setting['key'] + "=" + auth_setting['value']
+        elif auth_setting['in'] == 'header':
+            if auth_setting['type'] != 'http-signature':
+                headers[auth_setting['key']] = auth_setting['value']
+        elif auth_setting['in'] == 'query':
+            queries.append((auth_setting['key'], auth_setting['value']))
+        else:
+            raise ApiValueError(
+                'Authentication token must be in `query` or `header`'
+            )
+
+
+class Endpoint(object):
+    def __init__(self, settings=None, params_map=None, root_map=None,
+                 headers_map=None, api_client=None, callable=None):
+        """Creates an endpoint
 
         Args:
-            identifier (str): The PhotoIdentifier to get an approved photo for in the format `<value>@<scheme>`
+            settings (dict): see below key value pairs
+                'response_type' (tuple/None): response type
+                'auth' (list): a list of auth type keys
+                'endpoint_path' (str): the endpoint path
+                'operation_id' (str): endpoint string identifier
+                'http_method' (str): POST/PUT/PATCH/GET etc
+                'servers' (list): list of str servers that this endpoint is at
+            params_map (dict): see below key value pairs
+                'all' (list): list of str endpoint parameter names
+                'required' (list): list of required parameter names
+                'nullable' (list): list of nullable parameter names
+                'enum' (list): list of parameters with enum values
+                'validation' (list): list of parameters with validations
+            root_map
+                'validations' (dict): the dict mapping endpoint parameter tuple
+                    paths to their validation dictionaries
+                'allowed_values' (dict): the dict mapping endpoint parameter
+                    tuple paths to their allowed_values (enum) dictionaries
+                'openapi_types' (dict): param_name to openapi type
+                'attribute_map' (dict): param_name to camelCase name
+                'location_map' (dict): param_name to  'body', 'file', 'form',
+                    'header', 'path', 'query'
+                collection_format_map (dict): param_name to `csv` etc.
+            headers_map (dict): see below key value pairs
+                'accept' (list): list of Accept header strings
+                'content_type' (list): list of Content-Type header strings
+            api_client (ApiClient) api client instance
+            callable (function): the function which is invoked when the
+                Endpoint is called
+        """
+        self.settings = settings
+        self.params_map = params_map
+        self.params_map['all'].extend([
+            'async_req',
+            '_host_index',
+            '_preload_content',
+            '_request_timeout',
+            '_return_http_data_only',
+            '_check_input_type',
+            '_check_return_type',
+            '_content_type',
+            '_spec_property_naming',
+            '_request_auths'
+        ])
+        self.params_map['nullable'].extend(['_request_timeout'])
+        self.validations = root_map['validations']
+        self.allowed_values = root_map['allowed_values']
+        self.openapi_types = root_map['openapi_types']
+        extra_types = {
+            'async_req': (bool,),
+            '_host_index': (none_type, int),
+            '_preload_content': (bool,),
+            '_request_timeout': (none_type, float, (float,), [float], int, (int,), [int]),
+            '_return_http_data_only': (bool,),
+            '_check_input_type': (bool,),
+            '_check_return_type': (bool,),
+            '_spec_property_naming': (bool,),
+            '_content_type': (none_type, str),
+            '_request_auths': (none_type, list)
+        }
+        self.openapi_types.update(extra_types)
+        self.attribute_map = root_map['attribute_map']
+        self.location_map = root_map['location_map']
+        self.collection_format_map = root_map['collection_format_map']
+        self.headers_map = headers_map
+        self.api_client = api_client
+        self.callable = callable
+
+    def __validate_inputs(self, kwargs):
+        for param in self.params_map['enum']:
+            if param in kwargs:
+                check_allowed_values(
+                    self.allowed_values,
+                    (param,),
+                    kwargs[param]
+                )
+
+        for param in self.params_map['validation']:
+            if param in kwargs:
+                check_validations(
+                    self.validations,
+                    (param,),
+                    kwargs[param],
+                    configuration=self.api_client.configuration
+                )
+
+        if kwargs['_check_input_type'] is False:
+            return
+
+        for key, value in kwargs.items():
+            fixed_val = validate_and_convert_types(
+                value,
+                self.openapi_types[key],
+                [key],
+                kwargs['_spec_property_naming'],
+                kwargs['_check_input_type'],
+                configuration=self.api_client.configuration
+            )
+            kwargs[key] = fixed_val
+
+    def __gather_params(self, kwargs):
+        params = {
+            'body': None,
+            'collection_format': {},
+            'file': {},
+            'form': [],
+            'header': {},
+            'path': {},
+            'query': []
+        }
+
+        for param_name, param_value in kwargs.items():
+            param_location = self.location_map.get(param_name)
+            if param_location is None:
+                continue
+            if param_location:
+                if param_location == 'body':
+                    params['body'] = param_value
+                    continue
+                base_name = self.attribute_map[param_name]
+                if (param_location == 'form' and
+                        self.openapi_types[param_name] == (file_type,)):
+                    params['file'][base_name] = [param_value]
+                elif (param_location == 'form' and
+                        self.openapi_types[param_name] == ([file_type],)):
+                    # param_value is already a list
+                    params['file'][base_name] = param_value
+                elif param_location in {'form', 'query'}:
+                    param_value_full = (base_name, param_value)
+                    params[param_location].append(param_value_full)
+                if param_location not in {'form', 'query'}:
+                    params[param_location][base_name] = param_value
+                collection_format = self.collection_format_map.get(param_name)
+                if collection_format:
+                    params['collection_format'][base_name] = collection_format
+
+        return params
+
+    def __call__(self, *args, **kwargs):
+        """ This method is invoked when endpoints are called
+        Example:
+
+        api_instance = APIVersionsApi()
+        api_instance.root_retrieve  # this is an instance of the class Endpoint
+        api_instance.root_retrieve()  # this invokes api_instance.root_retrieve.__call__()
+        which then invokes the callable functions stored in that endpoint at
+        api_instance.root_retrieve.callable or self.callable in this class
 
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            TransientImageUrl
-                If the method is called asynchronously, returns the request
-                thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['identifier'] = \
-            identifier
-        return self.v1beta1_approved_photos_thumbnail_transient_url_retrieve_endpoint.call_with_http_info(**kwargs)
+        return self.callable(self, *args, **kwargs)
+
+    def call_with_http_info(self, **kwargs):
 
+        try:
+            index = self.api_client.configuration.server_operation_index.get(
+                self.settings['operation_id'], self.api_client.configuration.server_index
+            ) if kwargs['_host_index'] is None else kwargs['_host_index']
+            server_variables = self.api_client.configuration.server_operation_variables.get(
+                self.settings['operation_id'], self.api_client.configuration.server_variables
+            )
+            _host = self.api_client.configuration.get_host_from_settings(
+                index, variables=server_variables, servers=self.settings['servers']
+            )
+        except IndexError:
+            if self.settings['servers']:
+                raise ApiValueError(
+                    "Invalid host index. Must be 0 <= index < %s" %
+                    len(self.settings['servers'])
+                )
+            _host = None
+
+        for key, value in kwargs.items():
+            if key not in self.params_map['all']:
+                raise ApiTypeError(
+                    "Got an unexpected parameter '%s'"
+                    " to method `%s`" %
+                    (key, self.settings['operation_id'])
+                )
+            # only throw this nullable ApiValueError if _check_input_type
+            # is False, if _check_input_type==True we catch this case
+            # in self.__validate_inputs
+            if (key not in self.params_map['nullable'] and value is None
+                    and kwargs['_check_input_type'] is False):
+                raise ApiValueError(
+                    "Value may not be None for non-nullable parameter `%s`"
+                    " when calling `%s`" %
+                    (key, self.settings['operation_id'])
+                )
+
+        for key in self.params_map['required']:
+            if key not in kwargs.keys():
+                raise ApiValueError(
+                    "Missing the required parameter `%s` when calling "
+                    "`%s`" % (key, self.settings['operation_id'])
+                )
+
+        self.__validate_inputs(kwargs)
+
+        params = self.__gather_params(kwargs)
+
+        accept_headers_list = self.headers_map['accept']
+        if accept_headers_list:
+            params['header']['Accept'] = self.api_client.select_header_accept(
+                accept_headers_list)
+
+        if kwargs.get('_content_type'):
+            params['header']['Content-Type'] = kwargs['_content_type']
+        else:
+            content_type_headers_list = self.headers_map['content_type']
+            if content_type_headers_list:
+                if params['body'] != "":
+                    content_types_list = self.api_client.select_header_content_type(
+                        content_type_headers_list, self.settings['http_method'],
+                        params['body'])
+                    if content_types_list:
+                        params['header']['Content-Type'] = content_types_list
+
+        return self.api_client.call_api(
+            self.settings['endpoint_path'], self.settings['http_method'],
+            params['path'],
+            params['query'],
+            params['header'],
+            body=params['body'],
+            post_params=params['form'],
+            files=params['file'],
+            response_type=self.settings['response_type'],
+            auth_settings=self.settings['auth'],
+            async_req=kwargs['async_req'],
+            _check_type=kwargs['_check_return_type'],
+            _return_http_data_only=kwargs['_return_http_data_only'],
+            _preload_content=kwargs['_preload_content'],
+            _request_timeout=kwargs['_request_timeout'],
+            _host=_host,
+            _request_auths=kwargs['_request_auths'],
+            collection_formats=params['collection_format'])
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/api/permissions_api.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,158 +5,155 @@
 
     The version of the OpenAPI document: v1beta1
     Contact: devops+photoapi@uis.cam.ac.uk
     Generated by: https://openapi-generator.tech
 """
 
 
-import re  # noqa: F401
-import sys  # noqa: F401
+class OpenApiException(Exception):
+    """The base exception class for all OpenAPIExceptions"""
 
-from identitylib.photo_client.api_client import ApiClient, Endpoint as _Endpoint
-from identitylib.photo_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
-)
-from identitylib.photo_client.model.permissions import Permissions
-
-
-class PermissionsApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.permissions_retrieve_endpoint = _Endpoint(
-            settings={
-                'response_type': (Permissions,),
-                'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
-                ],
-                'endpoint_path': '/permissions',
-                'operation_id': 'permissions_retrieve',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
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
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-
-    def permissions_retrieve(
-        self,
-        **kwargs
-    ):
-        """List permissions  # noqa: E501
-
-        List the permissions of the current principal  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.permissions_retrieve(async_req=True)
-        >>> result = thread.get()
+class ApiTypeError(OpenApiException, TypeError):
+    def __init__(self, msg, path_to_item=None, valid_classes=None,
+                 key_type=None):
+        """ Raises an exception for TypeErrors
 
+        Args:
+            msg (str): the exception message
 
         Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            Permissions
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.permissions_retrieve_endpoint.call_with_http_info(**kwargs)
+            path_to_item (list): a list of keys an indices to get to the
+                                 current_item
+                                 None if unset
+            valid_classes (tuple): the primitive classes that current item
+                                   should be an instance of
+                                   None if unset
+            key_type (bool): False if our value is a value in a dict
+                             True if it is a key in a dict
+                             False if our item is an item in a list
+                             None if unset
+        """
+        self.path_to_item = path_to_item
+        self.valid_classes = valid_classes
+        self.key_type = key_type
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiTypeError, self).__init__(full_msg)
+
+
+class ApiValueError(OpenApiException, ValueError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (list) the path to the exception in the
+                received_data dict. None if unset
+        """
+
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiValueError, self).__init__(full_msg)
+
+
+class ApiAttributeError(OpenApiException, AttributeError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Raised when an attribute reference or assignment fails.
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiAttributeError, self).__init__(full_msg)
+
+
+class ApiKeyError(OpenApiException, KeyError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiKeyError, self).__init__(full_msg)
+
+
+class ApiException(OpenApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
+        else:
+            self.status = status
+            self.reason = reason
+            self.body = None
+            self.headers = None
+
+    def __str__(self):
+        """Custom error messages for exception"""
+        error_message = "Status Code: {0}\n"\
+                        "Reason: {1}\n".format(self.status, self.reason)
+        if self.headers:
+            error_message += "HTTP response headers: {0}\n".format(
+                self.headers)
+
+        if self.body:
+            error_message += "HTTP response body: {0}\n".format(self.body)
+
+        return error_message
+
+
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
 
+def render_path(path_to_item):
+    """Returns a string representation of a path"""
+    result = ""
+    for pth in path_to_item:
+        if isinstance(pth, int):
+            result += "[{0}]".format(pth)
+        else:
+            result += "['{0}']".format(pth)
+    return result
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifiers_api.py` & `ucam-identitylib-2.0.0/identitylib/student_client/api/students_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,320 +1,227 @@
 """
-    University Photo API
+    University Student API
 
-     ## Introduction  The Photo API allows access to Photos of members of the University. The Photos exposed by this API are expected to be a good representation of the person they relate to.  The API broadly follows the principles of REST and strives to provide an interface that can be easily consumed by downstream systems.  ### Stability  This release of the Photo API is a `beta` offering: a service we are moving towards live but which requires wider testing with a broader group of users.  ### Versioning  The Photo API is versioned using URL path prefixes in the format: `/v1beta1/photos`. This follows the pattern established by the [GCP API](https://cloud.google.com/apis/design/versioning). Breaking changes will not be made without a change in API major version, however non-breaking changes will be introduced without changes to the version path prefix. All changes will be documented in the project's [CHANGELOG](https://gitlab.developers.cam.ac.uk/uis/devops/iam/photo-api/-/blob/master/CHANGELOG.md)  The available versions of the API are listed at the API's root.  ### Domain  The Photo API serves Photos of members of the University, linking a Photo to an individual through `PhotoIdentifiers` (see below) which pertain to a person record within an external system.  The Photos served by the Photo API are expected to be of sufficient quality to identify the person they represent. Photos which have been reviewed and determined to be sufficient quality are marked as having the status `approved` and exposed through the `approved-photos` endpoints.  ### Data source  The Photos exposed by the Photo API are currently a mirror of card Photos contained within the [Card Database](https://webservices.admin.cam.ac.uk/uc/). With Photos being synced from the Card Database to the Photo API hourly.  In future, the Photo API will be extended to allow Photos to be created and 'approved' using the API.  ## Core entities  ### The `Photo` Entity  The `Photo` entity contains information and metadata about a Photo of a member of the university. The `status` field on a Photo indicates whether this Photo has been reviewed and approved. Only Photos which have the status `approved` are exposed through the `approved-photos` endpoints. Each photo entity has a unique identifier - termed UUID - which is used in the system to refer to the specific photo entity. The UUID is provided in JSON documents as the `id` property.   Each Photo entity contains a link to the image data itself and a thumbnail for this Photo, which is guaranteed to be less than 128x128 pixels. Images are served by redirecting to a temporary URL provided by the service used to host images. These temporary URLs will expire after an hour and should not be retained for long-lasting access to a given Photo.  Each Photo may contain a block of JSON metadata recording information about the Photo. Photos cannot be updated once created (apart from to move their status to `approved`) hence this metadata should not be used to store application state or any other information which is not related to the content of the Photo.  Each Photo will have a set of `PhotoIdentifier` which allow the Photo to be linked to a person record within another system.  ### The `PhotoIdentifier` Entity  The `PhotoIdentifier` entity holds the `value` and `scheme` of a given identifier. The `value` field of a `PhotoIdentifier` is a simple ID string - e.g. `wgd23` or `000001`. The `scheme` field of a `PhotoIdentifier` indicates what system this identifier relates to or was issued by. This allows many identifiers which relate to different systems to be recorded against a single `Photo`.  The supported schemes are: * `v1.person.identifiers.cam.ac.uk`: The CRSID of the person represented by this Photo * `person.v1.student-records.university.identifiers.cam.ac.uk`: The CamSIS identifier (USN) of the person represented by this Photo * `person.v1.human-resources.university.identifiers.cam.ac.uk`: The CHRIS identifier (staff number) of the person represented by this Photo * `photo.v1.legacy-card.university.identifiers.cam.ac.uk`: The id of this Photo within the legacy card system  ## Using the API  ### Auth  To authenticate against the Photo API, an application must be registered within the API Gateway and granted access to the `University Photo` product. Details of how to register an application and grant access to products can be found in the [API Gateway Getting Started Guide](https://developer.api.apps.cam.ac.uk/start-using-an-api).    # noqa: E501
+    This API exposes identity information about university students. The purpose of this API is to give access to basic identity information about university students for use by downstream systems, therefore the data exposed is limited to basic information about who a student is and which institutions they are affiliated with.  This API uses the following identifiers to link people to person-records held within different systems:  * `person.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) identifier of this person -   also referred to as USN  Additionally this API uses the following identifiers to link people to institutions or entities which a person may have an affiliation to:  * `institution.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) institution identifier.     This encompasses colleges, departments and faculties. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under A01 and M01). * `academic-plan.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) academic plan     identifier. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under D07).  Both affiliations provide a `status` field which indicate a student's status within an affiliated entity. This `status` field is the short representation of the academic career field held in CamSIS. The [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual) lists the available values for the `status` field (under D05).  This API is currently backed by data from CamSIS, exposing a view of data that is refreshed nightly.    # noqa: E501
 
-    The version of the OpenAPI document: v1beta1
-    Contact: devops+photoapi@uis.cam.ac.uk
+    The version of the OpenAPI document: v1alpha2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from identitylib.photo_client.api_client import ApiClient, Endpoint as _Endpoint
-from identitylib.photo_client.model_utils import (  # noqa: F401
+from identitylib.student_client.api_client import ApiClient, Endpoint as _Endpoint
+from identitylib.student_client.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from identitylib.photo_client.model.bad_request import BadRequest
-from identitylib.photo_client.model.forbidden import Forbidden
-from identitylib.photo_client.model.internal_server_error import InternalServerError
-from identitylib.photo_client.model.not_found import NotFound
-from identitylib.photo_client.model.paginated_v1_beta1_photo_identifier_summary_list import PaginatedV1Beta1PhotoIdentifierSummaryList
-from identitylib.photo_client.model.photo_identifier_bulk_update_request_request import PhotoIdentifierBulkUpdateRequestRequest
-from identitylib.photo_client.model.unauthorized import Unauthorized
-from identitylib.photo_client.model.v1_beta1_photo_identifier_summary_request import V1Beta1PhotoIdentifierSummaryRequest
+from identitylib.student_client.model.http_exception import HTTPException
+from identitylib.student_client.model.http_validation_error import HTTPValidationError
+from identitylib.student_client.model.paginated_results_student import PaginatedResultsStudent
+from identitylib.student_client.model.student import Student
 
 
-class PhotoIdentifiersApi(object):
+class StudentsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.v1beta1_photo_identifiers_list_endpoint = _Endpoint(
+        self.get_v1alpha2_student_students_identifier_get_endpoint = _Endpoint(
             settings={
-                'response_type': (PaginatedV1Beta1PhotoIdentifierSummaryList,),
+                'response_type': (Student,),
                 'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
+                    'ApiGatewayOAuthClientCredentials'
                 ],
-                'endpoint_path': '/v1beta1/photo-identifiers',
-                'operation_id': 'v1beta1_photo_identifiers_list',
+                'endpoint_path': '/students/{identifier}',
+                'operation_id': 'get_v1alpha2_student_students_identifier_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'cursor',
-                    'deleted_at__gte',
-                    'deleted_at__is_null',
-                    'deleted_at__isnull',
-                    'deleted_at__lte',
                     'identifier',
-                    'is_highest_primary_identifier',
-                    'page_size',
-                    'retain_until__gte',
-                    'retain_until__is_null',
-                    'retain_until__isnull',
-                    'retain_until__lte',
-                    'scheme',
                 ],
-                'required': [],
+                'required': [
+                    'identifier',
+                ],
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
-                    'cursor':
-                        (str,),
-                    'deleted_at__gte':
-                        (str,),
-                    'deleted_at__is_null':
-                        (bool,),
-                    'deleted_at__isnull':
-                        (bool,),
-                    'deleted_at__lte':
-                        (str,),
                     'identifier':
                         (str,),
-                    'is_highest_primary_identifier':
-                        (bool,),
-                    'page_size':
-                        (int,),
-                    'retain_until__gte':
-                        (str,),
-                    'retain_until__is_null':
-                        (bool,),
-                    'retain_until__isnull':
-                        (bool,),
-                    'retain_until__lte':
-                        (str,),
-                    'scheme':
-                        (str,),
                 },
                 'attribute_map': {
-                    'cursor': 'cursor',
-                    'deleted_at__gte': 'deleted_at__gte',
-                    'deleted_at__is_null': 'deleted_at__isNull',
-                    'deleted_at__isnull': 'deleted_at__isnull',
-                    'deleted_at__lte': 'deleted_at__lte',
                     'identifier': 'identifier',
-                    'is_highest_primary_identifier': 'is_highest_primary_identifier',
-                    'page_size': 'pageSize',
-                    'retain_until__gte': 'retain_until__gte',
-                    'retain_until__is_null': 'retain_until__isNull',
-                    'retain_until__isnull': 'retain_until__isnull',
-                    'retain_until__lte': 'retain_until__lte',
-                    'scheme': 'scheme',
                 },
                 'location_map': {
-                    'cursor': 'query',
-                    'deleted_at__gte': 'query',
-                    'deleted_at__is_null': 'query',
-                    'deleted_at__isnull': 'query',
-                    'deleted_at__lte': 'query',
-                    'identifier': 'query',
-                    'is_highest_primary_identifier': 'query',
-                    'page_size': 'query',
-                    'retain_until__gte': 'query',
-                    'retain_until__is_null': 'query',
-                    'retain_until__isnull': 'query',
-                    'retain_until__lte': 'query',
-                    'scheme': 'query',
+                    'identifier': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.v1beta1_photo_identifiers_update_endpoint = _Endpoint(
+        self.list_v1alpha2_recent_graduates_recent_graduates_get_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (PaginatedResultsStudent,),
                 'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
+                    'ApiGatewayOAuthClientCredentials'
                 ],
-                'endpoint_path': '/v1beta1/photo-identifiers/{id}',
-                'operation_id': 'v1beta1_photo_identifiers_update',
-                'http_method': 'PUT',
+                'endpoint_path': '/recent-graduates',
+                'operation_id': 'list_v1alpha2_recent_graduates_recent_graduates_get',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id',
-                    'v1_beta1_photo_identifier_summary_request',
-                    'action',
-                ],
-                'required': [
-                    'id',
-                    'v1_beta1_photo_identifier_summary_request',
+                    'affiliation',
+                    'cursor',
                 ],
+                'required': [],
                 'nullable': [
+                    'affiliation',
                 ],
                 'enum': [
-                    'action',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('action',): {
-
-                        "HARD_DELETE": "hard_delete",
-                        "RESTORE": "restore",
-                        "SET_RETENTION": "set_retention",
-                        "SOFT_DELETE": "soft_delete"
-                    },
                 },
                 'openapi_types': {
-                    'id':
-                        (str,),
-                    'v1_beta1_photo_identifier_summary_request':
-                        (V1Beta1PhotoIdentifierSummaryRequest,),
-                    'action':
+                    'affiliation':
+                        (str, none_type,),
+                    'cursor':
                         (str,),
                 },
                 'attribute_map': {
-                    'id': 'id',
-                    'action': 'action',
+                    'affiliation': 'affiliation',
+                    'cursor': 'cursor',
                 },
                 'location_map': {
-                    'id': 'path',
-                    'v1_beta1_photo_identifier_summary_request': 'body',
-                    'action': 'query',
+                    'affiliation': 'query',
+                    'cursor': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.v1beta1_photo_identifiers_update_update_endpoint = _Endpoint(
+        self.list_v1alpha2_students_students_get_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (PaginatedResultsStudent,),
                 'auth': [
-                    'apiGatewayAuthorizationCodeSecurityScheme',
-                    'apiGatewayClientCredentialsSecurityScheme'
+                    'ApiGatewayOAuthClientCredentials'
                 ],
-                'endpoint_path': '/v1beta1/photo-identifiers/update',
-                'operation_id': 'v1beta1_photo_identifiers_update_update',
-                'http_method': 'PUT',
+                'endpoint_path': '/students',
+                'operation_id': 'list_v1alpha2_students_students_get',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'photo_identifier_bulk_update_request_request',
-                ],
-                'required': [
-                    'photo_identifier_bulk_update_request_request',
+                    'affiliation',
+                    'cursor',
                 ],
+                'required': [],
                 'nullable': [
+                    'affiliation',
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
-                    'photo_identifier_bulk_update_request_request':
-                        (PhotoIdentifierBulkUpdateRequestRequest,),
+                    'affiliation':
+                        (str, none_type,),
+                    'cursor':
+                        (str,),
                 },
                 'attribute_map': {
+                    'affiliation': 'affiliation',
+                    'cursor': 'cursor',
                 },
                 'location_map': {
-                    'photo_identifier_bulk_update_request_request': 'body',
+                    'affiliation': 'query',
+                    'cursor': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
 
-    def v1beta1_photo_identifiers_list(
+    def get_v1alpha2_student_students_identifier_get(
         self,
+        identifier,
         **kwargs
     ):
-        """List photo identifiers  # noqa: E501
+        """Get a single student  # noqa: E501
 
-         ## List photo identifiers  Returns a list of photo identifiers associated with the photos.  ### Permissions  Principals with the `PHOTO_VIEWER` permission are able to view all photo identifiers contained within the photo system.    # noqa: E501
+        Returns a single student based on the identifier provided. The identifier can be provided in the format `<value>@<scheme>`, if the scheme is omitted it shall be assumed that the scheme is `person.v1.student-records.university.identifiers.cam.ac.uk` (also know as the USN).   Currently this endpoint only supports querying by `person.v1.student-records.university.identifiers.cam.ac.uk` identifiers, but may be extended to allow querying by additional identifier schemes in future.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1beta1_photo_identifiers_list(async_req=True)
+        >>> thread = api.get_v1alpha2_student_students_identifier_get(identifier, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            identifier (str):
 
         Keyword Args:
-            cursor (str): The pagination cursor value.. [optional]
-            deleted_at__gte (str): Filter deletedAt by IsoDateTime greater than. [optional]
-            deleted_at__is_null (bool): Filter deletedAt by IsoDateTime is Null. [optional]
-            deleted_at__isnull (bool): [optional]
-            deleted_at__lte (str): Filter deletedAt by IsoDateTime less than. [optional]
-            identifier (str): PhotoIdentifier to get photos for using format `<value>@<scheme>`. [optional]
-            is_highest_primary_identifier (bool): Filter is_highest_primary_identifier. [optional]
-            page_size (int): Number of results to return per page.. [optional]
-            retain_until__gte (str): Filter retainUntil by IsoDateTime greater than. [optional]
-            retain_until__is_null (bool): Filter retainUntil by IsoDateTime is Null. [optional]
-            retain_until__isnull (bool): [optional]
-            retain_until__lte (str): Filter retainUntil by IsoDateTime less than. [optional]
-            scheme (str): PhotoIdentifier scheme to get photos for using format `<scheme>`. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -339,15 +246,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            PaginatedV1Beta1PhotoIdentifierSummaryList
+            Student
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -368,37 +275,35 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.v1beta1_photo_identifiers_list_endpoint.call_with_http_info(**kwargs)
+        kwargs['identifier'] = \
+            identifier
+        return self.get_v1alpha2_student_students_identifier_get_endpoint.call_with_http_info(**kwargs)
 
-    def v1beta1_photo_identifiers_update(
+    def list_v1alpha2_recent_graduates_recent_graduates_get(
         self,
-        id,
-        v1_beta1_photo_identifier_summary_request,
         **kwargs
     ):
-        """Update a photo identifier by photo identifier UUID.  # noqa: E501
+        """List students who have completed a course within the last six months  # noqa: E501
 
-         ## Update the photo identifier  This method allows a client to submit an action in the request query for a given photo identifier. The allowed actions are `set_retention`, `restore`, `soft_delete` and `hard_delete`.  ### Permissions  Principals with the `CARD_ADMIN` permission will be able to affect this endpoint.    # noqa: E501
+        Returns students who have ended their affiliation with an institution or academic plan within the last six months, indicating that they have recently completed their studies. This is to allow downstream systems access to data on students who may in-practice continue to have an affiliation with the University, even though their course has technically ended.  Affiliations populated on each recent graduate are limited to the affiliations which have ended within the last six months. Graduates may have additional affiliations which are not represented here. These affiliations can be accessed by querying the `/students` endpoint.  Students who have either been removed or withdrawn from a course are not returned.  To avoid returning very large responses, this endpoint produces a paged response. Where there are additional results which cannot be returned on a single page, a `next` field will be populated with a url containing the next page of results. These `next` urls should be followed until a page is returned with no `next` field, indicating that there are no further results. Each page returned will hold a maximum of 1000 results.  Graduates can be filtered by affiliation, by providing an `affiliation` query parameter. This affiliation should be provided in the format `<value>@<scheme>`. Graduates will only be returned if their affiliation with an institution or academic plan has ended within the last six months.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1beta1_photo_identifiers_update(id, v1_beta1_photo_identifier_summary_request, async_req=True)
+        >>> thread = api.list_v1alpha2_recent_graduates_recent_graduates_get(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            id (str): A UUID string identifying this photo identifier.
-            v1_beta1_photo_identifier_summary_request (V1Beta1PhotoIdentifierSummaryRequest):
 
         Keyword Args:
-            action (str): Action applied to the photo identifier.. [optional]
+            affiliation (str, none_type): An affiliation to filter by, in the format `<value>@<scheme>`. When included only graduates with a matching affiliation are returned.. [optional]
+            cursor (str): The cursor indicating a unique page of results - this should be auto generated on the `next` and `previous` fields and does not need to be manually added / updated.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -423,15 +328,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            PaginatedResultsStudent
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -452,38 +357,33 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['id'] = \
-            id
-        kwargs['v1_beta1_photo_identifier_summary_request'] = \
-            v1_beta1_photo_identifier_summary_request
-        return self.v1beta1_photo_identifiers_update_endpoint.call_with_http_info(**kwargs)
+        return self.list_v1alpha2_recent_graduates_recent_graduates_get_endpoint.call_with_http_info(**kwargs)
 
-    def v1beta1_photo_identifiers_update_update(
+    def list_v1alpha2_students_students_get(
         self,
-        photo_identifier_bulk_update_request_request,
         **kwargs
     ):
-        """Bulk update photo identifiers by photo identifier UUID.  # noqa: E501
+        """List students  # noqa: E501
 
-         ## Bulk update the photo identifier  This method allows a client to submit a list of photo identifiers and corresponding action to apply to the photo identifier. The allowed actions are `set_retention`, `restore`, `soft_delete` and `hard_delete`.  ### Permissions  Principals with the `CARD_ADMIN` permission will be able to affect this endpoint.    # noqa: E501
+        Lists all students held within the University Student management system, allowing basic filtering by affiliation.  To avoid returning very large responses, this endpoint produces a paged response. Where there are additional results which cannot be returned on a single page, a `next` field will be populated with a url containing the next page of results. These `next` urls should be followed until a page is returned with no `next` field, indicating that there are no further results. Each page returned will hold a maximum of 1000 results.  Students can be filtered by affiliation, by providing an `affiliation` query parameter. This affiliation should be provided in the format `<value>@<scheme>`.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1beta1_photo_identifiers_update_update(photo_identifier_bulk_update_request_request, async_req=True)
+        >>> thread = api.list_v1alpha2_students_students_get(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            photo_identifier_bulk_update_request_request (PhotoIdentifierBulkUpdateRequestRequest):
 
         Keyword Args:
+            affiliation (str, none_type): An affiliation to filter by, in the format `<value>@<scheme>`. When included only the students with a matching affiliation are returned.. [optional]
+            cursor (str): The cursor indicating a unique page of results - this should be auto generated on the `next` and `previous` fields and does not need to be manually added / updated.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -508,15 +408,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            PaginatedResultsStudent
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -537,11 +437,9 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['photo_identifier_bulk_update_request_request'] = \
-            photo_identifier_bulk_update_request_request
-        return self.v1beta1_photo_identifiers_update_update_endpoint.call_with_http_info(**kwargs)
+        return self.list_v1alpha2_students_students_get_endpoint.call_with_http_info(**kwargs)
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/api_client.py` & `ucam-identitylib-2.0.0/identitylib/student_client/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
-    University Photo API
+    University Student API
 
-     ## Introduction  The Photo API allows access to Photos of members of the University. The Photos exposed by this API are expected to be a good representation of the person they relate to.  The API broadly follows the principles of REST and strives to provide an interface that can be easily consumed by downstream systems.  ### Stability  This release of the Photo API is a `beta` offering: a service we are moving towards live but which requires wider testing with a broader group of users.  ### Versioning  The Photo API is versioned using URL path prefixes in the format: `/v1beta1/photos`. This follows the pattern established by the [GCP API](https://cloud.google.com/apis/design/versioning). Breaking changes will not be made without a change in API major version, however non-breaking changes will be introduced without changes to the version path prefix. All changes will be documented in the project's [CHANGELOG](https://gitlab.developers.cam.ac.uk/uis/devops/iam/photo-api/-/blob/master/CHANGELOG.md)  The available versions of the API are listed at the API's root.  ### Domain  The Photo API serves Photos of members of the University, linking a Photo to an individual through `PhotoIdentifiers` (see below) which pertain to a person record within an external system.  The Photos served by the Photo API are expected to be of sufficient quality to identify the person they represent. Photos which have been reviewed and determined to be sufficient quality are marked as having the status `approved` and exposed through the `approved-photos` endpoints.  ### Data source  The Photos exposed by the Photo API are currently a mirror of card Photos contained within the [Card Database](https://webservices.admin.cam.ac.uk/uc/). With Photos being synced from the Card Database to the Photo API hourly.  In future, the Photo API will be extended to allow Photos to be created and 'approved' using the API.  ## Core entities  ### The `Photo` Entity  The `Photo` entity contains information and metadata about a Photo of a member of the university. The `status` field on a Photo indicates whether this Photo has been reviewed and approved. Only Photos which have the status `approved` are exposed through the `approved-photos` endpoints. Each photo entity has a unique identifier - termed UUID - which is used in the system to refer to the specific photo entity. The UUID is provided in JSON documents as the `id` property.   Each Photo entity contains a link to the image data itself and a thumbnail for this Photo, which is guaranteed to be less than 128x128 pixels. Images are served by redirecting to a temporary URL provided by the service used to host images. These temporary URLs will expire after an hour and should not be retained for long-lasting access to a given Photo.  Each Photo may contain a block of JSON metadata recording information about the Photo. Photos cannot be updated once created (apart from to move their status to `approved`) hence this metadata should not be used to store application state or any other information which is not related to the content of the Photo.  Each Photo will have a set of `PhotoIdentifier` which allow the Photo to be linked to a person record within another system.  ### The `PhotoIdentifier` Entity  The `PhotoIdentifier` entity holds the `value` and `scheme` of a given identifier. The `value` field of a `PhotoIdentifier` is a simple ID string - e.g. `wgd23` or `000001`. The `scheme` field of a `PhotoIdentifier` indicates what system this identifier relates to or was issued by. This allows many identifiers which relate to different systems to be recorded against a single `Photo`.  The supported schemes are: * `v1.person.identifiers.cam.ac.uk`: The CRSID of the person represented by this Photo * `person.v1.student-records.university.identifiers.cam.ac.uk`: The CamSIS identifier (USN) of the person represented by this Photo * `person.v1.human-resources.university.identifiers.cam.ac.uk`: The CHRIS identifier (staff number) of the person represented by this Photo * `photo.v1.legacy-card.university.identifiers.cam.ac.uk`: The id of this Photo within the legacy card system  ## Using the API  ### Auth  To authenticate against the Photo API, an application must be registered within the API Gateway and granted access to the `University Photo` product. Details of how to register an application and grant access to products can be found in the [API Gateway Getting Started Guide](https://developer.api.apps.cam.ac.uk/start-using-an-api).    # noqa: E501
+    This API exposes identity information about university students. The purpose of this API is to give access to basic identity information about university students for use by downstream systems, therefore the data exposed is limited to basic information about who a student is and which institutions they are affiliated with.  This API uses the following identifiers to link people to person-records held within different systems:  * `person.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) identifier of this person -   also referred to as USN  Additionally this API uses the following identifiers to link people to institutions or entities which a person may have an affiliation to:  * `institution.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) institution identifier.     This encompasses colleges, departments and faculties. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under A01 and M01). * `academic-plan.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) academic plan     identifier. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under D07).  Both affiliations provide a `status` field which indicate a student's status within an affiliated entity. This `status` field is the short representation of the academic career field held in CamSIS. The [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual) lists the available values for the `status` field (under D05).  This API is currently backed by data from CamSIS, exposing a view of data that is refreshed nightly.    # noqa: E501
 
-    The version of the OpenAPI document: v1beta1
-    Contact: devops+photoapi@uis.cam.ac.uk
+    The version of the OpenAPI document: v1alpha2
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -17,18 +16,18 @@
 import os
 import re
 import typing
 from urllib.parse import quote
 from urllib3.fields import RequestField
 
 
-from identitylib.photo_client import rest
-from identitylib.photo_client.configuration import Configuration
-from identitylib.photo_client.exceptions import ApiTypeError, ApiValueError, ApiException
-from identitylib.photo_client.model_utils import (
+from identitylib.student_client import rest
+from identitylib.student_client.configuration import Configuration
+from identitylib.student_client.exceptions import ApiTypeError, ApiValueError, ApiException
+from identitylib.student_client.model_utils import (
     ModelNormal,
     ModelSimple,
     ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
@@ -800,19 +799,19 @@
 
         return params
 
     def __call__(self, *args, **kwargs):
         """ This method is invoked when endpoints are called
         Example:
 
-        api_instance = APIVersionsApi()
-        api_instance.root_retrieve  # this is an instance of the class Endpoint
-        api_instance.root_retrieve()  # this invokes api_instance.root_retrieve.__call__()
+        api_instance = StudentsApi()
+        api_instance.get_v1alpha2_student_students_identifier_get  # this is an instance of the class Endpoint
+        api_instance.get_v1alpha2_student_students_identifier_get()  # this invokes api_instance.get_v1alpha2_student_students_identifier_get.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.root_retrieve.callable or self.callable in this class
+        api_instance.get_v1alpha2_student_students_identifier_get.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
 
         try:
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/configuration.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/exceptions.py` & `ucam-identitylib-2.0.0/identitylib/student_client/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
-    University Photo API
+    University Student API
 
-     ## Introduction  The Photo API allows access to Photos of members of the University. The Photos exposed by this API are expected to be a good representation of the person they relate to.  The API broadly follows the principles of REST and strives to provide an interface that can be easily consumed by downstream systems.  ### Stability  This release of the Photo API is a `beta` offering: a service we are moving towards live but which requires wider testing with a broader group of users.  ### Versioning  The Photo API is versioned using URL path prefixes in the format: `/v1beta1/photos`. This follows the pattern established by the [GCP API](https://cloud.google.com/apis/design/versioning). Breaking changes will not be made without a change in API major version, however non-breaking changes will be introduced without changes to the version path prefix. All changes will be documented in the project's [CHANGELOG](https://gitlab.developers.cam.ac.uk/uis/devops/iam/photo-api/-/blob/master/CHANGELOG.md)  The available versions of the API are listed at the API's root.  ### Domain  The Photo API serves Photos of members of the University, linking a Photo to an individual through `PhotoIdentifiers` (see below) which pertain to a person record within an external system.  The Photos served by the Photo API are expected to be of sufficient quality to identify the person they represent. Photos which have been reviewed and determined to be sufficient quality are marked as having the status `approved` and exposed through the `approved-photos` endpoints.  ### Data source  The Photos exposed by the Photo API are currently a mirror of card Photos contained within the [Card Database](https://webservices.admin.cam.ac.uk/uc/). With Photos being synced from the Card Database to the Photo API hourly.  In future, the Photo API will be extended to allow Photos to be created and 'approved' using the API.  ## Core entities  ### The `Photo` Entity  The `Photo` entity contains information and metadata about a Photo of a member of the university. The `status` field on a Photo indicates whether this Photo has been reviewed and approved. Only Photos which have the status `approved` are exposed through the `approved-photos` endpoints. Each photo entity has a unique identifier - termed UUID - which is used in the system to refer to the specific photo entity. The UUID is provided in JSON documents as the `id` property.   Each Photo entity contains a link to the image data itself and a thumbnail for this Photo, which is guaranteed to be less than 128x128 pixels. Images are served by redirecting to a temporary URL provided by the service used to host images. These temporary URLs will expire after an hour and should not be retained for long-lasting access to a given Photo.  Each Photo may contain a block of JSON metadata recording information about the Photo. Photos cannot be updated once created (apart from to move their status to `approved`) hence this metadata should not be used to store application state or any other information which is not related to the content of the Photo.  Each Photo will have a set of `PhotoIdentifier` which allow the Photo to be linked to a person record within another system.  ### The `PhotoIdentifier` Entity  The `PhotoIdentifier` entity holds the `value` and `scheme` of a given identifier. The `value` field of a `PhotoIdentifier` is a simple ID string - e.g. `wgd23` or `000001`. The `scheme` field of a `PhotoIdentifier` indicates what system this identifier relates to or was issued by. This allows many identifiers which relate to different systems to be recorded against a single `Photo`.  The supported schemes are: * `v1.person.identifiers.cam.ac.uk`: The CRSID of the person represented by this Photo * `person.v1.student-records.university.identifiers.cam.ac.uk`: The CamSIS identifier (USN) of the person represented by this Photo * `person.v1.human-resources.university.identifiers.cam.ac.uk`: The CHRIS identifier (staff number) of the person represented by this Photo * `photo.v1.legacy-card.university.identifiers.cam.ac.uk`: The id of this Photo within the legacy card system  ## Using the API  ### Auth  To authenticate against the Photo API, an application must be registered within the API Gateway and granted access to the `University Photo` product. Details of how to register an application and grant access to products can be found in the [API Gateway Getting Started Guide](https://developer.api.apps.cam.ac.uk/start-using-an-api).    # noqa: E501
+    This API exposes identity information about university students. The purpose of this API is to give access to basic identity information about university students for use by downstream systems, therefore the data exposed is limited to basic information about who a student is and which institutions they are affiliated with.  This API uses the following identifiers to link people to person-records held within different systems:  * `person.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) identifier of this person -   also referred to as USN  Additionally this API uses the following identifiers to link people to institutions or entities which a person may have an affiliation to:  * `institution.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) institution identifier.     This encompasses colleges, departments and faculties. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under A01 and M01). * `academic-plan.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) academic plan     identifier. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under D07).  Both affiliations provide a `status` field which indicate a student's status within an affiliated entity. This `status` field is the short representation of the academic career field held in CamSIS. The [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual) lists the available values for the `status` field (under D05).  This API is currently backed by data from CamSIS, exposing a view of data that is refreshed nightly.    # noqa: E501
 
-    The version of the OpenAPI document: v1beta1
-    Contact: devops+photoapi@uis.cam.ac.uk
+    The version of the OpenAPI document: v1alpha2
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/action_enum.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/action_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'SET_RETENTION': "set_retention",
+            'REPAIR': "repair",
             'RESTORE': "restore",
             'SOFT_DELETE': "soft_delete",
             'HARD_DELETE': "hard_delete",
         },
     }
 
     validations = {
@@ -104,18 +104,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """ActionEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): * `set_retention` - Retention * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["set_retention", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
+            args[0] (str): * `repair` - Repair * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["repair", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
 
         Keyword Args:
-            value (str): * `set_retention` - Retention * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["set_retention", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
+            value (str): * `repair` - Repair * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["repair", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -198,18 +198,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """ActionEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): * `set_retention` - Retention * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["set_retention", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
+            args[0] (str): * `repair` - Repair * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["repair", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
 
         Keyword Args:
-            value (str): * `set_retention` - Retention * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["set_retention", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
+            value (str): * `repair` - Repair * `restore` - Restore * `soft_delete` - Soft Delete * `hard_delete` - Hard Delete., must be one of ["repair", "restore", "soft_delete", "hard_delete", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/api_versions.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/api_versions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/bad_request.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/bad_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/forbidden.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/forbidden.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/internal_server_error.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/internal_server_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/not_found.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/not_found.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/permissions.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/permissions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/photo_identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/scheme_enum.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/scheme_enum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/status_enum.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/status_enum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/transient_image_url.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/transient_image_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, expiration_seconds, url, *args, **kwargs):  # noqa: E501
         """TransientImageUrl - a model defined in OpenAPI
 
         Args:
             expiration_seconds (int): Get the number of seconds until this image link will expire.
-            url (str):
+            url (str): Get the image url.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/unauthorized.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/unauthorized.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/v1_beta1_photo.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/student.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """
-    University Photo API
+    University Student API
 
-     ## Introduction  The Photo API allows access to Photos of members of the University. The Photos exposed by this API are expected to be a good representation of the person they relate to.  The API broadly follows the principles of REST and strives to provide an interface that can be easily consumed by downstream systems.  ### Stability  This release of the Photo API is a `beta` offering: a service we are moving towards live but which requires wider testing with a broader group of users.  ### Versioning  The Photo API is versioned using URL path prefixes in the format: `/v1beta1/photos`. This follows the pattern established by the [GCP API](https://cloud.google.com/apis/design/versioning). Breaking changes will not be made without a change in API major version, however non-breaking changes will be introduced without changes to the version path prefix. All changes will be documented in the project's [CHANGELOG](https://gitlab.developers.cam.ac.uk/uis/devops/iam/photo-api/-/blob/master/CHANGELOG.md)  The available versions of the API are listed at the API's root.  ### Domain  The Photo API serves Photos of members of the University, linking a Photo to an individual through `PhotoIdentifiers` (see below) which pertain to a person record within an external system.  The Photos served by the Photo API are expected to be of sufficient quality to identify the person they represent. Photos which have been reviewed and determined to be sufficient quality are marked as having the status `approved` and exposed through the `approved-photos` endpoints.  ### Data source  The Photos exposed by the Photo API are currently a mirror of card Photos contained within the [Card Database](https://webservices.admin.cam.ac.uk/uc/). With Photos being synced from the Card Database to the Photo API hourly.  In future, the Photo API will be extended to allow Photos to be created and 'approved' using the API.  ## Core entities  ### The `Photo` Entity  The `Photo` entity contains information and metadata about a Photo of a member of the university. The `status` field on a Photo indicates whether this Photo has been reviewed and approved. Only Photos which have the status `approved` are exposed through the `approved-photos` endpoints. Each photo entity has a unique identifier - termed UUID - which is used in the system to refer to the specific photo entity. The UUID is provided in JSON documents as the `id` property.   Each Photo entity contains a link to the image data itself and a thumbnail for this Photo, which is guaranteed to be less than 128x128 pixels. Images are served by redirecting to a temporary URL provided by the service used to host images. These temporary URLs will expire after an hour and should not be retained for long-lasting access to a given Photo.  Each Photo may contain a block of JSON metadata recording information about the Photo. Photos cannot be updated once created (apart from to move their status to `approved`) hence this metadata should not be used to store application state or any other information which is not related to the content of the Photo.  Each Photo will have a set of `PhotoIdentifier` which allow the Photo to be linked to a person record within another system.  ### The `PhotoIdentifier` Entity  The `PhotoIdentifier` entity holds the `value` and `scheme` of a given identifier. The `value` field of a `PhotoIdentifier` is a simple ID string - e.g. `wgd23` or `000001`. The `scheme` field of a `PhotoIdentifier` indicates what system this identifier relates to or was issued by. This allows many identifiers which relate to different systems to be recorded against a single `Photo`.  The supported schemes are: * `v1.person.identifiers.cam.ac.uk`: The CRSID of the person represented by this Photo * `person.v1.student-records.university.identifiers.cam.ac.uk`: The CamSIS identifier (USN) of the person represented by this Photo * `person.v1.human-resources.university.identifiers.cam.ac.uk`: The CHRIS identifier (staff number) of the person represented by this Photo * `photo.v1.legacy-card.university.identifiers.cam.ac.uk`: The id of this Photo within the legacy card system  ## Using the API  ### Auth  To authenticate against the Photo API, an application must be registered within the API Gateway and granted access to the `University Photo` product. Details of how to register an application and grant access to products can be found in the [API Gateway Getting Started Guide](https://developer.api.apps.cam.ac.uk/start-using-an-api).    # noqa: E501
+    This API exposes identity information about university students. The purpose of this API is to give access to basic identity information about university students for use by downstream systems, therefore the data exposed is limited to basic information about who a student is and which institutions they are affiliated with.  This API uses the following identifiers to link people to person-records held within different systems:  * `person.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) identifier of this person -   also referred to as USN  Additionally this API uses the following identifiers to link people to institutions or entities which a person may have an affiliation to:  * `institution.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) institution identifier.     This encompasses colleges, departments and faculties. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under A01 and M01). * `academic-plan.v1.student-records.university.identifiers.cam.ac.uk` - the university student (ust) academic plan     identifier. The     [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual)     lists the available values for this affiliation (under D07).  Both affiliations provide a `status` field which indicate a student's status within an affiliated entity. This `status` field is the short representation of the academic career field held in CamSIS. The [CamSIS Coding Manual](https://www.camsis.cam.ac.uk/technical/camsis-coding-manual) lists the available values for the `status` field (under D05).  This API is currently backed by data from CamSIS, exposing a view of data that is refreshed nightly.    # noqa: E501
 
-    The version of the OpenAPI document: v1beta1
-    Contact: devops+photoapi@uis.cam.ac.uk
+    The version of the OpenAPI document: v1alpha2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from identitylib.photo_client.model_utils import (  # noqa: F401
+from identitylib.student_client.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from identitylib.photo_client.exceptions import ApiAttributeError
+from identitylib.student_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from identitylib.photo_client.model.scheme_enum import SchemeEnum
-    globals()['SchemeEnum'] = SchemeEnum
+    from identitylib.student_client.model.affiliation import Affiliation
+    from identitylib.student_client.model.identifier import Identifier
+    globals()['Affiliation'] = Affiliation
+    globals()['Identifier'] = Identifier
 
 
-class V1Beta1PhotoIdentifierSummaryRequest(ModelNormal):
+class Student(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,17 +60,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('value',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -87,41 +85,52 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'scheme': (SchemeEnum,),  # noqa: E501
-            'value': (str,),  # noqa: E501
+            'affiliations': ([Affiliation],),  # noqa: E501
+            'forenames': (str,),  # noqa: E501
+            'identifiers': ([Identifier],),  # noqa: E501
+            'name_prefixes': (str,),  # noqa: E501
+            'surname': (str,),  # noqa: E501
+            'date_of_birth': (date,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'scheme': 'scheme',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'affiliations': 'affiliations',  # noqa: E501
+        'forenames': 'forenames',  # noqa: E501
+        'identifiers': 'identifiers',  # noqa: E501
+        'name_prefixes': 'namePrefixes',  # noqa: E501
+        'surname': 'surname',  # noqa: E501
+        'date_of_birth': 'dateOfBirth',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, scheme, value, *args, **kwargs):  # noqa: E501
-        """V1Beta1PhotoIdentifierSummaryRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, affiliations, forenames, identifiers, name_prefixes, surname, *args, **kwargs):  # noqa: E501
+        """Student - a model defined in OpenAPI
 
         Args:
-            scheme (SchemeEnum):
-            value (str): The identifier's value
+            affiliations ([Affiliation]): The list of entities that this student is affiliated with. Currently this includes college and department affiliations (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`) and any active academic plan (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`).
+            forenames (str): The forenames of this student, split by a single space.
+            identifiers ([Identifier]): The identifiers attached to this student record. Currently only identifiers of the scheme person.v1.student-records.university.identifiers.cam.ac.uk (USN) are included, but additional identifier types may be added in future.
+            name_prefixes (str): The name prefixes of this student, split by a single space.
+            surname (str): The surname of this student.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,14 +155,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            date_of_birth (date): The date of birth of this student. There are a minority of cases where this is not known.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,16 +187,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.scheme = scheme
-        self.value = value
+        self.affiliations = affiliations
+        self.forenames = forenames
+        self.identifiers = identifiers
+        self.name_prefixes = name_prefixes
+        self.surname = surname
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -199,20 +212,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, scheme, value, *args, **kwargs):  # noqa: E501
-        """V1Beta1PhotoIdentifierSummaryRequest - a model defined in OpenAPI
+    def __init__(self, affiliations, forenames, identifiers, name_prefixes, surname, *args, **kwargs):  # noqa: E501
+        """Student - a model defined in OpenAPI
 
         Args:
-            scheme (SchemeEnum):
-            value (str): The identifier's value
+            affiliations ([Affiliation]): The list of entities that this student is affiliated with. Currently this includes college and department affiliations (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`) and any active academic plan (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`).
+            forenames (str): The forenames of this student, split by a single space.
+            identifiers ([Identifier]): The identifiers attached to this student record. Currently only identifiers of the scheme person.v1.student-records.university.identifiers.cam.ac.uk (USN) are included, but additional identifier types may be added in future.
+            name_prefixes (str): The name prefixes of this student, split by a single space.
+            surname (str): The surname of this student.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -237,14 +253,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            date_of_birth (date): The date of birth of this student. There are a minority of cases where this is not known.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -266,16 +283,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.scheme = scheme
-        self.value = value
+        self.affiliations = affiliations
+        self.forenames = forenames
+        self.identifiers = identifiers
+        self.name_prefixes = name_prefixes
+        self.surname = surname
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/model_utils.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/models/__init__.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,7 @@
 from identitylib.photo_client.model.photo_identifier_bulk_update_update_request import PhotoIdentifierBulkUpdateUpdateRequest
 from identitylib.photo_client.model.scheme_enum import SchemeEnum
 from identitylib.photo_client.model.status_enum import StatusEnum
 from identitylib.photo_client.model.transient_image_url import TransientImageUrl
 from identitylib.photo_client.model.unauthorized import Unauthorized
 from identitylib.photo_client.model.v1_beta1_photo import V1Beta1Photo
 from identitylib.photo_client.model.v1_beta1_photo_identifier_summary import V1Beta1PhotoIdentifierSummary
-from identitylib.photo_client.model.v1_beta1_photo_identifier_summary_request import V1Beta1PhotoIdentifierSummaryRequest
```

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client/rest.py` & `ucam-identitylib-2.0.0/identitylib/photo_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/photo_client_configuration.py` & `ucam-identitylib-2.0.0/identitylib/photo_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/__init__.py` & `ucam-identitylib-2.0.0/identitylib/student_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/configuration.py` & `ucam-identitylib-2.0.0/identitylib/student_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/affiliation.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation_scheme.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/affiliation_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/http_exception.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/http_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/http_validation_error.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/identifier.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/identifier_scheme.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/identifier_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/location_inner.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/location_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/paginated_results_student.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/paginated_results_student.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model/student.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model/validation_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,21 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from identitylib.student_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from identitylib.student_client.model.affiliation import Affiliation
-    from identitylib.student_client.model.identifier import Identifier
-    globals()['Affiliation'] = Affiliation
-    globals()['Identifier'] = Identifier
+    from identitylib.student_client.model.location_inner import LocationInner
+    globals()['LocationInner'] = LocationInner
 
 
-class Student(ModelNormal):
+class ValidationError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,52 +83,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'affiliations': ([Affiliation],),  # noqa: E501
-            'forenames': (str,),  # noqa: E501
-            'identifiers': ([Identifier],),  # noqa: E501
-            'name_prefixes': (str,),  # noqa: E501
-            'surname': (str,),  # noqa: E501
-            'date_of_birth': (date,),  # noqa: E501
+            'loc': ([LocationInner],),  # noqa: E501
+            'msg': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'affiliations': 'affiliations',  # noqa: E501
-        'forenames': 'forenames',  # noqa: E501
-        'identifiers': 'identifiers',  # noqa: E501
-        'name_prefixes': 'namePrefixes',  # noqa: E501
-        'surname': 'surname',  # noqa: E501
-        'date_of_birth': 'dateOfBirth',  # noqa: E501
+        'loc': 'loc',  # noqa: E501
+        'msg': 'msg',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, affiliations, forenames, identifiers, name_prefixes, surname, *args, **kwargs):  # noqa: E501
-        """Student - a model defined in OpenAPI
+    def _from_openapi_data(cls, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
 
         Args:
-            affiliations ([Affiliation]): The list of entities that this student is affiliated with. Currently this includes college and department affiliations (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`) and any active academic plan (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`).
-            forenames (str): The forenames of this student, split by a single space.
-            identifiers ([Identifier]): The identifiers attached to this student record. Currently only identifiers of the scheme person.v1.student-records.university.identifiers.cam.ac.uk (USN) are included, but additional identifier types may be added in future.
-            name_prefixes (str): The name prefixes of this student, split by a single space.
-            surname (str): The surname of this student.
+            loc ([LocationInner]):
+            msg (str):
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -155,15 +145,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            date_of_birth (date): The date of birth of this student. There are a minority of cases where this is not known.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,19 +176,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.affiliations = affiliations
-        self.forenames = forenames
-        self.identifiers = identifiers
-        self.name_prefixes = name_prefixes
-        self.surname = surname
+        self.loc = loc
+        self.msg = msg
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -212,23 +199,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, affiliations, forenames, identifiers, name_prefixes, surname, *args, **kwargs):  # noqa: E501
-        """Student - a model defined in OpenAPI
+    def __init__(self, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
 
         Args:
-            affiliations ([Affiliation]): The list of entities that this student is affiliated with. Currently this includes college and department affiliations (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`) and any active academic plan (under the scheme `institution.v1.student-records.university.identifiers.cam.ac.uk`).
-            forenames (str): The forenames of this student, split by a single space.
-            identifiers ([Identifier]): The identifiers attached to this student record. Currently only identifiers of the scheme person.v1.student-records.university.identifiers.cam.ac.uk (USN) are included, but additional identifier types may be added in future.
-            name_prefixes (str): The name prefixes of this student, split by a single space.
-            surname (str): The surname of this student.
+            loc ([LocationInner]):
+            msg (str):
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,15 +238,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            date_of_birth (date): The date of birth of this student. There are a minority of cases where this is not known.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -283,19 +267,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.affiliations = affiliations
-        self.forenames = forenames
-        self.identifiers = identifiers
-        self.name_prefixes = name_prefixes
-        self.surname = surname
+        self.loc = loc
+        self.msg = msg
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/model_utils.py` & `ucam-identitylib-2.0.0/identitylib/student_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/models/__init__.py` & `ucam-identitylib-2.0.0/identitylib/student_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/student_client/rest.py` & `ucam-identitylib-2.0.0/identitylib/student_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/university_hr_configuration.py` & `ucam-identitylib-2.0.0/identitylib/university_hr_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/identitylib/university_student_configuration.py` & `ucam-identitylib-2.0.0/identitylib/university_student_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/setup.py` & `ucam-identitylib-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 PACKAGE_NAME = "ucam-identitylib"
 PACKAGE_DESCRIPTION = (
     "A module containing helpers and shared code related to identity systems within UIS, "
     "University of Cambridge."
 )
-PACKAGE_VERSION = "1.6.0"
+PACKAGE_VERSION = "2.0.0"
 PACKAGE_URL = "https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib"
 
 
 def load_requirements(file: str):
     """
     Load requirements file and return non-empty, non-comment lines with leading and trailing
     whitespace stripped.
```

### Comparing `ucam-identitylib-1.6.0/tests/test_api_client_mixin.py` & `ucam-identitylib-2.0.0/tests/test_api_client_mixin.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.6.0/tests/test_identifiers.py` & `ucam-identitylib-2.0.0/tests/test_identifiers.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,20 @@
         self.assertEqual(
             Identifier.from_string(
                 "abc123@person.v1.student-records.university.identifiers.cam.ac.uk"
             ),
             Identifier("abc123", IdentifierSchemes.USN),
         )
 
+        # parsing CRSid cast to lower case
+        self.assertEqual(
+            Identifier.from_string("ABC123@v1.person.identifiers.cam.ac.uk"),
+            Identifier("abc123", IdentifierSchemes.CRSID),
+        )
+
         # fallback scheme given - actual scheme in identifier is used
         self.assertEqual(
             Identifier.from_string(
                 "xxx@v1.person.identifiers.cam.ac.uk",
                 fallback_scheme=IdentifierSchemes.USN,
             ),
             Identifier("xxx", IdentifierSchemes.CRSID),
```

### Comparing `ucam-identitylib-1.6.0/ucam_identitylib.egg-info/PKG-INFO` & `ucam-identitylib-2.0.0/ucam_identitylib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-identitylib
-Version: 1.6.0
+Version: 2.0.0
 Summary: A module containing helpers and shared code related to identity systems within UIS, University of Cambridge.
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib
 Author: University of Cambridge Information Services
 Author-email: devops+ucam-identitylib@uis.cam.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ucam-identitylib-1.6.0/ucam_identitylib.egg-info/SOURCES.txt` & `ucam-identitylib-2.0.0/ucam_identitylib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 identitylib/card_client/model/available_barcode.py
 identitylib/card_client/model/available_barcode_batch_request_type.py
 identitylib/card_client/model/available_barcode_batch_response_type.py
 identitylib/card_client/model/available_barcode_batch_response_type_details.py
 identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py
 identitylib/card_client/model/available_barcode_create_request_type.py
 identitylib/card_client/model/card.py
+identitylib/card_client/model/card_bulk_update_request_type.py
+identitylib/card_client/model/card_bulk_update_request_type_updates_inner.py
+identitylib/card_client/model/card_bulk_update_response_type.py
 identitylib/card_client/model/card_filter_request_type.py
 identitylib/card_client/model/card_filter_response_type.py
 identitylib/card_client/model/card_identifier.py
 identitylib/card_client/model/card_identifier_bulk_update_request_type.py
 identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
 identitylib/card_client/model/card_identifier_bulk_update_response_type.py
 identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
@@ -167,23 +170,17 @@
 identitylib/photo_client/__init__.py
 identitylib/photo_client/api_client.py
 identitylib/photo_client/configuration.py
 identitylib/photo_client/exceptions.py
 identitylib/photo_client/model_utils.py
 identitylib/photo_client/rest.py
 identitylib/photo_client/api/__init__.py
-identitylib/photo_client/api/all_photos_api.py
 identitylib/photo_client/api/api_versions_api.py
-identitylib/photo_client/api/approved_photos_api.py
 identitylib/photo_client/api/permissions_api.py
-identitylib/photo_client/api/photo_identifier_api.py
-identitylib/photo_client/api/photo_identifiers_api.py
-identitylib/photo_client/api/photo_identifiers_including_photos_api.py
-identitylib/photo_client/api/photos_including_unapproved_photos_api.py
-identitylib/photo_client/api/unapproved_photos_api.py
+identitylib/photo_client/api/v1beta1_api.py
 identitylib/photo_client/apis/__init__.py
 identitylib/photo_client/model/__init__.py
 identitylib/photo_client/model/action_enum.py
 identitylib/photo_client/model/api_versions.py
 identitylib/photo_client/model/bad_request.py
 identitylib/photo_client/model/forbidden.py
 identitylib/photo_client/model/internal_server_error.py
@@ -196,15 +193,14 @@
 identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py
 identitylib/photo_client/model/scheme_enum.py
 identitylib/photo_client/model/status_enum.py
 identitylib/photo_client/model/transient_image_url.py
 identitylib/photo_client/model/unauthorized.py
 identitylib/photo_client/model/v1_beta1_photo.py
 identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
-identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py
 identitylib/photo_client/models/__init__.py
 identitylib/student_client/__init__.py
 identitylib/student_client/api_client.py
 identitylib/student_client/configuration.py
 identitylib/student_client/exceptions.py
 identitylib/student_client/model_utils.py
 identitylib/student_client/rest.py
```

