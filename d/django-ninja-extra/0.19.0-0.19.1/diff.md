# Comparing `tmp/django_ninja_extra-0.19.0.tar.gz` & `tmp/django_ninja_extra-0.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_extra-0.19.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_ninja_extra-0.19.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_ninja_extra-0.19.0.tar` & `django_ninja_extra-0.19.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0      269 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.coveragerc
--rw-r--r--   0        0        0       64 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.dockerignore
--rw-r--r--   0        0        0      126 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.flake8
--rw-r--r--   0        0        0      528 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/dependabot.yml
--rw-r--r--   0        0        0      661 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      571 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1323 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/workflows/test_full.yml
--rw-r--r--   0        0        0      114 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.gitignore
--rw-r--r--   0        0        0       52 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.isort.cfg
--rw-r--r--   0        0        0     1069 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1082 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/LICENSE
--rw-r--r--   0        0        0      968 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/Makefile
--rw-r--r--   0        0        0     3989 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/README.md
--rw-r--r--   0        0        0     3371 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/api_controller_permission.md
--rw-r--r--   0        0        0     3476 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/api_controller_route.md
--rw-r--r--   0        0        0     1546 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/api_controller_router.md
--rw-r--r--   0        0        0     7774 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/index.md
--rw-r--r--   0        0        0    51900 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/images/benchmark.png
--rw-r--r--   0        0        0  1100522 2023-06-08 21:53:49.993941 django_ninja_extra-0.19.0/docs/images/custom_exception.gif
--rwxr-xr-x   0        0        0  5136836 2023-06-08 21:53:50.021942 django_ninja_extra-0.19.0/docs/images/pagination_example.gif
--rw-r--r--   0        0        0  1478750 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/images/ui_swagger_preview_readme.gif
--rw-r--r--   0        0        0     4038 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/index.md
--rw-r--r--   0        0        0     5705 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/route_context.md
--rw-r--r--   0        0        0    12801 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/service_module_injector.md
--rw-r--r--   0        0        0     2028 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/settings.md
--rw-r--r--   0        0        0     2694 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/authentication.md
--rw-r--r--   0        0        0     1497 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/body_request.md
--rw-r--r--   0        0        0      975 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/custom_exception.md
--rw-r--r--   0        0        0     1025 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/form.md
--rw-r--r--   0        0        0     2958 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/index.md
--rw-r--r--   0        0        0     2782 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/ordering.md
--rw-r--r--   0        0        0     2324 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/pagination.md
--rw-r--r--   0        0        0      595 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/path.md
--rw-r--r--   0        0        0      756 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/query.md
--rw-r--r--   0        0        0     1276 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/schema.md
--rw-r--r--   0        0        0     3621 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/searching.md
--rw-r--r--   0        0        0     1847 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/testing.md
--rw-r--r--   0        0        0     7330 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/throttling.md
--rw-r--r--   0        0        0     2064 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/versioning.md
--rw-r--r--   0        0        0     1778 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/mkdocs.yml
--rw-r--r--   0        0        0      414 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/mypy.ini
--rw-r--r--   0        0        0     1087 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/__init__.py
--rw-r--r--   0        0        0     1291 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/apps.py
--rw-r--r--   0        0        0      440 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/compatible.py
--rw-r--r--   0        0        0       55 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/conf/__init__.py
--rw-r--r--   0        0        0     3554 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/conf/settings.py
--rw-r--r--   0        0        0      276 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/constants.py
--rw-r--r--   0        0        0      700 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/__init__.py
--rw-r--r--   0        0        0    17997 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/base.py
--rw-r--r--   0        0        0     1313 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/registry.py
--rw-r--r--   0        0        0     6265 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/response.py
--rw-r--r--   0        0        0    25969 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/route/__init__.py
--rw-r--r--   0        0        0     1125 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/route/context.py
--rw-r--r--   0        0        0     7744 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/route/route_functions.py
--rw-r--r--   0        0        0     1434 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/dependency_resolver.py
--rw-r--r--   0        0        0     1876 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/details.py
--rw-r--r--   0        0        0     8814 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/exceptions.py
--rw-r--r--   0        0        0     1775 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/generic.py
--rw-r--r--   0        0        0      597 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/helper.py
--rw-r--r--   0        0        0      670 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/lazy.py
--rw-r--r--   0        0        0       61 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/logger.py
--rw-r--r--   0        0        0     4322 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/main.py
--rw-r--r--   0        0        0     1305 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/modules.py
--rw-r--r--   0        0        0    19913 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/operation.py
--rw-r--r--   0        0        0     8324 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/ordering.py
--rw-r--r--   0        0        0     8259 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/pagination.py
--rw-r--r--   0        0        0      281 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/permissions/__init__.py
--rw-r--r--   0        0        0     5311 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/permissions/base.py
--rw-r--r--   0        0        0     1622 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/permissions/common.py
--rw-r--r--   0        0        0        0 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/py.typed
--rw-r--r--   0        0        0     2194 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/router.py
--rw-r--r--   0        0        0      313 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/schemas/__init__.py
--rw-r--r--   0        0        0     3573 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/schemas/response.py
--rw-r--r--   0        0        0     9412 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/searching.py
--rw-r--r--   0        0        0      748 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/__init__.py
--rw-r--r--   0        0        0      880 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/api_key.py
--rw-r--r--   0        0        0     1705 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/http.py
--rw-r--r--   0        0        0      542 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/session.py
--rw-r--r--   0        0        0     2516 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/shortcuts.py
--rw-r--r--   0        0        0      103 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/signals.py
--rw-r--r--   0        0        0     2515 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/status.py
--rw-r--r--   0        0        0      112 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/testing/__init__.py
--rw-r--r--   0        0        0     2059 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/testing/client.py
--rw-r--r--   0        0        0      318 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/throttling/__init__.py
--rw-r--r--   0        0        0     3921 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/throttling/decorator.py
--rw-r--r--   0        0        0     8211 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/throttling/model.py
--rw-r--r--   0        0        0      267 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/types.py
--rw-r--r--   0        0        0     1116 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/urls.py
--rw-r--r--   0        0        0     2392 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/pyproject.toml
--rwxr-xr-x   0        0        0       61 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/pytest.ini
--rw-r--r--   0        0        0        0 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/__init__.py
--rw-r--r--   0        0        0     2181 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/conftest.py
--rw-r--r--   0        0        0     1332 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/controllers.py
--rw-r--r--   0        0        0      495 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/models.py
--rw-r--r--   0        0        0       89 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/schemas.py
--rw-r--r--   0        0        0     2121 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_api_instance.py
--rw-r--r--   0        0        0     7322 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_async_auth.py
--rw-r--r--   0        0        0    13342 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_controller.py
--rw-r--r--   0        0        0     1571 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_controller_registry.py
--rw-r--r--   0        0        0     2725 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_controller_response.py
--rw-r--r--   0        0        0     1871 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_dependency_resolver.py
--rw-r--r--   0        0        0     1059 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_django_model.py
--rw-r--r--   0        0        0     3533 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_django_ninja_router.py
--rw-r--r--   0        0        0     2157 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_event_controller.py
--rw-r--r--   0        0        0     6706 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     2048 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_generic_patch.py
--rw-r--r--   0        0        0      460 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_lazy_import.py
--rw-r--r--   0        0        0     4227 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_operation.py
--rw-r--r--   0        0        0    14220 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_ordering.py
--rw-r--r--   0        0        0    12132 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_pagination.py
--rw-r--r--   0        0        0    10048 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_permissions.py
--rw-r--r--   0        0        0    15512 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_route.py
--rw-r--r--   0        0        0    13597 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_searching.py
--rw-r--r--   0        0        0     2316 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_settings.py
--rw-r--r--   0        0        0     2466 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_shortcuts.py
--rw-r--r--   0        0        0     1051 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_status.py
--rw-r--r--   0        0        0     1274 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_testclient.py
--rw-r--r--   0        0        0        0 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/__init__.py
--rw-r--r--   0        0        0      461 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/sample_models.py
--rw-r--r--   0        0        0    10309 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_decorator.py
--rw-r--r--   0        0        0     7286 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_models.py
--rw-r--r--   0        0        0     2797 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_controller.py
--rw-r--r--   0        0        0     3536 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_decorator_on_controllers.py
--rw-r--r--   0        0        0     3345 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_throttling_xxf.py
--rw-r--r--   0        0        0      293 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/urls.py
--rw-r--r--   0        0        0     1769 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/utils.py
--rw-r--r--   0        0        0     6958 1970-01-01 00:00:00.000000 django_ninja_extra-0.19.0/PKG-INFO
+-rw-r--r--   0        0        0      269 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.coveragerc
+-rw-r--r--   0        0        0       64 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.dockerignore
+-rw-r--r--   0        0        0      126 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.flake8
+-rw-r--r--   0        0        0      528 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      661 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      571 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1323 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0      114 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.gitignore
+-rw-r--r--   0        0        0       52 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.isort.cfg
+-rw-r--r--   0        0        0     1069 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1082 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/LICENSE
+-rw-r--r--   0        0        0      968 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/Makefile
+-rw-r--r--   0        0        0     3989 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/README.md
+-rw-r--r--   0        0        0     3371 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/docs/api_controller/api_controller_permission.md
+-rw-r--r--   0        0        0     3476 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/docs/api_controller/api_controller_route.md
+-rw-r--r--   0        0        0     1546 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/docs/api_controller/api_controller_router.md
+-rw-r--r--   0        0        0     7774 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/docs/api_controller/index.md
+-rw-r--r--   0        0        0    51900 2023-06-14 13:32:44.365382 django_ninja_extra-0.19.1/docs/images/benchmark.png
+-rw-r--r--   0        0        0  1100522 2023-06-14 13:32:44.373382 django_ninja_extra-0.19.1/docs/images/custom_exception.gif
+-rwxr-xr-x   0        0        0  5136836 2023-06-14 13:32:44.401382 django_ninja_extra-0.19.1/docs/images/pagination_example.gif
+-rw-r--r--   0        0        0  1478750 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/images/ui_swagger_preview_readme.gif
+-rw-r--r--   0        0        0     4038 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/index.md
+-rw-r--r--   0        0        0     5705 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/route_context.md
+-rw-r--r--   0        0        0    12801 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/service_module_injector.md
+-rw-r--r--   0        0        0     2028 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/settings.md
+-rw-r--r--   0        0        0     2710 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/authentication.md
+-rw-r--r--   0        0        0     1497 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/body_request.md
+-rw-r--r--   0        0        0      975 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/custom_exception.md
+-rw-r--r--   0        0        0     1025 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/form.md
+-rw-r--r--   0        0        0     2958 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/index.md
+-rw-r--r--   0        0        0     2782 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/ordering.md
+-rw-r--r--   0        0        0     2324 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/pagination.md
+-rw-r--r--   0        0        0      595 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/path.md
+-rw-r--r--   0        0        0      756 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/query.md
+-rw-r--r--   0        0        0     1276 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/schema.md
+-rw-r--r--   0        0        0     3621 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/searching.md
+-rw-r--r--   0        0        0     1847 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     7330 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/throttling.md
+-rw-r--r--   0        0        0     2064 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/docs/tutorial/versioning.md
+-rw-r--r--   0        0        0     1778 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/mkdocs.yml
+-rw-r--r--   0        0        0      414 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/mypy.ini
+-rw-r--r--   0        0        0     1087 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/__init__.py
+-rw-r--r--   0        0        0     1291 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/apps.py
+-rw-r--r--   0        0        0      440 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/compatible.py
+-rw-r--r--   0        0        0       55 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/conf/__init__.py
+-rw-r--r--   0        0        0     3554 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/conf/settings.py
+-rw-r--r--   0        0        0      276 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/constants.py
+-rw-r--r--   0        0        0      700 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/controllers/__init__.py
+-rw-r--r--   0        0        0    17997 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/controllers/base.py
+-rw-r--r--   0        0        0     1313 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/controllers/registry.py
+-rw-r--r--   0        0        0     6265 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/controllers/response.py
+-rw-r--r--   0        0        0    25969 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/controllers/route/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/controllers/route/context.py
+-rw-r--r--   0        0        0     7744 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/controllers/route/route_functions.py
+-rw-r--r--   0        0        0     1434 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/dependency_resolver.py
+-rw-r--r--   0        0        0     1876 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/details.py
+-rw-r--r--   0        0        0     8814 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/exceptions.py
+-rw-r--r--   0        0        0     1775 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/generic.py
+-rw-r--r--   0        0        0      597 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/helper.py
+-rw-r--r--   0        0        0      670 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/lazy.py
+-rw-r--r--   0        0        0       61 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/logger.py
+-rw-r--r--   0        0        0     4322 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/main.py
+-rw-r--r--   0        0        0     1305 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/modules.py
+-rw-r--r--   0        0        0    19913 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/operation.py
+-rw-r--r--   0        0        0     8324 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/ordering.py
+-rw-r--r--   0        0        0     8259 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/pagination.py
+-rw-r--r--   0        0        0      281 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/permissions/__init__.py
+-rw-r--r--   0        0        0     5311 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/permissions/base.py
+-rw-r--r--   0        0        0     1622 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/permissions/common.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/py.typed
+-rw-r--r--   0        0        0     2194 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/router.py
+-rw-r--r--   0        0        0      313 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/schemas/__init__.py
+-rw-r--r--   0        0        0     3809 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/schemas/response.py
+-rw-r--r--   0        0        0     9412 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/searching.py
+-rw-r--r--   0        0        0      748 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/security/__init__.py
+-rw-r--r--   0        0        0      880 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/security/api_key.py
+-rw-r--r--   0        0        0     1705 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/security/http.py
+-rw-r--r--   0        0        0      542 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/security/session.py
+-rw-r--r--   0        0        0     2516 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/shortcuts.py
+-rw-r--r--   0        0        0      103 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/signals.py
+-rw-r--r--   0        0        0     2515 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/status.py
+-rw-r--r--   0        0        0      112 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2059 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/testing/client.py
+-rw-r--r--   0        0        0      318 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/throttling/__init__.py
+-rw-r--r--   0        0        0     3921 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/throttling/decorator.py
+-rw-r--r--   0        0        0     8211 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/throttling/model.py
+-rw-r--r--   0        0        0      267 2023-06-14 13:32:44.413382 django_ninja_extra-0.19.1/ninja_extra/types.py
+-rw-r--r--   0        0        0     1116 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/ninja_extra/urls.py
+-rw-r--r--   0        0        0     2392 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/pyproject.toml
+-rwxr-xr-x   0        0        0       61 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/pytest.ini
+-rw-r--r--   0        0        0        0 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/__init__.py
+-rw-r--r--   0        0        0     2181 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/conftest.py
+-rw-r--r--   0        0        0     1332 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/controllers.py
+-rw-r--r--   0        0        0      495 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/models.py
+-rw-r--r--   0        0        0       89 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/schemas.py
+-rw-r--r--   0        0        0     2121 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_api_instance.py
+-rw-r--r--   0        0        0     7322 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_async_auth.py
+-rw-r--r--   0        0        0    13342 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_controller.py
+-rw-r--r--   0        0        0     1571 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_controller_registry.py
+-rw-r--r--   0        0        0     2725 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_controller_response.py
+-rw-r--r--   0        0        0     1871 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_dependency_resolver.py
+-rw-r--r--   0        0        0     1059 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_django_model.py
+-rw-r--r--   0        0        0     3533 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_django_ninja_router.py
+-rw-r--r--   0        0        0     2157 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_event_controller.py
+-rw-r--r--   0        0        0     6706 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     2048 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_generic_patch.py
+-rw-r--r--   0        0        0      460 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_lazy_import.py
+-rw-r--r--   0        0        0     4227 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_operation.py
+-rw-r--r--   0        0        0    14220 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_ordering.py
+-rw-r--r--   0        0        0    12685 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_pagination.py
+-rw-r--r--   0        0        0    10048 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_permissions.py
+-rw-r--r--   0        0        0    15512 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_route.py
+-rw-r--r--   0        0        0    13597 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_searching.py
+-rw-r--r--   0        0        0     2316 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_settings.py
+-rw-r--r--   0        0        0     2466 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_shortcuts.py
+-rw-r--r--   0        0        0     1051 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_status.py
+-rw-r--r--   0        0        0     1274 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_testclient.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_throthling/__init__.py
+-rw-r--r--   0        0        0      461 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_throthling/sample_models.py
+-rw-r--r--   0        0        0    10309 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_throthling/test_decorator.py
+-rw-r--r--   0        0        0     7286 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_throthling/test_models.py
+-rw-r--r--   0        0        0     2797 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_throthling/test_throttle_controller.py
+-rw-r--r--   0        0        0     3536 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_throthling/test_throttle_decorator_on_controllers.py
+-rw-r--r--   0        0        0     3345 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/test_throthling/test_throttling_xxf.py
+-rw-r--r--   0        0        0      293 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/urls.py
+-rw-r--r--   0        0        0     1769 2023-06-14 13:32:44.417382 django_ninja_extra-0.19.1/tests/utils.py
+-rw-r--r--   0        0        0     6958 1970-01-01 00:00:00.000000 django_ninja_extra-0.19.1/PKG-INFO
```

### Comparing `django_ninja_extra-0.19.0/.github/dependabot.yml` & `django_ninja_extra-0.19.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/.github/workflows/publish.yml` & `django_ninja_extra-0.19.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/.github/workflows/test.yml` & `django_ninja_extra-0.19.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/.github/workflows/test_full.yml` & `django_ninja_extra-0.19.1/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/.pre-commit-config.yaml` & `django_ninja_extra-0.19.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/LICENSE` & `django_ninja_extra-0.19.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/Makefile` & `django_ninja_extra-0.19.1/Makefile`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/README.md` & `django_ninja_extra-0.19.1/README.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/api_controller/api_controller_permission.md` & `django_ninja_extra-0.19.1/docs/api_controller/api_controller_permission.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/api_controller/api_controller_route.md` & `django_ninja_extra-0.19.1/docs/api_controller/api_controller_route.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/api_controller/api_controller_router.md` & `django_ninja_extra-0.19.1/docs/api_controller/api_controller_router.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/api_controller/index.md` & `django_ninja_extra-0.19.1/docs/api_controller/index.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/images/benchmark.png` & `django_ninja_extra-0.19.1/docs/images/benchmark.png`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/images/custom_exception.gif` & `django_ninja_extra-0.19.1/docs/images/custom_exception.gif`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/images/pagination_example.gif` & `django_ninja_extra-0.19.1/docs/images/pagination_example.gif`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/images/ui_swagger_preview_readme.gif` & `django_ninja_extra-0.19.1/docs/images/ui_swagger_preview_readme.gif`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/index.md` & `django_ninja_extra-0.19.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/route_context.md` & `django_ninja_extra-0.19.1/docs/route_context.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/service_module_injector.md` & `django_ninja_extra-0.19.1/docs/service_module_injector.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/settings.md` & `django_ninja_extra-0.19.1/docs/settings.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/authentication.md` & `django_ninja_extra-0.19.1/docs/tutorial/authentication.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         if token == "supersecret":
             return token
 
 @api_controller(tags=['My Operations'], auth=NOT_SET, permissions=[])
 class MyController:
     @route.get("/bearer", auth=AuthBearer())
     def bearer(self):
-        return {"token": self.request.auth}
+        return {"token": self.context.request.auth}
 
 ```
 
 ## **Global authentication** 
 
 In case you need to secure **all** route methods defined in `api` and APIController, you can pass the `auth` argument to the `NinjaExtraAPI` constructor:
 
@@ -69,15 +69,15 @@
             return token
 
 
 @api_controller(tags=['My Operations'], auth=NOT_SET, permissions=[])
 class MyController:
     @route.get("/bearer", auth=AuthBearer())
     async def bearer(self):
-        return {"token": self.request.auth}
+        return {"token": self.context.request.auth}
 
 ```
 In example above, we changed `HttpBearer` to `AsyncHttpBearer` and changed bearer to `async` endpoint. 
 If `AuthBearer` is to be applied to a `MyController` **auth**, then all route handlers under `MyController` must be asynchronous route handlers.
 
 
 ## **JWT Authentication**
```

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/body_request.md` & `django_ninja_extra-0.19.1/docs/tutorial/body_request.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/custom_exception.md` & `django_ninja_extra-0.19.1/docs/tutorial/custom_exception.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/form.md` & `django_ninja_extra-0.19.1/docs/tutorial/form.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/index.md` & `django_ninja_extra-0.19.1/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/ordering.md` & `django_ninja_extra-0.19.1/docs/tutorial/ordering.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/pagination.md` & `django_ninja_extra-0.19.1/docs/tutorial/pagination.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/path.md` & `django_ninja_extra-0.19.1/docs/tutorial/path.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/query.md` & `django_ninja_extra-0.19.1/docs/tutorial/query.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/schema.md` & `django_ninja_extra-0.19.1/docs/tutorial/schema.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/searching.md` & `django_ninja_extra-0.19.1/docs/tutorial/searching.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/testing.md` & `django_ninja_extra-0.19.1/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/throttling.md` & `django_ninja_extra-0.19.1/docs/tutorial/throttling.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/docs/tutorial/versioning.md` & `django_ninja_extra-0.19.1/docs/tutorial/versioning.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/mkdocs.yml` & `django_ninja_extra-0.19.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/__init__.py` & `django_ninja_extra-0.19.1/ninja_extra/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)"""
 
-__version__ = "0.19.0"
+__version__ = "0.19.1"
 
 import django
 
 from ninja_extra.controllers import (
     ControllerBase,
     api_controller,
     http_delete,
```

### Comparing `django_ninja_extra-0.19.0/ninja_extra/apps.py` & `django_ninja_extra-0.19.1/ninja_extra/apps.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/conf/settings.py` & `django_ninja_extra-0.19.1/ninja_extra/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/controllers/__init__.py` & `django_ninja_extra-0.19.1/ninja_extra/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/controllers/base.py` & `django_ninja_extra-0.19.1/ninja_extra/controllers/base.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/controllers/registry.py` & `django_ninja_extra-0.19.1/ninja_extra/controllers/registry.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/controllers/response.py` & `django_ninja_extra-0.19.1/ninja_extra/controllers/response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/controllers/route/__init__.py` & `django_ninja_extra-0.19.1/ninja_extra/controllers/route/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/controllers/route/context.py` & `django_ninja_extra-0.19.1/ninja_extra/controllers/route/context.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/controllers/route/route_functions.py` & `django_ninja_extra-0.19.1/ninja_extra/controllers/route/route_functions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/dependency_resolver.py` & `django_ninja_extra-0.19.1/ninja_extra/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/details.py` & `django_ninja_extra-0.19.1/ninja_extra/details.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/exceptions.py` & `django_ninja_extra-0.19.1/ninja_extra/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/generic.py` & `django_ninja_extra-0.19.1/ninja_extra/generic.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/helper.py` & `django_ninja_extra-0.19.1/ninja_extra/helper.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/lazy.py` & `django_ninja_extra-0.19.1/ninja_extra/lazy.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/main.py` & `django_ninja_extra-0.19.1/ninja_extra/main.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/modules.py` & `django_ninja_extra-0.19.1/ninja_extra/modules.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/operation.py` & `django_ninja_extra-0.19.1/ninja_extra/operation.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/ordering.py` & `django_ninja_extra-0.19.1/ninja_extra/ordering.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/pagination.py` & `django_ninja_extra-0.19.1/ninja_extra/pagination.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/permissions/base.py` & `django_ninja_extra-0.19.1/ninja_extra/permissions/base.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/permissions/common.py` & `django_ninja_extra-0.19.1/ninja_extra/permissions/common.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/router.py` & `django_ninja_extra-0.19.1/ninja_extra/router.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/schemas/response.py` & `django_ninja_extra-0.19.1/ninja_extra/schemas/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from typing import Any, Dict, Generic, List, Optional, Type, TypeVar
 
 from ninja import Schema
 from ninja.constants import NOT_SET
+from pydantic import validator
 from pydantic.generics import GenericModel
 from pydantic.main import BaseModel
 from pydantic.networks import AnyHttpUrl
 
 from ninja_extra.generic import GenericType
 
 T = TypeVar("T")
@@ -82,14 +83,20 @@
     PaginatedResponseSchema.__generic_model__ = PaginatedResponseSchema
 
     class NinjaPaginationResponseSchema(
         GenericModel, Generic[T], BaseNinjaResponseSchema
     ):
         items: List[T]
 
+        @validator("items", pre=True)
+        def validate_items(cls, value: Any) -> Any:
+            if value and not isinstance(value, list):
+                return list(value)
+            return value
+
     NinjaPaginationResponseSchema.__generic_model__ = NinjaPaginationResponseSchema
 
     class IdSchema(GenericModel, Generic[T], Schema):
         id: T
 
     IdSchema.__generic_model__ = IdSchema
```

### Comparing `django_ninja_extra-0.19.0/ninja_extra/searching.py` & `django_ninja_extra-0.19.1/ninja_extra/searching.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/security/__init__.py` & `django_ninja_extra-0.19.1/ninja_extra/security/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/security/api_key.py` & `django_ninja_extra-0.19.1/ninja_extra/security/api_key.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/security/http.py` & `django_ninja_extra-0.19.1/ninja_extra/security/http.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/security/session.py` & `django_ninja_extra-0.19.1/ninja_extra/security/session.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/shortcuts.py` & `django_ninja_extra-0.19.1/ninja_extra/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/status.py` & `django_ninja_extra-0.19.1/ninja_extra/status.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/testing/client.py` & `django_ninja_extra-0.19.1/ninja_extra/testing/client.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/throttling/decorator.py` & `django_ninja_extra-0.19.1/ninja_extra/throttling/decorator.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/throttling/model.py` & `django_ninja_extra-0.19.1/ninja_extra/throttling/model.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/ninja_extra/urls.py` & `django_ninja_extra-0.19.1/ninja_extra/urls.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/pyproject.toml` & `django_ninja_extra-0.19.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/conftest.py` & `django_ninja_extra-0.19.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/controllers.py` & `django_ninja_extra-0.19.1/tests/controllers.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_api_instance.py` & `django_ninja_extra-0.19.1/tests/test_api_instance.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_async_auth.py` & `django_ninja_extra-0.19.1/tests/test_async_auth.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_controller.py` & `django_ninja_extra-0.19.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_controller_registry.py` & `django_ninja_extra-0.19.1/tests/test_controller_registry.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_controller_response.py` & `django_ninja_extra-0.19.1/tests/test_controller_response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_dependency_resolver.py` & `django_ninja_extra-0.19.1/tests/test_dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_django_model.py` & `django_ninja_extra-0.19.1/tests/test_django_model.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_django_ninja_router.py` & `django_ninja_extra-0.19.1/tests/test_django_ninja_router.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_event_controller.py` & `django_ninja_extra-0.19.1/tests/test_event_controller.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_exceptions.py` & `django_ninja_extra-0.19.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_generic_patch.py` & `django_ninja_extra-0.19.1/tests/test_generic_patch.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_operation.py` & `django_ninja_extra-0.19.1/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_ordering.py` & `django_ninja_extra-0.19.1/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_pagination.py` & `django_ninja_extra-0.19.1/tests/test_pagination.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import inspect
+import typing
+from abc import abstractmethod
+from typing import Sequence, overload
 
 import django
 import pytest
 from ninja import Schema
 
 from ninja_extra import NinjaExtraAPI, api_controller, route
 from ninja_extra.controllers import RouteFunction
@@ -10,19 +13,35 @@
     AsyncPaginatorOperation,
     PageNumberPagination,
     PageNumberPaginationExtra,
     PaginationBase,
     PaginatorOperation,
     paginate,
 )
+from ninja_extra.schemas import NinjaPaginationResponseSchema
 from ninja_extra.testing import TestAsyncClient, TestClient
 
 ITEMS = list(range(100))
 
 
+class FakeQuerySet(typing.Sequence):
+    def __init__(self, items=None):
+        self.items = items or ITEMS
+
+    def __getitem__(self, index: int) -> typing.Any:
+        return FakeQuerySet(self.items[index])
+
+    def __len__(self) -> int:
+        return len(self.items)
+
+    def __iter__(self):
+        for item in self.items:
+            yield item
+
+
 class CustomPagination(PaginationBase):
     # only offset param, defaults to 5 per page
     class Input(Schema):
         skip: int
 
     def paginate_queryset(self, items, request, **params):
         skip = params["pagination"].skip
@@ -32,19 +51,19 @@
 @api_controller
 class SomeAPIController:
     @route.get("/items_1")
     @paginate  # WITHOUT brackets (should use default pagination)
     def items_1(self):
         return ITEMS
 
-    @route.get("/items_2")
+    @route.get("/items_2", response=NinjaPaginationResponseSchema[int])
     @paginate()  # with brackets (should use default pagination)
     def items_2(self, someparam: int = 0):
         # also having custom param `someparam` - that should not be lost
-        return ITEMS
+        return FakeQuerySet()
 
     @route.get("/items_3")
     @paginate(CustomPagination, pass_parameter="pass_kwargs")
     def items_3(self, **kwargs):
         return ITEMS
 
     @route.get("/items_4", response=PageNumberPaginationExtra.get_response_schema(int))
```

### Comparing `django_ninja_extra-0.19.0/tests/test_permissions.py` & `django_ninja_extra-0.19.1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_route.py` & `django_ninja_extra-0.19.1/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_searching.py` & `django_ninja_extra-0.19.1/tests/test_searching.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_settings.py` & `django_ninja_extra-0.19.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_shortcuts.py` & `django_ninja_extra-0.19.1/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_status.py` & `django_ninja_extra-0.19.1/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_testclient.py` & `django_ninja_extra-0.19.1/tests/test_testclient.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_throthling/test_decorator.py` & `django_ninja_extra-0.19.1/tests/test_throthling/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_throthling/test_models.py` & `django_ninja_extra-0.19.1/tests/test_throthling/test_models.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_controller.py` & `django_ninja_extra-0.19.1/tests/test_throthling/test_throttle_controller.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_decorator_on_controllers.py` & `django_ninja_extra-0.19.1/tests/test_throthling/test_throttle_decorator_on_controllers.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/test_throthling/test_throttling_xxf.py` & `django_ninja_extra-0.19.1/tests/test_throthling/test_throttling_xxf.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/tests/utils.py` & `django_ninja_extra-0.19.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.19.0/PKG-INFO` & `django_ninja_extra-0.19.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ninja-extra
-Version: 0.19.0
+Version: 0.19.1
 Summary: Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)
 Home-page: https://github.com/eadwinCode/django-ninja-extra
 Author: Ezeudoh Tochukwu
 Author-email: tochukwu.ezeudoh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

