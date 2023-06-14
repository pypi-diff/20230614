# Comparing `tmp/pulumiverse_mssql-0.0.6.tar.gz` & `tmp/pulumiverse_mssql-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_mssql-0.0.6.tar", last modified: Wed Jun  7 15:26:23 2023, max compression
+gzip compressed data, was "pulumiverse_mssql-0.0.7.tar", last modified: Wed Jun 14 10:08:54 2023, max compression
```

## Comparing `pulumiverse_mssql-0.0.6.tar` & `pulumiverse_mssql-0.0.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:26:23.255383 pulumiverse_mssql-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-07 15:26:23.255383 pulumiverse_mssql-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:26:23.255383 pulumiverse_mssql-0.0.6/pulumiverse_mssql/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/azuread_service_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/azuread_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:26:23.255383 pulumiverse_mssql-0.0.6/pulumiverse_mssql/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/database_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/database_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/database_role_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_azuread_service_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_azuread_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_schema_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_server_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_server_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_server_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/schema_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/server_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/server_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/server_role_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    32023 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/sql_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql/sql_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:26:23.255383 pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-07 15:26:23.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-07 15:26:23.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:26:23.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:26:23.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 15:26:23.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 15:26:23.000000 pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:26:23.255383 pulumiverse_mssql-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-07 15:26:22.000000 pulumiverse_mssql-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:54.119635 pulumiverse_mssql-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-14 10:08:54.119635 pulumiverse_mssql-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:54.115635 pulumiverse_mssql-0.0.7/pulumiverse_mssql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/azuread_service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/azuread_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:54.119635 pulumiverse_mssql-0.0.7/pulumiverse_mssql/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/database_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/database_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/database_role_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_azuread_service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_azuread_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_schema_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_server_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_server_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_server_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_logins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/schema_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/server_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/server_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/server_role_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32023 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/sql_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql/sql_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:08:54.119635 pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-14 10:08:54.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-14 10:08:54.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:08:54.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:08:54.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 10:08:54.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 10:08:54.000000 pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:08:54.119635 pulumiverse_mssql-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-14 10:08:53.000000 pulumiverse_mssql-0.0.7/setup.py
```

### Comparing `pulumiverse_mssql-0.0.6/PKG-INFO` & `pulumiverse_mssql-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_mssql
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Pulumi Provider for Microsoft SQL Server and Azure SQL
 Home-page: https://github.com/pulumiverse/pulumi-mssql
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-mssql
 Keywords: pulumi mssql category/database
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_mssql-0.0.6/README.md` & `pulumiverse_mssql-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/__init__.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/_inputs.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/_utilities.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/azuread_service_principal.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/azuread_service_principal.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/azuread_user.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/azuread_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/config/outputs.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/config/vars.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/database.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/database_permission.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/database_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/database_role.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/database_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/database_role_member.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/database_role_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_azuread_service_principal.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_azuread_service_principal.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_azuread_user.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_azuread_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database_permissions.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database_role.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_database_roles.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_database_roles.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_databases.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_query.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_query.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_schema.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_schema.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_schema_permissions.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_schema_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_schemas.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_server_permissions.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_server_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_server_role.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_server_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_server_roles.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_server_roles.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_login.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_login.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_logins.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_logins.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_user.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/get_sql_users.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/get_sql_users.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/outputs.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/provider.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/schema.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/schema.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/schema_permission.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/schema_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/script.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/script.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/server_permission.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/server_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/server_role.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/server_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/server_role_member.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/server_role_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/sql_login.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/sql_login.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql/sql_user.py` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql/sql_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/PKG-INFO` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-mssql
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Pulumi Provider for Microsoft SQL Server and Azure SQL
 Home-page: https://github.com/pulumiverse/pulumi-mssql
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-mssql
 Keywords: pulumi mssql category/database
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_mssql-0.0.6/pulumiverse_mssql.egg-info/SOURCES.txt` & `pulumiverse_mssql-0.0.7/pulumiverse_mssql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_mssql-0.0.6/setup.py` & `pulumiverse_mssql-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.6"
-PLUGIN_VERSION = "0.0.6"
+VERSION = "0.0.7"
+PLUGIN_VERSION = "0.0.7"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'mssql', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-mssql'])
         except OSError as error:
```

