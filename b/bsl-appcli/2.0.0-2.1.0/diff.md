# Comparing `tmp/bsl-appcli-2.0.0.tar.gz` & `tmp/bsl-appcli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl-appcli-2.0.0.tar", last modified: Thu May 18 03:23:35 2023, max compression
+gzip compressed data, was "bsl-appcli-2.1.0.tar", last modified: Tue Jun 13 23:46:58 2023, max compression
```

## Comparing `bsl-appcli-2.0.0.tar` & `bsl-appcli-2.1.0.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/backup_manager/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/backup_manager/remote_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/cli_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/appcli_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/backup_manager_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/configure_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/configure_template_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/debug_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/encrypt_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/init_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/install_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/launcher_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/migrate_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/service_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/task_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/version_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/common/data_class_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/configuration/configuration_dir_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/crypto/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/git_repositories/git_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/keycloak_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/models/cli_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    28248 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/orchestrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/templates/installer.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/templates/launcher.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/bsl_appcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/backup_manager/test_backup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/cipher/test_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands/test_install_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands_task/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands_task/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands_task/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands_task/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands_task/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands_task/test_commands_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration/test_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/expected_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_manager/expected_generated/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_manager/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_state/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_state/test_configuration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/crypto/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/git_repositories/test_git_repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/string_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/string_transformer/test_string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/variables_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/variables_manager/test_variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/version/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/version/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    36362 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36003 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/backup_manager/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/backup_manager/remote_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16721 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/cli_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/appcli_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/backup_manager_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/configure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/configure_template_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/debug_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/encrypt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/init_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/install_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/launcher_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/migrate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/service_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/task_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/version_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/common/data_class_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/configuration/configuration_dir_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/git_repositories/git_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/keycloak_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/models/cli_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28248 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/orchestrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/templates/installer.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/templates/launcher.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/bsl_appcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36362 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    36566 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/backup_manager/test_backup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/cipher/test_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/commands/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands/test_install_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/commands_task/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands_task/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands_task/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands_task/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/commands_task/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands_task/test_commands_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration/test_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/expected_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_manager/expected_generated/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_manager/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_state/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_state/test_configuration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/crypto/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/git_repositories/test_git_repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/string_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/string_transformer/test_string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/variables_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/variables_manager/test_variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/version/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/version/test_version.py
```

### Comparing `bsl-appcli-2.0.0/LICENSE` & `bsl-appcli-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/PKG-INFO` & `bsl-appcli-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 2.0.0
+Version: 2.1.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # BSL Application CLI Library
 
+[![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
 ## Overview
 
 This library can be leveraged to add a standardised CLI capability to applications to:
```

### Comparing `bsl-appcli-2.0.0/README.md` & `bsl-appcli-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # BSL Application CLI Library
 
+[![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
 ## Overview
 
 This library can be leveraged to add a standardised CLI capability to applications to:
```

### Comparing `bsl-appcli-2.0.0/appcli/backup_manager/backup_manager.py` & `bsl-appcli-2.1.0/appcli/backup_manager/backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/backup_manager/remote_strategy.py` & `bsl-appcli-2.1.0/appcli/backup_manager/remote_strategy.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/cli_builder.py` & `bsl-appcli-2.1.0/appcli/cli_builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,34 +7,37 @@
 
 Created by brightSPARK Labs
 www.brightsparklabs.com
 """
 
 # standard libraries
 import os
+import pwd
 import sys
 from pathlib import Path
 from typing import Dict, Iterable
 
 # vendor libraries
 import click
+import pyfiglet
 from tabulate import tabulate
 
 # local libraries
 from appcli.commands.backup_manager_cli import BackupManagerCli
 from appcli.commands.configure_cli import ConfigureCli
 from appcli.commands.debug_cli import DebugCli
 from appcli.commands.encrypt_cli import EncryptCli
 from appcli.commands.init_cli import InitCli
 from appcli.commands.install_cli import InstallCli
 from appcli.commands.launcher_cli import LauncherCli
 from appcli.commands.migrate_cli import MigrateCli
 from appcli.commands.service_cli import ServiceCli
 from appcli.commands.task_cli import TaskCli
 from appcli.commands.version_cli import VersionCli
+from appcli.dev_mode import wrap_dev_mode
 from appcli.functions import error_and_exit, extract_valid_environment_variable_names
 from appcli.logger import enable_debug_logging, logger
 from appcli.models.cli_context import CliContext
 from appcli.models.configuration import Configuration
 
 # ------------------------------------------------------------------------------
 # CONSTANTS
@@ -52,15 +55,50 @@
     """Build the CLI to be run
 
     Args:
         configuration (Configuration): the application's configuration settings
     """
     APP_NAME = configuration.app_name
     APP_NAME_SLUG = configuration.app_name_slug
+    APP_NAME_SLUG_UPPER = APP_NAME_SLUG.upper()
     APP_VERSION = os.environ.get("APP_VERSION", "latest")
+    IS_DEV_MODE: bool = f"{APP_NAME_SLUG_UPPER}_DEV_MODE" in os.environ
+
+    # Details of the user who ran the CLI app.
+    CLI_USER = os.environ.get(
+        f"{APP_NAME_SLUG_UPPER}_CLI_USER", pwd.getpwuid(os.getuid()).pw_name
+    )
+    CLI_UID = os.environ.get(f"{APP_NAME_SLUG_UPPER}_CLI_UID", str(os.getuid()))
+    CLI_GID = os.environ.get(f"{APP_NAME_SLUG_UPPER}_CLI_GID", str(os.getgid()))
+
+    # Mandatory environment variables this script will set.
+    ENV_VAR_CONFIG_DIR = f"{APP_NAME_SLUG_UPPER}_CONFIG_DIR"
+    ENV_VAR_GENERATED_CONFIG_DIR = f"{APP_NAME_SLUG_UPPER}_GENERATED_CONFIG_DIR"
+    ENV_VAR_DATA_DIR = f"{APP_NAME_SLUG_UPPER}_DATA_DIR"
+    ENV_VAR_BACKUP_DIR = f"{APP_NAME_SLUG_UPPER}_BACKUP_DIR"
+    ENV_VAR_ENVIRONMENT = f"{APP_NAME_SLUG_UPPER}_ENVIRONMENT"
+
+    if IS_DEV_MODE:
+        with wrap_dev_mode():
+            environment = "local-dev"
+            install_dir = Path("/tmp/") / APP_NAME_SLUG.lower() / environment
+            install_dir.mkdir(parents=True, exist_ok=True)
+
+            overrides = {
+                f"{APP_NAME_SLUG_UPPER}_CLI_DEBUG": True,
+                f"{APP_NAME_SLUG_UPPER}_CLI_CONFIGURATION_DIR": install_dir / "conf",
+                f"{APP_NAME_SLUG_UPPER}_CLI_DATA_DIR": install_dir / "data",
+                f"{APP_NAME_SLUG_UPPER}_CLI_BACKUP_DIR": install_dir / "backup",
+                f"{APP_NAME_SLUG_UPPER}_CLI_ENVIRONMENT": environment,
+            }
+
+            logger.info("Overriding CLI options via environment variables")
+            for key, value in overrides.items():
+                logger.info(f"  {key}={value}")
+                os.environ[key] = str(value)
 
     # --------------------------------------------------------------------------
     # CREATE_CLI: LOGIC
     # --------------------------------------------------------------------------
 
     default_commands = {}
     for cli_class in (
@@ -150,79 +188,71 @@
         data_dir,
         environment,
         docker_credentials_file,
         additional_data_dir,
         additional_env_var,
         backup_dir,
     ):
+        title = pyfiglet.figlet_format(APP_NAME, font="slant")
+        logger.info(f"\n{title}")
+
         if debug:
             logger.info("Enabling debug logging")
             enable_debug_logging()
 
-        ctx.obj = CliContext(
+        cli_context: CliContext = CliContext(
             configuration_dir=configuration_dir,
             data_dir=data_dir,
             application_context_files_dir=configuration.application_context_files_dir,
             additional_data_dirs=additional_data_dir,
             additional_env_variables=additional_env_var,
             environment=environment,
             docker_credentials_file=docker_credentials_file,
             subcommand_args=ctx.obj,
             debug=debug,
+            is_dev_mode=IS_DEV_MODE,
             app_name_slug=APP_NAME_SLUG,
             app_version=APP_VERSION,
             commands=default_commands,
             backup_dir=backup_dir,
         )
+        ctx.obj = cli_context
 
         if ctx.invoked_subcommand is None:
             click.echo(ctx.get_help())
             sys.exit(1)
 
-        # attempt to set desired environment
-        initialised_environment = {}
-        for k, v in desired_environment.items():
-            if v is None:
-                logger.warning("Environment variable [%s] has not been set", k)
-            else:
-                logger.debug("Exporting environment variable [%s]", k)
-                os.environ[k] = v
-                initialised_environment[k] = v
-        if len(initialised_environment) != len(desired_environment):
-            error_and_exit(
-                "Could not set desired environment. Please ensure specified environment variables are set."
-            )
-
         # For the `installer`/`launcher` commands, no further output/checks required.
         if ctx.invoked_subcommand in ("launcher", "install"):
             # Don't execute this function any further, continue to run subcommand with the current CLI context
             return
 
-        check_docker_socket()
-        check_environment()
+        __set_environment(cli_context, desired_environment)
+
+        __check_docker_socket()
+        __check_environment()
 
         # Table of configuration variables to print
         table = [
-            ["Configuration directory", f"{ctx.obj.configuration_dir}"],
+            ["Application", f"{APP_NAME} (slug: {APP_NAME_SLUG})"],
+            ["Version", APP_VERSION],
+            ["Environment", f"{cli_context.environment}"],
+            ["Configuration directory", f"{cli_context.configuration_dir}"],
             [
                 "Generated Configuration directory",
-                f"{ctx.obj.get_generated_configuration_dir()}",
+                f"{cli_context.get_generated_configuration_dir()}",
             ],
-            ["Data directory", f"{ctx.obj.data_dir}"],
-            ["Backup directory", f"{ctx.obj.backup_dir}"],
-            ["Environment", f"{ctx.obj.environment}"],
+            ["Data directory", f"{cli_context.data_dir}"],
+            ["Backup directory", f"{cli_context.backup_dir}"],
+            ["Current user", f"{CLI_USER} (uid: {CLI_UID} / gid: {CLI_GID})"],
         ]
 
         # Print out the configuration values as an aligned table
-        logger.info(
-            "%s (version: %s) CLI running with:\n\n%s\n",
-            APP_NAME,
-            APP_VERSION,
-            tabulate(table, colalign=("right",)),
-        )
+        details = tabulate(table, colalign=("right",))
+        logger.info(f"Current context:\n{details}\n")
         if additional_data_dir:
             logger.info(
                 "Additional data directories:\n\n%s\n",
                 tabulate(
                     additional_data_dir,
                     headers=["Environment Variable", "Path"],
                     colalign=("right",),
@@ -234,36 +264,76 @@
                 tabulate(
                     additional_env_var,
                     headers=["Environment Variable", "Value"],
                     colalign=("right",),
                 ),
             )
 
+        if IS_DEV_MODE:
+            with wrap_dev_mode():
+                # Auto configure init/apply if not specified.
+                if ctx.invoked_subcommand not in ("configure",):
+                    configure_cli = cli_context.commands["configure"]
+                    try:
+                        ctx.invoke(configure_cli.commands["init"])
+                    except SystemExit:
+                        # At completion, the invoked command tries to exit the script, so we have to catch
+                        # the SystemExit.
+                        pass
+
+                    try:
+                        ctx.invoke(configure_cli.commands["apply"], force=True)
+                    except SystemExit:
+                        # At completion, the invoked command tries to exit the script, so we have to catch
+                        # the SystemExit.
+                        pass
+
     def run():
         """Run the entry-point click CLI command"""
         cli(  # pylint: disable=no-value-for-parameter,unexpected-keyword-arg
-            prog_name=configuration.app_name_slug
+            prog_name=configuration.app_name_slug,
+            auto_envvar_prefix=f"{APP_NAME_SLUG_UPPER}_CLI",
         )
 
-    def check_docker_socket():
+    def __check_docker_socket():
         """Check that the docker socket exists, and exit if it does not"""
         if not os.path.exists("/var/run/docker.sock"):
             error_msg = """Docker socket not present. Please launch with a mounted /var/run/docker.sock"""
             error_and_exit(error_msg)
 
-    def check_environment():
-        """Confirm that mandatory environment variables and additional data directories are defined."""
+    def __set_environment(
+        cli_context: CliContext, desired_environment: Dict[str, str] = {}
+    ):
+        mandatory_environment = {
+            ENV_VAR_CONFIG_DIR: cli_context.configuration_dir,
+            ENV_VAR_GENERATED_CONFIG_DIR: cli_context.get_generated_configuration_dir(),
+            ENV_VAR_DATA_DIR: cli_context.data_dir,
+            ENV_VAR_BACKUP_DIR: cli_context.backup_dir,
+            ENV_VAR_ENVIRONMENT: cli_context.environment,
+        }
 
-        app_name_slug_upper = APP_NAME_SLUG.upper()
+        final_environment = mandatory_environment | desired_environment
+
+        # Attempt to set desired environment.
+        initialised_environment = {}
+        for k, v in final_environment.items():
+            if v is None:
+                logger.warning(f"Environment variable `{k}` has not been set")
+            else:
+                logger.debug(f"Exporting environment variable: {k}={v}")
+                os.environ[k] = str(v)
+                initialised_environment[k] = str(v)
+        if len(initialised_environment) != len(final_environment):
+            error_and_exit(
+                "Could not set desired environment. Please ensure specified environment variables are set."
+            )
+
+    def __check_environment():
+        """Confirm that mandatory environment variables and additional data directories are defined."""
 
-        ENV_VAR_CONFIG_DIR = f"{app_name_slug_upper}_CONFIG_DIR"
-        ENV_VAR_GENERATED_CONFIG_DIR = f"{app_name_slug_upper}_GENERATED_CONFIG_DIR"
-        ENV_VAR_DATA_DIR = f"{app_name_slug_upper}_DATA_DIR"
-        ENV_VAR_BACKUP_DIR = f"{app_name_slug_upper}_BACKUP_DIR"
-        ENV_VAR_ENVIRONMENT = f"{app_name_slug_upper}_ENVIRONMENT"
         launcher_set_mandatory_env_vars = [
             ENV_VAR_CONFIG_DIR,
             ENV_VAR_GENERATED_CONFIG_DIR,
             ENV_VAR_DATA_DIR,
             ENV_VAR_BACKUP_DIR,
             ENV_VAR_ENVIRONMENT,
         ]
@@ -313,15 +383,15 @@
         for env_variable in env_variables:
             value = os.environ.get(env_variable)
             if value is None:
                 logger.error(error_message_template, env_variable, env_variable)
                 result = False
             else:
                 logger.debug(
-                    f"Confirmed environment variable is set - '{env_variable}' = '{value}'"
+                    f"Confirmed environment variable is set: {env_variable}={value}"
                 )
         if not result:
             logger.error(exit_message)
 
         return result
 
     for command in default_commands.values():
@@ -353,12 +423,17 @@
         )
         super(NotRequiredOn, self).__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         subcommand = args[0] if len(args) > 0 else ""
         if subcommand in self.not_required_on:
             self.prompt = None
-        elif self.name not in opts:
+            return super(NotRequiredOn, self).handle_parse_result(ctx, opts, args)
+
+        # Delegate to super to try and populate value from opts/env vars, etc.
+        result = super(NotRequiredOn, self).handle_parse_result(ctx, opts, args)
+        # First item in the tuple is the parsed value for the option. Fail if missing.
+        if result[0] is None:
             options = " / ".join([f"'{x}'" for x in self.opts])
             raise click.UsageError(f"Error: Missing option {options}.")
 
-        return super(NotRequiredOn, self).handle_parse_result(ctx, opts, args)
+        return result
```

### Comparing `bsl-appcli-2.0.0/appcli/commands/appcli_command.py` & `bsl-appcli-2.1.0/appcli/commands/appcli_command.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/backup_manager_cli.py` & `bsl-appcli-2.1.0/appcli/commands/backup_manager_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/configure_cli.py` & `bsl-appcli-2.1.0/appcli/commands/configure_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/configure_template_cli.py` & `bsl-appcli-2.1.0/appcli/commands/configure_template_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/debug_cli.py` & `bsl-appcli-2.1.0/appcli/commands/debug_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ________________________________________________________________________________
 
 Created by brightSPARK Labs
 www.brightsparklabs.com
 """
 
 # standard library
+import os
 from pprint import pprint
 
 # vendor libraries
 import click
 
 # local libraries
 from appcli.commands.appcli_command import AppcliCommand
@@ -68,9 +69,16 @@
             print("=== ORCHESTRATOR CONFIGURATION ===")
             pprint(vars(self.cli_configuration.orchestrator))
 
             print()
             print("=== VARIABLES ===")
             pprint(variables_manager.get_all_variables())
 
+        @debug.command(
+            help="Drops into a shell within the launcher for advanced debugging.",
+        )
+        @click.pass_context
+        def shell(ctx):
+            os.system("bash")
+
         # Expose the commands
         self.commands = {"debug": debug}
```

### Comparing `bsl-appcli-2.0.0/appcli/commands/encrypt_cli.py` & `bsl-appcli-2.1.0/appcli/commands/encrypt_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/init_cli.py` & `bsl-appcli-2.1.0/appcli/commands/init_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/install_cli.py` & `bsl-appcli-2.1.0/appcli/commands/install_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/launcher_cli.py` & `bsl-appcli-2.1.0/appcli/commands/launcher_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/migrate_cli.py` & `bsl-appcli-2.1.0/appcli/commands/migrate_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/service_cli.py` & `bsl-appcli-2.1.0/appcli/commands/service_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/task_cli.py` & `bsl-appcli-2.1.0/appcli/commands/task_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/commands/version_cli.py` & `bsl-appcli-2.1.0/appcli/commands/version_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/common/data_class_extensions.py` & `bsl-appcli-2.1.0/appcli/common/data_class_extensions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/configuration/configuration_dir_state.py` & `bsl-appcli-2.1.0/appcli/configuration/configuration_dir_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/configuration_manager.py` & `bsl-appcli-2.1.0/appcli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/crypto/cipher.py` & `bsl-appcli-2.1.0/appcli/crypto/cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/crypto/crypto.py` & `bsl-appcli-2.1.0/appcli/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/functions.py` & `bsl-appcli-2.1.0/appcli/functions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/git_repositories/git_repositories.py` & `bsl-appcli-2.1.0/appcli/git_repositories/git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/keycloak_manager.py` & `bsl-appcli-2.1.0/appcli/keycloak_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/logger.py` & `bsl-appcli-2.1.0/appcli/logger.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/models/cli_context.py` & `bsl-appcli-2.1.0/appcli/models/cli_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,18 @@
     docker_credentials_file: Path
     """ Path to the Docker credentials file (config.json) on the host for private docker registries. """
 
     subcommand_args: tuple
     """ Arguments passed to CLI subcommand. """
 
     debug: bool
-    """ Whether to print debug logs. """
+    """ True to enable debug level logging. """
+
+    is_dev_mode: bool
+    """ True if the application is running in DEV MODE. """
 
     # ---------------------------------
     # CLI build data
     # ---------------------------------
 
     app_name_slug: str
     """ The application's name """
```

### Comparing `bsl-appcli-2.0.0/appcli/models/configuration.py` & `bsl-appcli-2.1.0/appcli/models/configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/orchestrators.py` & `bsl-appcli-2.1.0/appcli/orchestrators.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/string_transformer.py` & `bsl-appcli-2.1.0/appcli/string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/appcli/templates/installer.j2` & `bsl-appcli-2.1.0/appcli/templates/installer.j2`

 * *Files 5% similar despite different names*

```diff
@@ -31,36 +31,43 @@
     mkdir -p "{{ install_dir }}" || print_error_and_exit "Could not create [{{ install_dir }}]"
     [[ -w "{{ install_dir }}" ]] || print_error_and_exit "No permissions to write to [{{ install_dir }}]"
 
     cd "{{ install_dir }}"
 
     # Create versioned launcher
     local _launcher_versioned=".$(date -Isec --utc)_{{ app_name_slug_lower }}_{{ cli_context.app_version }}"
-    generate_launcher > "${_launcher_versioned}" || print_error_and_exit "No permissions to write to [${_launcher_versioned}]"
+    generate_launcher > "${_launcher_versioned}" || print_error_and_exit "Could not generate launcher at $(pwd)/[${_launcher_versioned}]"
     chmod a+x "${_launcher_versioned}"
 
     local _launcher_generic="{{ app_name_slug_lower }}"
 
-    # If the generic launcher already exists, upgrade the existing application
-    [[ -e "${_launcher_generic}" ]] && upgrade_existing_application "${_launcher_generic}" "${_launcher_versioned}"
+    # If the generic launcher already exists, upgrade the existing application.
+    local _install_type=install
+    if [[ -e "${_launcher_generic}" ]]; then
+        _install_type=upgrade
+        upgrade_existing_application "${_launcher_generic}" "${_launcher_versioned}"
+    fi
 
     # Update the symlink to the generic launcher
     rm -f "${_launcher_generic}" || print_error_and_exit "No permissions to delete to [${_launcher_generic}]"
     ln -s "${_launcher_versioned}" "${_launcher_generic}"
 
     # Auto configure if enabled.
     if [[ $AUTO_CONFIGURE = true ]]; then
-        NO_TTY=true {{ install_dir }}/${_launcher_generic} configure init
+        # Only need to init if an install (i.e. not an upgrade)
+        [[ "${_install_type}" == "install" ]] && NO_TTY=true {{ install_dir }}/${_launcher_generic} configure init
+
         NO_TTY=true {{ install_dir }}/${_launcher_generic} configure apply
     fi
 
     >&2 cat <<EOF
     $(date -Isec --utc) INFO: {{ app_name_slug_lower }} version [{{ cli_context.app_version }}] can be launched via:
 
         {{ install_dir }}/{{ app_name_slug_lower }}
+
 EOF
 }
 
 ##
  # Processes the arguments passed in on the command line.
  #
  # @param $@ Arguments passed in on the command line.
@@ -117,15 +124,15 @@
  # @param $1 The path of the new launcher script.
  ##
 function upgrade_existing_application()
 {
     local _launcher_existing="$(realpath ${1})"
     local _launcher_upgrade="$(realpath ${2})"
 
-    >&2 echo "Installing an upgrade on existing application..."
+    >&2 echo "$(date -Isec --utc) INFO: Installing an upgrade on existing application..."
 
     # Stop services and apply with the old launcher
     NO_TTY=true ${_launcher_existing} service stop
     NO_TTY=true ${_launcher_existing} configure apply --force
 
     # Migrate and apply with the new launcher
     NO_TTY=true ${_launcher_upgrade} migrate
```

### Comparing `bsl-appcli-2.0.0/appcli/templates/launcher.j2` & `bsl-appcli-2.1.0/appcli/templates/launcher.j2`

 * *Files 25% similar despite different names*

```diff
@@ -18,16 +18,34 @@
 # Variables are defaulted so that they can be overridden at runtime if desired
 MOUNTED_CONFIG_DIR="{{ '${' }}{{ app_name_slug_upper }}_CONFIG_DIR:-{{ cli_context.configuration_dir }}{{ '}' }}"
 MOUNTED_GENERATED_CONFIG_DIR="{{ '${' }}{{ app_name_slug_upper }}_GENERATED_CONFIG_DIR:-{{ cli_context.get_generated_configuration_dir() }}{{ '}' }}"
 MOUNTED_DATA_DIR="{{ '${' }}{{ app_name_slug_upper }}_DATA_DIR:-{{ cli_context.data_dir }}{{ '}' }}"
 MOUNTED_BACKUP_DIR="{{ '${' }}{{ app_name_slug_upper }}_BACKUP_DIR:-{{ cli_context.backup_dir }}{{ '}' }}"
 ENVIRONMENT="{{ '${' }}{{ app_name_slug_upper }}_ENVIRONMENT:-{{ cli_context.environment }}{{ '}' }}"
 
+if [[ -e /var/run/docker.sock ]]; then
+    DOCKER_SOCKET=/var/run/docker.sock
+elif [[ -e /run/podman/podman.sock ]]; then
+    DOCKER_SOCKET=/run/podman/podman.sock
+else
+    echo "ERROR: No docker socket found on host"
+    exit 1
+fi
+
+CLI_USER=${USER:-unknown}
+[[ -n "${SUDO_USER:-}" ]] && CLI_USER=${SUDO_USER}
+
+CLI_UID=$(id -u)
+[[ -n "${SUDO_UID:-}" ]] && CLI_UID=${SUDO_UID}
+
+CLI_GID=$(id -g)
+[[ -n "${SUDO_GID:-}" ]] && CLI_GID=${SUDO_GID}
+
 # ------------------------------------------------------------------------------
-# LOGIC
+# FUNCTIONS
 # ------------------------------------------------------------------------------
 
 function main()
 {
 
     docker run \
         --name {{ app_name_slug }}_{{ cli_context.environment }}_launcher_$(date +%s) \
@@ -40,25 +58,29 @@
 {% for name, value in cli_context.additional_env_variables %}
         --env {{ name }}="{{ value }}" \
 {% endfor %}
 {% for name, path in cli_context.additional_data_dirs %}
         --env {{ name }}="{{ path }}" \
         --volume "{{ path }}:{{ path }}" \
 {% endfor %}
-        --volume /var/run/docker.sock:/var/run/docker.sock \
+        --volume "${DOCKER_SOCKET}:/var/run/docker.sock" \
+        --volume "${MOUNTED_DATA_DIR}/cli/home:/root" \
         --env APP_NAME="{{ app_name }}" \
         --env {{ app_name_slug_upper }}_CONFIG_DIR="${MOUNTED_CONFIG_DIR}" \
         --volume "${MOUNTED_CONFIG_DIR}:${MOUNTED_CONFIG_DIR}" \
         --env {{ app_name_slug_upper }}_GENERATED_CONFIG_DIR="${MOUNTED_GENERATED_CONFIG_DIR}" \
         --volume "${MOUNTED_GENERATED_CONFIG_DIR}:${MOUNTED_GENERATED_CONFIG_DIR}" \
         --env {{ app_name_slug_upper }}_DATA_DIR="${MOUNTED_DATA_DIR}" \
         --volume "${MOUNTED_DATA_DIR}:${MOUNTED_DATA_DIR}" \
         --env {{ app_name_slug_upper }}_BACKUP_DIR="${MOUNTED_BACKUP_DIR}" \
         --volume "${MOUNTED_BACKUP_DIR}:${MOUNTED_BACKUP_DIR}" \
         --env {{ app_name_slug_upper }}_ENVIRONMENT="${ENVIRONMENT}" \
+        --env {{ app_name_slug_upper }}_CLI_USER="${CLI_USER}" \
+        --env {{ app_name_slug_upper }}_CLI_UID="${CLI_UID}" \
+        --env {{ app_name_slug_upper }}_CLI_GID="${CLI_GID}" \
         --network host \
         {{ configuration.docker_image }}:{{ app_version }} \
             --configuration-dir "${MOUNTED_CONFIG_DIR}" \
             --data-dir "${MOUNTED_DATA_DIR}" \
             --backup-dir "${MOUNTED_BACKUP_DIR}" \
             --environment "${ENVIRONMENT}" \
 {% for name, path in cli_context.additional_data_dirs %}
```

### Comparing `bsl-appcli-2.0.0/appcli/variables_manager.py` & `bsl-appcli-2.1.0/appcli/variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/bsl_appcli.egg-info/PKG-INFO` & `bsl-appcli-2.1.0/bsl_appcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 2.0.0
+Version: 2.1.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # BSL Application CLI Library
 
+[![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
 ## Overview
 
 This library can be leveraged to add a standardised CLI capability to applications to:
```

### Comparing `bsl-appcli-2.0.0/bsl_appcli.egg-info/SOURCES.txt` & `bsl-appcli-2.1.0/bsl_appcli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 appcli/cli_builder.py
 appcli/configuration_manager.py
+appcli/dev_mode.py
 appcli/functions.py
 appcli/keycloak_manager.py
 appcli/logger.py
 appcli/orchestrators.py
 appcli/string_transformer.py
 appcli/variables_manager.py
 appcli/backup_manager/backup_manager.py
```

### Comparing `bsl-appcli-2.0.0/setup.py` & `bsl-appcli-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,26 +53,27 @@
     license="MIT License",
     author="brightSPARK Labs",
     author_email="enquire@brightsparklabs.com",
     url="https://www.brightsparklabs.com",
     packages=find_namespace_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     install_requires=[
-        "boto3==1.26.123",
+        "boto3==1.26.145",
         "click==8.1.3",
         "coloredlogs==15.0.1",
         "cronex==0.1.3.1",
         "dataclasses-json==0.5.7",
         "deepdiff==6.3.0",
         "GitPython==3.1.31",
         "jinja2==3.1.2",
-        "pre-commit==3.2.2",
-        "pycryptodome==3.17",
-        "pydantic==1.10.7",
+        "pre-commit==3.3.2",
+        "pycryptodome==3.18.0",
+        "pydantic==1.10.8",
+        "pyfiglet==0.8.post1",
         "python-keycloak==0.22.0",
         "python-slugify==8.0.1",
-        "ruamel-yaml==0.17.21",
+        "ruamel-yaml==0.17.31",
         "tabulate==0.9.0",
         "wheel==0.40.0",
     ],
     extras_require={"dev": ["black", "flake8", "isort", "pytest"]},
 )
```

### Comparing `bsl-appcli-2.0.0/tests/backup_manager/test_backup_manager.py` & `bsl-appcli-2.1.0/tests/backup_manager/test_backup_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
             app_name_slug="test_app",
             additional_data_dirs=None,
             additional_env_variables=None,
             environment="test",
             docker_credentials_file=None,
             subcommand_args=None,
             debug=True,
+            is_dev_mode=False,
             app_version="1.0",
             commands=commands,
         ),
         command=click.Command(
             name="backup", context_settings={"allow_extra_args": False}
         ),
     )
```

### Comparing `bsl-appcli-2.0.0/tests/cipher/test_cipher.py` & `bsl-appcli-2.1.0/tests/cipher/test_cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/commands/test_commands.py` & `bsl-appcli-2.1.0/tests/commands/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,15 @@
             additional_data_dirs=None,
             backup_dir=backup_dir,
             additional_env_variables=None,
             environment="test",
             docker_credentials_file=None,
             subcommand_args=None,
             debug=True,
+            is_dev_mode=False,
             app_name_slug=APP_NAME,
             app_version="0.0.0",
             commands=ConfigureCli(config).commands,
         )
 
     def _create_config(self) -> Configuration:
         return Configuration(
```

### Comparing `bsl-appcli-2.0.0/tests/commands/test_install_script.py` & `bsl-appcli-2.1.0/tests/commands/test_install_script.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/commands_task/test_commands_task.py` & `bsl-appcli-2.1.0/tests/commands_task/test_commands_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
             additional_data_dirs=None,
             backup_dir=backup_dir,
             additional_env_variables=None,
             environment="test",
             docker_credentials_file=None,
             subcommand_args=None,
             debug=True,
+            is_dev_mode=False,
             app_name_slug=APP_NAME_SLUG,
             app_version="0.0.0",
             commands=ConfigureCli(config).commands,
         )
 
     def _create_config(self) -> Configuration:
         return Configuration(
```

### Comparing `bsl-appcli-2.0.0/tests/configuration/test_configuration.py` & `bsl-appcli-2.1.0/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/configuration_manager/test_configuration_manager.py` & `bsl-appcli-2.1.0/tests/configuration_manager/test_configuration_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,15 @@
         additional_data_dirs=None,
         backup_dir=backup_dir,
         additional_env_variables=None,
         environment="test",
         docker_credentials_file=None,
         subcommand_args=None,
         debug=True,
+        is_dev_mode=False,
         app_name_slug=APP_NAME_SLUG,
         app_version=app_version,
         commands={},
     )
 
 
 def create_conf_manager(tmpdir, cli_context: CliContext = None) -> ConfigurationManager:
```

### Comparing `bsl-appcli-2.0.0/tests/configuration_state/test_configuration_state.py` & `bsl-appcli-2.1.0/tests/configuration_state/test_configuration_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/crypto/test_crypto.py` & `bsl-appcli-2.1.0/tests/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/git_repositories/test_git_repositories.py` & `bsl-appcli-2.1.0/tests/git_repositories/test_git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/string_transformer/test_string_transformer.py` & `bsl-appcli-2.1.0/tests/string_transformer/test_string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/variables_manager/test_variables_manager.py` & `bsl-appcli-2.1.0/tests/variables_manager/test_variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.0.0/tests/version/test_version.py` & `bsl-appcli-2.1.0/tests/version/test_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         additional_data_dirs=None,
         backup_dir=None,
         additional_env_variables=None,
         environment="test",
         docker_credentials_file=None,
         subcommand_args=None,
         debug=True,
+        is_dev_mode=False,
         app_name_slug="APP_NAME",
         app_version=f"{version}",
         commands=None,
     )
     runner = CliRunner()
     result = runner.invoke(VersionCli(None).commands["version"], obj=cli_context)
     assert result.exit_code == 0
```

