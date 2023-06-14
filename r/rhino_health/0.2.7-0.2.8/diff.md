# Comparing `tmp/rhino_health-0.2.7.tar.gz` & `tmp/rhino_health-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhino_health-0.2.7.tar", last modified: Wed Dec 14 08:45:11 2022, max compression
+gzip compressed data, was "rhino_health-0.2.8.tar", last modified: Thu Dec 15 08:45:41 2022, max compression
```

## Comparing `rhino_health-0.2.7.tar` & `rhino_health-0.2.8.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      337 2022-12-14 08:45:05.828954 rhino_health-0.2.7/.coveragerc
--rw-r--r--   0        0        0      178 2022-12-14 08:45:05.828954 rhino_health-0.2.7/.editorconfig
--rw-r--r--   0        0        0     1827 2022-12-14 08:45:05.828954 rhino_health-0.2.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1180 2022-12-14 08:45:05.828954 rhino_health-0.2.7/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1282 2022-12-14 08:45:05.828954 rhino_health-0.2.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      113 2022-12-14 08:45:05.828954 rhino_health-0.2.7/.gitignore
--rw-r--r--   0        0        0      569 2022-12-14 08:45:05.828954 rhino_health-0.2.7/DEVELOPMENT.md
--rw-r--r--   0        0        0     9484 2022-12-14 08:45:05.828954 rhino_health-0.2.7/LICENSE.md
--rw-r--r--   0        0        0      465 2022-12-14 08:45:05.828954 rhino_health-0.2.7/Makefile
--rw-r--r--   0        0        0     2513 2022-12-14 08:45:05.828954 rhino_health-0.2.7/README.md
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs/.gitkeep
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs/.nojekyll
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs/html/.gitkeep
--rw-r--r--   0        0        0      215 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs/index.html
--rw-r--r--   0        0        0      638 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs_src/Makefile
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs_src/build/.gitkeep
--rw-r--r--   0        0        0      769 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs_src/make.bat
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs_src/source/_static/.gitkeep
--rw-r--r--   0        0        0      120 2022-12-14 08:45:05.828954 rhino_health-0.2.7/docs_src/source/_static/switcher.json
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/docs_src/source/_templates/.gitkeep
--rw-r--r--   0        0        0     8940 2022-12-14 08:45:05.832954 rhino_health-0.2.7/docs_src/source/conf.py
--rw-r--r--   0        0        0      443 2022-12-14 08:45:05.832954 rhino_health-0.2.7/docs_src/source/index.rst
--rw-r--r--   0        0        0     2325 2022-12-14 08:45:05.832954 rhino_health-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1545 2022-12-14 08:45:05.832954 rhino_health-0.2.7/requirements.txt
--rw-r--r--   0        0        0     3060 2022-12-14 08:45:11.261035 rhino_health-0.2.7/rhino_health/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/__init__.py
--rw-r--r--   0        0        0     1700 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/constants.py
--rw-r--r--   0        0        0     2382 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/dataclass.py
--rw-r--r--   0        0        0      288 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/__init__.py
--rw-r--r--   0        0        0      143 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/aimodel/__init__.py
--rw-r--r--   0        0        0     9213 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/aimodel/aimodel_dataclass.py
--rw-r--r--   0        0        0     7624 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/aimodel/aimodel_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/cohort/__init__.py
--rw-r--r--   0        0        0     9791 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/cohort/cohort_dataclass.py
--rw-r--r--   0        0        0     9965 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/cohort/cohort_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/dataschema/__init__.py
--rw-r--r--   0        0        0     4660 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/dataschema/dataschema_dataclass.py
--rw-r--r--   0        0        0     7939 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/dataschema/dataschema_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/dicomweb_query/__init__.py
--rw-r--r--   0        0        0     2947 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_dataclass.py
--rw-r--r--   0        0        0     4290 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_endpoints.py
--rw-r--r--   0        0        0      931 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/endpoint.py
--rw-r--r--   0        0        0       87 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/model_result/__init__.py
--rw-r--r--   0        0        0     2806 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/model_result/model_result_dataclass.py
--rw-r--r--   0        0        0      982 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/model_result/model_result_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/project/__init__.py
--rw-r--r--   0        0        0     8119 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/project/project_dataclass.py
--rw-r--r--   0        0        0    11534 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/project/project_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/user/__init__.py
--rw-r--r--   0        0        0     2407 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/user/user_dataclass.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/workgroup/__init__.py
--rw-r--r--   0        0        0      922 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/workgroup/workgroup_dataclass.py
--rw-r--r--   0        0        0       23 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/endpoints/workgroup/workgroup_endpoints.py
--rw-r--r--   0        0        0      853 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/__init__.py
--rw-r--r--   0        0        0     4697 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/aggregate_metrics.py
--rw-r--r--   0        0        0     2762 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/base_metric.py
--rw-r--r--   0        0        0      920 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/basic.py
--rw-r--r--   0        0        0     8671 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/classification.py
--rw-r--r--   0        0        0     2511 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/filter_variable.py
--rw-r--r--   0        0        0      764 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/froc.py
--rw-r--r--   0        0        0     1399 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/metric_utils.py
--rw-r--r--   0        0        0      733 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/metrics/roc_auc.py
--rw-r--r--   0        0        0       27 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/rest_api/__init__.py
--rw-r--r--   0        0        0     1440 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/rest_api/api_request.py
--rw-r--r--   0        0        0     4577 2022-12-14 08:45:05.832954 rhino_health-0.2.7/rhino_health/lib/rest_api/api_response.py
--rw-r--r--   0        0        0     1061 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_api/error_handler.py
--rw-r--r--   0        0        0       23 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_api/error_parsers/__init__.py
--rw-r--r--   0        0        0      518 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_api/error_parsers/error_parser.py
--rw-r--r--   0        0        0      991 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_api/error_parsers/eula.py
--rw-r--r--   0        0        0      689 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_api/error_parsers/reverse_rpc.py
--rw-r--r--   0        0        0      497 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_api/request_adapter.py
--rw-r--r--   0        0        0     6876 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_api/rhino_authenticator.py
--rw-r--r--   0        0        0     2764 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rest_handler.py
--rw-r--r--   0        0        0     3809 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rhino_client.py
--rw-r--r--   0        0        0     5208 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/rhino_session.py
--rw-r--r--   0        0        0     2558 2022-12-14 08:45:05.836954 rhino_health-0.2.7/rhino_health/lib/utils.py
--rw-r--r--   0        0        0      159 2022-12-14 08:45:05.836954 rhino_health-0.2.7/sonar-project.properties
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/aimodel/__init__.py
--rw-r--r--   0        0        0      848 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/aimodel/test_aimodel_dataclass.py
--rw-r--r--   0        0        0     4938 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/aimodel/test_aimodel_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/model_result/__init__.py
--rw-r--r--   0        0        0     1514 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/model_result/test_model_result_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/project/__init__.py
--rw-r--r--   0        0        0      946 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/endpoints/project/test_project_endpoints.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/metrics/__init__.py
--rw-r--r--   0        0        0     2460 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/metrics/test_aggregate_metrics.py
--rw-r--r--   0        0        0     1575 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/metrics/test_metric_utils.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/rest_api/__init__.py
--rw-r--r--   0        0        0      992 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/rest_api/api_response_factory.py
--rw-r--r--   0        0        0        0 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/rest_api/error_parsers/__init__.py
--rw-r--r--   0        0        0      996 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/rest_api/error_parsers/test_eula.py
--rw-r--r--   0        0        0     1026 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/rest_api/error_parsers/test_reverse_rpc.py
--rw-r--r--   0        0        0      974 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/rhino_session_factory.py
--rw-r--r--   0        0        0      583 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/lib/test_utils.py
--rw-r--r--   0        0        0     2040 2022-12-14 08:45:05.836954 rhino_health-0.2.7/test/test_happy_path.py
--rw-r--r--   0        0        0      414 2022-12-14 08:45:05.836954 rhino_health-0.2.7/tox.ini
--rw-r--r--   0        0        0      454 2022-12-14 08:45:05.836954 rhino_health-0.2.7/tox_install_deps.py
--rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 rhino_health-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      337 2022-12-15 08:45:21.706197 rhino_health-0.2.8/.coveragerc
+-rw-r--r--   0        0        0      178 2022-12-15 08:45:21.706197 rhino_health-0.2.8/.editorconfig
+-rw-r--r--   0        0        0     1827 2022-12-15 08:45:21.706197 rhino_health-0.2.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1180 2022-12-15 08:45:21.706197 rhino_health-0.2.8/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1282 2022-12-15 08:45:21.706197 rhino_health-0.2.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      113 2022-12-15 08:45:21.706197 rhino_health-0.2.8/.gitignore
+-rw-r--r--   0        0        0      569 2022-12-15 08:45:21.706197 rhino_health-0.2.8/DEVELOPMENT.md
+-rw-r--r--   0        0        0     9484 2022-12-15 08:45:21.706197 rhino_health-0.2.8/LICENSE.md
+-rw-r--r--   0        0        0      465 2022-12-15 08:45:21.706197 rhino_health-0.2.8/Makefile
+-rw-r--r--   0        0        0     2513 2022-12-15 08:45:21.706197 rhino_health-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.706197 rhino_health-0.2.8/docs/.gitkeep
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.706197 rhino_health-0.2.8/docs/.nojekyll
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.706197 rhino_health-0.2.8/docs/html/.gitkeep
+-rw-r--r--   0        0        0      215 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs/index.html
+-rw-r--r--   0        0        0      638 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/Makefile
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/build/.gitkeep
+-rw-r--r--   0        0        0      769 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/make.bat
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/source/_static/.gitkeep
+-rw-r--r--   0        0        0      120 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/source/_static/switcher.json
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/source/_templates/.gitkeep
+-rw-r--r--   0        0        0     8940 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/source/conf.py
+-rw-r--r--   0        0        0      443 2022-12-15 08:45:21.710198 rhino_health-0.2.8/docs_src/source/index.rst
+-rw-r--r--   0        0        0     2325 2022-12-15 08:45:21.710198 rhino_health-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1545 2022-12-15 08:45:21.710198 rhino_health-0.2.8/requirements.txt
+-rw-r--r--   0        0        0     3060 2022-12-15 08:45:40.559458 rhino_health-0.2.8/rhino_health/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/__init__.py
+-rw-r--r--   0        0        0     1700 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/constants.py
+-rw-r--r--   0        0        0     2382 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/dataclass.py
+-rw-r--r--   0        0        0      288 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/__init__.py
+-rw-r--r--   0        0        0      143 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/aimodel/__init__.py
+-rw-r--r--   0        0        0     9213 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/aimodel/aimodel_dataclass.py
+-rw-r--r--   0        0        0     7624 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/aimodel/aimodel_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/cohort/__init__.py
+-rw-r--r--   0        0        0     9791 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/cohort/cohort_dataclass.py
+-rw-r--r--   0        0        0     9965 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/cohort/cohort_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/dataschema/__init__.py
+-rw-r--r--   0        0        0     4660 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/dataschema/dataschema_dataclass.py
+-rw-r--r--   0        0        0     7939 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/dataschema/dataschema_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/dicomweb_query/__init__.py
+-rw-r--r--   0        0        0     2947 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_dataclass.py
+-rw-r--r--   0        0        0     4290 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_endpoints.py
+-rw-r--r--   0        0        0      931 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/endpoint.py
+-rw-r--r--   0        0        0       87 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/model_result/__init__.py
+-rw-r--r--   0        0        0     2806 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/model_result/model_result_dataclass.py
+-rw-r--r--   0        0        0      982 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/model_result/model_result_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/project/__init__.py
+-rw-r--r--   0        0        0     8119 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/project/project_dataclass.py
+-rw-r--r--   0        0        0    11473 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/project/project_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/user/__init__.py
+-rw-r--r--   0        0        0     2407 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/user/user_dataclass.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/workgroup/__init__.py
+-rw-r--r--   0        0        0      922 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/workgroup/workgroup_dataclass.py
+-rw-r--r--   0        0        0       23 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/endpoints/workgroup/workgroup_endpoints.py
+-rw-r--r--   0        0        0      853 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/__init__.py
+-rw-r--r--   0        0        0     4697 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/aggregate_metrics.py
+-rw-r--r--   0        0        0     2762 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/base_metric.py
+-rw-r--r--   0        0        0      920 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/basic.py
+-rw-r--r--   0        0        0     8671 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/classification.py
+-rw-r--r--   0        0        0     2511 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/filter_variable.py
+-rw-r--r--   0        0        0      764 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/froc.py
+-rw-r--r--   0        0        0     1399 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/metric_utils.py
+-rw-r--r--   0        0        0      733 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/metrics/roc_auc.py
+-rw-r--r--   0        0        0       27 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/__init__.py
+-rw-r--r--   0        0        0     1440 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/api_request.py
+-rw-r--r--   0        0        0     4577 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/api_response.py
+-rw-r--r--   0        0        0     1061 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/error_handler.py
+-rw-r--r--   0        0        0       23 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/error_parsers/__init__.py
+-rw-r--r--   0        0        0      518 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/error_parsers/error_parser.py
+-rw-r--r--   0        0        0      991 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/error_parsers/eula.py
+-rw-r--r--   0        0        0      689 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/error_parsers/reverse_rpc.py
+-rw-r--r--   0        0        0      497 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/request_adapter.py
+-rw-r--r--   0        0        0     6876 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_api/rhino_authenticator.py
+-rw-r--r--   0        0        0     2764 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rest_handler.py
+-rw-r--r--   0        0        0     3809 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rhino_client.py
+-rw-r--r--   0        0        0     5208 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/rhino_session.py
+-rw-r--r--   0        0        0     2558 2022-12-15 08:45:21.710198 rhino_health-0.2.8/rhino_health/lib/utils.py
+-rw-r--r--   0        0        0      159 2022-12-15 08:45:21.710198 rhino_health-0.2.8/sonar-project.properties
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/aimodel/__init__.py
+-rw-r--r--   0        0        0      848 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/aimodel/test_aimodel_dataclass.py
+-rw-r--r--   0        0        0     4938 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/aimodel/test_aimodel_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/model_result/__init__.py
+-rw-r--r--   0        0        0     1514 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/model_result/test_model_result_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/project/__init__.py
+-rw-r--r--   0        0        0      946 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/endpoints/project/test_project_endpoints.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/metrics/__init__.py
+-rw-r--r--   0        0        0     2460 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/metrics/test_aggregate_metrics.py
+-rw-r--r--   0        0        0     1575 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/metrics/test_metric_utils.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/rest_api/__init__.py
+-rw-r--r--   0        0        0      992 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/rest_api/api_response_factory.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/rest_api/error_parsers/__init__.py
+-rw-r--r--   0        0        0      996 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/rest_api/error_parsers/test_eula.py
+-rw-r--r--   0        0        0     1026 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/rest_api/error_parsers/test_reverse_rpc.py
+-rw-r--r--   0        0        0      974 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/rhino_session_factory.py
+-rw-r--r--   0        0        0      583 2022-12-15 08:45:21.710198 rhino_health-0.2.8/test/lib/test_utils.py
+-rw-r--r--   0        0        0     2040 2022-12-15 08:45:21.714198 rhino_health-0.2.8/test/test_happy_path.py
+-rw-r--r--   0        0        0      414 2022-12-15 08:45:21.714198 rhino_health-0.2.8/tox.ini
+-rw-r--r--   0        0        0      454 2022-12-15 08:45:21.714198 rhino_health-0.2.8/tox_install_deps.py
+-rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 rhino_health-0.2.8/PKG-INFO
```

### Comparing `rhino_health-0.2.7/.github/workflows/ci.yml` & `rhino_health-0.2.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/.github/workflows/docs.yml` & `rhino_health-0.2.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/.github/workflows/publish.yml` & `rhino_health-0.2.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/DEVELOPMENT.md` & `rhino_health-0.2.8/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/LICENSE.md` & `rhino_health-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/README.md` & `rhino_health-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/docs_src/Makefile` & `rhino_health-0.2.8/docs_src/Makefile`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/docs_src/make.bat` & `rhino_health-0.2.8/docs_src/make.bat`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/docs_src/source/conf.py` & `rhino_health-0.2.8/docs_src/source/conf.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/pyproject.toml` & `rhino_health-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/requirements.txt` & `rhino_health-0.2.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/__init__.py` & `rhino_health-0.2.8/rhino_health/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Entry point to using the Rhino Health Python SDK."""
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 from typing import Optional
 
 import rhino_health.lib.endpoints
 import rhino_health.lib.metrics
 from rhino_health.lib.constants import ApiEnvironment
 from rhino_health.lib.rest_api.rhino_authenticator import SSOAuthenticationDetails
```

### Comparing `rhino_health-0.2.7/rhino_health/lib/constants.py` & `rhino_health-0.2.8/rhino_health/lib/constants.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/aimodel/aimodel_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/aimodel/aimodel_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/aimodel/aimodel_endpoints.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/aimodel/aimodel_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/cohort/cohort_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/cohort/cohort_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/cohort/cohort_endpoints.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/cohort/cohort_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/dataschema/dataschema_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/dataschema/dataschema_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/dataschema/dataschema_endpoints.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/dataschema/dataschema_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_endpoints.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/dicomweb_query/dicomweb_query_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/endpoint.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/model_result/model_result_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/model_result/model_result_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/model_result/model_result_endpoints.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/model_result/model_result_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/project/project_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/project/project_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/project/project_endpoints.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/project/project_endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,17 +180,15 @@
     @rhino_error_wrapper
     def get_cohorts(self, project_uid: str) -> List[Cohort]:
         """
         Returns Cohorts associated with the project_uid
         """
         if not project_uid:
             raise ValueError("Must provide a project id")
-        query_params = self._get_filter_query_params(
-            {"project_uid": project_uid}, name_filter_mode=NameFilterMode.EXACT
-        )
+        query_params = self._get_filter_query_params({"project_uid": project_uid})
         return self.session.get("cohorts", params=query_params).to_dataclasses(
             self.cohort_dataclass
         )
 
     @rhino_error_wrapper
     def get_cohort_by_name(
         self, name, version=VersionMode.LATEST, project_uid=None
```

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/user/user_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/user/user_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/endpoints/workgroup/workgroup_dataclass.py` & `rhino_health-0.2.8/rhino_health/lib/endpoints/workgroup/workgroup_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/__init__.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/aggregate_metrics.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/aggregate_metrics.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/base_metric.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/base_metric.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/basic.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/basic.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/classification.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/filter_variable.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/filter_variable.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/froc.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/metric_utils.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/metric_utils.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/metrics/roc_auc.py` & `rhino_health-0.2.8/rhino_health/lib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_api/api_request.py` & `rhino_health-0.2.8/rhino_health/lib/rest_api/api_request.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_api/api_response.py` & `rhino_health-0.2.8/rhino_health/lib/rest_api/api_response.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_api/error_handler.py` & `rhino_health-0.2.8/rhino_health/lib/rest_api/error_handler.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_api/error_parsers/error_parser.py` & `rhino_health-0.2.8/rhino_health/lib/rest_api/error_parsers/error_parser.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_api/error_parsers/eula.py` & `rhino_health-0.2.8/rhino_health/lib/rest_api/error_parsers/eula.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_api/error_parsers/reverse_rpc.py` & `rhino_health-0.2.8/rhino_health/lib/rest_api/error_parsers/reverse_rpc.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_api/rhino_authenticator.py` & `rhino_health-0.2.8/rhino_health/lib/rest_api/rhino_authenticator.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rest_handler.py` & `rhino_health-0.2.8/rhino_health/lib/rest_handler.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rhino_client.py` & `rhino_health-0.2.8/rhino_health/lib/rhino_client.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/rhino_session.py` & `rhino_health-0.2.8/rhino_health/lib/rhino_session.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/rhino_health/lib/utils.py` & `rhino_health-0.2.8/rhino_health/lib/utils.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/endpoints/aimodel/test_aimodel_dataclass.py` & `rhino_health-0.2.8/test/lib/endpoints/aimodel/test_aimodel_dataclass.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/endpoints/aimodel/test_aimodel_endpoints.py` & `rhino_health-0.2.8/test/lib/endpoints/aimodel/test_aimodel_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/endpoints/model_result/test_model_result_endpoints.py` & `rhino_health-0.2.8/test/lib/endpoints/model_result/test_model_result_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/endpoints/project/test_project_endpoints.py` & `rhino_health-0.2.8/test/lib/endpoints/project/test_project_endpoints.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/metrics/test_aggregate_metrics.py` & `rhino_health-0.2.8/test/lib/metrics/test_aggregate_metrics.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/metrics/test_metric_utils.py` & `rhino_health-0.2.8/test/lib/metrics/test_metric_utils.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/rest_api/api_response_factory.py` & `rhino_health-0.2.8/test/lib/rest_api/api_response_factory.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/rest_api/error_parsers/test_eula.py` & `rhino_health-0.2.8/test/lib/rest_api/error_parsers/test_eula.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/rest_api/error_parsers/test_reverse_rpc.py` & `rhino_health-0.2.8/test/lib/rest_api/error_parsers/test_reverse_rpc.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/rhino_session_factory.py` & `rhino_health-0.2.8/test/lib/rhino_session_factory.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/lib/test_utils.py` & `rhino_health-0.2.8/test/lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/test/test_happy_path.py` & `rhino_health-0.2.8/test/test_happy_path.py`

 * *Files identical despite different names*

### Comparing `rhino_health-0.2.7/PKG-INFO` & `rhino_health-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhino_health
-Version: 0.2.7
+Version: 0.2.8
 Summary: Standard Development Kit for interacting with the Rhino Health Federated Learning Platform
 Keywords: SDK,Rhino,Rhino Health,Federated Learning,Federated,AI
 Author-email: Rhino Health <rhino-sdk@rhinohealth.com>
 Maintainer-email: Rhino Health <rhino-sdk@rhinohealth.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

