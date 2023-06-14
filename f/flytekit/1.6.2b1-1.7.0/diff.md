# Comparing `tmp/flytekit-1.6.2b1.tar.gz` & `tmp/flytekit-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.2b1.tar", last modified: Thu Jun  8 23:49:31 2023, max compression
+gzip compressed data, was "flytekit-1.7.0.tar", last modified: Wed Jun 14 04:33:19 2023, max compression
```

## Comparing `flytekit-1.6.2b1.tar` & `flytekit-1.7.0.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.811171 flytekit-1.6.2b1/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-08 23:49:29.000000 flytekit-1.6.2b1/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.811171 flytekit-1.6.2b1/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23142 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.815171 flytekit-1.6.2b1/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.827171 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.827171 flytekit-1.6.2b1/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.835171 flytekit-1.6.2b1/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31002 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.835171 flytekit-1.6.2b1/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/backend/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/backend/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.847171 flytekit-1.6.2b1/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.847171 flytekit-1.6.2b1/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.847171 flytekit-1.6.2b1/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.811171 flytekit-1.6.2b1/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-08 23:49:29.000000 flytekit-1.6.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.741187 flytekit-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-14 04:33:05.000000 flytekit-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-14 04:33:05.000000 flytekit-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-14 04:33:19.741187 flytekit-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-14 04:33:05.000000 flytekit-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-14 04:33:17.000000 flytekit-1.7.0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23182 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.713186 flytekit-1.7.0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.713186 flytekit-1.7.0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36185 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.717187 flytekit-1.7.0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31002 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/backend/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/backend/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.733187 flytekit-1.7.0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.733187 flytekit-1.7.0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.741187 flytekit-1.7.0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.741187 flytekit-1.7.0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-14 04:33:05.000000 flytekit-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-14 04:33:19.741187 flytekit-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-14 04:33:17.000000 flytekit-1.7.0/setup.py
```

### Comparing `flytekit-1.6.2b1/LICENSE` & `flytekit-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/MANIFEST.in` & `flytekit-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/PKG-INFO` & `flytekit-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.7.0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.2b1/README.md` & `flytekit-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/__init__.py` & `flytekit-1.7.0/flytekit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.2b1"
+__version__ = "1.7.0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.2b1/flytekit/bin/entrypoint.py` & `flytekit-1.7.0/flytekit/bin/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,16 +154,19 @@
         logger.error(exc_str)
         logger.error("!! End Error Captured by Flyte !!")
 
     for k, v in output_file_dict.items():
         utils.write_proto_to_file(v.to_flyte_idl(), os.path.join(ctx.execution_state.engine_dir, k))
 
     ctx.file_access.put_data(ctx.execution_state.engine_dir, output_prefix, is_multipart=True)
-    _output_deck(task_def.name.split(".")[-1], ctx.user_space_params)
     logger.info(f"Engine folder written successfully to the output prefix {output_prefix}")
+
+    if not task_def.disable_deck:
+        _output_deck(task_def.name.split(".")[-1], ctx.user_space_params)
+
     logger.debug("Finished _dispatch_execute")
 
     if os.environ.get("FLYTE_FAIL_ON_ERROR", "").lower() == "true" and _constants.ERROR_FILE_NAME in output_file_dict:
         # This env is set by the flytepropeller
         # AWS batch job get the status from the exit code, so once we catch the error,
         # we should return the error code here
         exit(1)
```

### Comparing `flytekit-1.6.2b1/flytekit/clients/auth/auth_client.py` & `flytekit-1.7.0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clients/auth/authenticator.py` & `flytekit-1.7.0/flytekit/clients/auth/authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     token_endpoint: str
     authorization_endpoint: str
     redirect_uri: str
     client_id: str
     device_authorization_endpoint: typing.Optional[str] = None
     scopes: typing.List[str] = None
     header_key: str = "authorization"
+    audience: typing.Optional[str] = None
 
 
 class ClientConfigStore(object):
     """
     Client Config store retrieve client config. this can be done in multiple ways
     """
 
@@ -170,43 +171,52 @@
         client_id: str,
         client_secret: str,
         cfg_store: ClientConfigStore,
         header_key: typing.Optional[str] = None,
         scopes: typing.Optional[typing.List[str]] = None,
         http_proxy_url: typing.Optional[str] = None,
         verify: typing.Optional[typing.Union[bool, str]] = None,
+        audience: typing.Optional[str] = None,
     ):
         if not client_id or not client_secret:
             raise ValueError("Client ID and Client SECRET both are required.")
         cfg = cfg_store.get_client_config()
         self._token_endpoint = cfg.token_endpoint
         # Use scopes from `flytekit.configuration.PlatformConfig` if passed
         self._scopes = scopes or cfg.scopes
         self._client_id = client_id
         self._client_secret = client_secret
+        self._audience = audience or cfg.audience
         super().__init__(endpoint, cfg.header_key or header_key, http_proxy_url=http_proxy_url, verify=verify)
 
     def refresh_credentials(self):
         """
         This function is used by the _handle_rpc_error() decorator, depending on the AUTH_MODE config object. This handler
         is meant for SDK use-cases of auth (like pyflyte, or when users call SDK functions that require access to Admin,
         like when waiting for another workflow to complete from within a task). This function uses basic auth, which means
         the credentials for basic auth must be present from wherever this code is running.
 
         """
         token_endpoint = self._token_endpoint
         scopes = self._scopes
+        audience = self._audience
 
         # Note that unlike the Pkce flow, the client ID does not come from Admin.
         logging.debug(f"Basic authorization flow with client id {self._client_id} scope {scopes}")
         authorization_header = token_client.get_basic_authorization_header(self._client_id, self._client_secret)
 
         token, expires_in = token_client.get_token(
-            token_endpoint, scopes, authorization_header, http_proxy_url=self._http_proxy_url, verify=self._verify
+            token_endpoint=token_endpoint,
+            authorization_header=authorization_header,
+            http_proxy_url=self._http_proxy_url,
+            verify=self._verify,
+            scopes=scopes,
+            audience=audience,
         )
+
         logging.info("Retrieved new token, expires in {}".format(expires_in))
         self._creds = Credentials(token)
 
 
 class DeviceCodeAuthenticator(Authenticator):
     """
     This Authenticator implements the Device Code authorization flow useful for headless user authentication.
```

### Comparing `flytekit-1.6.2b1/flytekit/clients/auth/keyring.py` & `flytekit-1.7.0/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clients/auth/token_client.py` & `flytekit-1.7.0/flytekit/clients/auth/token_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 def get_token(
     token_endpoint: str,
     scopes: typing.Optional[typing.List[str]] = None,
     authorization_header: typing.Optional[str] = None,
     client_id: typing.Optional[str] = None,
     device_code: typing.Optional[str] = None,
+    audience: typing.Optional[str] = None,
     grant_type: GrantType = GrantType.CLIENT_CREDS,
     http_proxy_url: typing.Optional[str] = None,
     verify: typing.Optional[typing.Union[bool, str]] = None,
 ) -> typing.Tuple[str, int]:
     """
     :rtype: (Text,Int) The first element is the access token retrieved from the IDP, the second is the expiration
             in seconds
@@ -94,17 +95,20 @@
     }
     if client_id:
         body["client_id"] = client_id
     if device_code:
         body["device_code"] = device_code
     if scopes is not None:
         body["scope"] = ",".join(scopes)
+    if audience:
+        body["audience"] = audience
 
     proxies = {"https": http_proxy_url, "http": http_proxy_url} if http_proxy_url else None
     response = requests.post(token_endpoint, data=body, headers=headers, proxies=proxies, verify=verify)
+
     if not response.ok:
         j = response.json()
         if "error" in j:
             err = j["error"]
             if err == error_auth_pending or err == error_slow_down:
                 raise AuthenticationPending(f"Token not yet available, try again in some time {err}")
         logging.error("Status Code ({}) received from IDP: {}".format(response.status_code, response.text))
```

### Comparing `flytekit-1.6.2b1/flytekit/clients/auth_helper.py` & `flytekit-1.7.0/flytekit/clients/auth_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             token_endpoint=oauth2_metadata.token_endpoint,
             authorization_endpoint=oauth2_metadata.authorization_endpoint,
             redirect_uri=public_client_config.redirect_uri,
             client_id=public_client_config.client_id,
             scopes=public_client_config.scopes,
             header_key=public_client_config.authorization_metadata_key or None,
             device_authorization_endpoint=oauth2_metadata.device_authorization_endpoint,
+            audience=public_client_config.audience,
         )
 
 
 def get_authenticator(cfg: PlatformConfig, cfg_store: ClientConfigStore) -> Authenticator:
     """
     Returns a new authenticator based on the platform config.
     """
@@ -69,14 +70,15 @@
     elif cfg_auth == AuthType.BASIC or cfg_auth == AuthType.CLIENT_CREDENTIALS or cfg_auth == AuthType.CLIENTSECRET:
         return ClientCredentialsAuthenticator(
             endpoint=cfg.endpoint,
             client_id=cfg.client_id,
             client_secret=cfg.client_credentials_secret,
             cfg_store=cfg_store,
             scopes=cfg.scopes,
+            audience=cfg.audience,
             http_proxy_url=cfg.http_proxy_url,
             verify=verify,
         )
     elif cfg_auth == AuthType.EXTERNAL_PROCESS or cfg_auth == AuthType.EXTERNALCOMMAND:
         client_cfg = None
         if cfg_store:
             client_cfg = cfg_store.get_client_config()
```

### Comparing `flytekit-1.6.2b1/flytekit/clients/friendly.py` & `flytekit-1.7.0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.7.0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.7.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clients/helpers.py` & `flytekit-1.7.0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clients/raw.py` & `flytekit-1.7.0/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/flyte_cli/main.py` & `flytekit-1.7.0/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/helpers.py` & `flytekit-1.7.0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._filename = pathlib.Path(filename).resolve()
 
     def list_commands(self, ctx):
-        entities = get_entities_in_file(self._filename.__str__())
+        entities = get_entities_in_file(self._filename.__str__(), False)
         return entities.all()
 
     def get_command(self, ctx, exe_entity):
         """
         This command uses the filename with which this command was created, and the string name of the entity passed
           after the Python filename on the command line, to load the Python object, and then return the Command that
           click should run.
```

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 CTX_PACKAGES = "pkgs"
 CTX_NOTIFICATIONS = "notifications"
 CTX_CONFIG_FILE = "config_file"
 CTX_PROJECT_ROOT = "project_root"
 CTX_MODULE = "module"
 CTX_VERBOSE = "verbose"
 CTX_COPY_ALL = "copy_all"
+CTX_FILE_NAME = "file_name"
 
 
 project_option = _click.option(
     "-p",
     "--project",
     required=True,
     type=str,
```

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing_extensions import get_args
 
 from flytekit import BlobType, Literal, Scalar
 from flytekit.clis.sdk_in_container.constants import (
     CTX_CONFIG_FILE,
     CTX_COPY_ALL,
     CTX_DOMAIN,
+    CTX_FILE_NAME,
     CTX_MODULE,
     CTX_PROJECT,
     CTX_PROJECT_ROOT,
 )
 from flytekit.clis.sdk_in_container.helpers import (
     FLYTE_REMOTE_INSTANCE_KEY,
     get_and_save_remote_with_click_context,
@@ -622,15 +623,15 @@
     def all(self) -> typing.List[str]:
         e = []
         e.extend(self.workflows)
         e.extend(self.tasks)
         return e
 
 
-def get_entities_in_file(filename: str) -> Entities:
+def get_entities_in_file(filename: pathlib.Path, should_delete: bool) -> Entities:
     """
     Returns a list of flyte workflow names and list of Flyte tasks in a file.
     """
     flyte_ctx = context_manager.FlyteContextManager.current_context().new_builder()
     module_name = os.path.splitext(os.path.relpath(filename))[0].replace(os.path.sep, ".")
     with context_manager.FlyteContextManager.with_context(flyte_ctx):
         with module_loader.add_sys_path(os.getcwd()):
@@ -642,14 +643,16 @@
     for name in dir(module):
         o = module.__dict__[name]
         if isinstance(o, WorkflowBase):
             workflows.append(name)
         elif isinstance(o, PythonTask):
             tasks.append(name)
 
+    if should_delete and os.path.exists(filename):
+        os.remove(filename)
     return Entities(workflows, tasks)
 
 
 def run_command(ctx: click.Context, entity: typing.Union[PythonFunctionWorkflow, PythonTask]):
     """
     Returns a function that is used to implement WorkflowCommand and execute a flyte workflow.
     """
@@ -662,14 +665,16 @@
         inputs = {}
         for input_name, _ in entity.python_interface.inputs.items():
             inputs[input_name] = kwargs.get(input_name)
 
         if not ctx.obj[REMOTE_FLAG_KEY]:
             output = entity(**inputs)
             click.echo(output)
+            if ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME):
+                os.remove(ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME))
             return
 
         remote = ctx.obj[FLYTE_REMOTE_INSTANCE_KEY]
         config_file = ctx.obj.get(CTX_CONFIG_FILE)
 
         image_config = run_level_params.get("image_config")
         image_config = patch_image_config(config_file, image_config)
@@ -707,28 +712,40 @@
 
         console_url = remote.generate_console_url(execution)
         click.secho(f"Go to {console_url} to see execution in the console.")
 
         if run_level_params.get("dump_snippet"):
             dump_flyte_remote_snippet(execution, project, domain)
 
+        if ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME):
+            os.remove(ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME))
+
     return _run
 
 
 class WorkflowCommand(click.RichGroup):
     """
     click multicommand at the python file layer, subcommands should be all the workflows in the file.
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._filename = pathlib.Path(filename).resolve()
+
+        ctx = context_manager.FlyteContextManager.current_context()
+        if ctx.file_access.is_remote(filename):
+            local_path = os.path.join(os.path.curdir, filename.rsplit("/", 1)[1])
+            ctx.file_access.download(filename, local_path)
+            self._filename = pathlib.Path(local_path).resolve()
+            self._should_delete = True
+        else:
+            self._filename = pathlib.Path(filename).resolve()
+            self._should_delete = False
 
     def list_commands(self, ctx):
-        entities = get_entities_in_file(self._filename)
+        entities = get_entities_in_file(self._filename, self._should_delete)
         return entities.all()
 
     def get_command(self, ctx, exe_entity):
         """
         This command uses the filename with which this command was created, and the string name of the entity passed
           after the Python filename on the command line, to load the Python object, and then return the Command that
           click should run.
@@ -750,15 +767,16 @@
         # N.B.: by construction project_root will necessarily be an ancestor of the filename passed in as
         # a parameter.
         rel_path = self._filename.relative_to(project_root)
         module = os.path.splitext(rel_path)[0].replace(os.path.sep, ".")
 
         ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_PROJECT_ROOT] = project_root
         ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_MODULE] = module
-
+        if self._should_delete:
+            ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_FILE_NAME] = self._filename
         entity = load_naive_entity(module, exe_entity, project_root)
 
         # If this is a remote execution, which we should know at this point, then create the remote object
         p = ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_PROJECT)
         d = ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_DOMAIN)
         r = get_and_save_remote_with_click_context(ctx, p, d)
         get_upload_url_fn = functools.partial(r.client.get_upload_signed_url, project=p, domain=d)
```

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.7.0/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/configuration/__init__.py` & `flytekit-1.7.0/flytekit/configuration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,15 @@
             "client_credentials_secret",
             client_credentials_secret,
         )
         kwargs = set_if_exists(kwargs, "scopes", _internal.Credentials.SCOPES.read(config_file))
         kwargs = set_if_exists(kwargs, "auth_mode", _internal.Credentials.AUTH_MODE.read(config_file))
         kwargs = set_if_exists(kwargs, "endpoint", _internal.Platform.URL.read(config_file))
         kwargs = set_if_exists(kwargs, "console_endpoint", _internal.Platform.CONSOLE_ENDPOINT.read(config_file))
+
         kwargs = set_if_exists(kwargs, "http_proxy_url", _internal.Platform.HTTP_PROXY_URL.read(config_file))
         return PlatformConfig(**kwargs)
 
     @classmethod
     def for_endpoint(cls, endpoint: str, insecure: bool = False) -> PlatformConfig:
         return PlatformConfig(endpoint=endpoint, insecure=insecure)
```

### Comparing `flytekit-1.6.2b1/flytekit/configuration/default_images.py` & `flytekit-1.7.0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/configuration/feature_flags.py` & `flytekit-1.7.0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/configuration/file.py` & `flytekit-1.7.0/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/configuration/internal.py` & `flytekit-1.7.0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/annotation.py` & `flytekit-1.7.0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/base_sql_task.py` & `flytekit-1.7.0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/base_task.py` & `flytekit-1.7.0/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/checkpointer.py` & `flytekit-1.7.0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/class_based_resolver.py` & `flytekit-1.7.0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/condition.py` & `flytekit-1.7.0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/constants.py` & `flytekit-1.7.0/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/container_task.py` & `flytekit-1.7.0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/context_manager.py` & `flytekit-1.7.0/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/data_persistence.py` & `flytekit-1.7.0/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/docstring.py` & `flytekit-1.7.0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.7.0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/gate.py` & `flytekit-1.7.0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/interface.py` & `flytekit-1.7.0/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/launch_plan.py` & `flytekit-1.7.0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/local_cache.py` & `flytekit-1.7.0/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/map_task.py` & `flytekit-1.7.0/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/mock_stats.py` & `flytekit-1.7.0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/node.py` & `flytekit-1.7.0/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/node_creation.py` & `flytekit-1.7.0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/notification.py` & `flytekit-1.7.0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/pod_template.py` & `flytekit-1.7.0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/promise.py` & `flytekit-1.7.0/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/python_auto_container.py` & `flytekit-1.7.0/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/python_customized_container_task.py` & `flytekit-1.7.0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/python_function_task.py` & `flytekit-1.7.0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/reference.py` & `flytekit-1.7.0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/reference_entity.py` & `flytekit-1.7.0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/resources.py` & `flytekit-1.7.0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/schedule.py` & `flytekit-1.7.0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/shim_task.py` & `flytekit-1.7.0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/task.py` & `flytekit-1.7.0/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/testing.py` & `flytekit-1.7.0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/tracker.py` & `flytekit-1.7.0/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/type_engine.py` & `flytekit-1.7.0/flytekit/core/type_engine.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/type_helpers.py` & `flytekit-1.7.0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/utils.py` & `flytekit-1.7.0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/core/workflow.py` & `flytekit-1.7.0/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/deck/deck.py` & `flytekit-1.7.0/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/deck/html/template.html` & `flytekit-1.7.0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/deck/renderer.py` & `flytekit-1.7.0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/exceptions/scopes.py` & `flytekit-1.7.0/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/exceptions/system.py` & `flytekit-1.7.0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/exceptions/user.py` & `flytekit-1.7.0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extend/__init__.py` & `flytekit-1.7.0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extend/backend/agent_service.py` & `flytekit-1.7.0/flytekit/extend/backend/agent_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extend/backend/base_agent.py` & `flytekit-1.7.0/flytekit/extend/backend/base_agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+import time
 import typing
 from abc import ABC, abstractmethod
+from collections import OrderedDict
 
 import grpc
 from flyteidl.admin.agent_pb2 import (
+    PERMANENT_FAILURE,
     RETRYABLE_FAILURE,
     RUNNING,
     SUCCEEDED,
     CreateTaskResponse,
     DeleteTaskResponse,
     GetTaskResponse,
     State,
 )
 from flyteidl.core.tasks_pb2 import TaskTemplate
+from rich.progress import Progress
 
-from flytekit import logger
+from flytekit import FlyteContext, logger
+from flytekit.configuration import ImageConfig, SerializationSettings
+from flytekit.core.base_task import PythonTask
+from flytekit.core.type_engine import TypeEngine
 from flytekit.models.literals import LiteralMap
 
 
 class AgentBase(ABC):
     """
     This is the base class for all agents. It defines the interface that all agents must implement.
     The agent service will be run either locally or in a pod, and will be responsible for
@@ -101,7 +108,56 @@
     if state in ["failed"]:
         return RETRYABLE_FAILURE
     elif state in ["done", "succeeded"]:
         return SUCCEEDED
     elif state in ["running"]:
         return RUNNING
     raise ValueError(f"Unrecognized state: {state}")
+
+
+def is_terminal_state(state: State) -> bool:
+    """
+    Return true if the state is terminal.
+    """
+    return state in [SUCCEEDED, RETRYABLE_FAILURE, PERMANENT_FAILURE]
+
+
+class AsyncAgentExecutorMixin:
+    """
+    This mixin class is used to run the agent task locally, and it's only used for local execution.
+    Task should inherit from this class if the task can be run in the agent.
+    """
+
+    def execute(self, **kwargs) -> typing.Any:
+        from unittest.mock import MagicMock
+
+        from flytekit.tools.translator import get_serializable
+
+        entity = typing.cast(PythonTask, self)
+        m: OrderedDict = OrderedDict()
+        dummy_context = MagicMock(spec=grpc.ServicerContext)
+        cp_entity = get_serializable(m, settings=SerializationSettings(ImageConfig()), entity=entity)
+        agent = AgentRegistry.get_agent(dummy_context, cp_entity.template.type)
+
+        if agent is None:
+            raise Exception("Cannot run the task locally, please mock.")
+        literals = {}
+        ctx = FlyteContext.current_context()
+        for k, v in kwargs.items():
+            literals[k] = TypeEngine.to_literal(ctx, v, type(v), entity.interface.inputs[k].type)
+        inputs = LiteralMap(literals) if literals else None
+        output_prefix = ctx.file_access.get_random_local_directory()
+        cp_entity = get_serializable(m, settings=SerializationSettings(ImageConfig()), entity=entity)
+        res = agent.create(dummy_context, output_prefix, cp_entity.template, inputs)
+        state = RUNNING
+        metadata = res.resource_meta
+        progress = Progress(transient=True)
+        task = progress.add_task(f"[cyan]Running Task {entity.name}...", total=None)
+        with progress:
+            while not is_terminal_state(state):
+                progress.start_task(task)
+                time.sleep(1)
+                res = agent.get(dummy_context, metadata)
+                state = res.resource.state
+                logger.info(f"Task state: {state}")
+
+        return LiteralMap.from_flyte_idl(res.resource.outputs)
```

### Comparing `flytekit-1.6.2b1/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.7.0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/pytorch/__init__.py` & `flytekit-1.7.0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.7.0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/pytorch/native.py` & `flytekit-1.7.0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/sklearn/__init__.py` & `flytekit-1.7.0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/sklearn/native.py` & `flytekit-1.7.0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/sqlite3/task.py` & `flytekit-1.7.0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/tasks/shell.py` & `flytekit-1.7.0/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.7.0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/tensorflow/model.py` & `flytekit-1.7.0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/extras/tensorflow/record.py` & `flytekit-1.7.0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/image_spec/image_spec.py` & `flytekit-1.7.0/flytekit/image_spec/image_spec.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/interaction/parse_stdin.py` & `flytekit-1.7.0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.7.0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/interfaces/random.py` & `flytekit-1.7.0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/interfaces/stats/client.py` & `flytekit-1.7.0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/interfaces/stats/taggable.py` & `flytekit-1.7.0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/lazy_import/lazy_module.py` & `flytekit-1.7.0/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/loggers.py` & `flytekit-1.7.0/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/admin/common.py` & `flytekit-1.7.0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/admin/task_execution.py` & `flytekit-1.7.0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/admin/workflow.py` & `flytekit-1.7.0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/annotation.py` & `flytekit-1.7.0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/array_job.py` & `flytekit-1.7.0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/common.py` & `flytekit-1.7.0/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/catalog.py` & `flytekit-1.7.0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/compiler.py` & `flytekit-1.7.0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/condition.py` & `flytekit-1.7.0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/errors.py` & `flytekit-1.7.0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/execution.py` & `flytekit-1.7.0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/identifier.py` & `flytekit-1.7.0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/types.py` & `flytekit-1.7.0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/core/workflow.py` & `flytekit-1.7.0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/documentation.py` & `flytekit-1.7.0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/dynamic_job.py` & `flytekit-1.7.0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/execution.py` & `flytekit-1.7.0/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/filters.py` & `flytekit-1.7.0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/interface.py` & `flytekit-1.7.0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/launch_plan.py` & `flytekit-1.7.0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/literals.py` & `flytekit-1.7.0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/matchable_resource.py` & `flytekit-1.7.0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/named_entity.py` & `flytekit-1.7.0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/node_execution.py` & `flytekit-1.7.0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/presto.py` & `flytekit-1.7.0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/project.py` & `flytekit-1.7.0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/qubole.py` & `flytekit-1.7.0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/schedule.py` & `flytekit-1.7.0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/security.py` & `flytekit-1.7.0/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/task.py` & `flytekit-1.7.0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/types.py` & `flytekit-1.7.0/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/models/workflow_closure.py` & `flytekit-1.7.0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/remote/__init__.py` & `flytekit-1.7.0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/remote/backfill.py` & `flytekit-1.7.0/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/remote/entities.py` & `flytekit-1.7.0/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/remote/executions.py` & `flytekit-1.7.0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/remote/lazy_entity.py` & `flytekit-1.7.0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/remote/remote.py` & `flytekit-1.7.0/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/remote/remote_callable.py` & `flytekit-1.7.0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/testing/__init__.py` & `flytekit-1.7.0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/fast_registration.py` & `flytekit-1.7.0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/ignore.py` & `flytekit-1.7.0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/module_loader.py` & `flytekit-1.7.0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/repo.py` & `flytekit-1.7.0/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/script_mode.py` & `flytekit-1.7.0/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/serialize_helpers.py` & `flytekit-1.7.0/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/subprocess.py` & `flytekit-1.7.0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/tools/translator.py` & `flytekit-1.7.0/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/directory/__init__.py` & `flytekit-1.7.0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/directory/types.py` & `flytekit-1.7.0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/file/__init__.py` & `flytekit-1.7.0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/file/file.py` & `flytekit-1.7.0/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/numpy/ndarray.py` & `flytekit-1.7.0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/pickle/pickle.py` & `flytekit-1.7.0/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/schema/types.py` & `flytekit-1.7.0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/schema/types_pandas.py` & `flytekit-1.7.0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/structured/__init__.py` & `flytekit-1.7.0/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/structured/basic_dfs.py` & `flytekit-1.7.0/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/structured/bigquery.py` & `flytekit-1.7.0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit/types/structured/structured_dataset.py` & `flytekit-1.7.0/flytekit/types/structured/structured_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         except KeyError:
             ...
 
         if protocol_specific_handler or fsspec_handler or single_handler:
             return protocol_specific_handler or fsspec_handler or single_handler
         else:
-            raise ValueError(f"Failed to find a handler for {df_type}, protocol {protocol}, fmt |{format}|")
+            raise ValueError(f"Failed to find a handler for {df_type}, protocol [{protocol}], fmt ['{format}']")
 
     @classmethod
     def get_encoder(cls, df_type: Type, protocol: str, format: str):
         return cls._finder(StructuredDatasetTransformerEngine.ENCODERS, df_type, protocol, format)
 
     @classmethod
     def get_decoder(cls, df_type: Type, protocol: str, format: str):
```

### Comparing `flytekit-1.6.2b1/flytekit.egg-info/PKG-INFO` & `flytekit-1.7.0/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.7.0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.2b1/flytekit.egg-info/SOURCES.txt` & `flytekit-1.7.0/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit.egg-info/requires.txt` & `flytekit-1.7.0/flytekit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.7.0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b1/setup.py` & `flytekit-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.2b1"
+__version__ = "1.7.0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
```

