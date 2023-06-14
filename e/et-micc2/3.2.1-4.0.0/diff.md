# Comparing `tmp/et-micc2-3.2.1.tar.gz` & `tmp/et_micc2-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "et-micc2-3.2.1.tar", max compression
+gzip compressed data, was "et_micc2-4.0.0.tar", max compression
```

## Comparing `et-micc2-3.2.1.tar` & `et_micc2-4.0.0.tar`

### file list

```diff
@@ -1,54 +1,68 @@
--rw-r--r--   0        0        0     1077 2019-06-06 12:46:17.209535 et-micc2-3.2.1/LICENSE
--rw-r--r--   0        0        0     3701 2021-04-23 08:03:05.754390 et-micc2-3.2.1/README.rst
--rw-r--r--   0        0        0      227 2022-04-26 12:24:27.095692 et-micc2-3.2.1/et_micc2/__init__.py
--rw-r--r--   0        0        0     7547 2021-04-02 11:56:37.606233 et-micc2-3.2.1/et_micc2/check_environment.py
--rw-r--r--   0        0        0    31969 2022-03-10 07:31:11.817789 et-micc2-3.2.1/et_micc2/cli_micc.py
--rw-r--r--   0        0        0     4776 2021-04-22 19:10:47.178338 et-micc2-3.2.1/et_micc2/config.py
--rw-r--r--   0        0        0     1356 2021-03-25 21:59:58.023070 et-micc2-3.2.1/et_micc2/db.py
--rw-r--r--   0        0        0    10081 2021-10-15 09:08:59.111430 et-micc2-3.2.1/et_micc2/expand.py
--rw-r--r--   0        0        0     7458 2021-05-07 14:23:41.767474 et-micc2-3.2.1/et_micc2/logger.py
--rw-r--r--   0        0        0     1406 2021-04-21 09:30:10.812321 et-micc2-3.2.1/et_micc2/micc.json
--rw-r--r--   0        0        0    75450 2022-04-26 10:18:42.392406 et-micc2-3.2.1/et_micc2/project.py
--rw-r--r--   0        0        0     5244 2021-05-11 08:19:15.767015 et-micc2-3.2.1/et_micc2/scripts/install-e.py
--rw-r--r--   0        0        0      705 2021-04-23 06:50:07.006119 et-micc2-3.2.1/et_micc2/static_vars.py
--rw-r--r--   0        0        0      838 2021-08-05 17:44:02.739349 et-micc2-3.2.1/et_micc2/templates/app-single-command/{{tmpl.project_name}}/tests/{{tmpl.test_}}{{tmpl.cli_app_name}}.py
--rw-r--r--   0        0        0      548 2021-08-05 17:44:02.739942 et-micc2-3.2.1/et_micc2/templates/app-single-command/{{tmpl.project_name}}/{{tmpl.package_name}}/{{tmpl.cli_app_name}}.py
--rw-r--r--   0        0        0      929 2021-08-05 17:44:02.740796 et-micc2-3.2.1/et_micc2/templates/app-sub-commands/{{tmpl.project_name}}/tests/{{tmpl.test_]}{{tmpl.cli_app_name}}.py
--rw-r--r--   0        0        0     1128 2021-08-05 17:44:02.741435 et-micc2-3.2.1/et_micc2/templates/app-sub-commands/{{tmpl.project_name}}/{{tmpl.package_name}}/{{tmpl.cli_app_name}}.py
--rw-r--r--   0        0        0     2924 2021-08-05 17:44:02.743115 et-micc2-3.2.1/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/CMakeLists.txt
--rw-r--r--   0        0        0     1741 2021-08-05 17:44:02.743790 et-micc2-3.2.1/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.cpp
--rw-r--r--   0        0        0      648 2021-08-05 17:44:02.744610 et-micc2-3.2.1/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.rst
--rw-r--r--   0        0        0      997 2021-08-12 20:44:47.442120 et-micc2-3.2.1/et_micc2/templates/submodule-cpp-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py
--rw-r--r--   0        0        0    11609 2021-08-05 17:44:02.746498 et-micc2-3.2.1/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/CMakeLists.txt
--rw-r--r--   0        0        0     1708 2021-08-05 17:44:02.747223 et-micc2-3.2.1/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.f90
--rw-r--r--   0        0        0      672 2021-08-05 17:44:02.747848 et-micc2-3.2.1/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.rst
--rw-r--r--   0        0        0     1063 2021-08-05 17:44:02.745386 et-micc2-3.2.1/et_micc2/templates/submodule-f90-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py
--rw-r--r--   0        0        0      252 2021-08-10 09:44:59.308521 et-micc2-3.2.1/et_micc2/templates/submodule-py/{{tmpl.module_name}}/__init__.py
--rw-r--r--   0        0        0      839 2021-10-08 09:30:00.829082 et-micc2-3.2.1/et_micc2/templates/submodule-py-test/{{tmpl.module_name}}/{{tmpl.test_}}{{tmpl.module_name}}.py
--rw-r--r--   0        0        0     1357 2021-08-05 17:44:02.750468 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/.gitignore
--rw-r--r--   0        0        0      502 2021-08-05 17:44:02.751088 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/.readthedocs.yml
--rw-r--r--   0        0        0       64 2021-08-05 17:44:02.751821 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/API.rst
--rw-r--r--   0        0        0       40 2021-08-05 17:44:02.752544 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/APPS.rst
--rw-r--r--   0        0        0       72 2021-08-05 17:44:02.753238 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/AUTHORS.rst
--rw-r--r--   0        0        0      152 2021-08-05 17:44:02.753948 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/CHANGELOG.rst
--rw-r--r--   0        0        0      139 2021-08-05 17:44:02.754671 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/README.rst
--rw-r--r--   0        0        0     1787 2021-08-05 17:44:02.755766 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/Makefile
--rw-r--r--   0        0        0       24 2021-08-05 17:44:02.756423 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/api.rst
--rw-r--r--   0        0        0       25 2021-08-05 17:44:02.757055 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/apps.rst
--rw-r--r--   0        0        0       28 2021-08-05 17:44:02.757610 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/authors.rst
--rw-r--r--   0        0        0       30 2021-08-05 17:44:02.758155 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/changelog.rst
--rwxr-xr-x   0        0        0     5316 2021-08-05 17:44:02.758712 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      391 2021-08-05 17:44:02.759334 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/index.rst
--rw-r--r--   0        0        0     1290 2021-08-05 17:44:02.760095 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/installation.rst
--rw-r--r--   0        0        0       27 2021-08-05 17:44:02.760879 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/readme.rst
--rw-r--r--   0        0        0       72 2021-08-05 17:44:02.761631 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/requirements.txt
--rw-r--r--   0        0        0      587 2021-08-05 17:44:02.762325 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      230 2021-08-05 17:44:02.763204 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0     1038 2022-03-17 08:01:04.640090 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/tests/{{tmpl.package_name}}/test_{{tmpl.package_name}}.py
--rw-r--r--   0        0        0      377 2021-08-05 17:44:02.765001 et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/{{tmpl.package_name}}/__init__.py
--rw-r--r--   0        0        0     3673 2022-04-26 12:23:20.502789 et-micc2-3.2.1/et_micc2/tmpl.py
--rw-r--r--   0        0        0     2263 2021-03-25 21:59:58.047549 et-micc2-3.2.1/et_micc2/tomlfile.py
--rw-r--r--   0        0        0    11487 2021-08-05 17:44:02.813840 et-micc2-3.2.1/et_micc2/utils.py
--rw-r--r--   0        0        0      675 2022-04-26 12:24:27.094783 et-micc2-3.2.1/pyproject.toml
--rw-r--r--   0        0        0    10757 2022-04-26 12:32:44.548970 et-micc2-3.2.1/setup.py
--rw-r--r--   0        0        0     4610 2022-04-26 12:32:44.550022 et-micc2-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-10 19:04:59.677430 et_micc2-4.0.0/LICENSE
+-rw-r--r--   0        0        0     3701 2023-03-10 19:04:59.678751 et_micc2-4.0.0/README.rst
+-rw-r--r--   0        0        0      229 2023-06-14 15:26:48.643683 et_micc2-4.0.0/et_micc2/__init__.py
+-rw-r--r--   0        0        0    32483 2023-06-14 15:23:40.230980 et_micc2-4.0.0/et_micc2/cli_micc.py
+-rw-r--r--   0        0        0     4776 2023-06-14 15:23:40.231902 et_micc2-4.0.0/et_micc2/obsolete/config.py
+-rw-r--r--   0        0        0     1356 2023-06-14 15:23:40.232218 et_micc2-4.0.0/et_micc2/obsolete/db.py
+-rw-r--r--   0        0        0    10087 2023-06-14 15:23:40.260177 et_micc2-4.0.0/et_micc2/obsolete/expand.py
+-rw-r--r--   0        0        0     7458 2023-06-14 15:23:40.260643 et_micc2-4.0.0/et_micc2/obsolete/logger.py
+-rw-r--r--   0        0        0     1406 2023-06-14 15:23:40.260925 et_micc2-4.0.0/et_micc2/obsolete/micc.json
+-rw-r--r--   0        0        0    75426 2023-06-14 15:23:40.288470 et_micc2-4.0.0/et_micc2/obsolete/project.py
+-rw-r--r--   0        0        0      705 2023-06-14 15:23:40.288805 et_micc2-4.0.0/et_micc2/obsolete/static_vars.py
+-rw-r--r--   0        0        0    11493 2023-06-14 15:23:40.315737 et_micc2-4.0.0/et_micc2/obsolete/utils.py
+-rw-r--r--   0        0        0     5244 2023-03-13 20:43:58.878511 et_micc2-4.0.0/et_micc2/scripts/install-e.py
+-rw-r--r--   0        0        0    18028 2023-06-14 15:23:40.343857 et_micc2-4.0.0/et_micc2/subcmds/add.py
+-rw-r--r--   0        0        0     8365 2023-06-14 15:23:40.370937 et_micc2-4.0.0/et_micc2/subcmds/build.py
+-rw-r--r--   0        0        0     7547 2023-06-14 15:23:40.397904 et_micc2-4.0.0/et_micc2/subcmds/check_env.py
+-rw-r--r--   0        0        0    11121 2023-06-14 15:23:40.425257 et_micc2-4.0.0/et_micc2/subcmds/create.py
+-rw-r--r--   0        0        0     1804 2023-06-14 15:23:40.452444 et_micc2-4.0.0/et_micc2/subcmds/doc.py
+-rw-r--r--   0        0        0     2450 2023-06-14 15:23:40.479957 et_micc2-4.0.0/et_micc2/subcmds/info.py
+-rw-r--r--   0        0        0     8515 2023-06-14 15:23:40.560815 et_micc2-4.0.0/et_micc2/subcmds/mv.py
+-rw-r--r--   0        0        0     1877 2023-06-14 15:23:40.601378 et_micc2-4.0.0/et_micc2/subcmds/tag.py
+-rw-r--r--   0        0        0     2616 2023-06-14 15:23:40.642356 et_micc2-4.0.0/et_micc2/subcmds/version.py
+-rw-r--r--   0        0        0      834 2023-06-14 15:23:40.682367 et_micc2-4.0.0/et_micc2/templates/app-single-command/{{tmpl.project_name}}/tests/{{tmpl.package_name}}/cli/{{tmpl.test_}}{{tmpl.app_name}}.py
+-rw-r--r--   0        0        0      548 2023-06-14 15:23:40.683219 et_micc2-4.0.0/et_micc2/templates/app-single-command/{{tmpl.project_name}}/{{tmpl.package_name}}/cli/{{tmpl.app_name}}.py
+-rw-r--r--   0        0        0      925 2023-06-14 15:23:40.722122 et_micc2-4.0.0/et_micc2/templates/app-sub-commands/{{tmpl.project_name}}/tests/{{tmpl.package_name}}/cli/{{tmpl.test_}}{{tmpl.app_name}}.py
+-rw-r--r--   0        0        0     1128 2023-06-14 15:23:40.722654 et_micc2-4.0.0/et_micc2/templates/app-sub-commands/{{tmpl.project_name}}/{{tmpl.package_name}}/cli/{{tmpl.app_name}}.py
+-rw-r--r--   0        0        0     2924 2023-03-13 20:43:58.883077 et_micc2-4.0.0/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/CMakeLists.txt
+-rw-r--r--   0        0        0     1741 2023-03-13 20:43:58.883715 et_micc2-4.0.0/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.cpp
+-rw-r--r--   0        0        0      648 2023-03-13 20:43:58.884319 et_micc2-4.0.0/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.rst
+-rw-r--r--   0        0        0      997 2023-03-13 20:43:58.885071 et_micc2-4.0.0/et_micc2/templates/submodule-cpp-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py
+-rw-r--r--   0        0        0    11609 2023-03-13 20:43:58.885869 et_micc2-4.0.0/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/CMakeLists.txt
+-rw-r--r--   0        0        0     1708 2023-03-13 20:43:58.886675 et_micc2-4.0.0/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.f90
+-rw-r--r--   0        0        0      672 2023-03-13 20:43:58.887919 et_micc2-4.0.0/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.rst
+-rw-r--r--   0        0        0     1063 2023-03-13 20:43:58.889185 et_micc2-4.0.0/et_micc2/templates/submodule-f90-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py
+-rw-r--r--   0        0        0      252 2023-03-13 20:43:58.890550 et_micc2-4.0.0/et_micc2/templates/submodule-py/{{tmpl.module_name}}/__init__.py
+-rw-r--r--   0        0        0      839 2023-03-13 20:43:58.891985 et_micc2-4.0.0/et_micc2/templates/submodule-py-test/{{tmpl.module_name}}/{{tmpl.test_}}{{tmpl.module_name}}.py
+-rw-r--r--   0        0        0     1357 2023-03-13 20:43:58.893371 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/.gitignore
+-rw-r--r--   0        0        0      502 2023-03-13 20:43:58.894757 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/.readthedocs.yml
+-rw-r--r--   0        0        0       64 2023-03-13 20:43:58.895860 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/API.rst
+-rw-r--r--   0        0        0       40 2023-03-13 20:43:58.896929 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/APPS.rst
+-rw-r--r--   0        0        0       72 2023-03-13 20:43:58.898598 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/AUTHORS.rst
+-rw-r--r--   0        0        0      152 2023-03-13 20:43:58.899926 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/CHANGELOG.rst
+-rw-r--r--   0        0        0      139 2023-03-13 20:43:58.901141 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/README.rst
+-rw-r--r--   0        0        0     1787 2023-03-13 20:43:58.902561 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/Makefile
+-rw-r--r--   0        0        0       24 2023-03-13 20:43:58.903700 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/api.rst
+-rw-r--r--   0        0        0       25 2023-03-13 20:43:58.905442 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/apps.rst
+-rw-r--r--   0        0        0       28 2023-03-13 20:43:58.908001 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/authors.rst
+-rw-r--r--   0        0        0       30 2023-03-13 20:43:58.909148 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/changelog.rst
+-rwxr-xr-x   0        0        0     5316 2023-03-13 20:43:58.911602 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      391 2023-03-13 20:43:58.913858 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/index.rst
+-rw-r--r--   0        0        0     1290 2023-03-13 20:43:58.916015 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/installation.rst
+-rw-r--r--   0        0        0       27 2023-03-13 20:43:58.917886 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/readme.rst
+-rw-r--r--   0        0        0       72 2023-03-13 20:43:58.919513 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/requirements.txt
+-rw-r--r--   0        0        0      587 2023-03-13 20:43:58.920707 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      230 2023-03-13 20:43:58.922479 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0     1038 2023-03-13 20:43:58.924174 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/tests/{{tmpl.package_name}}/test_{{tmpl.package_name}}.py
+-rw-r--r--   0        0        0      377 2023-03-13 20:43:58.925432 et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/{{tmpl.package_name}}/__init__.py
+-rw-r--r--   0        0        0     4139 2023-06-14 15:23:40.764160 et_micc2-4.0.0/et_micc2/tools/components.py
+-rw-r--r--   0        0        0     4776 2023-06-14 15:23:40.764632 et_micc2-4.0.0/et_micc2/tools/config.py
+-rw-r--r--   0        0        0     6151 2023-06-14 15:23:40.803824 et_micc2-4.0.0/et_micc2/tools/env.py
+-rw-r--r--   0        0        0     4215 2023-06-14 15:23:40.845057 et_micc2-4.0.0/et_micc2/tools/expand.py
+-rw-r--r--   0        0        0     9040 2023-06-14 15:23:40.884905 et_micc2-4.0.0/et_micc2/tools/messages.py
+-rw-r--r--   0        0        0    12596 2023-06-14 15:23:40.925922 et_micc2-4.0.0/et_micc2/tools/project.py
+-rw-r--r--   0        0        0     3663 2023-06-14 15:23:40.965864 et_micc2-4.0.0/et_micc2/tools/tmpl.py
+-rw-r--r--   0        0        0     2263 2023-06-14 15:23:40.966184 et_micc2-4.0.0/et_micc2/tools/tomlfile.py
+-rw-r--r--   0        0        0    10936 2023-06-14 15:23:41.007179 et_micc2-4.0.0/et_micc2/tools/utils.py
+-rw-r--r--   0        0        0      675 2023-06-14 15:28:06.075920 et_micc2-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 et_micc2-4.0.0/PKG-INFO
```

### Comparing `et-micc2-3.2.1/LICENSE` & `et_micc2-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/README.rst` & `et_micc2-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/check_environment.py` & `et_micc2-4.0.0/et_micc2/subcmds/check_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             else:
                 click.secho(f'    {tool} is available:', fg='green')
                 print(f'      {version_string}')
                 print(f'      {which_string}')
                 return True
 
 
-def check_cmd(options):
+def check_env(options):
     """
     """
     
     where = os.environ['VSC_INSTITUTE_CLUSTER'] if 'VSC_HOME' in os.environ else 'local'
     local = where=='local'
 
     print('Python\n'
```

### Comparing `et-micc2-3.2.1/et_micc2/cli_micc.py` & `et_micc2-4.0.0/et_micc2/cli_micc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 # -*- coding: utf-8 -*-
 
 """
 Application micc2
 """
+import os
+from pathlib import Path
+import pkg_resources
+import shutil
 import subprocess
+import sys
+from types import SimpleNamespace
 
+import click
 
+from et_micc2.tools.messages import ExitCodes
 
 def sys_path_helper():
     """Make sure that et_micc2 can be imported in case this file is executed as::
 
             (.venv)> python et_micc2/cli_micc.py <args>
     """
     try:
         import et_micc2
     except ModuleNotFoundError:
         p = Path(__file__) / '..' / '..'
         sys.path.insert(0, str(p.resolve()))
 
-
-import os, sys, shutil
-from types import SimpleNamespace
-from pathlib import Path
-
-import click
-
 sys_path_helper()
-from et_micc2.project import Project, micc_version, error
-import et_micc2.logger
-import et_micc2.config
-import pkg_resources
+
+import et_micc2
+from et_micc2.tools.project import Project
+import et_micc2.tools.config as config
+import et_micc2.tools.messages as messages
+
+from et_micc2.subcmds.add import add as add_cmd
+from et_micc2.subcmds.build import build as build_cmd
+from et_micc2.subcmds.check_env import check_env as check_cmd
+from et_micc2.subcmds.create import create as create_cmd
+from et_micc2.subcmds.doc import doc as doc_cmd
+from et_micc2.subcmds.info import info as info_cmd
+from et_micc2.subcmds.mv import mv as mv_cmd
 
 if '3.8' < sys.version:
-    from et_micc2.check_environment import check_cmd
+    from et_micc2.subcmds.check_env import check_env
 
 __template_help = "Ordered list of Cookiecutter templates, or a single Cookiecutter template."
 
 
 def underscore2space(text):
     return text.replace('_', ' ')
 
@@ -68,14 +78,18 @@
 # main
 ####################################################################################################
 @click.group()
 @click.option('-v', '--verbosity', count=True
     , help="The verbosity of the program output."
     , default=1
 )
+@click.option('-s', '--silent'
+    , help="The verbosity of the program output."
+    , default=False, is_flag=True
+)
 @click.option('-p', '--project-path'
     , help="The path to the project directory. "
            "The default is the current working directory."
     , default='.'
     , type=str
 )
 @click.option('--clear-log'
@@ -109,17 +123,17 @@
 )
 @click.option('--minimal_python_version'
     , help=f"Overwrite preference `minimal_python_version`. (supporting sub-commands only {_subcmds_supporting_overwrite_preferences})"
     , default=''
 )
 # end of preferences overwrite options
 # Don't put any options below, otherwise they will be treated as overwrite preferences.
-@click.version_option(version=micc_version())
+@click.version_option(version=et_micc2.__version__)
 @click.pass_context
-def main( ctx, verbosity, project_path, clear_log
+def main( ctx, verbosity, silent, project_path, clear_log
         , **overwrite_preferences
         ):
     """Micc2 command line interface.
 
     All commands that change the state of the project produce some output that
     is send to the console (taking verbosity into account). It is also sent to
     a logfile ``et_micc2.log`` in the project directory. All output is always appended
@@ -134,21 +148,21 @@
         print(f"micc2 ({et_micc2.__version__}) using Python", sys.version.replace('\n', ' '), end='\n\n')
 
     if clear_log:
         os.remove(project_path / 'micc.log')
 
     ctx.obj = SimpleNamespace(
         verbosity=verbosity,
+        silent=silent,
         project_path=Path(project_path).resolve(),
         default_project_path=(project_path=='.'),
         clear_log=clear_log,
         _cfg_filename=_cfg_filename,
         _cfg_dir=_cfg_dir,
         invoked_subcommand=ctx.invoked_subcommand
-
     )
 
     overwrite_preferences_set = {}
     if ctx.invoked_subcommand in _subcmds_supporting_overwrite_preferences:
         # Remove overwrite_preferences which have not been explicitly set:
         for key,value in overwrite_preferences.items():
             if value:
@@ -163,18 +177,18 @@
     else:
         for key, value in overwrite_preferences.items():
             if value:
                 print(f'Warning: overwriting preferences is supported only for subcommands `setup` and `create`.\n'
                       f'         Ignoring `{key}={value}`.')
 
     try:
-        preferences = et_micc2.config.Config(file_loc=ctx.obj.project_path / _cfg_filename)
+        preferences = config.Config(file_loc=ctx.obj.project_path / _cfg_filename)
     except FileNotFoundError:
         try:
-            preferences = et_micc2.config.Config(file_loc=_cfg_dir / _cfg_filename)
+            preferences = config.Config(file_loc=_cfg_dir / _cfg_filename)
         except FileNotFoundError:
             preferences = None
 
     if preferences is None:
         # no preferences file found
         if ctx.invoked_subcommand == 'setup':
             # we're about to create one.
@@ -252,28 +266,28 @@
         if name in context.overwrite_preferences:
             selected[name] = context.overwrite_preferences[name]
         else:
             if modify: # use the previous setting as default
                 if not 'choices' in description:
                     description['default'] = context.preferences[name]
             try:
-                selected[name] = et_micc2.config.get_param(name, description)
+                selected[name] = config.get_param(name, description)
             except KeyboardInterrupt:
                 print('Interupted - Preferences are not saved.')
                 ctx.exit(1)
 
     # set some preferences for which the default is almost always ok
     selected['version'] = '0.0.0'  # default initial version number of a new projec
     selected["github_repo"] = "{{cookiecutter.project_name}}"  # default github repo name for a project
     selected["git_default_branch"] = "master" # default git branch
     selected["minimal_python_version"] = "3.7"  # default minimal Python version"
     selected["py"] = "py"
 
     # Transfer the selected preferences to a Config object and save it to disk.
-    context.preferences = et_micc2.config.Config(**selected)
+    context.preferences = config.Config(**selected)
     save_to = _cfg_dir / _cfg_filename
     print(f'These preferences are saved to {save_to}:\n{context.preferences}')
     answer = input("Continue? yes/no >:")
     if not answer.lower().startswith('n'):
         context.preferences.save(save_to, mkdir=True)
         print(f'Preferences saved to {save_to}.')
         print('Configuring git:')
@@ -393,50 +407,50 @@
         if not context.default_project_path:
             # global option -p and argument name were both specified.
             print( "ERROR: you specified both global option -p and argument 'name':"
                   f"         -p -> {context.project_path}"
                   f"         name -> {name}"
                    "       You must choose one or the other, not both."
                  )
-            ctx.exit(-1)
+            ctx.exit(ExitCodes.RuntimeError)
         else:
             # overwrite the -p global option so the project will be created:
             context.project_path = Path(name).resolve()
             context.default_project_path = False
 
     # context.package_structure = package
     context.publish = publish
     context.module_name = module_name
     if not remote in ['public','private', 'none']:
         print(f"ERROR: --remote={remote} is not recognized. Valid options are:\n"
               f"       --remote=public\n"
               f"       --remote=private\n"
               f"       --remote=none\n"
               )
-        ctx.exit(-1)
+        ctx.exit(ExitCodes.ValueError)
 
     context.no_git = no_git
     if no_git:
-        context.remote_access = 'none'
+        context.github_repo = 'none'
     else:
-        context.remote_access = None if remote=='none' else remote
+        context.github_repo = None if remote=='none' else remote
 
     context.templates = ['top-level-package']
 
     context.allow_nesting = allow_nesting
 
     context.preferences.update(context.overwrite_preferences)
 
     context.template_parameters = { 'project_short_description': underscore2space(description) }
 
     try:
         project = Project(context)
-        project.create_cmd()
-    except RuntimeError:
-        ctx.exit(2)
+        create_cmd(project)
+    except RuntimeError as runtime_error:
+        ctx.exit(runtime_error.exit_code)
 
 
 ####################################################################################################
 # convert_to_package
 ####################################################################################################
 @main.command()
 @click.option('--overwrite', '-o'
@@ -512,17 +526,17 @@
     if name:
         print(project.package_name)
         return
     if version:
         print(project.version)
         return
     else:
-        with et_micc2.logger.logtime(project):
+        with messages.logtime(project):
             try:
-                project.info_cmd()
+                info_cmd(project)
             except RuntimeError:
                 ctx.exit(project.exit_code)
 
 
 ####################################################################################################
 # version
 ####################################################################################################
@@ -574,40 +588,40 @@
     context.rule = rule
     context.short = short
     context.dry_run = dry_run
 
     try:
         project = Project(context)
     except RuntimeError:
-        ctx.exit(2)
+        ctx.exit(ExitCodes.RuntimeError)
 
     with et_micc2.logger.logtime(project):
         try:
             project.version_cmd()
         except RuntimeError:
-            ctx.exit(2)
+            ctx.exit(ExitCodes.RuntimeError)
         else:
             if tag:
                 project.tag_cmd()
 
 
 ####################################################################################################
 # tag
 ####################################################################################################
 @main.command()
 @click.pass_context
 def tag(ctx):
-    """Create a git tag for the current version and push it to the remote repo."""
+    """Create a git tag and push it to the GitHub repo."""
     context = ctx.obj
 
     try:
         project = Project(context)
         project.tag_cmd()
     except RuntimeError:
-        ctx.exit(2)
+        ctx.exit(ExitCodes.RuntimeError)
 
 
 ####################################################################################################
 # add
 ####################################################################################################
 @main.command()
 @click.option('--cli'
@@ -656,16 +670,17 @@
         # , package
         , f90
         , cpp
         # , templates
         , overwrite
         , backup
         ):
-    """Add a component to the projcect, e.g. CLI, sub-module, sub-package, binary extension 
-    module (C++, Fortran, C++/CUDA )
+    """Add a component to the project
+
+    E.g. a CLI, sub-module, sub-package, binary extension module (C++, Fortran, C++/CUDA ).
 
     :param str name: name of the component. Maybe path-like relative to package directory to
         create sub-sub-modules.
     """
     context = ctx.obj
     context.add_name = name
     
@@ -683,63 +698,61 @@
     context.overwrite = overwrite
     context.backup = backup
 
     try:
         project = Project(context)
         n_selected = cli+clisub+py+f90+cpp # yes, you can add bool variables, they are literally 0|1
         if n_selected == 0:
-            error('You must select a component type:\n    add flag: --py | --cli | --clisub | --f90 | --cpp.')
+            messages.error('You must select a component type:\n    add flag: --py | --cli | --clisub | --f90 | --cpp.')
         if n_selected > 1:
-            error(f'You must select just one component type, not {n_selected}.')
-        with et_micc2.logger.logtime(project):
-            project.add_cmd()
+            messages.error(f'You must select just one component type, not {n_selected}.')
+        with messages.logtime(project):
+            add_cmd(project)
     except RuntimeError as exc:
         ctx.exit(exc.args[1])
 
 
 ####################################################################################################
 # mv
 ####################################################################################################
 @main.command()
-@click.option('--silent', is_flag=True
-    , help="Do not ask for confirmation on deleting a component."
-    , default=False
+@click.option('-m', '--msg', type=str,
+    help="If specified, execute `git commit -a -m <msg>` prior to the mv.",
+    default=''
 )
-@click.option('--entire-package', is_flag=True
-    , help="Replace all occurences of <cur_name> in the entire package and in the ``tests`` directory."
+@click.option('--no-commit', is_flag=True
+    , help="Don't commit the current git status."
     , default=False
 )
-@click.option('--entire-project', is_flag=True
-    , help="Replace all occurences of <cur_name> in the entire project."
-    , default=False
-)
-@click.argument('cur_name', type=str)
-@click.argument('new_name', type=str, default='')
+@click.argument('component', type=str)
+@click.argument('to', default='')
 @click.pass_context
-def mv(ctx, cur_name, new_name, silent, entire_package, entire_project):
-    """Rename or remove a component, i.e an app (CLI) or a submodule.
+def mv(ctx, component, to, msg, no_commit):
+    """Rename, remove or move a component.
 
-    :param cur_name: name of component to be removed or renamed.
-    :param new_name: new name of the component. If empty, the component will be removed.
+    Params:
+        component: name or relative path to the component that is to be renamed, removed or moved.
+        to: New name for <component>, relative path of the component's new location, or ''
+            to remove the component.
     """
     context = ctx.obj
 
-    context.cur_name = cur_name
-    context.new_name = new_name
-    context.silent = silent
-    if new_name:
-        context.entire_package, context.entire_project =  entire_package, entire_project
-    # else these flags are ignored.
+    context.component = component
+    context.to = to
+    if not no_commit:
+        if not msg:
+            msg = f"Commit prior to `micc2 mv {component} {to}`"
+    context.commit_msg = msg
 
     try:
         project = Project(context)
-        with et_micc2.logger.logtime(context):
-            project.mv_component()
-    except RuntimeError:
-        ctx.exit(2)
+        with messages.logtime(context):
+            mv_cmd(project)
+    except RuntimeError as rte:
+        ctx.exit(rte.exit_code)
 
 
 ####################################################################################################
 # build
 ####################################################################################################
 @main.command()
 @click.argument('module', type=str, default='')
@@ -772,45 +785,45 @@
     # Warn for non standard build_type:
     if not build_type in ('','Release', 'Debug', 'RelWithDebInfo', 'MinSizeRel'):
         print(f'[Warning]\nNon-standard build type: `{build_type}`\n'
               f'(Standard build types are: Release, Debug, RelWithDebInfo, MinSizeRel)')
         answer = input('>: Continue? (y/N)')
         if answer != 'y':
             print('')
-            ctx.exit(-1)
+            ctx.exit(ExitCodes.UserInterruptError)
 
     context = ctx.obj
     context.build_options = SimpleNamespace( module_to_build = module
                                            , clean           = clean
                                            , cleanup         = cleanup
                                            , cmake           = {}
                                            )
     if build_type:
         context.build_options.cmake['CMAKE_BUILD_TYPE'] = build_type
 
     try:
         project = Project(context)
-        with et_micc2.logger.logtime(context):
-            project.build_cmd()
-    except RuntimeError:
-        ctx.exit(2)
+        with messages.logtime(context):
+            build_cmd(project)
+    except RuntimeError as runtime_error:
+        ctx.exit(runtime_error.exit_code)
 
 
 ####################################################################################################
 # check
 ####################################################################################################
 @main.command()
 # @click.option('--force', '-f', is_flag=True
 #     , help="Overwrite existing setup."
 #     , default=False
 # )
 @click.pass_context
 def check( ctx
          ):
-    """Check wether the current environment has all the neccessary tools available.
+    """Check the completeness of the environment.
 
     Python packages:
 
     * Numpy
     * Pybind11
     * sphinx
     * sphinx-rtd-theme
@@ -842,21 +855,21 @@
 
     :param str what: this argument is passed to the make command.
     """
     context = ctx.obj
     context.what = what
     try:
         project = Project(context)
-        with et_micc2.logger.logtime(context):
-            project.doc_cmd()
+        with messages.logtime(context):
+            doc_cmd(project)
 
-    except RuntimeError:
-        pass
+    except RuntimeError as runtime_error:
+        ctx.exit(runtime_error.exit_code)
 
-    ctx.exit(project.exit_code)
+    ctx.exit(0)
 
 
 ####################################################################################################
 # venv
 ####################################################################################################
 # @main.command()
 # @click.option('--python'
```

### Comparing `et-micc2-3.2.1/et_micc2/config.py` & `et_micc2-4.0.0/et_micc2/obsolete/config.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/db.py` & `et_micc2-4.0.0/et_micc2/obsolete/db.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/expand.py` & `et_micc2-4.0.0/et_micc2/obsolete/expand.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import click
 # from cookiecutter.main import cookiecutter
 
 import et_micc2.logger
 
 EXIT_OVERWRITE = -3
 __FILE__ = Path(__file__).resolve() 
-import et_micc2.tmpl
+import et_micc2.tools.tmpl
 
 
 def expand_templates(options):
     for template in options.templates:
         path_to_template = Path(__FILE__).parent / 'templates' / template
         if not path_to_template.exists():
             raise RuntimeError(f'Template not found: {path_to_template}')
```

### Comparing `et-micc2-3.2.1/et_micc2/logger.py` & `et_micc2-4.0.0/et_micc2/obsolete/logger.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/micc.json` & `et_micc2-4.0.0/et_micc2/obsolete/micc.json`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/project.py` & `et_micc2-4.0.0/et_micc2/obsolete/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import click
 import semantic_version
 
 import et_micc2.config
 import et_micc2.utils
 import et_micc2.expand
 import et_micc2.logger
-from et_micc2.tomlfile import TomlFile
+from et_micc2.tools.tomlfile import TomlFile
 import pkg_resources
 
 
 __FILE__ = Path(__file__).resolve()
 
 
 def micc_version():
@@ -115,16 +115,14 @@
         if self.which:
             completed_version = subprocess.run([self.exe, '--version'], capture_output=True, text=True)
             self.version = completed_version.stdout.strip().replace('\n\n','\n')#.replace('\n','\n        ')
         else:
             self.version = ''
         return self.version
 
-_exit_missing_component = -1
-
 
 def is_project_directory(path, project=None):
     """Verify that the directory :file:`path` is a project directory. 
 
     :param Path path: path to a directory.
     :param Project project: if not None these variables are set:
```

### Comparing `et-micc2-3.2.1/et_micc2/scripts/install-e.py` & `et_micc2-4.0.0/et_micc2/scripts/install-e.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/static_vars.py` & `et_micc2-4.0.0/et_micc2/obsolete/static_vars.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/app-single-command/{{tmpl.project_name}}/tests/{{tmpl.test_}}{{tmpl.cli_app_name}}.py` & `et_micc2-4.0.0/et_micc2/templates/app-single-command/{{tmpl.project_name}}/tests/{{tmpl.package_name}}/cli/{{tmpl.test_}}{{tmpl.app_name}}.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-"""Tests for `{{tmpl.project_name}}.{{tmpl.cli_app_name}} ` CLI."""
+"""Tests for `{{tmpl.project_name}}.{{tmpl.app_name}} ` CLI."""
 
 from click.testing import CliRunner
 
-from {{tmpl.package_name}}.{{tmpl.cli_app_name}} import main
+from {{tmpl.package_name}}.cli.{{tmpl.app_name}} import main
 
 
 def test_main():
     runner = CliRunner()
     result = runner.invoke(main, ['-vv'])
     print(result.output)
     assert 'running' in result.output
```

### Comparing `et-micc2-3.2.1/et_micc2/templates/app-single-command/{{tmpl.project_name}}/{{tmpl.package_name}}/{{tmpl.cli_app_name}}.py` & `et_micc2-4.0.0/et_micc2/templates/app-single-command/{{tmpl.project_name}}/{{tmpl.package_name}}/cli/{{tmpl.app_name}}.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/app-sub-commands/{{tmpl.project_name}}/tests/{{tmpl.test_]}{{tmpl.cli_app_name}}.py` & `et_micc2-4.0.0/et_micc2/templates/submodule-py-test/{{tmpl.module_name}}/{{tmpl.test_}}{{tmpl.module_name}}.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-"""Tests for `{{tmpl.project_name}}.{{tmpl.cli_app_name}} ` CLI."""
+"""Tests for sub-module {{tmpl.import_lib}}."""
 
 import pytest
+import {{tmpl.import_lib}}
 
-from click.testing import CliRunner
-from click import echo
 
-from click.testing import CliRunner
-
-from {{tmpl.package_name}}.{{tmpl.cli_app_name}} import main
-
-
-def test_hello():
-    runner = CliRunner()
-    result = runner.invoke(main, ['-vv','hello'])
-    print(result.output)
-    assert 'Hello world' in result.output
+def test_greet():
+    expected = "Hello John!"
+    greeting = {{tmpl.package_name}}.{{tmpl.module_name}}.greet("John")
+    assert greeting==expected
 
 
 # ==============================================================================
 # The code below is for debugging a particular test in eclipse/pydev.
 # (normally all tests are run with pytest)
 # ==============================================================================
 if __name__ == "__main__":
-    the_test_you_want_to_debug = test_hello
+    the_test_you_want_to_debug = test_greet
 
-    print(f"__main__ running {the_test_you_want_to_debug}")
+    print("__main__ running", the_test_you_want_to_debug)
     the_test_you_want_to_debug()
-    print('-*# finished #*-')
-# eof
+    print("-*# finished #*-")
+# ==============================================================================
```

### Comparing `et-micc2-3.2.1/et_micc2/templates/app-sub-commands/{{tmpl.project_name}}/{{tmpl.package_name}}/{{tmpl.cli_app_name}}.py` & `et_micc2-4.0.0/et_micc2/templates/app-sub-commands/{{tmpl.project_name}}/{{tmpl.package_name}}/cli/{{tmpl.app_name}}.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/CMakeLists.txt` & `et_micc2-4.0.0/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.cpp` & `et_micc2-4.0.0/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.cpp`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.rst` & `et_micc2-4.0.0/et_micc2/templates/submodule-cpp/{{tmpl.module_name}}/{{tmpl.module_name}}.rst`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-cpp-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py` & `et_micc2-4.0.0/et_micc2/templates/submodule-cpp-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/CMakeLists.txt` & `et_micc2-4.0.0/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.f90` & `et_micc2-4.0.0/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.f90`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.rst` & `et_micc2-4.0.0/et_micc2/templates/submodule-f90/{{tmpl.module_name}}/{{tmpl.module_name}}.rst`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/submodule-f90-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py` & `et_micc2-4.0.0/et_micc2/templates/submodule-f90-test/{{tmpl.module_name}}/test_{{tmpl.module_name}}.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/.gitignore` & `et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/Makefile` & `et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/conf.py` & `et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/installation.rst` & `et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/pyproject.toml` & `et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/templates/top-level-package/{{tmpl.project_name}}/tests/{{tmpl.package_name}}/test_{{tmpl.package_name}}.py` & `et_micc2-4.0.0/et_micc2/templates/top-level-package/{{tmpl.project_name}}/tests/{{tmpl.package_name}}/test_{{tmpl.package_name}}.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/tmpl.py` & `et_micc2-4.0.0/et_micc2/tools/tmpl.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 """
 Package tmpl
 =======================================
 
 Top-level package for tmpl.
 """
 
-__version__ = "0.0.0"
-
-import re,os
+import os
 from pathlib import Path
+import re
 import shutil
 
+
 def expand_string(s, parameters):
     for parameter,value in parameters.items():
         pattern = '{{tmpl.' + parameter +'}}'
-        s = s.replace(pattern, value)
+        s = s.replace(pattern, str(value))
     validate(s)
     return s
 
 def validate(s):
     """Verify that there are no more variables to be replaced.
 
     :param str s: string to be validated
```

### Comparing `et-micc2-3.2.1/et_micc2/tomlfile.py` & `et_micc2-4.0.0/et_micc2/tools/tomlfile.py`

 * *Files identical despite different names*

### Comparing `et-micc2-3.2.1/et_micc2/utils.py` & `et_micc2-4.0.0/et_micc2/obsolete/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import subprocess
 import copy
 from pathlib import Path
 from contextlib import contextmanager
 
 import semantic_version as sv
 
-from et_micc2.tomlfile import TomlFile
+from et_micc2.tools.tomlfile import TomlFile
 import et_micc2.logger
 
 from pypi_simple import PyPISimple
 
 
 def operator_version(version_constraint_string):
     """Split version_constraint_string in operator and version.
```

### Comparing `et-micc2-3.2.1/pyproject.toml` & `et_micc2-4.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "et-micc2"
-version = "3.2.1"
+version = "4.0.0"
 description = "A practical Python project skeleton generator."
 authors = ["Engelbert Tijskens <engelbert.tijskens@uantwerpen.be>"]
 license = "MIT"
 
 readme = 'README.rst'
 
 repository = "https://github.com/etijskens/et-micc2"
```

### Comparing `et-micc2-3.2.1/PKG-INFO` & `et_micc2-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: et-micc2
-Version: 3.2.1
+Version: 4.0.0
 Summary: A practical Python project skeleton generator.
 Home-page: https://github.com/etijskens/et-micc2
 License: MIT
 Keywords: project management
 Author: Engelbert Tijskens
 Author-email: engelbert.tijskens@uantwerpen.be
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7.0,<8.0)
 Requires-Dist: pypi-simple (>=0.8.0,<0.9.0)
 Requires-Dist: semantic_version (>=2.8.3,<3.0.0)
 Requires-Dist: tomlkit (>=0.7.0,<0.8.0)
 Requires-Dist: walkdir (>=0.4.1,<0.5.0)
 Project-URL: Repository, https://github.com/etijskens/et-micc2
 Description-Content-Type: text/x-rst
```

