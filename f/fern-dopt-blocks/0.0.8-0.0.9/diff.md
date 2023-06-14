# Comparing `tmp/fern_dopt_blocks-0.0.8.tar.gz` & `tmp/fern_dopt_blocks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_dopt_blocks-0.0.8.tar", max compression
+gzip compressed data, was "fern_dopt_blocks-0.0.9.tar", max compression
```

## Comparing `fern_dopt_blocks-0.0.8.tar` & `fern_dopt_blocks-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1994 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/README.md
--rw-r--r--   0        0        0      375 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2350 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/__init__.py
--rw-r--r--   0        0        0    14068 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/client.py
--rw-r--r--   0        0        0      348 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      158 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/environment.py
--rw-r--r--   0        0        0      352 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/py.typed
--rw-r--r--   0        0        0     3248 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/__init__.py
--rw-r--r--   0        0        0      888 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/bad_request_error_response_body.py
--rw-r--r--   0        0        0      676 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/bad_request_error_response_body_code.py
--rw-r--r--   0        0        0      996 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/block_transition_query_string.py
--rw-r--r--   0        0        0      761 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/block_transition_request_params.py
--rw-r--r--   0        0        0     1342 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response.py
--rw-r--r--   0        0        0      459 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response_fields_item.py
--rw-r--r--   0        0        0      894 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response_fields_item_find_blocks_response_fields_item.py
--rw-r--r--   0        0        0      795 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response_state.py
--rw-r--r--   0        0        0     1162 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response_type.py
--rw-r--r--   0        0        0      957 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_query_string.py
--rw-r--r--   0        0        0      800 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_request_intent.py
--rw-r--r--   0        0        0      875 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_request_params.py
--rw-r--r--   0        0        0      830 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_request_params_intent.py
--rw-r--r--   0        0        0      870 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/get_block_query_string.py
--rw-r--r--   0        0        0      754 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/get_block_request_params.py
--rw-r--r--   0        0        0     1044 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_query_string.py
--rw-r--r--   0        0        0      753 2023-06-13 17:15:48.073024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_request_params.py
--rw-r--r--   0        0        0     1120 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response.py
--rw-r--r--   0        0        0     1418 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item.py
--rw-r--r--   0        0        0      540 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_fields_item.py
--rw-r--r--   0        0        0      908 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py
--rw-r--r--   0        0        0      802 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_state.py
--rw-r--r--   0        0        0     1211 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_type.py
--rw-r--r--   0        0        0      795 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_state.py
--rw-r--r--   0        0        0      780 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/health_check_response_body.py
--rw-r--r--   0        0        0      854 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/internal_server_error_response_body.py
--rw-r--r--   0        0        0      842 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/not_found_error_response_body.py
--rw-r--r--   0        0        0      847 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/timeout_error_response_body.py
--rw-r--r--   0        0        0      849 2023-06-13 17:15:48.077024 fern_dopt_blocks-0.0.8/src/dopt/types/unauthorized_error_response_body.py
--rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 fern_dopt_blocks-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1994 2023-06-14 16:38:07.956145 fern_dopt_blocks-0.0.9/README.md
+-rw-r--r--   0        0        0      375 2023-06-14 16:38:07.956145 fern_dopt_blocks-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2350 2023-06-14 16:38:07.956145 fern_dopt_blocks-0.0.9/src/dopt/__init__.py
+-rw-r--r--   0        0        0    14068 2023-06-14 16:38:07.956145 fern_dopt_blocks-0.0.9/src/dopt/client.py
+-rw-r--r--   0        0        0      348 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      158 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/environment.py
+-rw-r--r--   0        0        0      352 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/py.typed
+-rw-r--r--   0        0        0     3248 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/types/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/types/bad_request_error_response_body.py
+-rw-r--r--   0        0        0      676 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/types/bad_request_error_response_body_code.py
+-rw-r--r--   0        0        0      996 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/types/block_transition_query_string.py
+-rw-r--r--   0        0        0      761 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/types/block_transition_request_params.py
+-rw-r--r--   0        0        0     1342 2023-06-14 16:38:07.960145 fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response.py
+-rw-r--r--   0        0        0      459 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response_fields_item.py
+-rw-r--r--   0        0        0      894 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response_fields_item_find_blocks_response_fields_item.py
+-rw-r--r--   0        0        0      795 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response_state.py
+-rw-r--r--   0        0        0     1162 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response_type.py
+-rw-r--r--   0        0        0      957 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_query_string.py
+-rw-r--r--   0        0        0      800 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_request_intent.py
+-rw-r--r--   0        0        0      875 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_request_params.py
+-rw-r--r--   0        0        0      830 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_request_params_intent.py
+-rw-r--r--   0        0        0      870 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_block_query_string.py
+-rw-r--r--   0        0        0      754 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_block_request_params.py
+-rw-r--r--   0        0        0     1044 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_query_string.py
+-rw-r--r--   0        0        0      753 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_request_params.py
+-rw-r--r--   0        0        0     1120 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response.py
+-rw-r--r--   0        0        0     1418 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item.py
+-rw-r--r--   0        0        0      540 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_fields_item.py
+-rw-r--r--   0        0        0      908 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py
+-rw-r--r--   0        0        0      802 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_state.py
+-rw-r--r--   0        0        0     1211 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_type.py
+-rw-r--r--   0        0        0      795 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_state.py
+-rw-r--r--   0        0        0      780 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/health_check_response_body.py
+-rw-r--r--   0        0        0      854 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/internal_server_error_response_body.py
+-rw-r--r--   0        0        0      842 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/not_found_error_response_body.py
+-rw-r--r--   0        0        0      847 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/timeout_error_response_body.py
+-rw-r--r--   0        0        0      849 2023-06-14 16:38:07.964145 fern_dopt_blocks-0.0.9/src/dopt/types/unauthorized_error_response_body.py
+-rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 fern_dopt_blocks-0.0.9/PKG-INFO
```

### Comparing `fern_dopt_blocks-0.0.8/README.md` & `fern_dopt_blocks-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/__init__.py` & `fern_dopt_blocks-0.0.9/src/dopt/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/client.py` & `fern_dopt_blocks-0.0.9/src/dopt/client.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/core/datetime_utils.py` & `fern_dopt_blocks-0.0.9/src/dopt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/core/jsonable_encoder.py` & `fern_dopt_blocks-0.0.9/src/dopt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/__init__.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/bad_request_error_response_body.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/bad_request_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/bad_request_error_response_body_code.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/bad_request_error_response_body_code.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/block_transition_query_string.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/block_transition_query_string.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/block_transition_request_params.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/block_transition_request_params.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response_fields_item_find_blocks_response_fields_item.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response_fields_item_find_blocks_response_fields_item.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response_state.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response_state.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/find_blocks_response_type.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/find_blocks_response_type.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_query_string.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_query_string.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_request_intent.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_request_intent.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_request_params.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_request_params.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/flow_intent_request_params_intent.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/flow_intent_request_params_intent.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_block_query_string.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_block_query_string.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_block_request_params.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_block_request_params.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_query_string.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_query_string.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_request_params.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_request_params.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_fields_item.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_fields_item.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_state.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_state.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_blocks_item_type.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_blocks_item_type.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/get_flow_response_state.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/get_flow_response_state.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/health_check_response_body.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/health_check_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/internal_server_error_response_body.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/internal_server_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/not_found_error_response_body.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/not_found_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/timeout_error_response_body.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/timeout_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/src/dopt/types/unauthorized_error_response_body.py` & `fern_dopt_blocks-0.0.9/src/dopt/types/unauthorized_error_response_body.py`

 * *Files identical despite different names*

### Comparing `fern_dopt_blocks-0.0.8/PKG-INFO` & `fern_dopt_blocks-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-dopt-blocks
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

