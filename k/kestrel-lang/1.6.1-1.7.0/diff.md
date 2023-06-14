# Comparing `tmp/kestrel-lang-1.6.1.tar.gz` & `tmp/kestrel-lang-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.6.1.tar", last modified: Wed May 31 15:55:47 2023, max compression
+gzip compressed data, was "kestrel-lang-1.7.0.tar", last modified: Wed Jun 14 19:55:14 2023, max compression
```

## Comparing `kestrel-lang-1.6.1.tar` & `kestrel-lang-1.7.0.tar`

### file list

```diff
@@ -1,100 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 15:55:47.604294 kestrel-lang-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.588294 kestrel-lang-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    20339 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_fast_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.063361 kestrel-lang-1.7.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.059361 kestrel-lang-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.063361 kestrel-lang-1.7.0/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.063361 kestrel-lang-1.7.0/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.075361 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.075361 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/transmitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.075361 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_stixshifter_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.6.1/AUTHORS.rst` & `kestrel-lang-1.7.0/AUTHORS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 - `Charlie Wu`_
 - `Jill Casavant`_
 - `Sulakshan Vajipayajula`_
 - `Chew Kin Zhong`_
 - `Ian Molloy`_
 - `Constantin Adam`_
 - `Ting Dai`_
+- `Leila Rashidi`_
 
 .. _Xiaokui Shu: https://github.com/subbyte
 .. _Paul Coccoli: https://github.com/pcoccoli
 .. _Charlie Wu: https://github.com/charliewutw
 .. _Jill Casavant: https://github.com/jmcasava
 .. _Sulakshan Vajipayajula: https://github.com/svajipay
 .. _Chew Kin Zhong: https://github.com/kinzhong
 .. _Ian Molloy: https://github.com/imolloy
 .. _Constantin Adam: https://github.com/cmadam
 .. _Ting Dai: https://github.com/tingdai
+.. _Leila Rashidi: https://github.com/leila-rashidi
```

### Comparing `kestrel-lang-1.6.1/LICENSE.md` & `kestrel-lang-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/PKG-INFO` & `kestrel-lang-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.6.1
+Version: 1.7.0
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.6.1/README.rst` & `kestrel-lang-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/setup.cfg` & `kestrel-lang-1.7.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.6.1
+version = 1.7.0
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -33,15 +33,15 @@
 	requests
 	nest-asyncio>=1.5.6
 	lark>=1.1.5
 	pyarrow>=5.0.0
 	docker>=5.0.0
 	stix-shifter>=5.3.0
 	stix-shifter-utils>=5.3.0
-	firepit>=2.3.20
+	firepit>=2.3.21
 	typeguard
 tests_require = 
 	pytest
 
 [options.packages.find]
 where = src
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/__main__.py` & `kestrel-lang-1.7.0/src/kestrel/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,35 +6,29 @@
 
 import argparse
 import logging
 
 from kestrel.session import Session
 from kestrel.utils import add_logging_handler, clear_logging_handlers
 
-_logger = logging.getLogger(__name__)
-
-
-def logging_setup(if_verbose_mode, if_debug_mode):
-    clear_logging_handlers()
-    if if_verbose_mode:
-        add_logging_handler(logging.StreamHandler(), if_debug_mode)
-
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Kestrel Interpreter")
     parser.add_argument("huntflow", help="huntflow in .hf file")
     parser.add_argument(
         "-v", "--verbose", help="print verbose log", action="store_true"
     )
     parser.add_argument(
         "--debug", help="debug level log (default is info level)", action="store_true"
     )
     args = parser.parse_args()
 
-    logging_setup(args.verbose, args.debug)
+    clear_logging_handlers()
+    if args.verbose:
+        add_logging_handler(logging.StreamHandler(), args.debug)
 
     with Session(debug_mode=args.debug) as session:
         with open(args.huntflow, "r") as fp:
             huntflow = fp.read()
         outputs = session.execute(huntflow)
         results = "\n\n".join([o.to_string() for o in outputs])
         print(results)
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.7.0/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/analytics/interface.py` & `kestrel-lang-1.7.0/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/analytics/manager.py` & `kestrel-lang-1.7.0/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/codegen/commands.py` & `kestrel-lang-1.7.0/src/kestrel/codegen/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,18 +107,22 @@
 ################################################################
 
 
 @_debug_logger
 @_default_output
 def assign(stmt, session):
     entity_table = session.symtable[stmt["input"]].entity_table
-    transform = stmt.get("transform")
+    transform = stmt.get("transformer")
     if transform:
         if transform.lower() == "timestamped":
             qry = session.store.timestamped(entity_table, run=False)
+        elif transform.lower() == "addobsid":
+            qry = session.store.extract_observeddata_attribute(
+                entity_table, name_of_attribute="id", run=False
+            )
         else:
             qry = Query(entity_table)
     else:
         qry = Query(entity_table)
 
     qry = _build_query(session.store, entity_table, qry, stmt, [])
 
@@ -210,18 +214,22 @@
 
     return None, DisplayDict(disp)
 
 
 @_debug_logger
 def disp(stmt, session):
     entity_table = session.symtable[stmt["input"]].entity_table
-    transform = stmt.get("transform")
+    transform = stmt.get("transformer")
     if transform and entity_table:
         if transform.lower() == "timestamped":
             qry = session.store.timestamped(entity_table, run=False)
+        elif transform.lower() == "addobsid":
+            qry = session.store.extract_observeddata_attribute(
+                entity_table, name_of_attribute="id", run=False
+            )
         else:
             qry = Query(entity_table)
     else:
         qry = Query(entity_table)
 
     qry = _build_query(session.store, entity_table, qry, stmt)
     try:
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/codegen/data.py` & `kestrel-lang-1.7.0/src/kestrel/codegen/data.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/codegen/display.py` & `kestrel-lang-1.7.0/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/codegen/queries.py` & `kestrel-lang-1.7.0/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/codegen/relations.py` & `kestrel-lang-1.7.0/src/kestrel/codegen/relations.py`

 * *Files 25% similar despite different names*

```diff
@@ -133,108 +133,26 @@
                 if all_values:
                     id_attr = attr
                     break
 
     return id_attr
 
 
-def are_entities_associated_with_x_ibm_event(entity_types):
-    flags = [entity_type in stix_x_ibm_event_mapping for entity_type in entity_types]
-    return all(flags)
-
-
-def compile_generic_relation_to_pattern(return_type, input_type, input_var_name):
-    comp_exps = []
-    for relation, is_reversed in _enumerate_relations_between_entities(
-        return_type, input_type
-    ):
-        comp_exps += _generate_paramstix_comparison_expressions(
-            return_type, relation, input_type, is_reversed, input_var_name
-        )
-    pattern = "[" + " OR ".join(comp_exps) + "]"
-    _logger.debug(f"generic relation pattern compiled: {pattern}")
-    return pattern
-
-
-def compile_specific_relation_to_pattern(
-    return_type, relation, input_type, is_reversed, input_var_name
-):
-    comp_exps = _generate_paramstix_comparison_expressions(
-        return_type, relation, input_type, is_reversed, input_var_name
-    )
-    pattern = "[" + " OR ".join(comp_exps) + "]"
-    _logger.debug(f"specific relation pattern compiled: {pattern}")
-    return pattern
-
-
 def compile_identical_entity_search_pattern(var_name, var_struct, does_support_id):
     # "id" attribute may not be available for STIX 2.0 via STIX-shifter
     # so `does_support_id` is set to False in default kestrel config file
     attribute = get_entity_id_attribute(var_struct)
     if attribute == "id" and not does_support_id:
         pattern_raw = None
     else:
         pattern_raw = f"[{var_struct.type}:{attribute} = {var_name}.{attribute}]"
     _logger.debug(f"identical entity search raw pattern generated: {pattern_raw}")
     return pattern_raw
 
 
-def compile_x_ibm_event_search_flow_in_pattern(input_type, input_var_name):
-    ref = stix_x_ibm_event_mapping[input_type]
-    pattern = f"[x-oca-event:{ref}.id = {input_var_name}.id]"
-    _logger.debug(f"x-oca-event flow in pattern compiled: {pattern}")
-    return pattern
-
-
-def compile_x_ibm_event_search_flow_out_pattern(return_type, input_event_var_name):
-    ref = stix_x_ibm_event_mapping[return_type]
-    pattern = f"[{return_type}:id = {input_event_var_name}.{ref}.id]"
-    _logger.debug(f"x-oca-event flow out pattern compiled: {pattern}")
-    return pattern
-
-
-def _enumerate_relations_between_entities(return_type, input_type):
-    # return: [(relation, is_reversed)]
-    relations = []
-    for x, r, y in stix_2_0_ref_mapping.keys():
-        if x == return_type and y == input_type:
-            relations.append((r, False))
-        if y == return_type and x == input_type:
-            relations.append((r, True))
-    _logger.debug(
-        f'enumerated relations between "{return_type}" and "{input_type}": {relations}'
-    )
-    return relations
-
-
-def _generate_paramstix_comparison_expressions(
-    return_type, relation, input_type, is_reversed, input_var_name
-):
-    (entity_x, entity_y) = (
-        (input_type, return_type) if is_reversed else (return_type, input_type)
-    )
-
-    stix_src_refs, stix_tgt_refs = stix_2_0_ref_mapping[(entity_x, relation, entity_y)]
-
-    comp_exps = []
-    for stix_ref in stix_src_refs:
-        if stix_ref.endswith("_refs"):
-            comp_exps.append(f"{return_type}:id = {input_var_name}.{stix_ref}[*].id")
-        else:
-            comp_exps.append(f"{return_type}:id = {input_var_name}.{stix_ref}.id")
-
-    for stix_ref in stix_tgt_refs:
-        if stix_ref.endswith("_refs"):
-            comp_exps.append(f"{return_type}:id = {input_var_name}.{stix_ref}[*].id")
-        else:
-            comp_exps.append(f"{return_type}:id = {input_var_name}.{stix_ref}.id")
-
-    return comp_exps
-
-
 def fine_grained_relational_process_filtering(
     local_var, prefetch_entity_table, store, config
 ):
     # Two-step search for matched processes
     # 1. anchor process search (find anchor process in pfeh_processes against ref_processes)
     # 2. precise process search (find process in pfeh_processes against anchor_processes)
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/codegen/summary.py` & `kestrel-lang-1.7.0/src/kestrel/codegen/summary.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/config.py` & `kestrel-lang-1.7.0/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/config.yaml` & `kestrel-lang-1.7.0/src/kestrel/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
   # retrieve the file from a process and then start prefetch to gain
   # information/connections of the file from all processes. Retrieval of
   # millions records will likely result in a performance issue, thus the user
   # can put `file` in this list to disable prefetch for it.
   excluded_entities:
     -
     # - file
-    # - process
+    # - user-account
+    # - x-oca-asset
 
   # Detailed logic to identify the same process from different records is more
   # complex than many data source query language can express, so Kestrel
   # retrieves potential same process candidate records and perform fine-grained
   # process identification in Kestrel with these parameters.
   process_identification:
     pid_but_name_changed_time_begin_offset: -5 # seconds
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/datasource/interface.py` & `kestrel-lang-1.7.0/src/kestrel/datasource/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/datasource/manager.py` & `kestrel-lang-1.7.0/src/kestrel/datasource/manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 from kestrel.absinterface import InterfaceManager
 from kestrel.datasource import MODULE_PREFIX, AbstractDataSourceInterface
 from kestrel.exceptions import (
     DataSourceInterfaceNotFound,
     InvalidDataSourceInterfaceImplementation,
     ConflictingDataSourceInterfaceScheme,
 )
-import asyncio
-import inspect
-
-# TODO: better solution to avoid using nest_asyncio for run_until_complete()
-#       maybe putting entire Kestrel in async mode
-import nest_asyncio
-
-nest_asyncio.apply()
 
 
 class DataSourceManager(InterfaceManager):
     def __init__(self, config):
         super().__init__(
             config,
             "datasources",
@@ -34,13 +26,10 @@
     def list_data_sources_from_scheme(self, scheme):
         i, c = self._get_interface_with_config(scheme)
         return i.list_data_sources(c)
 
     def query(self, uri, pattern, session_id, store):
         scheme, uri = self._parse_and_complete_uri(uri)
         i, c = self._get_interface_with_config(scheme)
-        if inspect.iscoroutinefunction(i.query):
-            rs = asyncio.run(i.query(uri, pattern, session_id, c, store))
-        else:
-            rs = i.query(uri, pattern, session_id, c, store)
+        rs = i.query(uri, pattern, session_id, c, store)
         self.queried_data_sources.append(uri)
         return rs
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.7.0/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/exceptions.py` & `kestrel-lang-1.7.0/src/kestrel/exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/semantics/completor.py` & `kestrel-lang-1.7.0/src/kestrel/semantics/completor.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 from kestrel.symboltable.symtable import SymbolTable
 from kestrel.datasource.manager import DataSourceManager
 from kestrel.analytics.manager import AnalyticsManager
 from kestrel.syntax.utils import (
     get_entity_types,
     get_keywords,
     all_relations,
-    TRANSFORMS,
 )
 from firepit.timestamp import timefmt
 
 _logger = logging.getLogger(__name__)
 
 ISO_TS_RE = re.compile(r"\d{4}(-\d{2}(-\d{2}(T\d{2}(:\d{2}(:\d{2}Z?)?)?)?)?)?")
 
@@ -131,16 +130,14 @@
                 expected_values.extend(get_entity_types())
             elif token == "RELATION":
                 expected_values.extend(all_relations)
             elif token == "REVERSED":
                 expected_values.append("BY")
             elif token == "EQUAL":
                 expected_values.append("=")
-            elif token == "TRANSFORM":
-                expected_values.extend(TRANSFORMS)
             elif token == "ATTRIBUTE":
                 # TODO: attribute completion
                 # https://github.com/opencybersecurityalliance/kestrel-lang/issues/79
                 _logger.debug(f"TODO: ATTRIBUTE COMPLETION")
             elif token == "ENTITY_ATTRIBUTE_PATH":
                 # TODO: attribute completion
                 # https://github.com/opencybersecurityalliance/kestrel-lang/issues/79
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/semantics/processor.py` & `kestrel-lang-1.7.0/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/semantics/reference.py` & `kestrel-lang-1.7.0/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/session.py` & `kestrel-lang-1.7.0/src/kestrel/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,17 @@
         # remove logging handler
         if self.logging_handler:
             logging.getLogger().removeHandler(self.logging_handler)
             self.logging_handler.close()
             # ensure this does not executed twice
             self.logging_handler = None
 
+        if self.original_logging_level:
+            logging.getLogger().setLevel(self.original_logging_level)
+
         # close store/database
         if self.store:
             # release resources
             self.store.close()
             # ensure this does not executed twice
             self.store = None
 
@@ -512,8 +515,10 @@
 
         master_dir.symlink_to(self.runtime_directory)
 
     def _logging_setup(self):
         log_file_name = self.config["session"]["log_path"]
         log_file_path = os.path.join(self.runtime_directory, log_file_name)
         handler = logging.FileHandler(log_file_path)
-        self.logging_handler = add_logging_handler(handler, self.debug_mode)
+        self.logging_handler, self.original_logging_level = add_logging_handler(
+            handler, self.debug_mode
+        )
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.7.0/src/kestrel/symboltable/variable.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.7.0/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/syntax/kestrel.lark` & `kestrel-lang-1.7.0/src/kestrel/syntax/kestrel.lark`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,24 @@
 // Expression
 //
 
 expression: vtrans where_clause? attr_clause? sort_clause? limit_clause? offset_clause?
 
 // not use rule name `transform` since it is a special function in Lark
 // the function in transformer will mal-function in `merge_transformers()`
-vtrans: TRANSFORM "(" VARIABLE ")"
+vtrans: transformer "(" VARIABLE ")"
       | VARIABLE
 
-TRANSFORM: (TIMESTAMPED)
+transformer: TIMESTAMPED
+           | ADDOBSID
 
 TIMESTAMPED: "TIMESTAMPED"i
 
+ADDOBSID: "ADDOBSID"i
+
 where_clause: "WHERE"i ecg_pattern
 attr_clause: "ATTR"i ATTRIBUTES
 sort_clause: "SORT"i BY ATTRIBUTE (ASC|DESC)?
 limit_clause: "LIMIT"i INT
 offset_clause: "OFFSET"i INT
 
 ?ecg_pattern: disjunction
@@ -111,18 +114,18 @@
          | "last"i INT timeunit                 -> timespan_relative
 
 ?timeunit: DAY
          | HOUR
          | MINUTE
          | SECOND
 
-DAY: "days"i | "d"i
-HOUR: "hours"i | "h"i
-MINUTE: "minutes"i | "m"i
-SECOND: "seconds"i | "s"i
+DAY: "days"i | "day"i | "d"i
+HOUR: "hours"i | "hour"i | "h"i
+MINUTE: "minutes"i | "minute"i | "m"i
+SECOND: "seconds"i | "second"i | "s"i
 
 timestamp:       ISOTIMESTAMP
          | "\""  ISOTIMESTAMP "\""
          | "'"   ISOTIMESTAMP "'"
          | "t\"" ISOTIMESTAMP "\""
          | "t'"  ISOTIMESTAMP "'"
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/syntax/parser.py` & `kestrel-lang-1.7.0/src/kestrel/syntax/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,18 +204,26 @@
     def expression(self, args):
         packet = args[0]
         for arg in args:
             packet.update(arg)
         return packet
 
     def vtrans(self, args):
-        return {
-            "input": self._extract_var(args),
-            "transform": self._assert_and_extract_single("TRANSFORM", args),
-        }
+        if len(args) == 1:
+            return {
+                "input": self._extract_var(args),
+            }
+        else:
+            return {
+                "input": self._extract_var(args),
+                "transformer": args[0],
+            }
+
+    def transformer(self, args):
+        return args[0]
 
     def where_clause(self, args):
         pattern = ExtCenteredGraphPattern(args[0])
         return {
             "where": pattern,
         }
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/syntax/reference.py` & `kestrel-lang-1.7.0/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel/syntax/utils.py` & `kestrel-lang-1.7.0/src/kestrel/syntax/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     all_relations,
     stix_2_0_ref_mapping,
     stix_2_0_identical_mapping,
 )
 
 LITERALS = {"CNAME", "LETTER", "DIGIT", "WS", "INT", "WORD", "ESCAPED_STRING", "NUMBER"}
 AGG_FUNCS = {"MIN", "MAX", "AVG", "SUM", "COUNT", "NUNIQUE"}
-TRANSFORMS = {"TIMESTAMPED"}
 EXPRESSION_OPTIONS = {"WHERE", "ATTR", "SORT", "LIMIT", "OFFSET"}
+TRANSFORMS = {"TIMESTAMPED", "ADDOBSID"}
 
 
 def get_keywords():
     grammar = get_data(__name__, "kestrel.lark").decode("utf-8")
     parser = Lark(grammar, parser="lalr")
     alphabet_patterns = filter(lambda x: x.pattern.value.isalnum(), parser.terminals)
     keywords = [x.pattern.value for x in alphabet_patterns] + all_relations
```

### Comparing `kestrel-lang-1.6.1/src/kestrel/utils.py` & `kestrel-lang-1.7.0/src/kestrel/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,18 +68,19 @@
     fmt = "%(asctime)s %(levelname)s %(name)s %(message)s"
     datefmt = "%H:%M:%S"
     formatter = logging.Formatter(fmt=fmt, datefmt=datefmt)
 
     handler.setFormatter(formatter)
 
     root_logger = logging.getLogger()
+    current_logging_level = root_logger.getEffectiveLevel()
     root_logger.addHandler(handler)
     root_logger.setLevel(logging.DEBUG if if_debug else logging.INFO)
 
-    return handler
+    return handler, current_logging_level
 
 
 def clear_logging_handlers():
     root_logger = logging.getLogger()
     for h in root_logger.handlers[:]:
         root_logger.removeHandler(h)
         h.close()
```

### Comparing `kestrel-lang-1.6.1/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.7.0/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.7.0/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.7.0/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.7.0/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/config.py` & `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import json
 import logging
+import multiprocessing
 
 from kestrel.config import (
     CONFIG_DIR_DEFAULT,
     load_user_config,
 )
 from kestrel.utils import update_nested_dict
 from kestrel.exceptions import InvalidDataSource
@@ -12,15 +13,14 @@
 PROFILE_PATH_DEFAULT = CONFIG_DIR_DEFAULT / "stixshifter.yaml"
 PROFILE_PATH_ENV_VAR = "KESTREL_STIXSHIFTER_CONFIG"
 STIXSHIFTER_DEBUG_ENV_VAR = "KESTREL_STIXSHIFTER_DEBUG"  # debug mode for stix-shifter if the environment variable exists
 ENV_VAR_PREFIX = "STIXSHIFTER_"
 RETRIEVAL_BATCH_SIZE = 2000
 SINGLE_BATCH_TIMEOUT = 60
 FAST_TRANSLATE_CONNECTORS = []  # Suggested: ["qradar", "elastic_ecs"]
-ASYNC_TRANSLATION_WORKERS_CNT = 1
 
 
 _logger = logging.getLogger(__name__)
 
 
 def set_stixshifter_logging_level():
     debug_mode = os.getenv(STIXSHIFTER_DEBUG_ENV_VAR, False)
@@ -203,12 +203,12 @@
     else:
         _logger.debug(
             "either config file does not exist or no stix-shifter options found in config file. This may indicate a config syntax error if config file exists."
         )
         config = {"options": {}}
     if "fast_translate" not in config["options"]:
         config["options"]["fast_translate"] = FAST_TRANSLATE_CONNECTORS
-    if "async_translation_workers_count" not in config["options"]:
-        config["options"][
-            "async_translation_workers_count"
-        ] = ASYNC_TRANSLATION_WORKERS_CNT
+    if "translation_workers_count" not in config["options"]:
+        config["options"]["translation_workers_count"] = min(
+            2, max(1, multiprocessing.cpu_count() - 2)
+        )
     return config["options"]
```

### Comparing `kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from kestrel.exceptions import DataSourceError
 
 
 _logger = logging.getLogger(__name__)
 
 
-XPATH_PYPI_PKG_HOME = "/html/body/main/div[5]/div/div/div[1]/div[2]/ul/li[1]/a/@href"
-XPATH_PYPI_PKG_SOURCE = "/html/body/main/div[5]/div/div/div[1]/div[2]/ul/li[2]/a/@href"
+XPATH_PYPI_PKG_HOME = "/html/body/main/div[4]/div/div/div[1]/div[2]/ul/li[1]/a/@href"
+XPATH_PYPI_PKG_SOURCE = "/html/body/main/div[4]/div/div/div[1]/div[2]/ul/li[2]/a/@href"
 STIX_SHIFTER_HOMEPAGE = "https://github.com/opencybersecurityalliance/stix-shifter"
 
 
 def get_package_name(connector_name):
     return "stix-shifter-modules-" + connector_name.replace("_", "-")
```

### Comparing `kestrel-lang-1.6.1/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.7.0/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.6.1
+Version: 1.7.0
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.6.1/tests/test_command_assign.py` & `kestrel-lang-1.7.0/tests/test_command_assign.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_disp.py` & `kestrel-lang-1.7.0/tests/test_command_disp.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_find.py` & `kestrel-lang-1.7.0/tests/test_command_find.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_get.py` & `kestrel-lang-1.7.0/tests/test_command_get.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_group.py` & `kestrel-lang-1.7.0/tests/test_command_group.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_join.py` & `kestrel-lang-1.7.0/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_load.py` & `kestrel-lang-1.7.0/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_merge.py` & `kestrel-lang-1.7.0/tests/test_command_merge.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_new.py` & `kestrel-lang-1.7.0/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_command_save.py` & `kestrel-lang-1.7.0/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_completion.py` & `kestrel-lang-1.7.0/tests/test_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,18 @@
     with open(profile_file, "w") as pf:
         pf.write(profiles)
 
     os.environ["KESTREL_STIXSHIFTER_CONFIG"] = str(
         profile_file.expanduser().resolve()
     )
 
+    # https://docs.pytest.org/en/latest/how-to/fixtures.html#teardown-cleanup-aka-fixture-finalization
+    yield None
+    del os.environ["KESTREL_STIXSHIFTER_CONFIG"]
+
 
 @pytest.fixture
 def analytics_env_setup(tmp_path):
 
     analytics_module_path = str(
         pathlib.Path(__file__).resolve().parent / "python_analytics_mockup.py"
     )
```

### Comparing `kestrel-lang-1.6.1/tests/test_display.py` & `kestrel-lang-1.7.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_exceptions.py` & `kestrel-lang-1.7.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_expressions.py` & `kestrel-lang-1.7.0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_parser.py` & `kestrel-lang-1.7.0/tests/test_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import re
+from datetime import datetime, timedelta, timezone
 
 from lark import UnexpectedToken
 import pytest
 
 from kestrel.syntax.parser import parse_kestrel, parse_ecgpattern
 from kestrel.syntax.ecgpattern import Reference
 from kestrel.exceptions import InvalidECGPattern
@@ -202,14 +202,63 @@
     assert timefmt(result["timerange"][1]) == "2022-10-19T04:05:06.000Z"
 
     stix = "[process:name = 'asdf'] START t'2022-10-18T01:02:03.000Z' STOP t'2022-10-19T04:05:06.000Z'"
     result["where"].add_center_entity(result["type"])
     assert result["where"].to_stix(result["timerange"], None) == stix
 
 
+@pytest.mark.parametrize(
+    "n, unit, delta",
+    [
+        (1, "d", timedelta(days=1)),
+        (1, "D", timedelta(days=1)),
+        (1, "day", timedelta(days=1)),
+        (1, "DAY", timedelta(days=1)),
+        (1, "days", timedelta(days=1)),
+        (1, "DAYS", timedelta(days=1)),
+        (3, "d", timedelta(days=3)),
+        (3, "D", timedelta(days=3)),
+        (3, "day", timedelta(days=3)),
+        (3, "DAY", timedelta(days=3)),
+        (3, "days", timedelta(days=3)),
+        (3, "DAYS", timedelta(days=3)),
+        (1, "h", timedelta(hours=1)),
+        (1, "H", timedelta(hours=1)),
+        (1, "hour", timedelta(hours=1)),
+        (1, "HOUR", timedelta(hours=1)),
+        (1, "hours", timedelta(hours=1)),
+        (1, "HOURS", timedelta(hours=1)),
+        (2, "H", timedelta(hours=2)),
+        (2, "HOUR", timedelta(hours=2)),
+        (2, "HOURS", timedelta(hours=2)),
+        (1, "m", timedelta(minutes=1)),
+        (1, "minute", timedelta(minutes=1)),
+        (1, "MINUTES", timedelta(minutes=1)),
+        (2, "m", timedelta(minutes=2)),
+        (2, "MINUTES", timedelta(minutes=2)),
+        (90, "s", timedelta(seconds=90)),
+        (90, "SECONDS", timedelta(seconds=90)),
+    ]
+)
+def test_get_timerange_relative(n, unit, delta):
+    now = datetime.now()  #timezone.utc)
+    results = parse_kestrel(f"""
+        x = GET process
+            FROM xxx
+            WHERE name = 'asdf'
+            LAST {n} {unit}
+        """)
+    result = results[0]
+    def close_enough(x, y):
+        print(x, y, y - x)
+        return y - x < timedelta(seconds=30)
+    assert close_enough(result["timerange"][0], now - delta)
+    assert close_enough(result["timerange"][1], now)
+
+
 def test_apply_params():
     results = parse_kestrel("apply xyz://my_analytic on foo with x=1, y=(a, b,c)")
     result = results[0]
     assert result["command"] == "apply"
     assert result["analytics_uri"] == "xyz://my_analytic"
     assert result["inputs"] == ["foo"]
     assert result["arguments"] == {"x": 1, "y": ["a", "b", "c"]}
```

### Comparing `kestrel-lang-1.6.1/tests/test_python_analytics.py` & `kestrel-lang-1.7.0/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.1/tests/test_session.py` & `kestrel-lang-1.7.0/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 def test_session_1(fake_bundle_file):
     with Session(debug_mode=True) as session:
         execute(
             session,
             f"""conns = get network-traffic
             from file://{fake_bundle_file}
-            where [network-traffic:dst_port < 10000]""",
+            where dst_port < 10000""",
         )
         conns = get_df(session, "conns")
         assert len(conns.index) == 100
         execute(session, "sort conns by dst_port asc")
         s = get_df(session, "_")
         assert len(s.index) == 100
         assert s.iloc[0]["dst_port"] == 22
```

### Comparing `kestrel-lang-1.6.1/tests/test_stixshifter.py` & `kestrel-lang-1.7.0/tests/test_stixshifter.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     connectors = ["stix_bundle"]
     for connector_name in connectors:
         check_module_availability(connector_name)
 
 
 def test_yaml_profiles_refresh(tmp_path):
 
-    profileA = f"""profiles:
+    profileA = f"""
 profiles:
     host101:
         connector: elastic_ecs
         connection:
             host: elastic.securitylog.company.com
             port: 9200
             indices: host101
         config:
             auth:
                 id: profileA
                 api_key: qwer
 """
 
-    profileB = f"""profiles:
+    profileB = f"""
 profiles:
     host101:
         connector: elastic_ecs
         connection:
             host: elastic.securitylog.company.com
             port: 9200
             indices: host101
@@ -96,7 +96,9 @@
         connector_name, connection, configuration, retrieval_batch_size = get_datasource_from_profiles("host101", ss_profiles)
         assert connector_name == "elastic_ecs"
         assert configuration["auth"]["id"] == "profileB"
         assert configuration["auth"]["api_key"] == "asdf"
         assert connection["options"]["timeout"] == 120
         assert connection["options"]["result_limit"] == 10000 * 2
         assert retrieval_batch_size == 10000
+
+    del os.environ["KESTREL_STIXSHIFTER_CONFIG"]
```

### Comparing `kestrel-lang-1.6.1/tests/test_timestamped.py` & `kestrel-lang-1.7.0/tests/test_timestamped.py`

 * *Files identical despite different names*

