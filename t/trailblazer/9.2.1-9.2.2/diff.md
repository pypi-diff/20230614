# Comparing `tmp/trailblazer-9.2.1.tar.gz` & `tmp/trailblazer-9.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trailblazer-9.2.1.tar", last modified: Tue Jan 19 09:50:39 2021, max compression
+gzip compressed data, was "dist/trailblazer-9.2.2.tar", last modified: Tue Jan 19 09:54:22 2021, max compression
```

## Comparing `trailblazer-9.2.1.tar` & `trailblazer-9.2.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1057 2021-01-19 09:50:32.000000 trailblazer-9.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      177 2021-01-19 09:50:32.000000 trailblazer-9.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8141 2021-01-19 09:50:39.000000 trailblazer-9.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6247 2021-01-19 09:50:32.000000 trailblazer-9.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       31 2021-01-19 09:50:32.000000 trailblazer-9.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       72 2021-01-19 09:50:32.000000 trailblazer-9.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      316 2021-01-19 09:50:32.000000 trailblazer-9.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      117 2021-01-19 09:50:39.000000 trailblazer-9.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2591 2021-01-19 09:50:32.000000 trailblazer-9.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (116)     8444 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (116)     2680 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/tests/fixtures/case/
--rw-r--r--   0 runner    (1001) docker     (116)      101 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/case/blazinginsect_slurm_job_ids.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       98 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/case/crackpanda_slurm_job_ids.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       95 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/case/escapegoat_slurm_job_ids.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       93 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/case/lateraligator_slurm_job_ids.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       92 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/case/nicemice_slurm_job_ids.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/tests/fixtures/sacct/
--rw-r--r--   0 runner    (1001) docker     (116)      421 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/blazinginsect_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      223 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/broken_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      421 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/crackpanda_sacct
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/daringpidgeon_sacct
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/emptydinosaur_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/escapegoat_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      427 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/fancymole_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/happycow_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      473 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/lateraligator_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      417 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/liberatedunicorn_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      430 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/nicemice_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      430 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/rarekitten_sacct
--rw-r--r--   0 runner    (1001) docker     (116)      432 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sacct/trueferret_sacct
--rw-r--r--   0 runner    (1001) docker     (116)     4354 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/fixtures/sample-data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (116)     6576 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/store/test_store_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      323 2021-01-19 09:50:32.000000 trailblazer-9.2.1/tests/store/test_store_models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer/
--rw-r--r--   0 runner    (1001) docker     (116)      136 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer/cli/
--rw-r--r--   0 runner    (1001) docker     (116)       47 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5496 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (116)      600 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)      262 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/environ.py
--rw-r--r--   0 runner    (1001) docker     (116)      280 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer/server/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8728 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/server/api.py
--rw-r--r--   0 runner    (1001) docker     (116)      796 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/server/app.py
--rw-r--r--   0 runner    (1001) docker     (116)      207 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer/store/
--rw-r--r--   0 runner    (1001) docker     (116)       60 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17691 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/store/api.py
--rw-r--r--   0 runner    (1001) docker     (116)     2782 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer/store/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/store/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      401 2021-01-19 09:50:32.000000 trailblazer-9.2.1/trailblazer/store/utils/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8141 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1671 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       54 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      207 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-01-19 09:50:39.000000 trailblazer-9.2.1/trailblazer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/
+-rw-r--r--   0 runner    (1001) docker     (116)     1057 2021-01-19 09:54:14.000000 trailblazer-9.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      177 2021-01-19 09:54:14.000000 trailblazer-9.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8141 2021-01-19 09:54:22.000000 trailblazer-9.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6247 2021-01-19 09:54:14.000000 trailblazer-9.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       31 2021-01-19 09:54:14.000000 trailblazer-9.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       72 2021-01-19 09:54:14.000000 trailblazer-9.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      316 2021-01-19 09:54:14.000000 trailblazer-9.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      117 2021-01-19 09:54:22.000000 trailblazer-9.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2591 2021-01-19 09:54:14.000000 trailblazer-9.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)     8444 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2680 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/tests/fixtures/case/
+-rw-r--r--   0 runner    (1001) docker     (116)      101 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/case/blazinginsect_slurm_job_ids.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       98 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/case/crackpanda_slurm_job_ids.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       95 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/case/escapegoat_slurm_job_ids.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       93 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/case/lateraligator_slurm_job_ids.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       92 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/case/nicemice_slurm_job_ids.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/tests/fixtures/sacct/
+-rw-r--r--   0 runner    (1001) docker     (116)      421 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/blazinginsect_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      223 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/broken_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      421 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/crackpanda_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/daringpidgeon_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/emptydinosaur_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/escapegoat_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      427 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/fancymole_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/happycow_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      473 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/lateraligator_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      417 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/liberatedunicorn_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/nicemice_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/rarekitten_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)      432 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sacct/trueferret_sacct
+-rw-r--r--   0 runner    (1001) docker     (116)     4354 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/fixtures/sample-data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (116)     6576 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/store/test_store_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      323 2021-01-19 09:54:14.000000 trailblazer-9.2.2/tests/store/test_store_models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer/
+-rw-r--r--   0 runner    (1001) docker     (116)      136 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5496 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (116)      600 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)      262 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/environ.py
+-rw-r--r--   0 runner    (1001) docker     (116)      280 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer/server/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8728 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      796 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (116)      207 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer/store/
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17691 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/store/api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2782 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer/store/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/store/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      401 2021-01-19 09:54:14.000000 trailblazer-9.2.2/trailblazer/store/utils/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8141 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1671 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       54 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      207 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2021-01-19 09:54:22.000000 trailblazer-9.2.2/trailblazer.egg-info/top_level.txt
```

### Comparing `trailblazer-9.2.1/LICENSE` & `trailblazer-9.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/PKG-INFO` & `trailblazer-9.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailblazer
-Version: 9.2.1
+Version: 9.2.2
 Summary: Trailblazer is a tool to manage and track state of analyses
 Home-page: https://github.com/Clinical-Genomics/trailblazer
 Author: henrik.stranneheim
 Author-email: henrik.stranneheim@scilifelab.se
 License: MIT
 Description: 
         # Trailblazer [![Coverage Status][coveralls-image]][coveralls-url]
```

### Comparing `trailblazer-9.2.1/README.md` & `trailblazer-9.2.2/README.md`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/setup.py` & `trailblazer-9.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 
 setup(
     name=NAME,
-    version="9.2.1",
+    version="9.2.2",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="analysis monitoring",
     author=AUTHOR,
     author_email=EMAIL,
     license="MIT",
```

### Comparing `trailblazer-9.2.1/tests/cli/test_cli_core.py` & `trailblazer-9.2.2/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/tests/conftest.py` & `trailblazer-9.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/tests/fixtures/sample-data.yaml` & `trailblazer-9.2.2/tests/fixtures/sample-data.yaml`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/tests/store/test_store_api.py` & `trailblazer-9.2.2/tests/store/test_store_api.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/trailblazer/cli/core.py` & `trailblazer-9.2.2/trailblazer/cli/core.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/trailblazer/constants.py` & `trailblazer-9.2.2/trailblazer/constants.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/trailblazer/server/api.py` & `trailblazer-9.2.2/trailblazer/server/api.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/trailblazer/server/app.py` & `trailblazer-9.2.2/trailblazer/server/app.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/trailblazer/store/api.py` & `trailblazer-9.2.2/trailblazer/store/api.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/trailblazer/store/models.py` & `trailblazer-9.2.2/trailblazer/store/models.py`

 * *Files identical despite different names*

### Comparing `trailblazer-9.2.1/trailblazer.egg-info/PKG-INFO` & `trailblazer-9.2.2/trailblazer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailblazer
-Version: 9.2.1
+Version: 9.2.2
 Summary: Trailblazer is a tool to manage and track state of analyses
 Home-page: https://github.com/Clinical-Genomics/trailblazer
 Author: henrik.stranneheim
 Author-email: henrik.stranneheim@scilifelab.se
 License: MIT
 Description: 
         # Trailblazer [![Coverage Status][coveralls-image]][coveralls-url]
```

### Comparing `trailblazer-9.2.1/trailblazer.egg-info/SOURCES.txt` & `trailblazer-9.2.2/trailblazer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

