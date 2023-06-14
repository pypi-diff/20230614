# Comparing `tmp/spyctl-0.9.8.tar.gz` & `tmp/spyctl-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyctl-0.9.8.tar", last modified: Fri Jan 27 22:22:40 2023, max compression
+gzip compressed data, was "spyctl-0.9.9.tar", last modified: Mon Jan 30 18:22:13 2023, max compression
```

## Comparing `spyctl-0.9.8.tar` & `spyctl-0.9.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.425929 spyctl-0.9.8/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)       38 2023-01-27 22:22:20.000000 spyctl-0.9.8/.flake8
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.375930 spyctl-0.9.8/.github/
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.385930 spyctl-0.9.8/.github/workflows/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      239 2023-01-25 16:23:37.000000 spyctl-0.9.8/.github/workflows/black.yml
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1279 2023-01-25 16:23:37.000000 spyctl-0.9.8/.github/workflows/python-package.yml
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)       45 2023-01-20 16:20:03.000000 spyctl-0.9.8/.gitignore
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    11357 2023-01-11 15:13:43.000000 spyctl-0.9.8/LICENSE
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      484 2023-01-11 20:00:46.000000 spyctl-0.9.8/Makefile
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15017 2023-01-27 22:22:40.425929 spyctl-0.9.8/PKG-INFO
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1245 2023-01-11 19:50:22.000000 spyctl-0.9.8/README.md
--rwxr-xr-x   0 brhaub    (1000) brhaub    (1000)      324 2023-01-09 15:25:40.000000 spyctl-0.9.8/cmdline_test.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.395930 spyctl-0.9.8/docs/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      634 2023-01-11 15:13:43.000000 spyctl-0.9.8/docs/Makefile
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.395930 spyctl-0.9.8/docs/_static/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    14074 2023-01-27 22:22:20.000000 spyctl-0.9.8/docs/_static/sb-logo-sidebar.png
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    35777 2023-01-27 22:22:20.000000 spyctl-0.9.8/docs/_static/sb-logo.png
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1292 2023-01-27 22:22:20.000000 spyctl-0.9.8/docs/conf.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.395930 spyctl-0.9.8/docs/getting_started/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      240 2023-01-11 15:13:43.000000 spyctl-0.9.8/docs/getting_started/getting_started.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     2333 2023-01-17 19:49:40.000000 spyctl-0.9.8/docs/getting_started/install.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1372 2023-01-13 21:32:02.000000 spyctl-0.9.8/docs/index.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      800 2023-01-11 15:13:43.000000 spyctl-0.9.8/docs/make.bat
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)       99 2023-01-20 16:20:03.000000 spyctl-0.9.8/docs/requirements.txt
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.395930 spyctl-0.9.8/docs/tutorials/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    13912 2023-01-20 16:20:03.000000 spyctl-0.9.8/docs/tutorials/policy_management.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15415 2023-01-17 19:49:40.000000 spyctl-0.9.8/docs/tutorials/spyctl_basics.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      359 2023-01-11 15:13:43.000000 spyctl-0.9.8/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.395930 spyctl-0.9.8/docs/user/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      265 2023-01-20 16:20:03.000000 spyctl-0.9.8/docs/user/commands.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      127 2023-01-17 19:49:40.000000 spyctl-0.9.8/docs/user/configuration.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1189 2023-01-13 21:32:02.000000 spyctl-0.9.8/docs/user/resources.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1107 2023-01-12 20:49:43.000000 spyctl-0.9.8/docs/user/spyderbat_concepts.rst
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1221 2023-01-27 22:22:20.000000 spyctl-0.9.8/pyproject.toml
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)       38 2023-01-27 22:22:40.425929 spyctl-0.9.8/setup.cfg
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.405930 spyctl-0.9.8/spyctl/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2022-11-23 15:16:31.000000 spyctl-0.9.8/spyctl/__init__.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    12268 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/api.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.405930 spyctl-0.9.8/spyctl/archive/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    21283 2022-12-15 14:59:39.000000 spyctl-0.9.8/spyctl/archive/old_args.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    17397 2023-01-13 21:32:02.000000 spyctl-0.9.8/spyctl/archive/old_merge.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     4402 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/cli.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.415930 spyctl-0.9.8/spyctl/commands/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-20 16:20:03.000000 spyctl-0.9.8/spyctl/commands/__init__.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1047 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/commands/apply.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      614 2023-01-13 21:32:02.000000 spyctl-0.9.8/spyctl/commands/create.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1162 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/commands/delete.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      935 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/commands/diff.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     7709 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/commands/get.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      999 2023-01-13 21:32:02.000000 spyctl-0.9.8/spyctl/commands/merge.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      221 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/commands/validate.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.415930 spyctl-0.9.8/spyctl/config/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-20 16:20:03.000000 spyctl-0.9.8/spyctl/config/__init__.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    26325 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/config/configs.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    13361 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/config/secrets.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    13762 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/filter_resource.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    66471 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/merge_lib.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.425929 spyctl-0.9.8/spyctl/resources/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-20 16:20:03.000000 spyctl-0.9.8/spyctl/resources/__init__.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     7488 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/resources/baselines.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      922 2022-12-14 23:54:46.000000 spyctl-0.9.8/spyctl/resources/clusters.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15890 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/resources/fingerprints.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      868 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/resources/machines.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1272 2023-01-13 21:32:02.000000 spyctl-0.9.8/spyctl/resources/namespaces.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     3089 2023-01-13 21:32:02.000000 spyctl-0.9.8/spyctl/resources/pods.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     9692 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/resources/policies.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    18115 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/schemas.py
--rwxr-xr-x   0 brhaub    (1000) brhaub    (1000)    21440 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/spyctl.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    24440 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/spyctl_lib.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.425929 spyctl-0.9.8/spyctl/tests/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-20 16:20:03.000000 spyctl-0.9.8/spyctl/tests/__init__.py
--rwxr-xr-x   0 brhaub    (1000) brhaub    (1000)     7224 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/tests/test_commands.py
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    12660 2023-01-27 22:22:20.000000 spyctl-0.9.8/spyctl/tests/test_config.py
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.425929 spyctl-0.9.8/spyctl/tests/test_resources/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1959 2023-01-20 16:20:03.000000 spyctl-0.9.8/spyctl/tests/test_resources/test_baseline.yaml
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     4348 2023-01-20 16:20:03.000000 spyctl-0.9.8/spyctl/tests/test_resources/test_frpint_group.yaml
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-20 16:20:03.000000 spyctl-0.9.8/spyctl/tests/test_resources/test_policy.yaml
-drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:22:40.405930 spyctl-0.9.8/spyctl.egg-info/
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15017 2023-01-27 22:22:40.000000 spyctl-0.9.8/spyctl.egg-info/PKG-INFO
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1686 2023-01-27 22:22:40.000000 spyctl-0.9.8/spyctl.egg-info/SOURCES.txt
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        1 2023-01-27 22:22:40.000000 spyctl-0.9.8/spyctl.egg-info/dependency_links.txt
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)       46 2023-01-27 22:22:40.000000 spyctl-0.9.8/spyctl.egg-info/entry_points.txt
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)      122 2023-01-27 22:22:40.000000 spyctl-0.9.8/spyctl.egg-info/requires.txt
--rw-r--r--   0 brhaub    (1000) brhaub    (1000)        7 2023-01-27 22:22:40.000000 spyctl-0.9.8/spyctl.egg-info/top_level.txt
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.170305 spyctl-0.9.9/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)       38 2023-01-27 22:28:13.000000 spyctl-0.9.9/.flake8
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.000297 spyctl-0.9.9/.github/
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.070300 spyctl-0.9.9/.github/workflows/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      239 2023-01-27 22:28:13.000000 spyctl-0.9.9/.github/workflows/black.yml
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1279 2023-01-27 22:28:13.000000 spyctl-0.9.9/.github/workflows/python-package.yml
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)       45 2023-01-27 22:28:13.000000 spyctl-0.9.9/.gitignore
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    11357 2023-01-11 15:13:43.000000 spyctl-0.9.9/LICENSE
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      484 2023-01-11 20:00:46.000000 spyctl-0.9.9/Makefile
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15017 2023-01-30 18:22:13.170305 spyctl-0.9.9/PKG-INFO
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1245 2023-01-11 19:50:22.000000 spyctl-0.9.9/README.md
+-rwxr-xr-x   0 brhaub    (1000) brhaub    (1000)      324 2023-01-09 15:25:40.000000 spyctl-0.9.9/cmdline_test.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.070300 spyctl-0.9.9/docs/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      634 2023-01-11 15:13:43.000000 spyctl-0.9.9/docs/Makefile
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.090301 spyctl-0.9.9/docs/_static/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    14074 2023-01-27 22:28:13.000000 spyctl-0.9.9/docs/_static/sb-logo-sidebar.png
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    35777 2023-01-27 22:28:13.000000 spyctl-0.9.9/docs/_static/sb-logo.png
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1292 2023-01-30 18:21:49.000000 spyctl-0.9.9/docs/conf.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.090301 spyctl-0.9.9/docs/getting_started/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      240 2023-01-11 15:13:43.000000 spyctl-0.9.9/docs/getting_started/getting_started.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     2333 2023-01-17 19:49:40.000000 spyctl-0.9.9/docs/getting_started/install.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1372 2023-01-13 21:32:02.000000 spyctl-0.9.9/docs/index.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      800 2023-01-11 15:13:43.000000 spyctl-0.9.9/docs/make.bat
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)       99 2023-01-27 22:28:13.000000 spyctl-0.9.9/docs/requirements.txt
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.090301 spyctl-0.9.9/docs/tutorials/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    13912 2023-01-27 22:28:13.000000 spyctl-0.9.9/docs/tutorials/policy_management.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15415 2023-01-17 19:49:40.000000 spyctl-0.9.9/docs/tutorials/spyctl_basics.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      359 2023-01-11 15:13:43.000000 spyctl-0.9.9/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.090301 spyctl-0.9.9/docs/user/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      265 2023-01-30 18:04:58.000000 spyctl-0.9.9/docs/user/commands.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      127 2023-01-17 19:49:40.000000 spyctl-0.9.9/docs/user/configuration.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1189 2023-01-13 21:32:02.000000 spyctl-0.9.9/docs/user/resources.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1107 2023-01-12 20:49:43.000000 spyctl-0.9.9/docs/user/spyderbat_concepts.rst
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1221 2023-01-30 18:21:49.000000 spyctl-0.9.9/pyproject.toml
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)       38 2023-01-30 18:22:13.170305 spyctl-0.9.9/setup.cfg
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.110302 spyctl-0.9.9/spyctl/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2022-11-23 15:16:31.000000 spyctl-0.9.9/spyctl/__init__.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    12268 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/api.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.110302 spyctl-0.9.9/spyctl/archive/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    21283 2022-12-15 14:59:39.000000 spyctl-0.9.9/spyctl/archive/old_args.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    17397 2023-01-13 21:32:02.000000 spyctl-0.9.9/spyctl/archive/old_merge.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     4061 2023-01-30 18:21:49.000000 spyctl-0.9.9/spyctl/cli.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.120302 spyctl-0.9.9/spyctl/commands/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/commands/__init__.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1047 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/commands/apply.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      614 2023-01-13 21:32:02.000000 spyctl-0.9.9/spyctl/commands/create.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1162 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/commands/delete.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      935 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/commands/diff.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     7709 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/commands/get.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      999 2023-01-13 21:32:02.000000 spyctl-0.9.9/spyctl/commands/merge.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      221 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/commands/validate.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.130303 spyctl-0.9.9/spyctl/config/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/config/__init__.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    26325 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/config/configs.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    13361 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/config/secrets.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    13762 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/filter_resource.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    66471 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/merge_lib.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.150304 spyctl-0.9.9/spyctl/resources/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/resources/__init__.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     7488 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/resources/baselines.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      922 2022-12-14 23:54:46.000000 spyctl-0.9.9/spyctl/resources/clusters.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15890 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/resources/fingerprints.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      868 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/resources/machines.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1272 2023-01-13 21:32:02.000000 spyctl-0.9.9/spyctl/resources/namespaces.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     3089 2023-01-13 21:32:02.000000 spyctl-0.9.9/spyctl/resources/pods.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     9692 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/resources/policies.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    18115 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/schemas.py
+-rwxr-xr-x   0 brhaub    (1000) brhaub    (1000)    21440 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/spyctl.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    24640 2023-01-30 18:21:49.000000 spyctl-0.9.9/spyctl/spyctl_lib.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.150304 spyctl-0.9.9/spyctl/tests/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/tests/__init__.py
+-rwxr-xr-x   0 brhaub    (1000) brhaub    (1000)     7224 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/tests/test_commands.py
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    12660 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/tests/test_config.py
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.160304 spyctl-0.9.9/spyctl/tests/test_resources/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1959 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/tests/test_resources/test_baseline.yaml
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     4348 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/tests/test_resources/test_frpint_group.yaml
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        0 2023-01-27 22:28:13.000000 spyctl-0.9.9/spyctl/tests/test_resources/test_policy.yaml
+drwxr-xr-x   0 brhaub    (1000) brhaub    (1000)        0 2023-01-30 18:22:13.110302 spyctl-0.9.9/spyctl.egg-info/
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)    15017 2023-01-30 18:22:12.000000 spyctl-0.9.9/spyctl.egg-info/PKG-INFO
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)     1686 2023-01-30 18:22:12.000000 spyctl-0.9.9/spyctl.egg-info/SOURCES.txt
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        1 2023-01-30 18:22:12.000000 spyctl-0.9.9/spyctl.egg-info/dependency_links.txt
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)       46 2023-01-30 18:22:12.000000 spyctl-0.9.9/spyctl.egg-info/entry_points.txt
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)      122 2023-01-30 18:22:12.000000 spyctl-0.9.9/spyctl.egg-info/requires.txt
+-rw-r--r--   0 brhaub    (1000) brhaub    (1000)        7 2023-01-30 18:22:12.000000 spyctl-0.9.9/spyctl.egg-info/top_level.txt
```

### Comparing `spyctl-0.9.8/.github/workflows/python-package.yml` & `spyctl-0.9.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/LICENSE` & `spyctl-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/PKG-INFO` & `spyctl-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyctl
-Version: 0.9.8
+Version: 0.9.9
 Summary: A command line tool for viewing and managing Spyderbat Resources
 Author-email: Brent Haub <dev@spyderbat.com>, Kyle Smith Hanna <dev@spyderbat.com>
 Maintainer-email: Brent Haub <dev@spyderbat.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `spyctl-0.9.8/README.md` & `spyctl-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/Makefile` & `spyctl-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/_static/sb-logo-sidebar.png` & `spyctl-0.9.9/docs/_static/sb-logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/_static/sb-logo.png` & `spyctl-0.9.9/docs/_static/sb-logo.png`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/conf.py` & `spyctl-0.9.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "Spyctl"
 copyright = "2023, SPYDERBAT, Inc., All Rights Reserved"
 author = "Spyderbat"
 release = "0.9"
-version = "0.9.8"
+version = "0.9.9"
 
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.duration",
```

### Comparing `spyctl-0.9.8/docs/getting_started/install.rst` & `spyctl-0.9.9/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/index.rst` & `spyctl-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/make.bat` & `spyctl-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/tutorials/policy_management.rst` & `spyctl-0.9.9/docs/tutorials/policy_management.rst`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/tutorials/spyctl_basics.rst` & `spyctl-0.9.9/docs/tutorials/spyctl_basics.rst`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/user/resources.rst` & `spyctl-0.9.9/docs/user/resources.rst`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/docs/user/spyderbat_concepts.rst` & `spyctl-0.9.9/docs/user/spyderbat_concepts.rst`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/pyproject.toml` & `spyctl-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spyctl"
-version = "0.9.8"
+version = "0.9.9"
 
 description = "A command line tool for viewing and managing Spyderbat Resources"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["spyctl", "spyderbat", "kubectl", "kubernetes"]
 authors = [
```

### Comparing `spyctl-0.9.8/spyctl/api.py` & `spyctl-0.9.9/spyctl/api.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/archive/old_args.py` & `spyctl-0.9.9/spyctl/archive/old_args.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/archive/old_merge.py` & `spyctl-0.9.9/spyctl/archive/old_merge.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/cli.py` & `spyctl-0.9.9/spyctl/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,15 @@
 
 WARNING_MSG = "is_warning"
 WARNING_COLOR = lib.WARNING_COLOR
 COLOR_END = lib.COLOR_END
 
 
 def try_log(*args, **kwargs):
-    try:
-        if kwargs.pop(WARNING_MSG, False):
-            msg = f"{WARNING_COLOR}{' '.join(args)}{COLOR_END}"
-            print(msg, **kwargs, file=sys.stderr)
-        else:
-            print(*args, **kwargs, file=sys.stderr)
-        sys.stderr.flush()
-    except BrokenPipeError:
-        devnull = os.open(os.devnull, os.O_WRONLY)
-        os.dup2(devnull, sys.stderr.fileno())
-        sys.exit(1)
+    lib.try_log(*args, **kwargs)
 
 
 def try_print(*args, **kwargs):
     try:
         print(*args, **kwargs)
         sys.stdout.flush()
     except BrokenPipeError:
@@ -150,8 +140,9 @@
             err_exit("start time was before end time")
         return tuple(args.time_range)
     else:
         t = args.time if args.time else time.time()
         return t, t
 
 
-err_exit = lib.err_exit
+def err_exit(message: str):
+    lib.err_exit(message)
```

### Comparing `spyctl-0.9.8/spyctl/commands/apply.py` & `spyctl-0.9.9/spyctl/commands/apply.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/commands/create.py` & `spyctl-0.9.9/spyctl/commands/create.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/commands/delete.py` & `spyctl-0.9.9/spyctl/commands/delete.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/commands/diff.py` & `spyctl-0.9.9/spyctl/commands/diff.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/commands/get.py` & `spyctl-0.9.9/spyctl/commands/get.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/commands/merge.py` & `spyctl-0.9.9/spyctl/commands/merge.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/config/configs.py` & `spyctl-0.9.9/spyctl/config/configs.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/config/secrets.py` & `spyctl-0.9.9/spyctl/config/secrets.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/filter_resource.py` & `spyctl-0.9.9/spyctl/filter_resource.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/merge_lib.py` & `spyctl-0.9.9/spyctl/merge_lib.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/resources/baselines.py` & `spyctl-0.9.9/spyctl/resources/baselines.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/resources/clusters.py` & `spyctl-0.9.9/spyctl/resources/clusters.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/resources/fingerprints.py` & `spyctl-0.9.9/spyctl/resources/fingerprints.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/resources/machines.py` & `spyctl-0.9.9/spyctl/resources/machines.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/resources/namespaces.py` & `spyctl-0.9.9/spyctl/resources/namespaces.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/resources/pods.py` & `spyctl-0.9.9/spyctl/resources/pods.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/resources/policies.py` & `spyctl-0.9.9/spyctl/resources/policies.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/schemas.py` & `spyctl-0.9.9/spyctl/schemas.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/spyctl.py` & `spyctl-0.9.9/spyctl/spyctl.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/spyctl_lib.py` & `spyctl-0.9.9/spyctl/spyctl_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 
     def __eq__(self, __o: object) -> bool:
         plural_match = __o == self.name_plural if self.name_plural else False
         return __o in self.aliases or __o == self.name or plural_match
 
 
 APP_NAME = "spyctl"
+WARNING_MSG = "is_warning"
+WARNING_COLOR = "\033[38;5;203m"
+COLOR_END = "\033[0m"
 
 # Resource Aliases
 CLUSTERS_RESOURCE = Aliases(
     ["clusters", "cluster", "clust", "clusts", "clus"], "cluster", "clusters"
 )
 BASELINES_RESOURCE = Aliases(
     [
@@ -645,15 +648,19 @@
             epilog = inspect.cleandoc(self.epilog)
             formatter.write_paragraph()
             formatter.write_text(epilog)
 
 
 def try_log(*args, **kwargs):
     try:
-        print(*args, **kwargs, file=sys.stderr)
+        if kwargs.pop(WARNING_MSG, False):
+            msg = f"{WARNING_COLOR}{' '.join(args)}{COLOR_END}"
+            print(msg, **kwargs, file=sys.stderr)
+        else:
+            print(*args, **kwargs, file=sys.stderr)
         sys.stderr.flush()
     except BrokenPipeError:
         devnull = os.open(os.devnull, os.O_WRONLY)
         os.dup2(devnull, sys.stderr.fileno())
         sys.exit(1)
 
 
@@ -723,18 +730,14 @@
     return rv
 
 
 def make_uuid():
     return b64url(uuid4().bytes).decode("ascii").strip("=")
 
 
-WARNING_COLOR = "\033[38;5;203m"
-COLOR_END = "\033[0m"
-
-
 def err_exit(message: str):
     sys.exit(f"{WARNING_COLOR}Error: {message}{COLOR_END}")
 
 
 def dict_raise_on_duplicates(ordered_pairs):
     """Reject duplicate keys.
```

### Comparing `spyctl-0.9.8/spyctl/tests/test_commands.py` & `spyctl-0.9.9/spyctl/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/tests/test_config.py` & `spyctl-0.9.9/spyctl/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/tests/test_resources/test_baseline.yaml` & `spyctl-0.9.9/spyctl/tests/test_resources/test_baseline.yaml`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl/tests/test_resources/test_frpint_group.yaml` & `spyctl-0.9.9/spyctl/tests/test_resources/test_frpint_group.yaml`

 * *Files identical despite different names*

### Comparing `spyctl-0.9.8/spyctl.egg-info/PKG-INFO` & `spyctl-0.9.9/spyctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyctl
-Version: 0.9.8
+Version: 0.9.9
 Summary: A command line tool for viewing and managing Spyderbat Resources
 Author-email: Brent Haub <dev@spyderbat.com>, Kyle Smith Hanna <dev@spyderbat.com>
 Maintainer-email: Brent Haub <dev@spyderbat.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `spyctl-0.9.8/spyctl.egg-info/SOURCES.txt` & `spyctl-0.9.9/spyctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

