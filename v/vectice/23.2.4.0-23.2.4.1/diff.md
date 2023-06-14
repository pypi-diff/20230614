# Comparing `tmp/vectice-23.2.4.0.tar.gz` & `tmp/vectice-23.2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.4.0.tar", last modified: Thu Jun  1 08:01:23 2023, max compression
+gzip compressed data, was "vectice-23.2.4.1.tar", last modified: Wed Jun  7 11:17:22 2023, max compression
```

## Comparing `vectice-23.2.4.0.tar` & `vectice-23.2.4.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 08:01:12.000000 vectice-23.2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-01 08:01:23.730807 vectice-23.2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 08:01:12.000000 vectice-23.2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 08:01:12.000000 vectice-23.2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 08:01:23.730807 vectice-23.2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-01 08:01:12.000000 vectice-23.2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.710807 vectice-23.2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.710807 vectice-23.2.4.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.714807 vectice-23.2.4.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.722807 vectice-23.2.4.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25210 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.722807 vectice-23.2.4.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/dataframe_column_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    30033 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.714807 vectice-23.2.4.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.112568 vectice-23.2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 11:17:11.000000 vectice-23.2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-07 11:17:22.112568 vectice-23.2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-07 11:17:11.000000 vectice-23.2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 11:17:11.000000 vectice-23.2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 11:17:22.112568 vectice-23.2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-07 11:17:11.000000 vectice-23.2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.080568 vectice-23.2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.084568 vectice-23.2.4.1/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.092568 vectice-23.2.4.1/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.100568 vectice-23.2.4.1/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25210 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.104568 vectice-23.2.4.1/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.104568 vectice-23.2.4.1/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.108569 vectice-23.2.4.1/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.108569 vectice-23.2.4.1/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/metadata/dataframe_column_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30010 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.112568 vectice-23.2.4.1/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-07 11:17:11.000000 vectice-23.2.4.1/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:17:22.084568 vectice-23.2.4.1/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-07 11:17:22.000000 vectice-23.2.4.1/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-07 11:17:22.000000 vectice-23.2.4.1/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:17:22.000000 vectice-23.2.4.1/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-07 11:17:22.000000 vectice-23.2.4.1/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 11:17:22.000000 vectice-23.2.4.1/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.4.0/LICENSE` & `vectice-23.2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/PKG-INFO` & `vectice-23.2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.4.0
+Version: 23.2.4.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.4.0/setup.py` & `vectice-23.2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/__init__.py` & `vectice-23.2.4.1/src/vectice/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Vectice package.
 
 [![PyPI version](/_static/img/current_package.svg)](https://pypi.org/project/vectice/) [![PyPI pyversions](/_static/img/python_versions.svg)](https://pypi.python.org/pypi/vectice/)
 
 The Vectice package is a library allowing data-scientists
-to record their progress in the [Vectice app](https://docs.vectice.com/learn-vectice/what-is-vectice).
+to record their progress in the [Vectice app](https://docs.vectice.com/).
 
 This package exposes essential Vectice classes and methods:
 
 - the [connect][vectice.Connection.connect] method
 - the [Workspace][vectice.models.Workspace] class
 - the [Project][vectice.models.Project] class
 - the [Phase][vectice.models.Phase] class
```

### Comparing `vectice-23.2.4.0/src/vectice/api/__init__.py` & `vectice-23.2.4.1/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/_auth.py` & `vectice-23.2.4.1/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/attachment.py` & `vectice-23.2.4.1/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/client.py` & `vectice-23.2.4.1/src/vectice/api/client.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_api.py` & `vectice-23.2.4.1/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_code.py` & `vectice-23.2.4.1/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_code_version.py` & `vectice-23.2.4.1/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_dataset.py` & `vectice-23.2.4.1/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_entity_file.py` & `vectice-23.2.4.1/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.4.1/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_model.py` & `vectice-23.2.4.1/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.4.1/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/http_error.py` & `vectice-23.2.4.1/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/http_error_handlers.py` & `vectice-23.2.4.1/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/iteration.py` & `vectice-23.2.4.1/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/__init__.py` & `vectice-23.2.4.1/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/artifact_version.py` & `vectice-23.2.4.1/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/code.py` & `vectice-23.2.4.1/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/code_version.py` & `vectice-23.2.4.1/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/dataset_register.py` & `vectice-23.2.4.1/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/dataset_representation.py` & `vectice-23.2.4.1/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/dataset_version.py` & `vectice-23.2.4.1/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-23.2.4.1/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/files_metadata.py` & `vectice-23.2.4.1/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/iteration.py` & `vectice-23.2.4.1/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/last_assets.py` & `vectice-23.2.4.1/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/metric.py` & `vectice-23.2.4.1/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/model.py` & `vectice-23.2.4.1/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/model_register.py` & `vectice-23.2.4.1/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/model_representation.py` & `vectice-23.2.4.1/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/model_version.py` & `vectice-23.2.4.1/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/model_version_representation.py` & `vectice-23.2.4.1/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/paged_response.py` & `vectice-23.2.4.1/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/phase.py` & `vectice-23.2.4.1/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/project.py` & `vectice-23.2.4.1/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/property.py` & `vectice-23.2.4.1/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/public_config.py` & `vectice-23.2.4.1/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/step.py` & `vectice-23.2.4.1/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/json/workspace.py` & `vectice-23.2.4.1/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/last_assets.py` & `vectice-23.2.4.1/src/vectice/api/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/phase.py` & `vectice-23.2.4.1/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/project.py` & `vectice-23.2.4.1/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/rest_api.py` & `vectice-23.2.4.1/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/step.py` & `vectice-23.2.4.1/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/version.py` & `vectice-23.2.4.1/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/api/workspace.py` & `vectice-23.2.4.1/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/connection.py` & `vectice-23.2.4.1/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/__init__.py` & `vectice-23.2.4.1/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/attachment_container.py` & `vectice-23.2.4.1/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/dataset.py` & `vectice-23.2.4.1/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/git_version.py` & `vectice-23.2.4.1/src/vectice/models/git_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/iteration.py` & `vectice-23.2.4.1/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/metric.py` & `vectice-23.2.4.1/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/model.py` & `vectice-23.2.4.1/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/phase.py` & `vectice-23.2.4.1/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/project.py` & `vectice-23.2.4.1/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/property.py` & `vectice-23.2.4.1/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/representation/dataset_representation.py` & `vectice-23.2.4.1/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/__init__.py` & `vectice-23.2.4.1/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/base.py` & `vectice-23.2.4.1/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.4.1/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/description.py` & `vectice-23.2.4.1/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/file_resource.py` & `vectice-23.2.4.1/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/gcs_resource.py` & `vectice-23.2.4.1/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.4.1/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.4.1/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.2.4.1/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/metadata/dataframe_column_parser.py` & `vectice-23.2.4.1/src/vectice/models/resource/metadata/dataframe_column_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,34 @@
 
     return [column.asdict() for column in columns]
 
 
 def capture_column_stats(
     series: Series,
 ) -> tuple[ColumnCategoryType | None, TextStat | BooleanStat | NumericalStat | DateStat | None]:
+    def is_date_series(column: Series) -> bool:
+        if api.types.is_datetime64_any_dtype(column):
+            return True
+
+        try:
+            # Temporary fixing issue -> TypeError: data type 'dbdate' not understood [EN-2534]
+            if column.dtypes == "dbdate":
+                return True
+        except TypeError:
+            pass
+
+        return False
+
     if api.types.is_bool_dtype(series):
         return ColumnCategoryType.BOOLEAN, compute_boolean_column_statistics(series)
     elif api.types.is_numeric_dtype(series):
         return ColumnCategoryType.NUMERICAL, compute_numeric_column_statistics(series)
-    elif api.types.is_datetime64_any_dtype(series) | (series.dtypes == "dbdate"):
+    elif is_date_series(series):
         return ColumnCategoryType.DATE, compute_date_column_statistics(series)
-    elif api.types.is_string_dtype(series) | api.types.is_categorical_dtype(series):
+    if api.types.is_string_dtype(series) | api.types.is_categorical_dtype(series):
         return ColumnCategoryType.TEXT, compute_string_column_statistics(series)
     return None, None
 
 
 def compute_boolean_column_statistics(series: Series) -> BooleanStat:
     """Parse a dataframe series and return statistics about it.
```

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.4.1/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.2.4.1/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.4.1/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.4.1/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/step.py` & `vectice-23.2.4.1/src/vectice/models/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,17 +211,16 @@
                 [
                     IterationStepArtifact(entityFileId=attach["fileId"], type="EntityFile")
                     for attach in attachments_output
                 ]
                 if attachments_output
                 else []
             )
-            self.artifacts += attachments
+            self.artifacts.extend([model_artifact, *attachments])
             copy_artifacts = self.artifacts.copy()
-            self.artifacts += [model_artifact]
             self._keep_artifacts_and_update_step(StepType.StepModel, value)
             step = StepModel(self, model_artifact, value)
             _register_model_logging(self, model_data, value, self.name, attachments_output, _logger, copy_artifacts)
         elif (
             isinstance(value, Dataset)
             or isinstance(value, DatasetRepresentation)
             or isinstance(value, DatasetVersionRepresentation)
```

### Comparing `vectice-23.2.4.0/src/vectice/models/step_dataset.py` & `vectice-23.2.4.1/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/step_image.py` & `vectice-23.2.4.1/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/step_model.py` & `vectice-23.2.4.1/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/step_number.py` & `vectice-23.2.4.1/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/step_string.py` & `vectice-23.2.4.1/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/models/workspace.py` & `vectice-23.2.4.1/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/utils/automatic_link_utils.py` & `vectice-23.2.4.1/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/utils/common_utils.py` & `vectice-23.2.4.1/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/utils/configuration.py` & `vectice-23.2.4.1/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/utils/deprecation.py` & `vectice-23.2.4.1/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/utils/last_assets.py` & `vectice-23.2.4.1/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice/utils/logging_utils.py` & `vectice-23.2.4.1/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.4.1/src/vectice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.4.0
+Version: 23.2.4.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.4.0/src/vectice.egg-info/SOURCES.txt` & `vectice-23.2.4.1/src/vectice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectice-23.2.4.0/src/vectice.egg-info/requires.txt` & `vectice-23.2.4.1/src/vectice.egg-info/requires.txt`

 * *Files identical despite different names*

