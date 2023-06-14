# Comparing `tmp/dls-bxflow-2.4.2.tar.gz` & `tmp/dls-bxflow-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-bxflow-2.4.2.tar", last modified: Tue May 30 18:22:56 2023, max compression
+gzip compressed data, was "dls-bxflow-2.5.0.tar", last modified: Wed Jun 14 04:47:16 2023, max compression
```

## Comparing `dls-bxflow-2.4.2.tar` & `dls-bxflow-2.5.0.tar`

### file list

```diff
@@ -1,444 +1,445 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.769602 dls-bxflow-2.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.717602 dls-bxflow-2.4.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-30 18:22:56.769602 dls-bxflow-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.717602 dls-bxflow-2.4.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/explanations/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:22:56.769602 dls-bxflow-2.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.721602 dls-bxflow-2.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/src/dls_bxflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-30 18:22:56.000000 dls-bxflow-2.4.2/src/dls_bxflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-05-30 18:22:56.000000 dls-bxflow-2.4.2/src/dls_bxflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:22:56.000000 dls-bxflow-2.4.2/src/dls_bxflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 18:22:56.000000 dls-bxflow-2.4.2/src/dls_bxflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-30 18:22:56.000000 dls-bxflow-2.4.2/src/dls_bxflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 18:22:56.000000 dls-bxflow-2.4.2/src/dls_bxflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/src/dls_bxflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.729602 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_api/remex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.733602 dls-bxflow-2.4.2/src/dls_bxflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.733602 dls-bxflow-2.4.2/src/dls_bxflow_cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/contexts/dataface_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/contexts/filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/contexts/news_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.733602 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/execute_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/find_xanes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/fire_i22.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/recipe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/report_dcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/report_ispyb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.733602 dls-bxflow-2.4.2/src/dls_bxflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 18:22:56.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.733602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/ispyb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.737602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/gdascan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.737602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/bx_composers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.737602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_configurators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.737602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/classic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.737602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24323 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_databases/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_databases/bx_databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.737602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30122 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/news_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.737602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/scandir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_gamls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_gamls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_gamls/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_gamls/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40198 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/bx_guis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/curses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.741602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.745602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.721602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.745602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.721602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.745602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.721602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.745602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.745602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.745602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.745602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.749602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24679 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/island.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/popener.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/qsubber.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.749602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/graylogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.749602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/bx_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.749602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/zocalo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.749602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/bx_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.753602 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.753602 dls-bxflow-2.4.2/src/dls_bxflow_lib/dummies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/dummies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/dummies/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.753602 dls-bxflow-2.4.2/src/dls_bxflow_lib/recipe_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/recipe_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/recipe_parser/overall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/recipe_parser/parser1.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.753602 dls-bxflow-2.4.2/src/dls_bxflow_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.753602 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/bx_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.757602 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/bx_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dawn_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/execution_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/filename_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/module_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/pickled_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/symlink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.757602 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_variables/bx_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_variables/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/bx_variables/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/src/dls_bxflow_run/main_isolated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.761602 dls-bxflow-2.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.761602 dls-bxflow-2.4.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/configurations/backend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/configurations/filestore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/configurations/ispyb-local.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.761602 dls-bxflow-2.4.2/tests/configurations/ptypy_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.761602 dls-bxflow-2.4.2/tests/configurations/ptyrex_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/configurations/ptyrex_configfiles/region_p4_p6.json
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/datafiles/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/datafiles/dawn2_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.725602 dls-bxflow-2.4.2/tests/datafiles/gaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/datafiles/gaml/workflow1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/datafiles/gaml/workflow1/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/datafiles/gaml/workflow2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/datafiles/gaml/workflow2/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/datafiles/i22-4996.nxs
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/gda_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/gda_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/jupyter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/jupyter/execute.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/jupyter/jupyter1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/jupyter/jupyter2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/jupyter/jupyter_bad_cell.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/jupyter/random_string.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/notebooks/c.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)     1800 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/qacct
--rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/qstat
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/qsub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/stub_commands/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/stub_commands/dawn
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/stub_commands/mpirun
--rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/stub_commands/ptychotools.ptypy_mpi_recipe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_collector_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_dataface_revision5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_extract_error_lines_dawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_extract_error_lines_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_gaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_job_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_job_a_bc_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_job_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_job_pubcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_job_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_launcher_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_launcher_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_launcher_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_launcher_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_logstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_protocolj.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_scheduler_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/test_workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/workflows/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/a/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/workflows/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/b/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/workflows/c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/c/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/workflows/e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/e/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.765602 dls-bxflow-2.4.2/tests/workflows/f/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/f/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/f/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:56.769602 dls-bxflow-2.4.2/tests/workflows/g/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/g/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 18:22:46.000000 dls-bxflow-2.4.2/tests/workflows/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.371026 dls-bxflow-2.5.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.359026 dls-bxflow-2.5.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.359026 dls-bxflow-2.5.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_launchers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/remex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.387026 dls-bxflow-2.5.0/src/dls_bxflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.387026 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/dataface_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/news_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.387026 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/execute_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/find_xanes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/fire_i22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/recipe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_dcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_ispyb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.391026 dls-bxflow-2.5.0/src/dls_bxflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.391026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.391026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gdascan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/bx_composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/classic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24323 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/bx_databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30122 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/scandir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40198 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/bx_guis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/curses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24839 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/island.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/popener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/qsubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/slurmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/graylogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/bx_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/bx_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19775 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/overall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/parser1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.415026 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/bx_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.415026 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/execution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/filename_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/module_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/pickled_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/symlink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.415026 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/bx_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/main_isolated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/backend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/filestore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/ispyb-local.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/configurations/ptypy_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/configurations/ptyrex_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/dawn2_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.371026 dls-bxflow-2.5.0/tests/datafiles/gaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow1/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow2/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/i22-4996.nxs
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/gda_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/gda_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/jupyter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/execute.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/jupyter1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/jupyter2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/jupyter_bad_cell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/random_string.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/notebooks/c.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/stub_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/dawn
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/mpirun
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/qstat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/qsub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_collector_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dataface_revision5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_extract_error_lines_dawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_extract_error_lines_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_gaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_a_bc_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_pubcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_logstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_protocolj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_ptyrex_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_scheduler_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/a/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/b/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/c/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/e/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/f/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/f/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/f/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/tests/workflows/g/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/g/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/utilities.py
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/Makefile` & `dls-bxflow-2.5.0/.dae-devops/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint e6429d30b68cdf1d9bf59cd6ba82a897
+# dae_devops_fingerprint da37516b8f7bcbfeb9885a49c08b1e85
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/docs/conventions.rst` & `dls-bxflow-2.5.0/.dae-devops/docs/conventions.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 .. # ********** For repository_name dls-bxflow
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint 9d64e1bb797ab206899b7140463b1ffa
+.. # dae_devops_fingerprint 1fe857971e77142a36a37997051a7289
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/docs/developing.rst` & `dls-bxflow-2.5.0/.dae-devops/docs/developing.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 .. # ********** For repository_name dls-bxflow
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
@@ -24,8 +24,8 @@
 
     $ cd dls-bxflow
     $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
 
-.. # dae_devops_fingerprint b43f9e92eb02335baa66fc0122af159e
+.. # dae_devops_fingerprint 4b6f21ffa82227a90036da2ba46aaedb
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/docs/devops.rst` & `dls-bxflow-2.5.0/.dae-devops/docs/devops.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 .. # ********** For repository_name dls-bxflow
 
 Devops
 =======================================================================
 
 In the top level of the repository there exists a configuration file called ``.dae-devops/project.yaml``.
 
@@ -40,8 +40,8 @@
 Publishing (for the Diamond intranet)::
 
     $ make -f .dae-devops/Makefile publish_pip
     $ make -f .dae-devops/Makefile publish_docs
     
 The Diamond intranet commands are not used for production. The production packaging and publishing are handled in the GitHub Actions workflows mechanism.
 
-.. # dae_devops_fingerprint 0bdf01a58645f01f7153360f52c5d06f
+.. # dae_devops_fingerprint 8d6b0f96c36b5d913fa0074fc843ec5f
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/docs/documenting.rst` & `dls-bxflow-2.5.0/.dae-devops/docs/documenting.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 .. # ********** For repository_name dls-bxflow
 
 Documenting
 =======================================================================
 
 If you plan to make update the documentation in this repository, you can use the steps below.
 
@@ -23,8 +23,8 @@
     file:///<your development area>/dls-bxflow/build/html/index.html
 
 When you push either the main branch or a tag to GitHub, the documents are built and published automatically to this url::
 
     https://diamondlightsource.github.io/dls-bxflow/main/index.html
 
 
-.. # dae_devops_fingerprint 9fba7a454042706a32f08bd2fd4fcce3
+.. # dae_devops_fingerprint 0c8114d3b93fa74e80958882b45a6957
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/docs/installing.rst` & `dls-bxflow-2.5.0/.dae-devops/docs/installing.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 .. # ********** For repository_name dls-bxflow
 
 Installing
 =======================================================================
 
 
 You will need python 3.10 or later. 
@@ -35,8 +35,8 @@
 
 The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-bxflow --version
     $ dls-bxflow --version-json
 
-.. # dae_devops_fingerprint 8ccbf8988522125959e98a89c3955b2f
+.. # dae_devops_fingerprint 274dbcfedd4feea41d06ffaab3fc4b25
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/docs/testing.rst` & `dls-bxflow-2.5.0/.dae-devops/docs/testing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 .. # ********** For repository_name dls-bxflow
 
 Testing
 =======================================================================
 
 The package uses pytest for unit testing.
 
@@ -27,8 +27,8 @@
 
 The tests clear their directory when they start, but not when they finish.
 This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint 58ccb8ff8aa55ed529e1d7942f96bd3c
+.. # dae_devops_fingerprint 2afce2f25b27f584270a1f93218bce37
```

### Comparing `dls-bxflow-2.4.2/.dae-devops/project.yaml` & `dls-bxflow-2.5.0/.dae-devops/project.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         - aio-pika
         - dask[distributed]
         - dls-servbase
         - dls-mainiac
         - dls-multiconf
         - dls-utilpack
         - dls-pairstream
+        - dls-slurmjob
         - future
         - graypy
         - h5py
         # There is a newer version 7 of ispyb but it doesn't support the import ispyb.model.__future__.
         # TODO: Change away from using import ispyb.model.__future__.
         - ispyb==6.13.0
         - ipykernel
```

### Comparing `dls-bxflow-2.4.2/.devcontainer/Dockerfile` & `dls-bxflow-2.5.0/.devcontainer/Dockerfile`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-bxflow"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 4b16385a09d58128346881a6b53ef58a
+# dae_devops_fingerprint 2987054ae9b53ba099e0e37774e6fb46
```

### Comparing `dls-bxflow-2.4.2/.devcontainer/devcontainer.json` & `dls-bxflow-2.5.0/.devcontainer/devcontainer.json`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+// ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 // ********** For repository_name dls-bxflow
 
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "Dockerfile",
@@ -53,8 +53,8 @@
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
     "postCreateCommand": "pip install -e .[dev]"
 }
 
-// dae_devops_fingerprint 8ee55efb6c475521fa40db01bb2eb177
+// dae_devops_fingerprint 5ebaaca7d58787f31793553084e238d1
```

### Comparing `dls-bxflow-2.4.2/.github/CONTRIBUTING.rst` & `dls-bxflow-2.5.0/.github/CONTRIBUTING.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 .. # ********** For repository_name dls-bxflow
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-bxflow/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 12687dadc26b00ae0ff61a410a4e6ff1
+.. # dae_devops_fingerprint 64a480c612412a8e9973d9fa32679061
```

### Comparing `dls-bxflow-2.4.2/.github/actions/install_requirements/action.yml` & `dls-bxflow-2.5.0/.github/actions/install_requirements/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 name: Install requirements
 description: Run pip install with requirements and upload resulting requirements
 inputs:
   requirements_file:
     description: Name of requirements file to use and upload
@@ -57,8 +57,8 @@
             echo "Error: ${{ inputs.requirements_file }} need the above changes to be exhaustive"
             exit 1
           fi
         fi
       shell: bash
 
 
-# dae_devops_fingerprint a5800c88a9ba24077377747d0c06fb25
+# dae_devops_fingerprint eb5296912f183adb712ebeace6d7ab4b
```

### Comparing `dls-bxflow-2.4.2/.github/dependabot.yml` & `dls-bxflow-2.5.0/.github/dependabot.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 # To get started with Dependabot version updates, you'll need to specify which
 # package ecosystems to update and where the package manifests are located.
 # Please see the documentation for all configuration options:
 # https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates
 
@@ -15,8 +15,8 @@
       interval: "weekly"
 
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
       interval: "weekly"
 
-# dae_devops_fingerprint 3e961ff662b90c708fef894a672a209d
+# dae_devops_fingerprint d3c68a555c6ee16924961d36cbfdde35
```

### Comparing `dls-bxflow-2.4.2/.github/pages/index.html` & `dls-bxflow-2.5.0/.github/pages/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!-- ********** Please don't edit this file! -->
-<!-- ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527. -->
+<!-- ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608. -->
 <!-- ********** For repository_name dls-bxflow -->
 
 <!DOCTYPE html>
 <html>
 
 <head>
     <title>Redirecting to main branch</title>
     <meta charset="utf-8">
     <meta http-equiv="refresh" content="0; url=./main/index.html">
     <link rel="canonical" href="main/index.html">
 </head>
 
 </html>
 
-<!-- dae_devops_fingerprint 5edcc0cfa9d05ece0c7ed1b015fad825 -->
+<!-- dae_devops_fingerprint b0a85e8cb19199869260cf27a7800d11 -->
```

### Comparing `dls-bxflow-2.4.2/.github/pages/make_switcher.py` & `dls-bxflow-2.5.0/.github/pages/make_switcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
@@ -98,8 +98,8 @@
     versions = get_versions("origin/gh-pages", args.add, args.remove)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
 
-# dae_devops_fingerprint d522d9d0c207340dbb11712b0fc3a203
+# dae_devops_fingerprint c85d7f049c7523f9efec55b5ec2d2698
```

### Comparing `dls-bxflow-2.4.2/.github/workflows/code.yml` & `dls-bxflow-2.5.0/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -207,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint 76b2b7d9457d45b8ee28d0cfc2a4c3df
+# dae_devops_fingerprint 5e01d2d3265331751a95a292afbd47ef
```

### Comparing `dls-bxflow-2.4.2/.github/workflows/docs.yml` & `dls-bxflow-2.5.0/.github/workflows/docs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 name: Docs CI
 
 on:
   push:
   pull_request:
@@ -52,8 +52,8 @@
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
         uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
 
-# dae_devops_fingerprint 2fe29e6e6518358f37cbab02c9e4e875
+# dae_devops_fingerprint d21dd6a115b3fbff73a11f5105dfe32d
```

### Comparing `dls-bxflow-2.4.2/.github/workflows/docs_clean.yml` & `dls-bxflow-2.5.0/.github/workflows/docs_clean.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 name: Docs Cleanup CI
 
 # delete branch documentation when a branch is deleted
 # also allow manually deleting a documentation version
 on:
@@ -42,8 +42,8 @@
           rm -r $DOCS_VERSION
           python make_switcher.py --remove $DOCS_VERSION ${{ github.repository }} switcher.json
           git config --global user.name 'GitHub Actions Docs Cleanup CI'
           git config --global user.email 'GithubActionsCleanup@noreply.github.com'
           git commit -am "Removing redundant docs version $DOCS_VERSION"
           git push
 
-# dae_devops_fingerprint 1dbde6e7935c64316f9a184d42056d54
+# dae_devops_fingerprint b30bd40d1c0f21c63e16ff1ab3102468
```

### Comparing `dls-bxflow-2.4.2/.github/workflows/linkcheck.yml` & `dls-bxflow-2.5.0/.github/workflows/linkcheck.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 name: Link Check
 
 on:
   workflow_dispatch:
   schedule:
@@ -23,8 +23,8 @@
         with:
           requirements_file: requirements-dev-3.x.txt
           install_options: -e .[dev]
 
       - name: Check links
         run: tox -e docs build -- -b linkcheck
 
-# dae_devops_fingerprint 821f149f612e9691d905f5f92c28f03c
+# dae_devops_fingerprint 1a299befecb0a7a90359e49213429df2
```

### Comparing `dls-bxflow-2.4.2/.gitignore` & `dls-bxflow-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/.gitlab-ci.yml` & `dls-bxflow-2.5.0/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -83,8 +83,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint 5af5158b679b480e93d4a7acac724eb2
+# dae_devops_fingerprint 63cc2bca187f39b9b6fdd5367be2a1d4
```

### Comparing `dls-bxflow-2.4.2/.vscode/launch.json` & `dls-bxflow-2.5.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/LICENSE` & `dls-bxflow-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/PKG-INFO` & `dls-bxflow-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.4.2
+Version: 2.5.0
 Summary: Distributed beamline automated data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-2.4.2/docs/conf.py` & `dls-bxflow-2.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -51,15 +51,15 @@
     # Create pages from jupyter notebooks
     "nbsphinx",
     "IPython.sphinxext.ipython_console_highlighting",
 ]
 
 # If true, Sphinx will warn about all references where the target cannot
 # be found.
-nitpicky = True
+nitpicky = False
 
 # A list of (type, target) tuples (by default empty) that should be ignored when
 # generating warnings in "nitpicky mode". Note that type should include the
 # domain name if present. Example entries would be ('py:func', 'int') or
 # ('envvar', 'LD_LIBRARY_PATH').
 nitpick_ignore = [("py:class", "numpy.ma.core.MaskedArray")]
 
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 381ce18acea8a261e7dad332b63a5366
+# dae_devops_fingerprint 67f12942c62a1495ca10314b0fb1f55b
```

### Comparing `dls-bxflow-2.4.2/docs/explanations/jobs.rst` & `dls-bxflow-2.5.0/docs/explanations/jobs.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/docs/explanations/todo.rst` & `dls-bxflow-2.5.0/docs/explanations/todo.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/docs/images/dls-favicon.ico` & `dls-bxflow-2.5.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/docs/images/dls-logo.svg` & `dls-bxflow-2.5.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/pyproject.toml` & `dls-bxflow-2.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,50 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev3+g9aafdd5.d20230608.
 # ********** For repository_name dls-bxflow
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dls-bxflow"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
 ]
 description = "Distributed beamline automated data processing workflow engine and gui platform core."
-dependencies = ["aio-pika", "dask[distributed]", "dls-servbase", "dls-mainiac", "dls-multiconf", "dls-utilpack", "dls-pairstream", "future", "graypy", "h5py", "ispyb==6.13.0", "ipykernel", "jsonpickle", "lxml", "nbclient", "nbconvert", "nbformat", "pika", "prettytable", "pyyaml", "ruamel.yaml", "stomp.py", "workflows", "beautifulsoup4"]
+dependencies = [
+    "aio-pika",
+    "dask[distributed]",
+    "dls-servbase",
+    "dls-mainiac",
+    "dls-multiconf",
+    "dls-utilpack",
+    "dls-pairstream",
+    "dls-slurmjob",
+    "future",
+    "graypy",
+    "h5py",
+    "ispyb==6.13.0",
+    "ipykernel",
+    "jsonpickle",
+    "lxml",
+    "nbclient",
+    "nbconvert",
+    "nbformat",
+    "pika",
+    "prettytable",
+    "pyyaml",
+    "ruamel.yaml",
+    "stomp.py",
+    "workflows",
+    "beautifulsoup4",
+]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
@@ -79,15 +105,15 @@
 ]
 max-line-length = 88 # Respect black's line length (default 88),
 exclude = [".tox", "venv"]
 
 
 [tool.pytest.ini_options]
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
-addopts = "    --tb=native -vv --doctest-modules --doctest-glob=\"*.rst\"\n    --cov=dls_bxflow_lib --cov-report term --cov-report xml:cov.xml\n    "
+addopts = "    --tb=native -vv --doctest-modules --doctest-glob=\"*.rst\"\n    "
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
 filterwarnings = "error"
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/dls_bxflow_lib.coverage"
@@ -97,8 +123,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 360bf0c450e119e24130fdf6a4e98ae8
+# dae_devops_fingerprint 93cd5608f3251be3373cc0f58f844c14
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow.egg-info/PKG-INFO` & `dls-bxflow-2.5.0/src/dls_bxflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.4.2
+Version: 2.5.0
 Summary: Distributed beamline automated data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow.egg-info/SOURCES.txt` & `dls-bxflow-2.5.0/src/dls_bxflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 src/dls_bxflow_api/bx_databases/__init__.py
 src/dls_bxflow_api/bx_databases/constants.py
 src/dls_bxflow_api/bx_datafaces/__init__.py
 src/dls_bxflow_api/bx_datafaces/aiohttp.py
 src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
 src/dls_bxflow_api/bx_datafaces/constants.py
 src/dls_bxflow_api/bx_datafaces/context.py
+src/dls_bxflow_api/bx_launchers/constants.py
 src/dls_bxflow_cli/__init__.py
 src/dls_bxflow_cli/main.py
 src/dls_bxflow_cli/version.py
 src/dls_bxflow_cli/contexts/dataface_client.py
 src/dls_bxflow_cli/contexts/filestore.py
 src/dls_bxflow_cli/contexts/news_consumer.py
 src/dls_bxflow_cli/subcommands/__init__.py
@@ -191,19 +192,19 @@
 src/dls_bxflow_lib/bx_jobs/context.py
 src/dls_bxflow_lib/bx_jobs/standard.py
 src/dls_bxflow_lib/bx_jobs/states.py
 src/dls_bxflow_lib/bx_launchers/__init__.py
 src/dls_bxflow_lib/bx_launchers/aiohttp.py
 src/dls_bxflow_lib/bx_launchers/base.py
 src/dls_bxflow_lib/bx_launchers/bx_launchers.py
-src/dls_bxflow_lib/bx_launchers/constants.py
 src/dls_bxflow_lib/bx_launchers/context.py
 src/dls_bxflow_lib/bx_launchers/island.py
 src/dls_bxflow_lib/bx_launchers/popener.py
 src/dls_bxflow_lib/bx_launchers/qsubber.py
+src/dls_bxflow_lib/bx_launchers/slurmer.py
 src/dls_bxflow_lib/bx_launchers/states.py
 src/dls_bxflow_lib/bx_logstores/__init__.py
 src/dls_bxflow_lib/bx_logstores/aiohttp.py
 src/dls_bxflow_lib/bx_logstores/base.py
 src/dls_bxflow_lib/bx_logstores/bx_logstores.py
 src/dls_bxflow_lib/bx_logstores/constants.py
 src/dls_bxflow_lib/bx_logstores/context.py
@@ -278,17 +279,14 @@
 tests/base.py
 tests/base_context_tester.py
 tests/base_specification_tester.py
 tests/base_tester.py
 tests/conftest.py
 tests/gda_parser.py
 tests/gda_workflow.py
-tests/qacct
-tests/qstat
-tests/qsub
 tests/test_catalog.py
 tests/test_collector.py
 tests/test_collector_scraper.py
 tests/test_composer.py
 tests/test_configurator.py
 tests/test_database.py
 tests/test_dataface.py
@@ -336,14 +334,16 @@
 tests/jupyter/jupyter2.ipynb
 tests/jupyter/jupyter_bad_cell.ipynb
 tests/jupyter/random_string.png
 tests/notebooks/c.ipynb
 tests/stub_commands/dawn
 tests/stub_commands/mpirun
 tests/stub_commands/ptychotools.ptypy_mpi_recipe
+tests/stub_commands/qstat
+tests/stub_commands/qsub
 tests/task_classes/task_z.py
 tests/workflows/__init__.py
 tests/workflows/base.py
 tests/workflows/utilities.py
 tests/workflows/a/__init__.py
 tests/workflows/a/workflow.py
 tests/workflows/b/__init__.py
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow.egg-info/requires.txt` & `dls-bxflow-2.5.0/src/dls_bxflow.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 aio-pika
 dask[distributed]
 dls-servbase
 dls-mainiac
 dls-multiconf
 dls-utilpack
 dls-pairstream
+dls-slurmjob
 future
 graypy
 h5py
 ispyb==6.13.0
 ipykernel
 jsonpickle
 lxml
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_api/bx_databases/constants.py` & `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_api/bx_datafaces/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class Context:
     """
     Client context for a bx_dataface object.
     On entering, it creates the object according to the specification (a dict).
     On exiting, it closes client connection.
 
-    The aenter and aexit methods are exposed for use by an enclosing context.
+    The aenter and aexit methods are exposed for use by an enclosing context and the base class.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
         self.__specification = specification
         self.__bx_dataface = None
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_api/exceptions.py` & `dls-bxflow-2.5.0/src/dls_bxflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_api/remex.py` & `dls-bxflow-2.5.0/src/dls_bxflow_api/remex.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,17 +27,18 @@
     GPU_ARCH = "gpu_arch"
     HOST = "host"
 
 
 class Clusters:
     HAMILTON = "dls_bxflow_api::remex::cluster::hamilton"
     SCIENCE = "dls_bxflow_api::remex::cluster::global/cluster"
+    SLURM = "dls_bxflow_api::remex::cluster::slurm"
     TEST = "dls_bxflow_api::remex::cluster::global/testcluster"
     LOCAL = "dls_bxflow_api::remex::cluster::local"
 
-    __list = [HAMILTON, SCIENCE, TEST, LOCAL]
+    __list = [HAMILTON, SCIENCE, SLURM, TEST, LOCAL]
 
     def validate(name):
         if name not in Clusters.__list:
             raise NotFound(
                 'cluster name "%s" is not in %s' % (name, str(Clusters.__list))
             )
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/contexts/dataface_client.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/dataface_client.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/contexts/filestore.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/contexts/news_consumer.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/news_consumer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/main.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/execute_workflow.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/find_xanes.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/find_xanes.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/fire_i22.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/fire_i22.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/recipe_parser.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/recipe_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/report_dcg.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_dcg.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/report_ispyb.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/start_services.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/subcommands/submit.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/submit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_cli/version.py` & `dls-bxflow-2.5.0/src/dls_bxflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/__main__.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_catalogs/ispyb.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/bx_collectors.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/gdascan.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gdascan.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/manual.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/manual.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_collectors/scraper.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         data_filenames = glob.glob(
             self.__scrape_glob, recursive=self.__scrape_recursive
         )
         t1 = time.time()
 
         seconds = "%0.3f" % (t1 - t0)
         logger.debug(
-            f"glob {self.__scrape_glob} found {len(data_filenames)} files in {seconds} seconds"
+            f"[SCRAPER_POLL] glob {self.__scrape_glob} found {len(data_filenames)} files in {seconds} seconds"
         )
 
         for data_filename in data_filenames:
             data_label = self.derive_data_label(data_filename)
 
             if data_label not in self.__data_labels:
                 await self.trigger_workflow_for_filename(data_filename)
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/bx_composers.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/bx_composers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/html.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/html.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/prettyhelper.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_composers/text.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/text.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_configurators/bx_configurators.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/bx_contexts.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_contexts/classic.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_databases/aiosqlite.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_databases/bx_databases.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/bx_databases.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_datafaces/news_producer.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/bx_filestores.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/explicit.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/explicit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_filestores/scandir.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/scandir.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_gamls/bx_gamls.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_gamls/html.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/html.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/bx_guis.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/bx_guis.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/constants.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/curses.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/curses.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/css/styles.css` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/index.html` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/index.html`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/index.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/bx_jobs.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_jobs/standard.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/standard.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 from dls_utilpack.thing import Thing
 
 from dls_bxflow_api.bx_databases.constants import BxLauncherFieldnames
 
 # Global bx_dataface.
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
+# BxLauncher protocolj things.
+from dls_bxflow_api.bx_launchers.constants import ClassTypes, Commands, Keywords
+
 # Remex things.
 from dls_bxflow_api.remex import Clusters as RemexClusters
 
 # Base class for an aiohttp server.
 from dls_bxflow_lib.base_aiohttp import BaseAiohttp
 
 # BxJobs manager.
 from dls_bxflow_lib.bx_jobs.bx_jobs import BxJobs
 
 # Factory to make a BxLauncher.
 from dls_bxflow_lib.bx_launchers.bx_launchers import BxLaunchers
 
-# BxLauncher protocolj things.
-from dls_bxflow_lib.bx_launchers.constants import Commands, Keywords
-
 # Possible bx_launcher states.
 from dls_bxflow_lib.bx_launchers.states import States as BxLauncherStates
 
 # BxTasks manager.
 from dls_bxflow_run.bx_tasks.bx_tasks import BxTasks
 
 logger = logging.getLogger(__name__)
 
-thing_type = "dls_bxflow_lib.bx_launchers.aiohttp"
+
+thing_type = ClassTypes.AIOHTTP
 
 
 # ------------------------------------------------------------------------------------------
 class Aiohttp(Thing, BaseAiohttp):
     """
     Object representing a bx_launcher which receives bx_tasks from aiohttp.
     """
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,16 @@
         bash_lines.append(f"echo 'hostname: ' `hostname`>> {prepare_log}")
         bash_lines.append(f"echo 'uname: ' `uname -a` >> {prepare_log}")
         bash_lines.append(f"echo 'id: ' `id` >> {prepare_log}")
         bash_lines.append(
             f"echo 'date: ' `date +'%Y-%m-%d %H:%M:%S %z'` >> {prepare_log}"
         )
         bash_lines.append(f"echo 'pwd: ' `pwd` >> {prepare_log}")
+        bash_lines.append(f"echo 'MODULEPATH: ' $MODULEPATH >> {prepare_log}")
+        bash_lines.append(f"echo 'MODULESHOME: ' $MODULESHOME >> {prepare_log}")
 
         bash_lines.append(f"echo '-----------------' >> {prepare_log}")
 
         if keyword not in bx_task.specification():
             bash_lines.append(f"# {bx_task} specification {keyword} is not present")
         else:
             prepare_environment = bx_task.specification().get(keyword)
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/bx_launchers.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Use standard logging in this module.
 import logging
 
 # Class managing list of things.
 from dls_utilpack.things import Things
 
+from dls_bxflow_api.bx_launchers.constants import ClassTypes
+
 # Exceptions.
 from dls_bxflow_api.exceptions import NotFound
 
 logger = logging.getLogger(__name__)
 
 
 class BxLaunchers(Things):
@@ -37,28 +39,33 @@
 
         return bx_launcher_object
 
     # ----------------------------------------------------------------------------------------
     def lookup_class(self, class_type):
         """"""
 
-        if class_type == "dls_bxflow_lib.bx_launchers.aiohttp":
+        if class_type == ClassTypes.AIOHTTP:
             from dls_bxflow_lib.bx_launchers.aiohttp import Aiohttp
 
             return Aiohttp
 
-        elif class_type == "dls_bxflow_lib.bx_launchers.island":
+        elif class_type == ClassTypes.ISLAND:
             from dls_bxflow_lib.bx_launchers.island import Island
 
             return Island
 
-        elif class_type == "dls_bxflow_lib.bx_launchers.popener":
+        elif class_type == ClassTypes.POPENER:
             from dls_bxflow_lib.bx_launchers.popener import Popener
 
             return Popener
 
-        elif class_type == "dls_bxflow_lib.bx_launchers.qsubber":
+        elif class_type == ClassTypes.QSUBBER:
             from dls_bxflow_lib.bx_launchers.qsubber import Qsubber
 
             return Qsubber
 
+        elif class_type == ClassTypes.SLURMER:
+            from dls_bxflow_lib.bx_launchers.slurmer import Slurmer
+
+            return Slurmer
+
         raise NotFound("unable to get bx_launcher class for %s" % (class_type))
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/island.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/island.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/popener.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/popener.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 import psutil
 
 # Utilities.
 from dls_utilpack.callsign import callsign
 from dls_utilpack.require import require
 
-# Describes a particular launch in terms of the job and task it belongs to.
-# Base class for bx_launcher instances.
+from dls_bxflow_api.bx_launchers.constants import ClassTypes
 from dls_bxflow_lib.bx_launchers.base import Base as BxLauncherBase
 from dls_bxflow_lib.bx_launchers.base import BaseLaunchInfo
 
 logger = logging.getLogger(__name__)
 
-thing_type = "dls_bxflow_lib.bx_launchers.popener"
+
+thing_type = ClassTypes.POPENER
 
 
 # ------------------------------------------------------------------------------------------
 class PopenerLaunchInfo(BaseLaunchInfo):
     """Launch info specific to this launcher type needed to identify a launched task."""
 
     def __init__(self, bx_job, bx_task):
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_launchers/qsubber.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/qsubber.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 # Utilities.
 from dls_utilpack.callsign import callsign
 
 # Environment module loader.
 from dls_utilpack.module import module_get_environ
 from dls_utilpack.require import require
 
+from dls_bxflow_api.bx_launchers.constants import ClassTypes
+
 # Remex (remote execution) API.
 from dls_bxflow_api.remex import Clusters as RemexClusters
 from dls_bxflow_api.remex import Keywords as RemexKeywords
 
 # Describes a particular launch in terms of the job and task it belongs to.
 # Base class for bx_launcher instances.
 from dls_bxflow_lib.bx_launchers.base import Base as BxLauncherBase
 from dls_bxflow_lib.bx_launchers.base import BaseLaunchInfo
 
 logger = logging.getLogger(__name__)
 
-thing_type = "dls_bxflow_lib.bx_launchers.qsubber"
+thing_type = ClassTypes.QSUBBER
 
 
 # ------------------------------------------------------------------------------------------
 class QsubberLaunchInfo(BaseLaunchInfo):
     """Launch info specific to this launcher type needed to identify a launched task."""
 
     def __init__(self, bx_job, bx_task):
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/bx_logstores.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_logstores/graylogger.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/graylogger.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/aio_pika.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aio_pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/bx_news.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/bx_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/constants.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/pika.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_news/zmq_pubsub.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/aiohttp.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/context.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/dask.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/dask.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/naive.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/naive.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_schedulers/zocalo.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from dls_utilpack.explain import explain
 
 # Utilities.
 from dls_utilpack.require import require
 from dls_utilpack.thing import Thing
 
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
+
+# BxLauncher manager.
+from dls_bxflow_api.bx_launchers.constants import Queues
 from dls_bxflow_lib.base_aiohttp import BaseAiohttp
 from dls_bxflow_lib.bx_jobs.bx_jobs import BxJobs
 
 # States of things.
 from dls_bxflow_lib.bx_jobs.states import States as BxJobStates
 
-# BxLauncher manager.
-from dls_bxflow_lib.bx_launchers.constants import Queues
-
 # Parameters manager.
 from dls_bxflow_run.bx_variables.bx_variables import BxVariables
 
 logger = logging.getLogger(__name__)
 
 thing_type = "dls_bxflow_lib.bx_schedulers.zocalo"
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/boolean.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/boolean.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/bx_settings.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/bx_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/float.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/float.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/integer.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/integer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_settings/string.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/string.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 
 # Exceptions.
 from dls_multiconf_lib.exceptions import NotFound
 
 # Utilities.
 from dls_utilpack.callsign import callsign
+from dls_utilpack.describe import describe
 from dls_utilpack.explain import explain2
 from dls_utilpack.require import require
 
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
 # Remote execution.
 from dls_bxflow_api.remex import Clusters as RemexClusters
@@ -201,18 +202,29 @@
         try:
             overall_default_hints = self.bx_configurator.require(
                 "bx_task_remex_hints.default"
             )
         except NotFound:
             pass
 
+        logger.debug(describe("[TSKRHNT] overall_default_hints", overall_default_hints))
+        logger.debug(
+            describe(
+                f"[TSKRHNT] task_type_default_hints for {thing_type}",
+                task_type_default_hints,
+            )
+        )
+
+        logger.debug(describe("[TSKRHNT] task_remex_hints", task_remex_hints))
         remex_hints = copy.deepcopy(overall_default_hints)
         remex_hints.update(task_type_default_hints)
         remex_hints.update(task_remex_hints)
 
+        logger.debug(describe("[TSKRHNT] assembled remex_hints", remex_hints))
+
         # Check that the clusters are valid.
         remex_clusters = require(
             f"{callsign} assembled remex_hints",
             remex_hints,
             RemexKeywords.CLUSTER,
         )
         if not isinstance(remex_clusters, list):
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/main.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/notebook_helper.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/bx_workflows/workflow_finder.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/dummies/writer.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/writer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/envvar.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/recipe_parser/overall.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/overall.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/recipe_parser/parser1.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/parser1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_lib/version.py` & `dls-bxflow-2.5.0/src/dls_bxflow_lib/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 
 # TODO: Use ImportlibMetadataVersion to get package versions.
 # from importlib.metadata import PackageNotFoundError
 # from importlib.metadata import version as ImportlibMetadataVersion
 
 from typing import Optional
 
-import dls_mainiac_lib.version
-import dls_pairstream_lib.version
-import dls_servbase_lib.version
-import dls_utilpack.version
-
 from dls_bxflow_lib import __version__
 
 
 # ----------------------------------------------------------
 def version() -> str:
     """
     Version of the dls_bxflow package as a string.
@@ -35,19 +30,49 @@
     Returns version information from the dls_bxflow package
     and its dependencies as a dict.
     Adds version information to a given meta dict if it was provided.
     """
 
     meta = {}
     meta["dls_bxflow"] = version()
-    meta.update(dls_utilpack.version.meta())
-    meta.update(dls_servbase_lib.version.meta())
-    meta.update(dls_mainiac_lib.version.meta())
-    meta.update(dls_utilpack.version.meta())
-    meta.update(dls_pairstream_lib.version.meta())
+
+    try:
+        import dls_utilpack.version
+
+        meta.update(dls_utilpack.version.meta())
+    except Exception:
+        meta["dls_utilpack"] = "unavailable"
+
+    try:
+        import dls_servbase_lib.version
+
+        meta.update(dls_servbase_lib.version.meta())
+    except Exception:
+        meta["dls_servbase_lib"] = "unavailable"
+
+    try:
+        import dls_slurmjob_lib.version
+
+        meta.update(dls_slurmjob_lib.version.meta())
+    except Exception:
+        meta["dls_slurmjob_lib"] = "unavailable"
+
+    try:
+        import dls_mainiac_lib.version
+
+        meta.update(dls_mainiac_lib.version.meta())
+    except Exception:
+        meta["dls_mainiac_lib"] = "unavailable"
+
+    try:
+        import dls_pairstream_lib.version
+
+        meta.update(dls_pairstream_lib.version.meta())
+    except Exception:
+        meta["dls_pairstream_lib"] = "unavailable"
 
     try:
         import stomp
 
         parts = stomp.__version__
         parts = [str(s) for s in parts]
         meta["stomp"] = ".".join(parts)
```

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_gates/bx_gates.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/bx_gates.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/bx_tasks.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/constants.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dawn1.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dawn2.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dawn_base.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/dummy.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/execution_summary.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/execution_summary.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/filename_classname.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/filename_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/jupyter.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/jupyter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/module_classname.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/module_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/pickled_class.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/pickled_class.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/shell.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_tasks/symlink.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/symlink.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/bx_variables/bx_variables.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/bx_variables.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/src/dls_bxflow_run/main_isolated.py` & `dls-bxflow-2.5.0/src/dls_bxflow_run/main_isolated.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/base.py` & `dls-bxflow-2.5.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/base_context_tester.py` & `dls-bxflow-2.5.0/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/base_specification_tester.py` & `dls-bxflow-2.5.0/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/base_tester.py` & `dls-bxflow-2.5.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/configurations/backend.yaml` & `dls-bxflow-2.5.0/tests/configurations/backend.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -43,27 +43,32 @@
     dls_servbase_dataface_server: &DLS_SERVBASE_DATAFACE_SERVER http://*:22427
     dls_servbase_dataface_client: &DLS_SERVBASE_DATAFACE_CLIENT http://localhost:22427
     dataface_port: &DATAFACE_PORT 22422
     launcher1_server: &LAUNCHER1_SERVER http://*:22424
     launcher1_client: &LAUNCHER1_CLIENT http://localhost:22424
     launcher2_server: &LAUNCHER2_SERVER http://*:22429
     launcher2_client: &LAUNCHER2_CLIENT http://localhost:22429
+    launcher3_server: &LAUNCHER3_SERVER http://*:22430
+    launcher3_client: &LAUNCHER3_CLIENT http://localhost:22430
     scheduler_server: &SCHEDULER_SERVER http://*:22425
     scheduler_client: &SCHEDULER_CLIENT http://localhost:22425
     catalog_server: &CATALOG_SERVER http://*:22426
     catalog_client: &CATALOG_CLIENT http://localhost:22426
     collector_server: &COLLECTOR_SERVER http://*:22428
     collector_client: &COLLECTOR_CLIENT http://localhost:22428
     bx_gui_server: &BX_GUI_SERVER http://*:22222
     bx_gui_client: &BX_GUI_CLIENT http://127.0.0.1:22222
     graylog_client: &GRAYLOG_CLIENT http://172.23.7.128:9000
 
     stomp_server: &STOMP_SERVER stomp://172.23.7.128:61613
     stomp_client: &STOMP_CLIENT stomp://172.23.7.128:61613
 
+dls_slurmjob_restd_specification: &DLS_SLURMJOB_RESTD_SPECIFICATION
+    type: "dls_slurmjob_lib.restds.dummy"
+
 bx_task_specification:
     pairstream:
         producer:
             class_name: "dls::pairstream::zmq_pushpull"
             endpoint: "tcp://*:0"
         consumer:
             class_name: "dls::pairstream::zmq_pushpull"
@@ -79,14 +84,15 @@
 
 # Task remex hints.
 # These describe the remex hints for tasks.
 # It can be different for different task thing_types.
 remex_clusters:
     - &CLUSTER_HAMILTON "dls_bxflow_api::remex::cluster::hamilton"
     - &CLUSTER_SCIENCE "dls_bxflow_api::remex::cluster::global/cluster"
+    - &CLUSTER_SLURM "dls_bxflow_api::remex::cluster::slurm"
     - &CLUSTER_TEST "dls_bxflow_api::remex::cluster::global/testcluster"
     - &CLUSTER_LOCAL "dls_bxflow_api::remex::cluster::local"
 
 # Remex hints predefined.
 # The following keywords are honored:
 # cluster
 # m_mem_free
@@ -200,18 +206,18 @@
                 filename: "${output_directory}/bx_dataface.sqlite"
                 log_level: "WARNING"
             bx_news_specification: *BX_NEWS_SPECIFICATION
     context:
         start_as: process
 
 # The available bx_launchers.
-bx_launcher_popener_specification: &BX_LAUNCHER_POPENER_SPECIFICATION
+bx_launcher_popener_specification:
     type: "dls_bxflow_lib.bx_launchers.aiohttp"
     uuid: "popener-01"
-    remex_cluster: "dls_bxflow_api::remex::cluster::local"
+    remex_cluster: *CLUSTER_LOCAL
     type_specific_tbd:
         aiohttp_specification:
             server: *LAUNCHER1_SERVER
             client: *LAUNCHER1_CLIENT
         actual_bx_launcher_specification:
             type: "dls_bxflow_lib.bx_launchers.popener"
             type_specific_tbd:
@@ -219,32 +225,49 @@
                 task_count_max: 10
     context:
         start_as: process
 
 bx_launcher_qsubber_specification:
     type: "dls_bxflow_lib.bx_launchers.aiohttp"
     uuid: "qsubber-01"
-    remex_cluster: "dls_bxflow_api::remex::cluster::global/testcluster"
+    remex_cluster: *CLUSTER_TEST
     type_specific_tbd:
         aiohttp_specification:
             server: *LAUNCHER2_SERVER
             client: *LAUNCHER2_CLIENT
         actual_bx_launcher_specification:
             type: "dls_bxflow_lib.bx_launchers.qsubber"
             type_specific_tbd:
                 task_count_max: 10
                 cluster_project: test_project
                 cluster_queue: test_queue
     context:
         start_as: process
 
+bx_launcher_slurmer_specification:
+    type: "dls_bxflow_lib.bx_launchers.aiohttp"
+    uuid: "slurmer-01"
+    remex_cluster: *CLUSTER_SLURM
+    type_specific_tbd:
+        aiohttp_specification:
+            server: *LAUNCHER3_SERVER
+            client: *LAUNCHER3_CLIENT
+        actual_bx_launcher_specification:
+            type: "dls_bxflow_lib.bx_launchers.slurmer"
+            type_specific_tbd:
+                task_count_max: 10
+                slurmjob_specification: *DLS_SLURMJOB_RESTD_SPECIFICATION
+    context:
+        start_as: process
+
 # The bx_launchers pool.
 bx_launcher_specifications:
     - bx_launcher_popener_specification
     - bx_launcher_qsubber_specification
+    - bx_launcher_slurmer_specification
 
 # The bx_job.
 bx_job_specification:
     type: "dls_bxflow_lib.bx_jobs.standard"
     label: "unlabeled"
 
 # The bx_scheduler.
```

### Comparing `dls-bxflow-2.4.2/tests/configurations/filestore.yaml` & `dls-bxflow-2.5.0/tests/configurations/filestore.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml` & `dls-bxflow-2.5.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/configurations/ptyrex_configfiles/region_p4_p6.json` & `dls-bxflow-2.5.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/conftest.py` & `dls-bxflow-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/datafiles/dawn2_configuration.json` & `dls-bxflow-2.5.0/tests/datafiles/dawn2_configuration.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/datafiles/i22-4996.nxs` & `dls-bxflow-2.5.0/tests/datafiles/i22-4996.nxs`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/gda_parser.py` & `dls-bxflow-2.5.0/tests/gda_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/gda_workflow.py` & `dls-bxflow-2.5.0/tests/gda_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/jupyter/jupyter1.ipynb` & `dls-bxflow-2.5.0/tests/jupyter/jupyter1.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/jupyter/jupyter2.ipynb` & `dls-bxflow-2.5.0/tests/jupyter/jupyter2.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/jupyter/jupyter_bad_cell.ipynb` & `dls-bxflow-2.5.0/tests/jupyter/jupyter_bad_cell.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/jupyter/random_string.png` & `dls-bxflow-2.5.0/tests/jupyter/random_string.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/notebooks/c.ipynb` & `dls-bxflow-2.5.0/tests/notebooks/c.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/qstat` & `dls-bxflow-2.5.0/tests/stub_commands/qstat`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/stub_commands/ptychotools.ptypy_mpi_recipe` & `dls-bxflow-2.5.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_catalog.py` & `dls-bxflow-2.5.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_collector.py` & `dls-bxflow-2.5.0/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_collector_scraper.py` & `dls-bxflow-2.5.0/tests/test_collector_scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_composer.py` & `dls-bxflow-2.5.0/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_configurator.py` & `dls-bxflow-2.5.0/tests/test_configurator.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_database.py` & `dls-bxflow-2.5.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_dataface.py` & `dls-bxflow-2.5.0/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_dataface_revision5.py` & `dls-bxflow-2.5.0/tests/test_dataface_revision5.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_dawn1.py` & `dls-bxflow-2.5.0/tests/test_dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_dawn2.py` & `dls-bxflow-2.5.0/tests/test_dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_extract_error_lines_dawn.py` & `dls-bxflow-2.5.0/tests/test_extract_error_lines_dawn.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_extract_error_lines_dummy.py` & `dls-bxflow-2.5.0/tests/test_extract_error_lines_dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_filestore.py` & `dls-bxflow-2.5.0/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_gaml.py` & `dls-bxflow-2.5.0/tests/test_gaml.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_gui.py` & `dls-bxflow-2.5.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_job_a.py` & `dls-bxflow-2.5.0/tests/test_job_a.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 
         logger.info(f"job summary\n{job_summary_text}")
 
         # logger.info(describe("self.consumed_news", self.consumed_news))
 
         # Check we got all the news.
         count = len(self.consumed_news)
-        expected_news_count = 9
+        expected_news_count = 10
         if count != expected_news_count:
             logger.info(describe("self.consumed_news", self.consumed_news))
 
         assert count == expected_news_count
 
         topic, headline, payload = self.consumed_news[0]
         assert topic == BxNewsTopics.BXJOB_WAS_ENABLED
@@ -265,7 +265,11 @@
         topic, headline, payload = self.consumed_news[7]
         assert topic == BxNewsTopics.BXLAUNCHER_WAS_UPDATED
         assert payload["bx_launcher"]["state"] == BxLauncherStates.SHUTDOWN
 
         topic, headline, payload = self.consumed_news[8]
         assert topic == BxNewsTopics.BXLAUNCHER_WAS_UPDATED
         assert payload["bx_launcher"]["state"] == BxLauncherStates.SHUTDOWN
+
+        topic, headline, payload = self.consumed_news[9]
+        assert topic == BxNewsTopics.BXLAUNCHER_WAS_UPDATED
+        assert payload["bx_launcher"]["state"] == BxLauncherStates.SHUTDOWN
```

### Comparing `dls-bxflow-2.4.2/tests/test_job_a_bc_d.py` & `dls-bxflow-2.5.0/tests/test_job_a_bc_d.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_job_notebook.py` & `dls-bxflow-2.5.0/tests/test_job_notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
         logger.info(f"job summary\n{job_summary_text}")
 
         # logger.info(describe("self.consumed_news", self.consumed_news))
 
         # Check we got all the news.
         count = len(self.consumed_news)
-        expected_news_count = 8
+        expected_news_count = 9
         if count != expected_news_count:
             logger.info(describe("self.consumed_news", self.consumed_news))
 
         assert count == expected_news_count
 
         topic, headline, payload = self.consumed_news[0]
         assert topic == BxNewsTopics.BXJOB_WAS_ENABLED
@@ -193,7 +193,11 @@
         topic, headline, payload = self.consumed_news[6]
         assert topic == BxNewsTopics.BXLAUNCHER_WAS_UPDATED
         assert payload["bx_launcher"]["state"] == BxLauncherStates.SHUTDOWN
 
         topic, headline, payload = self.consumed_news[7]
         assert topic == BxNewsTopics.BXLAUNCHER_WAS_UPDATED
         assert payload["bx_launcher"]["state"] == BxLauncherStates.SHUTDOWN
+
+        topic, headline, payload = self.consumed_news[8]
+        assert topic == BxNewsTopics.BXLAUNCHER_WAS_UPDATED
+        assert payload["bx_launcher"]["state"] == BxLauncherStates.SHUTDOWN
```

### Comparing `dls-bxflow-2.4.2/tests/test_job_pubcon.py` & `dls-bxflow-2.5.0/tests/test_job_pubcon.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_job_x.py` & `dls-bxflow-2.5.0/tests/test_job_x.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_jupyter.py` & `dls-bxflow-2.5.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_launcher.py` & `dls-bxflow-2.5.0/tests/test_launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,16 +154,19 @@
         self.__expected_exit_code = expected_exit_code
         self.__expected_error_lines = expected_error_lines
         self.__bx_task_prepare_environment = bx_task_prepare_environment
 
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
-        # Make the fake qsub findable in the path.
-        os.environ["PATH"] = "%s:%s" % (os.path.dirname(__file__), os.environ["PATH"])
+        # Make the qsub stub findable in the path.
+        os.environ["PATH"] = "%s/stub_commands:%s" % (
+            os.path.dirname(__file__),
+            os.environ["PATH"],
+        )
 
         # Supply environment variable for substitution in the bx configurator.
         os.environ["OUTPUT_DIRECTORY"] = output_directory
 
         # Directory where the task should write its files.
         bx_task_directory = f"{output_directory}/task_directory"
```

### Comparing `dls-bxflow-2.4.2/tests/test_launcher_capacity.py` & `dls-bxflow-2.5.0/tests/test_launcher_capacity.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_launcher_direct.py` & `dls-bxflow-2.5.0/tests/test_launcher_direct.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,30 @@
 
         LauncherDirectTester(launcher_keyword).main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
+# TODO: Vitalize TestLauncherDirectSlurmer when its dummy implementation can produce the residuals.
+class XTestLauncherDirectSlurmer:
+    def test(self, constants, logging_setup, output_directory):
+        """ """
+
+        configuration_file = "tests/configurations/backend.yaml"
+
+        # The launcher configuration to replace in the configuration file for this test.
+        launcher_keyword = "bx_launcher_slurmer_specification"
+
+        LauncherDirectTester(launcher_keyword).main(
+            constants, configuration_file, output_directory
+        )
+
+
+# ----------------------------------------------------------------------------------------
 class LauncherDirectTester(BaseContextTester):
     """
     Class to test the launcher being restarted.
     """
 
     def __init__(
         self,
@@ -68,16 +84,19 @@
 
         self.__launcher_keyword = launcher_keyword
 
     # ------------------------------------------------------------------------------------
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
-        # Make the fake qsub findable in the path.
-        os.environ["PATH"] = "%s:%s" % (os.path.dirname(__file__), os.environ["PATH"])
+        # Make the qsub stub commands findable in the path.
+        os.environ["PATH"] = "%s/stub_commands:%s" % (
+            os.path.dirname(__file__),
+            os.environ["PATH"],
+        )
 
         # Supply environment variable for substitution in the bx configurator.
         os.environ["OUTPUT_DIRECTORY"] = output_directory
 
         # Directory where the task should write its files.
         bx_task_directory = f"{output_directory}/task_directory"
```

### Comparing `dls-bxflow-2.4.2/tests/test_launcher_multiple.py` & `dls-bxflow-2.5.0/tests/test_launcher_multiple.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,19 @@
         self,
     ):
         BaseContextTester.__init__(self)
 
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
-        # Make the fake qsub findable in the path.
-        os.environ["PATH"] = "%s:%s" % (os.path.dirname(__file__), os.environ["PATH"])
+        # Make the qsub stub commands findable in the path.
+        os.environ["PATH"] = "%s/stub_commands:%s" % (
+            os.path.dirname(__file__),
+            os.environ["PATH"],
+        )
 
         # Supply environment variable for substitution in the bx configurator.
         os.environ["OUTPUT_DIRECTORY"] = output_directory
 
         bx_configurator = self.get_bx_configurator()
 
         # Don't start the services we don't need for this test.
```

### Comparing `dls-bxflow-2.4.2/tests/test_launcher_restart.py` & `dls-bxflow-2.5.0/tests/test_launcher_restart.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,16 +82,19 @@
 
         self.__desired_bx_launcher_specification = desired_bx_launcher_specification
 
     # ------------------------------------------------------------------------------------
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
-        # Make the fake qsub findable in the path.
-        os.environ["PATH"] = "%s:%s" % (os.path.dirname(__file__), os.environ["PATH"])
+        # Make the qsub stub commands findable in the path.
+        os.environ["PATH"] = "%s/stub_commands:%s" % (
+            os.path.dirname(__file__),
+            os.environ["PATH"],
+        )
 
         # Supply environment variable for substitution in the bx configurator.
         os.environ["OUTPUT_DIRECTORY"] = output_directory
 
         # Load the configuration.
         bx_configurator = self.get_bx_configurator()
```

### Comparing `dls-bxflow-2.4.2/tests/test_logstore.py` & `dls-bxflow-2.5.0/tests/test_logstore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_news.py` & `dls-bxflow-2.5.0/tests/test_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_protocolj.py` & `dls-bxflow-2.5.0/tests/test_protocolj.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_ptypy_mpi.py` & `dls-bxflow-2.5.0/tests/test_ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_ptyrex_mpi.py` & `dls-bxflow-2.5.0/tests/test_ptyrex_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_scheduler_naive.py` & `dls-bxflow-2.5.0/tests/test_scheduler_naive.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,17 +59,19 @@
         self,
     ):
         BaseContextTester.__init__(self)
 
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
-        # Make the fake qsub findable in the path.
-        os.environ["PATH"] = "%s:%s" % (os.path.dirname(__file__), os.environ["PATH"])
-
+        # Make the qsub stub commands findable in the path.
+        os.environ["PATH"] = "%s/stub_commands:%s" % (
+            os.path.dirname(__file__),
+            os.environ["PATH"],
+        )
         # Supply environment variable for substitution in the bx configurator.
         os.environ["OUTPUT_DIRECTORY"] = output_directory
 
         bx_configurator = self.get_bx_configurator()
 
         # Don't start the services we don't need for this test.
         # bx_configurator.remove("bx_scheduler_specification")
@@ -141,17 +143,18 @@
                 )
                 assert False, case
             except TransientError as exception:
                 assert "[NOLAUNCH2]" in str(exception)
 
             # ----------------------------------------------------------------------
             case = "single hint, found no idle launchers"
-            row = {"uuid": "popener-01", "state": BxLauncherStates.BUSY}
             row = {"uuid": "qsubber-01", "state": BxLauncherStates.BUSY}
             await bx_datafaces_get_default().update_bx_launcher(row)
+            row = {"uuid": "slurmer-01", "state": BxLauncherStates.BUSY}
+            await bx_datafaces_get_default().update_bx_launcher(row)
             task_specification[RemexKeywords.HINTS] = {
                 RemexKeywords.CLUSTER: RemexClusters.LOCAL
             }
             try:
                 launcher_record = await naive_scheduler.select_launcher_record(
                     bx_task_uuid, task_specification
                 )
```

### Comparing `dls-bxflow-2.4.2/tests/test_settings.py` & `dls-bxflow-2.5.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_shell.py` & `dls-bxflow-2.5.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_task.py` & `dls-bxflow-2.5.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_workflow.py` & `dls-bxflow-2.5.0/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/test_workflow_finder.py` & `dls-bxflow-2.5.0/tests/test_workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/a/workflow.py` & `dls-bxflow-2.5.0/tests/workflows/a/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/b/workflow.py` & `dls-bxflow-2.5.0/tests/workflows/b/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/base.py` & `dls-bxflow-2.5.0/tests/workflows/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/c/workflow.py` & `dls-bxflow-2.5.0/tests/workflows/c/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/e/workflow.py` & `dls-bxflow-2.5.0/tests/workflows/e/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/f/workflow.py` & `dls-bxflow-2.5.0/tests/workflows/f/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/g/workflow.py` & `dls-bxflow-2.5.0/tests/workflows/g/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.4.2/tests/workflows/utilities.py` & `dls-bxflow-2.5.0/tests/workflows/utilities.py`

 * *Files identical despite different names*

