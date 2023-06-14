# Comparing `tmp/dcrx-api-0.4.0.tar.gz` & `tmp/dcrx-api-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.4.0.tar", last modified: Mon Jun 12 20:42:14 2023, max compression
+gzip compressed data, was "dcrx-api-0.4.1.tar", last modified: Wed Jun 14 00:54:40 2023, max compression
```

## Comparing `dcrx-api-0.4.0.tar` & `dcrx-api-0.4.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.779478 dcrx-api-0.4.0/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/connection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/models/database_transaction_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/image_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_step_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/remote_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/server_limit_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/cpu/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/registry/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/registry/table/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.018278 dcrx-api-0.4.1/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/database/connection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/database/models/database_transaction_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/env/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/job_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/job_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/models/server_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/registry/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/models/registry_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/models/registry_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/registry/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:54:40.022278 dcrx-api-0.4.1/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-14 00:54:39.000000 dcrx-api-0.4.1/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-14 00:54:40.000000 dcrx-api-0.4.1/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:54:39.000000 dcrx-api-0.4.1/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 00:54:39.000000 dcrx-api-0.4.1/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 00:54:39.000000 dcrx-api-0.4.1/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 00:54:39.000000 dcrx-api-0.4.1/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:54:40.026278 dcrx-api-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-14 00:54:36.000000 dcrx-api-0.4.1/setup.py
```

### Comparing `dcrx-api-0.4.0/LICENSE` & `dcrx-api-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/PKG-INFO` & `dcrx-api-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.4.0/README.md` & `dcrx-api-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/cli/base.py` & `dcrx-api-0.4.1/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/cli/database.py` & `dcrx-api-0.4.1/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/cli/server.py` & `dcrx-api-0.4.1/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/context/manager.py` & `dcrx-api-0.4.1/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/database/connection.py` & `dcrx-api-0.4.1/dcrx_api/database/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                     last_error = str(transaction_exception)
                     await connection.rollback()
 
                 await connection.commit()
         
         return DatabaseTransactionResult(
             message='Database transaction failed',
-            last_error=last_error
+            error=last_error
         )
     
     async def insert_or_update(
         self,
         statements: List[
             Union[Insert, Update]
         ]
@@ -195,15 +195,15 @@
                     last_error = str(transaction_exception)
                     await connection.rollback()
                 
                 await connection.commit()
         
         return DatabaseTransactionResult(
             message='Database transaction failed',
-            last_error=last_error
+            error=last_error
         )
 
 
     async def delete(
         self,
         statements: List[Delete]
     ) -> DatabaseTransactionResult[T]:
@@ -226,15 +226,15 @@
                     last_error = str(transaction_exception)
                     await connection.rollback()
             
                 await connection.commit()
         
         return DatabaseTransactionResult(
             message='Database transaction failed',
-            last_error=last_error
+            error=last_error
         )
 
     async def drop_table(
         self,
         table: Table
     ) -> DatabaseTransactionResult[T]:
         
@@ -261,15 +261,15 @@
                     last_error = str(transaction_exception)
                     await connection.rollback()
 
                 await connection.commit()
         
         return DatabaseTransactionResult(
             message='Database transaction failed',
-            last_error=last_error
+            error=last_error
         )
     
     async def close(self):
 
         last_error: Union[str, None]=None
         for _ in range(self.config.database_transaction_retries):
 
@@ -283,9 +283,9 @@
                 )
 
             except Exception as transaction_exception:
                 last_error = str(transaction_exception)
 
         return DatabaseTransactionResult(
             message='Database transaction failed',
-            last_error=last_error
+            error=last_error
         )
```

### Comparing `dcrx-api-0.4.0/dcrx_api/env/env.py` & `dcrx-api-0.4.1/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/env/load_env.py` & `dcrx-api-0.4.1/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/env/time_parser.py` & `dcrx-api-0.4.1/dcrx_api/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/lifespan.py` & `dcrx-api-0.4.1/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.4.1/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/auth/manager.py` & `dcrx-api-0.4.1/dcrx_api/services/auth/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
 import base64
 import datetime
 import functools
-from cryptography.fernet import Fernet
 from concurrent.futures import ThreadPoolExecutor
+from cryptography.fernet import Fernet
 from dcrx_api.env import Env
 from jose import JWTError, jwt
 from fastapi.security import OAuth2PasswordBearer
 from fastapi.security.utils import get_authorization_scheme_param
 from passlib.context import CryptContext
 from typing import (
     Optional,
     Dict,
     Any,
-    List,
     Union
 )
 from dcrx_api.env.time_parser import TimeParser
 from dcrx_api.services.users.connection import UsersConnection
 from dcrx_api.services.users.models import (
     DBUser,
     LoginUser
```

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/context.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/job.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/job.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/queue.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/service.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.4.1/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/monitoring/base/monitor.py` & `dcrx-api-0.4.1/dcrx_api/services/monitoring/base/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/monitoring/context.py` & `dcrx-api-0.4.1/dcrx_api/services/monitoring/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/monitor.py` & `dcrx-api-0.4.1/dcrx_api/services/monitoring/memory/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/registry/connection.py` & `dcrx-api-0.4.1/dcrx_api/services/registry/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/registry/context.py` & `dcrx-api-0.4.1/dcrx_api/services/registry/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/registry/service.py` & `dcrx-api-0.4.1/dcrx_api/services/registry/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_mysql_table.py` & `dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_postgres_table.py` & `dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_sqlite_table.py` & `dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_table.py` & `dcrx-api-0.4.1/dcrx_api/services/registry/table/registry_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/users/connection.py` & `dcrx-api-0.4.1/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/users/context.py` & `dcrx-api-0.4.1/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/users/service.py` & `dcrx-api-0.4.1/dcrx_api/services/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.4.1/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.4.1/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.4.1/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.4.1/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.4.1/dcrx_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.4.0/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.4.1/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.4.0/setup.py` & `dcrx-api-0.4.1/setup.py`

 * *Files identical despite different names*

