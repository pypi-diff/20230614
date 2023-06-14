# Comparing `tmp/cli_command_parser-2023.5.8.tar.gz` & `tmp/cli_command_parser-2023.6.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2023.5.8.tar", last modified: Mon May  8 11:55:54 2023, max compression
+gzip compressed data, was "cli_command_parser-2023.6.14.tar", last modified: Wed Jun 14 11:33:24 2023, max compression
```

## Comparing `cli_command_parser-2023.5.8.tar` & `cli_command_parser-2023.6.14.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.577103 cli_command_parser-2023.5.8/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5610 2023-05-08 11:55:54.577103 cli_command_parser-2023.5.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.453103 cli_command_parser-2023.5.8/lib/
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.510103 cli_command_parser-2023.5.8/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1136 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2023-05-08 11:55:42.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0      463 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/actions.py
--rw-rw-rw-   0        0        0     2868 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    22365 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    12631 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    16428 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    16563 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.545104 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0     9987 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    14808 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     8078 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.554103 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     6914 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    20503 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     9198 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5440 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.568104 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2105 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6363 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     8551 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     7734 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0    21187 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6490 2023-01-14 20:20:57.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0    10659 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     7415 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.576103 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      300 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    27355 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    17032 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    10574 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     6884 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    25861 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0     2072 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     4184 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11375 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    15172 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0    10811 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1956 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     4900 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.520104 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     5610 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2314 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/pyproject.toml
--rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/readme.rst
--rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.5.8/requirements-dev.txt
--rw-rw-rw-   0        0        0     1293 2023-05-08 11:55:54.580105 cli_command_parser-2023.5.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.916368 cli_command_parser-2023.6.14/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     5611 2023-06-14 11:33:24.916368 cli_command_parser-2023.6.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.777369 cli_command_parser-2023.6.14/lib/
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.840368 cli_command_parser-2023.6.14/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1158 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2023-06-14 11:33:14.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0     2430 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    19228 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    12619 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    18449 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    18586 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.866369 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8297 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.879368 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     9618 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    20740 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     5445 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.901370 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6582 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     8897 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0     7601 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/patterns.py
+-rw-rw-rw-   0        0        0    22732 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    13618 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.915368 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    16944 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/actions.py
+-rw-rw-rw-   0        0        0    22558 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    16514 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    10656 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     8242 2023-05-21 20:53:58.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    24296 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4422 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    16701 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    12301 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     1882 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     5216 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.850368 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     5611 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.6.14/pyproject.toml
+-rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.6.14/readme.rst
+-rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.6.14/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1293 2023-06-14 11:33:24.917369 cli_command_parser-2023.6.14/setup.cfg
```

### Comparing `cli_command_parser-2023.5.8/LICENSE` & `cli_command_parser-2023.6.14/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/PKG-INFO` & `cli_command_parser-2023.6.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2023.5.8
+Version: 2023.6.14
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/__init__.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     CommandDefinitionError,
     ParameterDefinitionError,
     UsageError,
     ParamUsageError,
     BadArgument,
     InvalidChoice,
     MissingArgument,
+    TooManyArguments,
     NoSuchOption,
     ParserExit,
     ParamConflict,
     ParamsMissing,
     NoActiveContext,
     AmbiguousParseTree,
 )
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/annotations.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/annotations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Utilities for extracting types from annotations.
 
 :author: Doug Skrypa
 """
 
-from __future__ import annotations
-
 from collections.abc import Collection, Iterable
 from inspect import isclass
 from typing import Union, Optional, get_type_hints, get_origin, get_args as _get_args  # pylint: disable=C0412
 
 try:
     from types import NoneType
 except ImportError:  # Added in 3.10
@@ -23,26 +21,22 @@
         annotation = get_type_hints(command_cls)[attr]
     except (KeyError, NameError):  # KeyError due to attr missing; NameError for forward references
         return None
 
     return get_annotation_value_type(annotation)
 
 
-def get_annotation_value_type(annotation) -> Optional[type]:
+def get_annotation_value_type(annotation, from_union: bool = True, from_collection: bool = True) -> Optional[type]:
     origin = get_origin(annotation)
-    # Note on get_origin return values:
-    # get_origin(List[str]) -> list
-    # get_origin(List) -> list
-    # get_origin(list[str]) -> list
-    # get_origin(list) -> None
+    # Note: get_origin returns `list` for `List[str]`, `List`, and `list[str]`; it returns `None` for `list`
     if origin is None and isinstance(annotation, type):
         return annotation
-    elif isclass(origin) and issubclass(origin, (Collection, Iterable)):
+    elif from_collection and isclass(origin) and issubclass(origin, (Collection, Iterable)):
         return _type_from_collection(origin, annotation)
-    elif origin is Union:
+    elif from_union and origin is Union:
         return _type_from_union(annotation)
     return None
 
 
 def get_args(annotation) -> tuple:
     """
     Wrapper around :func:`python:typing.get_args` for 3.7~8 compatibility, to make it behave more like it does in 3.9+
@@ -52,38 +46,18 @@
     return _get_args(annotation)
 
 
 def _type_from_union(annotation) -> Optional[type]:
     args = get_args(annotation)
     # Note: Unions of a single argument return the argument; i.e., Union[T] returns T, so the len can never be 1
     if len(args) == 2 and NoneType in args:
-        arg = args[0] if args[1] is NoneType else args[1]
-    else:
-        return None
-
-    origin = get_origin(arg)
-    if origin is None and isinstance(arg, type):
-        return arg
-    elif isclass(origin) and issubclass(origin, (Collection, Iterable)):
-        return _type_from_collection(origin, arg)
-    else:
-        return None
+        return get_annotation_value_type(args[0] if args[1] is NoneType else args[1], from_union=False)
+    return None
 
 
 def _type_from_collection(origin, annotation) -> Optional[type]:
-    args = get_args(annotation)
-    try:
-        annotation = args[0]
-    except IndexError:  # The annotation was a collection with no content types specified
-        return origin
-
+    if not (args := get_args(annotation)):
+        return origin  # The annotation was a collection with no content types specified
     n_args = len(args)
-    if n_args > 1 and (origin is not tuple or not ((n_args == 2 and args[1] is Ellipsis) or len(set(args)) == 1)):
-        return None
-
-    origin = get_origin(annotation)
-    if origin is None and isinstance(annotation, type):
-        return annotation
-    elif origin is Union:
-        return _type_from_union(annotation)
-    else:
-        return None
+    if n_args == 1 or (origin is tuple and ((n_args == 2 and args[1] is Ellipsis) or len(set(args)) == 1)):
+        return get_annotation_value_type(args[0], from_collection=False)
+    return None
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/command_parameters.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,25 +10,23 @@
 
 from __future__ import annotations
 
 from collections import defaultdict
 from functools import cached_property
 from typing import TYPE_CHECKING, Optional, Collection, Iterator, List, Dict, Set, Tuple
 
-from .actions import help_action
 from .config import CommandConfig, AmbiguousComboMode
-from .exceptions import CommandDefinitionError, ParameterDefinitionError, ParamsMissing
-from .exceptions import AmbiguousShortForm, AmbiguousCombo
+from .exceptions import CommandDefinitionError, ParameterDefinitionError, AmbiguousShortForm, AmbiguousCombo
 from .parameters.base import ParamBase, Parameter, BaseOption, BasePositional
-from .parameters import SubCommand, PassThru, ActionFlag, ParamGroup, Action, Option
+from .parameters import SubCommand, PassThru, ActionFlag, ParamGroup, Action, help_action
 
 if TYPE_CHECKING:
     from .context import Context
     from .formatting.commands import CommandHelpFormatter
-    from .typing import CommandCls
+    from .typing import CommandCls, Strings
 
 __all__ = ['CommandParameters']
 
 OptionMap = Dict[str, BaseOption]
 ActionFlags = List[ActionFlag]
 
 
@@ -64,77 +62,75 @@
 
     def __repr__(self) -> str:
         positionals = len(self.positionals)
         options = len(self.options)
         cls_name = self.__class__.__name__
         return f'<{cls_name}[command={self.command.__name__}, {positionals=}, {options=}]>'
 
+    # region PassThru Properties
+
     @property
     def pass_thru(self) -> Optional[PassThru]:
         if self._pass_thru:
             return self._pass_thru
         elif self.parent:
             return self.parent.pass_thru
         return None
 
+    @property
+    def has_nested_pass_thru(self) -> bool:
+        return any(params._pass_thru for params in self._iter_nested_params())
+
+    # endregion
+
     @cached_property
     def all_positionals(self) -> List[BasePositional]:
         try:
             if not self.parent.sub_command:
                 return self.parent.all_positionals + self.positionals
         except AttributeError:
             pass
         return self.positionals
 
     def get_positionals_to_parse(self, ctx: Context) -> List[BasePositional]:
-        positionals = self.all_positionals
-        if not positionals:
-            return []
-        for i, param in enumerate(positionals):
-            if not ctx.num_provided(param):
-                return [p for p in positionals[i:]]
-        return []
+        if positionals := self.all_positionals:
+            for i, param in enumerate(positionals):
+                if not ctx.num_provided(param):
+                    return [p for p in positionals[i:]]
 
-    @cached_property
-    def always_available_action_flags(self) -> Tuple[ActionFlag, ...]:
-        """
-        The :paramref:`.ActionFlag.before_main` :class:`.ActionFlag` actions that are always available, even if parsing
-        failed (such as the one for ``--help``).
-        """
-        return tuple(af for af in self.action_flags if af.always_available)
+        return []
 
     @cached_property
     def formatter(self) -> CommandHelpFormatter:
         from .formatting.commands import CommandHelpFormatter
 
         formatter_factory = self.config.command_formatter or CommandHelpFormatter
         formatter = formatter_factory(self.command, self)
         formatter.maybe_add_positionals(self.all_positionals)
         formatter.maybe_add_option(self._pass_thru)
         formatter.maybe_add_options(self.options)
         formatter.maybe_add_groups(self.groups)
         return formatter
 
-    @property
+    @cached_property
     def _has_help(self) -> bool:
-        return help_action in self.always_available_action_flags or (self.parent and self.parent._has_help)
+        return help_action in self.action_flags or (self.parent and self.parent._has_help)
 
     # region Initialization
 
     def _iter_parameters(self) -> Iterator[ParamBase]:
         name_param_map = {}  # Allow subclasses to override names, but not within a given command
-        for attr, param in self.command.__dict__.items():
+        for item in self.command.__dict__.items():
+            attr, param = item
             if attr.startswith('__') or not isinstance(param, ParamBase):  # Name mangled Parameters are still processed
                 continue
-            try:
-                other_attr, other_param = name_param_map[param.name]
-            except KeyError:
-                name_param_map[param.name] = (attr, param)
-                yield param
+            elif (other := name_param_map.setdefault(param.name, item)) is item:
+                yield param  # There was no other param with the same name
             else:
+                other_attr, other_param = other
                 raise CommandDefinitionError(
                     'Name conflict - multiple parameters within a Command cannot have the same name - conflicting'
                     f' params: {other_attr}={other_param}, {attr}={param}'
                 )
 
     def _process_parameters(self):
         """
@@ -159,35 +155,35 @@
                 self._pass_thru = param
             else:
                 raise CommandDefinitionError(
                     f'Unexpected type={param.__class__} for {param=} - custom parameters must extend'
                     ' BasePositional, BaseOption, or ParamGroup'
                 )
 
-            if param.group:
-                _find_groups(groups, param)
+            param_group = param
+            while param_group := param_group.group:
+                groups.add(param_group)
 
         if self.config.add_help and self.command_parent is not None and (not self.parent or not self.parent._has_help):
             options.append(help_action)
 
         self._process_positionals(positionals)
         self._process_options(options)
         self._process_groups(groups)
 
     def _process_groups(self, groups: Set[ParamGroup]):
         if self.parent:
-            _groups, groups = groups, self.parent.groups.copy()
-            groups.extend(_groups)
-
-        self.groups = sorted(groups)
+            self.groups = sorted((*self.parent.groups, *groups)) if groups else self.parent.groups.copy()
+        else:
+            self.groups = sorted(groups) if groups else []
 
     def _process_positionals(self, params: List[BasePositional]):
         unfollowable = action_or_sub_cmd = split_index = None
-        if (parent := self.parent) and parent._deferred_positionals:
-            params = parent._deferred_positionals + params
+        if self.parent and (deferred := self.parent._deferred_positionals):
+            params = deferred + params
 
         for i, param in enumerate(params):
             if unfollowable:
                 if 0 in unfollowable.nargs:
                     why = 'because it is a positional that is not required'
                 else:
                     why = 'because it accepts a variable number of arguments with no specific choices defined'
@@ -216,57 +212,56 @@
             if self.sub_command.has_local_choices:
                 self._deferred_positionals = params[split_index:]
             else:
                 params, self._deferred_positionals = params[:split_index], params[split_index:]
 
         self.positionals = params
 
-    def _process_options(self, params: Collection[BaseOption]):
+    def _process_options(self, params: List[BaseOption]):
         if parent := self.parent:
             option_map = parent.option_map.copy()
             combo_option_map = parent.combo_option_map.copy()
-            options = parent.options.copy()
+            self.options = parent.options + params
         else:
             option_map = {}
             combo_option_map = {}
-            options = []
+            self.options = params
 
         for param in params:
-            options.append(param)
             opts = param.option_strs
-            if not opts.has_min_opts():
+            if not opts.has_min_opts():  # This is checked here and not earlier due to possible additions in set_name
                 raise ParameterDefinitionError(f'No option strings were registered for {param=}')
-            self._process_option_strs(param, 'long', opts.long, option_map, combo_option_map)
-            self._process_option_strs(param, 'short', opts.short, option_map, combo_option_map)
-
-        self.options = options
-        self.option_map = option_map
-        self._process_action_flags(options)
-        self.combo_option_map = dict(sorted(combo_option_map.items(), key=lambda kv: (-len(kv[0]), kv[0])))  # noqa
 
-        if self.config.ambiguous_short_combos == AmbiguousComboMode.STRICT:
-            self._strict_ambiguous_short_combo_check()
-
-    def _process_option_strs(
-        self, param: BaseOption, opt_type: str, opt_strs: List[str], option_map: OptionMap, combo_option_map: OptionMap
-    ):
-        for opt in opt_strs:
-            try:
-                existing = option_map[opt]
-            except KeyError:
-                option_map[opt] = param
-                if opt_type == 'short':
+            long_opts, short_opts = opts.get_sets()
+            self._process_option_strs(param, 'long', long_opts, option_map)
+            if short_opts:
+                self._process_option_strs(param, 'short', short_opts, option_map)
+                for opt in short_opts:
                     combo_option_map[opt[1:]] = param
+
+        self.option_map = option_map
+        self._process_action_flags()
+        self.combo_option_map = dict(sorted(combo_option_map.items(), key=_sort_kv))
+        if self.config.ambiguous_short_combos == AmbiguousComboMode.STRICT and self._potentially_ambiguous_combo_opts:
+            raise AmbiguousShortForm({p: c.values() for p, c in self._potentially_ambiguous_combo_opts.values()})
+
+    def _process_option_strs(self, param: BaseOption, opt_type: str, opt_strs: Strings, option_map: OptionMap):
+        for option in opt_strs:
+            if option not in option_map:
+                option_map[option] = param
             else:
+                # It is more efficient for the typical code path to avoid a try/except or .get call since the
+                # likelihood of a conflict is extremely low, and the extra lookup is acceptable for the error case.
+                existing = option_map[option]
                 raise CommandDefinitionError(
-                    f'{opt_type} option={opt!r} conflict for command={self.command!r} between {existing} and {param}'
+                    f'{opt_type} {option=} conflict for command={self.command!r} between {existing} and {param}'
                 )
 
-    def _process_action_flags(self, options: List[BaseOption]):
-        action_flags = sorted((p for p in options if isinstance(p, ActionFlag)))
+    def _process_action_flags(self):
+        action_flags = sorted(p for p in self.options if isinstance(p, ActionFlag))
         grouped_ordered_flags = {True: defaultdict(list), False: defaultdict(list)}
         for param in action_flags:
             if param.func is None:
                 raise ParameterDefinitionError(f'No function was registered for {param=}')
             grouped_ordered_flags[param.before_main][param.order].append(param)  # noqa  # PyCharm infers the wrong type
 
         found_non_always = False
@@ -298,221 +293,126 @@
         self.action_flags = action_flags
         self.split_action_flags = action_flags[:n_before], action_flags[n_before:]
 
     # endregion
 
     # region Ambiguous Short Combo Handling
 
-    def _strict_ambiguous_short_combo_check(self):
-        # Called during initial Option processing when using AmbiguousComboMode.STRICT
-        if not (potentially_ambiguous_combo_options := self._potentially_ambiguous_combo_options):
-            return
-
-        param_conflicts_map = {
-            param: singles.values() for param, singles in potentially_ambiguous_combo_options.values()
-        }
-        raise AmbiguousShortForm(param_conflicts_map)
-
     @cached_property
     def _classified_combo_options(self) -> Tuple[OptionMap, OptionMap]:
         multi_char_combos = {}
-        single_char_combos = {}
-        for combo, param in self.combo_option_map.items():
-            if len(combo) == 1:
-                single_char_combos[combo] = param
-            else:
-                multi_char_combos[combo] = param
-        return single_char_combos, multi_char_combos
+        items = self.combo_option_map.items()
+        for combo, param in items:
+            if len(combo) == 1:  # combo_option_map is sorted in reverse length order, so all following will be 1 char
+                return dict([(combo, param), *items]), multi_char_combos
+            multi_char_combos[combo] = param
+        return {}, multi_char_combos
 
     @cached_property
-    def _potentially_ambiguous_combo_options(self) -> Dict[str, Tuple[BaseOption, OptionMap]]:
-        single_char_combos, multi_char_combos = self._classified_combo_options
-        if not multi_char_combos:
-            return {}
-        return _find_ambiguous_combos(single_char_combos, multi_char_combos)
+    def _potentially_ambiguous_combo_opts(self) -> Dict[str, Tuple[BaseOption, OptionMap]]:
+        return _find_ambiguous_combos(*self._classified_combo_options)
 
     @cached_property
     def _nested_potentially_ambiguous_combo_options(self):
-        single_char_combos, multi_char_combos = self._classified_combo_options
+        single_char_combos, multi_char_combos = (xcc.copy() for xcc in self._classified_combo_options)
         for params in self._iter_nested_params():
             nested_single_char_combos, nested_multi_char_combos = params._classified_combo_options
             single_char_combos.update(nested_single_char_combos)
             multi_char_combos.update(nested_multi_char_combos)
-
-        if not multi_char_combos:
-            return {}
         return _find_ambiguous_combos(single_char_combos, multi_char_combos)
 
     def _is_combo_potentially_ambiguous(self, option: str) -> Optional[bool]:
         # Called by short_option_to_param_value_pairs after ensuring the length is > 1
         to_check = option[1:]  # Strip leading '-'
         # Note: len(to_check) will never be 2 here - this is only called if len(option) > 2
-        potentially_ambiguous_combo_options = self._nested_potentially_ambiguous_combo_options
         acm = self.config.ambiguous_short_combos
-        if acm == AmbiguousComboMode.PERMISSIVE and to_check in potentially_ambiguous_combo_options:
+        if acm == AmbiguousComboMode.PERMISSIVE and to_check in self._nested_potentially_ambiguous_combo_options:
             return True  # Permissive mode allows exact matches of multi-char short forms
         elif acm == AmbiguousComboMode.IGNORE:
             return None
 
         ambiguous = set()
-        for multi, (param, singles) in potentially_ambiguous_combo_options.items():
+        for multi, (param, singles) in self._nested_potentially_ambiguous_combo_options.items():
             if multi in to_check:
                 ambiguous.add(param)
                 ambiguous.update(p for c, p in singles.items() if c in to_check)
 
         if ambiguous:
             raise AmbiguousCombo(ambiguous, option)
 
         return False
 
     # endregion
 
-    # region Option Processing
-
     def _iter_nested_params(self) -> Iterator[CommandParameters]:
         if not self.sub_command:
             return
+        get_params = self.command.__class__.params
         for choice in self.sub_command.choices.values():
-            command = choice.target
-            try:
-                yield command.__class__.params(command)
-            except AttributeError:  # The target was None (it's a subcommand's local choice)
-                pass
+            if choice.target is not None:  # None indicates it's a subcommand's local choice
+                params: CommandParameters = get_params(choice.target)
+                yield params
+                yield from params._iter_nested_params()
 
-    def get_option_param_value_pairs(self, option: str) -> Optional[Tuple[BaseOption, ...]]:
-        if option.startswith('---'):
-            return None
-        elif option.startswith('--'):
-            try:
-                opt, param, value = self.long_option_to_param_value_pair(option)
-            except KeyError:
-                return None
-            else:
-                return (param,)  # noqa
-        elif option.startswith('-'):
-            try:
-                param_value_pairs = self.short_option_to_param_value_pairs(option)
-            except KeyError:
-                return None
-            else:
-                return tuple(param for opt, param, value in param_value_pairs)
-        else:
-            return None
-
-    def long_option_to_param_value_pair(self, option: str) -> Tuple[str, BaseOption, Optional[str]]:
-        try:
-            return option, self.option_map[option], None
-        except KeyError:
-            if '=' in option:
-                option, value = option.split('=', 1)
-                return option, self.option_map[option], value
-            else:
-                raise
+    # region Option Processing
 
-    def short_option_to_param_value_pairs(self, option: str) -> List[Tuple[str, BaseOption, Optional[str]]]:
-        try:
-            option, value = option.split('=', 1)
-        except ValueError:
-            value = None
-        else:
+    def short_option_to_param_value_pairs(
+        self, option: str
+    ) -> Tuple[List[Tuple[str, BaseOption, Optional[str]]], bool]:
+        option, eq, value = option.partition('=')
+        if eq:  # An `=` was present in the string
             # Note: if the option is not in this Command's option_map, the KeyError is handled by CommandParser
-            return [(option, self.option_map[option], value)]
+            return [(option, self.option_map[option], value)], True
+        else:
+            value = None
 
         try:
             param = self.option_map[option]
         except KeyError:
             opt_len = len(option)
             if opt_len < 2 or (opt_len > 2 and self._is_combo_potentially_ambiguous(option)):
                 raise
         else:
-            return [(option, param, value)]
+            return [(option, param, value)], False
 
         key, value = option[1], option[2:]
         # value will never be empty if key is a valid option because by this point, option is not a short option
-        combo_option_map = self.combo_option_map
-        param = combo_option_map[key]
-        if param.would_accept(value, short_combo=True):
-            return [(key, param, value)]
+        param = self.combo_option_map[key]
+        if param.action.would_accept(value, combo=True):
+            return [(key, param, value)], False
         else:
             # Multi-char short options can never be combined with each other, but single-char ones can
-            return [(c, combo_option_map[c], None) for c in option[1:]]
-
-    def find_option_that_accepts_values(self, option: str) -> Optional[BaseOption]:
-        if option.startswith('--'):
-            param = self.long_option_to_param_value_pair(option)[1]
-            if param.accepts_values:
-                return param
-        elif option.startswith('-'):
-            for _, param, _ in self.short_option_to_param_value_pairs(option):
-                if param.accepts_values:
-                    return param
-        else:
-            raise ValueError(f'Invalid {option=}')
-        return None
-
-    def find_nested_option_that_accepts_values(self, option: str) -> Optional[BaseOption]:
-        for params in self._iter_nested_params():
-            try:
-                param = params.find_option_that_accepts_values(option)
-            except KeyError:
-                pass
-            else:
-                if param is not None:
-                    return param
-
-            param = params.find_nested_option_that_accepts_values(option)
-            if param is not None:
-                return param
-
-        return None
-
-    def find_nested_pass_thru(self) -> Optional[PassThru]:
-        for params in self._iter_nested_params():
-            if params._pass_thru:
-                return params._pass_thru
-
-        return None
+            return [(c, self.combo_option_map[c], None) for c in option[1:]], False
 
     # endregion
 
-    def validate_groups(self):
-        exc = None
-        for group in self.groups:
-            try:
-                group.validate()
-            except ParamsMissing as e:  # Let ParamConflict propagate before ParamsMissing
-                if exc is None:
-                    exc = e
-
-        if exc is not None:
-            raise exc
-
-    def try_env_params(self, ctx: Context) -> Iterator[Option]:
-        """Yields Option parameters that have an environment variable configured, and did not have any CLI values."""
-        for param in self.options:
-            if param.env_var and ctx.num_provided(param) == 0:
-                yield param
+    def iter_params(self, exclude: Collection[Parameter] = ()) -> Iterator[Parameter]:
+        if exclude:
+            yield from (p for g in (self.all_positionals, self.options) for p in g if p not in exclude)
+        else:
+            yield from self.all_positionals
+            yield from self.options
+        if (pass_thru := self.pass_thru) and pass_thru not in exclude:
+            yield pass_thru
 
     def required_check_params(self) -> Iterator[Parameter]:
         ignore = SubCommand
         yield from (p for p in self.all_positionals if p.required and not p.group and not isinstance(p, ignore))
         yield from (p for p in self.options if p.required and not p.group)
         if (pass_thru := self._pass_thru) and pass_thru.required and not pass_thru.group:
             yield pass_thru
 
 
-def _find_groups(groups: Set[ParamGroup], param: ParamBase):
-    group = param.group
-    while group:
-        groups.add(group)
-        group = group.group
-
-
 def _find_ambiguous_combos(
     single_char_combos: OptionMap, multi_char_combos: OptionMap
 ) -> Dict[str, Tuple[BaseOption, OptionMap]]:
     ambiguous_combo_options = {}
     for combo, param in multi_char_combos.items():
         if singles := {c: single_char_combos[c] for c in combo if c in single_char_combos}:
             ambiguous_combo_options[combo] = (param, singles)
 
     return ambiguous_combo_options
+
+
+def _sort_kv(kv):
+    k = kv[0]
+    return -len(k), k
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/commands.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from abc import ABC
 from contextlib import ExitStack
 from typing import TYPE_CHECKING, Type, Sequence, Optional, overload
 
 from .core import CommandMeta, get_top_level_commands, get_params
 from .context import Context, ActionPhase, get_or_create_context
 from .exceptions import ParamConflict
-from .parser import CommandParser
+from .parser import parse_args_and_get_next_cmd
 
 if TYPE_CHECKING:
     from .typing import Bool, CommandObj
 
 __all__ = ['Command', 'main']
 log = logging.getLogger(__name__)
 
@@ -29,19 +29,18 @@
     """The main class that other Commands should extend."""
 
     #: The parsing Context used for this Command. Provided here for convenience - this reference to it is not used by
     #: any CLI Command Parser internals, so it is safe for subclasses to redefine / overwrite it.
     ctx: Context
 
     def __new__(cls):
-        ctx = get_or_create_context(cls)
         # By storing the Context here instead of __init__, every single subclass won't need to
         # call super().__init__(...) from their own __init__ for this step
         self = super().__new__(cls)
-        self.__ctx = ctx
+        self.__ctx = ctx = get_or_create_context(cls)
         if not hasattr(self, 'ctx'):
             self.ctx: Context = ctx  # noqa  # PyCharm complains this is invalid, but doesn't understand it without it
         return self
 
     def __repr__(self) -> str:
         cls = self.__class__
         return f'<{cls.__name__} in prog={cls.__class__.meta(cls).prog!r}>'
@@ -108,15 +107,15 @@
         :param argv: The arguments to parse (defaults to :data:`sys.argv`)
         :return: A Command instance with parsed arguments that is ready for :meth:`.__call__` or :meth:`.main`
         """
         ctx = get_or_create_context(cls, argv)
         cmd_cls = cls
         with ExitStack() as stack:
             stack.enter_context(ctx)
-            while sub_cmd := CommandParser.parse_args_and_get_next_cmd(ctx):
+            while sub_cmd := parse_args_and_get_next_cmd(ctx):
                 cmd_cls = sub_cmd
                 ctx = stack.enter_context(ctx._sub_context(cmd_cls))
 
             return cmd_cls()
 
     # endregion
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/compat.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/compat.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/config.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from __future__ import annotations
 
 from collections import ChainMap
 from enum import Enum
 from typing import TYPE_CHECKING, Optional, Any, Union, Callable, Type, TypeVar, Generic, overload, Dict
 
-from .utils import FixedFlag, MissingMixin, _NotSet
+from .utils import FixedFlag, MissingMixin, _NotSet, positive_int
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .error_handling import ErrorHandler
     from .formatting.commands import CommandHelpFormatter
     from .formatting.params import ParamHelpFormatter
     from .typing import Bool, ParamOrGroup, CommandType
@@ -74,34 +74,38 @@
 class OptionNameMode(FixedFlag):
     """
     How the default long form that is added for Option/Flag/Counter/etc. Parameters should handle underscores/dashes.
 
     Given a Parameter defined as ``foo_bar = Option(...)``, the default long form handling based on this setting would
     be:
 
-    :UNDERSCORE: ``--foo_bar``
-    :DASH: ``--foo-bar``
-    :BOTH: Both ``--foo-bar`` and ``--foo_bar`` will be accepted
+    :UNDERSCORE: ``--foo_bar`` - the attribute name is used verbatim.
+    :DASH: ``--foo-bar`` - any underscores present in the attribute name will be replaced with dashes (this is
+      the default behavior).
+    :BOTH: Both ``--foo-bar`` and ``--foo_bar`` will be accepted, and both will be displayed in help text.
     :BOTH_UNDERSCORE: Both ``--foo-bar`` and ``--foo_bar`` will be accepted, but only ``--foo_bar`` with be displayed
-      in help text
+      in help text.  This may be useful for compatibility purposes, and helps prevent help text from being too
+      cluttered.
     :BOTH_DASH: Both ``--foo-bar`` and ``--foo_bar`` will be accepted, but only ``--foo-bar`` with be displayed
-      in help text
+      in help text.  This may be useful for compatibility purposes, and helps prevent help text from being too
+      cluttered.
     :NONE: No long form option string will be added.  At least one short form option string must be defined.  Note that
-      it is NOT necessary to use ``name_mode=None`` to prevent the automatic creation of long form option strings - if
-      any long form option strings are explicitly provided for a given Parameter, then no automatic ones will be added.
+      it is NOT necessary to use ``name_mode=None`` to prevent the automatic creation of long form option strings in
+      general.  If any long form option strings are explicitly provided for a given Parameter, then an automatic one
+      will not be added, regardless of value for this configuration option.
 
     If a long form is provided explicitly for a given optional Parameter, then this setting will be ignored.
 
     The value may be specified to Commands as ``option_name_mode=<mode>`` or to Parameters as ``name_mode=<mode>``,
     where ``<mode>`` is one of:
 
+        - ``'_'`` or ``'-'`` or ``'*'`` or ``'*_'`` or ``'*-'`` or ``'_*'`` or ``'-*'`` or ``None``
         - ``OptionNameMode.UNDERSCORE`` or ``OptionNameMode.DASH`` or ``OptionNameMode.BOTH``
-          or ``OptionNameMode.BOTH_UNDERSCORE`` or ``OptionNameMode.BOTH_DASH``
-        - ``'underscore'`` or ``'dash'`` or ``'both'`` or ``'both_underscore'`` or ``'both_dash'``
-        - ``'_'`` or ``'-'`` or ``'*'`` or ``'*_'`` or ``'*-'``
+          or ``OptionNameMode.BOTH_UNDERSCORE`` or ``OptionNameMode.BOTH_DASH`` or ``OptionNameMode.NONE``
+        - ``'underscore'`` or ``'dash'`` or ``'both'`` or ``'both_underscore'`` or ``'both_dash'`` or ``'none'``
     """
 
     UNDERSCORE = 1
     DASH = 2
     BOTH = 3                # = 1|2
     #                         & 4  -> display options set
     BOTH_UNDERSCORE = 15    # & 8  -> show only underscore version
@@ -153,21 +157,14 @@
     COMBINE = 'combine'     # Combine aliases onto a single line
     ALIAS = 'alias'         # Indicate the subcommand that it is an alias for; do not repeat the description
 
 
 CmdAliasMode = Union[SubcommandAliasHelpMode, str]
 
 
-def _cmd_alias_mode(mode: CmdAliasMode) -> CmdAliasMode:
-    try:
-        return SubcommandAliasHelpMode(mode)
-    except ValueError:
-        return mode
-
-
 class AmbiguousComboMode(MissingMixin, Enum):
     """
     Options for handling potentially ambiguous combinations of short forms of Option / Flag / etc. Parameters.
 
     The behavior based on each supported option:
 
     :IGNORE: Ignore potentially ambiguous combinations of short options entirely.  Best effort parsing will be
@@ -213,18 +210,21 @@
             return cls.NEVER
         return super()._missing_(value)  # noqa
 
 
 # endregion
 
 
+# region Config Item Descriptors / Decorators
+
+
 class ConfigItem(Generic[CV, DV]):
     __slots__ = ('default', 'type', 'name')
 
-    def __init__(self, default: DV, type: Callable[[Any], CV] = None):  # noqa
+    def __init__(self, default: DV, type: Callable[..., CV] = None):  # noqa
         self.default = default
         self.type = type
 
     def __set_name__(self, owner: Type[CommandConfig], name: str):
         self.name = name
         owner.FIELDS.add(name)
 
@@ -240,30 +240,50 @@
         if instance is None:
             return self
         return instance._data.get(self.name, self.default)
 
     def __set__(self, instance: CommandConfig, value: ConfigValue):
         if instance._read_only:
             raise AttributeError(f'Unable to set attribute {self.name}={value!r} because {instance} is read-only')
-        elif self.type is not None:
-            value = self.type(value)
+        elif (type_func := self.type) is not None:
+            value = type_func(value)
         instance._data[self.name] = value
 
     def __delete__(self, instance: CommandConfig):
         if instance._read_only:
             raise AttributeError(f'Unable to delete attribute {self.name} because {instance} is read-only')
         try:
             del instance._data[self.name]
         except KeyError as e:
             raise AttributeError(f'No {self.name!r} config was stored for {instance}') from e
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}({self.default!r}, type={self.type!r})>'
 
 
+class DynamicConfigItem(ConfigItem):
+    __slots__ = ('__doc__',)
+
+    def __init__(self, default: DV, type: Callable[..., CV]):  # noqa
+        super().__init__(default, type)
+        self.__doc__ = type.__doc__
+
+    def __set__(self, instance: CommandConfig, value: ConfigValue):
+        if instance._read_only:
+            raise AttributeError(f'Unable to set attribute {self.name}={value!r} because {instance} is read-only')
+        instance._data[self.name] = self.type(instance, value)
+
+
+def config_item(default: DV):
+    return lambda func: DynamicConfigItem(default, func)
+
+
+# endregion
+
+
 class CommandConfig:
     """Configuration options for Commands."""
 
     # Note: PyCharm may incorrectly think ConfigItem attrs are read only: https://youtrack.jetbrains.com/issue/PY-29770
 
     __slots__ = ('_data', '_read_only')
     _data: ChainMap
@@ -328,20 +348,28 @@
     #: Whether the metavar for Parameters that accept values should default to the name of the specified type
     #: (default: the name of the parameter)
     use_type_metavar: Bool = ConfigItem(False, bool)
 
     #: Whether the default value for Parameters should be shown in help text, and related behavior
     show_defaults: ShowDefaults = ConfigItem(ShowDefaults.MISSING | ShowDefaults.NON_EMPTY, ShowDefaults)
 
-    #: How subcommand aliases should be displayed in help text.
-    cmd_alias_mode: CmdAliasMode = ConfigItem(None, _cmd_alias_mode)  # noqa
+    @config_item(None)
+    def cmd_alias_mode(self, value: CmdAliasMode) -> CmdAliasMode:
+        """How subcommand aliases should be displayed in help text."""
+        try:
+            return SubcommandAliasHelpMode(value)
+        except ValueError:
+            return value
 
     #: Whether Parameter `choices` values and Action / Subcommand choices should be sorted
     sort_choices: Bool = ConfigItem(False, bool)
 
+    #: Delimiter to use between choices in usage / help text
+    choice_delim: str = ConfigItem('|', str)
+
     #: Whether there should be a visual indicator in help text for the parameters that are members of a given group
     show_group_tree: Bool = ConfigItem(False, bool)
 
     #: Whether mutually exclusive / dependent groups should include that fact in their descriptions
     show_group_type: Bool = ConfigItem(True, bool)
 
     #: A callable that accepts 2 arguments, a :class:`.Command` class (not object) and a :class:`.CommandParameters`
@@ -351,26 +379,43 @@
     #: A callable that accepts a :class:`.Parameter` or :class:`.ParamGroup` and returns a :class:`.ParamHelpFormatter`
     param_formatter: Callable[[ParamOrGroup], ParamHelpFormatter] = ConfigItem(None)
 
     #: Whether the program version, author email, and documentation URL should be included in the help text epilog, if
     #: they were successfully detected
     extended_epilog: Bool = ConfigItem(True, bool)
 
-    #: Whether the top level script's docstring should be included in generated documentation
-    show_docstring: Bool = ConfigItem(True, bool)
-
-    #: Delimiter to use between choices in usage / help text
-    choice_delim: str = ConfigItem('|', str)
-
     #: Width (in characters) for the usage column in help text
     usage_column_width: int = ConfigItem(30, int)
 
     #: Min width (in chars) for the usage column in help text after adjusting for group indentation / terminal width
     min_usage_column_width: int = ConfigItem(20, int)
 
+    @config_item(False)
+    def wrap_usage_str(self, value: Any) -> Union[int, bool]:
+        """
+        Wrap the basic usage string after the specified number of characters, or automatically based on terminal size
+        if ``True`` is specified instead.
+        """
+        if value is True or value is False:
+            return value
+        return positive_int(value, 'a bool or a positive integer', min_val=1)
+
+    # endregion
+
+    # region Documentation Generation Options
+
+    #: Whether the top level script's docstring should be included in generated documentation
+    show_docstring: Bool = ConfigItem(True, bool)
+
+    #: Whether inherited descriptions should be included in subcommand sections of generated documentation
+    show_inherited_descriptions: Bool = ConfigItem(False, bool)
+
+    #: Maximum subcommand depth to include in generated documentation (default: include all)
+    sub_cmd_doc_depth: int = ConfigItem(None, positive_int)
+
     # endregion
 
     def __init__(self, parent: Optional[CommandConfig] = None, read_only: bool = False, **kwargs):
         self._data = parent._data.new_child() if parent else ChainMap()
         self._read_only = read_only
         if kwargs:
             try:
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/context.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from functools import cached_property
 from inspect import Signature, Parameter as _Parameter
 from typing import TYPE_CHECKING, Any, Callable, Union, Sequence, Optional, Iterator, Collection, cast
 from typing import Dict, Tuple, List
 
 from .config import CommandConfig, DEFAULT_CONFIG
 from .error_handling import ErrorHandler, NullErrorHandler, extended_error_handler
-from .exceptions import NoActiveContext, MissingArgument
+from .exceptions import NoActiveContext
 from .utils import _NotSet, Terminal
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .commands import Command
-    from .parameters import Parameter, ActionFlag
+    from .parameters import Parameter, Option, ActionFlag
     from .typing import Bool, ParamOrGroup, CommandType, AnyConfig, OptStr, PathLike
 
 __all__ = ['Context', 'ctx', 'get_current_context', 'get_or_create_context', 'get_context', 'get_parsed', 'get_raw_arg']
 
-_context_stack = ContextVar('cli_command_parser.context.stack', default=[])
+_context_stack = ContextVar('cli_command_parser.context.stack')
 _TERMINAL = Terminal()
 
 
 class Context(AbstractContextManager):  # Extending AbstractContextManager to make PyCharm's type checker happy
     """
     The parsing context.
 
@@ -57,33 +57,28 @@
         terminal_width: int = None,
         allow_argv_prog: Bool = None,
         **kwargs,
     ):
         self.command = command
         self.parent = parent
         self.config = _normalize_config(config, kwargs, parent, command)
+        self.actions_taken = 0
         if parent:
             self._set_argv(parent.prog, argv)
             self._parsed = parent._parsed.copy()
-            self.unknown = parent.unknown.copy()
             self._provided = parent._provided.copy()
-            if terminal_width is None:
-                terminal_width = parent._terminal_width
-            if allow_argv_prog is None:
-                allow_argv_prog = parent.allow_argv_prog
+            self._terminal_width = parent._terminal_width if terminal_width is None else terminal_width
+            self.allow_argv_prog = parent.allow_argv_prog if allow_argv_prog is None else allow_argv_prog
         else:
             self._set_argv(None, argv)
             self._parsed = {}
-            self.unknown = {}
             self._provided = defaultdict(int)
-
-        self._terminal_width = terminal_width
-        if allow_argv_prog is not None:
-            self.allow_argv_prog = allow_argv_prog
-        self.actions_taken = 0
+            self._terminal_width = terminal_width
+            if allow_argv_prog is not None:
+                self.allow_argv_prog = allow_argv_prog
 
     # region Internal Methods
 
     @classmethod
     def for_prog(cls, prog: PathLike, *args, **kwargs) -> Context:
         self = cls(*args, **kwargs)
         self.prog = getattr(prog, 'name', prog)
@@ -101,18 +96,23 @@
 
     def _sub_context(self, command: CommandType, argv: Optional[Sequence[str]] = None, **kwargs) -> Context:
         if argv is None:
             argv = self.remaining
         return self.__class__(argv, command, parent=self, **kwargs)
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__}[command={getattr(self.command, "__name__", None)}]>'
+        command = getattr(self.command, '__name__', None)
+        prog, argv, allow_argv_prog = self.prog, self.argv, self.allow_argv_prog
+        return f'<{self.__class__.__name__}[{command=!s}, {prog=}, {allow_argv_prog=}, {argv=}]>'
 
     def __enter__(self) -> Context:
-        _context_stack.get().append(self)
+        try:
+            _context_stack.get().append(self)
+        except LookupError:
+            _context_stack.set([self])
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         _context_stack.get().pop()
 
     def __contains__(self, param: Union[ParamOrGroup, str, Any]) -> bool:
         try:
@@ -130,93 +130,107 @@
             return True
 
     # endregion
 
     @property
     def terminal_width(self) -> int:
         """Returns the current terminal width as the number of characters that fit on a single line."""
-        if self._terminal_width is not None:
-            return self._terminal_width
+        if (width := self._terminal_width) is not None:
+            return width
         return _TERMINAL.width
 
-    def get_parsed(self, exclude: Collection[Parameter] = (), recursive: Bool = True) -> Dict[str, Any]:
+    def get_parsed(
+        self, exclude: Collection[Parameter] = (), recursive: Bool = True, default: Any = None
+    ) -> Dict[str, Any]:
         """
         Returns all of the parsed arguments as a dictionary.
 
         The :ref:`get_parsed() <advanced:Parsed Args as a Dictionary>` helper function provides an easier way to access
         this functionality.
 
         :param exclude: Parameter objects that should be excluded from the returned results
         :param recursive: Whether parsed arguments should be recursively gathered from parent Commands
+        :param default: The default value to use for parameters that raise :class:`.MissingArgument` when attempting to
+          obtain their result values.
         :return: A dictionary containing all of the arguments that were parsed.  The keys in the returned dict match
           the names assigned to the Parameters in the Command associated with this Context.
         """
         with self:
-            if recursive and self.parent:
-                parsed = self.parent.get_parsed(exclude, recursive)
+            if recursive and (parent := self.parent):
+                parsed = parent.get_parsed(exclude, recursive)
             else:
                 parsed = {}
 
             if params := self.params:
-                for group in (params.all_positionals, params.options, (params.pass_thru,)):
-                    for param in group:
-                        if param and param not in exclude:
-                            try:
-                                parsed[param.name] = param.result_value()
-                            except MissingArgument:
-                                parsed[param.name] = None
+                for param in params.iter_params(exclude):
+                    parsed[param.name] = param.result_value(default)
 
         return parsed
 
     @cached_property
     def params(self) -> Optional[CommandParameters]:
         """
         The :class:`.CommandParameters` object that contains the categorized Parameters from the Command associated
         with this Context.
         """
-        try:
-            return self.command.__class__.params(self.command)
-        except AttributeError:  # self.command is None
-            return None
+        if (command := self.command) is not None:
+            return command.__class__.params(command)
+        return None
 
     def get_error_handler(self) -> Union[ErrorHandler, NullErrorHandler]:
         """Returns the :class:`.ErrorHandler` configured to be used."""
         if (error_handler := self.config.error_handler) is _NotSet:
             return extended_error_handler
         elif error_handler is None:
             return NullErrorHandler()
         else:
             return error_handler
 
-    # region Parsing
+    # region Parsing Methods - Generally not intended to be called by users
 
-    def get_parsed_value(self, param: Parameter):
+    def has_parsed_value(self, param: Parameter) -> bool:
+        return param in self._parsed
+
+    def get_parsed_value(self, param: Parameter, default=_NotSet):
         """Not intended to be called by users.  Used by Parameters to access their parsed values."""
-        try:
-            return self._parsed[param]
-        except KeyError:
-            self._parsed[param] = value = param._init_value_factory()
-            return value
+        return self._parsed.get(param, default)
 
     def set_parsed_value(self, param: Parameter, value: Any):
         """Not intended to be called by users.  Used by Parameters during parsing to store parsed values."""
         self._parsed[param] = value
 
+    def pop_parsed_value(self, param: Parameter):
+        """Not intended to be called by users.  Used by Parameters during parsing if backtracking is necessary."""
+        self._provided[param] = 0
+        return self._parsed.pop(param)
+
+    def roll_back_parsed_values(self, param: Parameter, count: int):
+        """Not intended to be called by users.  Used during parsing as part of backtracking."""
+        values = self._parsed[param]
+        self._parsed[param] = values[:-count]
+        self._provided[param] -= count
+        return values[-count:]
+
     def record_action(self, param: ParamOrGroup, val_count: int = 1):
         """
         Not intended to be called by users.  Used by Parameters during parsing to indicate that they were provided.
         """
         self._provided[param] += val_count
 
     def num_provided(self, param: ParamOrGroup) -> int:
         """Not intended to be called by users.  Used by Parameters during parsing to handle nargs."""
         return self._provided[param]
 
     def get_missing(self) -> List[Parameter]:
-        return [p for p in self.params.required_check_params() if self._provided[p] == 0]
+        """Not intended to be called by users.  Used during parsing to determine if any Parameters are missing."""
+        return [p for p in self.params.required_check_params() if not self._provided[p]]
+
+    def missing_options_with_env_var(self) -> Iterator[Option]:
+        """Yields Option parameters that have an environment variable configured, and did not have any CLI values."""
+        yield from (p for p in self.params.options if p.env_var and not self._provided[p])
 
     # endregion
 
     # region Actions
 
     @cached_property
     def _parsed_action_flags(self) -> Tuple[int, List[ActionFlag], List[ActionFlag]]:
@@ -226,36 +240,36 @@
         """
         try:
             before_main, after_main = self.params.split_action_flags  # Each part is already sorted
         except AttributeError:  # self.command is None
             return 0, [], []
 
         parsed = self._parsed
-        before_main = [p for p in before_main if p in parsed]
-        after_main = [p for p in after_main if p in parsed]
+        before_main = [p for p in before_main if p in parsed] if before_main else []
+        after_main = [p for p in after_main if p in parsed] if after_main else []
         return len(before_main) + len(after_main), before_main, after_main
 
     @property
     def action_flag_count(self) -> int:
         """Not intended to be accessed by users.  Returns the count of parsed action flags."""
         return self._parsed_action_flags[0]
 
     @cached_property
     def all_action_flags(self) -> List[ActionFlag]:
         """Not intended to be accessed by users.  Returns all parsed action flags."""
-        before_main, after_main = self._parsed_action_flags[1:]
+        _, before_main, after_main = self._parsed_action_flags
         return before_main + after_main
 
     @cached_property
     def categorized_action_flags(self) -> Dict[ActionPhase, Sequence[ActionFlag]]:
         """
         Not intended to be accessed by users.  Returns a dict of parsed action flags, categorized by the
         :class:`ActionPhase` during which they will run.
         """
-        before_main, after_main = self._parsed_action_flags[1:]
+        _, before_main, after_main = self._parsed_action_flags
         init_actions, before_actions = [], []
         for flag in before_main:
             if flag.always_available:
                 init_actions.append(flag)
             else:
                 before_actions.append(flag)
 
@@ -313,46 +327,74 @@
     Proxy for the currently active :class:`Context` object.  Allows usage similar to the ``request`` object in Flask.
 
     This class should not be instantiated by users - use the common :data:`ctx` instance.
     """
 
     __slots__ = ()
 
+    # region Generic Proxy Methods
+
     def __getattr__(self, attr: str):
         return getattr(get_current_context(), attr)
 
     def __setattr__(self, attr: str, value):
         return setattr(get_current_context(), attr, value)
 
     def __eq__(self, other) -> bool:
         return get_current_context() == other
 
     def __contains__(self, item) -> bool:
         return item in get_current_context()
 
     def __enter__(self) -> Context:
-        return get_current_context().__enter__()
+        # The current context is already active, so there's no need to re-enter it - it can just be returned
+        return get_current_context()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        return get_current_context().__exit__(exc_type, exc_val, exc_tb)
+        pass
+
+    # endregion
+
+    # region Proxied Parsing Methods
+
+    def has_parsed_value(self, param: Parameter) -> bool:
+        return get_current_context().has_parsed_value(param)
+
+    def get_parsed_value(self, param: Parameter):
+        return get_current_context().get_parsed_value(param)
+
+    def set_parsed_value(self, param: Parameter, value: Any):
+        get_current_context().set_parsed_value(param, value)
+
+    def record_action(self, param: ParamOrGroup, val_count: int = 1):
+        get_current_context().record_action(param, val_count)
+
+    def num_provided(self, param: ParamOrGroup) -> int:
+        return get_current_context().num_provided(param)
+
+    # endregion
+
+    # region Properties with Inactive Handlers
 
     @property
     def terminal_width(self) -> int:
-        try:
-            return get_current_context().terminal_width
-        except NoActiveContext:
+        if context := get_current_context(True):
+            return context.terminal_width
+        else:
             return _TERMINAL.width
 
     @property
     def config(self) -> CommandConfig:
-        try:
-            return get_current_context().config
-        except NoActiveContext:
+        if context := get_current_context(True):
+            return context.config
+        else:
             return DEFAULT_CONFIG
 
+    # endregion
+
 
 ctx: Context = cast(Context, ContextProxy())
 
 
 # region Public / Semi-Public Functions
 
 
@@ -362,48 +404,45 @@
 
     :param silent: If True, allow this function to return ``None`` if there is no active :class:`Context`
     :return: The active :class:`Context` object
     :raises: :class:`~.exceptions.NoActiveContext` if there is no active Context and ``silent=False`` (default)
     """
     try:
         return _context_stack.get()[-1]
-    except (AttributeError, IndexError):
+    except (LookupError, IndexError):
         if silent:
             return None
         raise NoActiveContext('There is no active context') from None
 
 
 def get_or_create_context(command_cls: CommandType, argv: Sequence[str] = None, **kwargs) -> Context:
     """
     Used internally by Commands to re-use an existing user-activated Context, or to create a new Context if there was
     no active Context.
     """
-    try:
-        context = get_current_context()
-    except NoActiveContext:
+    if not (context := get_current_context(True)):
         return Context(argv, command_cls, **kwargs)
+    elif argv is None and context.command is command_cls and not kwargs:
+        return context
     else:
-        if argv is None and context.command is command_cls and not kwargs:
-            return context
-        else:
-            return context._sub_context(command_cls, argv=argv, **kwargs)
+        return context._sub_context(command_cls, argv=argv, **kwargs)
 
 
 def get_context(command: Command) -> Context:
     """
     :param command: An initialized Command object
     :return: The Context associated with the given Command
     """
     try:
         return command._Command__ctx  # noqa
     except AttributeError as e:
         raise TypeError('get_context only supports Command objects') from e
 
 
-def get_parsed(command: Command, to_call: Callable = None) -> Dict[str, Any]:
+def get_parsed(command: Command, to_call: Callable = None, default: Any = None) -> Dict[str, Any]:
     """
     Provides a way to obtain all of the arguments that were parsed for the given Command as a dictionary.
 
     If the parsed arguments are intended to be used to call a particular function/method, or to initialize a particular
     class, then that callable can be provided as the ``to_call`` parameter to filter the parsed arguments to only the
     ones that would be accepted by it.  It will not be called by this function.
 
@@ -414,18 +453,20 @@
     :attr:`POSITIONAL_ONLY or VAR_POSITIONAL <python:inspect.Parameter.kind>`), then they must be handled after calling
     this function.  They will be included in the returned dict.
 
     :param command: An initialized Command object for which arguments were already parsed.
     :param to_call: A :class:`callable <python:collections.abc.Callable>` (function, method, class, etc.) that should
       be used to filter the parsed arguments.  If provided, then only the keys that match the callable's signature will
       be included in the returned dictionary of parsed arguments.
+    :param default: The default value to use for parameters that raise :class:`.MissingArgument` when attempting to
+      obtain their result values.
     :return: A dictionary containing all of the (optionally filtered) arguments that were parsed.  The keys in the
       returned dict match the names assigned to the Parameters in the given Command.
     """
-    parsed = get_context(command).get_parsed()
+    parsed = get_context(command).get_parsed(default=default)
     if to_call is not None:
         sig = Signature.from_callable(to_call)
         keys = {k for k, p in sig.parameters.items() if p.kind != _Parameter.VAR_KEYWORD}
         parsed = {k: v for k, v in parsed.items() if k in keys}
 
     return parsed
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/command_builder.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/visitor.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/documentation.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/documentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 import logging
 import sys
+from abc import ABC
 from collections import defaultdict
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, Mapping, List, Dict
+from typing import TYPE_CHECKING, Iterable, Mapping, Any, List, Dict
 
 from .commands import Command
 from .context import Context
 from .core import CommandMeta, get_params, get_parent, get_metadata
 from .formatting.commands import get_formatter, NameFunc
 from .formatting.restructured_text import MODULE_TEMPLATE, rst_header, rst_toc_tree
 
@@ -44,15 +45,15 @@
     :param command: The :class:`.Command` to document
     :param fix_name: Whether the file name should be re-formatted from CamelCase / snake_case to separate Title Case
       words or not (default: True)
     :param fix_name_func: The function to call if ``fix_name`` is True instead of the default one.
     :return: The help text for the given Command, formatted using RST
     """
     with Context([], command, allow_argv_prog=False):
-        return get_formatter(command).format_rst(fix_name, fix_name_func, no_sys_argv=True)
+        return get_formatter(command).format_rst(fix_name, fix_name_func)
 
 
 def _render_commands_rst(commands: Commands, fix_name: Bool = True, fix_name_func: NameFunc = None) -> str:
     # This could be better, but it's relatively unlikely to have multiple top level commands in a script...
     # For the same reason that main() does not try to pick one, this will just combine all of them.
     parts = []
     for i, (_name, command) in enumerate(sorted(commands.items())):
@@ -68,39 +69,47 @@
 
 # endregion
 
 
 # region Import and Load Commands
 
 
-def load_commands(path: PathLike, top_only: Bool = False) -> Commands:
+def load_commands(path: PathLike, top_only: Bool = False, include_abc: Bool = False) -> Commands:
     """
     Load all of the commands from the file with the given path and return them as a dict of ``{name: Command}``.
 
     If an :class:`python:OSError` or a subclass thereof is encountered while attempting to load the file (due to the
     path not existing, or a permission error, etc), it will be allowed to propagate.  An :class:`python:ImportError`
     may be raised by :func:`import_module` if the specified path cannot be imported.
 
     :param path: The path to a file containing one or more :class:`.Command` classes
     :param top_only: If True, then only top-level commands are returned (default: all)
+    :param include_abc: Whether Command classes that extend :class:`python:abc.ABC` should be included in results.
     :return: Dict containing the Commands loaded from the given file
     """
     with Context(allow_argv_prog=False):
         module = import_module(path)
-    commands = {key: val for key, val in module.__dict__.items() if not key.startswith('__') and _is_command(val)}
-    if top_only:
-        commands = top_level_commands(commands)
+
+    commands = filtered_commands(module.__dict__, top_only, include_abc)
 
     if doc_str := module.__doc__:
         for command in commands.values():
             get_metadata(command).pkg_doc_str = doc_str
 
     return commands
 
 
+def filtered_commands(obj_map: Dict[str, Any], top_only: Bool = False, include_abc: Bool = False) -> Commands:
+    commands = {key: val for key, val in obj_map.items() if not key.startswith('__') and _is_command(val, include_abc)}
+    if top_only:
+        commands = top_level_commands(commands)
+
+    return commands
+
+
 def top_level_commands(commands: Commands) -> Commands:
     """Filter the given commands to only the ones that do not have a parent present in the provided dict of commands"""
     if len(commands) <= 1:
         return commands
 
     indirect_parents = defaultdict(set)
     for name, command in commands.items():
@@ -136,16 +145,19 @@
         spec.loader.exec_module(module)
     except Exception:
         del sys.modules[spec.name]
         raise
     return module
 
 
-def _is_command(obj) -> bool:
-    return isinstance(obj, CommandMeta) and obj is not Command
+def _is_command(obj, include_abc: Bool = False) -> bool:
+    if not (isinstance(obj, CommandMeta) and obj is not Command):
+        return False
+    else:
+        return True if include_abc else ABC not in obj.__bases__
 
 
 # endregion
 
 
 class RstWriter:
     """
@@ -279,14 +291,15 @@
         """
         if name:
             index_subdir = content_subdir = f'{subdir}/{name}' if subdir else name
         else:
             index_subdir = None
             content_subdir = subdir
 
+        # TODO: This needs improvement for multi-package repos
         contents = self._generate_code_rsts(pkg_name, pkg_path, content_subdir, max_depth=max_depth)
         if (not contents and not empty) or not index:
             return contents
 
         if not header:
             header = f'{pkg_name.split(".")[-1].title()} Package'
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/error_handling.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     'MultiParamUsageError',
     'AmbiguousCombo',
     'ParamConflict',
     'ParamsMissing',
     'BadArgument',
     'InvalidChoice',
     'MissingArgument',
+    'TooManyArguments',
     'NoSuchOption',
     'NoActiveContext',
 ]
 
 
 class CommandParserException(Exception):
     """Base class for all other Command Parser exceptions"""
@@ -221,31 +222,35 @@
 
 class MissingArgument(BadArgument):
     """Error raised when a value for a Parameter was not provided"""
 
     message = 'missing required argument value'
 
 
+class TooManyArguments(BadArgument):
+    """Error raised when too many values were provided for a Parameter"""
+
+    def __init__(self, param: ParamOrGroup, message: str = None):
+        msg = f'expected {param.nargs} args - cannot accept any additional args'
+        super().__init__(param, f'{msg} - {message}' if message else msg)
+
+
 class NoSuchOption(UsageError):
     """Error raised when an option that was not defined as a Parameter was provided"""
 
 
 class NoActiveContext(CommandParserException, RuntimeError):
     """Raised when attempting to perform an action that requires an active context while no context is active."""
 
 
 # endregion
 
 # region Internal Exceptions
 
 
-class UnsupportedAction(CommandParserException):
-    """Indicates that an attempted action cannot be completed.  Only used internally."""
-
-
 class Backtrack(CommandParserException):
     """Raised when backtracking took place.  Only used internally."""
 
 
 class NextCommand(CommandParserException):
     """Raised by the parser to advance to the next Command in certain cases.  Only used internally."""
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,31 @@
 Command usage / help text formatters
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Type, Callable, Iterator, Iterable, Optional
+from functools import cached_property
+from textwrap import TextWrapper
+from typing import TYPE_CHECKING, Union, Type, Callable, Iterator, Iterable, Optional
 
 from ..context import ctx, NoActiveContext
 from ..core import get_params, get_metadata
 from ..parameters.groups import ParamGroup
-from ..utils import camel_to_snake_case
-from .restructured_text import rst_header, RstTable
+from ..utils import camel_to_snake_case, _NotSet
+from .restructured_text import RstTable, spaced_rst_header
+from .utils import combine_and_wrap
 
 if TYPE_CHECKING:
     from ..core import CommandMeta
     from ..command_parameters import CommandParameters
-    from ..parameters import Parameter, BasePositional, BaseOption, SubCommand
+    from ..config import CommandConfig
+    from ..metadata import ProgramMetadata
+    from ..parameters import Parameter, BasePositional, BaseOption, SubCommand, PassThru
     from ..typing import Bool, CommandType, CommandCls, CommandAny
 
 __all__ = ['CommandHelpFormatter', 'get_formatter']
 
 NameFunc = Callable[[str], str]
 
 
@@ -29,14 +34,18 @@
     def __init__(self, command: CommandType, params: CommandParameters):
         self.command = command
         self.params = params
         self.pos_group = ParamGroup(description='Positional arguments')
         self.opt_group = ParamGroup(description='Optional arguments')
         self.groups = [self.pos_group, self.opt_group]
 
+    @cached_property
+    def _meta(self) -> ProgramMetadata:
+        return get_metadata(self.command)
+
     def maybe_add_groups(self, groups: Iterable[ParamGroup]):
         for group in groups:
             if group.group:  # prevent duplicates
                 continue
             if group.contains_positional:
                 self.pos_group.add(group)
             else:
@@ -46,137 +55,186 @@
         if param is not None and not param.group:
             self.opt_group.add(param)
 
     def maybe_add_positionals(self, params: Iterable[BasePositional]):
         self.pos_group.extend(param for param in params if not param.group)
 
     def maybe_add_options(self, params: Iterable[BaseOption]):
+        # TODO: It would be good for required options' default group to indicate they are required, instead of the
+        #  default group saying "Optional"
         self.opt_group.extend(param for param in params if not param.group)
 
-    def format_usage(self, delim: str = ' ', sub_cmd_choice: str = None) -> str:
-        meta = get_metadata(self.command)
-        if meta.usage:
-            return meta.usage
-
-        params = self.params.all_positionals + self.params.options  # noqa
-        if (pass_thru := self.params.pass_thru) is not None:
-            params.append(pass_thru)
-
-        parts = ['usage:', meta.prog]
+    def _iter_params(self) -> Iterator[Union[BasePositional, BaseOption, PassThru]]:
+        params = self.params
+        yield from params.all_positionals
+        yield from params.options
+        if (pass_thru := params.pass_thru) is not None:
+            yield pass_thru
+
+    def _usage_parts(self, sub_cmd_choice: str = None, allow_sys_argv: Bool = True) -> Iterator[str]:
+        yield 'usage:'
+        yield self._meta.get_prog(allow_sys_argv)
         if sub_cmd_choice:
-            parts.append(sub_cmd_choice)
+            yield sub_cmd_choice
         else:
-            parts.extend(get_usage_sub_cmds(self.command))
+            yield from get_usage_sub_cmds(self.command)
+
+        yield from (param.formatter.format_basic_usage() for param in self._iter_params() if param.show_in_help)
+
+    def format_usage(
+        self,
+        delim: str = ' ',
+        sub_cmd_choice: str = None,
+        allow_sys_argv: Bool = True,
+        cont_indent: int = 4,
+    ) -> str:
+        if (wrap_usage_str := ctx.config.wrap_usage_str) is True:
+            wrap_usage_str = ctx.terminal_width
 
-        parts.extend(param.formatter.format_basic_usage() for param in params if param.show_in_help)
+        if usage := self._meta.usage:
+            if wrap_usage_str:
+                return '\n'.join(TextWrapper(width=wrap_usage_str, subsequent_indent=' ' * cont_indent).wrap(usage))
+            return usage
+
+        parts = self._usage_parts(sub_cmd_choice, allow_sys_argv)
+        if wrap_usage_str:
+            return '\n'.join(combine_and_wrap(parts, wrap_usage_str, cont_indent, delim))
         return delim.join(parts)
 
-    def format_help(self) -> str:
-        meta = get_metadata(self.command)
-        parts = [self.format_usage(), '']
-        if meta.description:
-            parts += [meta.description, '']
+    def format_help(self, allow_sys_argv: Bool = True) -> str:
+        parts = [self.format_usage(allow_sys_argv=allow_sys_argv), '']
+        if description := self._meta.description:
+            parts += [description, '']
 
         for group in self.groups:
             if group.show_in_help:
                 parts.append(group.formatter.format_help())
 
-        if epilog := meta.format_epilog(ctx.config.extended_epilog):
+        if epilog := self._meta.format_epilog(ctx.config.extended_epilog, allow_sys_argv):
             parts.append(epilog)
 
         return '\n'.join(parts)
 
+    # region RST Formatting
+
+    def format_rst(
+        self, fix_name: Bool = True, fix_name_func: NameFunc = None, init_level: int = 1, allow_sys_argv: Bool = False
+    ) -> str:
+        """Generate the RST content for the Command associated with this formatter and all of its subcommands"""
+        return '\n'.join(self._format_rst(fix_name, fix_name_func, init_level, allow_sys_argv))
+
     def _format_rst(
-        self, include_epilog: Bool = False, sub_cmd_choice: str = None, no_sys_argv: Bool = False
+        self, fix_name: Bool = True, fix_name_func: NameFunc = None, init_level: int = 1, allow_sys_argv: Bool = False
+    ) -> Iterator[str]:
+        name = self._meta.doc_name
+        if fix_name:
+            name = fix_name_func(name) if fix_name_func else _fix_name(name)  # noqa
+
+        yield from spaced_rst_header(name, init_level, False)
+
+        config = ctx.config
+        if config.show_docstring and (doc_str := self._meta.get_doc_str()):
+            yield doc_str
+            yield ''
+
+        yield ''
+        yield from self._cmd_rst_lines(config, allow_sys_argv=allow_sys_argv, include_epilog=True)
+        if sub_command := self.params.sub_command:
+            yield from self._sub_cmds_rst_lines(config, sub_command, init_level + 2, allow_sys_argv=allow_sys_argv)
+
+    def _cmd_rst_lines(
+        self,
+        config: CommandConfig,
+        sub_cmd_choice: str = None,
+        allow_sys_argv: Bool = False,
+        include_epilog: Bool = False,
     ) -> Iterator[str]:
         """Generate the RST content for the specific Command associated with this formatter"""
-        meta = get_metadata(self.command, no_sys_argv=no_sys_argv)
-        # TODO: Line wrap usage text?
-        yield from ('::', '', '    ' + self.format_usage(sub_cmd_choice=sub_cmd_choice), '', '')
-        if meta.description:
-            yield meta.description
+        yield '::'
+        yield ''
+        yield '    ' + self.format_usage(sub_cmd_choice=sub_cmd_choice, allow_sys_argv=allow_sys_argv, cont_indent=8)
+        yield ''
+        yield ''
+
+        if description := self._meta.get_description(config.show_inherited_descriptions):
+            yield description
             yield ''
 
         # TODO: The subcommand names in the group containing subcommand targets should link to their respective
         #  subcommand sections
         for group in self.groups:
+            # TODO: Nested subcommands' local choices should not repeat the `subcommands` positional arguments section
+            #  that includes the nested subcommand choice being documented
             if group.show_in_help:
                 table: RstTable = group.formatter.rst_table()  # noqa
-                yield from table.iter_build()  # noqa
+                yield from table.iter_build()
 
-        if include_epilog and (epilog := meta.format_epilog(ctx.config.extended_epilog)):
+        if include_epilog and (epilog := self._meta.format_epilog(config.extended_epilog, allow_sys_argv)):
             yield epilog
 
-    def format_rst(
-        self, fix_name: Bool = True, fix_name_func: NameFunc = None, init_level: int = 1, no_sys_argv: Bool = False
-    ) -> str:
-        """Generate the RST content for the Command associated with this formatter and all of its subcommands"""
-        # TODO: Nested subcommands do not have full sections, but they should
-        meta = get_metadata(self.command, no_sys_argv=no_sys_argv)
-        name = meta.doc_name
-        # TODO: Usage name for subcommands seems to always be ``build_docs.py``
-        if fix_name:
-            name = fix_name_func(name) if fix_name_func else _fix_name(name)
-
-        # TODO: Use class docstring as description if no description is provided?
-
-        parts = [rst_header(name, init_level), '']
-        if ctx.config.show_docstring and (doc_str := meta.get_doc_str()):
-            parts += [doc_str, '']
-
-        parts.append('')
-        parts.extend(self._format_rst(True, no_sys_argv=no_sys_argv))
-
-        if (sub_command := get_params(self.command).sub_command) and sub_command.show_in_help:
-            parts += ['', rst_header('Subcommands', init_level + 1), '']
-            for cmd_name, choice in sub_command.choices.items():
-                # TODO: Config to disable inherited docstring/description from being printed for each subcommand
-                parts += ['', rst_header(f'Subcommand: {cmd_name}', init_level + 2), '']
-                if choice.help:
-                    parts += [choice.help, '']
-
-                try:
-                    formatter = get_formatter(choice.target)
-                except TypeError:  # choice.target is None (it is the default choice, pointing back to the same Command)
-                    formatter = self
-
-                parts.extend(formatter._format_rst(sub_cmd_choice=cmd_name, no_sys_argv=no_sys_argv))
+    def _sub_cmds_rst_lines(
+        self,
+        config: CommandConfig,
+        sub_command: SubCommand,
+        level: int,
+        choice_base: str = None,
+        depth: int = 0,
+        allow_sys_argv: Bool = False,
+    ):
+        if not sub_command.show_in_help or ((max_depth := config.sub_cmd_doc_depth) is not None and depth == max_depth):
+            return
+        elif depth == 0:
+            yield from spaced_rst_header('Subcommands', level - 1)
+
+        for cmd_name, choice in sub_command.choices.items():
+            # TODO: There are some cases where multiple aliases for the same command (possibly local choices, possibly
+            #  multiple choices all handled by a single class) would be better documented without separate sections for
+            #  each choice value (should probably be configurable to explode or condense)
+            choice_str = f'{choice_base} {cmd_name}' if choice_base else cmd_name
+            yield from spaced_rst_header(f'Subcommand: {choice_str}', level)
+            if choice_help := choice.help:
+                yield choice_help
+                yield ''
+
+            if (command := choice.target) is None:
+                # When choice.target is None, that means it is the default choice, pointing back to the same Command
+                yield from self._cmd_rst_lines(config, choice_str, allow_sys_argv)
+            else:
+                params = get_params(command)
+                formatter = params.formatter
+                yield from formatter._cmd_rst_lines(config, choice_str, allow_sys_argv)
+                if nested_sub_cmd := params.sub_command:
+                    yield from formatter._sub_cmds_rst_lines(
+                        config, nested_sub_cmd, level, choice_str, depth + 1, allow_sys_argv
+                    )
 
-        return '\n'.join(parts)
+    # endregion
 
 
 def _fix_name(name: str) -> str:
     return camel_to_snake_case(name).replace('_', ' ').title()
 
 
 def get_formatter(command: CommandAny) -> CommandHelpFormatter:
     """Get the :class:`CommandHelpFormatter` for the given Command"""
     return get_params(command).formatter
 
 
 def get_usage_sub_cmds(command: CommandCls):
     cmd_mcs: Type[CommandMeta] = command.__class__  # Using metaclass to avoid potentially overwritten attrs
-    parent: CommandType = cmd_mcs.parent(command, False)
-    if not parent:
-        return []
-
-    cmd_chain = get_usage_sub_cmds(parent)
-
-    sub_cmd_param: SubCommand = cmd_mcs.params(parent).sub_command
-    if not sub_cmd_param:
-        return cmd_chain
+    if not (parent := cmd_mcs.parent(command, False)):  # type: CommandType
+        return
+
+    yield from get_usage_sub_cmds(parent)
+
+    if not (sub_cmd_param := cmd_mcs.params(parent).sub_command):  # type: SubCommand
+        return
 
     try:
         parsed = ctx.get_parsed_value(sub_cmd_param)
     except NoActiveContext:
         parsed = []
 
-    if parsed:  # May have been called directly on the subcommand without parsing
-        cmd_chain.extend(parsed)
-        return cmd_chain
-
-    for name, choice in sub_cmd_param.choices.items():
-        if choice.target is command:
-            cmd_chain.append(name)
-            break
-
-    return cmd_chain
+    if parsed and parsed is not _NotSet:  # May have been called directly on the subcommand without parsing
+        yield from parsed
+    elif chosen := next((name for name, choice in sub_cmd_param.choices.items() if choice.target is command), None):
+        yield chosen
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from ..parameters.base import BasePositional, BaseOption
 from ..parameters.choice_map import ChoiceMap, Choice
 from ..parameters import ParamGroup, PassThru, TriFlag
 from .restructured_text import RstTable
 from .utils import format_help_entry, _should_add_default
 
 if TYPE_CHECKING:
+    from ..nargs import Nargs
     from ..parameters.option_strings import TriFlagOptionStrings
     from ..typing import Bool, ParamOrGroup, OptStr
 
 BoolFormatterMap = Dict[bool, Callable[[str], str]]
 
 
 class ParamHelpFormatter:
@@ -64,27 +65,28 @@
         try:
             return self.required_formatter_map[self.param.required](text)
         except KeyError:
             return text
 
     def format_metavar(self) -> str:
         param = self.param
-        if param.metavar:
+        if param.metavar and param.action.accepts_values:
             return param.metavar
+
+        config = ctx.config
         if (t := param.type) is not None:
             try:
-                config = ctx.config
                 metavar = t.format_metavar(config.choice_delim, config.sort_choices)
             except Exception:  # noqa  # pylint: disable=W0703
                 pass
             else:
                 if metavar is not NotImplemented:
                     return metavar
 
-        if ctx.config.use_type_metavar and t is not None:
+        if config.use_type_metavar and t is not None:
             try:
                 name = t.__name__
             except AttributeError:
                 pass
             else:
                 if name != '<lambda>':
                     return name.upper()
@@ -139,16 +141,20 @@
         metavar = self.format_metavar()
         return metavar if not full or self.param.nargs == 1 else f'{metavar} [{metavar} ...]'
 
 
 class OptionHelpFormatter(ParamHelpFormatter, param_cls=BaseOption):
     def _format_usage_metavar(self) -> str:
         metavar = self.format_metavar()
-        if 0 in self.param.nargs:
-            metavar = f'[{metavar}]'
+        nargs: Nargs = self.param.nargs
+        variable = nargs.variable and nargs.max != 1
+        if 0 in nargs:
+            return f'[{metavar} ...]' if variable else f'[{metavar}]'
+        elif variable:
+            return f'{metavar} [{metavar} ...]'
         return metavar
 
     def iter_usage_parts(self, include_meta: Bool = False, full: Bool = False) -> Iterator[str]:
         param: BaseOption = self.param
         opts = param.option_strs
         if param.nargs == 0:
             yield from opts.option_strs()
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,21 @@
 
 
 def rst_header(text: str, level: int = 1, overline: Bool = False) -> str:
     bar = rst_bar(text, level)
     return f'{bar}\n{text}\n{bar}' if overline else f'{text}\n{bar}'
 
 
+def spaced_rst_header(text: str, level: int = 1, before: bool = True) -> Iterator[str]:
+    if before:
+        yield ''
+    yield f'{text}\n{rst_bar(text, level)}'
+    yield ''
+
+
 def _rst_directive(
     directive: str, args: str = None, options: Dict[str, Any] = None, indent: int = 4, check: Bool = False
 ) -> Iterator[str]:
     yield f'.. {directive}:: {args}' if args else f'.. {directive}::'
     if options:
         pre = ' ' * indent
         for key, val in options.items():
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """Combine the given strings using the given delimiter, wrapping to a new line at max_width."""
     delim_end = delim.rstrip()
     delim_len = len(delim)
     line_len = delim_end_len = len(delim_end)
     line_parts = []
     last = None
     for part in parts:
-        part_len = len(part)
+        part_len = wcswidth(part)
         line_len += part_len + delim_len
         if line_len >= max_width:
             if last:
                 yield last + delim_end
                 prefix = ' ' * cont_indent
             else:
                 prefix = ''
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,45 +12,54 @@
 from ..exceptions import ParameterDefinitionError as _ParameterDefinitionError
 from .exceptions import InputValidationError, InvalidChoiceError
 from .utils import StatMode, FileWrapper
 from .base import InputType
 from .choices import Choices, ChoiceMap, EnumChoices
 from .files import Path, File, Serialized, Json, Pickle
 from .numeric import Range, NumRange
+from .patterns import Regex, RegexMode, Glob
 from .time import Day, Month, TimeDelta, DateTime, Date, Time, DTFormatMode
 
 if _t.TYPE_CHECKING:
     from ..typing import TypeFunc, InputTypeFunc, ChoicesType
 
 # fmt: off
 __all__ = [
     'StatMode', 'FileWrapper', 'Path', 'File', 'Serialized', 'Json', 'Pickle',
     'Range', 'NumRange',
     'Choices', 'ChoiceMap', 'EnumChoices',
+    'Regex', 'RegexMode', 'Glob',
     'Day', 'Month', 'TimeDelta', 'DateTime', 'Date', 'Time', 'DTFormatMode',
     'normalize_input_type',
 ]
 # fmt: on
 
+_INVALID_CHOICES_TYPES = (_t.Pattern, InputType)
+_INVALID_TYPES_WITH_CHOICES = (Range, range, Regex, _t.Pattern, Glob)
+
 
 def normalize_input_type(type_func: InputTypeFunc, param_choices: ChoicesType) -> _t.Optional[TypeFunc]:
     if choices_provided := param_choices is not None:
         if not param_choices:
             raise _ParameterDefinitionError(
                 f'Invalid choices={param_choices!r} - when specified, choices cannot be empty'
             )
         elif isinstance(param_choices, range):
             return Range(param_choices, type_func)
-        elif isinstance(type_func, (Range, range)):
-            raise ValueError(f'Cannot combine type={type_func!r} with choices={param_choices!r}')
+        elif isinstance(param_choices, _INVALID_CHOICES_TYPES):
+            raise _ParameterDefinitionError(f'Invalid choices={param_choices!r} - use type={param_choices!r} instead')
+        elif isinstance(type_func, _INVALID_TYPES_WITH_CHOICES):
+            raise _ParameterDefinitionError(f'Cannot combine type={type_func!r} with choices={param_choices!r}')
 
     if type_func is None:
         return Choices(param_choices) if choices_provided else type_func
     elif isinstance(type_func, range):
         return Range(type_func)
+    elif isinstance(type_func, _t.Pattern):
+        return Regex(type_func)
 
     try:
         is_enum = issubclass(type_func, _Enum)
     except TypeError:
         pass
     else:
         if is_enum:
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 
 :author: Doug Skrypa
 """
 
 from abc import ABC, abstractmethod
 from typing import Any, Generic, Optional
 
-from ..typing import T
+from ..typing import T, Bool
 
 __all__ = ['InputType']
 
 
 class InputType(Generic[T], ABC):
-    __slots__ = ()
+    __slots__ = ('_fix_default',)
+
+    def __init__(self, fix_default: Bool = True):
+        self._fix_default = fix_default
 
     @abstractmethod
     def __call__(self, value: str) -> T:
         """Process the parsed argument and convert it to the desired type"""
         raise NotImplementedError
 
     def is_valid_type(self, value: str) -> bool:  # pylint: disable=W0613
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/choices.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,20 @@
 if TYPE_CHECKING:
     from ..typing import Bool
 
 __all__ = ['Choices', 'ChoiceMap', 'EnumChoices']
 
 EnumT = TypeVar('EnumT', bound=Enum)
 
-# TODO: Add support for input validation based on regex or fnmatch pattern
-
 
 class _ChoicesBase(InputType[T], ABC):
+    __slots__ = ('choices', 'type', 'case_sensitive')
     choices: Collection[T]
-    type: Optional[TypeFunc] = None
-    case_sensitive: bool = True
+    type: Optional[TypeFunc]
+    case_sensitive: bool
 
     def __contains__(self, value: str) -> bool:
         try:
             self(value)
         except InvalidChoiceError:
             return False
         return True
@@ -84,20 +83,22 @@
     :param choices: A collection of choices allowed for a given Parameter.
     :param type: Called before evaluating whether a value matches one of the allowed choices, if provided.  Must accept
       a single string argument.
     :param case_sensitive: Whether choices should be case-sensitive.  Defaults to True.  If the choices values are not
       all strings, then this cannot be set to False.
     """
 
+    __slots__ = ()
+
     def __init__(self, choices: Collection[T], type: TypeFunc = None, case_sensitive: Bool = True):  # noqa
         if not case_sensitive and not all(isinstance(c, str) for c in choices):
             raise TypeError(f'Cannot combine case_sensitive=False with non-str {choices=}')
-        elif isinstance(type, EnumChoices) and not any(isinstance(c, type.enum) for c in choices):
+        elif isinstance(type, EnumChoices) and not any(isinstance(c, type.type) for c in choices):
             raise TypeError(f'Invalid {choices=} for {type=}')
-
+        super().__init__()  # fix_default is not implemented here, so it's not necessary to expose
         self.choices = choices
         self.type = type
         self.case_sensitive = case_sensitive
 
     def _choices_repr(self, delim: str = ',') -> str:
         return delim.join(map(repr, sorted(self.choices)))
 
@@ -125,14 +126,15 @@
       provided as an argument, and the value is what should be stored in the Parameter for that argument.
     :param type: Called before evaluating whether a value matches one of the allowed choices, if provided.  Must accept
       a single string argument.
     :param case_sensitive: Whether choices should be case-sensitive.  Defaults to True.  If the choices keys are not
       all strings, then this cannot be set to False.
     """
 
+    __slots__ = ()
     choices: Mapping[Any, T]
 
     def __init__(self, choices: Mapping[Any, T], *args, **kwargs):
         super().__init__(choices, *args, **kwargs)
 
     def __call__(self, value: str) -> T:
         value = self._normalize(value)
@@ -149,29 +151,31 @@
     """
     Similar to :class:`ChoiceMap`, but uses an Enum to validate / normalize input instead of the keys in a dict.
 
     :param enum: A subclass of :class:`python:enum.Enum`.
     :param case_sensitive: Whether choices should be case-sensitive.  Defaults to False.
     """
 
-    enum: Type[EnumT]
+    __slots__ = ()
+    type: Type[EnumT]
 
     def __init__(self, enum: Type[EnumT], case_sensitive: Bool = False):
-        self.enum = enum
+        super().__init__()  # fix_default is not implemented here, so it's not necessary to expose
+        self.type = enum
         self.case_sensitive = case_sensitive
         self.choices = enum._member_map_
 
     def _type_str(self) -> str:
-        return f'type={self.enum.__name__}, '
+        return f'type={self.type.__name__}, '
 
     def _choices_repr(self, delim: str = ',') -> str:
-        return delim.join(self.enum._member_map_)
+        return delim.join(self.type._member_map_)
 
     def __call__(self, value: str) -> EnumT:
-        enum = self.enum
+        enum = self.type
         for val in self._iter_normalized(value):
             try:
                 return enum[val]
             except KeyError:
                 pass
             try:
                 return enum(val)
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/files.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import os
 from abc import ABC
 from pathlib import Path as _Path
 from typing import Union, Optional
 
 from ..typing import Bool, T, PathLike, Converter
 from .base import InputType
+from .exceptions import InputValidationError
 from .utils import InputParam, StatMode, FileWrapper, allows_write, fix_windows_path
 
 __all__ = ['Path', 'File', 'Serialized', 'Json', 'Pickle']
 
 
 class FileInput(InputType[T], ABC):
     exists: bool = InputParam(None)
@@ -35,15 +36,17 @@
         expand: Bool = True,
         resolve: Bool = False,
         type: Union[StatMode, str] = StatMode.ANY,  # noqa
         readable: Bool = False,
         writable: Bool = False,
         allow_dash: Bool = False,
         use_windows_fix: Bool = True,
+        fix_default: Bool = True,
     ):
+        super().__init__(fix_default)
         self.exists = exists
         self.expand = expand
         self.resolve = resolve
         self.type = StatMode(type)  # pylint: disable=E1120
         self.readable = readable
         self.writable = writable
         self.allow_dash = allow_dash
@@ -54,65 +57,66 @@
         return f'<{self.__class__.__name__}({non_defaults})>'
 
     def fix_default(self, value: Optional[T]) -> Optional[T]:
         """
         Fixes the default value to conform to the expected return type for this input.  Allows the default value for a
         path to be provided as a string, for example.
         """
-        if value is None:
+        if value is None or not self._fix_default:
             return value
         return self(value)
 
     def validated_path(self, path: PathLike) -> _Path:
         if not isinstance(path, _Path):
-            path = path.strip()
-            if not path:
-                raise ValueError('A valid path is required')
+            if not (path := path.strip()):
+                raise InputValidationError('A valid path is required')
             path = _Path(path)
         if path.parts == ('-',):
             if not self.allow_dash:
-                raise ValueError('Dash (-) is not supported for this parameter')
+                raise InputValidationError('Dash (-) is not supported for this parameter')
             return path
         if self.use_windows_fix and os.name == 'nt':
             try:
                 path = fix_windows_path(path)
             except OSError:
                 pass
         if self.expand:
             path = path.expanduser()
         if self.resolve:
             path = path.resolve()
         if self.exists is not None:
             if self.exists and not path.exists():
-                raise ValueError('it does not exist')
+                raise InputValidationError('it does not exist')
             elif not self.exists and path.exists():
-                raise ValueError('it already exists')
+                raise InputValidationError('it already exists')
         if self.type != StatMode.ANY and path.exists() and not self.type.matches(path.stat().st_mode):
-            raise ValueError(f'expected a {self.type}')
+            raise InputValidationError(f'expected a {self.type}')
         if self.readable and not os.access(path, os.R_OK):
-            raise ValueError('it is not readable')
+            raise InputValidationError('it is not readable')
         if self.writable and not os.access(path, os.W_OK):
-            raise ValueError('it is not writable')
+            raise InputValidationError('it is not writable')
         return path
 
 
 class Path(FileInput[_Path]):
+    # noinspection PyUnresolvedReferences
     """
     :param exists: If set, then the provided path must already exist if True, or must not already exist if False.
       Default: existence is not checked.
     :param expand: Whether tilde (``~``) should be expanded.
     :param resolve: Whether the path should be fully resolved to its absolute path, with symlinks resolved, or not.
     :param type: To restrict the acceptable types of files/directories that are accepted, specify the
       :class:`StatMode` that matches the desired type.  By default, any type is accepted.  To accept specifically
       only regular files or directories, for example, use ``type=StatMode.DIR | StatMode.FILE``.
     :param readable: If True, the path must be readable.
     :param writable: If True, the path must be writable.
     :param allow_dash: Allow a dash (``-``) to be provided to indicate stdin/stdout (default: False).
     :param use_windows_fix: If True (the default) and the program is running on Windows, then :func:`.fix_windows_path`
       will be called to fix issues caused by auto-completion via Git Bash.
+    :param fix_default: Whether default values should be normalized using :meth:`~FileInput.fix_default`.
     """
 
     def __call__(self, value: PathLike) -> _Path:
         return self.validated_path(value)
 
 
 class File(FileInput[Union[FileWrapper, str, bytes]]):
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/numeric.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Union, Optional
 
 from ..typing import Bool, NT, Number, NumType, RngType
 from .base import InputType
+from .exceptions import InputValidationError
 
 __all__ = ['Range', 'NumRange']
 
 _range = range
 
 
 class NumericInput(InputType[NT], ABC):
@@ -41,35 +42,39 @@
     def _range_str(self, var: str = 'N') -> str:
         raise NotImplementedError
 
     def format_metavar(self, choice_delim: str = ',', sort_choices: bool = False) -> str:
         return f'{{{self._range_str()}}}'
 
     def fix_default(self, value: Union[str, NT, None]) -> Optional[NT]:
-        if value is None or not isinstance(value, str):
+        if value is None or not isinstance(value, str) or not self._fix_default:
             return value
         return self(value)
 
 
 class Range(NumericInput[NT]):
     """
     A range of integers that uses the builtin :class:`python:range`.  If a range object is passed to a
     :class:`.Parameter` as the ``type=`` value, it will automatically be wrapped by this class.
 
     :param range: A :class:`python:range` object
     :param snap: If True and a provided value is outside the allowed range, snap to the nearest bound.  The min or max
       of the provided range (not necessarily the start/stop values) will be used, depending on which one the provided
       value is closer to.
+    :param type: Callable that returns a numeric type, to be used on parsed values before validating whether they are
+      in the allowed range.  Defaults to :class:`python:int`.
+    :param fix_default: Whether default values should be normalized using :meth:`~NumericInput.fix_default`.
     """
 
     type: NumType = int
     range: Optional[_range]
     snap: bool
 
-    def __init__(self, range: RngType, snap: Bool = False, type: NumType = None):  # noqa
+    def __init__(self, range: RngType, snap: Bool = False, type: NumType = None, fix_default: Bool = True):  # noqa
+        super().__init__(fix_default)
         self.snap = snap
         if isinstance(range, int):
             self.range = _range(range)
         elif not isinstance(range, _range):
             self.range = _range(*range)
         else:
             self.range = range
@@ -86,20 +91,19 @@
         return base if step == 1 else f'{base}, {step=}'
 
     def __call__(self, value: str) -> NT:
         value = self.type(value)
         if value in self.range:
             return value
         elif self.snap:
-            rng_min = min(self.range)
-            if value < rng_min:
+            if (rng_min := min(self.range)) > value:
                 return rng_min
             return max(self.range)
 
-        raise ValueError(f'expected a value in the range {self._range_str()}')
+        raise InputValidationError(f'expected a value in the range {self._range_str()}')
 
 
 class NumRange(NumericInput[NT]):
     """
     A range of integers or floats, optionally only bounded on one side.
 
     By default, the min and max behave like the builtin :class:`python:range` - the min is inclusive, and the max
@@ -109,14 +113,15 @@
     :param snap: If True and a provided value is outside the allowed range, snap to the nearest bound.  Respects
       inclusivity/exclusivity of the bound.  Not supported for floats since there is not an obviously correct
       behavior for handling them in this context.
     :param min: The minimum allowed value, or None to have no lower bound
     :param max: The maximum allowed value, or None to have no upper bound
     :param include_min: Whether the minimum is inclusive (default: True)
     :param include_max: Whether the maximum is inclusive (default: False)
+    :param fix_default: Whether default values should be normalized using :meth:`~NumericInput.fix_default`.
     """
 
     __slots__ = ('type', 'snap', 'min', 'max', 'include_min', 'include_max')
     snap: bool
     min: Number
     max: Number
     include_min: bool
@@ -127,20 +132,22 @@
         type: NumType = None,  # noqa
         snap: Bool = False,
         *,
         min: Number = None,  # noqa
         max: Number = None,  # noqa
         include_min: Bool = True,
         include_max: Bool = False,
+        fix_default: Bool = True,
     ):
         if min is None and max is None:
             raise ValueError('NumRange inputs must be initialized with at least one of min and/or max values')
         elif min is not None and max is not None and min >= max:
             raise ValueError(f'Invalid {min=} >= {max=} - min must be less than max')
 
+        super().__init__(fix_default)
         if type is None:
             self.type = float if isinstance(min, float) or isinstance(max, float) else int
         else:
             self.type = type
 
         if snap:
             if self.type is float:
@@ -184,15 +191,15 @@
         :param bound: The bound (min or max) that was violated
         :param inclusive: True if the bound is inclusive, False if it is exclusive
         :param snap_dir: The direction to adjust the bound if it is exclusive as ``+1`` or ``-1``
         :return: The snap value if :attr:`.snap` is True, otherwise a :class:`python:ValueError` is raised
         """
         if self.snap:
             return bound if inclusive else (bound + snap_dir)
-        raise ValueError(f'expected a value in the range {self._range_str()}')
+        raise InputValidationError(f'expected a value in the range {self._range_str()}')
 
     def __call__(self, value: str) -> NT:
         value = self.type(value)
         if self.min is not None:
             # Bad if < when inclusive, bad if <= when exclusive
             if (value < self.min) if self.include_min else (value <= self.min):
                 return self.handle_invalid(self.min, self.include_min, 1)
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/time.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,16 +52,15 @@
     __slots__ = ('locale', 'original')
 
     def __init__(self, locale: Optional[Locale]):
         self.locale = locale
 
     def __enter__(self):
         self._lock.acquire()
-        locale = self.locale
-        if not locale:
+        if not (locale := self.locale):
             return
         # locale.getlocale does not support LC_ALL, but `setlocale(LC_ALL)` with no locale to set will return a str
         # containing all of the current locale settings as `key1=val1;key2=val2;...;keyN=valN`
         self.original = setlocale(LC_ALL)
         # The calendar.different_locale implementation only calls setlocale with LC_TIME, which caused LC_CTYPE
         # to remain set to `English_United States.1252` on Windows 10, which resulted in incorrectly encoded results.
         # Using f'LC_CTYPE={locale};LC_TIME={locale}' seemed cleaner than setting LC_ALL in its entirety, but it
@@ -82,23 +81,24 @@
     def __init_subclass__(cls, dt_type: str = None, **kwargs):
         """
         :param dt_type: Used in InvalidChoiceError / ValueError messages
         """
         super().__init_subclass__(**kwargs)
         cls.dt_type = dt_type
 
-    def __init__(self, locale: Locale = None):
+    def __init__(self, locale: Locale = None, fix_default: Bool = True):
+        super().__init__(fix_default)
         self.locale = locale
 
     @abstractmethod
     def choice_str(self, choice_delim: str = ',', sort_choices: bool = False) -> str:
         raise NotImplementedError
 
     def fix_default(self, value: Union[str, T, None]) -> Optional[T]:
-        if value is None or not isinstance(value, str):
+        if value is None or not isinstance(value, str) or not self._fix_default:
             return value
         return self(value)
 
 
 # region Calendar Unit Inputs
 
 
@@ -123,28 +123,30 @@
         *,
         full: Bool = True,
         abbreviation: Bool = True,
         numeric: Bool = False,
         locale: Locale = None,
         out_format: Union[str, DTFormatMode] = DTFormatMode.FULL,
         out_locale: Locale = None,
+        fix_default: Bool = True,
     ):
         """
         Input type representing a date/time unit.
 
         :param full: Allow the full unit name to be provided
         :param abbreviation: Allow abbreviations of unit names to be provided
         :param numeric: Allow unit values to be specified as a decimal number
         :param locale: An alternate locale to use when parsing input
         :param out_format: A :class:`DTFormatMode` or str that matches a format mode.  Defaults to full weekday name.
         :param out_locale: Alternate locale to use for output.  Defaults to the same value as ``locale``.
+        :param fix_default: Whether default values should be normalized using :meth:`~DTInput.fix_default`.
         """
         if not (full or abbreviation or numeric):
             raise ValueError('At least one of full, abbreviation, or numeric must be True')
-        super().__init__(locale=locale)
+        super().__init__(locale=locale, fix_default=fix_default)
         self.full = full
         self.abbreviation = abbreviation
         self.numeric = numeric
         self.out_format = DTFormatMode(out_format)
         self.out_locale = out_locale or self.locale
         if self.out_format not in self._formats:
             raise ValueError(f'Unsupported out_format={self.out_format} for {self.__class__.__name__} inputs')
@@ -206,24 +208,17 @@
 
         raise InvalidChoiceError(value, self.choices(), self.dt_type)
 
     def __call__(self, value: str) -> Union[str, int]:
         normalized = self.parse(value)
         if normalized < self._min_index:
             raise InvalidChoiceError(value, self.choices(), self.dt_type)
-
-        out_mode = self.out_format
-        if out_mode in (DTFormatMode.NUMERIC, DTFormatMode.NUMERIC_ISO):
+        elif (out_mode := self.out_format) in (DTFormatMode.NUMERIC, DTFormatMode.NUMERIC_ISO):
             return self._formats[out_mode][normalized]
-
-        try:
-            names_or_abbreviations = self._formats[out_mode]
-        except KeyError:
-            pass
-        else:
+        elif (names_or_abbreviations := self._formats.get(out_mode)) is not None:
             with different_locale(self.out_locale):
                 return names_or_abbreviations[normalized]
 
         raise ValueError(f'Unexpected output format={out_mode!r} for {self.dt_type}={normalized}')
 
 
 class Day(CalendarUnitInput, dt_type='day of the week'):
@@ -242,37 +237,40 @@
         full: Bool = True,
         abbreviation: Bool = True,
         numeric: Bool = False,
         iso: Bool = False,
         locale: Locale = None,
         out_format: Union[str, DTFormatMode] = DTFormatMode.FULL,
         out_locale: Locale = None,
+        fix_default: Bool = True,
     ):
         """
         Input type representing a day of the week.
 
         :param full: Allow the full day name to be provided
         :param abbreviation: Allow abbreviations of day names to be provided
         :param numeric: Allow weekdays to be specified as a decimal number
         :param iso: Ignored if ``numeric`` is False.  If True, then numeric weekdays are treated as ISO 8601 weekdays,
           where 1 is Monday and 7 is Sunday.  If False, then 0 is Monday and 6 is Sunday.
         :param locale: An alternate locale to use when parsing input
         :param out_format: A :class:`DTFormatMode` or str that matches a format mode.  Defaults to full weekday name.
         :param out_locale: Alternate locale to use for output.  Defaults to the same value as ``locale``.
+        :param fix_default: Whether default values should be normalized using :meth:`~DTInput.fix_default`.
         """
         ...
 
     def __init__(self, *, iso: Bool = False, **kwargs):
         super().__init__(**kwargs)
         self.iso = iso
 
     def parse_numeric(self, value: str) -> int:
         try:
             dow_num = int(value)
         except (ValueError, TypeError) as e:
+            # Note: The use of ValueError here is intentional and is handled by :meth:`.parse`
             raise ValueError(f'Invalid numeric weekday={value!r}') from e
 
         start, stop = (1, 7) if self.iso else (0, 6)
         if start <= dow_num <= stop:
             return (dow_num - 1) if self.iso else dow_num
 
         with different_locale(self.locale):
@@ -296,34 +294,37 @@
         *,
         full: Bool = True,
         abbreviation: Bool = True,
         numeric: Bool = True,
         locale: Locale = None,
         out_format: Union[str, DTFormatMode] = DTFormatMode.FULL,
         out_locale: Locale = None,
+        fix_default: Bool = True,
     ):
         """
         Input type representing a month.
 
         :param full: Allow the full month name to be provided
         :param abbreviation: Allow abbreviations of month names to be provided
         :param numeric: Allow months to be specified as a decimal number
         :param locale: An alternate locale to use when parsing input
         :param out_format: A :class:`DTFormatMode` or str that matches a format mode.  Defaults to full month name.
         :param out_locale: Alternate locale to use for output.  Defaults to the same value as ``locale``.
+        :param fix_default: Whether default values should be normalized using :meth:`~DTInput.fix_default`.
         """
         ...
 
     def __init__(self, *, numeric: Bool = True, **kwargs):
         super().__init__(numeric=numeric, **kwargs)
 
     def parse_numeric(self, value: str) -> int:
         try:
             month = int(value)
         except (ValueError, TypeError) as e:
+            # Note: The use of ValueError here is intentional and is handled by :meth:`.parse`
             raise ValueError(f'Invalid numeric weekday={value!r}') from e
 
         if 1 <= month <= 12:
             return month
 
         with different_locale(self.locale):
             raise InputValidationError(
@@ -333,18 +334,19 @@
 
 # endregion
 
 
 class TimeDelta(InputType[timedelta]):
     __slots__ = ('unit',)
 
-    def __init__(self, unit: TimeUnit):
+    def __init__(self, unit: TimeUnit, fix_default: Bool = True):
         unit = unit.lower()
         if unit not in _TIMEDELTA_UNITS:
             raise TypeError(f'Invalid {unit=} - expected one of: {", ".join(sorted(_TIMEDELTA_UNITS))}')
+        super().__init__(fix_default)
         self.unit = unit
         # TODO: min/max params like NumRange?
 
     def __call__(self, value: Union[str, int, float]) -> timedelta:
         if isinstance(value, str):
             try:
                 value = float(value.replace(',', '').replace('_', ''))  # allow comma or _ between thousands
@@ -352,15 +354,15 @@
                 raise InputValidationError(
                     f'Invalid numeric {self.unit}={value!r} - expected an integer or float'
                 ) from e
 
         return timedelta(**{self.unit: value})
 
     def fix_default(self, value: Union[int, float, timedelta, None]) -> Optional[timedelta]:
-        if value is None or isinstance(value, timedelta):
+        if value is None or isinstance(value, timedelta) or not self._fix_default:
             return value
         return self(value)
 
     def format_metavar(self, choice_delim: str = ',', sort_choices: bool = False) -> str:
         return f'{{{self.unit}}}'
 
 
@@ -374,17 +376,22 @@
     _latest: TimeBound = None
 
     def __init_subclass__(cls, type: Type[DT], **kwargs):  # noqa
         super().__init_subclass__(dt_type=type.__name__, **kwargs)
         cls._type = type
 
     def __init__(
-        self, formats: Collection[str], locale: Locale = None, earliest: TimeBound = None, latest: TimeBound = None
+        self,
+        formats: Collection[str],
+        locale: Locale = None,
+        earliest: TimeBound = None,
+        latest: TimeBound = None,
+        fix_default: Bool = True,
     ):
-        super().__init__(locale=locale)
+        super().__init__(locale=locale, fix_default=fix_default)
         self.formats = formats
         self.earliest = earliest
         self.latest = latest
 
     @classmethod
     def _fix_type(cls, dt: datetime) -> DT:
         try:
@@ -461,56 +468,86 @@
     def __call__(self, value: str) -> DT:
         parsed = self.parse(value)
         self._validate_bounds(parsed)
         return parsed
 
 
 class DateTime(DateTimeInput[datetime], type=datetime):
-    def __init__(self, *formats: str, locale: Locale = None, earliest: TimeBound = None, latest: TimeBound = None):
+    def __init__(
+        self,
+        *formats: str,
+        locale: Locale = None,
+        earliest: TimeBound = None,
+        latest: TimeBound = None,
+        fix_default: Bool = True,
+    ):
         """
         Input type that accepts any number of datetime format strings for parsing input.  Parsing results in returning
         a :class:`python:datetime.datetime` object.
 
         :param formats: One or more :ref:`datetime format strings <python:strftime-strptime-behavior>`.  Defaults to
           :data:`DEFAULT_DT_FMT`.
         :param locale: An alternate locale to use when parsing input
         :param earliest: If specified, the parsed value must be later than or equal to this
         :param latest: If specified, the parsed value must be earlier than or equal to this
+        :param fix_default: Whether default values should be normalized using :meth:`~DTInput.fix_default`.
         """
-        super().__init__(formats or (DEFAULT_DT_FMT,), locale=locale, earliest=earliest, latest=latest)
+        super().__init__(
+            formats or (DEFAULT_DT_FMT,), locale=locale, earliest=earliest, latest=latest, fix_default=fix_default
+        )
 
 
 class Date(DateTimeInput[date], type=date):
-    def __init__(self, *formats: str, locale: Locale = None, earliest: TimeBound = None, latest: TimeBound = None):
+    def __init__(
+        self,
+        *formats: str,
+        locale: Locale = None,
+        earliest: TimeBound = None,
+        latest: TimeBound = None,
+        fix_default: Bool = True,
+    ):
         """
         Input type that accepts any number of datetime format strings for parsing input.  Parsing results in returning
         a :class:`python:datetime.date` object.
 
         :param formats: One or more :ref:`datetime format strings <python:strftime-strptime-behavior>`.  Defaults to
           :data:`DEFAULT_DT_FMT`.
         :param locale: An alternate locale to use when parsing input
         :param earliest: If specified, the parsed value must be later than or equal to this
         :param latest: If specified, the parsed value must be earlier than or equal to this
+        :param fix_default: Whether default values should be normalized using :meth:`~DTInput.fix_default`.
         """
-        super().__init__(formats or (DEFAULT_DATE_FMT,), locale=locale, earliest=earliest, latest=latest)
+        super().__init__(
+            formats or (DEFAULT_DATE_FMT,), locale=locale, earliest=earliest, latest=latest, fix_default=fix_default
+        )
 
 
 class Time(DateTimeInput[time], type=time):
-    def __init__(self, *formats: str, locale: Locale = None, earliest: TimeBound = None, latest: TimeBound = None):
+    def __init__(
+        self,
+        *formats: str,
+        locale: Locale = None,
+        earliest: TimeBound = None,
+        latest: TimeBound = None,
+        fix_default: Bool = True,
+    ):
         """
         Input type that accepts any number of datetime format strings for parsing input.  Parsing results in returning
         a :class:`python:datetime.time` object.
 
         :param formats: One or more :ref:`datetime format strings <python:strftime-strptime-behavior>`.  Defaults to
           :data:`DEFAULT_DT_FMT`.
         :param locale: An alternate locale to use when parsing input
         :param earliest: If specified, the parsed value must be later than or equal to this
         :param latest: If specified, the parsed value must be earlier than or equal to this
+        :param fix_default: Whether default values should be normalized using :meth:`~DTInput.fix_default`.
         """
-        super().__init__(formats or (DEFAULT_TIME_FMT,), locale=locale, earliest=earliest, latest=latest)
+        super().__init__(
+            formats or (DEFAULT_TIME_FMT,), locale=locale, earliest=earliest, latest=latest, fix_default=fix_default
+        )
 
 
 # endregion
 
 
 def dt_repr(dt: Union[datetime, date, time], use_repr: bool = True) -> str:
     try:
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     def __init__(self, default: Any):
         self.default = default
 
     def __set_name__(self, owner, name: str):
         self.name = name
 
     def __get__(self, instance, owner) -> Any:
-        if instance is None:
-            return self
         try:
             return instance.__dict__[self.name]
+        except AttributeError:  # instance is None
+            return self
         except KeyError:
             return self.default
 
     def __set__(self, instance, value: Any):
         if value != self.default:
             instance.__dict__[self.name] = value
 
@@ -104,15 +104,15 @@
         self.converter = converter
         self.pass_file = pass_file
         self.parents = parents
         self._fp: Union[TextIO, BinaryIO, None] = None
         self._finalizer = None
 
     def __eq__(self, other: FileWrapper) -> bool:
-        attrs = ('path', 'mode', 'binary', 'encoding', 'errors', 'converter', 'pass_file')
+        attrs = ('path', 'mode', 'binary', 'encoding', 'errors', 'converter', 'pass_file', 'parents')
         try:
             return all(getattr(self, a) == getattr(other, a) for a in attrs)
         except AttributeError:
             return NotImplemented
 
     def read(self) -> Any:
         with self._file() as f:
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/metadata.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,77 +10,123 @@
 from collections import defaultdict
 from functools import cached_property
 from importlib.metadata import entry_points, EntryPoint
 from inspect import getmodule
 from pathlib import Path
 from sys import modules
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Type, Optional, Union, Tuple, Dict
+from typing import TYPE_CHECKING, Any, Type, Callable, Optional, Union, Iterator, Tuple, Dict
 from urllib.parse import urlparse
 
 from .context import ctx, NoActiveContext
 
 if TYPE_CHECKING:
     from .typing import Bool, CommandType, OptStr
 
 __all__ = ['ProgramMetadata']
 
 DEFAULT_FILE_NAME: str = 'UNKNOWN'
 
-# TODO: Make it possible to auto-detect author email/url more centrally without needing to import version vars in every
-#  CLI module
 
+# region Metadata Descriptors
 
-class Metadata:
-    __slots__ = ('default', 'name')
 
-    def __init__(self, default):
-        self.default = default
+class MetadataBase:
+    __slots__ = ('name', 'inheritable')
+
+    def __init__(self, inheritable: bool = True):
+        self.inheritable = inheritable
 
     def __set_name__(self, owner: Type[ProgramMetadata], name: str):
         self.name = name
         owner._fields.add(name)
 
     def __get__(self, instance: Optional[ProgramMetadata], owner: Type[ProgramMetadata]):
-        if instance is None:
-            return self
         try:
             return instance.__dict__[self.name]
+        except AttributeError:  # instance is None
+            return self
         except KeyError:
             pass
-        try:
-            return getattr(instance.parent, self.name)
-        except AttributeError:  # parent is None
-            return self.default
+        if self.inheritable and (parent := self.get_parent(instance)):
+            return getattr(parent, self.name)
+        return self.get_value(instance)
 
     def __set__(self, instance: ProgramMetadata, value: Union[str, Path, None]):
         if value is not None:
             instance.__dict__[self.name] = value
 
     def __repr__(self) -> str:
-        return f'Metadata(default={self.default!r})'
+        return f'{self.__class__.__name__}({", ".join(f"{a}={v}" for a, v in self._attrs())})'
+
+    def _attrs(self) -> Iterator[Tuple[str, Any]]:
+        for base in self.__class__.mro()[:-1]:
+            for attr in base.__slots__:
+                if attr != 'name':
+                    value = getattr(self, attr)
+                    yield attr, (getattr(value, '__qualname__', value) if attr == 'func' else repr(value))
+
+    def get_parent(self, instance: ProgramMetadata) -> Optional[ProgramMetadata]:
+        # if (parent := instance.parent) and parent.distribution == instance.distribution:
+        if (parent := instance.parent) and parent.package == instance.package:
+            return parent
+        return None
+
+    def get_value(self, instance: ProgramMetadata):
+        raise NotImplementedError
+
+
+class Metadata(MetadataBase):
+    __slots__ = ('default',)
+
+    def __init__(self, default, inheritable: bool = True):
+        super().__init__(inheritable)
+        self.default = default
+
+    def get_value(self, instance: ProgramMetadata):
+        return self.default
+
+
+class DynamicMetadata(MetadataBase):
+    __slots__ = ('func',)
+
+    def __init__(self, func: Callable[[ProgramMetadata], Any], inheritable: bool = True):
+        super().__init__(inheritable)
+        self.func = func
+
+    def get_value(self, instance: ProgramMetadata):
+        instance.__dict__[self.name] = result = self.func(instance)
+        return result
+
+
+def dynamic_metadata(func=None, *, inheritable: bool = True):
+    if func is None:
+        return lambda f: DynamicMetadata(f, inheritable)
+    else:
+        return DynamicMetadata(func, inheritable)
+
+
+# endregion
 
 
 class ProgramMetadata:
     _fields = {'parent'}
     parent: Optional[ProgramMetadata] = None
-    path: Path = Metadata(None)
-    package: str = Metadata(None)
-    module: str = Metadata(None)
-    command: str = Metadata(None)
-    prog: str = Metadata(None)
-    prog_src: str = Metadata(None)
+    path: Path = Metadata(None, inheritable=False)
+    package: str = Metadata(None, inheritable=False)
+    module: str = Metadata(None, inheritable=False)
+    cmd_module: str = Metadata(None, inheritable=False)
+    command: str = Metadata(None, inheritable=False)
     url: str = Metadata(None)
     docs_url: str = Metadata(None)
     email: str = Metadata(None)
     version: str = Metadata('')
     usage: str = Metadata(None)
     description: str = Metadata(None)
     epilog: str = Metadata(None)
-    doc_name: str = Metadata(None)
     doc_str: str = Metadata('')
     pkg_doc_str: str = Metadata('')  # Set by :func:`~.documentation.load_commands` to capture package docstrings
 
     def __init__(self, **kwargs):
         fields = self._fields
         for key, val in kwargs.items():
             if key in fields:
@@ -104,68 +150,106 @@
         docs_url: str = None,
         email: str = None,
         version: str = None,
         usage: str = None,
         description: str = None,
         epilog: str = None,
         doc_name: str = None,
-        no_sys_argv: Bool = None,
     ) -> ProgramMetadata:
         path, g = _path_and_globals(command, path)
-        if command.__module__ != 'cli_command_parser.commands':
+        if (cmd_module := command.__module__) != 'cli_command_parser.commands':
             # Prevent inheritors from getting docstrings from the base Command
             doc_str = g.get('__doc__')
             doc = command.__doc__
         else:
             doc = doc_str = None
 
-        prog, prog_src = _prog_finder.normalize(prog, path, parent, no_sys_argv, command)
         return cls(
             parent=parent,
             path=path,
             package=g.get('__package__'),
             module=g.get('__module__'),
+            cmd_module=cmd_module,
             command=command.__qualname__,
             prog=prog,
-            prog_src=prog_src,
             url=url or g.get('__url__'),
-            docs_url=docs_url or _docs_url_from_repo_url(url) or _docs_url_from_repo_url(g.get('__url__')),
+            docs_url=docs_url,
             email=email or g.get('__author_email__'),
             version=version or g.get('__version__'),
             usage=usage,
             description=_description(description, doc),
             epilog=epilog,
-            doc_name=_doc_name(doc_name, path, prog),
+            doc_name=doc_name,
             doc_str=doc_str,
         )
 
     def __repr__(self) -> str:
         return _repr(self)
 
-    def format_epilog(self, extended: Bool = True) -> str:
+    # region Program Name Properties
+
+    @cached_property
+    def _prog_and_src(self) -> Tuple[str, str]:
+        if prog := self.__dict__.get('prog'):
+            return prog, 'class kwargs'
+        return _prog_finder.normalize(self.path, self.parent, None, self.cmd_module, self.command)
+
+    @dynamic_metadata
+    def prog(self) -> str:
+        return self._prog_and_src[0]
+
+    @cached_property
+    def _doc_prog_and_src(self) -> Tuple[str, str]:
+        if prog := self.__dict__.get('prog'):
+            return prog, 'class kwargs'
+        return _prog_finder.normalize(self.path, self.parent, False, self.cmd_module, self.command)
+
+    def get_prog(self, allow_sys_argv: Bool = None) -> str:
+        return self._get_prog(allow_sys_argv)[0]
+
+    def _get_prog(self, allow_sys_argv: Bool = None) -> Tuple[str, str]:
+        return self._prog_and_src if allow_sys_argv or allow_sys_argv is None else self._doc_prog_and_src
+
+    @dynamic_metadata(inheritable=False)
+    def doc_name(self) -> str:
+        return Path(self._doc_prog_and_src[0]).stem
+
+    # endregion
+
+    @dynamic_metadata
+    def docs_url(self) -> OptStr:
+        return _docs_url_from_repo_url(self.url)
+
+    def format_epilog(self, extended: Bool = True, allow_sys_argv: Bool = None) -> str:
         parts = [self.epilog] if self.epilog else []
         if parts and not extended:
             return parts[0]
 
         if version := self.version:
             version = f' [ver. {version}]'
         if self.email:
-            parts.append(f'Report {self.prog}{version} bugs to {self.email}')
+            parts.append(f'Report {self.get_prog(allow_sys_argv)}{version} bugs to {self.email}')
         if url := self.docs_url or self.url:
             parts.append(f'Online documentation: {url}')
         return '\n\n'.join(parts)
 
-    def get_doc_str(self, strip: bool = True) -> OptStr:
+    def get_doc_str(self, strip: Bool = True) -> OptStr:
         if (doc_str := self.pkg_doc_str) and strip:
             doc_str = doc_str.strip()
         if not doc_str:
             if (doc_str := self.doc_str) and strip:
                 doc_str = doc_str.strip()
         return doc_str
 
+    def get_description(self, allow_inherited: Bool = True) -> OptStr:
+        if description := self.description:
+            if not allow_inherited and (parent := self.parent) and (parent_description := parent.description):  # noqa
+                return description if parent_description != description else None
+        return description
+
 
 def _repr(obj, indent=0) -> str:
     if not isinstance(obj, ProgramMetadata):
         return repr(obj)
 
     field_dict = {field: getattr(obj, field) for field in sorted(obj._fields)}
     prev_str = ' ' * indent
@@ -186,72 +270,72 @@
 
         mod_obj_prog_map.default_factory = None  # Disable automatic defaults
         return mod_obj_prog_map
 
     @classmethod
     def _get_console_scripts(cls) -> Tuple[EntryPoint, ...]:
         try:
-            return entry_points(group='console_scripts')
+            return entry_points(group='console_scripts')  # noqa
         except TypeError:  # Python 3.8 or 3.9
             return entry_points()['console_scripts']
 
     def normalize(
         self,
-        prog: OptStr,
         cmd_path: Path,
         parent: Optional[ProgramMetadata],
-        no_sys_argv: Bool,
-        command: CommandType,
+        allow_sys_argv: Bool,
+        cmd_module: str,
+        cmd_name: str,
     ) -> Tuple[OptStr, str]:
-        if prog:
-            return prog, 'class kwargs'
-
-        # TODO: This isn't working for documentation generation...
-        if ep_name := self._from_entry_point(command):
+        if ep_name := self._from_entry_point(cmd_module, cmd_name):
             return ep_name, 'entry_points'
 
-        if no_sys_argv is None:
+        if allow_sys_argv is None:
             try:
-                no_sys_argv = not ctx.allow_argv_prog
+                allow_sys_argv = ctx.allow_argv_prog
             except NoActiveContext:
-                no_sys_argv = False
+                allow_sys_argv = True
+
+        if parent:
+            p_prog, p_src = parent._get_prog(allow_sys_argv)
+            if p_prog and p_src != 'path':
+                return p_prog, p_src
 
-        if parent and parent.prog != parent.path.name and (not no_sys_argv or parent.prog_src != 'sys.argv'):
-            return parent.prog, parent.prog_src
-        elif not no_sys_argv:
-            if argv_name := self._from_sys_argv():
-                return argv_name, 'sys.argv'
+        if allow_sys_argv and (argv_name := self._from_sys_argv()):
+            return argv_name, 'sys.argv'
 
         return cmd_path.name, 'path'
 
-    def _from_entry_point(self, command: CommandType) -> OptStr:
+    def _from_entry_point(self, cmd_module: str, cmd_name: str) -> OptStr:
+        # TODO: Verify whether this is working for documentation generation...
         main_mod = 'cli_command_parser.commands'
-        for prog, obj, obj_mod, obj_name in self._iter_entry_point_candidates(command):
-            if obj is command or (obj_mod == main_mod and obj_name == 'main'):
+        for prog, obj, obj_mod, obj_name in self._iter_entry_point_candidates(cmd_module):
+            if (obj_name == cmd_name and obj_mod == cmd_module) or (obj_mod == main_mod and obj_name == 'main'):
                 return prog
 
         return None
 
-    def _iter_entry_point_candidates(self, command: CommandType):
+    def _iter_entry_point_candidates(self, cmd_module: str):
+        # TODO: Use ProgramMetadata.distribution.entry_points() instead?
         try:
             # TODO: This likely won't work for a base command in one module, sub commands defined in separate modules,
             #  and main imported from cli_command_parser in the package's __init__/__main__ module...
-            obj_prog_map = self.mod_obj_prog_map[command.__module__]
-            module = modules[command.__module__]
+            obj_prog_map = self.mod_obj_prog_map[cmd_module]
+            module = modules[cmd_module]
         except KeyError:
             pass
         else:
             for obj_name, prog in obj_prog_map.items():
                 base_name = obj_name.split('.', 1)[0]
                 try:
                     obj = getattr(module, base_name)
                 except AttributeError:
                     pass
                 else:
-                    yield prog, obj, getattr(obj, '__module__', ''), getattr(obj, '__name__', '')
+                    yield prog, obj, getattr(obj, '__module__', ''), getattr(obj, '__qualname__', '')
 
     def _from_sys_argv(self) -> OptStr:
         try:
             ctx_prog = ctx.prog
         except NoActiveContext:
             return None
 
@@ -264,50 +348,44 @@
         return None
 
 
 _prog_finder = ProgFinder()
 
 
 def _path_and_globals(command: CommandType, path: Path = None) -> Tuple[Path, Dict[str, Any]]:
-    module = getmodule(command)
+    module = getmodule(command)  # Returns the module object (obj.__module__ just provides the name of the module)
     if path is None:
         try:
             path = Path(module.__file__).resolve()
         except AttributeError:  # module is None
             path = Path.cwd().joinpath(DEFAULT_FILE_NAME)
 
     if module is None:
         return path, {}
 
     return path, module.__dict__
 
 
-def _description(description: Optional[str], doc: Optional[str]) -> Optional[str]:
+def _description(description: OptStr, doc: OptStr) -> OptStr:
     if description:
         return description
     elif doc:
         doc = dedent(doc).lstrip()
         if doc.strip():  # avoid space-only doc, but let possibly intentional trailing spaces / newlines to persist
             return doc
     return None
 
 
-def _docs_url_from_repo_url(repo_url: Optional[str]) -> Optional[str]:
+def _docs_url_from_repo_url(repo_url: OptStr) -> OptStr:
     if not repo_url:
         return None
 
     parsed = urlparse(repo_url)
     if parsed.scheme == 'https' and parsed.hostname == 'github.com':
         try:
             user, repo = parsed.path[1:].split('/', 1)
         except ValueError:
             pass
         else:
             return f'https://{user}.github.io/{repo}/'
 
     return None
-
-
-def _doc_name(doc_name: Optional[str], path: Path, prog: str) -> str:
-    if doc_name:
-        return doc_name
-    return Path(prog).stem
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/nargs.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/nargs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Helpers for handling ``nargs=...`` for Parameters.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import Union, Optional, Sequence, Collection, Iterable, Tuple, Set, FrozenSet
+from typing import Any, Union, Optional, Sequence, Collection, Iterable, Tuple, Set, FrozenSet
 
-__all__ = ['Nargs', 'NargsValue', 'REMAINDER', 'nargs_max_sum', 'nargs_min_sum']
+__all__ = ['Nargs', 'NargsValue', 'REMAINDER', 'nargs_min_and_max_sums']
 
 REMAINDER = type('REMAINDER', (), {})()
 _UNBOUND = (None, REMAINDER)
 NARGS_STR_RANGES = {'?': (0, 1), '*': (0, None), '+': (1, None), 'REMAINDER': (0, REMAINDER)}
 SET_ERROR_FMT = 'Invalid nargs={!r} set - expected non-empty set where all values are integers >= 0'
 SEQ_ERROR_FMT = 'Invalid nargs={!r} sequence - expected 2 ints where 0 <= a <= b or b is None'
 
@@ -156,22 +156,41 @@
         numbers provided for this to return True.
         """
         if self._has_upper_bound:
             return count in self.allowed
         else:
             return count >= self.min
 
+    def max_reached(self, parsed_values: Collection[Any]) -> bool:
+        """
+        :param parsed_values: The value(s) parsed so far for a Parameter.
+        :return: True if ``parsed_values`` has a length and that length meets or exceeds the maximum count allowed,
+          False otherwise.
+        """
+        if self._has_upper_bound:
+            return len(parsed_values) >= self.max
+        return False
+
     @property
     def has_upper_bound(self) -> bool:
         return self._has_upper_bound
 
     @property
     def upper_bound(self) -> Union[int, float]:
         return self.max if self._has_upper_bound else float('inf')
 
 
-def nargs_max_sum(nargs_objects: Iterable[Nargs]) -> Union[int, float]:
-    return sum(obj.upper_bound for obj in nargs_objects)
+def nargs_min_and_max_sums(nargs_objects: Iterable[Nargs]) -> Tuple[int, Union[int, float]]:
+    min_sum, max_sum = 0, 0
+    iter_nargs = iter(nargs_objects)
+    for obj in iter_nargs:
+        min_sum += obj.min
+        if obj._has_upper_bound:
+            max_sum += obj.max
+        else:
+            max_sum = float('inf')
+            break
 
+    for obj in iter_nargs:  # If any had no upper bound, then this loop will complete the min total
+        min_sum += obj.min  # Otherwise, it will not have anything to iterate over
 
-def nargs_min_sum(nargs_objects: Iterable[Nargs]) -> int:
-    return sum(obj.min for obj in nargs_objects)
+    return min_sum, max_sum
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/options.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,645 +1,492 @@
 """
-Base classes and helpers for Parameters and Groups
+Optional Parameters
 
 :author: Doug Skrypa
 """
-# pylint: disable=R0801
 
 from __future__ import annotations
 
-import re
-from abc import ABC, abstractmethod
-from contextvars import ContextVar
-from functools import partial, update_wrapper, cached_property
-from itertools import chain
-from typing import TYPE_CHECKING, Any, Type, Generic, Optional, Callable, Collection, Union, Iterator, overload
-from typing import List, Tuple, FrozenSet
-
-from ..annotations import get_descriptor_value_type
-from ..config import CommandConfig, OptionNameMode, AllowLeadingDash
-from ..context import Context, ctx, get_current_context
-from ..exceptions import ParameterDefinitionError, BadArgument, MissingArgument, InvalidChoice
-from ..exceptions import ParamUsageError, NoActiveContext, UnsupportedAction
-from ..inputs import InputType, normalize_input_type
-from ..inputs.choices import _ChoicesBase, Choices, ChoiceMap as ChoiceMapInput
-from ..inputs.exceptions import InputValidationError, InvalidChoiceError
-from ..nargs import Nargs, REMAINDER
-from ..typing import Bool, ValSrc, OptStrs, CommandCls, CommandObj, CommandAny, Param, LeadingDash, T_co
-from ..utils import _NotSet, ValueSource
-from .option_strings import OptionStrings
+import logging
+from abc import ABC
+from functools import partial, update_wrapper
+from typing import TYPE_CHECKING, Any, Optional, Callable, Union, TypeVar, NoReturn, Literal, Tuple
+
+from ..exceptions import ParameterDefinitionError, BadArgument, CommandDefinitionError, ParamUsageError, ParserExit
+from ..inputs import normalize_input_type
+from ..nargs import Nargs, NargsValue
+from ..typing import T_co, TypeFunc
+from ..utils import _NotSet, str_to_bool
+from .actions import Store, StoreConst, Append, AppendConst, Count
+from .base import BaseOption, AllowLeadingDashProperty
+from .option_strings import TriFlagOptionStrings
 
 if TYPE_CHECKING:
-    from types import MethodType
-    from ..formatting.params import ParamHelpFormatter
-    from .groups import ParamGroup
+    from ..typing import Bool, ChoicesType, InputTypeFunc, CommandCls, CommandObj, OptStr, LeadingDash
 
-__all__ = ['Parameter', 'BasePositional', 'BaseOption']
+__all__ = [
+    'Option',
+    'Flag',
+    'TriFlag',
+    'ActionFlag',
+    'Counter',
+    'action_flag',
+    'before_main',
+    'after_main',
+    'help_action',
+]
+log = logging.getLogger(__name__)
+
+TD = TypeVar('TD')
+TC = TypeVar('TC')
+TA = TypeVar('TA')
+ConstAct = Literal['store_const', 'append_const']
 
-_group_stack = ContextVar('cli_command_parser.parameters.base.group_stack', default=[])
-_is_numeric = re.compile(r'^-\d+$|^-\d*\.\d+?$').match
 
-
-class parameter_action:  # pylint: disable=C0103
-    """
-    Decorator that is used to register :paramref:`Parameter.__init__.action` handler methods to store values that are
-    provided for that type of :class:`Parameter`.  The name of the decorated method is used as the ``action`` name.
-
-    :param method: The method that should be used to handle storing values
-    """
-
-    def __init__(self, method: MethodType):
-        self.method = method
-        update_wrapper(self, method)
-
-    def __set_name__(self, parameter_cls: Type[Parameter], name: str):
-        """
-        Registers the decorated method in the Parameter subclass's _actions dict, then replaces the action decorator
-        with the original method.
-
-        Since `__set_name__` is called on descriptors before their containing class's parent's `__init_subclass__` is
-        called, name action/method name conflicts are handled by imitating a name mangled dunder attribute that will be
-        unique to each subclass.  The mangled name is replaced with the friendlier `_actions` in
-        :meth:`Parameter.__init_subclass__`.
-        """
-        attr = f'_{parameter_cls.__name__}__actions'
-        try:
-            actions = getattr(parameter_cls, attr)
-        except AttributeError:
-            actions = set()
-            setattr(parameter_cls, attr, actions)
-
-        actions.add(name)
-
-    def __call__(self, *args, **kwargs) -> int:
-        result = self.method(*args, **kwargs)
-        return 1 if result is None else result
-
-    def __get__(self, instance: Optional[Parameter], owner: Type[Parameter]):
-        if instance is None:
-            return self
-        return partial(self.__call__, instance)
-
-
-class ParamBase(ABC):
+class Option(BaseOption[Union[T_co, TD]], actions=(Store, Append)):
     """
-    Base class for :class:`Parameter` and :class:`.ParamGroup`.
+    A generic option that can be specified as ``--foo bar`` or by using other similar forms.
 
-    :param name: The name to use for this parameter.  Defaults to the name assigned to this parameter.
+    :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
+      then one will automatically be added based on the name assigned to this parameter.
+    :param nargs: The number of values that are expected/required when this parameter is specified.  Defaults to ``+``
+      when ``action='append'``, and to ``1`` otherwise. See :class:`.Nargs` for more info.
+    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
+      that extend Parameter, and must be registered via :class:`.parameter_action`.  Defaults to ``store`` when
+      ``nargs=1``, and to ``append`` otherwise.  A single value will be stored when ``action='store'``, and a list
+      of values will be stored when ``action='append'``.
+    :param default: The default value for this parameter if it is not specified.  Defaults to ``None`` if
+      this parameter is not required; not used if it is required.
     :param required: Whether this parameter is required or not.  If it is required, then an exception will be
       raised if the user did not provide a value for this parameter.  Defaults to ``False``.
-    :param help: A brief description of this parameter that will appear in ``--help`` text.
-    :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
+    :param type: A callable (function, class, etc.) that accepts a single string argument, which should be called
+      on every value for this parameter to transform the value.  By default, no transformation is performed, and
+      values will be strings.  If not specified, but a type annotation is detected, then that annotation will be
+      used as if it was provided here.  When both are present, this argument takes precedence.
+    :param choices: A container that holds the specific values that users must pick from.  By default, any value is
+      allowed.
+    :param allow_leading_dash: Whether string values may begin with a dash (``-``).  By default, if a value begins with
+      a dash, it is only accepted if it appears to be a negative numeric value.  Use ``True`` / ``always`` /
+      ``AllowLeadingDash.ALWAYS`` to allow any value that begins with a dash (as long as it is not an option string for
+      an Option/Flag/etc).  To reject all values beginning with a dash, including numbers, use ``False`` / ``never`` /
+      ``AllowLeadingDash.NEVER``.
+    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
     """
 
-    __name: str = None              #: Always the name of the attr that points to this object
-    _name: str = None               #: An explicitly provided name, or the name of the attr that points to this object
-    group: ParamGroup = None        #: The group this object is a member of, if any
-    command: CommandCls = None      #: The :class:`.Command` this object is a member of
-    required: Bool = False          #: Whether this param/group is required
-    help: str = None                #: The description for this param/group that will appear in ``--help`` text
-    hide: Bool = False              #: Whether this param/group should be hidden in ``--help`` text
-    missing_hint: str = None        #: Hint to provide if this param/group is missing
-
-    def __init__(self, name: str = None, required: Bool = False, help: str = None, hide: Bool = False):  # noqa
-        self.__doc__ = help  # Prevent this class's docstring from showing up for params in generated documentation
-        self.required = required
-        self.name = name
-        self.help = help
-        self.hide = hide
-        if group := get_active_param_group():
-            group.register(self)  # noqa  # This sets self.group = group
+    default: TD
+    allow_leading_dash = AllowLeadingDashProperty()
 
-    @property
-    def name(self) -> str:
-        if (name := self._name) is not None:
-            return name
-        return self._default_name()
-
-    @name.setter
-    def name(self, value: Optional[str]):
-        if value is not None:
-            self._name = value
-
-    def _default_name(self) -> str:
-        return f'{self.__class__.__name__}#{id(self)}'
-
-    def __set_name__(self, command: CommandCls, name: str):
-        self.command = command
-        if self._name is None:
-            self.name = name
-        self.__name = name
+    def __init__(
+        self,
+        *option_strs: str,
+        nargs: NargsValue = None,
+        action: Literal['store', 'append'] = None,
+        default: TD = _NotSet,
+        required: Bool = False,
+        type: InputTypeFunc = None,  # noqa
+        choices: ChoicesType = None,
+        allow_leading_dash: LeadingDash = None,
+        **kwargs,
+    ):
+        if nargs_provided := nargs is not None:
+            nargs = Nargs(nargs)
+            if 0 in nargs:
+                nargs = nargs._orig
+                details = 'use Flag or Counter for Options that can be specified without a value'
+                if isinstance(nargs, range) and nargs.start == 0 and nargs.step != nargs.stop:
+                    suffix = f', {nargs.step}' if nargs.step != 1 else ''
+                    details = f'try using range({nargs.step}, {nargs.stop}{suffix}) instead, or {details}'
+                raise ParameterDefinitionError(f'Invalid {nargs=} - {details}')
+
+        if not action:
+            if nargs_provided:
+                action = 'store' if nargs == 1 else 'append'
+            else:
+                action = 'store'
+        elif nargs_provided and action == 'store' and nargs != 1:
+            raise ParameterDefinitionError(f'Invalid {nargs=} for {action=}')
 
-    def __hash__(self) -> int:
-        return hash(self.__class__) ^ hash(self.__name) ^ hash(self.name) ^ hash(self.command)
+        super().__init__(*option_strs, action=action, default=default, required=required, **kwargs)
+        if not nargs_provided:
+            nargs = self.action.default_nargs
 
-    def _ctx(self, command: CommandAny = None) -> Context:
-        try:
-            return get_current_context()
-        except NoActiveContext:
-            pass
-        if command is None:
-            command = self.command
-        try:
-            return command._Command__ctx
-        except AttributeError:
-            pass
-        raise NoActiveContext('There is no active context')
+        self.nargs = nargs
+        self.type = normalize_input_type(type, choices)
+        self.allow_leading_dash = allow_leading_dash
 
-    def _config(self, command: CommandAny = None) -> CommandConfig:
-        try:
-            return self._ctx(command).config
-        except NoActiveContext:
-            if command is None:
-                command = self.command
-            return command.__class__.config(command)
-
-    # region Usage / Help Text
-
-    @cached_property
-    def formatter(self) -> ParamHelpFormatter:
-        from ..formatting.params import ParamHelpFormatter  # Here due to circular dependency
+    def _handle_bad_action(self, action: str) -> NoReturn:
+        if action in ('store_const', 'append_const'):
+            raise ParameterDefinitionError(f'Invalid {action=} for {self.__class__.__name__} - use Flag instead')
+        super()._handle_bad_action(action)
 
-        try:
-            formatter_factory = self._config().param_formatter or ParamHelpFormatter
-        except AttributeError:  # self.command is None
-            formatter_factory = ParamHelpFormatter
 
-        return formatter_factory(self)  # noqa
+class Flag(BaseOption[Union[TD, TC]], actions=(StoreConst, AppendConst)):
+    """
+    A (typically boolean) option that does not accept any values.
 
-    @property
-    @abstractmethod
-    def show_in_help(self) -> bool:
-        raise NotImplementedError
+    :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
+      then one will automatically be added based on the name assigned to this parameter.
+    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
+      that extend Parameter, and must be registered via :class:`.parameter_action`.  Defaults to ``store_const``, but
+      accepts ``append_const`` to build a list of the specified constant.
+    :param default: The default value for this parameter if it is not specified.  Defaults to ``False`` when
+      ``const=True`` (the default), and to ``True`` when ``const=False``.  Defaults to ``None`` for any other
+      constant.
+    :param const: The constant value to store/append when this parameter is specified.  Defaults to ``True``.
+    :param type: A callable (function, class, etc.) that accepts a single string argument and returns a boolean value,
+      which should be called on environment variable values, if any are configured for this Flag via
+      :paramref:`.BaseOption.env_var`.  It should return a truthy value if any action should be taken (i.e., if the
+      constant should be stored/appended), or a falsey value for no action to be taken.  The
+      :func:`default function<.str_to_bool>` handles parsing ``1`` / ``true`` / ``yes`` and similar as ``True``,
+      and ``0`` / ``false`` / ``no`` and similar as ``False``.  If :paramref:`use_env_value` is ``True``, then this
+      function should return either the default or constant value instead.
+    :param strict_env: When ``True`` (the default), if an :paramref:`.BaseOption.env_var` is used as the source of a
+      value for this parameter and that value is invalid, then parsing will fail.  When ``False``, invalid values from
+      environment variables will be ignored (and a warning message will be logged).
+    :param use_env_value: If ``True``, when an :paramref:`.BaseOption.env_var` is used as the source of a value for
+      this Flag, the parsed value will be stored as this Flag's value (it must match either the default or constant
+      value).  If ``False`` (the default), then the parsed value will be used to determine whether this Flag's normal
+      action should be taken as if it was specified via a CLI argument.
+    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
+    """
 
-    def format_usage(self, *args, **kwargs) -> str:
-        """Convenience method for calling :meth:`.ParamHelpFormatter.format_usage`"""
-        return self.formatter.format_usage(*args, **kwargs)
+    nargs = Nargs(0)
+    type = staticmethod(str_to_bool)  # Without staticmethod, this would be interpreted as a normal method
+    use_env_value: bool = False
+    __default_const_map = {True: False, False: True, _NotSet: True}
+    default: TD
+    const: TC
 
-    def format_help(self, *args, **kwargs) -> str:
-        """Convenience method for calling :meth:`.ParamHelpFormatter.format_help`"""
-        return self.formatter.format_help(*args, **kwargs)
+    def __init__(
+        self,
+        *option_strs: str,
+        action: ConstAct = 'store_const',
+        default: TD = _NotSet,
+        const: TC = _NotSet,
+        type: TypeFunc = None,  # noqa
+        **kwargs,
+    ):
+        if const is _NotSet:
+            try:
+                const = self.__default_const_map[default]
+            except KeyError as e:
+                raise ParameterDefinitionError(
+                    f"A 'const' value is required for {self.__class__.__name__} since {default=} is not True or False"
+                ) from e
+        if default is _NotSet:
+            default = self.__default_const_map.get(const, _NotSet)  # will be True or False
+        if default is False:  # Avoid surprises for custom non-truthy values
+            kwargs.setdefault('show_default', False)
+        super().__init__(*option_strs, action=action, default=default, **kwargs)
+        self.const = const
+        if type is not None:
+            self.type = type
 
-    # endregion
+    def get_env_const(self, value: str, env_var: str) -> Tuple[Union[TC, TD], bool]:
+        try:
+            parsed = self.type(value)
+        except Exception as e:
+            raise ParamUsageError(self, f'unable to parse {value=} from {env_var=}: {e}') from e
+        if self.use_env_value and parsed != self.const and parsed != self.default:
+            raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
+        return parsed, self.use_env_value
 
 
-class Parameter(ParamBase, Generic[T_co], ABC):
+class TriFlag(BaseOption[Union[TD, TC, TA]], ABC, actions=(StoreConst, AppendConst)):
     """
-    Base class for all other parameters.  It is not meant to be used directly.
-
-    Custom parameter classes should generally extend :class:`BasePositional` or :class:`BaseOption` instead of this,
-    otherwise additional handling may be necessary in the parser.
-
-    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
-      that extend Parameter, and must be registered via :class:`parameter_action`.
-    :param name: The name to use for this parameter.  Defaults to the name assigned to this parameter.
-    :param default: The default value for this parameter if it is not specified.  Defaults to ``None`` if this
-      parameter is not required; not used if it is required.
-    :param required: Whether this parameter is required or not.  If it is required, then an exception will be
-      raised if the user did not provide a value for this parameter.  Defaults to ``False``.
-    :param metavar: The name to use as a placeholder for values in usage / help messages.
-    :param help: A brief description of this parameter that will appear in ``--help`` text.
-    :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
-    :param show_default: Override the :attr:`.CommandConfig.show_defaults` setting for this parameter to always or
-      never include the default value in usage / help messages.  Default: follow the ``show_defaults`` setting.
+    A trinary / ternary Flag.  While :class:`.Flag` only supports 1 constant when provided, with 1 default if not
+    provided, this class accepts a pair of constants for the primary and alternate values to store, along with a
+    separate default.
+
+    :param option_strs: The primary long and/or short option prefixes for this option.  If no long prefixes are
+      specified, then one will automatically be added based on the name assigned to this parameter.
+    :param consts: A 2-tuple containing the ``(primary, alternate)`` values to store.  Defaults to ``(True, False)``.
+    :param alt_prefix: The prefix to add to the assigned name for the alternate long form.  Ignored if ``alt_long`` is
+      specified.  Defaults to ``no`` if ``alt_long`` is not specified.
+    :param alt_long: The alternate long form to use.
+    :param alt_short: The alternate short form to use.
+    :param alt_help: The help text to display with the alternate option strings.
+    :param action: The action to take on individual parsed values.  Only ``store_const`` (the default) is supported.
+    :param default: The default value to use if neither the primary or alternate options are provided.  Defaults
+      to None.
+    :param name_mode: Override the configured :ref:`configuration:Parsing Options:option_name_mode` for this TriFlag.
+    :param type: A callable (function, class, etc.) that accepts a single string argument and returns a boolean value,
+      which should be called on environment variable values, if any are configured for this TriFlag via
+      :paramref:`.BaseOption.env_var`.  It should return a truthy value if the primary constant should be stored, or a
+      falsey value if the alternate constant should be stored.  The :func:`default function<.str_to_bool>` handles
+      parsing ``1`` / ``true`` / ``yes`` and similar as ``True``, and ``0`` / ``false`` / ``no`` and similar
+      as ``False``.  If :paramref:`use_env_value` is ``True``, then this function should return the primary or
+      alternate constant or the default value instead.
+    :param strict_env: When ``True`` (the default), if an :paramref:`.BaseOption.env_var` is used as the source of a
+      value for this parameter and that value is invalid, then parsing will fail.  When ``False``, invalid values from
+      environment variables will be ignored (and a warning message will be logged).
+    :param use_env_value: If ``True``, when an :paramref:`.BaseOption.env_var` is used as the source of a value for
+      this TriFlag, the parsed value will be stored as this TriFlag's value (it must match the primary or alternate
+      constant, or the default value).  If ``False`` (the default), then the parsed value will be used to determine
+      whether this TriFlag's normal action should be taken as if it was specified via a CLI argument.
+    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
     """
 
-    # region Attributes & Initialization
-
-    # Class attributes
-    _actions: FrozenSet[str] = frozenset()          #: The actions supported by this Parameter
-    _repr_attrs: Optional[Collection[str]] = None   #: Attributes to include in ``repr()`` output
-    accepts_none: bool = False                      #: Whether this Parameter can be provided without a value
-    accepts_values: bool = True                     #: Whether this Parameter can be provided with at least 1 value
-    # Instance attributes with class defaults
-    metavar: str = None
-    nargs: Nargs = Nargs(1)                         # Set in subclasses
-    type: Optional[Callable[[str], T_co]] = None    # Only set here if not set by __init__ in Option/Positional
-    show_default: bool = None
-    allow_leading_dash: AllowLeadingDash = AllowLeadingDash.NUMERIC  # Set in some subclasses
+    nargs = Nargs(0)
+    type = staticmethod(str_to_bool)  # Without staticmethod, this would be interpreted as a normal method
+    use_env_value: bool = False
+    _opt_str_cls = TriFlagOptionStrings
+    option_strs: TriFlagOptionStrings
+    alt_help: OptStr = None
+    default: TD
+    consts: Tuple[TC, TA]
 
-    def __init_subclass__(
-        cls, accepts_values: bool = None, accepts_none: bool = None, repr_attrs: Collection[str] = None, **kwargs
-    ):
-        """
-        :param accepts_values: Indicates whether a given subclass of Parameter accepts values, or not.  :class:`.Flag`
-          is an example of a class that does not accept values.
-        :param accepts_none: Indicates whether a given subclass of Parameter accepts being specified without a value,
-          like :class:`.Flag` and :class:`.Counter`.
-        :param repr_attrs: Additional attributes to include in the repr.
-        """
-        super().__init_subclass__(**kwargs)
-        actions = set(cls._actions)  # Inherit actions from parent
-        actions.update(getattr(cls, '_BasicActionMixin__actions', ()))  # Inherit from mixin, if present
-        try:
-            actions.update(getattr(cls, f'_{cls.__name__}__actions'))
-        except AttributeError:
-            pass
-        else:
-            delattr(cls, f'_{cls.__name__}__actions')
-        cls._actions = frozenset(actions)
-        if accepts_values is not None:
-            cls.accepts_values = accepts_values
-        if accepts_none is not None:
-            cls.accepts_none = accepts_none
-        if repr_attrs is not None:
-            cls._repr_attrs = repr_attrs
-
-    def __init__(  # pylint: disable=R0913
+    def __init__(
         self,
-        action: str,
-        name: str = None,
-        default: Any = _NotSet,
-        required: Bool = False,
-        metavar: str = None,
-        help: str = None,  # noqa
-        hide: Bool = False,
-        show_default: Bool = None,
+        *option_strs: str,
+        consts: Tuple[TC, TA] = (True, False),
+        alt_prefix: str = None,
+        alt_long: str = None,
+        alt_short: str = None,
+        alt_help: str = None,
+        action: ConstAct = 'store_const',
+        default: TD = _NotSet,
+        type: TypeFunc = None,  # noqa
+        **kwargs,
     ):
-        if action not in self._actions:
-            raise ParameterDefinitionError(
-                f'Invalid {action=} for {self.__class__.__name__} - valid actions: {sorted(self._actions)}'
-            )
-        if required and default is not _NotSet:
+        if alt_short and '-' in alt_short[1:]:
+            raise ParameterDefinitionError(f"Bad alt_short option - may not contain '-': {alt_short}")
+        elif alt_prefix and ('=' in alt_prefix or alt_prefix.startswith('-')):
+            raise ParameterDefinitionError(f"Bad alt_prefix - may not contain '=' or start with '-': {alt_prefix}")
+        elif not alt_prefix and not alt_long:
+            alt_prefix = 'no'
+
+        try:
+            _pos, _neg = consts
+        except (ValueError, TypeError) as e:
+            msg = f'Invalid {consts=} - expected a 2-tuple of (positive, negative) constants to store'
+            raise ParameterDefinitionError(msg) from e
+
+        if default is _NotSet and not kwargs.get('required', False):
+            default = None
+        if default in consts:
             raise ParameterDefinitionError(
-                f'Invalid combination of required=True with {default=} for {self.__class__.__name__} -'
-                ' required Parameters cannot have a default value'
+                f'Invalid {default=} with {consts=} - the default must not match either value'
             )
-        super().__init__(name=name, required=required, help=help, hide=hide)
-        self.action = action
-        self.default = None if default is _NotSet and not required and self.nargs.max == 1 else default
-        self.metavar = metavar
-        if show_default is not None:
-            self.show_default = show_default
 
-    def _init_value_factory(self):
-        return _NotSet
+        alt_opt_strs = (opt for opt in (alt_short, alt_long) if opt)
+        super().__init__(*option_strs, *alt_opt_strs, action=action, default=default, **kwargs)
+        self.consts = consts
+        self.option_strs.add_alts(alt_prefix, alt_long, alt_short)
+        if alt_help:
+            self.alt_help = alt_help
+        if type is not None:
+            self.type = type
 
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
-        type_attr = self.type
-        choices = isinstance(type_attr, (ChoiceMapInput, Choices)) and type_attr.type is None
-        if (
-            not (choices or type_attr is None)
-            or not self._config(command).allow_annotation_type
-            or self.nargs.max is REMAINDER
-        ):
-            return
+        self.option_strs.update_alts(name)
 
-        if (annotated_type := get_descriptor_value_type(command, name)) is None:
-            return
-        elif choices:
-            type_attr.type = annotated_type
-        else:  # self.type must be None
-            # Choices present earlier would have already been converted
-            self.type = normalize_input_type(annotated_type, None)
-
-    @property
-    def has_choices(self) -> bool:
-        type_attr = self.type
-        return isinstance(type_attr, _ChoicesBase) and type_attr.choices
-
-    # endregion
-
-    def __repr__(self) -> str:
-        attr_names = ('action', 'const', 'default', 'type', 'choices', 'required', 'hide', 'help')
-        if extra_attrs := self._repr_attrs:
-            attr_names = chain(attr_names, extra_attrs)
-
-        attrs = ((a, getattr(self, a, None)) for a in attr_names)
-        kwargs = ', '.join(f'{a}={v!r}' for a, v in attrs if v not in (None, _NotSet) and not (a == 'hide' and not v))
-        return f'{self.__class__.__name__}({self.name!r}, {kwargs})'
-
-    # region Argument Handling
-
-    @overload
-    def __get__(self: Param, command: None, owner: CommandCls) -> Param:
-        ...
-
-    @overload
-    def __get__(self, command: CommandObj, owner: CommandCls) -> Optional[T_co]:
-        ...
-
-    def __get__(self, command, owner):
-        if command is None:
-            return self
-
-        with self._ctx(command):
-            value = self.result()
-
-        if (name := self._name) is not None:
-            command.__dict__[name] = value  # Skip __get__ on subsequent accesses
-        return value
-
-    def _get_parsed_and_max_reached(self) -> Tuple[List[T_co], bool]:
-        parsed = ctx.get_parsed_value(self)
-        try:
-            nargs_max_reached = len(parsed) >= self.nargs.max
-        except TypeError:  # None or REMAINDER
-            nargs_max_reached = False
-        return parsed, nargs_max_reached
-
-    def take_action(
-        self, value: Optional[str], short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
-    ):
-        ctx.record_action(self)
-        return getattr(self, self.action)(self.prepare_and_validate(value, short_combo))
+    def get_const(self, opt_str: OptStr = None) -> Union[TC, TA]:
+        if opt_str in self.option_strs.alt_allowed:
+            return self.consts[1]
+        else:
+            return self.consts[0]
 
-    def would_accept(self, value: str, short_combo: bool = False) -> bool:
-        action = self.action
-        if action in {'store', 'store_all'} and ctx.get_parsed_value(self) is not _NotSet:
-            return False
-        elif action == 'append' and self._get_parsed_and_max_reached()[1]:
-            return False
-        try:
-            normalized = self.prepare_value(value, short_combo, True)
-        except BadArgument:
-            return False
-        return self.is_valid_arg(normalized)
-
-    def prepare_and_validate(self, value: str, short_combo: bool = False) -> T_co:
-        """Called by :meth:`.take_action` to prepare/validate the value before it is passed to the action method."""
-        if value is not None:
-            value = self.prepare_value(value, short_combo)
-        self.validate(value)
-        return value
-
-    def prepare_value(  # pylint: disable=W0613
-        self, value: str, short_combo: bool = False, pre_action: bool = False
-    ) -> T_co:
-        type_func = self.type
-        if type_func is None or (pre_action and isinstance(type_func, InputType) and type_func.is_valid_type(value)):
-            return value
+    def get_env_const(self, value: str, env_var: str) -> Tuple[Union[TC, TA, TD], bool]:
         try:
-            return type_func(value)
-        except InvalidChoiceError as e:
-            raise InvalidChoice(self, e.invalid, e.choices) from e
-        except InputValidationError as e:
-            raise BadArgument(self, str(e)) from e
-        except (TypeError, ValueError) as e:
-            raise BadArgument(self, f'bad {value=} for type={type_func!r}: {e}') from e
+            parsed = self.type(value)
         except Exception as e:
-            raise BadArgument(self, f'unable to cast {value=} to type={type_func!r}') from e
-
-    def validate(self, value: Optional[T_co]):
-        if isinstance(value, str) and value.startswith('-'):
-            if self.allow_leading_dash == AllowLeadingDash.NUMERIC:
-                if len(value) > 1 and not _is_numeric(value):
-                    raise BadArgument(self, f'invalid {value=}')
-            elif self.allow_leading_dash == AllowLeadingDash.NEVER:
-                raise BadArgument(self, f'invalid {value=}')
-        elif value is None:
-            if not self.accepts_none:
-                raise MissingArgument(self)
-        elif not self.accepts_values:
-            raise BadArgument(self, f'does not accept values, but {value=} was provided')
-
-    def is_valid_arg(self, value: Any) -> bool:
-        try:
-            self.validate(value)
-        except (InvalidChoice, BadArgument, MissingArgument):
-            return False
+            raise ParamUsageError(self, f'unable to parse {value=} from {env_var=}: {e}') from e
+        if self.use_env_value:
+            if parsed not in self.consts and parsed != self.default:
+                raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
+            return parsed, True
         else:
-            return True
-
-    def _fix_default(self, value) -> Optional[T_co]:
-        type_func = self.type
-        if type_func is not None and isinstance(type_func, InputType):
-            return type_func.fix_default(value)
-        return value
-
-    def _fix_default_collection(self, values) -> Optional[T_co]:
-        type_func = self.type
-        if type_func is None or not isinstance(type_func, InputType) or not isinstance(values, (list, tuple, set)):
-            return values
-        return values.__class__(map(type_func.fix_default, values))
-
-    def result_value(self) -> Optional[T_co]:
-        if (value := ctx.get_parsed_value(self)) is _NotSet:
-            if self.required:
-                raise MissingArgument(self)
-            else:
-                return self._fix_default(self.default)
-
-        if self.action == 'store':
-            return value
+            const = self.consts[0] if parsed else self.consts[1]
+            return const, True
 
-        # action == 'append' or 'store_all'
-        if not value:
-            if (default := self.default) is not _NotSet:
-                if isinstance(default, Collection) and not isinstance(default, str):
-                    value = self._fix_default_collection(default)
-                else:
-                    value.append(self._fix_default(default))
 
-        nargs = self.nargs
-        if (val_count := len(value)) == 0 and 0 not in nargs:
-            if self.required:
-                raise MissingArgument(self)
-        elif val_count not in nargs:
-            raise BadArgument(self, f'expected {nargs=} values but found {val_count}')
+# region Action Flag
 
-        return value
 
-    result = result_value
-
-    def can_pop_counts(self) -> List[int]:  # noqa
-        return []
-
-    def pop_last(self, count: int = 1) -> List[str]:
-        raise UnsupportedAction
+class ActionFlag(Flag, repr_attrs=('order', 'before_main')):
+    """
+    A :class:`.Flag` that triggers the execution of a function / method / other callable when specified.
 
-    # endregion
+    :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
+      then one will automatically be added based on the name assigned to this parameter.
+    :param order: The priority / order in which this ActionFlag should be executed, relative to other ActionFlags, if
+      others would also be executed.  Two ActionFlags in a given :class:`.Command` may not have the same combination
+      of ``before_main`` and ``order`` values.  ActionFlags with lower ``order`` values are executed before those with
+      higher values.  The ``--help`` action is implemented as an ActionFlag with ``order=float('-inf')``.
+    :param func: The function to execute when this parameter is specified.
+    :param before_main: Whether this ActionFlag should be executed before the :meth:`.Command.main` method or
+      after it.
+    :param always_available: Whether this ActionFlag should always be available to be called, even if parsing
+      failed.  Only allowed when ``before_main=True``.  The intended use case is for actions like ``--help`` text.
+    :param kwargs: Additional keyword arguments to pass to :class:`.Flag`.
+    """
 
-    # region Usage / Help Text
+    def __init__(
+        self,
+        *option_strs: str,
+        order: Union[int, float] = 1,
+        func: Callable = None,
+        before_main: Bool = True,  # noqa  # pylint: disable=W0621
+        always_available: Bool = False,
+        **kwargs,
+    ):
+        expected = {'action': 'store_const', 'default': False, 'const': _NotSet}
+        if bad := {k: fv for k, ev in expected.items() if (fv := kwargs.setdefault(k, ev)) != ev}:
+            raise ParameterDefinitionError(f'Unsupported kwargs for {self.__class__.__name__}: {bad}')
+        elif always_available and not before_main:
+            raise ParameterDefinitionError('always_available=True cannot be combined with before_main=False')
+        super().__init__(*option_strs, **kwargs)
+        self.func = func
+        self.order = order
+        self.before_main = before_main
+        self.always_available = always_available
 
     @property
-    def show_in_help(self) -> bool:
-        if self.hide:
-            return False
-        elif self.group is not None:
-            return self.group.show_in_help
-        return True
-
-    # endregion
-
-
-class BasicActionMixin:
-    action: str
-    nargs: Nargs
-    type: Optional[Callable]
-
-    def _init_value_factory(self):
-        if self.action == 'append':
-            return []
-        return super()._init_value_factory()  # noqa
-
-    @parameter_action
-    def store(self: Parameter, value: T_co):
-        if (prev := ctx.get_parsed_value(self)) is not _NotSet:
-            raise ParamUsageError(self, f'can only be specified once - found multiple values: {prev!r}, {value!r}')
-        ctx.set_parsed_value(self, value)
-
-    @parameter_action
-    def append(self: Parameter, value: T_co):
-        parsed, nargs_max_reached = self._get_parsed_and_max_reached()
-        if nargs_max_reached:
-            raise ParamUsageError(
-                self, f'cannot accept any additional args with nargs={self.nargs} - already found {len(parsed)} values'
-            )
-        parsed.append(value)
-
-    def _pre_pop_values(self: Parameter):
-        if self.action != 'append' or not self.nargs.variable or self.type not in (None, str):
-            return []
+    def func(self):
+        return self._func
 
-        return ctx.get_parsed_value(self)
+    @func.setter
+    def func(self, func: Optional[Callable]):
+        self._func = func
+        if func is not None:
+            if self.help is None:
+                try:
+                    self.help = func.__doc__
+                except AttributeError:
+                    pass
+            update_wrapper(self, func)
 
-    def can_pop_counts(self) -> List[int]:
-        if not (values := self._pre_pop_values()):
-            return []
-
-        n_values = len(values)
-        return [i for i in range(1, n_values) if self.nargs.satisfied(n_values - i)]
-
-    def _reset(self: Union[Parameter, BasicActionMixin]) -> List[str]:
-        if self.action != 'append' or self.type not in (None, str):
-            raise UnsupportedAction
+    def __hash__(self) -> int:
+        result = hash(self.__class__)
+        for attr in (self.name, self.command, self.func, self.order, self.before_main):
+            result ^= hash(attr)
+        return result
+
+    def __eq__(self, other: ActionFlag) -> bool:
+        if not isinstance(other, ActionFlag):
+            return NotImplemented
+        return all(getattr(self, a) == getattr(other, a) for a in ('name', 'func', 'command', 'order', 'before_main'))
+
+    def __lt__(self, other: ActionFlag) -> bool:
+        if not isinstance(other, ActionFlag):
+            return NotImplemented
+        # noinspection PyTypeChecker
+        return (not self.before_main, self.order, self.name) < (not other.before_main, other.order, other.name)
 
-        if not (values := ctx.get_parsed_value(self)):
-            return values
+    def __call__(self, func: Callable) -> ActionFlag:
+        """
+        Allows use as a decorator on the method to be called.  A given method can only be decorated with one ActionFlag.
 
-        ctx.set_parsed_value(self, self._init_value_factory())
-        ctx._provided[self] = 0
-        return values
+        If stacking :class:`.Action` and :class:`.ActionFlag` decorators, the Action decorator must be first (i.e., the
+        ActionFlag decorator must be above the Action decorator).
+        """
+        if self.func is not None:
+            raise CommandDefinitionError(f'Cannot re-assign the func to call for {self}')
+        self.func = func
+        return self
 
-    def pop_last(self: Union[Parameter, BasicActionMixin], count: int = 1) -> List[str]:
-        values = self._pre_pop_values()
-        if not values or count >= len(values) or not self.nargs.satisfied(len(values) - count):
-            raise UnsupportedAction
+    def __get__(self, command: Optional[CommandObj], owner: CommandCls) -> Union[ActionFlag, Callable]:
+        # Allow the method to be called, regardless of whether it was specified
+        if command is None:
+            return self
+        return partial(self.func, command)  # imitates a bound method
 
-        ctx.set_parsed_value(self, values[:-count])
-        ctx.record_action(self, -count)
-        return values[-count:]
+    def result(self) -> Optional[Callable]:
+        if self.result_value():
+            if func := self.func:
+                return func
+            raise ParameterDefinitionError(f'No function was registered for {self}')
+        return None
 
-    def _validate_nargs_and_allow_leading_dash(self, allow_leading_dash: LeadingDash):
-        if allow_leading_dash is not None:
-            allow_leading_dash = AllowLeadingDash(allow_leading_dash)
 
-        if self.nargs.max is REMAINDER:
-            if self.type is not None:
-                raise ParameterDefinitionError(f'Type casting and choices are not supported with nargs={self.nargs!r}')
-            elif allow_leading_dash not in (None, AllowLeadingDash.ALWAYS):
-                raise ParameterDefinitionError(
-                    f'With nargs={self.nargs!r}, only allow_leading_dash=AllowLeadingDash.ALWAYS is supported - found:'
-                    f' {allow_leading_dash!r}'
-                )
-            allow_leading_dash = AllowLeadingDash.ALWAYS
+#: Alias for :class:`ActionFlag`
+action_flag = ActionFlag  # pylint: disable=C0103
 
-        if allow_leading_dash is not None:
-            self.allow_leading_dash = allow_leading_dash
 
+def before_main(*option_strs: str, order: Union[int, float] = 1, func: Callable = None, **kwargs) -> ActionFlag:
+    """An ActionFlag that will be executed before :meth:`.Command.main`"""
+    return ActionFlag(*option_strs, order=order, func=func, before_main=True, **kwargs)
 
-class BasePositional(Parameter[T_co], ABC):
-    """
-    Base class for :class:`.Positional`, :class:`.SubCommand`, :class:`.Action`, and any other parameters that are
-    provided positionally, without prefixes.  It is not meant to be used directly.
 
-    All positional parameters are required by default.
+def after_main(*option_strs: str, order: Union[int, float] = 1, func: Callable = None, **kwargs) -> ActionFlag:
+    """An ActionFlag that will be executed after :meth:`.Command.main`"""
+    return ActionFlag(*option_strs, order=order, func=func, before_main=False, **kwargs)
 
-    Custom positional parameter classes should extend this class to be treated the same as other positionals by the
-    parser.
 
-    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
-      that extend Parameter, and must be registered via :class:`parameter_action`.
-    :param kwargs: Additional keyword arguments to pass to :class:`Parameter`.
-    """
+@action_flag(
+    '--help', '-h', order=float('-inf'), name='help', always_available=True, help='Show this help message and exit'
+)
+def help_action(self):
+    """The ``--help`` / ``-h`` action.  Prints help text, then exits."""
+    cls = self.__class__
+    print(cls.__class__.params(cls).formatter.format_help())
+    raise ParserExit
 
-    _default_ok: bool = False
 
-    def __init_subclass__(cls, default_ok: bool = None, **kwargs):  # pylint: disable=W0222
-        """
-        :param default_ok: Whether default values are supported for this Parameter type
-        :param kwargs: Additional keyword arguments to pass to :meth:`.Parameter.__init_subclass__`.
-        """
-        super().__init_subclass__(**kwargs)
-        if default_ok is not None:
-            cls._default_ok = default_ok
-
-    def __init__(self, action: str, *, required: Bool = True, default: Any = _NotSet, **kwargs):
-        default_bad = not self._default_ok or 0 not in self.nargs
-        if not required and default_bad:
-            cls_name = self.__class__.__name__
-            raise ParameterDefinitionError(f'All {cls_name} parameters must be required - invalid {required=}')
-        elif default_bad and default is not _NotSet:
-            cls_name = self.__class__.__name__
-            raise ParameterDefinitionError(f"The 'default' arg is not supported for {cls_name} parameters")
-        super().__init__(action, default=default, required=required, **kwargs)
+# endregion
 
 
-class BaseOption(Parameter[T_co], ABC):
+class Counter(BaseOption[int], actions=(Count,)):
     """
-    Base class for :class:`.Option`, :class:`.Flag`, :class:`.Counter`, and any other keyword-like parameters that have
-    ``--long`` and ``-short`` prefixes before values.
-
-    Only the handling for processing long/short options and formatting usage of these parameters is provided in this
-    class - it is not meant to be used directly.
-
-    Custom option classes should extend this class to be treated the same as other options by the parser.
+    A :class:`.Flag`-like option that counts the number of times it was specified.  Supports an optional integer value
+    to explicitly increase the stored value by that amount.
 
     :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
       then one will automatically be added based on the name assigned to this parameter.
-    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
-      that extend Parameter, and must be registered via :class:`parameter_action`.
-    :param name_mode: Override the configured :ref:`configuration:Parsing Options:option_name_mode` for this
-      Option/Flag/Counter/etc.
-    :param env_var: A string or sequence (tuple, list, etc) of strings representing environment variables that should
-      be searched for a value when no value was provided via CLI.  If a value was provided via CLI, then these variables
-      will not be checked.  If multiple env variable names/keys were provided, then they will be checked in the order
-      that they were provided.  When enabled, values from env variables take precedence over the default value.  When
-      enabled and the Parameter is required, then either a CLI value or an env var value must be provided.
-    :param kwargs: Additional keyword arguments to pass to :class:`Parameter`.
+    :param action: The action to take on individual parsed values.  Defaults to ``append``, and no other actions
+      are supported (unless this class is extended).
+    :param init: The initial value that will be incremented when this parameter is specified.  Defaults to ``0``.
+    :param default: The default value for this parameter if it is not specified.  Defaults to ``0`` unless this
+      Parameter is required.
+    :param const: The value by which the stored value should increase whenever this parameter is specified.
+      Defaults to ``1``.  If a different ``const`` value is used, and if an explicit value is provided by a user,
+      the user-provided value will be added verbatim - it will NOT be multiplied by ``const``.
+    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
     """
 
-    _opt_str_cls: Type[OptionStrings] = OptionStrings
-    option_strs: OptionStrings
-    env_var: OptStrs = None
+    type = int
+    nargs = Nargs('?')
+    init: int
+    default: int
+    const: int
 
     def __init__(
         self,
         *option_strs: str,
-        action: str,
-        name_mode: Union[OptionNameMode, str, None] = _NotSet,
-        env_var: OptStrs = None,
+        action: str = 'count',
+        init: int = 0,
+        const: int = 1,
+        default: int = _NotSet,
+        required: bool = False,
         **kwargs,
     ):
-        _validate_opt_strs(option_strs)
-        super().__init__(action, **kwargs)
-        self.option_strs = self._opt_str_cls(option_strs, name_mode)
-        if env_var:
-            self.env_var = env_var
-
-    def __set_name__(self, command: CommandCls, name: str):
-        super().__set_name__(command, name)
-        if not self.option_strs.name_mode:
-            self.option_strs.name_mode = command.__class__.config(command).option_name_mode
-        self.option_strs.update(name)
-
-    def env_vars(self) -> Iterator[str]:
-        if env_var := self.env_var:
-            if isinstance(env_var, str):
-                yield env_var
-            else:
-                yield from env_var
-
-
-def get_active_param_group() -> Optional[ParamGroup]:
-    try:
-        return _group_stack.get()[-1]
-    except (AttributeError, IndexError):
-        return None
+        type_check_vals = {'const': const, 'init': init}
+        if default is not _NotSet:
+            type_check_vals['default'] = default
+        elif not required:
+            default = 0
+        if bad_types := ', '.join(f'{k}={v!r}' for k, v in type_check_vals.items() if not isinstance(v, self.type)):
+            raise ParameterDefinitionError(f'Invalid type for parameters (expected int): {bad_types}')
+        super().__init__(*option_strs, action=action, default=default, required=required, **kwargs)
+        self.init = init
+        self.const = const
 
+    def prepare_value(self, value: Optional[str], short_combo: bool = False, pre_action: bool = False) -> int:
+        try:
+            return self.type(value)
+        except (ValueError, TypeError) as e:
+            combinable = self.option_strs.combinable
+            if short_combo and combinable and all(c in combinable for c in value):
+                return len(value) + 1  # +1 for the -short that preceded this value
+            raise BadArgument(self, f'bad counter {value=}') from e
 
-def _validate_opt_strs(opt_strs: Collection[str]):
-    if bad := ', '.join(opt for opt in opt_strs if not 0 < opt.count('-', 0, 3) < 3 or opt.endswith('-') or '=' in opt):
-        msg = f"Bad option(s) - they must start with '--' or '-', may not end with '-', and may not contain '=': {bad}"
-        raise ParameterDefinitionError(msg)
+    def validate(self, value: Any, joined: Bool = False):
+        if value is None or isinstance(value, self.type):
+            return
+        try:
+            value = self.type(value)
+        except (ValueError, TypeError) as e:
+            raise BadArgument(self, f'invalid {value=} (expected an integer)') from e
+        else:
+            return
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/choice_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 
 from functools import partial
 from string import whitespace, printable
 from typing import Type, TypeVar, Generic, Optional, Callable, Union, Collection, Mapping, NoReturn, Dict
 from types import MethodType
 
 from ..context import ctx
-from ..exceptions import ParameterDefinitionError, BadArgument, MissingArgument, InvalidChoice, CommandDefinitionError
+from ..exceptions import ParameterDefinitionError, BadArgument, InvalidChoice, CommandDefinitionError
 from ..formatting.utils import format_help_entry
 from ..nargs import Nargs
 from ..typing import Bool, CommandCls
 from ..utils import _NotSet, camel_to_snake_case, short_repr
-from .base import BasePositional, parameter_action
+from .actions import Concatenate
+from .base import BasePositional
 
 __all__ = ['SubCommand', 'Action', 'Choice', 'ChoiceMap']
 
 T = TypeVar('T')
+TD = TypeVar('TD')
 OptStr = Optional[str]
 # TODO: Combine SubCommand and Action, replacing `local_choices` with stackable decorators on the target method,
 #  optionally injecting the selected choice into positional args for the decorated method, which may be main?
 
 
 class Choice(Generic[T]):
     """
@@ -50,15 +52,15 @@
         return '(default)' if self.choice is None else self.choice
 
     def format_help(self, lpad: int = 4, tw_offset: int = 0, prefix: str = '') -> str:
         # Note: no longer called by formatters
         return format_help_entry((self.format_usage(),), self.help, prefix, tw_offset, lpad=lpad)
 
 
-class ChoiceMap(BasePositional[str], Generic[T]):
+class ChoiceMap(BasePositional[str], Generic[T], actions=(Concatenate,)):
     """
     Base class for :class:`SubCommand` and :class:`Action`.  It is not meant to be used directly.
 
     Allows choices to be defined and provided as a string that may contain spaces, without requiring users to escape or
     quote the string (i.e., as technically separate arguments).  This allows for a more natural way to provide
     multi-word commands, without needing to jump through hoops to handle them.
 
@@ -90,23 +92,20 @@
         """
         super().__init_subclass__(**kwargs)
         if title is not None:
             cls._default_title = title
         if choice_validation_exc is not None:
             cls._choice_validation_exc = choice_validation_exc
 
-    def __init__(self, *, action: str = 'append', title: str = None, description: str = None, **kwargs):
+    def __init__(self, *, action: str = 'concatenate', title: str = None, description: str = None, **kwargs):
         super().__init__(action=action, **kwargs)
         self.title = title
         self.description = description
         self.choices = {}
 
-    def _init_value_factory(self):
-        return []
-
     # region Choice Registration
 
     @property
     def has_choices(self) -> bool:
         return bool(self.choices)
 
     def _update_nargs(self):
@@ -147,56 +146,37 @@
     def _no_choices_error(self) -> NoReturn:
         raise CommandDefinitionError(f'No choices were registered for {self}')
 
     # endregion
 
     # region Argument Handling
 
-    @parameter_action
-    def append(self, value: str):
-        values = value.split()
-        if not self.is_valid_arg(' '.join(values)):
-            raise InvalidChoice(self, value, self.choices)
-
-        ctx.get_parsed_value(self).extend(values)
-        n_values = len(values)
-        ctx.record_action(self, n_values - 1)  # - 1 because it was already called before dispatching to this method
-        return n_values
-
-    def validate(self, value: str):
+    def validate(self, value: str, joined: Bool = False):
         if not (choices := self.choices):
             self._no_choices_error()
 
-        values = (*ctx.get_parsed_value(self), value)
+        parsed = ctx.get_parsed_value(self)
+        values = (value,) if parsed is _NotSet else (*parsed, value)
         if (choice := ' '.join(values)) in choices:
             return
         elif len(values) > self.nargs.max:
             raise BadArgument(self, 'too many values')
         prefix = choice + ' '
         if not any(c.startswith(prefix) for c in choices if c):
             raise InvalidChoice(self, prefix[:-1], choices)
 
-    def result_value(self) -> OptStr:
-        if not (choices := self.choices):
+    def result_value(self, missing_default: TD = _NotSet) -> Union[OptStr, TD]:
+        if not self.choices:
             self._no_choices_error()
-        if not (values := ctx.get_parsed_value(self)):
-            if None in choices:
-                return None
-            raise MissingArgument(self)
-        if (val_count := len(values)) not in self.nargs:
-            raise BadArgument(self, f'expected nargs={self.nargs} values but found {val_count}')
-        if (choice := ' '.join(values)) not in choices:
-            raise InvalidChoice(self, choice, choices)
-        return choice
+        return super().result_value(missing_default)
 
     result = result_value
 
     def target(self) -> T:
-        choice = self.result_value()
-        return self.choices[choice].target
+        return self.choices[self.result_value()].target
 
     # endregion
 
     # region Usage / Help Text
 
     @property
     def show_in_help(self) -> bool:
@@ -235,14 +215,15 @@
         :param kwargs: Additional keyword arguments to pass to :class:`ChoiceMap`.
         """
         super().__init__(**kwargs)
         self.required = required
         if not required:
             # This results in next_cmd=None in parse_args, so the base cmd will run
             self._register_choice(None, None, default_help)
+            self.default = None
         if local_choices:
             self._register_local_choices(local_choices)
 
     @property
     def has_local_choices(self) -> bool:
         return None in self.choices or any(c.target is None for c in self.choices.values())
 
@@ -266,14 +247,15 @@
         except CommandDefinitionError:
             from ..core import get_parent
 
             parent = get_parent(command)
             msg = f'Invalid {choice=} for {command} with {parent=} - already assigned to {self.choices[choice].target}'
             raise CommandDefinitionError(msg) from None
 
+        command._is_subcommand_ = True  # This is used indirectly by ``main()`` to filter out non-top-level Commands
         return command
 
     def register(
         self, command_or_choice: Union[str, CommandCls] = None, *, choice: str = None, help: str = None  # noqa
     ) -> Callable[[CommandCls], CommandCls]:
         """
         Class decorator version of :meth:`.register_command`.  Registers the wrapped :class:`.Command` as the
@@ -324,14 +306,16 @@
 
         if default:
             if help is None:
                 help = 'Default action if no other action is specified'  # noqa
             if choice:  # register both the explicit and the default choices
                 self.register_choice(choice, method, help)
             self._register_choice(None, method, help)
+            self.default = None
+            self.required = False
         else:
             self.register_choice(choice or method.__name__, method, help)
 
         return method
 
     def register(
         self,
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,18 @@
     # region Active Group Methods
 
     def __enter__(self) -> ParamGroup:
         """
         A ParamGroup can be used as a context manager, where all Parameters (and ParamGroups) defined inside the
         ``with`` block will be registered as members of that group.
         """
-        _group_stack.get().append(self)
+        try:
+            _group_stack.get().append(self)
+        except LookupError:
+            _group_stack.set([self])
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         _group_stack.get().pop()
 
     # endregion
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/option_strings.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 if TYPE_CHECKING:
     from ..typing import Bool
 
 __all__ = ['OptionStrings', 'TriFlagOptionStrings']
 
 
 class OptionStrings:
+    """Container for the option strings registered for a given BaseOption (or subclass thereof)."""
+
     __slots__ = ('name_mode', '_long', '_short', 'combinable', '_display_long')
     name_mode: Optional[OptionNameMode]
     combinable: Set[str]
     _display_long: Set[str]
     _long: Set[str]
     _short: Set[str]
 
     def __init__(self, option_strs: Collection[str], name_mode: Union[OptionNameMode, str, None] = _NotSet):
         self.name_mode = OptionNameMode(name_mode) if name_mode is not _NotSet else None
-        self._display_long = self._long = {opt for opt in option_strs if opt.startswith('--')}
-        self._short = short_opts = {opt for opt in option_strs if 1 == opt.count('-', 0, 2)}
+        long_opts, short_opts = _split_options(option_strs)
+        self._display_long = self._long = long_opts
+        self._short = short_opts
         self.combinable = {opt[1:] for opt in short_opts if len(opt) == 2}
-        if bad_opts := ', '.join(opt for opt in short_opts if '-' in opt[1:]):
-            raise ParameterDefinitionError(f"Bad short option(s) - may not contain '-': {bad_opts}")
 
     def __repr__(self) -> str:
         options = ', '.join(self.all_option_strs())
         return f'<{self.__class__.__name__}[name_mode={self.name_mode}][{options}]>'
 
     def has_long(self) -> Bool:
         """Whether any (primary / non-alternate, for TriFlag) long option strings were defined"""
@@ -64,37 +65,42 @@
                 self._display_long.add(option)
         if mode & OptionNameMode.UNDERSCORE:
             option = f'--{name}'
             self._long.add(option)
             if mode_val & 8:  # OptionNameMode.BOTH_UNDERSCORE = OptionNameMode.DASH | 4 | 8
                 self._display_long.add(option)
 
+    def get_sets(self) -> Tuple[Set[str], Set[str]]:
+        return self._long, self._short
+
     @property
     def long(self) -> List[str]:
-        return _sort_options(self._long)
+        return sorted(self._long, key=_options_sort_key)
 
     @property
     def short(self) -> List[str]:
-        return _sort_options(self._short)
+        return sorted(self._short, key=_options_sort_key)
 
     @property
     def display_long(self) -> List[str]:
-        return _sort_options(self._display_long)
+        return sorted(self._display_long, key=_options_sort_key)
 
     def get_usage_opt(self) -> str:
         return next(self.option_strs())
 
     def option_strs(self) -> Iterator[str]:
         yield from self.display_long
         yield from self.short
 
     all_option_strs = option_strs
 
 
 class TriFlagOptionStrings(OptionStrings):
+    """Container for the option strings registered for a given TriFlag."""
+
     __slots__ = ('_alt_prefix', '_alt_long', '_alt_short')
     _alt_prefix: Optional[str]
     _alt_short: Optional[str]
     _alt_long: Union[Set[str], Tuple[str]]
 
     def has_long(self) -> Bool:
         """Whether any primary / non-alternate long option strings were defined"""
@@ -148,15 +154,15 @@
 
     @property
     def short_primary(self) -> List[str]:
         return [opt for opt in self.short if opt != self._alt_short]
 
     # @property
     # def long_alt(self) -> List[str]:
-    #     return _sort_options(self._alt_long)
+    #     return sorted(self._alt_long, key=_options_sort_key)
 
     @property
     def display_long_alt(self) -> List[str]:
         return [opt for opt in self.display_long if opt in self._alt_long]
 
     @property
     def short_alt(self) -> List[str]:
@@ -180,9 +186,38 @@
             yield from self.primary_option_strs()
 
     def all_option_strs(self) -> Iterator[str]:
         yield from self.option_strs(False)
         yield from self.option_strs(True)
 
 
-def _sort_options(options: Collection[str]):
-    return sorted(options, key=lambda opt: (-len(opt), opt))
+def _options_sort_key(opt: str):
+    """Used to sort option strings in descending length order (alphanumeric order for options with the same length)"""
+    return -len(opt), opt
+
+
+def _split_options(opt_strs: Collection[str]) -> Tuple[Set[str], Set[str]]:
+    """Split long and short option strings and ensure that all of the provided option strings are valid."""
+    long_opts, short_opts, bad_opts, bad_short = set(), set(), [], []
+    for opt in opt_strs:
+        if not opt:     # Ignore None / empty strings / etc
+            continue    # Only raise an exception if invalid values that were intended to be used were provided
+        elif not 0 < opt.count('-', 0, 3) < 3 or opt.endswith('-') or '=' in opt:
+            bad_opts.append(opt)
+        elif opt.startswith('--'):
+            long_opts.add(opt)
+        elif '-' in opt[2:]:
+            bad_short.append(opt)
+        else:
+            short_opts.add(opt)
+
+    if bad_opts:
+        bad = ', '.join(map(repr, bad_opts))
+        raise ParameterDefinitionError(
+            f"Bad option(s) - they must start with '--' or '-', may not end with '-', and may not contain '=': {bad}"
+        )
+    elif bad_short:
+        raise ParameterDefinitionError(
+            f"Bad short option(s) - they may not contain '-': {', '.join(map(repr, bad_short))}"
+        )
+
+    return long_opts, short_opts
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,531 +1,514 @@
 """
-Optional Parameters
+Base classes and helpers for Parameters and Groups
 
 :author: Doug Skrypa
 """
+# pylint: disable=R0801
 
 from __future__ import annotations
 
-import logging
+import re
 from abc import ABC, abstractmethod
-from functools import partial, update_wrapper
-from typing import TYPE_CHECKING, Any, Optional, Callable, Union, TypeVar, Tuple
-
-from ..context import ctx
-from ..exceptions import ParameterDefinitionError, BadArgument, CommandDefinitionError, ParamUsageError, ParamConflict
-from ..inputs import normalize_input_type
-from ..nargs import Nargs, NargsValue
-from ..typing import T_co, TypeFunc
-from ..utils import _NotSet, ValueSource, str_to_bool
-from .base import BasicActionMixin, BaseOption, parameter_action
-from .option_strings import TriFlagOptionStrings
+from contextvars import ContextVar
+from functools import cached_property
+from itertools import chain
+from typing import TYPE_CHECKING, Any, Type, Generic, Optional, Callable, Collection, Union, Iterator, TypeVar, overload
+from typing import NoReturn, Dict, Tuple
+
+from ..annotations import get_descriptor_value_type
+from ..config import CommandConfig, OptionNameMode, AllowLeadingDash, DEFAULT_CONFIG
+from ..context import Context, ctx, get_current_context
+from ..exceptions import ParameterDefinitionError, BadArgument, MissingArgument, InvalidChoice
+from ..inputs import InputType, normalize_input_type
+from ..inputs.choices import _ChoicesBase
+from ..inputs.exceptions import InputValidationError, InvalidChoiceError
+from ..nargs import Nargs, REMAINDER
+from ..typing import T_co
+from ..utils import _NotSet
+from .option_strings import OptionStrings
 
 if TYPE_CHECKING:
-    from ..typing import Bool, ChoicesType, InputTypeFunc, CommandCls, CommandObj, OptStr, ValSrc, LeadingDash
+    from ..formatting.params import ParamHelpFormatter
+    from ..typing import OptStr, OptStrs, Strings, Bool, CommandCls, CommandObj, CommandAny, Param, LeadingDash
+    from .actions import ParamAction
+    from .groups import ParamGroup
 
-__all__ = ['Option', 'Flag', 'TriFlag', 'ActionFlag', 'Counter', 'action_flag', 'before_main', 'after_main']
-log = logging.getLogger(__name__)
+__all__ = ['Parameter', 'BasePositional', 'BaseOption']
 
+_group_stack = ContextVar('cli_command_parser.parameters.base.group_stack')
+_is_numeric = re.compile(r'^-\d+$|^-\d*\.\d+?$').match
 TD = TypeVar('TD')
-TC = TypeVar('TC')
-TA = TypeVar('TA')
 
 
-class Option(BasicActionMixin, BaseOption[T_co]):
+class ParamBase(ABC):
     """
-    A generic option that can be specified as ``--foo bar`` or by using other similar forms.
+    Base class for :class:`Parameter` and :class:`.ParamGroup`.
 
-    :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
-      then one will automatically be added based on the name assigned to this parameter.
-    :param nargs: The number of values that are expected/required when this parameter is specified.  Defaults to 1.
-      See :class:`.Nargs` for more info.
-    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
-      that extend Parameter, and must be registered via :class:`.parameter_action`.  Defaults to ``store`` when
-      ``nargs=1``, and to ``append`` otherwise.  A single value will be stored when ``action='store'``, and a list
-      of values will be stored when ``action='append'``.
-    :param default: The default value for this parameter if it is not specified.  Defaults to ``None`` if
-      this parameter is not required; not used if it is required.
+    :param name: The name to use for this parameter.  Defaults to the name assigned to this parameter.
     :param required: Whether this parameter is required or not.  If it is required, then an exception will be
       raised if the user did not provide a value for this parameter.  Defaults to ``False``.
-    :param type: A callable (function, class, etc.) that accepts a single string argument, which should be called
-      on every value for this parameter to transform the value.  By default, no transformation is performed, and
-      values will be strings.  If not specified, but a type annotation is detected, then that annotation will be
-      used as if it was provided here.  When both are present, this argument takes precedence.
-    :param choices: A container that holds the specific values that users must pick from.  By default, any value is
-      allowed.
-    :param allow_leading_dash: Whether string values may begin with a dash (``-``).  By default, if a value begins with
-      a dash, it is only accepted if it appears to be a negative numeric value.  Use ``True`` / ``always`` /
-      ``AllowLeadingDash.ALWAYS`` to allow any value that begins with a dash (as long as it is not an option string for
-      an Option/Flag/etc).  To reject all values beginning with a dash, including numbers, use ``False`` / ``never`` /
-      ``AllowLeadingDash.NEVER``.
-    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
+    :param help: A brief description of this parameter that will appear in ``--help`` text.
+    :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
     """
 
-    def __init__(
-        self,
-        *option_strs: str,
-        nargs: NargsValue = None,
-        action: str = _NotSet,
-        default: Any = _NotSet,
-        required: Bool = False,
-        type: InputTypeFunc = None,  # noqa
-        choices: ChoicesType = None,
-        allow_leading_dash: LeadingDash = None,
-        **kwargs,
-    ):
-        if nargs is not None:
-            self.nargs = Nargs(nargs)
-        if 0 in self.nargs:
-            details = 'use Flag or Counter for Options with 0 args'
-            if isinstance(nargs, range) and nargs.start == 0 and nargs.step != nargs.stop:
-                suffix = f', {nargs.step}' if nargs.step != 1 else ''
-                details = f'try using range({nargs.step}, {nargs.stop}{suffix}) instead, or {details}'
-            raise ParameterDefinitionError(f'Invalid {nargs=} - {details}')
-        if action is _NotSet:
-            action = 'store' if self.nargs == 1 else 'append'
-        elif action == 'store' and self.nargs != 1:
-            raise ParameterDefinitionError(f'Invalid nargs={self.nargs} for {action=}')
-        super().__init__(*option_strs, action=action, default=default, required=required, **kwargs)
-        self.type = normalize_input_type(type, choices)
-        self._validate_nargs_and_allow_leading_dash(allow_leading_dash)
-
-
-class _Flag(BaseOption[T_co], ABC):
-    nargs = Nargs(0)
-    type = staticmethod(str_to_bool)  # Without staticmethod, this would be interpreted as a normal method
-    strict_env: bool
-    use_env_value: bool = False
-    _use_opt_str: bool = False
+    # Class Attributes
+    missing_hint: str = None        #: Hint to provide if this param/group is missing
+    # Instance Attributes
+    _attr_name: str = None          #: Always the name of the attr that points to this object
+    _name: str = None               #: An explicitly provided name, or the name of the attr that points to this object
+    group: ParamGroup = None        #: The group this object is a member of, if any
+    command: CommandCls = None      #: The :class:`.Command` this object is a member of
+    required: Bool                  #: Whether this param/group is required
+    help: str                       #: The description for this param/group that will appear in ``--help`` text
+    hide: Bool                      #: Whether this param/group should be hidden in ``--help`` text
+
+    def __init__(self, name: str = None, required: Bool = False, help: str = None, hide: Bool = False):  # noqa
+        self.__doc__ = help  # Prevent this class's docstring from showing up for params in generated documentation
+        self.required = required
+        self.help = help
+        self.hide = hide
+        self.name = name
+        if param_groups := _group_stack.get(None):  # If truthy, there's at least 1 active ParamGroup
+            param_groups[-1].register(self)  # This sets self.group = group
 
-    def __init_subclass__(cls, use_opt_str: bool = False, **kwargs):  # pylint: disable=W0222
-        super().__init_subclass__(**kwargs)
-        cls._use_opt_str = use_opt_str
+    # region Name
 
-    def __init__(
-        self,
-        *option_strs: str,
-        type: TypeFunc = None,  # noqa
-        strict_env: bool = True,
-        use_env_value: bool = False,
-        **kwargs,
-    ):
-        if 'metavar' in kwargs:
-            raise TypeError(f"{self.__class__.__name__}.__init__() got an unexpected keyword argument: 'metavar'")
-        super().__init__(*option_strs, **kwargs)
-        self.strict_env = strict_env
-        if use_env_value:
-            self.use_env_value = use_env_value
-        if type is not None:
-            self.type = type
+    @property
+    def name(self) -> str:
+        if (name := self._name) is not None:
+            return name
+        return self._default_name()
+
+    @name.setter
+    def name(self, value: Optional[str]):
+        if value is not None:
+            self._name = value
 
-    def _init_value_factory(self):
-        if self.action == 'store_const':
-            return self.default
-        else:
-            return []
+    def _default_name(self) -> str:
+        return f'{self.__class__.__name__}#{id(self)}'
 
-    def take_action(
-        self, value: Optional[str], short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
-    ):
-        # log.debug(f'{self!r}.take_action({value!r})')
-        ctx.record_action(self)
-        if value is None:
-            action_method = getattr(self, self.action)
-            return action_method(opt_str) if self._use_opt_str else action_method()
-        elif src != ValueSource.CLI:
-            src, env_var = src
-            try:
-                return self.take_env_var_action(value, env_var)
-            except ParamUsageError as e:
-                if not self.strict_env:
-                    log.warning(e)
-                    return
-                raise
+    def __set_name__(self, command: CommandCls, name: str):
+        self.command = command
+        if self._name is None:
+            self._name = name
+        self._attr_name = name
+
+    # endregion
 
-        raise ParamUsageError(self, f'received {value=} but no values are accepted for action={self.action!r}')
+    def __hash__(self) -> int:
+        return hash(self.__class__) ^ hash(self._attr_name) ^ hash(self._name) ^ hash(self.command)
 
-    def prepare_env_var_value(self, value: str, env_var: str) -> T_co:
+    def _ctx(self, command: CommandAny = None) -> Optional[Context]:
+        if context := get_current_context(True):
+            return context
+        if command is None:
+            command = self.command
         try:
-            return self.type(value)
-        except Exception as e:
-            raise ParamUsageError(self, f'unable to parse {value=} from {env_var=}: {e}') from e
+            return command._Command__ctx
+        except AttributeError:
+            return None
+
+    def _config(self, command: CommandAny = None) -> CommandConfig:
+        if context := self._ctx(command):
+            return context.config
+        if command is None:
+            command = self.command
+        return command.__class__.config(command, DEFAULT_CONFIG)
+
+    # region Usage / Help Text
+
+    @cached_property
+    def formatter(self) -> ParamHelpFormatter:
+        from ..formatting.params import ParamHelpFormatter  # Here due to circular dependency
+
+        try:
+            formatter_factory = self._config().param_formatter or ParamHelpFormatter
+        except AttributeError:  # self.command is None
+            formatter_factory = ParamHelpFormatter
 
+        return formatter_factory(self)  # noqa
+
+    @property
     @abstractmethod
-    def take_env_var_action(self, value: str, env_var: str):
+    def show_in_help(self) -> bool:
         raise NotImplementedError
 
-    def would_accept(self, value: Optional[str], short_combo: bool = False) -> bool:  # noqa
-        return value is None
+    def format_usage(self, *args, **kwargs) -> str:
+        """Convenience method for calling :meth:`.ParamHelpFormatter.format_usage`"""
+        return self.formatter.format_usage(*args, **kwargs)
 
-    def result_value(self) -> Any:
-        return ctx.get_parsed_value(self)
+    def format_help(self, *args, **kwargs) -> str:
+        """Convenience method for calling :meth:`.ParamHelpFormatter.format_help`"""
+        return self.formatter.format_help(*args, **kwargs)
 
-    result = result_value
+    # endregion
 
 
-class Flag(_Flag[Union[TD, TC]], accepts_values=False, accepts_none=True):
+class Parameter(ParamBase, Generic[T_co], ABC):
     """
-    A (typically boolean) option that does not accept any values.
+    Base class for all other parameters.  It is not meant to be used directly.
+
+    Custom parameter classes should generally extend :class:`BasePositional` or :class:`BaseOption` instead of this,
+    otherwise additional handling may be necessary in the parser.
 
-    :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
-      then one will automatically be added based on the name assigned to this parameter.
     :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
-      that extend Parameter, and must be registered via :class:`.parameter_action`.  Defaults to ``store_const``, but
-      accepts ``append_const`` to build a list of the specified constant.
-    :param default: The default value for this parameter if it is not specified.  Defaults to ``False`` when
-      ``const=True`` (the default), and to ``True`` when ``const=False``.  Defaults to ``None`` for any other
-      constant.
-    :param const: The constant value to store/append when this parameter is specified.  Defaults to ``True``.
-    :param type: A callable (function, class, etc.) that accepts a single string argument and returns a boolean value,
-      which should be called on environment variable values, if any are configured for this Flag via
-      :paramref:`.BaseOption.env_var`.  It should return a truthy value if any action should be taken (i.e., if the
-      constant should be stored/appended), or a falsey value for no action to be taken.  The
-      :func:`default function<.str_to_bool>` handles parsing ``1`` / ``true`` / ``yes`` and similar as ``True``,
-      and ``0`` / ``false`` / ``no`` and similar as ``False``.  If :paramref:`use_env_value` is ``True``, then this
-      function should return either the default or constant value instead.
-    :param strict_env: When ``True`` (the default), if an :paramref:`.BaseOption.env_var` is used as the source of a
-      value for this parameter and that value is invalid, then parsing will fail.  When ``False``, invalid values from
-      environment variables will be ignored (and a warning message will be logged).
-    :param use_env_value: If ``True``, when an :paramref:`.BaseOption.env_var` is used as the source of a value for
-      this Flag, the parsed value will be stored as this Flag's value (it must match either the default or constant
-      value).  If ``False`` (the default), then the parsed value will be used to determine whether this Flag's normal
-      action should be taken as if it was specified via a CLI argument.
-    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
+      that extend Parameter, and must be registered via :class:`parameter_action`.
+    :param name: The name to use for this parameter.  Defaults to the name assigned to this parameter.
+    :param default: The default value for this parameter if it is not specified.  Defaults to ``None`` if this
+      parameter is not required; not used if it is required.
+    :param required: Whether this parameter is required or not.  If it is required, then an exception will be
+      raised if the user did not provide a value for this parameter.  Defaults to ``False``.
+    :param metavar: The name to use as a placeholder for values in usage / help messages.
+    :param help: A brief description of this parameter that will appear in ``--help`` text.
+    :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
+    :param show_default: Override the :attr:`.CommandConfig.show_defaults` setting for this parameter to always or
+      never include the default value in usage / help messages.  Default: follow the ``show_defaults`` setting.
     """
 
-    __default_const_map = {True: False, False: True, _NotSet: True}
-    default: TD
-    const: TC
-
-    def __init__(
-        self, *option_strs: str, action: str = 'store_const', default: TD = _NotSet, const: TC = _NotSet, **kwargs
-    ):
-        if const is _NotSet:
-            try:
-                const = self.__default_const_map[default]
-            except KeyError as e:
-                cls = self.__class__.__name__
-                raise ParameterDefinitionError(f"Missing parameter='const' for {cls} with {default=}") from e
-        if default is _NotSet:
-            default = self.__default_const_map.get(const)  # will be True, False, or None
-        if default is False:  # Avoid surprises for custom non-truthy values
-            kwargs.setdefault('show_default', False)
-        super().__init__(*option_strs, action=action, default=default, **kwargs)
-        self.const = const
-
-    def take_env_var_action(self, value: str, env_var: str):
-        parsed = self.prepare_env_var_value(value, env_var)
-        if self.use_env_value:
-            if parsed == self.const:
-                getattr(self, self.action)()
-            elif parsed != self.default:
-                raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
-        elif parsed:
-            getattr(self, self.action)()
-
-    @parameter_action
-    def store_const(self):
-        ctx.set_parsed_value(self, self.const)
-
-    @parameter_action
-    def append_const(self):
-        ctx.get_parsed_value(self).append(self.const)
-
+    # region Attributes & Initialization
 
-class TriFlag(_Flag[Union[TD, TC, TA]], accepts_values=False, accepts_none=True, use_opt_str=True):
-    """
-    A trinary / ternary Flag.  While :class:`.Flag` only supports 1 constant when provided, with 1 default if not
-    provided, this class accepts a pair of constants for the primary and alternate values to store, along with a
-    separate default.
-
-    :param option_strs: The primary long and/or short option prefixes for this option.  If no long prefixes are
-      specified, then one will automatically be added based on the name assigned to this parameter.
-    :param consts: A 2-tuple containing the ``(primary, alternate)`` values to store.  Defaults to ``(True, False)``.
-    :param alt_prefix: The prefix to add to the assigned name for the alternate long form.  Ignored if ``alt_long`` is
-      specified.  Defaults to ``no`` if ``alt_long`` is not specified.
-    :param alt_long: The alternate long form to use.
-    :param alt_short: The alternate short form to use.
-    :param alt_help: The help text to display with the alternate option strings.
-    :param action: The action to take on individual parsed values.  Only ``store_const`` (the default) is supported.
-    :param default: The default value to use if neither the primary or alternate options are provided.  Defaults
-      to None.
-    :param name_mode: Override the configured :ref:`configuration:Parsing Options:option_name_mode` for this TriFlag.
-    :param type: A callable (function, class, etc.) that accepts a single string argument and returns a boolean value,
-      which should be called on environment variable values, if any are configured for this TriFlag via
-      :paramref:`.BaseOption.env_var`.  It should return a truthy value if the primary constant should be stored, or a
-      falsey value if the alternate constant should be stored.  The :func:`default function<.str_to_bool>` handles
-      parsing ``1`` / ``true`` / ``yes`` and similar as ``True``, and ``0`` / ``false`` / ``no`` and similar
-      as ``False``.  If :paramref:`use_env_value` is ``True``, then this function should return the primary or
-      alternate constant or the default value instead.
-    :param strict_env: When ``True`` (the default), if an :paramref:`.BaseOption.env_var` is used as the source of a
-      value for this parameter and that value is invalid, then parsing will fail.  When ``False``, invalid values from
-      environment variables will be ignored (and a warning message will be logged).
-    :param use_env_value: If ``True``, when an :paramref:`.BaseOption.env_var` is used as the source of a value for
-      this TriFlag, the parsed value will be stored as this TriFlag's value (it must match the primary or alternate
-      constant, or the default value).  If ``False`` (the default), then the parsed value will be used to determine
-      whether this TriFlag's normal action should be taken as if it was specified via a CLI argument.
-    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
-    """
+    # Class attributes
+    _action_map: Dict[str, Type[ParamAction]] = {}
+    _repr_attrs: Optional[Strings] = None           #: Attributes to include in ``repr()`` output
+    # Instance attributes with class defaults
+    metavar: str = None
+    nargs: Nargs                                    # Expected to be set in subclasses
+    type: Optional[Callable[[str], T_co]] = None    # Expected to be set in subclasses
+    show_default: Bool = None
+    allow_leading_dash: AllowLeadingDash = AllowLeadingDash.NUMERIC  # Set in some subclasses
+    strict_default: Bool = False
 
-    _opt_str_cls = TriFlagOptionStrings
-    option_strs: TriFlagOptionStrings
-    alt_help: OptStr = None
-    default: TD
-    consts: Tuple[TC, TA]
+    def __init_subclass__(cls, repr_attrs: Strings = None, actions: Collection[Type[ParamAction]] = None, **kwargs):
+        """
+        :param repr_attrs: Additional attributes to include in the repr.
+        :param actions: Collection of ParamAction classes that this type of Parameter supports
+        """
+        super().__init_subclass__(**kwargs)
+        if actions:
+            # Extend the parent class's actions without modifying the parent's supported actions
+            cls._action_map = action_map = cls._action_map.copy()
+            action_map.update((action.name, action) for action in actions)
+        if repr_attrs:
+            cls._repr_attrs = repr_attrs
 
-    def __init__(
+    def __init__(  # pylint: disable=R0913
         self,
-        *option_strs: str,
-        consts: Tuple[TC, TA] = (True, False),
-        alt_prefix: str = None,
-        alt_long: str = None,
-        alt_short: str = None,
-        alt_help: str = None,
-        action: str = 'store_const',
-        default: TD = _NotSet,
-        **kwargs,
+        action: str,
+        name: str = None,
+        default: Any = _NotSet,
+        required: Bool = False,
+        metavar: str = None,
+        help: str = None,  # noqa
+        hide: Bool = False,
+        show_default: Bool = None,
+        strict_default: Bool = False,
     ):
-        if alt_short and '-' in alt_short[1:]:
-            raise ParameterDefinitionError(f"Bad alt_short option - may not contain '-': {alt_short}")
-        elif alt_prefix and ('=' in alt_prefix or alt_prefix.startswith('-')):
-            raise ParameterDefinitionError(f"Bad alt_prefix - may not contain '=' or start with '-': {alt_prefix}")
-        elif not alt_prefix and not alt_long:
-            alt_prefix = 'no'
-
-        try:
-            _pos, _neg = consts
-        except (ValueError, TypeError) as e:
-            msg = f'Invalid {consts=} - expected a 2-tuple of (positive, negative) constants to store'
-            raise ParameterDefinitionError(msg) from e
-
-        if default is _NotSet and not kwargs.get('required', False):
-            default = None
-        if default in consts:
+        if not (param_action := self._action_map.get(action)):
+            self._handle_bad_action(action)
+        if required and default is not _NotSet:
+            # TODO: For required mutually dependent groups, or a required group with all params having a default,
+            #  is another check needed, or does this check make sense, or should this check be removed?
             raise ParameterDefinitionError(
-                f'Invalid {default=} with {consts=} - the default must not match either value'
+                f'Invalid combination of required=True with {default=} for {self.__class__.__name__} -'
+                ' required Parameters cannot have a default value'
             )
+        super().__init__(name=name, required=required, help=help, hide=hide)
+        self.action = param_action(self)
+        self.default = default
+        self.metavar = metavar
+        self.strict_default = strict_default
+        if show_default is not None:
+            self.show_default = show_default
 
-        alt_opt_strs = filter(None, (alt_short, alt_long))
-        super().__init__(*option_strs, *alt_opt_strs, action=action, default=default, **kwargs)
-        self.consts = consts
-        self.option_strs.add_alts(alt_prefix, alt_long, alt_short)
-        if alt_help:
-            self.alt_help = alt_help
+    def _handle_bad_action(self, action: str) -> NoReturn:
+        """
+        Called when an action not supported by this type of Parameter was provided.  May be overwritten in subclasses
+        to provide hints about more appropriate options.
+        """
+        raise ParameterDefinitionError(
+            f'Invalid {action=} for {self.__class__.__name__} - valid actions: {sorted(self._action_map)}'
+        )
 
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
-        self.option_strs.update_alts(name)
+        # If self.type is None, a type may still be inferred from an annotation, which happens in this method.
+        if untyped_choices := self.type is not None:
+            if not isinstance(self.type, _ChoicesBase) or self.type.type is not None:
+                return  # An explicit type was provided to either stand alone or be used for Choices values
+            # self.type is therefore a Choices object with no explicit type provided, so from here on, the var
+            # name `untyped_choices` is accurate.  The type for its values may still be inferred from an annotation.
+        elif self.nargs.max is REMAINDER or not self._config(command).allow_annotation_type:
+            return
 
-    def _get_const(self, opt_str: str) -> Union[TC, TA]:
-        if opt_str in self.option_strs.alt_allowed:
-            return self.consts[1]
-        else:
-            return self.consts[0]
+        if (annotated_type := get_descriptor_value_type(command, name)) is None:
+            return
+        elif untyped_choices:
+            self.type.type = annotated_type
+        else:  # self.type must be None
+            # Choices present earlier would have already been converted
+            self.type = normalize_input_type(annotated_type, None)
 
-    @parameter_action
-    def store_const(self, opt_str: str):
-        self._store_const(self._get_const(opt_str))
+    @property
+    def has_choices(self) -> bool:
+        if type_attr := self.type:
+            return isinstance(type_attr, _ChoicesBase) and type_attr.choices
+        return False
+
+    # endregion
+
+    def __repr__(self) -> str:
+        names = ('action', 'const', 'default', 'type', 'choices', 'required', 'hide', 'help')
+        if extra_attrs := self._repr_attrs:
+            names = chain(names, extra_attrs)
+
+        skip = (None, _NotSet)
+        attrs = (
+            (a, str(v) if a == 'action' else v)
+            for a in names
+            if (v := getattr(self, a, None)) not in skip and not (a == 'hide' and not v)
+        )
+        kwargs = ', '.join(f'{a}={v!r}' for a, v in attrs)
+        return f'{self.__class__.__name__}({self.name!r}, {kwargs})'
+
+    # region Parsing / Argument Handling
+
+    def get_const(self, opt_str: OptStr = None):
+        return _NotSet
+
+    def get_env_const(self, value: str, env_var: str) -> Tuple[T_co, bool]:
+        return _NotSet, False
+
+    def prepare_value(self, value: str, short_combo: Bool = False, pre_action: Bool = False) -> T_co:
+        type_func = self.type
+        if type_func is None or (pre_action and isinstance(type_func, InputType) and type_func.is_valid_type(value)):
+            return value
+        try:
+            return type_func(value)
+        except InvalidChoiceError as e:
+            raise InvalidChoice(self, e.invalid, e.choices) from e
+        except InputValidationError as e:
+            raise BadArgument(self, str(e)) from e
+        except (TypeError, ValueError) as e:
+            raise BadArgument(self, f'bad {value=} for type={type_func!r}: {e}') from e
+        except Exception as e:
+            raise BadArgument(self, f'unable to cast {value=} to type={type_func!r}') from e
 
-    def _store_const(self, const: Union[TC, TA]):
-        ctx.set_parsed_value(self, const)
+    def validate(self, value: Optional[T_co], joined: Bool = False):
+        if not isinstance(value, str) or not value or not value[0] == '-':
+            return
+        elif self.allow_leading_dash == AllowLeadingDash.NUMERIC:
+            if not joined and len(value) > 1 and not _is_numeric(value):
+                raise BadArgument(self, f'invalid {value=}')
+        elif self.allow_leading_dash == AllowLeadingDash.NEVER:
+            raise BadArgument(self, f'invalid {value=}')
 
-    def take_action(
-        self, value: Optional[str], short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
-    ):
-        if value is None:
-            prev_parsed = ctx.get_parsed_value(self)
-            const = self._get_const(opt_str)
-            if prev_parsed is not self.default and prev_parsed != const:
-                raise ParamConflict([self])
-        return super().take_action(value, short_combo, opt_str, src)
-
-    def take_env_var_action(self, value: str, env_var: str):
-        parsed = self.prepare_env_var_value(value, env_var)
-        if self.use_env_value:
-            if parsed in self.consts:
-                self._store_const(parsed)
-            elif parsed != self.default:
-                raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
+    def is_valid_arg(self, value: Any) -> bool:
+        try:
+            self.validate(value)
+        except (InvalidChoice, BadArgument, MissingArgument):
+            return False
         else:
-            self._store_const(self.consts[0] if parsed else self.consts[1])
+            return True
 
+    # endregion
 
-# region Action Flag
+    # region Parse Results / Argument Value Handling
 
+    @overload
+    def __get__(self: Param, command: None, owner: CommandCls) -> Param:
+        ...
 
-class ActionFlag(Flag, repr_attrs=('order', 'before_main')):
-    """
-    A :class:`.Flag` that triggers the execution of a function / method / other callable when specified.
+    @overload
+    def __get__(self, command: CommandObj, owner: CommandCls) -> Optional[T_co]:
+        ...
 
-    :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
-      then one will automatically be added based on the name assigned to this parameter.
-    :param order: The priority / order in which this ActionFlag should be executed, relative to other ActionFlags, if
-      others would also be executed.  Two ActionFlags in a given :class:`.Command` may not have the same combination
-      of ``before_main`` and ``order`` values.  ActionFlags with lower ``order`` values are executed before those with
-      higher values.  The ``--help`` action is implemented as an ActionFlag with ``order=float('-inf')``.
-    :param func: The function to execute when this parameter is specified.
-    :param before_main: Whether this ActionFlag should be executed before the :meth:`.Command.main` method or
-      after it.
-    :param always_available: Whether this ActionFlag should always be available to be called, even if parsing
-      failed.  Only allowed when ``before_main=True``.  The intended use case is for actions like ``--help`` text.
-    :param kwargs: Additional keyword arguments to pass to :class:`.Flag`.
-    """
+    def __get__(self, command, owner):
+        if command is None:
+            return self
 
-    def __init__(
-        self,
-        *option_strs: str,
-        order: Union[int, float] = 1,
-        func: Callable = None,
-        before_main: Bool = True,  # noqa  # pylint: disable=W0621
-        always_available: Bool = False,
-        **kwargs,
-    ):
-        expected = {'action': 'store_const', 'default': False, 'const': _NotSet}
-        found = {k: kwargs.setdefault(k, v) for k, v in expected.items()}
-        if bad := {k: v for k, v in found.items() if expected[k] != v}:
-            raise ParameterDefinitionError(f'Unsupported kwargs for {self.__class__.__name__}: {bad}')
-        elif always_available and not before_main:
-            raise ParameterDefinitionError('always_available=True cannot be combined with before_main=False')
-        super().__init__(*option_strs, **kwargs)
-        self.func = func
-        self.order = order
-        self.before_main = before_main
-        self.always_available = always_available
+        with self._ctx(command):
+            value = self.result()
 
-    @property
-    def func(self):
-        return self._func
+        if (name := self._attr_name) is not None:
+            command.__dict__[name] = value  # Skip __get__ on subsequent accesses
+        return value
+
+    def result_value(self, missing_default: TD = _NotSet) -> Union[T_co, TD, None]:
+        value = ctx.get_parsed_value(self)
+        if value is _NotSet:
+            if self.required:
+                if missing_default is _NotSet:
+                    raise MissingArgument(self)
+                return missing_default
+            else:
+                return self.action.get_default(missing_default)
 
-    @func.setter
-    def func(self, func: Optional[Callable]):
-        self._func = func
-        if func is not None:
-            if self.help is None:
-                try:
-                    self.help = func.__doc__
-                except AttributeError:
-                    pass
-            update_wrapper(self, func)
+        return self.action.finalize_value(value)
 
-    def __hash__(self) -> int:
-        result = hash(self.__class__)
-        for attr in (self.name, self.command, self.func, self.order, self.before_main):
-            result ^= hash(attr)
-        return result
-
-    def __eq__(self, other: ActionFlag) -> bool:
-        if not isinstance(other, ActionFlag):
-            return NotImplemented
-        return all(getattr(self, a) == getattr(other, a) for a in ('name', 'func', 'command', 'order', 'before_main'))
-
-    def __lt__(self, other: ActionFlag) -> bool:
-        if not isinstance(other, ActionFlag):
-            return NotImplemented
-        # noinspection PyTypeChecker
-        return (not self.before_main, self.order, self.name) < (not other.before_main, other.order, other.name)
+    result = result_value
 
-    def __call__(self, func: Callable) -> ActionFlag:
-        """
-        Allows use as a decorator on the method to be called.  A given method can only be decorated with one ActionFlag.
+    # endregion
 
-        If stacking :class:`.Action` and :class:`.ActionFlag` decorators, the Action decorator must be first (i.e., the
-        ActionFlag decorator must be above the Action decorator).
-        """
-        if self.func is not None:
-            raise CommandDefinitionError(f'Cannot re-assign the func to call for {self}')
-        self.func = func
-        return self
+    # region Usage / Help Text
 
-    def __get__(self, command: Optional[CommandObj], owner: CommandCls) -> Union[ActionFlag, Callable]:
-        # Allow the method to be called, regardless of whether it was specified
-        if command is None:
-            return self
-        return partial(self.func, command)  # imitates a bound method
+    @property
+    def show_in_help(self) -> bool:
+        if self.hide:
+            return False
+        elif self.group is not None:
+            return self.group.show_in_help
+        return True
 
-    def result(self) -> Optional[Callable]:
-        if self.result_value():
-            if func := self.func:
-                return func
-            raise ParameterDefinitionError(f'No function was registered for {self}')
-        return None
+    # endregion
 
 
-#: Alias for :class:`ActionFlag`
-action_flag = ActionFlag  # pylint: disable=C0103
+class BasePositional(Parameter[T_co], ABC):
+    """
+    Base class for :class:`.Positional`, :class:`.SubCommand`, :class:`.Action`, and any other parameters that are
+    provided positionally, without prefixes.  It is not meant to be used directly.
 
+    All positional parameters are required by default.
 
-def before_main(*option_strs: str, order: Union[int, float] = 1, func: Callable = None, **kwargs) -> ActionFlag:
-    """An ActionFlag that will be executed before :meth:`.Command.main`"""
-    return ActionFlag(*option_strs, order=order, func=func, before_main=True, **kwargs)
+    Custom positional parameter classes should extend this class to be treated the same as other positionals by the
+    parser.
 
+    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
+      that extend Parameter, and must be registered via :class:`parameter_action`.
+    :param kwargs: Additional keyword arguments to pass to :class:`Parameter`.
+    """
 
-def after_main(*option_strs: str, order: Union[int, float] = 1, func: Callable = None, **kwargs) -> ActionFlag:
-    """An ActionFlag that will be executed after :meth:`.Command.main`"""
-    return ActionFlag(*option_strs, order=order, func=func, before_main=False, **kwargs)
+    _default_ok: bool = False
 
+    def __init_subclass__(cls, default_ok: bool = None, **kwargs):  # pylint: disable=W0222
+        """
+        :param default_ok: Whether default values are supported for this Parameter type
+        :param kwargs: Additional keyword arguments to pass to :meth:`.Parameter.__init_subclass__`.
+        """
+        super().__init_subclass__(**kwargs)
+        if default_ok is not None:
+            cls._default_ok = default_ok
 
-# endregion
+    def __init__(self, action: str, *, required: Bool = True, default: Any = _NotSet, **kwargs):
+        if not (self._default_ok and 0 in self.nargs):  # Indicates that having a default is bad
+            if not required:
+                cls_name = self.__class__.__name__
+                raise ParameterDefinitionError(f'All {cls_name} parameters must be required - invalid {required=}')
+            elif default is not _NotSet:
+                cls_name = self.__class__.__name__
+                raise ParameterDefinitionError(f"The 'default' arg is not supported for {cls_name} parameters")
+        super().__init__(action, default=default, required=required, **kwargs)
 
 
-class Counter(BaseOption[int], accepts_values=True, accepts_none=True):
+class BaseOption(Parameter[T_co], ABC):
     """
-    A :class:`.Flag`-like option that counts the number of times it was specified.  Supports an optional integer value
-    to explicitly increase the stored value by that amount.
+    Base class for :class:`.Option`, :class:`.Flag`, :class:`.Counter`, and any other keyword-like parameters that have
+    ``--long`` and ``-short`` prefixes before values.
+
+    Only the handling for processing long/short options and formatting usage of these parameters is provided in this
+    class - it is not meant to be used directly.
+
+    Custom option classes should extend this class to be treated the same as other options by the parser.
 
     :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
       then one will automatically be added based on the name assigned to this parameter.
-    :param action: The action to take on individual parsed values.  Defaults to ``append``, and no other actions
-      are supported (unless this class is extended).
-    :param default: The default value for this parameter if it is not specified.  This value is also be used as the
-      initial value that will be incremented when this parameter is specified.  Defaults to ``0``.
-    :param const: The value by which the stored value should increase whenever this parameter is specified.
-      Defaults to ``1``.  If a different ``const`` value is used, and if an explicit value is provided by a user,
-      the user-provided value will be added verbatim - it will NOT be multiplied by ``const``.
-    :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
+    :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
+      that extend Parameter, and must be registered via :class:`parameter_action`.
+    :param name_mode: Override the configured :ref:`configuration:Parsing Options:option_name_mode` for this
+      Option/Flag/Counter/etc.
+    :param env_var: A string or sequence (tuple, list, etc) of strings representing environment variables that should
+      be searched for a value when no value was provided via CLI.  If a value was provided via CLI, then these variables
+      will not be checked.  If multiple env variable names/keys were provided, then they will be checked in the order
+      that they were provided.  When enabled, values from env variables take precedence over the default value.  When
+      enabled and the Parameter is required, then either a CLI value or an env var value must be provided.
+    :param strict_env: When ``True`` (the default), if an :paramref:`.BaseOption.env_var` is used as the source of a
+      value for this Parameter and that value is invalid, then parsing will fail.  When ``False``, invalid values from
+      environment variables will be ignored (and a warning message will be logged).
+    :param use_env_value: For optional Parameters that support storing a constant (such as Flag), this option controls
+      behavior when an :paramref:`.BaseOption.env_var` is used as the source of a value for this Parameter.
+      If ``True``, the parsed value will be stored as this Parameter's value (it must be a valid value).  If ``False``
+      (the default), then the parsed value will be used to determine whether the store/append const action should be
+      taken as if it was specified as a CLI flag (e.g., ``--foo`` with no value).
+    :param kwargs: Additional keyword arguments to pass to :class:`Parameter`.
     """
 
-    type = int
-    nargs = Nargs('?')
+    _opt_str_cls: Type[OptionStrings] = OptionStrings
+    option_strs: OptionStrings
+    env_var: OptStrs = None
+    strict_env: Bool
+    use_env_value: Bool
+    const = _NotSet
 
-    def __init__(self, *option_strs: str, action: str = 'append', default: int = 0, const: int = 1, **kwargs):
-        vals = {'const': const, 'default': default}
-        if bad_types := ', '.join(f'{k}={v!r}' for k, v in vals.items() if not isinstance(v, self.type)):
-            raise ParameterDefinitionError(f'Invalid type for parameters (expected int): {bad_types}')
-        super().__init__(*option_strs, action=action, default=default, **kwargs)
-        self.const = const
-
-    def _init_value_factory(self):
-        return self.default
-
-    def prepare_value(self, value: Optional[str], short_combo: bool = False, pre_action: bool = False) -> int:
-        if value is None:
-            return self.const
-        try:
-            return self.type(value)
-        except (ValueError, TypeError) as e:
-            combinable = self.option_strs.combinable
-            if short_combo and combinable and all(c in combinable for c in value):
-                return len(value) + 1  # +1 for the -short that preceded this value
-            raise BadArgument(self, f'bad counter {value=}') from e
-
-    @parameter_action
-    def append(self, value: Optional[int]):
-        if value is None:
-            value = self.const
-        current = ctx.get_parsed_value(self)
-        ctx.set_parsed_value(self, current + value)
+    def __init__(
+        self,
+        *option_strs: str,
+        action: str,
+        name_mode: Union[OptionNameMode, str, None] = _NotSet,
+        env_var: OptStrs = None,
+        strict_env: bool = True,
+        use_env_value: Bool = None,
+        **kwargs,
+    ):
+        super().__init__(action, **kwargs)
+        self.option_strs = self._opt_str_cls(option_strs, name_mode)
+        self.strict_env = strict_env
+        if env_var:
+            self.env_var = env_var
+        if use_env_value is not None:
+            self.use_env_value = use_env_value
 
-    def validate(self, value: Any):
-        if value is None or isinstance(value, self.type):
-            return
-        try:
-            value = self.type(value)
-        except (ValueError, TypeError) as e:
-            raise BadArgument(self, f'invalid {value=} (expected an integer)') from e
-        else:
-            return
+    def _handle_bad_action(self, action: str) -> NoReturn:
+        if action in ('store', 'append') and (fixed := f'{action}_const') in self._action_map:
+            raise ParameterDefinitionError(f'Invalid {action=} for {self.__class__.__name__} - did you mean {fixed!r}?')
+        super()._handle_bad_action(action)
+
+    def __set_name__(self, command: CommandCls, name: str):
+        super().__set_name__(command, name)
+        if not (option_strs := self.option_strs).name_mode:
+            option_strs.name_mode = self._config(command).option_name_mode
+        option_strs.update(name)
+
+    def env_vars(self) -> Iterator[str]:
+        if env_var := self.env_var:
+            if isinstance(env_var, str):
+                yield env_var
+            else:
+                yield from env_var
 
-    def result_value(self) -> int:
-        return ctx.get_parsed_value(self)
+    def get_const(self, opt_str: OptStr = None):
+        return self.const
 
-    result = result_value
+
+class AllowLeadingDashProperty:
+    """
+    Custom value normalizer/validator for the ``allow_leading_dash`` property of ``Positional`` and ``Option`` classes.
+    """
+
+    __slots__ = ('name', 'default')
+
+    def __init__(self, default: AllowLeadingDash = AllowLeadingDash.NUMERIC):
+        self.default = default
+
+    def __set_name__(self, owner, name: str):
+        self.name = name
+
+    def __get__(self, instance: Optional[Parameter], owner) -> Union[AllowLeadingDash, AllowLeadingDashProperty]:
+        if instance is None:
+            return self
+        return instance.__dict__.get(self.name, self.default)
+
+    def __set__(self, instance: Parameter, value: LeadingDash):
+        if value is not None:
+            value = AllowLeadingDash(value)
+
+        nargs = instance.nargs
+        if nargs.max is REMAINDER:
+            if instance.type is not None:
+                raise ParameterDefinitionError(f'Type casting and choices are not supported with {nargs=}')
+            elif value not in (None, AllowLeadingDash.ALWAYS):
+                raise ParameterDefinitionError(
+                    f'With {nargs=}, only allow_leading_dash=AllowLeadingDash.ALWAYS is supported - found: {value!r}'
+                )
+            value = AllowLeadingDash.ALWAYS
+
+        if value is not None:
+            instance.__dict__[self.name] = value
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/positionals.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 Positional Parameters
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Literal
 
 from ..exceptions import ParameterDefinitionError
 from ..inputs import normalize_input_type
 from ..nargs import Nargs, NargsValue
 from ..utils import _NotSet
-from .base import BasicActionMixin, BasePositional
+from .actions import Store, Append
+from .base import BasePositional, AllowLeadingDashProperty
 
 if TYPE_CHECKING:
     from ..typing import InputTypeFunc, ChoicesType, LeadingDash
 
 __all__ = ['Positional']
 
 
-class Positional(BasicActionMixin, BasePositional, default_ok=True):
+class Positional(BasePositional, default_ok=True, actions=(Store, Append)):
     """
     A parameter that must be provided positionally.
 
     :param nargs: The number of values that are expected/required for this parameter.  Defaults to 1.  Use a value
       that allows 0 values to have the same effect as making this parameter not required (the ``required`` option
       is not supported for Positional parameters).  Only the last Positional parameter in a given :class:`.Command`
       may allow a variable / unbound number of arguments.  See :class:`.Nargs` for more info.
@@ -45,36 +46,45 @@
       a dash, it is only accepted if it appears to be a negative numeric value.  Use ``True`` / ``always`` /
       ``AllowLeadingDash.ALWAYS`` to allow any value that begins with a dash (as long as it is not an option string for
       an Option/Flag/etc).  To reject all values beginning with a dash, including numbers, use ``False`` / ``never`` /
       ``AllowLeadingDash.NEVER``.
     :param kwargs: Additional keyword arguments to pass to :class:`.BasePositional`.
     """
 
+    allow_leading_dash = AllowLeadingDashProperty()
+
     def __init__(
         self,
         nargs: NargsValue = None,
-        action: str = _NotSet,
+        action: Literal['store', 'append'] = None,
         type: InputTypeFunc = None,  # noqa
         default: Any = _NotSet,
         *,
         choices: ChoicesType = None,
         allow_leading_dash: LeadingDash = None,
         **kwargs,
     ):
-        if nargs is not None:
-            self.nargs = Nargs(nargs)
-            if self.nargs == 0:
-                cls_name = self.__class__.__name__
-                raise ParameterDefinitionError(f'Invalid nargs={self.nargs} - {cls_name} must allow at least 1 value')
-        if action is _NotSet:
-            action = 'store' if self.nargs == 1 or self.nargs == Nargs('?') else 'append'
-        elif action == 'store' and self.nargs.max != 1:
-            raise ParameterDefinitionError(f'Invalid {action=} for nargs={self.nargs}')
-        required = 0 not in self.nargs
-        if default is not _NotSet and required:
+        if nargs_provided := nargs is not None:
+            self.nargs = nargs = Nargs(nargs)
+            if nargs == 0:
+                raise ParameterDefinitionError(
+                    f'Invalid {nargs=} - {self.__class__.__name__} must allow at least 1 value'
+                )
+        else:
+            self.nargs = nargs = Nargs(1)
+
+        if not action:
+            if nargs_provided:
+                action = 'store' if nargs == 1 or nargs == Nargs('?') else 'append'
+            else:
+                action = 'store'
+        elif nargs_provided and action == 'store' and nargs.max != 1:
+            raise ParameterDefinitionError(f'Invalid {action=} for {nargs=}')
+
+        if (required := 0 not in nargs) and default is not _NotSet:
             raise ParameterDefinitionError(
                 f'Invalid {default=} - only allowed for Positional parameters when nargs=? or nargs=*'
             )
         kwargs.setdefault('required', required)
         super().__init__(action=action, default=default, **kwargs)
         self.type = normalize_input_type(type, choices)
-        self._validate_nargs_and_allow_leading_dash(allow_leading_dash)
+        self.allow_leading_dash = allow_leading_dash
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parse_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union, Optional, Collection, Iterable, Iterator, MutableMapping, Dict, Set, Tuple
 
 from .exceptions import AmbiguousParseTree
-from .nargs import nargs_max_sum, nargs_min_sum
+from .nargs import nargs_min_and_max_sums
 from .utils import _parse_tree_target_repr
 
 if TYPE_CHECKING:
     from .nargs import Nargs
     from .parameters.base import BasePositional
     from .parameters.choice_map import Choice
     from .typing import OptStr, CommandCls
@@ -85,19 +85,16 @@
     def _link_params(self, recursive: bool = False) -> Iterator[BasePositional]:
         for node in self.values():
             yield node.param
         if recursive:
             for node in self.values():
                 yield from node._link_params(_has_upper_bound(node))
 
-    def nargs_min(self) -> int:
-        return nargs_min_sum(p.nargs for p in self.link_params(True))
-
-    def nargs_max(self) -> Union[int, float]:
-        return nargs_max_sum(p.nargs for p in self.link_params(True))
+    def nargs_min_and_max(self) -> Tuple[int, Union[int, float]]:
+        return nargs_min_and_max_sums(p.nargs for p in self.link_params(True))
 
     # region AnyWord Methods
 
     @property
     def any_word(self) -> AnyWord:
         try:
             return self._any_word
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/parser.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,360 +2,397 @@
 The class that handles parsing input.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-# import logging
+import logging
 from collections import deque
 from os import environ
-from typing import TYPE_CHECKING, Optional, Union, Any, Deque, List
+from typing import TYPE_CHECKING, Optional, Iterable, Deque, List
 
+from .core import get_parent
 from .context import ActionPhase, Context
 from .exceptions import UsageError, ParamUsageError, NoSuchOption, MissingArgument, ParamsMissing
-from .exceptions import Backtrack, NextCommand, UnsupportedAction
-from .nargs import REMAINDER, nargs_max_sum, nargs_min_sum
+from .exceptions import Backtrack, NextCommand
+from .nargs import REMAINDER, nargs_min_and_max_sums
 from .parse_tree import PosNode
-from .parameters.base import BasicActionMixin, Parameter, BasePositional, BaseOption
-from .utils import ValueSource
+from .parameters.base import Parameter, BasePositional, BaseOption
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .config import CommandConfig
-    from .typing import CommandType
+    from .typing import CommandType, OptStr, Bool
 
-__all__ = ['CommandParser']
-# log = logging.getLogger(__name__)
+__all__ = ['CommandParser', 'parse_args_and_get_next_cmd']
+log = logging.getLogger(__name__)
+
+_PRE_INIT = ActionPhase.PRE_INIT
 
 
 class CommandParser:
     """Stateful parser used for a single pass of argument parsing"""
 
-    __slots__ = ('_last', 'arg_deque', 'config', 'deferred', 'params', 'positionals')
+    __slots__ = ('_last', 'arg_deque', 'ctx', 'config', 'deferred', 'params', 'positionals')
 
     arg_deque: Optional[Deque[str]]
     config: CommandConfig
     deferred: Optional[List[str]]
     params: CommandParameters
     positionals: List[BasePositional]
     _last: Optional[Parameter]
 
     def __init__(self, ctx: Context, params: CommandParameters, config: CommandConfig):
         self._last = None
+        self.ctx = ctx
         self.params = params
         self.positionals = params.get_positionals_to_parse(ctx)
         self.config = config
         if config.reject_ambiguous_pos_combos:
             PosNode.build_tree(ctx.command)
 
     @classmethod
     def parse_args_and_get_next_cmd(cls, ctx: Context) -> Optional[CommandType]:
         try:
             return cls(ctx, ctx.params, ctx.config).get_next_cmd(ctx)
         except UsageError:
-            if not ctx.categorized_action_flags[ActionPhase.PRE_INIT]:
+            if not ctx.categorized_action_flags[_PRE_INIT]:
                 raise
             return None
 
     def get_next_cmd(self, ctx: Context) -> Optional[CommandType]:
         self._parse_args(ctx)
-        params = self.params
-        params.validate_groups()
+        self._validate_groups()
         missing = ctx.get_missing()
-        no_pre_init_action = not ctx.categorized_action_flags[ActionPhase.PRE_INIT]
-        next_cmd = params.sub_command.target() if params.sub_command else None
-        if next_cmd is not None:
-            if missing and no_pre_init_action and next_cmd.__class__.parent(next_cmd) is not ctx.command:
+        if (sub_cmd_param := self.params.sub_command) and (next_cmd := sub_cmd_param.target()) is not None:
+            if missing and not ctx.categorized_action_flags[_PRE_INIT] and get_parent(next_cmd) is not ctx.command:
                 raise ParamsMissing(missing)
-        elif missing and not ctx.config.allow_missing and (not params.action or params.action not in missing):
-            if no_pre_init_action:
+            return next_cmd
+        elif missing and not ctx.config.allow_missing and (not self.params.action or self.params.action not in missing):
+            if not ctx.categorized_action_flags[_PRE_INIT]:  # No pre-init action was triggered
                 raise ParamsMissing(missing)
-        elif ctx.remaining and not ctx.config.ignore_unknown:
+        elif ctx.remaining and not ctx.config.ignore_unknown:  # Note: ctx.remaining is self.deferred at this point
             raise NoSuchOption(f'unrecognized arguments: {" ".join(ctx.remaining)}') from None
-        return next_cmd
+        return None
+
+    def _validate_groups(self):
+        exc = None
+        for group in self.params.groups:
+            try:
+                group.validate()
+            except ParamsMissing as e:  # Let ParamConflict propagate before ParamsMissing
+                if exc is None:
+                    exc = e
+
+        if exc is not None:
+            raise exc
 
     def _parse_args(self, ctx: Context):
         self.arg_deque = arg_deque = self.handle_pass_thru(ctx)
         self.deferred = ctx.remaining = []
+
         while arg_deque:
             arg = arg_deque.popleft()
             try:
-                if self._parse_arg(ctx, arg):
+                if self._handle_arg(arg):
                     break
             except NextCommand:
                 self.deferred.append(arg)
                 self.deferred.extend(arg_deque)
                 break
 
         self._parse_env_vars(ctx)
 
-    def _parse_arg(self, ctx: Context, arg: str):
-        if arg == '--':
-            if self._maybe_consume_remainder(arg):
-                return True
-            elif ctx.params.find_nested_pass_thru():  # pylint: disable=R1723
-                # TODO: Make sure a test exists where parsing fails because required params were not provided yet
-                raise NextCommand
-            else:
-                raise NoSuchOption(f'invalid argument: {arg}')
-        elif arg.startswith('---'):
-            if not self._maybe_consume_remainder(arg):
-                raise NoSuchOption(f'invalid argument: {arg}')
-        elif arg.startswith('--'):
-            self.handle_long(arg)
-        elif arg.startswith('-') and arg != '-':
-            self.handle_short(arg)
-        else:
-            self.handle_positional(arg)
-
-        return False
-
     def _parse_env_vars(self, ctx: Context):
         # TODO: It would be helpful to store arg provenance for error messages, especially for a conflict between
         #  mutually exclusive params when they were provided via env
-        env = ValueSource.ENV
-        for param in self.params.try_env_params(ctx):
+        for param in ctx.missing_options_with_env_var():
             for env_var in param.env_vars():
                 try:
                     value = environ[env_var]
                 except KeyError:
                     pass
                 else:
-                    param.take_action(value, src=(env, env_var))
+                    try:
+                        param.action.add_env_value(value, env_var)
+                    except ParamUsageError as e:
+                        if param.strict_env:
+                            raise
+                        log.warning(e)
                     break
 
+    def _handle_arg(self, arg: str):
+        if not arg or arg[0] != '-':
+            return self.handle_positional(arg)
+        n = len(arg)
+        if n > 1 and arg[1] != '-':  # arg starts with 1 dash followed by a non-dash
+            return self.handle_short(arg)
+        elif n > 2:  # arg starts with at least 1 dash, and may be a long option or invalid
+            return self.handle_long(arg) if arg[2] != '-' else self._handle_many_dashes(arg)
+        else:  # arg == '--'
+            return self._handle_double_dash(arg)
+
+    def _handle_double_dash(self, arg: str):
+        if self._maybe_consume_remainder(arg):
+            return True
+        elif self.params.has_nested_pass_thru:  # pylint: disable=R1723
+            # TODO: Make sure a test exists where parsing fails because required params were not provided yet
+            raise NextCommand
+        else:
+            raise NoSuchOption(f'invalid argument: {arg}')
+
+    def _handle_many_dashes(self, arg: str):
+        if not self._maybe_consume_remainder(arg):
+            raise NoSuchOption(f'invalid argument: {arg}')
+
+    # region PassThru / Remainder Handling
+
     def handle_pass_thru(self, ctx: Context) -> Deque[str]:
         remaining = ctx.remaining
-        pass_thru = self.params.pass_thru
-        if pass_thru is not None:
+        if pass_thru := self.params.pass_thru:
             try:
                 separator_pos = remaining.index('--')
             except ValueError:
                 pass  # If required, it's handled by the normal missing param handler
             else:
                 remainder_start = separator_pos + 1
-                pass_thru.take_action(remaining[remainder_start:])
+                pass_thru.action.add_values(remaining[remainder_start:])
                 return deque(remaining[:separator_pos])
         return deque(remaining)
 
     def _maybe_consume_remainder(self, arg: str) -> bool:
         if len(self.positionals) == 1:
             param = self.positionals[0]
             if param.nargs.max is REMAINDER:
                 self.handle_remainder(param, arg)
                 return True
         return False
 
     def handle_remainder(self, param: Parameter, value: str) -> int:
-        found = param.take_action(value)
+        found = param.action.add_value(value)
         arg_deque = self.arg_deque
         while arg_deque:
-            found += param.take_action(arg_deque.popleft())
+            found += param.action.add_value(arg_deque.popleft())
         return found
 
+    # endregion
+
     def handle_positional(self, arg: str):
         # log.debug(f'handle_positional({arg=})')
-        try:
-            param: BasePositional = self.positionals.pop(0)
-        except IndexError:
-            self.deferred.append(arg)
-        else:
+        if positionals := self.positionals:
+            param: BasePositional = positionals.pop(0)
             if param.nargs.max is REMAINDER:
                 self.handle_remainder(param, arg)
             else:
                 try:
-                    found = param.take_action(arg)
+                    found = param.action.add_value(arg)
                 except UsageError:
-                    self.positionals.insert(0, param)
+                    positionals.insert(0, param)
                     raise
                 try:
                     self.consume_values(param, found=found)
                 except Backtrack:
-                    self.positionals.insert(0, param)
+                    positionals.insert(0, param)
                 else:
                     self._last = param
+        else:
+            self.deferred.append(arg)
+
+    # region Option Handling
 
     def handle_long(self, arg: str):
         # log.debug(f'handle_long({arg=})')
-        try:
-            opt, param, value = self.params.long_option_to_param_value_pair(arg)
-        except KeyError:
-            if not self._maybe_consume_remainder(arg):
-                self._check_sub_command_options(arg)
-                self.deferred.append(arg)
-        else:
-            if value is not None or (param.accepts_none and not param.accepts_values):
-                param.take_action(value, opt_str=opt)
-            elif not self.consume_values(param) and param.accepts_none:
-                param.take_action(None, opt_str=opt)
-            self._last = param
+        opt, eq, value = arg.partition('=')
+        if param := self.params.option_map.get(opt):
+            self._handle_option_value(opt, param, value if eq else None, joined=eq)
+        elif not self._maybe_consume_remainder(arg):
+            self._check_sub_command_options(arg)
+            self.deferred.append(arg)
+
+    def _handle_option_value(
+        self, opt: str, param: BaseOption, value: OptStr, combo: bool = False, joined: Bool = False
+    ):
+        if value is not None:
+            param.action.add_value(value, opt=opt, combo=combo, joined=joined)
+        elif param.action.accepts_consts and not param.action.accepts_values:
+            param.action.add_const(opt=opt, combo=combo)
+        elif not self.consume_values(param) and param.action.accepts_consts:
+            # The order of conditions here is important - consume_values has an intended side effect even when
+            # the action does not accept constants
+            param.action.add_const(opt=opt, combo=combo)
+
+        self._last = param
+        # No need to raise MissingArgument if values were not consumed - consume_values handles checking nargs
 
     def handle_short(self, arg: str):
         # log.debug(f'handle_short({arg=})')
         try:
-            param_val_combos = self.params.short_option_to_param_value_pairs(arg)
+            param_val_combos, joined = self.params.short_option_to_param_value_pairs(arg)
         except KeyError:  # Handles 3 potential KeyErrors for either the full short option or a single-char combo
             self._handle_short_not_found(arg)
         else:
             # log.debug(f'Split {arg=} into {param_val_combos=}')
             last = param_val_combos.pop()
             if param_val_combos:
                 # Note: This loop is only executed for single char combined flags, where the values will always be None
-                for opt, param, value in param_val_combos:
-                    param.take_action(value, short_combo=True, opt_str=opt)
-            self._handle_short_value(*last)
+                for opt, param, _none_value in param_val_combos:
+                    param.action.add_const(opt=opt, combo=True)
+            self._handle_option_value(*last, combo=True, joined=joined)
 
     def _handle_short_not_found(self, arg: str):
         if self._maybe_consume_remainder(arg):
             return
         self._check_sub_command_options(arg)
         if self.positionals:
             try:
                 self.handle_positional(arg)
             except UsageError:
                 self.deferred.append(arg)
         else:
             self.deferred.append(arg)
 
-    def _handle_short_value(self, opt: str, param: BaseOption, value: Any):
-        # log.debug(f'Handling short {value=} for {param=}')
-        if value is not None or (param.accepts_none and not param.accepts_values):
-            param.take_action(value, short_combo=True, opt_str=opt)
-        elif not self.consume_values(param) and param.accepts_none:
-            param.take_action(None, short_combo=True, opt_str=opt)
-        self._last = param
-        # No need to raise MissingArgument if values were not consumed - consume_values handles checking nargs
+    # endregion
 
     def _check_sub_command_options(self, arg: str):
         # log.debug(f'_check_sub_command_options({arg=})')
         # This check is only needed when subcommand option values may be misinterpreted as positional values
         if not self.positionals:
             return
-        param = self.params.find_nested_option_that_accepts_values(arg)
-        if param is None:
-            return
-        elif len(self.positionals) == 1 and 0 in self.positionals[0].nargs:
-            raise NextCommand
-        else:
-            raise ParamUsageError(param, 'subcommand arguments must be provided after the subcommand')
+        option = arg.split('=', 1)[0]  # Strip any `=value` suffix if it exists
+        ncps = self.params._iter_nested_params()
+        # Try to find a nested Option that accepts values
+        if param := next((p for cp in ncps if (p := cp.option_map.get(option)) and p.action.accepts_values), None):
+            if len(self.positionals) == 1 and 0 in self.positionals[0].nargs:
+                raise NextCommand
+            else:
+                raise ParamUsageError(param, 'subcommand arguments must be provided after the subcommand')
+
+    # region Backtracking
 
     def _maybe_backtrack(self, param: Parameter, found: int) -> int:
         """
         If we hit the end of the list of provided argument values, unfulfilled Positional parameters remain, and the
         Parameter being processed accepts a variable number of arguments, then check to see if it's possible to
         backtrack to move some of those values to the remaining positionals.
 
         :param param: The :class:`.Parameter` that was consuming values when the arg_deque became empty
         :param found: The number of values that were consumed by the given Parameter
         :return: The updated found count, if backtracking was possible, otherwise the unmodified found count
         """
-        if not self.config.allow_backtrack or not self.positionals or found < 2:
-            return found
-
-        can_pop = param.can_pop_counts()
-        to_pop = _to_pop(self.positionals, can_pop, found - 1)
-        if to_pop is None:
-            return found
-
-        self.arg_deque.extendleft(reversed(param.pop_last(to_pop)))
-        return found - to_pop
+        if positionals := self.positionals:
+            can_pop = param.action.get_maybe_poppable_counts()
+            if rollback_count := _to_pop(positionals, can_pop, found - 1):
+                self.arg_deque.extendleft(reversed(self.ctx.roll_back_parsed_values(param, rollback_count)))
+                return found - rollback_count
+        return found
 
-    def _maybe_backtrack_last(self, param: Union[BasePositional, BasicActionMixin], found: int):
+    def _maybe_backtrack_last(self, param: BasePositional, found: int):
         """
         Similar to :meth:`._maybe_backtrack`, but allows backtracking even after starting to process a Positional.
         """
         if not self.config.allow_backtrack:
+            # This method is called relatively rarely & it's cleaner to have this check here than in _finalize_consume
             return
 
-        can_pop = self._last.can_pop_counts()
-        to_pop = _to_pop([param, *self.positionals], can_pop, max(can_pop, default=0) + found, found)
-        if to_pop is None:
-            return
+        can_pop = self._last.action.get_maybe_poppable_counts()
+        # It is extremely unlikely for this point to be reached without this resulting in triggering a backtrack
+        if rollback_count := _to_pop((param, *self.positionals), can_pop, max(can_pop, default=0) + found, found):
+            self.arg_deque.extendleft(reversed(self.ctx.pop_parsed_value(param)))
+            self.arg_deque.extendleft(reversed(self.ctx.roll_back_parsed_values(self._last, rollback_count)))
+            raise Backtrack
 
-        try:
-            reset = param._reset()
-        except UnsupportedAction:
-            return
+    # endregion
 
-        self.arg_deque.extendleft(reversed(reset))
-        self.arg_deque.extendleft(reversed(self._last.pop_last(to_pop)))
-        raise Backtrack
+    def _has_matching_short_option(self, arg: str) -> bool:
+        try:
+            self.params.short_option_to_param_value_pairs(arg)
+        except KeyError:
+            return False
+        return True
 
     def consume_values(self, param: Parameter, found: int = 0) -> int:
         """
         Consume values for the given Parameter.
 
         :param param: The active :class:`.Parameter` that should receive the discovered values
         :param found: The number of already discovered values for that Parameter (only specified for positional params)
         :return: The total number of values that were found for the given Parameter.
         """
-        remainder = param.nargs.max is REMAINDER
-        while True:
-            try:
-                value = self.arg_deque.popleft()
-            except IndexError:
-                # log.debug(f'Ran out of values in deque while processing {param=}')
-                found = self._maybe_backtrack(param, found)
-                return self._finalize_consume(param, None, found)
-            else:
-                # log.debug(f'Found {value=} in deque - may use it for {param=}')
-                if remainder:
-                    return self.handle_remainder(param, value)
-                elif value.startswith('--'):
-                    return self._finalize_consume(param, value, found)
-                elif value.startswith('-') and value != '-':
-                    if self.params.get_option_param_value_pairs(value):
-                        # log.debug(f'{value=} will not be used with {param=} - it is also a parameter')
-                        return self._finalize_consume(param, value, found)
-                    else:
-                        try:
-                            self._check_sub_command_options(value)
-                        except (ParamUsageError, NextCommand) as e:
-                            return self._finalize_consume(param, value, found, e)
-
-                    if not param.would_accept(value):
-                        # log.debug(f'{value=} will not be used with {param=} - it would not be accepted')
-                        return self._finalize_consume(param, value, found, NoSuchOption(f'invalid argument: {value}'))
-                    # log.debug(f'{value=} may be used with {param=} as a value')
+        arg_deque = self.arg_deque
+        if param.nargs.max is REMAINDER and arg_deque:
+            return self.handle_remainder(param, arg_deque.popleft())
 
+        while arg_deque:
+            value = arg_deque.popleft()
+            # log.debug(f'Found {value=} in deque - may use it for {param=}')
+            if prefix := get_opt_prefix(value):
+                if prefix == '--' or self._has_matching_short_option(value):
+                    return self._finalize_consume(param, value, found)
+                # Beyond this point, prefix == '-'
                 try:
-                    found += param.take_action(value)
-                except UsageError as e:
-                    # log.debug(f'{value=} was rejected by {param=}', exc_info=True)
+                    self._check_sub_command_options(value)
+                except (ParamUsageError, NextCommand) as e:
                     return self._finalize_consume(param, value, found, e)
 
-    def _finalize_consume(
-        self, param: Parameter, value: Optional[str], found: int, exc: Optional[Exception] = None
-    ) -> int:
-        if param.nargs.satisfied(found):
+                if not param.action.would_accept(value):
+                    # log.debug(f'{value=} will not be used with {param=} - it would not be accepted')
+                    return self._finalize_consume(param, value, found, NoSuchOption(f'invalid argument: {value}'))
+                # log.debug(f'{value=} may be used with {param=} as a value')
+
+            try:
+                found += param.action.add_value(value)
+            except UsageError as e:
+                # log.debug(f'{value=} was rejected by {param=}', exc_info=True)
+                return self._finalize_consume(param, value, found, e)
+
+        # log.debug(f'Ran out of values in deque while processing {param=}')
+        if found >= 2 and self.config.allow_backtrack:
+            found = self._maybe_backtrack(param, found)
+        return self._finalize_consume(param, None, found)
+
+    def _finalize_consume(self, param: Parameter, value: OptStr, found: int, exc: Optional[Exception] = None) -> int:
+        nargs = param.nargs
+        if nargs.satisfied(found):
             # Even if an exception was passed to this method, if the found number of values is acceptable, then it
             # doesn't need to be raised.  The value that (would have) caused the exception is added back to the deque.
             if value is not None:
                 self.arg_deque.appendleft(value)
             # log.debug(f'consume_values {found=} for {param=}')
             return found
         elif exc:
             raise exc
-        elif self._last and isinstance(param, BasePositional) and hasattr(param, '_reset'):
+        elif self._last and isinstance(param, BasePositional) and param.action.can_reset():
             self._maybe_backtrack_last(param, found)
 
-        n = param.nargs.min
-        s = '' if n == 1 else 's'
+        s = '' if (n := nargs.min) == 1 else 's'
         raise MissingArgument(param, f'expected {n} value{s}, but only found {found}')
 
 
-def _to_pop(positionals: List[BasePositional], can_pop: List[int], available: int, req_mod: int = 0) -> Optional[int]:
+parse_args_and_get_next_cmd = CommandParser.parse_args_and_get_next_cmd
+
+
+def _to_pop(positionals: Iterable[BasePositional], can_pop: List[int], available: int, req_mod: int = 0) -> int:
     if not can_pop:
-        return None
+        return 0
 
-    required = nargs_min_sum(p.nargs for p in positionals)
+    required, acceptable = nargs_min_and_max_sums(p.nargs for p in positionals)
     if available < required:
-        return None
+        return 0
 
     required -= req_mod
-    acceptable = nargs_max_sum(p.nargs for p in positionals)
     for n in can_pop:
         if required <= n <= acceptable:
             return n
 
+    return 0
+
+
+def get_opt_prefix(text: str) -> OptStr:
+    if not text or text[0] != '-':
+        return None
+    n = len(text)
+    if n > 1 and text[1] != '-':
+        return '-'
+    elif n > 2 and text[2] != '-':
+        return '--'
     return None
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/testing.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/testing.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,155 +7,168 @@
 
 from __future__ import annotations
 
 import sys
 from contextlib import AbstractContextManager, contextmanager
 from difflib import unified_diff
 from io import StringIO, BytesIO
+from pathlib import Path
+from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Any, Iterable, Type, Union, Callable, IO, ContextManager, Dict, List, Tuple
 from unittest import TestCase
 from unittest.mock import Mock, seal, patch
 
-from .actions import help_action
 from .commands import Command
 from .context import Context
 from .core import get_params
 from .documentation import load_commands
 from .exceptions import UsageError
+from .parameters import help_action
 
 if TYPE_CHECKING:
-    from pathlib import Path
-    from .typing import CommandCls
+    from .typing import CommandCls, OptStr
 
 __all__ = [
     'ParserTest',
     'RedirectStreams',
     'format_diff',
     'get_rst_text',
     'get_help_text',
     'get_usage_text',
     'sealed_mock',
     'load_command',
+    'TemporaryDir',
 ]
 
 Argv = List[str]
 Expected = Dict[str, Any]
 Kwargs = Dict[str, Any]
 Env = Dict[str, str]
 Case = Tuple[Argv, Expected]
 EnvCase = Tuple[Argv, Env, Expected]
-ExceptionCase = Union[Argv, Tuple[Argv, Type[Exception]], Tuple[Argv, Type[Exception], str]]
-CallExceptionCase = Union[Tuple[Kwargs, Type[Exception]], Tuple[Kwargs, Type[Exception], str]]
+ExcType = Type[Exception]
+ExceptionCase = Union[Argv, Tuple[Argv, ExcType], Tuple[Argv, ExcType, str]]
+ExcCases = Iterable[ExceptionCase]
+CallExceptionCase = Union[Tuple[Kwargs, ExcType], Tuple[Kwargs, ExcType, str]]
+CallExceptionCases = Iterable[CallExceptionCase]
 
 OPT_ENV_MOD = 'cli_command_parser.parser.environ'
 
 
+class AssertRaisesWithStringContext:
+    """
+    Simplified version of the stdlib ``_AssertRaisesContext`` that tests whether the raised exception's string contains
+    the given text rather than matching it against a regex pattern.  This avoids the regex overhead when it isn't
+    necessary, which is the majority of the time for such checks in this project.
+    """
+
+    __slots__ = ('test_case', 'expected_exc', 'expected_text', 'msg')
+
+    def __init__(self, test_case: TestCase, expected_exc: Type[BaseException], text: OptStr = None, msg: OptStr = None):
+        self.test_case = test_case
+        self.expected_exc = expected_exc
+        self.expected_text = text
+        self.msg = (' - ' + msg) if msg else ''
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type is None:
+            self.test_case.fail(f'{self.expected_exc.__name__} not raised{self.msg}')
+        elif not issubclass(exc_type, self.expected_exc):
+            return False  # Let unexpected exceptions be propagated
+        elif self.expected_text and self.expected_text not in str(exc_val):
+            self.test_case.fail(f'{self.expected_text!r} not found in {str(exc_val)!r}{self.msg}')
+        return True
+
+
 class ParserTest(TestCase):
     # def setUp(self):
     #     print()
     #
     # def subTest(self, *args, **kwargs):
     #     print()
     #     return super().subTest(*args, **kwargs)
 
     def assert_dict_equal(self, d1, d2, msg: str = None):
         self.assertIsInstance(d1, dict, 'First argument is not a dictionary')
         self.assertIsInstance(d2, dict, 'Second argument is not a dictionary')
         if d1 != d2:
-            standard_msg = f'{d1} != {d2}\n{format_dict_diff(d1, d2)}'
-            self.fail(self._formatMessage(msg, standard_msg))
+            self.fail(self._formatMessage(msg, f'{d1} != {d2}\n{format_dict_diff(d1, d2)}'))
+
+    def assert_raises_contains_str(self, expected_exc: Type[BaseException], expected_text: str, msg: str = None):
+        return AssertRaisesWithStringContext(self, expected_exc, expected_text, msg)
 
-    def assert_parse_results(self, cmd_cls: CommandCls, argv: Argv, expected: Expected, message: str = None) -> Command:
+    def assert_parse_results(self, cmd_cls: CommandCls, argv: Argv, expected: Expected, msg: str = None) -> Command:
         cmd = cmd_cls.parse(argv)
         parsed = cmd.ctx.get_parsed((help_action,))
-        self.assert_dict_equal(expected, parsed, message)
+        self.assert_dict_equal(expected, parsed, msg)
         return cmd
 
-    def assert_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[Case], message: str = None):
+    def assert_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[Case], msg: str = None):
         for argv, expected in cases:
             with self.subTest(expected='results', argv=argv):
-                self.assert_parse_results(cmd_cls, argv, expected, message)
+                self.assert_parse_results(cmd_cls, argv, expected, msg)
 
     def assert_env_parse_results(
-        self, cmd_cls: CommandCls, argv: Argv, env: Env, expected: Expected, message: str = None
+        self, cmd_cls: CommandCls, argv: Argv, env: Env, expected: Expected, msg: str = None
     ) -> Command:
         with patch(OPT_ENV_MOD, env):
-            return self.assert_parse_results(cmd_cls, argv, expected, message)
+            return self.assert_parse_results(cmd_cls, argv, expected, msg)
 
-    def assert_env_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[EnvCase], message: str = None):
+    def assert_env_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[EnvCase], msg: str = None):
         for argv, env, expected in cases:
             with self.subTest(expected='results', argv=argv, env=env):
-                self.assert_env_parse_results(cmd_cls, argv, env, expected, message)
+                self.assert_env_parse_results(cmd_cls, argv, env, expected, msg)
 
     def assert_parse_fails(
         self,
         cmd_cls: CommandCls,
         argv: Argv,
-        expected_exc: Type[Exception] = UsageError,
+        expected_exc: ExcType = UsageError,
         expected_pattern: str = None,
-        message: str = None,
+        msg: str = None,
+        regex: bool = False,
     ):
-        if expected_pattern:
-            with self.assertRaisesRegex(expected_exc, expected_pattern, msg=message):
+        if expected_pattern and regex:
+            with self.assertRaisesRegex(expected_exc, expected_pattern, msg=msg):
                 cmd_cls.parse(argv)
         else:
-            with self.assertRaises(expected_exc, msg=message):
+            with AssertRaisesWithStringContext(self, expected_exc, expected_pattern, msg):
                 cmd_cls.parse(argv)
 
-    def assert_parse_fails_cases(
-        self, cmd_cls: CommandCls, cases: Iterable[ExceptionCase], exc: Type[Exception] = None, message: str = None
-    ):
-        if exc is not None:
-            for argv in cases:
-                with self.subTest(expected='exception', argv=argv):
-                    self.assert_parse_fails(cmd_cls, argv, exc, message=message)
-        else:
-            for case in cases:
-                try:
-                    argv, exc = case
-                except ValueError:
-                    argv, exc, pat = case
-                else:
-                    pat = None
-
-                with self.subTest(expected='exception', argv=argv):
-                    self.assert_parse_fails(cmd_cls, argv, exc, pat, message=message)
+    def assert_parse_fails_cases(self, cmd_cls: CommandCls, cases: ExcCases, exc: ExcType = None, msg: str = None):
+        for argv, exc, pat in _iter_exc_cases(cases, exc):
+            with self.subTest(expected='exception', argv=argv):
+                with AssertRaisesWithStringContext(self, exc, pat, msg):
+                    cmd_cls.parse(argv)
 
     def assert_argv_parse_fails_cases(
-        self, cmd_cls: CommandCls, cases: Iterable[Argv], exc: Type[Exception] = UsageError, message: str = None
+        self, cmd_cls: CommandCls, cases: Iterable[Argv], exc: ExcType = UsageError, msg: str = None
     ):
         """Convenience method for calling :meth:`.assert_parse_fails_cases` with a default exception type."""
-        self.assert_parse_fails_cases(cmd_cls, cases, exc, message)
+        self.assert_parse_fails_cases(cmd_cls, cases, exc, msg)
 
     def assert_call_fails(
         self,
         func: Callable,
         kwargs: Kwargs,
-        exc: Type[Exception] = Exception,
-        pattern: str = None,
-        message: str = None,
+        exc: ExcType = Exception,
+        expected_exc_msg: str = None,
+        msg: str = None,
     ):
-        if pattern:
-            with self.assertRaisesRegex(exc, pattern, msg=message):
-                func(**kwargs)
-        else:
-            with self.assertRaises(exc, msg=message):
-                func(**kwargs)
-
-    def assert_call_fails_cases(self, func: Callable, cases: Iterable[CallExceptionCase], message: str = None):
-        for case in cases:
-            try:
-                kwargs, exc = case
-            except ValueError:
-                kwargs, exc, pat = case
-            else:
-                pat = None
+        with AssertRaisesWithStringContext(self, exc, expected_exc_msg, msg):
+            func(**kwargs)
 
+    def assert_call_fails_cases(self, func: Callable, cases: Iterable[CallExceptionCase], msg: str = None):
+        for kwargs, exc, pat in _iter_exc_cases(cases):
             with self.subTest(expected='exception', kwargs=kwargs):
-                self.assert_call_fails(func, kwargs, exc, pat, message=message)
+                with AssertRaisesWithStringContext(self, exc, pat, msg):
+                    func(**kwargs)
 
     def assert_strings_equal(
         self, expected: str, actual: str, message: str = None, diff_lines: int = 3, trim: bool = False
     ):
         if trim:
             expected = expected.rstrip()
             actual = '\n'.join(line.rstrip() for line in actual.splitlines())
@@ -179,14 +192,28 @@
 
     @contextmanager
     def env_vars(self, case: str, **env_vars):
         with self.subTest(case=case), patch(OPT_ENV_MOD, env_vars):
             yield
 
 
+def _iter_exc_cases(cases: Union[ExcCases, CallExceptionCases], exc: ExcType = None):
+    if exc is not None:
+        for args in cases:
+            yield args, exc, None
+    else:
+        for case in cases:
+            try:
+                args, exc = case
+            except ValueError:
+                yield case  # Assume it is a 3-tuple of ([argv|kwargs], exc, pattern)
+            else:
+                yield args, exc, None
+
+
 # region Formatting
 
 
 def _colored(text: str, color: int, end: str = '\n'):
     return f'\x1b[38;5;{color}m{text}\x1b[0m{end}'
 
 
@@ -315,11 +342,16 @@
     kwargs.setdefault('return_value', None)
     mock = Mock(*args, **kwargs)
     seal(mock)
     return mock
 
 
 @contextmanager
-def load_command(directory: Path, name: str, cmd_name: str) -> ContextManager[CommandCls]:
+def load_command(directory: Path, name: str, cmd_name: str, **kwargs) -> ContextManager[CommandCls]:
     path = directory.joinpath(name)
-    with Context.for_prog(path):
+    with Context.for_prog(path, **kwargs):
         yield load_commands(path)[cmd_name]
+
+
+class TemporaryDir(TemporaryDirectory):
+    def __enter__(self) -> Path:
+        return Path(self.name)
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/typing.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,39 +3,37 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, TypeVar, Type, Union, Optional, Collection, Sequence, TextIO, BinaryIO
-from typing import Tuple, List, Dict
+from typing import Pattern, Tuple, List, Dict
 
 if TYPE_CHECKING:
     from datetime import datetime, date, time, timedelta
     from enum import Enum
     from pathlib import Path
     from .commands import Command
     from .config import CommandConfig, AllowLeadingDash
     from .core import CommandMeta
     from .inputs import InputType
     from .parameters import Parameter, ParamGroup
-    from .utils import ValueSource
 
 T = TypeVar('T')
 T_co = TypeVar('T_co', covariant=True)
 TypeFunc = Callable[[str], T_co]
 
 NT = TypeVar('NT', bound=float, covariant=True)
 Number = Union[NT, None]
 NumType = Callable[[Union[str, float, int]], NT]
 RngType = Union[range, int, Sequence[int]]
 
-InputTypeFunc = Union[None, TypeFunc, 'InputType', range, Type['Enum']]
+InputTypeFunc = Union[None, TypeFunc, 'InputType', range, Type['Enum'], Pattern]
 ChoicesType = Optional[Collection[Any]]
-ValSrc = Union['ValueSource', Tuple['ValueSource', str]]
 
 Bool = Union[bool, Any]
 Strs = Union[str, Sequence[str]]
 OptStr = Optional[str]
 OptStrs = Optional[Strs]
 Strings = Collection[str]
 PathLike = Union[str, 'Path']
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser/utils.py` & `cli_command_parser-2023.6.14/lib/cli_command_parser/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Utilities for working with terminals, strings, and Enums.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from enum import Flag, Enum, EnumMeta
+from enum import Flag, EnumMeta
 from shutil import get_terminal_size
 from time import monotonic
 from typing import Any, Callable, TypeVar, List
 
 try:
     from enum import CONFORM
 except ImportError:
@@ -140,23 +140,28 @@
     def width(self) -> int:
         if monotonic() - self._last_time > self._cache_time:
             self._width = get_terminal_size()[0]
             self._last_time = monotonic()
         return self._width
 
 
-class ValueSource(Enum):
-    CLI = 'cli'
-    ENV = 'env'
-
-
 def str_to_bool(value: str) -> bool:
     try:
         return bool(int(value))
     except (TypeError, ValueError):
         pass
     lower = value.lower()
     if lower in {'t', 'true', 'y', 'yes'}:
         return True
     elif lower in {'f', 'false', 'n', 'no'}:
         return False
     raise ValueError(f'Unable to parse boolean value from {value=}')
+
+
+def positive_int(value: Any, expected: str = 'a positive integer', min_val: int = 0) -> int:
+    try:
+        value = int(value)
+    except (ValueError, TypeError) as e:
+        raise TypeError(f'Invalid {value=} - expected {expected} >= {min_val}') from e
+    if value < min_val:
+        raise ValueError(f'Invalid {value=} - expected {expected} >= {min_val}')
+    return value
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-command-parser
-Version: 2023.5.8
+Version: 2023.6.14
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 readme.rst
 requirements-dev.txt
 setup.cfg
 lib/cli_command_parser/__init__.py
 lib/cli_command_parser/__main__.py
 lib/cli_command_parser/__version__.py
-lib/cli_command_parser/actions.py
 lib/cli_command_parser/annotations.py
 lib/cli_command_parser/command_parameters.py
 lib/cli_command_parser/commands.py
 lib/cli_command_parser/compat.py
 lib/cli_command_parser/config.py
 lib/cli_command_parser/context.py
 lib/cli_command_parser/core.py
@@ -44,17 +43,19 @@
 lib/cli_command_parser/formatting/utils.py
 lib/cli_command_parser/inputs/__init__.py
 lib/cli_command_parser/inputs/base.py
 lib/cli_command_parser/inputs/choices.py
 lib/cli_command_parser/inputs/exceptions.py
 lib/cli_command_parser/inputs/files.py
 lib/cli_command_parser/inputs/numeric.py
+lib/cli_command_parser/inputs/patterns.py
 lib/cli_command_parser/inputs/time.py
 lib/cli_command_parser/inputs/utils.py
 lib/cli_command_parser/parameters/__init__.py
+lib/cli_command_parser/parameters/actions.py
 lib/cli_command_parser/parameters/base.py
 lib/cli_command_parser/parameters/choice_map.py
 lib/cli_command_parser/parameters/groups.py
 lib/cli_command_parser/parameters/option_strings.py
 lib/cli_command_parser/parameters/options.py
 lib/cli_command_parser/parameters/pass_thru.py
 lib/cli_command_parser/parameters/positionals.py
```

### Comparing `cli_command_parser-2023.5.8/readme.rst` & `cli_command_parser-2023.6.14/readme.rst`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.8/setup.cfg` & `cli_command_parser-2023.6.14/setup.cfg`

 * *Files identical despite different names*

