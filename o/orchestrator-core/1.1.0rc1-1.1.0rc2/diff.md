# Comparing `tmp/orchestrator_core-1.1.0rc1.tar.gz` & `tmp/orchestrator_core-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-1.1.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-1.1.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-1.1.0rc1.tar` & `orchestrator_core-1.1.0rc2.tar`

### file list

```diff
@@ -1,330 +1,364 @@
--rw-r--r--   0        0        0      346 2023-05-24 07:44:35.502022 orchestrator_core-1.1.0rc1/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-05-24 07:44:35.502022 orchestrator_core-1.1.0rc1/.coveragerc
--rw-r--r--   0        0        0     2620 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1163 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2113 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1782 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.gitignore
--rw-r--r--   0        0        0     2074 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.stignore
--rw-r--r--   0        0        0    29835 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/Dockerfile
--rw-r--r--   0        0        0    11409 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/LICENSE
--rw-r--r--   0        0        0      150 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/NOTICE
--rw-r--r--   0        0        0     4965 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/README.md
--rw-r--r--   0        0        0       76 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/codecov.yml
--rw-r--r--   0        0        0       45 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13931 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5641 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0     2080 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/index.md
--rw-r--r--   0        0        0     3897 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/js/termynal.js
--rw-r--r--   0        0        0     5605 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0      771 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     3601 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/mkdocs.yml
--rw-r--r--   0        0        0     1267 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/mutmut_config.py
--rw-r--r--   0        0        0     1098 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2871 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2841 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    12955 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5803 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11510 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      996 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11705 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5636 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/models.py
--rw-r--r--   0        0        0     7395 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13831 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6853 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10653 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9423 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24095 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1439 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      871 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20183 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8943 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4113 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2920 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10288 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/database.py
--rw-r--r--   0        0        0      301 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     3415 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0     4507 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0     1924 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0    23116 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/models.py
--rw-r--r--   0        0        0      104 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     1439 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      240 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0      368 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      346 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0     3413 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16866 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2508 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2533 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3329 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62844 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2694 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2977 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5434 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/forms/validators.py
--rw-r--r--   0        0        0     5091 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     1350 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/ErrorCollectorExtension.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4325 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     2105 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      317 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0     4097 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2576 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     3727 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0      203 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     2259 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0      690 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0      530 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      305 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      980 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0      172 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     2056 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      114 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0      992 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0       39 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40397 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2631 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1293 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3390 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1797 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3586 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/celery.py
--rw-r--r--   0        0        0    22351 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1530 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/products.py
--rw-r--r--   0        0        0     3879 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24204 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5707 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1719 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3708 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/targets.py
--rw-r--r--   0        0        0     9397 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6207 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     3839 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     2785 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8512 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3376 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13148 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7231 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1323 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3312 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33615 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9204 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8335 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0     8839 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4574 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2413 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/setup.cfg
--rw-r--r--   0        0        0      665 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/setup.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5159 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    20143 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    16019 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37706 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2367 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/config.py
--rw-r--r--   0        0        0    21642 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50537 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2824 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7530 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0    10123 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     4594 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0     5174 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26695 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12048 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1871 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12492 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 orchestrator_core-1.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      341 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1163 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2113 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1782 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.gitignore
+-rw-r--r--   0        0        0     2074 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/.stignore
+-rw-r--r--   0        0        0    29835 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/LICENSE
+-rw-r--r--   0        0        0      150 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/NOTICE
+-rw-r--r--   0        0        0     4965 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/README.md
+-rw-r--r--   0        0        0       76 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/codecov.yml
+-rw-r--r--   0        0        0       45 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13931 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0     2080 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/js/termynal.js
+-rw-r--r--   0        0        0     5605 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-05-25 06:10:30.152364 orchestrator_core-1.1.0rc2/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0      771 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     3601 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/mkdocs.yml
+-rw-r--r--   0        0        0     1267 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/mutmut_config.py
+-rw-r--r--   0        0        0     1098 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2871 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2841 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12955 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5803 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11510 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      996 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11705 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5636 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/api/models.py
+-rw-r--r--   0        0        0     7395 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13831 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6853 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10653 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9423 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24095 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1439 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     2371 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generate.md
+-rw-r--r--   0        0        0     5168 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     1758 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/fixed_input.py
+-rw-r--r--   0        0        0     2626 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     2607 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2152 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5811 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1400 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1794 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4234 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1957 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     6559 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      779 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      557 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      553 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      380 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      289 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0     4196 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      337 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      520 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4405 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2639 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1675 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2275 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      514 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     2808 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1764 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1689 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      984 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2391 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20183 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8943 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4113 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2920 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10288 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/db/database.py
+-rw-r--r--   0        0        0      301 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     3415 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4507 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0     1924 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0    23116 2023-05-25 06:10:30.156364 orchestrator_core-1.1.0rc2/orchestrator/db/models.py
+-rw-r--r--   0        0        0      104 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     1439 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      240 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      346 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0     3413 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16866 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2508 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2533 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3329 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62844 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2694 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2977 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5434 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0     5091 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     1350 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/extensions/ErrorCollectorExtension.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4325 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     2105 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      317 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0     4097 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2576 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     3727 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0      203 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     2259 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0      690 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0      530 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      305 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      980 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0      172 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     2056 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      114 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0       39 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40397 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2631 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1293 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3390 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1797 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    22605 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1530 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3879 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24204 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5707 2023-05-25 06:10:30.160364 orchestrator_core-1.1.0rc2/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1719 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3708 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/targets.py
+-rw-r--r--   0        0        0     9397 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6207 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     3839 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     2785 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8512 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3376 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13148 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7231 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1323 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3312 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33615 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9204 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8335 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12830 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4593 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2413 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/setup.cfg
+-rw-r--r--   0        0        0      665 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/setup.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5159 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    20143 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    16019 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37706 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2367 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/config.py
+-rw-r--r--   0        0        0    21642 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50537 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2824 2023-05-25 06:10:30.164364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7530 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0    10123 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     4594 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0     5174 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12048 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1871 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12492 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-05-25 06:10:30.168364 orchestrator_core-1.1.0rc2/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 orchestrator_core-1.1.0rc2/PKG-INFO
```

### Comparing `orchestrator_core-1.1.0rc1/.github/workflows/README.md` & `orchestrator_core-1.1.0rc2/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.github/workflows/build-push-container.yml` & `orchestrator_core-1.1.0rc2/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.github/workflows/codeql-analysis.yml` & `orchestrator_core-1.1.0rc2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.github/workflows/publish-package.yml` & `orchestrator_core-1.1.0rc2/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.github/workflows/run-linting-tests.yml` & `orchestrator_core-1.1.0rc2/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.github/workflows/run-unit-tests.yml` & `orchestrator_core-1.1.0rc2/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.github/workflows/scheduled-build.yml` & `orchestrator_core-1.1.0rc2/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.gitignore` & `orchestrator_core-1.1.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.pre-commit-config.yaml` & `orchestrator_core-1.1.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/.stignore` & `orchestrator_core-1.1.0rc2/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/CHANGELOG.md` & `orchestrator_core-1.1.0rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/LICENSE` & `orchestrator_core-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/README.md` & `orchestrator_core-1.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/cli.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/domainmodels.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/forms.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/openapi.json` & `orchestrator_core-1.1.0rc2/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/python.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/scaling.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/scaling.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
 The `init_app` should be replaced by your own function that at least makes sure that all the workflows are imported
 (which make sure that the are registered) so that the worker can recognize them. This is the minimum implementation
 you need, but you might want to add other initialisation that is needed to execute workflows.
 
 Next we instantiate Celery using our own `OrchestratorCelery` class:
 
 ```python
-broker = f"redis://{AppSettings().CACHE_HOST}:{AppSettings().CACHE_PORT}"
-backend = f"rpc://{AppSettings().CACHE_HOST}:{AppSettings().CACHE_PORT}/0"
+broker = f"redis://{AppSettings().CACHE_URI}"
+backend = f"rpc://{AppSettings().CACHE_URI}/0"
 
 celery = OrchestratorCelery(
     "proj", broker=broker, backend=backend, include=["orchestrator.services.tasks"]
 )
 
 celery.conf.update(result_expires=3600)
 ```
```

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/tasks.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/websockets.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/application/workflow.md` & `orchestrator_core-1.1.0rc2/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/architecture/tldr.md` & `orchestrator_core-1.1.0rc2/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/contributing/guidelines.md` & `orchestrator_core-1.1.0rc2/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/contributing/testing.md` & `orchestrator_core-1.1.0rc2/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/css/termynal.css` & `orchestrator_core-1.1.0rc2/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/getting-started/base.md` & `orchestrator_core-1.1.0rc2/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/getting-started/development.md` & `orchestrator_core-1.1.0rc2/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/index.md` & `orchestrator_core-1.1.0rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/js/custom.js` & `orchestrator_core-1.1.0rc2/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/js/termynal.js` & `orchestrator_core-1.1.0rc2/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/database-migration.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/debian.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/docker.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/domain-models.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/explore.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/input-forms.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/macos.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/overview.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/scenario.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/start-applications.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-1.1.0rc2/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/docs/workshops/images/metadata_products.png` & `orchestrator_core-1.1.0rc2/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/examples/basic/basic_orchestrator.py` & `orchestrator_core-1.1.0rc2/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/mkdocs.yml` & `orchestrator_core-1.1.0rc2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/mutmut_config.py` & `orchestrator_core-1.1.0rc2/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.1.0rc1"
+__version__ = "1.1.0rc2"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/api.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/error_handling.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/api/models.py` & `orchestrator_core-1.1.0rc2/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/app.py` & `orchestrator_core-1.1.0rc2/orchestrator/app.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/database.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/main.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import typer
 
-from orchestrator.cli import database, scheduler
+from orchestrator.cli import database, generate, scheduler
 
 app = typer.Typer()
 app.add_typer(scheduler.app, name="scheduler", help="Access all the scheduler functions")
 app.add_typer(database.app, name="db", help="Interact with the application database")
+app.add_typer(generate.app, name="generate", help="Generate products, workflows and other artifacts")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/migration_helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/cli/scheduler.py` & `orchestrator_core-1.1.0rc2/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/config/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/config/assignee.py` & `orchestrator_core-1.1.0rc2/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/database.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/filters/filters.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/filters/process.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/filters/product.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/models.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/range/range.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/db/sorting/sorting.py` & `orchestrator_core-1.1.0rc2/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/devtools/populator.py` & `orchestrator_core-1.1.0rc2/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/distlock/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-1.1.0rc2/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-1.1.0rc2/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-1.1.0rc2/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/domain/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/domain/base.py` & `orchestrator_core-1.1.0rc2/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/domain/lifecycle.py` & `orchestrator_core-1.1.0rc2/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/exception_handlers.py` & `orchestrator_core-1.1.0rc2/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/forms/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/forms/network_type_validators.py` & `orchestrator_core-1.1.0rc2/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/forms/validators.py` & `orchestrator_core-1.1.0rc2/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/ErrorCollectorExtension.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/extensions/ErrorCollectorExtension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/pagination.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/process.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/product.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/types.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-1.1.0rc2/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/alembic.ini` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/env.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-1.1.0rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schedules/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-1.1.0rc2/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schedules/scheduling.py` & `orchestrator_core-1.1.0rc2/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-1.1.0rc2/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_products.py` & `orchestrator_core-1.1.0rc2/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-1.1.0rc2/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/base.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/engine_settings.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/fixed_input.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/problem_detail.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/process.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/product.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/product_block.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/resource_type.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/schemas/workflow.py` & `orchestrator_core-1.1.0rc2/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/security.py` & `orchestrator_core-1.1.0rc2/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/celery.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/processes.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,21 @@
         user: user who resumed this process
         broadcast_func: Optional function to broadcast process data
 
     Returns:
         process id
 
     """
+    pstat = load_process(process)
+    try:
+        post_process(pstat.log[0].form, pstat.state.unwrap(), user_inputs=user_inputs or [])
+    except FormValidationError:
+        logger.exception("Validation errors", user_inputs=user_inputs)
+        raise
+
     resume_func = get_execution_context()["resume"]
     return resume_func(process, user_inputs=user_inputs, user=user, broadcast_func=broadcast_func)
 
 
 async def _async_resume_processes(
     processes: List[ProcessTable],
     user_name: str,
```

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/products.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/settings.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/subscriptions.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/tasks.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/services/translations.py` & `orchestrator_core-1.1.0rc2/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/settings.py` & `orchestrator_core-1.1.0rc2/orchestrator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/targets.py` & `orchestrator_core-1.1.0rc2/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/types.py` & `orchestrator_core-1.1.0rc2/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/crypt.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/datetime.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/docs.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/errors.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/functional.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/helpers.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/json.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/redis.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/show_process.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/speed.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/state.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/strings.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/utils/vlans.py` & `orchestrator_core-1.1.0rc2/orchestrator/utils/vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/version.py` & `orchestrator_core-1.1.0rc2/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/websocket/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-1.1.0rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-1.1.0rc2/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-1.1.0rc2/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflow.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/modify_note.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/steps.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/orchestrator/workflows/utils.py` & `orchestrator_core-1.1.0rc2/orchestrator/workflows/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,22 +20,25 @@
 
 from orchestrator.db import ProductTable, SubscriptionTable
 from orchestrator.forms import FormPage
 from orchestrator.forms.validators import ProductId
 from orchestrator.services import subscriptions
 from orchestrator.settings import app_settings
 from orchestrator.targets import Target
-from orchestrator.types import FormGenerator, InputForm, InputStepFunc, State, StateInputStepFunc
+from orchestrator.types import FormGenerator, InputForm, InputStepFunc, State, StateInputStepFunc, SubscriptionLifecycle
+from orchestrator.utils.redis import caching_models_enabled
 from orchestrator.utils.state import form_inject_args
-from orchestrator.workflow import StepList, Workflow, conditional, done, init, make_workflow, step
+from orchestrator.workflow import Step, StepList, Workflow, conditional, done, init, make_workflow, step
 from orchestrator.workflows.steps import (
     cache_domain_models,
     remove_domain_model_from_cache,
     resync,
+    set_status,
     store_process_subscription,
+    unsync,
     unsync_unchecked,
 )
 
 
 def _generate_new_subscription_form(workflow_target: str, workflow_name: str) -> InputForm:
     class NewProductPage(FormPage):
         product: ProductId
@@ -171,14 +174,129 @@
 
 
 modify_initial_input_form_generator = None
 
 
 validate_initial_input_form_generator = wrap_modify_initial_input_form(modify_initial_input_form_generator)
 
+push_domain_models = conditional(lambda _: caching_models_enabled())
+
+
+def create_workflow(
+    description: str,
+    initial_input_form: Optional[InputStepFunc] = None,
+    status: SubscriptionLifecycle = SubscriptionLifecycle.ACTIVE,
+    update_ticket_step: Optional[Step] = None,
+) -> Callable[[Callable[[], StepList]], Workflow]:
+    """Transform an initial_input_form and a step list into a workflow with a target=Target.CREATE.
+
+    Use this for create workflows only.
+
+    Example::
+
+        @create_workflow("create service port")
+        def create_service_port() -> StepList:
+            do_something
+            >> do_something_else
+    """
+    create_initial_input_form_generator = wrap_create_initial_input_form(initial_input_form)
+
+    def _create_workflow(f: Callable[[], StepList]) -> Workflow:
+        execute_ticket_step = conditional(lambda state: state.get("ticket_id", False))
+        steplist = (
+            init
+            >> f()
+            >> execute_ticket_step(update_ticket_step)
+            >> set_status(status)
+            >> resync
+            >> push_domain_models(cache_domain_models)
+            >> done
+        )
+
+        return make_workflow(f, description, create_initial_input_form_generator, Target.CREATE, steplist)
+
+    return _create_workflow
+
+
+def modify_workflow(
+    description: str,
+    initial_input_form: Optional[InputStepFunc] = None,
+    update_ticket_step: Optional[Step] = None,
+) -> Callable[[Callable[[], StepList]], Workflow]:
+    """Transform an initial_input_form and a step list into a workflow.
+
+    Use this for modify workflows.
+
+    Example::
+
+        @modify_workflow("create service port") -> StepList:
+        def create_service_port():
+            do_something
+            >> do_something_else
+    """
+
+    wrapped_modify_initial_input_form_generator = wrap_modify_initial_input_form(initial_input_form)
+
+    def _modify_workflow(f: Callable[[], StepList]) -> Workflow:
+        execute_ticket_step = conditional(lambda state: state.get("ticket_id", False))
+        steplist = (
+            init
+            >> store_process_subscription(Target.MODIFY)
+            >> push_domain_models(remove_domain_model_from_cache)
+            >> unsync
+            >> f()
+            >> execute_ticket_step(update_ticket_step)
+            >> resync
+            >> push_domain_models(cache_domain_models)
+            >> done
+        )
+
+        return make_workflow(f, description, wrapped_modify_initial_input_form_generator, Target.MODIFY, steplist)
+
+    return _modify_workflow
+
+
+def terminate_workflow(
+    description: str,
+    initial_input_form: Optional[InputStepFunc] = None,
+    update_ticket_step: Optional[Step] = None,
+) -> Callable[[Callable[[], StepList]], Workflow]:
+    """Transform an initial_input_form and a step list into a workflow.
+
+    Use this for terminate workflows.
+
+    Example::
+
+        @terminate_workflow("create service port") -> StepList:
+        def create_service_port():
+            do_something
+            >> do_something_else
+    """
+
+    wrapped_terminate_initial_input_form_generator = wrap_modify_initial_input_form(initial_input_form)
+
+    def _terminate_workflow(f: Callable[[], StepList]) -> Workflow:
+        execute_ticket_step = conditional(lambda state: state.get("ticket_id", False))
+        steplist = (
+            init
+            >> store_process_subscription(Target.TERMINATE)
+            >> push_domain_models(remove_domain_model_from_cache)
+            >> unsync
+            >> f()
+            >> execute_ticket_step(update_ticket_step)
+            >> set_status(SubscriptionLifecycle.TERMINATED)
+            >> resync
+            >> push_domain_models(cache_domain_models)
+            >> done
+        )
+
+        return make_workflow(f, description, wrapped_terminate_initial_input_form_generator, Target.TERMINATE, steplist)
+
+    return _terminate_workflow
+
 
 def validate_workflow(description: str) -> Callable[[Callable[[], StepList]], Workflow]:
     """Transform an initial_input_form and a step list into a workflow.
 
     Use this for subscription validate workflows.
 
     Example::
```

### Comparing `orchestrator_core-1.1.0rc1/pyproject.toml` & `orchestrator_core-1.1.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     "types-python-dateutil",
     "types-pytz",
     "types-redis",
     "types-requests",
     "types-tabulate",
     "types-toml",
     "types-ujson",
+    "types-PyYAML"
 ]
 doc = [
     "mkdocs",
     "mkdocs-material",
     "mkdocs-render-swagger-plugin",
     "mkdocs-include-markdown-plugin"
 ]
```

### Comparing `orchestrator_core-1.1.0rc1/setup.cfg` & `orchestrator_core-1.1.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/setup.py` & `orchestrator_core-1.1.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/acceptance_tests/conftest.py` & `orchestrator_core-1.1.0rc2/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-1.1.0rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/acceptance_tests/test_test_product.py` & `orchestrator_core-1.1.0rc2/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_caching.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_health.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_helpers.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_models.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_products.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_settings.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_workflows.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/conftest.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/processes.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/forms/shared.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_network_validators.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_post_process.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/graphql/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_product.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_processes.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_products.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_translations.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/test_db.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/test_workflow.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_errors.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_functional.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_json.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_speed.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_state.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_vlans.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/__init__.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-1.1.0rc2/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.0rc1/PKG-INFO` & `orchestrator_core-1.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Open source orchestration software for NREN's
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -111,12 +111,13 @@
 Requires-Dist: types-python-dateutil ; extra == "test"
 Requires-Dist: types-pytz ; extra == "test"
 Requires-Dist: types-redis ; extra == "test"
 Requires-Dist: types-requests ; extra == "test"
 Requires-Dist: types-tabulate ; extra == "test"
 Requires-Dist: types-toml ; extra == "test"
 Requires-Dist: types-ujson ; extra == "test"
+Requires-Dist: types-PyYAML ; extra == "test"
 Project-URL: documentation, https://workfloworchestrator.org/orchestrator-core/
 Provides-Extra: celery
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
```

