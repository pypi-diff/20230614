# Comparing `tmp/pycarlo-0.7.5.tar.gz` & `tmp/pycarlo-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycarlo-0.7.5.tar", last modified: Wed May 24 14:48:28 2023, max compression
+gzip compressed data, was "dist/pycarlo-0.7.6.tar", last modified: Wed Jun 14 13:35:23 2023, max compression
```

## Comparing `pycarlo-0.7.5.tar` & `pycarlo-0.7.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.285155 pycarlo-0.7.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.269155 pycarlo-0.7.5/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-24 14:48:12.000000 pycarlo-0.7.5/.circleci/README.md
--rw-r--r--   0 root         (0) root         (0)     3101 2023-05-24 14:48:12.000000 pycarlo-0.7.5/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.269155 pycarlo-0.7.5/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-24 14:48:12.000000 pycarlo-0.7.5/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 14:48:12.000000 pycarlo-0.7.5/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1832 2023-05-24 14:48:12.000000 pycarlo-0.7.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-24 14:48:12.000000 pycarlo-0.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1986 2023-05-24 14:48:12.000000 pycarlo-0.7.5/Makefile
--rw-r--r--   0 root         (0) root         (0)     7803 2023-05-24 14:48:28.285155 pycarlo-0.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7026 2023-05-24 14:48:12.000000 pycarlo-0.7.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.269155 pycarlo-0.7.5/examples/
--rw-r--r--   0 root         (0) root         (0)      505 2023-05-24 14:48:12.000000 pycarlo-0.7.5/examples/sample_circuit_breaker.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-24 14:48:12.000000 pycarlo-0.7.5/examples/sample_insight_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.269155 pycarlo-0.7.5/pycarlo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.273155 pycarlo-0.7.5/pycarlo/common/
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/errors.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/files.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/http.py
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/mcon.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/retries.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/settings.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.273155 pycarlo-0.7.5/pycarlo/core/
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4434 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/core/client.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/core/endpoint.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/core/operations.py
--rw-r--r--   0 root         (0) root         (0)     3826 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/core/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.273155 pycarlo-0.7.5/pycarlo/features/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.273155 pycarlo-0.7.5/pycarlo/features/circuit_breakers/
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/circuit_breakers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/circuit_breakers/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    11391 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/circuit_breakers/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.273155 pycarlo-0.7.5/pycarlo/features/dbt/
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/dbt/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17849 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/dbt/dbt_importer.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/dbt/queries.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.273155 pycarlo-0.7.5/pycarlo/features/metadata/
--rw-r--r--   0 root         (0) root         (0)      206 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5007 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/metadata/allow_block_list.py
--rw-r--r--   0 root         (0) root         (0)    12229 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/metadata/metadata_filters_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.273155 pycarlo-0.7.5/pycarlo/features/pii/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/pii/__init__.py
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/pii/constants.py
--rw-r--r--   0 root         (0) root         (0)     6051 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/pii/pii_filterer.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/pii/queries.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/pii/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.277155 pycarlo-0.7.5/pycarlo/features/user/
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/user/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/user/models.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/user/queries.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/features/user/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.277155 pycarlo-0.7.5/pycarlo/lib/
--rw-r--r--   0 root         (0) root         (0)      139 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/lib/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2701678 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/lib/schema.json
--rw-r--r--   0 root         (0) root         (0)   973803 2023-05-24 14:48:12.000000 pycarlo-0.7.5/pycarlo/lib/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.269155 pycarlo-0.7.5/pycarlo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7803 2023-05-24 14:48:28.000000 pycarlo-0.7.5/pycarlo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2554 2023-05-24 14:48:28.000000 pycarlo-0.7.5/pycarlo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 14:48:28.000000 pycarlo-0.7.5/pycarlo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-24 14:48:28.000000 pycarlo-0.7.5/pycarlo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 14:48:28.000000 pycarlo-0.7.5/pycarlo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-24 14:48:12.000000 pycarlo-0.7.5/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-24 14:48:12.000000 pycarlo-0.7.5/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-24 14:48:12.000000 pycarlo-0.7.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 14:48:28.289155 pycarlo-0.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1477 2023-05-24 14:48:12.000000 pycarlo-0.7.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.281155 pycarlo-0.7.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.281155 pycarlo-0.7.5/tests/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/common/data.json
--rw-r--r--   0 root         (0) root         (0)      912 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/common/test_files.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/common/test_http.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/common/test_mcon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.281155 pycarlo-0.7.5/tests/features/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.281155 pycarlo-0.7.5/tests/features/circuit_breakers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/circuit_breakers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7326 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/circuit_breakers/test_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.281155 pycarlo-0.7.5/tests/features/dbt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/dbt/__init__.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/dbt/sample_logs.txt
--rw-r--r--   0 root         (0) root         (0)    16826 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/dbt/sample_manifest.json
--rw-r--r--   0 root         (0) root         (0)     3237 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/dbt/sample_run_results.json
--rw-r--r--   0 root         (0) root         (0)    15115 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/dbt/test_dbt_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.281155 pycarlo-0.7.5/tests/features/metadata/
--rw-r--r--   0 root         (0) root         (0)    18130 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/metadata/test_dataset_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.281155 pycarlo-0.7.5/tests/features/pii/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.285155 pycarlo-0.7.5/tests/features/pii/sample_events/
--rw-r--r--   0 root         (0) root         (0)  1638574 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/pii/sample_events/sample_md_events_01.json
--rw-r--r--   0 root         (0) root         (0)   125065 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/pii/sample_events/sample_md_events_02.json
--rw-r--r--   0 root         (0) root         (0)    11340 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/pii/test_pii_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.285155 pycarlo-0.7.5/tests/features/user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/user/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/features/user/test_user_service.py
--rw-r--r--   0 root         (0) root         (0)    10305 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/test_operations.py
--rw-r--r--   0 root         (0) root         (0)     2278 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/test_retry_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-05-24 14:48:12.000000 pycarlo-0.7.5/tests/test_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 14:48:28.285155 pycarlo-0.7.5/utils/
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-24 14:48:12.000000 pycarlo-0.7.5/utils/env.sh
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-24 14:48:12.000000 pycarlo-0.7.5/utils/generate.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-05-24 14:48:12.000000 pycarlo-0.7.5/utils/sample.env
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-24 14:48:12.000000 pycarlo-0.7.5/utils/sanity.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-05-24 14:48:12.000000 pycarlo-0.7.5/utils/vars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.212459 pycarlo-0.7.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.196459 pycarlo-0.7.6/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-14 13:35:06.000000 pycarlo-0.7.6/.circleci/README.md
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-06-14 13:35:06.000000 pycarlo-0.7.6/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-14 13:35:06.000000 pycarlo-0.7.6/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-14 13:35:06.000000 pycarlo-0.7.6/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-14 13:35:06.000000 pycarlo-0.7.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-14 13:35:06.000000 pycarlo-0.7.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-06-14 13:35:06.000000 pycarlo-0.7.6/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7803 2023-06-14 13:35:23.212459 pycarlo-0.7.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7026 2023-06-14 13:35:06.000000 pycarlo-0.7.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/examples/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-14 13:35:06.000000 pycarlo-0.7.6/examples/sample_circuit_breaker.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-14 13:35:06.000000 pycarlo-0.7.6/examples/sample_insight_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/pycarlo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/pycarlo/common/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/files.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/http.py
+-rw-r--r--   0 root         (0) root         (0)      622 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/mcon.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/retries.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/pycarlo/core/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/core/client.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/core/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/core/operations.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/core/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/pycarlo/features/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/pycarlo/features/circuit_breakers/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/circuit_breakers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      229 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/circuit_breakers/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/circuit_breakers/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.204459 pycarlo-0.7.6/pycarlo/features/dbt/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/dbt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17849 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/dbt/dbt_importer.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/dbt/queries.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.204459 pycarlo-0.7.6/pycarlo/features/metadata/
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5007 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/metadata/allow_block_list.py
+-rw-r--r--   0 root         (0) root         (0)    12229 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/metadata/metadata_filters_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.204459 pycarlo-0.7.6/pycarlo/features/pii/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/pii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/pii/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/pii/pii_filterer.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/pii/queries.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/pii/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.204459 pycarlo-0.7.6/pycarlo/features/user/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/user/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/user/models.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/user/queries.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/features/user/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.208459 pycarlo-0.7.6/pycarlo/lib/
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/lib/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2701678 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/lib/schema.json
+-rw-r--r--   0 root         (0) root         (0)   973803 2023-06-14 13:35:06.000000 pycarlo-0.7.6/pycarlo/lib/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.200459 pycarlo-0.7.6/pycarlo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7803 2023-06-14 13:35:23.000000 pycarlo-0.7.6/pycarlo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-14 13:35:23.000000 pycarlo-0.7.6/pycarlo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 13:35:23.000000 pycarlo-0.7.6/pycarlo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-14 13:35:23.000000 pycarlo-0.7.6/pycarlo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 13:35:23.000000 pycarlo-0.7.6/pycarlo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-14 13:35:06.000000 pycarlo-0.7.6/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-14 13:35:06.000000 pycarlo-0.7.6/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-14 13:35:06.000000 pycarlo-0.7.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-14 13:35:23.212459 pycarlo-0.7.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-06-14 13:35:06.000000 pycarlo-0.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.208459 pycarlo-0.7.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.208459 pycarlo-0.7.6/tests/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/common/data.json
+-rw-r--r--   0 root         (0) root         (0)      912 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/common/test_files.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/common/test_http.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/common/test_mcon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.208459 pycarlo-0.7.6/tests/features/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.208459 pycarlo-0.7.6/tests/features/circuit_breakers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/circuit_breakers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/circuit_breakers/test_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.208459 pycarlo-0.7.6/tests/features/dbt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/dbt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/dbt/sample_logs.txt
+-rw-r--r--   0 root         (0) root         (0)    16826 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/dbt/sample_manifest.json
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/dbt/sample_run_results.json
+-rw-r--r--   0 root         (0) root         (0)    15115 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/dbt/test_dbt_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.208459 pycarlo-0.7.6/tests/features/metadata/
+-rw-r--r--   0 root         (0) root         (0)    18130 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/metadata/test_dataset_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.212459 pycarlo-0.7.6/tests/features/pii/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.212459 pycarlo-0.7.6/tests/features/pii/sample_events/
+-rw-r--r--   0 root         (0) root         (0)  1638574 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/pii/sample_events/sample_md_events_01.json
+-rw-r--r--   0 root         (0) root         (0)   125065 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/pii/sample_events/sample_md_events_02.json
+-rw-r--r--   0 root         (0) root         (0)    11340 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/pii/test_pii_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.212459 pycarlo-0.7.6/tests/features/user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/features/user/test_user_service.py
+-rw-r--r--   0 root         (0) root         (0)    10305 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/test_operations.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/test_retry_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-06-14 13:35:06.000000 pycarlo-0.7.6/tests/test_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 13:35:23.212459 pycarlo-0.7.6/utils/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-06-14 13:35:06.000000 pycarlo-0.7.6/utils/env.sh
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-14 13:35:06.000000 pycarlo-0.7.6/utils/generate.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-14 13:35:06.000000 pycarlo-0.7.6/utils/sample.env
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-06-14 13:35:06.000000 pycarlo-0.7.6/utils/sanity.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-06-14 13:35:06.000000 pycarlo-0.7.6/utils/vars.py
```

### Comparing `pycarlo-0.7.5/.circleci/config.yml` & `pycarlo-0.7.6/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/.gitignore` & `pycarlo-0.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/LICENSE` & `pycarlo-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/Makefile` & `pycarlo-0.7.6/Makefile`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/PKG-INFO` & `pycarlo-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycarlo
-Version: 0.7.5
+Version: 0.7.6
 Summary: Monte Carlo's Python SDK
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pycarlo-0.7.5/README.md` & `pycarlo-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/examples/sample_insight_upload.py` & `pycarlo-0.7.6/examples/sample_insight_upload.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/__init__.py` & `pycarlo-0.7.6/pycarlo/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/errors.py` & `pycarlo-0.7.6/pycarlo/common/errors.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/files.py` & `pycarlo-0.7.6/pycarlo/common/files.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/http.py` & `pycarlo-0.7.6/pycarlo/common/http.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/mcon.py` & `pycarlo-0.7.6/pycarlo/common/mcon.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/retries.py` & `pycarlo-0.7.6/pycarlo/common/retries.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/settings.py` & `pycarlo-0.7.6/pycarlo/common/settings.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/common/utils.py` & `pycarlo-0.7.6/pycarlo/common/utils.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/core/client.py` & `pycarlo-0.7.6/pycarlo/core/client.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/core/endpoint.py` & `pycarlo-0.7.6/pycarlo/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/core/operations.py` & `pycarlo-0.7.6/pycarlo/core/operations.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/core/session.py` & `pycarlo-0.7.6/pycarlo/core/session.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/circuit_breakers/service.py` & `pycarlo-0.7.6/pycarlo/features/circuit_breakers/service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/dbt/dbt_importer.py` & `pycarlo-0.7.6/pycarlo/features/dbt/dbt_importer.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/dbt/queries.py` & `pycarlo-0.7.6/pycarlo/features/dbt/queries.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/metadata/allow_block_list.py` & `pycarlo-0.7.6/pycarlo/features/metadata/allow_block_list.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/metadata/metadata_filters_container.py` & `pycarlo-0.7.6/pycarlo/features/metadata/metadata_filters_container.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/pii/pii_filterer.py` & `pycarlo-0.7.6/pycarlo/features/pii/pii_filterer.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/pii/service.py` & `pycarlo-0.7.6/pycarlo/features/pii/service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/features/user/service.py` & `pycarlo-0.7.6/pycarlo/features/user/service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/lib/schema.json` & `pycarlo-0.7.6/pycarlo/lib/schema.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo/lib/schema.py` & `pycarlo-0.7.6/pycarlo/lib/schema.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/pycarlo.egg-info/PKG-INFO` & `pycarlo-0.7.6/pycarlo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycarlo
-Version: 0.7.5
+Version: 0.7.6
 Summary: Monte Carlo's Python SDK
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pycarlo-0.7.5/pycarlo.egg-info/SOURCES.txt` & `pycarlo-0.7.6/pycarlo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/setup.py` & `pycarlo-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/common/test_files.py` & `pycarlo-0.7.6/tests/common/test_files.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/common/test_http.py` & `pycarlo-0.7.6/tests/common/test_http.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/common/test_mcon.py` & `pycarlo-0.7.6/tests/common/test_mcon.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/circuit_breakers/test_service.py` & `pycarlo-0.7.6/tests/features/circuit_breakers/test_service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/dbt/sample_manifest.json` & `pycarlo-0.7.6/tests/features/dbt/sample_manifest.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/dbt/sample_run_results.json` & `pycarlo-0.7.6/tests/features/dbt/sample_run_results.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/dbt/test_dbt_importer.py` & `pycarlo-0.7.6/tests/features/dbt/test_dbt_importer.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/metadata/test_dataset_filtering.py` & `pycarlo-0.7.6/tests/features/metadata/test_dataset_filtering.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/pii/sample_events/sample_md_events_01.json` & `pycarlo-0.7.6/tests/features/pii/sample_events/sample_md_events_01.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/pii/sample_events/sample_md_events_02.json` & `pycarlo-0.7.6/tests/features/pii/sample_events/sample_md_events_02.json`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/pii/test_pii_filtering.py` & `pycarlo-0.7.6/tests/features/pii/test_pii_filtering.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/features/user/test_user_service.py` & `pycarlo-0.7.6/tests/features/user/test_user_service.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/test_client.py` & `pycarlo-0.7.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/test_operations.py` & `pycarlo-0.7.6/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/test_retry_decorator.py` & `pycarlo-0.7.6/tests/test_retry_decorator.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/tests/test_session.py` & `pycarlo-0.7.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/utils/env.sh` & `pycarlo-0.7.6/utils/env.sh`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/utils/generate.py` & `pycarlo-0.7.6/utils/generate.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/utils/sanity.py` & `pycarlo-0.7.6/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `pycarlo-0.7.5/utils/vars.py` & `pycarlo-0.7.6/utils/vars.py`

 * *Files identical despite different names*

