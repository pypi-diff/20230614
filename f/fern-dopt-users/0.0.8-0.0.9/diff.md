# Comparing `tmp/fern_dopt_users-0.0.8.tar.gz` & `tmp/fern_dopt_users-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_dopt_users-0.0.8.tar", max compression
+gzip compressed data, was "fern_dopt_users-0.0.9.tar", max compression
```

## Comparing `fern_dopt_users-0.0.8.tar` & `fern_dopt_users-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        0 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/README.md
--rw-r--r--   0        0        0      374 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1594 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/__init__.py
--rw-r--r--   0        0        0    15183 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/client.py
--rw-r--r--   0        0        0      348 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/environment.py
--rw-r--r--   0        0        0      292 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/errors/bad_request_error.py
--rw-r--r--   0        0        0      346 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/errors/internal_server_error.py
--rw-r--r--   0        0        0      337 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/py.typed
--rw-r--r--   0        0        0     2090 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/__init__.py
--rw-r--r--   0        0        0      888 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/bad_request_error_response_body.py
--rw-r--r--   0        0        0      676 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/bad_request_error_response_body_code.py
--rw-r--r--   0        0        0      225 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_batch_request_body.py
--rw-r--r--   0        0        0     1080 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_batch_request_body_item.py
--rw-r--r--   0        0        0      912 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_batch_request_body_item_groups_item.py
--rw-r--r--   0        0        0      762 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_batch_response_body.py
--rw-r--r--   0        0        0      131 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_request_body.py
--rw-r--r--   0        0        0      761 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_request_params.py
--rw-r--r--   0        0        0      372 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_segment_request_body.py
--rw-r--r--   0        0        0     1203 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py
--rw-r--r--   0        0        0      764 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_segment_response_body.py
--rw-r--r--   0        0        0      907 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/identify_user_request_body_groups_item.py
--rw-r--r--   0        0        0      854 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/internal_server_error_response_body.py
--rw-r--r--   0        0        0      842 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/not_found_error_response_body.py
--rw-r--r--   0        0        0      956 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/segment_common.py
--rw-r--r--   0        0        0     1163 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/segment_group.py
--rw-r--r--   0        0        0     1031 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/segment_identify.py
--rw-r--r--   0        0        0      847 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/timeout_error_response_body.py
--rw-r--r--   0        0        0      849 2023-06-13 17:16:21.580427 fern_dopt_users-0.0.8/src/dopt/types/unauthorized_error_response_body.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 fern_dopt_users-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1883 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/README.md
+-rw-r--r--   0        0        0      374 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1594 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/__init__.py
+-rw-r--r--   0        0        0    15183 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/client.py
+-rw-r--r--   0        0        0      348 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/environment.py
+-rw-r--r--   0        0        0      292 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/errors/bad_request_error.py
+-rw-r--r--   0        0        0      346 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/errors/internal_server_error.py
+-rw-r--r--   0        0        0      337 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/py.typed
+-rw-r--r--   0        0        0     2090 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/bad_request_error_response_body.py
+-rw-r--r--   0        0        0      676 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/bad_request_error_response_body_code.py
+-rw-r--r--   0        0        0      225 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_batch_request_body.py
+-rw-r--r--   0        0        0     1080 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_batch_request_body_item.py
+-rw-r--r--   0        0        0      912 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_batch_request_body_item_groups_item.py
+-rw-r--r--   0        0        0      762 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_batch_response_body.py
+-rw-r--r--   0        0        0      131 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_request_body.py
+-rw-r--r--   0        0        0      761 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_request_params.py
+-rw-r--r--   0        0        0      372 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_segment_request_body.py
+-rw-r--r--   0        0        0     1203 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py
+-rw-r--r--   0        0        0      764 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_segment_response_body.py
+-rw-r--r--   0        0        0      907 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/identify_user_request_body_groups_item.py
+-rw-r--r--   0        0        0      854 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/internal_server_error_response_body.py
+-rw-r--r--   0        0        0      842 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/not_found_error_response_body.py
+-rw-r--r--   0        0        0      956 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/segment_common.py
+-rw-r--r--   0        0        0     1163 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/segment_group.py
+-rw-r--r--   0        0        0     1031 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/segment_identify.py
+-rw-r--r--   0        0        0      847 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/timeout_error_response_body.py
+-rw-r--r--   0        0        0      849 2023-06-14 16:38:19.144302 fern_dopt_users-0.0.9/src/dopt/types/unauthorized_error_response_body.py
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 fern_dopt_users-0.0.9/PKG-INFO
```

### Comparing `fern_dopt_users-0.0.8/src/dopt/__init__.py` & `fern_dopt_users-0.0.9/src/dopt/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/client.py` & `fern_dopt_users-0.0.9/src/dopt/client.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/core/datetime_utils.py` & `fern_dopt_users-0.0.9/src/dopt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/core/jsonable_encoder.py` & `fern_dopt_users-0.0.9/src/dopt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/__init__.py` & `fern_dopt_users-0.0.9/src/dopt/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/bad_request_error_response_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/bad_request_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/bad_request_error_response_body_code.py` & `fern_dopt_users-0.0.9/src/dopt/types/bad_request_error_response_body_code.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/identify_batch_request_body_item.py` & `fern_dopt_users-0.0.9/src/dopt/types/identify_batch_request_body_item.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/identify_batch_request_body_item_groups_item.py` & `fern_dopt_users-0.0.9/src/dopt/types/identify_batch_request_body_item_groups_item.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/identify_batch_response_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/identify_batch_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/identify_request_params.py` & `fern_dopt_users-0.0.9/src/dopt/types/identify_request_params.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/identify_segment_request_body_identify_segment_request_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/identify_segment_response_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/identify_segment_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/identify_user_request_body_groups_item.py` & `fern_dopt_users-0.0.9/src/dopt/types/identify_user_request_body_groups_item.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/internal_server_error_response_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/internal_server_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/not_found_error_response_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/not_found_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/segment_common.py` & `fern_dopt_users-0.0.9/src/dopt/types/segment_common.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/segment_group.py` & `fern_dopt_users-0.0.9/src/dopt/types/segment_group.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/segment_identify.py` & `fern_dopt_users-0.0.9/src/dopt/types/segment_identify.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/timeout_error_response_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/timeout_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_users-0.0.8/src/dopt/types/unauthorized_error_response_body.py` & `fern_dopt_users-0.0.9/src/dopt/types/unauthorized_error_response_body.py`

 * *Files identical despite different names*

