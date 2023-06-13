# Comparing `tmp/cirro-0.7.1.tar.gz` & `tmp/cirro-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro-0.7.1.tar", max compression
+gzip compressed data, was "cirro-0.7.2.tar", max compression
```

## Comparing `cirro-0.7.1.tar` & `cirro-0.7.2.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0     1086 2023-06-13 01:03:48.340354 cirro-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     5024 2023-06-13 01:03:48.340354 cirro-0.7.1/README.md
--rw-r--r--   0        0        0       65 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/__init__.py
--rw-r--r--   0        0        0       92 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/__init__.py
--rw-r--r--   0        0        0     1908 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/__init__.py
--rw-r--r--   0        0        0      576 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/base.py
--rw-r--r--   0        0        0     1653 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/iam.py
--rw-r--r--   0        0        0     6663 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/oauth_client.py
--rw-r--r--   0        0        0     1856 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/username.py
--rw-r--r--   0        0        0      133 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/__init__.py
--rw-r--r--   0        0        0     1460 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/api.py
--rw-r--r--   0        0        0     1559 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/portal.py
--rw-r--r--   0        0        0     4045 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/s3.py
--rw-r--r--   0        0        0      199 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/utils.py
--rw-r--r--   0        0        0     3544 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/config.py
--rw-r--r--   0        0        0        0 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/__init__.py
--rw-r--r--   0        0        0      101 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/api.py
--rw-r--r--   0        0        0      566 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/auth.py
--rw-r--r--   0        0        0     1763 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/dataset.py
--rw-r--r--   0        0        0      120 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/exceptions.py
--rw-r--r--   0        0        0     4250 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/file.py
--rw-r--r--   0        0        0     2659 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/form_specification.py
--rw-r--r--   0        0        0     3013 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/process.py
--rw-r--r--   0        0        0      539 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/project.py
--rw-r--r--   0        0        0     1425 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/reference.py
--rw-r--r--   0        0        0      430 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/s3_path.py
--rw-r--r--   0        0        0      268 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/status.py
--rw-r--r--   0        0        0      777 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/workflow_models.py
--rw-r--r--   0        0        0      382 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/__init__.py
--rw-r--r--   0        0        0     1045 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/base.py
--rw-r--r--   0        0        0      690 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/common.py
--rw-r--r--   0        0        0     6405 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/dataset.py
--rw-r--r--   0        0        0     4189 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/file.py
--rw-r--r--   0        0        0     6532 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/process.py
--rw-r--r--   0        0        0     2527 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/project.py
--rw-r--r--   0        0        0      244 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/__init__.py
--rw-r--r--   0        0        0     2523 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/cli.py
--rw-r--r--   0        0        0     6754 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/controller.py
--rw-r--r--   0        0        0        0 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/__init__.py
--rw-r--r--   0        0        0      318 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/auth_args.py
--rw-r--r--   0        0        0      770 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/common_args.py
--rw-r--r--   0        0        0     4610 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/download_args.py
--rw-r--r--   0        0        0      573 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/list_dataset_args.py
--rw-r--r--   0        0        0     3507 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/upload_args.py
--rw-r--r--   0        0        0     2250 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/utils.py
--rw-r--r--   0        0        0    12069 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/workflow_args.py
--rw-r--r--   0        0        0     9132 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/workflow_form_args.py
--rw-r--r--   0        0        0      371 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/models.py
--rw-r--r--   0        0        0     3685 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/file_utils.py
--rw-r--r--   0        0        0      257 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/__init__.py
--rw-r--r--   0        0        0     1708 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/constants.py
--rw-r--r--   0        0        0     5202 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/form.py
--rw-r--r--   0        0        0     5901 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/preprocess_dataset.py
--rw-r--r--   0        0        0     9137 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/workflow_config.py
--rw-r--r--   0        0        0       73 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/__init__.py
--rw-r--r--   0        0        0     2901 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/asset.py
--rw-r--r--   0        0        0     3758 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/dataset.py
--rw-r--r--   0        0        0      245 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/exceptions.py
--rw-r--r--   0        0        0     4317 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/file.py
--rw-r--r--   0        0        0     1670 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/helpers.py
--rw-r--r--   0        0        0     2779 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/portal.py
--rw-r--r--   0        0        0     1552 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/process.py
--rw-r--r--   0        0        0     6418 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/project.py
--rw-r--r--   0        0        0      861 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/reference.py
--rw-r--r--   0        0        0      964 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/reference_type.py
--rw-r--r--   0        0        0     1215 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/utils.py
--rw-r--r--   0        0        0      887 2023-06-13 01:03:48.344354 cirro-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 cirro-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-13 22:07:07.004667 cirro-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     5024 2023-06-13 22:07:07.004667 cirro-0.7.2/README.md
+-rw-r--r--   0        0        0       65 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/__init__.py
+-rw-r--r--   0        0        0     1461 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/auth/__init__.py
+-rw-r--r--   0        0        0      576 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/auth/base.py
+-rw-r--r--   0        0        0     1653 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/auth/iam.py
+-rw-r--r--   0        0        0     6663 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/auth/oauth_client.py
+-rw-r--r--   0        0        0      133 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/clients/__init__.py
+-rw-r--r--   0        0        0     1460 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/clients/api.py
+-rw-r--r--   0        0        0     1559 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/clients/portal.py
+-rw-r--r--   0        0        0     4045 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/clients/s3.py
+-rw-r--r--   0        0        0      199 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/clients/utils.py
+-rw-r--r--   0        0        0     3544 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/api.py
+-rw-r--r--   0        0        0      566 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/auth.py
+-rw-r--r--   0        0        0     1763 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/dataset.py
+-rw-r--r--   0        0        0      120 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/exceptions.py
+-rw-r--r--   0        0        0     4250 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/file.py
+-rw-r--r--   0        0        0     2659 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/form_specification.py
+-rw-r--r--   0        0        0     3013 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/process.py
+-rw-r--r--   0        0        0      539 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/project.py
+-rw-r--r--   0        0        0     1425 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/reference.py
+-rw-r--r--   0        0        0      430 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/s3_path.py
+-rw-r--r--   0        0        0      268 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/status.py
+-rw-r--r--   0        0        0      777 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/models/workflow_models.py
+-rw-r--r--   0        0        0      382 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/services/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/services/base.py
+-rw-r--r--   0        0        0      690 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/services/common.py
+-rw-r--r--   0        0        0     6405 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/services/dataset.py
+-rw-r--r--   0        0        0     4189 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/services/file.py
+-rw-r--r--   0        0        0     6556 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/services/process.py
+-rw-r--r--   0        0        0     2551 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/api/services/project.py
+-rw-r--r--   0        0        0      244 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/__init__.py
+-rw-r--r--   0        0        0     2523 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/cli.py
+-rw-r--r--   0        0        0     6754 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/controller.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/auth_args.py
+-rw-r--r--   0        0        0      770 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/common_args.py
+-rw-r--r--   0        0        0     4610 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/download_args.py
+-rw-r--r--   0        0        0      573 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/list_dataset_args.py
+-rw-r--r--   0        0        0     3507 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/upload_args.py
+-rw-r--r--   0        0        0     2250 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/utils.py
+-rw-r--r--   0        0        0    12069 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/workflow_args.py
+-rw-r--r--   0        0        0     9132 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/interactive/workflow_form_args.py
+-rw-r--r--   0        0        0      371 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/cli/models.py
+-rw-r--r--   0        0        0     3685 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/file_utils.py
+-rw-r--r--   0        0        0      257 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/helpers/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/helpers/constants.py
+-rw-r--r--   0        0        0     5202 2023-06-13 22:07:07.004667 cirro-0.7.2/cirro/helpers/form.py
+-rw-r--r--   0        0        0     5901 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/helpers/preprocess_dataset.py
+-rw-r--r--   0        0        0     9137 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/helpers/workflow_config.py
+-rw-r--r--   0        0        0       73 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/__init__.py
+-rw-r--r--   0        0        0     2901 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/asset.py
+-rw-r--r--   0        0        0     3758 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/dataset.py
+-rw-r--r--   0        0        0      245 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/exceptions.py
+-rw-r--r--   0        0        0     4317 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/file.py
+-rw-r--r--   0        0        0     1670 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/helpers.py
+-rw-r--r--   0        0        0     2779 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/portal.py
+-rw-r--r--   0        0        0     1552 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/process.py
+-rw-r--r--   0        0        0     6418 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/project.py
+-rw-r--r--   0        0        0      861 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/reference.py
+-rw-r--r--   0        0        0      964 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/sdk/reference_type.py
+-rw-r--r--   0        0        0     1215 2023-06-13 22:07:07.008667 cirro-0.7.2/cirro/utils.py
+-rw-r--r--   0        0        0      860 2023-06-13 22:07:07.008667 cirro-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6221 1970-01-01 00:00:00.000000 cirro-0.7.2/PKG-INFO
```

### Comparing `cirro-0.7.1/LICENSE.txt` & `cirro-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/README.md` & `cirro-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/auth/__init__.py` & `cirro-0.7.2/cirro/api/auth/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from cirro.api.auth.base import AuthInfo
 from cirro.api.auth.iam import IAMAuth
 from cirro.api.auth.oauth_client import ClientAuth
-from cirro.api.auth.username import UsernameAndPasswordAuth
 
 __all__ = [
     'AuthInfo',
     'IAMAuth',
-    'UsernameAndPasswordAuth',
     'ClientAuth',
     'get_auth_info_from_config'
 ]
 
 from cirro.api.config import AppConfig
 
 
@@ -19,15 +17,14 @@
     if not user_config or not user_config.auth_method:
         return ClientAuth(region=app_config.region,
                           client_id=app_config.client_id,
                           auth_endpoint=app_config.auth_endpoint)
 
     auth_methods = [
         ClientAuth,
-        UsernameAndPasswordAuth,
         IAMAuth
     ]
     matched_auth_method = next((m for m in auth_methods if m.__name__ == user_config.auth_method), None)
     if not matched_auth_method:
         raise RuntimeError(f'{user_config.auth_method} not found, please re-run configuration')
 
     auth_config = user_config.auth_method_config
@@ -39,13 +36,7 @@
                           enable_cache=auth_config.get('enable_cache') == 'True')
 
     if matched_auth_method == IAMAuth and auth_config.get('load_current'):
         return IAMAuth.load_current()
 
     if matched_auth_method == IAMAuth:
         return IAMAuth(region=app_config.region, **auth_config)
-
-    if matched_auth_method == UsernameAndPasswordAuth:
-        return UsernameAndPasswordAuth(region=app_config.region,
-                                       client_id=app_config.client_id,
-                                       user_pool_id=app_config.user_pool_id,
-                                       **auth_config)
```

### Comparing `cirro-0.7.1/cirro/api/auth/base.py` & `cirro-0.7.2/cirro/api/auth/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/auth/iam.py` & `cirro-0.7.2/cirro/api/auth/iam.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/auth/oauth_client.py` & `cirro-0.7.2/cirro/api/auth/oauth_client.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/clients/api.py` & `cirro-0.7.2/cirro/api/clients/api.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/clients/portal.py` & `cirro-0.7.2/cirro/api/clients/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/clients/s3.py` & `cirro-0.7.2/cirro/api/clients/s3.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/config.py` & `cirro-0.7.2/cirro/api/config.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/auth.py` & `cirro-0.7.2/cirro/api/models/auth.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/dataset.py` & `cirro-0.7.2/cirro/api/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/file.py` & `cirro-0.7.2/cirro/api/models/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/form_specification.py` & `cirro-0.7.2/cirro/api/models/form_specification.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/process.py` & `cirro-0.7.2/cirro/api/models/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/project.py` & `cirro-0.7.2/cirro/api/models/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/reference.py` & `cirro-0.7.2/cirro/api/models/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/models/workflow_models.py` & `cirro-0.7.2/cirro/api/models/workflow_models.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/services/base.py` & `cirro-0.7.2/cirro/api/services/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/services/common.py` & `cirro-0.7.2/cirro/api/services/common.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/services/dataset.py` & `cirro-0.7.2/cirro/api/services/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/services/file.py` & `cirro-0.7.2/cirro/api/services/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/api/services/process.py` & `cirro-0.7.2/cirro/api/services/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                   fileNamePatterns {
                     exampleName
                     description
                     sampleMatchingPattern
                   }
                 }
               }
+              nextToken
             }
           }
         '''
         item_filter = {}
         if process_type:
             item_filter['executor'] = {'eq': process_type.value}
```

### Comparing `cirro-0.7.1/cirro/api/services/project.py` & `cirro-0.7.2/cirro/api/services/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             listProjects(filter: $filter, limit: $limit, nextToken: $nextToken) {
               items {
                 id
                 name
                 desc
                 status
               }
+              nextToken
             }
           }
         '''
 
         items = fetch_all_items(self._api_client, query, {})
         not_deleted = filter_deleted(items)
         return [Project.from_record(item) for item in not_deleted]
```

### Comparing `cirro-0.7.1/cirro/cli/cli.py` & `cirro-0.7.2/cirro/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/controller.py` & `cirro-0.7.2/cirro/cli/controller.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/interactive/common_args.py` & `cirro-0.7.2/cirro/cli/interactive/common_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/interactive/download_args.py` & `cirro-0.7.2/cirro/cli/interactive/download_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/interactive/list_dataset_args.py` & `cirro-0.7.2/cirro/cli/interactive/list_dataset_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/interactive/upload_args.py` & `cirro-0.7.2/cirro/cli/interactive/upload_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/interactive/utils.py` & `cirro-0.7.2/cirro/cli/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/interactive/workflow_args.py` & `cirro-0.7.2/cirro/cli/interactive/workflow_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/cli/interactive/workflow_form_args.py` & `cirro-0.7.2/cirro/cli/interactive/workflow_form_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/file_utils.py` & `cirro-0.7.2/cirro/file_utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/helpers/constants.py` & `cirro-0.7.2/cirro/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/helpers/form.py` & `cirro-0.7.2/cirro/helpers/form.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/helpers/preprocess_dataset.py` & `cirro-0.7.2/cirro/helpers/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/helpers/workflow_config.py` & `cirro-0.7.2/cirro/helpers/workflow_config.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/asset.py` & `cirro-0.7.2/cirro/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/dataset.py` & `cirro-0.7.2/cirro/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/file.py` & `cirro-0.7.2/cirro/sdk/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/helpers.py` & `cirro-0.7.2/cirro/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/portal.py` & `cirro-0.7.2/cirro/sdk/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/process.py` & `cirro-0.7.2/cirro/sdk/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/project.py` & `cirro-0.7.2/cirro/sdk/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/reference.py` & `cirro-0.7.2/cirro/sdk/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/sdk/reference_type.py` & `cirro-0.7.2/cirro/sdk/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/cirro/utils.py` & `cirro-0.7.2/cirro/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.1/pyproject.toml` & `cirro-0.7.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [tool.poetry]
 name = "cirro"
-version = "0.7.1"
+version = "0.7.2"
 description = "CLI tool and SDK for interacting with the Cirro platform"
-authors = ["Fred Hutch <cirro@fredhutch.org>"]
+authors = ["Cirro Bio <support@cirro.bio>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FredHutch/Cirro-client"
 packages = [{include = "cirro"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
-boto3 = "^1.24.0"
+boto3 = "1.26.76"
 questionary = "^1.10.0"
-requests = "^2.28.0"
-requests_aws4auth = "^1.1.2"
-pycognito = "2022.12.0"
+requests = "^2.31.0"
+requests_aws4auth = "^1.2.3"
 tqdm = "^4.62.3"
-pygithub = "1.58.0"
+pygithub = "1.58.2"
 jsonschema = "^4.6.1"
-gql = {extras = ["requests"], version = "^3.4.0"}
+gql = {extras = ["requests"], version = "^3.4.1"}
 pandas = "^1.5.0"
-s3fs = "2023.1.0"
-pyjwt = "^2.4.0"
+s3fs = "2023.6.0"
+pyjwt = "^2.7.0"
 msal-extensions = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "*"
 flake8 = "*"
```

### Comparing `cirro-0.7.1/PKG-INFO` & `cirro-0.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: cirro
-Version: 0.7.1
+Version: 0.7.2
 Summary: CLI tool and SDK for interacting with the Cirro platform
 Home-page: https://github.com/FredHutch/Cirro-client
 License: MIT
-Author: Fred Hutch
-Author-email: cirro@fredhutch.org
+Author: Cirro Bio
+Author-email: support@cirro.bio
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.24.0,<2.0.0)
+Requires-Dist: boto3 (==1.26.76)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: gql[requests] (>=3.4.0,<4.0.0)
+Requires-Dist: gql[requests] (>=3.4.1,<4.0.0)
 Requires-Dist: jsonschema (>=4.6.1,<5.0.0)
 Requires-Dist: msal-extensions (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
-Requires-Dist: pycognito (==2022.12.0)
-Requires-Dist: pygithub (==1.58.0)
-Requires-Dist: pyjwt (>=2.4.0,<3.0.0)
+Requires-Dist: pygithub (==1.58.2)
+Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Requires-Dist: requests (>=2.28.0,<3.0.0)
-Requires-Dist: requests_aws4auth (>=1.1.2,<2.0.0)
-Requires-Dist: s3fs (==2023.1.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests_aws4auth (>=1.2.3,<2.0.0)
+Requires-Dist: s3fs (==2023.6.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Repository, https://github.com/FredHutch/Cirro-client
 Description-Content-Type: text/markdown
 
 # Cirro Client
 
 [![Build Python package](https://github.com/FredHutch/Cirro-client/actions/workflows/package.yml/badge.svg)](https://github.com/FredHutch/Cirro-client/actions/workflows/package.yml)
```

