# Comparing `tmp/astronomer_cosmos-0.7.1.tar.gz` & `tmp/astronomer_cosmos-0.7.2.tar.gz`

## Comparing `astronomer_cosmos-0.7.1.tar` & `astronomer_cosmos-0.7.2.tar`

### file list

```diff
@@ -1,80 +1,52 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/tests/test_airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/dataset.py
--rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9047 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/virtualenv.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_docker.py
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_local.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_virtualenv.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/base.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/token.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/thrift.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/base.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/warn_parsing.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/tests/test_project.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_dataset.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_export.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_render.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/test-connections.yaml
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/test_example_dags.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/test_version.py
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/utils.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/LICENSE
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/README.rst
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9047 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0    18883 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/virtualenv.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/base.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/base.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/ldap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/utils/warn_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/README.rst
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.2/PKG-INFO
```

### Comparing `astronomer_cosmos-0.7.1/cosmos/core/airflow.py` & `astronomer_cosmos-0.7.2/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.7.2/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/dag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 This module contains a function to render a dbt project as an Airflow DAG.
 """
+from __future__ import annotations
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from typing import Any, Callable, Dict, List, Optional
 
@@ -20,14 +22,16 @@
 
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The path to the dbt root directory
     :param dbt_models_dir: The path to the dbt models directory within the project
     :param dbt_seeds_dir: The path to the dbt seeds directory within the project
     :param conn_id: The Airflow connection ID to use for the dbt profile
     :param profile_args: Arguments to pass to the dbt profile
+    :param profile_name_override: A name to use for the dbt profile. If not provided, and no profile target is found
+        in your project's dbt_project.yml, "cosmos_profile" is used.
     :param dbt_args: Parameters to pass to the underlying dbt operators, can include dbt_executable_path to utilize venv
     :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
         or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
@@ -41,14 +45,15 @@
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         profile_args: Dict[str, str] = {},
         dbt_args: Dict[str, Any] = {},
+        profile_name_override: str | None = None,
         operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
         dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
@@ -72,14 +77,15 @@
             dbt_seeds_dir=dbt_seeds_dir,
             task_args=dbt_args,
             operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
             profile_args=profile_args,
+            profile_name=profile_name_override,
             select=select,
             exclude=exclude,
             execution_mode=execution_mode,
             on_warning_callback=on_warning_callback,
         )
 
         # call the airflow DAG constructor
```

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 This module contains a function to render a dbt project into Cosmos entities.
 """
+from __future__ import annotations
+
 import itertools
 import logging
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
@@ -36,14 +38,15 @@
     dbt_seeds_dir: str = "seeds",
     task_args: Dict[str, Any] = {},
     operator_args: Dict[str, Any] = {},
     test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
     emit_datasets: bool = True,
     conn_id: str = "default_conn_id",
     profile_args: Dict[str, str] = {},
+    profile_name: str | None = None,
     select: Dict[str, List[str]] = {},
     exclude: Dict[str, List[str]] = {},
     execution_mode: Literal["local", "docker", "kubernetes"] = "local",
     on_warning_callback: Optional[Callable] = None,
 ) -> Group:
     """
     Turn a dbt project into a Group
@@ -54,14 +57,16 @@
     :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
         or DockerOperator parameters
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param conn_id: The Airflow connection ID to use
     :param profile_args: Arguments to pass to the dbt profile
+    :param profile_name: A name to use for the dbt profile. If not provided, and no profile target is found
+        in your project's dbt_project.yml, "cosmos_profile" is used.
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2]}})
     :param execution_mode: The execution mode in which the dbt project should be run.
         Options are "local", "docker", and "kubernetes".
         Defaults to "local"
      :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
         and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
@@ -128,20 +133,22 @@
                 continue
 
         run_args: Dict[str, Any] = {
             **task_args,
             **operator_args,
             "models": model_name,
             "profile_args": profile_args,
+            "profile_name": profile_name,
         }
         test_args: Dict[str, Any] = {
             **task_args,
             **operator_args,
             "models": model_name,
             "profile_args": profile_args,
+            "profile_name": profile_name,
         }
         # DbtTestOperator specific arg
         test_args["on_warning_callback"] = on_warning_callback
         if emit_datasets:
             outlets = [get_dbt_dataset(conn_id, dbt_project_name, model_name)]
 
             if test_behavior == "after_each":
```

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/task_group.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 This module contains a function to render a dbt project as an Airflow Task Group.
 """
+from __future__ import annotations
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from typing import Any, Callable, Dict, List, Optional
 
@@ -21,14 +23,16 @@
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The path to the dbt root directory
     :param dbt_models_dir: The path to the dbt models directory within the project
     :param dbt_snapshots_dir: The path to the dbt snapshots directory within the project
     :param dbt_seeds_dir: The path to the dbt seeds directory within the project
     :param conn_id: The Airflow connection ID to use for the dbt profile
     :param profile_args: Arguments to pass to the dbt profile
+    :param profile_name_override: A name to use for the dbt profile. If not provided, and no profile target is found
+        in your project's dbt_project.yml, "cosmos_profile" is used.
     :param dbt_args: Parameters to pass to the underlying dbt operators, can include dbt_executable_path to utilize venv
     :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
         or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
@@ -41,14 +45,15 @@
     """
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         profile_args: Dict[str, str] = {},
+        profile_name_override: Optional[str] = None,
         dbt_args: Dict[str, Any] = {},
         operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
         dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_snapshots_dir: str = "snapshots",
         dbt_seeds_dir: str = "seeds",
@@ -75,14 +80,15 @@
             dbt_seeds_dir=dbt_seeds_dir,
             task_args=dbt_args,
             operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
             profile_args=profile_args,
+            profile_name=profile_name_override,
             select=select,
             exclude=exclude,
             execution_mode=execution_mode,
             on_warning_callback=on_warning_callback,
         )
 
         # call the airflow constructor
```

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import yaml
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.utils.context import Context
 from airflow.utils.session import NEW_SESSION, provide_session
 from sqlalchemy.orm import Session
 
+from cosmos.providers.dbt.constants import DEFAULT_DBT_PROFILE_NAME
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
 from cosmos.providers.dbt.core.profiles import get_profile_mapping
 from cosmos.providers.dbt.core.utils.adapted_subprocesshook import (
     FullOutputSubprocessHook,
     FullOutputSubprocessResult,
 )
 from cosmos.providers.dbt.core.utils.warn_parsing import (
@@ -31,33 +32,37 @@
 
 class DbtLocalBaseOperator(DbtBaseOperator):
     """
     Executes a dbt core cli command locally.
 
     :param profile_args: Arguments to pass to the profile. See
         :py:class:`cosmos.providers.dbt.core.profiles.BaseProfileMapping`.
+    :param profile_name: A name to use for the dbt profile. If not provided, and no profile target is found
+        in your project's dbt_project.yml, "cosmos_profile" is used.
     :param install_deps: If true, install dependencies before running the command
     :param callback: A callback function called on after a dbt run with a path to the dbt project directory.
     """
 
     template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)
     template_fields_renderers = {
         "compiled_sql": "sql",
     }
 
     def __init__(
         self,
         install_deps: bool = False,
         callback: Optional[Callable[[str], None]] = None,
         profile_args: dict[str, str] = {},
+        profile_name: str | None = None,
         **kwargs,
     ) -> None:
         self.install_deps = install_deps
         self.profile_args = profile_args
         self.callback = callback
+        self.profile_name = profile_name
         self.compiled_sql = ""
         super().__init__(**kwargs)
 
     @cached_property
     def subprocess_hook(self):
         """Returns hook for running the bash command."""
         return FullOutputSubprocessHook()
@@ -108,14 +113,46 @@
             RenderedTaskInstanceFields.run_id == ti.run_id,
         ).delete()
         session.add(rtif)
 
     def run_subprocess(self, *args, **kwargs):
         return self.subprocess_hook.run_command(*args, **kwargs)
 
+    def get_profile_name(self, project_dir: str) -> str:
+        """
+        Returns the profile name to use. Precedence is:
+        1. The profile name passed in to the operator
+        2. The profile name in the dbt_project.yml file
+        3. "cosmos_profile"
+        """
+        if self.profile_name:
+            return self.profile_name
+
+        # get the profile name from the dbt_project.yml file
+        dbt_project_path = os.path.join(project_dir, "dbt_project.yml")
+
+        # if there's no dbt_project.yml file, we're not in a dbt project
+        # and need to raise an error
+        if not os.path.exists(dbt_project_path):
+            raise AirflowException(f"dbt project directory {self.project_dir} does not contain a dbt_project.yml file.")
+
+        # get file contents using path
+        dbt_project = yaml.safe_load(Path(dbt_project_path).read_text(encoding="utf-8")) or {}
+
+        profile_name = dbt_project.get("profile", DEFAULT_DBT_PROFILE_NAME)
+
+        if not isinstance(profile_name, str):
+            raise AirflowException(
+                f"dbt project directory {self.project_dir} contains a dbt_project.yml file, but the profile "
+                f"specified in the file is not a string. Please specify a string profile name, or pass a profile "
+                f"name to the operator."
+            )
+
+        return profile_name
+
     def run_command(
         self,
         cmd: list[str],
         env: dict[str, str],
         context: Context,
     ) -> FullOutputSubprocessResult:
         """
@@ -131,28 +168,15 @@
             # need a subfolder because shutil.copytree will fail if the destination dir already exists
             tmp_project_dir = os.path.join(tmp_dir, "dbt_project")
             shutil.copytree(
                 self.project_dir,
                 tmp_project_dir,
             )
 
-            # get the profile name from the dbt_project.yml file
-            dbt_project_path = os.path.join(tmp_project_dir, "dbt_project.yml")
-
-            # if there's no dbt_project.yml file, we're not in a dbt project
-            # and need to raise an error
-            if not os.path.exists(dbt_project_path):
-                raise AirflowException(
-                    f"dbt project directory {self.project_dir} does not contain a dbt_project.yml file."
-                )
-
-            with open(dbt_project_path, encoding="utf-8") as f:
-                dbt_project = yaml.safe_load(f)
-
-            profile_name = dbt_project.get("profile")
+            profile_name = self.get_profile_name(tmp_project_dir)
 
             # need to write the profile to a file because dbt requires a profile file
             # and doesn't accept a profile as a string
             profile_mapping = get_profile_mapping(
                 conn_id=self.conn_id,
                 profile_args=self.profile_args,
             )
@@ -174,15 +198,15 @@
                     output_encoding=self.output_encoding,
                     cwd=tmp_project_dir,
                 )
 
             logger.info("Trying to run the command:\n %s\nFrom %s", cmd, tmp_project_dir)
 
             result = self.run_subprocess(
-                command=cmd,
+                command=cmd + ["--profile", profile_name],
                 env=env,
                 output_encoding=self.output_encoding,
                 cwd=tmp_project_dir,
             )
 
             self.exception_handling(result)
             self.store_compiled_sql(tmp_project_dir, context)
```

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/virtualenv.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/base.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/token.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/user_pass.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/user_pass.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/user_pass.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/thrift.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/base.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/certificate.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/jwt.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/ldap.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/warn_parsing.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/core/utils/warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.7.2/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/.gitignore` & `astronomer_cosmos-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/LICENSE` & `astronomer_cosmos-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/README.rst` & `astronomer_cosmos-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.1/pyproject.toml` & `astronomer_cosmos-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     { value = "apache-airflow==2.5", if = ["2.5"] },
     { value = "apache-airflow==2.6", if = ["2.6"] },
 ]
 
 [tool.hatch.envs.tests.scripts]
 freeze = "pip freeze"
 test = 'pytest -vv --durations=0 . -m "not integration"'
-test-cov = 'pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 . -m "not integration"'
+test-cov = 'pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 -m "not integration"'
 test-integration = "pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 -m integration"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
 minversion = "6.0"
```

### Comparing `astronomer_cosmos-0.7.1/PKG-INFO` & `astronomer_cosmos-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.7.1
+Version: 0.7.2
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
```

