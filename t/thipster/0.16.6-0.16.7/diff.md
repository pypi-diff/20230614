# Comparing `tmp/thipster-0.16.6.tar.gz` & `tmp/thipster-0.16.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.16.6.tar", last modified: Wed Jun 14 08:35:10 2023, max compression
+gzip compressed data, was "thipster-0.16.7.tar", last modified: Wed Jun 14 09:18:27 2023, max compression
```

## Comparing `thipster-0.16.6.tar` & `thipster-0.16.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.366348 thipster-0.16.6/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-14 08:35:06.000000 thipster-0.16.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-14 08:35:06.000000 thipster-0.16.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-14 08:35:10.366348 thipster-0.16.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-14 08:35:06.000000 thipster-0.16.6/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-14 08:35:06.000000 thipster-0.16.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-14 08:35:06.000000 thipster-0.16.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 08:35:10.366348 thipster-0.16.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-14 08:35:06.000000 thipster-0.16.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.358348 thipster-0.16.6/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.358348 thipster-0.16.6/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.358348 thipster-0.16.6/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.358348 thipster-0.16.6/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15331 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     2405 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3304 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-14 08:35:06.000000 thipster-0.16.6/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.358348 thipster-0.16.6/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.362348 thipster-0.16.6/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.362348 thipster-0.16.6/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.362348 thipster-0.16.6/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.366348 thipster-0.16.6/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9156 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2924 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13471 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    20105 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.366348 thipster-0.16.6/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4653 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.366348 thipster-0.16.6/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19049 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-14 08:35:06.000000 thipster-0.16.6/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:35:10.362348 thipster-0.16.6/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-14 08:35:10.000000 thipster-0.16.6/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1774 2023-06-14 08:35:10.000000 thipster-0.16.6/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 08:35:10.000000 thipster-0.16.6/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 08:35:10.000000 thipster-0.16.6/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-14 08:35:10.000000 thipster-0.16.6/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.588561 thipster-0.16.7/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-14 09:18:24.000000 thipster-0.16.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-14 09:18:24.000000 thipster-0.16.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-14 09:18:27.588561 thipster-0.16.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-14 09:18:24.000000 thipster-0.16.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      986 2023-06-14 09:18:24.000000 thipster-0.16.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-14 09:18:24.000000 thipster-0.16.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 09:18:27.588561 thipster-0.16.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-14 09:18:25.000000 thipster-0.16.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15286 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     2405 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9156 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13471 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    20105 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6549 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.588561 thipster-0.16.7/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4653 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.588561 thipster-0.16.7/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19049 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.16.6/LICENSE` & `thipster-0.16.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/PKG-INFO` & `thipster-0.16.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,256 +1,271 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 6970  : 2.1.Name: thip
-00000020: 7374 6572 0a56 6572 7369 6f6e 3a20 302e  ster.Version: 0.
-00000030: 3136 2e36 0a53 756d 6d61 7279 3a20 5448  16.6.Summary: TH
-00000040: 6970 7374 6572 2069 7320 6120 746f 6f6c  ipster is a tool
-00000050: 2064 6564 6963 6174 6564 2074 6f20 7369   dedicated to si
-00000060: 6d70 6c69 6679 696e 6720 7468 6520 6469  mplifying the di
-00000070: 6666 6963 756c 7479 2061 7373 6f63 6961  fficulty associa
-00000080: 7465 6420 7769 7468 2077 7269 7469 6e67  ted with writing
-00000090: 2054 6572 7261 666f 726d 2066 696c 6573   Terraform files
-000000a0: 2e20 4974 2061 6c6c 6f77 7320 7573 6572  . It allows user
-000000b0: 7320 746f 2077 7269 7465 2069 6e66 7261  s to write infra
-000000c0: 7374 7275 6374 7572 6520 6173 2063 6f64  structure as cod
-000000d0: 6520 696e 2061 2073 696d 706c 6966 6965  e in a simplifie
-000000e0: 6420 666f 726d 6174 2c20 7573 696e 6720  d format, using 
-000000f0: 6569 7468 6572 2059 414d 4c20 2877 6974  either YAML (wit
-00000100: 6820 4a49 4e4a 4129 206f 7220 7468 6520  h JINJA) or the 
-00000110: 6465 6469 6361 7465 6420 5468 6970 7374  dedicated Thipst
-00000120: 6572 2044 534c 2e0a 486f 6d65 2d70 6167  er DSL..Home-pag
-00000130: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000140: 622e 636f 6d2f 5448 6970 7374 6572 2f54  b.com/THipster/T
-00000150: 4869 7073 7465 720a 446f 776e 6c6f 6164  Hipster.Download
-00000160: 2d55 524c 3a20 6874 7470 733a 2f2f 6769  -URL: https://gi
-00000170: 7468 7562 2e63 6f6d 2f54 4869 7073 7465  thub.com/THipste
-00000180: 722f 5448 6970 7374 6572 2e67 6974 0a43  r/THipster.git.C
-00000190: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-000001a0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-000001b0: 2031 202d 2050 6c61 6e6e 696e 670a 436c   1 - Planning.Cl
-000001c0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000001d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001e0: 3a20 5079 7468 6f6e 0a44 6573 6372 6970  : Python.Descrip
-000001f0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00000200: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00000210: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000220: 2074 6573 740a 5072 6f76 6964 6573 2d45   test.Provides-E
-00000230: 7874 7261 3a20 6465 760a 5072 6f76 6964  xtra: dev.Provid
-00000240: 6573 2d45 7874 7261 3a20 646f 630a 5072  es-Extra: doc.Pr
-00000250: 6f76 6964 6573 2d45 7874 7261 3a20 676f  ovides-Extra: go
-00000260: 6f67 6c65 0a4c 6963 656e 7365 2d46 696c  ogle.License-Fil
-00000270: 653a 204c 4943 454e 5345 0a0a 2320 5448  e: LICENSE..# TH
-00000280: 6970 7374 6572 0a0a 5448 6970 7374 6572  ipster..THipster
-00000290: 2069 7320 6120 746f 6f6c 2064 6564 6963   is a tool dedic
-000002a0: 6174 6564 2074 6f20 7369 6d70 6c69 6679  ated to simplify
-000002b0: 696e 6720 7468 6520 6469 6666 6963 756c  ing the difficul
-000002c0: 7479 2061 7373 6f63 6961 7465 6420 7769  ty associated wi
-000002d0: 7468 2077 7269 7469 6e67 2054 6572 7261  th writing Terra
-000002e0: 666f 726d 2066 696c 6573 2e0a 4974 2061  form files..It a
-000002f0: 6c6c 6f77 7320 7573 6572 7320 746f 2077  llows users to w
-00000300: 7269 7465 2069 6e66 7261 7374 7275 6374  rite infrastruct
-00000310: 7572 6520 6173 2063 6f64 6520 696e 2061  ure as code in a
-00000320: 2073 696d 706c 6966 6965 6420 666f 726d   simplified form
-00000330: 6174 2c20 7573 696e 6720 6569 7468 6572  at, using either
-00000340: 2059 414d 4c20 2877 6974 6820 4a49 4e4a   YAML (with JINJ
-00000350: 4129 206f 7220 7468 6520 6465 6469 6361  A) or the dedica
-00000360: 7465 6420 5468 6970 7374 6572 2044 534c  ted Thipster DSL
-00000370: 2e0a 0a57 7269 7474 656e 2065 6e74 6972  ...Written entir
-00000380: 656c 7920 696e 2050 7974 686f 6e2c 2069  ely in Python, i
-00000390: 7420 6c65 7665 7261 6765 7320 7468 6520  t leverages the 
-000003a0: 5079 7468 6f6e 2043 444b 2066 6f72 2054  Python CDK for T
-000003b0: 6572 7261 666f 726d 2074 6f20 6372 6561  erraform to crea
-000003c0: 7465 2054 6572 7261 666f 726d 2066 696c  te Terraform fil
-000003d0: 6573 2061 6e64 2061 7070 6c79 2074 6865  es and apply the
-000003e0: 6d20 746f 2074 6865 2063 686f 7365 6e20  m to the chosen 
-000003f0: 7072 6f76 6964 6572 2e0a 0a23 2320 5465  provider...## Te
-00000400: 6368 6e6f 6c6f 6779 2053 7461 636b 0a57  chnology Stack.W
-00000410: 7269 7474 656e 2069 6e20 5079 7468 6f6e  ritten in Python
-00000420: 2033 2e31 312c 2074 6869 7073 7465 7220   3.11, thipster 
-00000430: 6973 2064 6573 6967 6e65 6420 6173 2061  is designed as a
-00000440: 2070 7974 686f 6e20 7061 636b 6167 652c   python package,
-00000450: 2074 6f20 6265 2075 7365 6420 6569 7468   to be used eith
-00000460: 6572 2061 7320 6120 7374 616e 6461 6c6f  er as a standalo
-00000470: 6e65 2074 6f6f 6c2c 206f 7220 6173 2061  ne tool, or as a
-00000480: 206d 6f64 756c 6520 696e 7369 6465 2061   module inside a
-00000490: 2072 756e 6e69 6e67 2070 726f 6365 7373   running process
-000004a0: 206c 696b 6520 6120 4349 2f43 4420 7069   like a CI/CD pi
-000004b0: 7065 6c69 6e65 2e0a 0a23 2320 5072 6f6a  peline...## Proj
-000004c0: 6563 7420 5374 6174 7573 0a54 4869 7073  ect Status.THips
-000004d0: 7465 7220 6973 2063 7572 7265 6e74 6c79  ter is currently
-000004e0: 2069 6e20 616e 2061 6374 6976 6520 6465   in an active de
-000004f0: 7665 6c6f 706d 656e 7420 7374 6174 652e  velopment state.
-00000500: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
-00000510: 6b6e 6f77 206d 6f72 652c 2070 6c65 6173  know more, pleas
-00000520: 6520 6368 6563 6b20 7468 6520 5b43 4841  e check the [CHA
-00000530: 4e47 454c 4f47 5d28 6874 7470 733a 2f2f  NGELOG](https://
-00000540: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
-00000550: 7465 722f 5448 6970 7374 6572 2f62 6c6f  ter/THipster/blo
-00000560: 622f 6d61 696e 2f43 4841 4e47 454c 4f47  b/main/CHANGELOG
-00000570: 2e6d 6429 2066 6f72 206d 6f72 6520 6465  .md) for more de
-00000580: 7461 696c 732e 0a0a 2323 2044 6570 656e  tails...## Depen
-00000590: 6465 6e63 6965 730a 0a49 6e20 6f72 6465  dencies..In orde
-000005a0: 7220 746f 2075 7365 7220 5448 6970 7374  r to user THipst
-000005b0: 6572 2c20 796f 7520 7769 6c6c 206e 6565  er, you will nee
-000005c0: 6420 746f 2068 6176 6520 7468 6520 666f  d to have the fo
-000005d0: 6c6c 6f77 696e 6720 696e 7374 616c 6c65  llowing installe
-000005e0: 643a 0a2d 205b 5079 7468 6f6e 5d28 6874  d:.- [Python](ht
-000005f0: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000600: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
-00000610: 2028 332e 3131 2b29 0a2d 205b 7069 7065   (3.11+).- [pipe
-00000620: 6e76 5d28 6874 7470 733a 2f2f 7069 7065  nv](https://pipe
-00000630: 6e76 2e70 7970 612e 696f 2f65 6e2f 6c61  nv.pypa.io/en/la
-00000640: 7465 7374 2f29 2076 3230 3231 2e35 2b0a  test/) v2021.5+.
-00000650: 2d20 5b54 6572 7261 666f 726d 2043 4c49  - [Terraform CLI
-00000660: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00000670: 7065 722e 6861 7368 6963 6f72 702e 636f  per.hashicorp.co
-00000680: 6d2f 7465 7272 6166 6f72 6d2f 7475 746f  m/terraform/tuto
-00000690: 7269 616c 732f 6177 732d 6765 742d 7374  rials/aws-get-st
-000006a0: 6172 7465 642f 696e 7374 616c 6c2d 636c  arted/install-cl
-000006b0: 6929 2028 312e 322b 290a 2d20 5b4e 6f64  i) (1.2+).- [Nod
-000006c0: 652e 6a73 5d28 6874 7470 733a 2f2f 6e6f  e.js](https://no
-000006d0: 6465 6a73 2e6f 7267 2f29 2061 6e64 206e  dejs.org/) and n
-000006e0: 706d 2076 3136 2b2e 0a0a 2323 2049 6e73  pm v16+...## Ins
-000006f0: 7461 6c6c 6174 696f 6e0a 0a54 6f20 7573  tallation..To us
-00000700: 6520 5448 6970 7374 6572 2c20 796f 7520  e THipster, you 
-00000710: 6361 6e20 7369 6d70 6c79 2069 6e73 7461  can simply insta
-00000720: 6c6c 2074 6865 2070 6163 6b61 6765 2077  ll the package w
-00000730: 6974 6820 7069 703a 0a0a 6060 6063 6f6e  ith pip:..```con
-00000740: 736f 6c65 0a70 6970 2069 6e73 7461 6c6c  sole.pip install
-00000750: 2074 6869 7073 7465 720a 6060 600a 0a49   thipster.```..I
-00000760: 6620 796f 7520 7761 6e74 2074 6f20 696e  f you want to in
-00000770: 7374 616c 6c20 7468 6520 676f 6f67 6c65  stall the google
-00000780: 2064 6570 656e 6465 6e63 6965 7320 6173   dependencies as
-00000790: 7765 6c6c 2075 7365 0a0a 6060 6063 6f6e  well use..```con
-000007a0: 736f 6c65 0a70 6970 2069 6e73 7461 6c6c  sole.pip install
-000007b0: 2074 6869 7073 7465 725b 676f 6f67 6c65   thipster[google
-000007c0: 5d0a 6060 600a 0a54 6865 206c 6973 7420  ].```..The list 
-000007d0: 6f66 2061 7661 696c 6162 6c65 2076 6572  of available ver
-000007e0: 7369 6f6e 7320 6361 6e20 6265 2066 6f75  sions can be fou
-000007f0: 6e64 206f 6e20 5b50 7950 495d 2868 7474  nd on [PyPI](htt
-00000800: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000810: 6f6a 6563 742f 7468 6970 7374 6572 2f29  oject/thipster/)
-00000820: 2e0a 0a23 2320 5573 6167 650a 0a59 6f75  ...## Usage..You
-00000830: 2063 616e 2075 7365 2054 4869 7073 7465   can use THipste
-00000840: 7220 696e 2074 776f 2077 6179 733a 0a2d  r in two ways:.-
-00000850: 2042 7920 6c65 7665 7261 6769 6e67 2074   By leveraging t
-00000860: 6865 205b 5448 6970 7374 6572 2043 4c49  he [THipster CLI
-00000870: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000880: 2e63 6f6d 2f54 4869 7073 7465 722f 5448  .com/THipster/TH
-00000890: 6970 7374 6572 2d63 6c69 290a 2d20 4279  ipster-cli).- By
-000008a0: 2064 6972 6563 746c 7920 7573 696e 6720   directly using 
-000008b0: 7468 6520 5b54 4869 7073 7465 7220 5079  the [THipster Py
-000008c0: 7468 6f6e 2070 6163 6b61 6765 5d28 6874  thon package](ht
-000008d0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-000008e0: 726f 6a65 6374 2f74 6869 7073 7465 722f  roject/thipster/
-000008f0: 2920 696e 2079 6f75 7220 6f77 6e20 636f  ) in your own co
-00000900: 6465 0a0a 4d61 696e 2066 6561 7475 7265  de..Main feature
-00000910: 3a0a 2d20 4765 6e65 7261 7465 2054 6572  :.- Generate Ter
-00000920: 7261 666f 726d 2066 696c 6573 2066 726f  raform files fro
-00000930: 6d20 6120 5941 4d4c 2b4a 494e 4a41 206f  m a YAML+JINJA o
-00000940: 7220 5448 4950 5320 6669 6c65 3a0a 6060  r THIPS file:.``
-00000950: 6070 7974 686f 6e0a 6672 6f6d 2074 6869  `python.from thi
-00000960: 7073 7465 7220 696d 706f 7274 2045 6e67  pster import Eng
-00000970: 696e 6520 6173 2054 6869 7073 7465 7245  ine as ThipsterE
-00000980: 6e67 696e 650a 6672 6f6d 2074 6869 7073  ngine.from thips
-00000990: 7465 722e 6175 7468 2069 6d70 6f72 7420  ter.auth import 
-000009a0: 476f 6f67 6c65 0a66 726f 6d20 7468 6970  Google.from thip
-000009b0: 7374 6572 2e70 6172 7365 7220 696d 706f  ster.parser impo
-000009c0: 7274 2050 6172 7365 7246 6163 746f 7279  rt ParserFactory
-000009d0: 0a66 726f 6d20 7468 6970 7374 6572 2e72  .from thipster.r
-000009e0: 6570 6f73 6974 6f72 7920 696d 706f 7274  epository import
-000009f0: 2047 6974 6875 6252 6570 6f0a 6672 6f6d   GithubRepo.from
-00000a00: 2074 6869 7073 7465 722e 7465 7272 6166   thipster.terraf
-00000a10: 6f72 6d20 696d 706f 7274 2054 6572 7261  orm import Terra
-00000a20: 666f 726d 0a0a 2320 6372 6561 7465 206e  form..# create n
-00000a30: 6577 2054 4869 7073 7465 7220 656e 6769  ew THipster engi
-00000a40: 6e65 0a65 6e67 696e 6520 3d20 5468 6970  ne.engine = Thip
-00000a50: 7374 6572 456e 6769 6e65 2850 6172 7365  sterEngine(Parse
-00000a60: 7246 6163 746f 7279 2829 2c20 4769 7468  rFactory(), Gith
-00000a70: 7562 5265 706f 2827 5448 6970 7374 6572  ubRepo('THipster
-00000a80: 2f6d 6f64 656c 7327 292c 2047 6f6f 676c  /models'), Googl
-00000a90: 652c 2054 6572 7261 666f 726d 2829 290a  e, Terraform()).
-00000aa0: 0a23 2067 656e 6572 6174 6520 5465 7272  .# generate Terr
-00000ab0: 6166 6f72 6d20 6669 6c65 7320 616e 6420  aform files and 
-00000ac0: 706c 616e 2066 726f 6d20 6120 5941 4d4c  plan from a YAML
-00000ad0: 2b4a 494e 4a41 2066 696c 650a 7465 7272  +JINJA file.terr
-00000ae0: 6166 6f72 6d5f 706c 616e 203d 2065 6e67  aform_plan = eng
-00000af0: 696e 652e 7275 6e28 2770 6174 682f 746f  ine.run('path/to
-00000b00: 2f66 696c 652f 6f72 2f64 6972 6563 746f  /file/or/directo
-00000b10: 7279 2729 0a70 7269 6e74 2874 6572 7261  ry').print(terra
-00000b20: 666f 726d 5f70 6c61 6e29 0a60 6060 0a0a  form_plan).```..
-00000b30: 2323 2048 6f77 2074 6f20 7465 7374 2074  ## How to test t
-00000b40: 6865 2073 6f66 7477 6172 650a 0a54 6f20  he software..To 
-00000b50: 7275 6e20 7468 6520 7465 7374 732c 2079  run the tests, y
-00000b60: 6f75 2063 616e 2075 7365 2074 6865 2066  ou can use the f
-00000b70: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00000b80: 3a0a 0a60 6060 636f 6e73 6f6c 650a 7069  :..```console.pi
-00000b90: 7020 696e 7374 616c 6c20 2d65 202e 5b74  p install -e .[t
-00000ba0: 6573 745d 0a70 7974 6573 7420 7465 7374  est].pytest test
-00000bb0: 730a 6060 600a 0a23 2320 4b6e 6f77 6e20  s.```..## Known 
-00000bc0: 6973 7375 6573 0a0a 416c 6c20 6b6e 6f77  issues..All know
-00000bd0: 6e20 6973 7375 6573 2c20 6275 6773 2c20  n issues, bugs, 
-00000be0: 616e 6420 6665 6174 7572 6520 7265 7175  and feature requ
-00000bf0: 6573 7473 2061 7265 2074 7261 636b 6564  ests are tracked
-00000c00: 2069 6e20 7468 6520 5b49 7373 7565 2074   in the [Issue t
-00000c10: 7261 636b 6572 5d28 6874 7470 733a 2f2f  racker](https://
-00000c20: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
-00000c30: 7465 722f 5448 6970 7374 6572 2f69 7373  ter/THipster/iss
-00000c40: 7565 7329 2e0a 0a23 2320 4765 7474 696e  ues)...## Gettin
-00000c50: 6720 6865 6c70 0a0a 4966 2079 6f75 2068  g help..If you h
-00000c60: 6176 6520 7175 6573 7469 6f6e 732c 2063  ave questions, c
-00000c70: 6f6e 6365 726e 732c 2062 7567 2072 6570  oncerns, bug rep
-00000c80: 6f72 7473 2c20 6574 632c 2070 6c65 6173  orts, etc, pleas
-00000c90: 6520 6669 6c65 2061 6e20 6973 7375 6520  e file an issue 
-00000ca0: 696e 2074 6869 7320 7265 706f 7369 746f  in this reposito
-00000cb0: 7279 2773 205b 4973 7375 6520 7472 6163  ry's [Issue trac
-00000cc0: 6b65 725d 2868 7474 7073 3a2f 2f67 6974  ker](https://git
-00000cd0: 6875 622e 636f 6d2f 5448 6970 7374 6572  hub.com/THipster
-00000ce0: 2f54 4869 7073 7465 722f 6973 7375 6573  /THipster/issues
-00000cf0: 292e 0a0a 2323 2047 6574 7469 6e67 2069  )...## Getting i
-00000d00: 6e76 6f6c 7665 640a 0a54 6f20 696e 7374  nvolved..To inst
-00000d10: 616c 6c20 7468 6520 7072 6f6a 6563 7420  all the project 
-00000d20: 666f 7220 6465 7665 6c6f 706d 656e 742c  for development,
-00000d30: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00000d40: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000d50: 6e64 3a0a 0a60 6060 636f 6e73 6f6c 650a  nd:..```console.
-00000d60: 7069 7020 696e 7374 616c 6c20 2d72 2072  pip install -r r
-00000d70: 6571 7569 7265 6d65 6e74 732e 7478 7420  equirements.txt 
-00000d80: 2626 2070 6970 2069 6e73 7461 6c6c 202d  && pip install -
-00000d90: 6520 2e5b 6465 762c 7465 7374 2c64 6f63  e .[dev,test,doc
-00000da0: 2c67 6f6f 676c 655d 0a70 7265 2d63 6f6d  ,google].pre-com
-00000db0: 6d69 7420 696e 7374 616c 6c20 2626 2070  mit install && p
-00000dc0: 7265 2d63 6f6d 6d69 7420 7275 6e20 2d2d  re-commit run --
-00000dd0: 616c 6c2d 6669 6c65 730a 6060 600a 0a46  all-files.```..F
-00000de0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00000df0: 696f 6e20 6f6e 2068 6f77 2074 6f20 6865  ion on how to he
-00000e00: 6c70 206f 7574 2c20 706c 6561 7365 2063  lp out, please c
-00000e10: 6865 636b 2074 6865 205b 434f 4e54 5249  heck the [CONTRI
-00000e20: 4255 5449 4e47 5d28 6874 7470 733a 2f2f  BUTING](https://
-00000e30: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
-00000e40: 7465 722f 5448 6970 7374 6572 2f62 6c6f  ter/THipster/blo
-00000e50: 622f 6d61 696e 2f43 4f4e 5452 4942 5554  b/main/CONTRIBUT
-00000e60: 494e 472e 6d64 2920 6669 6c65 2e0a 0a23  ING.md) file...#
-00000e70: 2320 4f70 656e 2073 6f75 7263 6520 6c69  # Open source li
-00000e80: 6365 6e73 696e 6720 696e 666f 0a31 2e20  censing info.1. 
-00000e90: 5b4c 4943 454e 5345 5d28 6874 7470 733a  [LICENSE](https:
-00000ea0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 4869  //github.com/THi
-00000eb0: 7073 7465 722f 5448 6970 7374 6572 2f62  pster/THipster/b
-00000ec0: 6c6f 622f 6d61 696e 2f4c 4943 454e 5345  lob/main/LICENSE
-00000ed0: 290a 322e 205b 4346 5042 2053 6f75 7263  ).2. [CFPB Sourc
-00000ee0: 6520 436f 6465 2050 6f6c 6963 795d 2868  e Code Policy](h
-00000ef0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000f00: 6d2f 6366 7062 2f73 6f75 7263 652d 636f  m/cfpb/source-co
-00000f10: 6465 2d70 6f6c 6963 792f 290a 0a23 2320  de-policy/)..## 
-00000f20: 4372 6564 6974 7320 616e 6420 7265 6665  Credits and refe
-00000f30: 7265 6e63 6573 0a0a 312e 2050 726f 6a65  rences..1. Proje
-00000f40: 6374 7320 7468 6174 2069 6e73 7069 7265  cts that inspire
-00000f50: 6420 796f 750a 2020 2020 2d20 5b41 5753  d you.    - [AWS
-00000f60: 2041 7070 6c69 6361 7469 6f6e 2043 6f6d   Application Com
-00000f70: 706f 7365 725d 2868 7474 7073 3a2f 2f61  poser](https://a
-00000f80: 7773 2e61 6d61 7a6f 6e2e 636f 6d2f 6170  ws.amazon.com/ap
-00000f90: 706c 6963 6174 696f 6e2d 636f 6d70 6f73  plication-compos
-00000fa0: 6572 2f3f 6e63 313d 685f 6c73 290a 322e  er/?nc1=h_ls).2.
-00000fb0: 2052 656c 6174 6564 2070 726f 6a65 6374   Related project
-00000fc0: 730a 2020 2020 2d20 5b57 696e 6720 5072  s.    - [Wing Pr
-00000fd0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000fe0: 6765 5d28 6874 7470 733a 2f2f 7777 772e  ge](https://www.
-00000ff0: 7769 6e67 6c61 6e67 2e69 6f2f 290a       winglang.io/).
+00000000: 2320 5448 6970 7374 6572 0a0a 5448 6970  # THipster..THip
+00000010: 7374 6572 2069 7320 6120 746f 6f6c 2064  ster is a tool d
+00000020: 6564 6963 6174 6564 2074 6f20 7369 6d70  edicated to simp
+00000030: 6c69 6679 696e 6720 7468 6520 6469 6666  lifying the diff
+00000040: 6963 756c 7479 2061 7373 6f63 6961 7465  iculty associate
+00000050: 6420 7769 7468 2077 7269 7469 6e67 2054  d with writing T
+00000060: 6572 7261 666f 726d 2066 696c 6573 2e0a  erraform files..
+00000070: 4974 2061 6c6c 6f77 7320 7573 6572 7320  It allows users 
+00000080: 746f 2077 7269 7465 2069 6e66 7261 7374  to write infrast
+00000090: 7275 6374 7572 6520 6173 2063 6f64 6520  ructure as code 
+000000a0: 696e 2061 2073 696d 706c 6966 6965 6420  in a simplified 
+000000b0: 666f 726d 6174 2c20 7573 696e 6720 6569  format, using ei
+000000c0: 7468 6572 2059 414d 4c20 2877 6974 6820  ther YAML (with 
+000000d0: 4a49 4e4a 4129 206f 7220 7468 6520 6465  JINJA) or the de
+000000e0: 6469 6361 7465 6420 5468 6970 7374 6572  dicated Thipster
+000000f0: 2044 534c 2e0a 0a57 7269 7474 656e 2065   DSL...Written e
+00000100: 6e74 6972 656c 7920 696e 2050 7974 686f  ntirely in Pytho
+00000110: 6e2c 2069 7420 6c65 7665 7261 6765 7320  n, it leverages 
+00000120: 7468 6520 5079 7468 6f6e 2043 444b 2066  the Python CDK f
+00000130: 6f72 2054 6572 7261 666f 726d 2074 6f20  or Terraform to 
+00000140: 6372 6561 7465 2054 6572 7261 666f 726d  create Terraform
+00000150: 2066 696c 6573 2061 6e64 2061 7070 6c79   files and apply
+00000160: 2074 6865 6d20 746f 2074 6865 2063 686f   them to the cho
+00000170: 7365 6e20 7072 6f76 6964 6572 2e0a 0a3c  sen provider...<
+00000180: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000190: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+000001a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001b0: 5448 6970 7374 6572 2f54 4869 7073 7465  THipster/THipste
+000001c0: 722f 626c 6f62 2f6d 6169 6e2f 4c49 4345  r/blob/main/LICE
+000001d0: 4e53 4522 2074 6172 6765 743d 225f 626c  NSE" target="_bl
+000001e0: 616e 6b22 2061 6c74 3d22 4c69 6365 6e73  ank" alt="Licens
+000001f0: 6522 3e0a 2020 2020 3c69 6d67 2073 7263  e">.    <img src
+00000200: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000210: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000220: 6c69 6365 6e73 652f 5448 6970 7374 6572  license/THipster
+00000230: 2f54 4869 7073 7465 7222 2061 6c74 3d22  /THipster" alt="
+00000240: 4c69 6365 6e73 6522 3e0a 2020 3c2f 613e  License">.  </a>
+00000250: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000260: 733a 2f2f 7468 6970 7374 6572 2e72 6561  s://thipster.rea
+00000270: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000280: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
+00000290: 6573 7422 2074 6172 6765 743d 225f 626c  est" target="_bl
+000002a0: 616e 6b22 2061 6c74 3d22 5265 6164 2074  ank" alt="Read t
+000002b0: 6865 2064 6f63 7320 646f 6375 6d65 6e74  he docs document
+000002c0: 6174 696f 6e22 3e0a 2020 2020 3c69 6d67  ation">.    <img
+000002d0: 2073 7263 3d22 6874 7470 733a 2f2f 7265   src="https://re
+000002e0: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+000002f0: 6f6a 6563 7473 2f74 6869 7073 7465 722f  ojects/thipster/
+00000300: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000310: 6174 6573 7422 2061 6c74 3d22 5265 6164  atest" alt="Read
+00000320: 2074 6865 2064 6f63 7320 646f 6375 6d65   the docs docume
+00000330: 6e74 6174 696f 6e22 3e0a 2020 3c2f 613e  ntation">.  </a>
+00000340: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000350: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000360: 6a65 6374 2f74 6869 7073 7465 722f 2220  ject/thipster/" 
+00000370: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
+00000380: 616c 743d 2250 7950 6920 7061 636b 6167  alt="PyPi packag
+00000390: 6522 3e0a 2020 2020 3c69 6d67 2073 7263  e">.    <img src
+000003a0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000003b0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+000003c0: 7468 6970 7374 6572 3f63 6f6c 6f72 3d62  thipster?color=b
+000003d0: 7269 6768 7467 7265 656e 266c 6162 656c  rightgreen&label
+000003e0: 3d70 7970 6925 3230 7061 636b 6167 6522  =pypi%20package"
+000003f0: 2061 6c74 3d22 5061 636b 6167 6520 7665   alt="Package ve
+00000400: 7273 696f 6e22 3e0a 2020 3c2f 613e 0a20  rsion">.  </a>. 
+00000410: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000420: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000430: 6374 2f74 6869 7073 7465 722f 2220 7461  ct/thipster/" ta
+00000440: 7267 6574 3d22 5f62 6c61 6e6b 2220 616c  rget="_blank" al
+00000450: 743d 2250 7950 6920 7061 636b 6167 6522  t="PyPi package"
+00000460: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00000470: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000480: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000490: 7273 696f 6e73 2f74 6869 7073 7465 723f  rsions/thipster?
+000004a0: 636f 6c6f 723d 6272 6967 6874 6772 6565  color=brightgree
+000004b0: 6e22 2061 6c74 3d22 5375 7070 6f72 7465  n" alt="Supporte
+000004c0: 6420 5079 7468 6f6e 2076 6572 7369 6f6e  d Python version
+000004d0: 7322 3e0a 2020 3c2f 613e 0a3c 2f70 3e0a  s">.  </a>.</p>.
+000004e0: 0a23 2320 5465 6368 6e6f 6c6f 6779 2053  .## Technology S
+000004f0: 7461 636b 0a57 7269 7474 656e 2069 6e20  tack.Written in 
+00000500: 5079 7468 6f6e 2033 2e31 312c 2074 6869  Python 3.11, thi
+00000510: 7073 7465 7220 6973 2064 6573 6967 6e65  pster is designe
+00000520: 6420 6173 2061 2070 7974 686f 6e20 7061  d as a python pa
+00000530: 636b 6167 652c 2074 6f20 6265 2075 7365  ckage, to be use
+00000540: 6420 6569 7468 6572 2061 7320 6120 7374  d either as a st
+00000550: 616e 6461 6c6f 6e65 2074 6f6f 6c2c 206f  andalone tool, o
+00000560: 7220 6173 2061 206d 6f64 756c 6520 696e  r as a module in
+00000570: 7369 6465 2061 2072 756e 6e69 6e67 2070  side a running p
+00000580: 726f 6365 7373 206c 696b 6520 6120 4349  rocess like a CI
+00000590: 2f43 4420 7069 7065 6c69 6e65 2e0a 0a23  /CD pipeline...#
+000005a0: 2320 5072 6f6a 6563 7420 5374 6174 7573  # Project Status
+000005b0: 0a54 4869 7073 7465 7220 6973 2063 7572  .THipster is cur
+000005c0: 7265 6e74 6c79 2069 6e20 616e 2061 6374  rently in an act
+000005d0: 6976 6520 6465 7665 6c6f 706d 656e 7420  ive development 
+000005e0: 7374 6174 652e 2049 6620 796f 7520 7761  state. If you wa
+000005f0: 6e74 2074 6f20 6b6e 6f77 206d 6f72 652c  nt to know more,
+00000600: 2070 6c65 6173 6520 6368 6563 6b20 7468   please check th
+00000610: 6520 5b43 4841 4e47 454c 4f47 5d28 6874  e [CHANGELOG](ht
+00000620: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000630: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00000640: 6572 2f62 6c6f 622f 6d61 696e 2f43 4841  er/blob/main/CHA
+00000650: 4e47 454c 4f47 2e6d 6429 2066 6f72 206d  NGELOG.md) for m
+00000660: 6f72 6520 6465 7461 696c 732e 0a0a 2323  ore details...##
+00000670: 2044 6570 656e 6465 6e63 6965 730a 0a49   Dependencies..I
+00000680: 6e20 6f72 6465 7220 746f 2075 7365 7220  n order to user 
+00000690: 5448 6970 7374 6572 2c20 796f 7520 7769  THipster, you wi
+000006a0: 6c6c 206e 6565 6420 746f 2068 6176 6520  ll need to have 
+000006b0: 7468 6520 666f 6c6c 6f77 696e 6720 696e  the following in
+000006c0: 7374 616c 6c65 643a 0a2d 205b 5079 7468  stalled:.- [Pyth
+000006d0: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
+000006e0: 7079 7468 6f6e 2e6f 7267 2f64 6f77 6e6c  python.org/downl
+000006f0: 6f61 6473 2f29 2028 332e 3131 2b29 0a2d  oads/) (3.11+).-
+00000700: 205b 7069 7065 6e76 5d28 6874 7470 733a   [pipenv](https:
+00000710: 2f2f 7069 7065 6e76 2e70 7970 612e 696f  //pipenv.pypa.io
+00000720: 2f65 6e2f 6c61 7465 7374 2f29 2076 3230  /en/latest/) v20
+00000730: 3231 2e35 2b0a 2d20 5b54 6572 7261 666f  21.5+.- [Terrafo
+00000740: 726d 2043 4c49 5d28 6874 7470 733a 2f2f  rm CLI](https://
+00000750: 6465 7665 6c6f 7065 722e 6861 7368 6963  developer.hashic
+00000760: 6f72 702e 636f 6d2f 7465 7272 6166 6f72  orp.com/terrafor
+00000770: 6d2f 7475 746f 7269 616c 732f 6177 732d  m/tutorials/aws-
+00000780: 6765 742d 7374 6172 7465 642f 696e 7374  get-started/inst
+00000790: 616c 6c2d 636c 6929 2028 312e 322b 290a  all-cli) (1.2+).
+000007a0: 2d20 5b4e 6f64 652e 6a73 5d28 6874 7470  - [Node.js](http
+000007b0: 733a 2f2f 6e6f 6465 6a73 2e6f 7267 2f29  s://nodejs.org/)
+000007c0: 2061 6e64 206e 706d 2076 3136 2b2e 0a0a   and npm v16+...
+000007d0: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
+000007e0: 0a54 6f20 7573 6520 5448 6970 7374 6572  .To use THipster
+000007f0: 2c20 796f 7520 6361 6e20 7369 6d70 6c79  , you can simply
+00000800: 2069 6e73 7461 6c6c 2074 6865 2070 6163   install the pac
+00000810: 6b61 6765 2077 6974 6820 7069 703a 0a0a  kage with pip:..
+00000820: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
+00000830: 6e73 7461 6c6c 2074 6869 7073 7465 720a  nstall thipster.
+00000840: 6060 600a 0a49 6620 796f 7520 7761 6e74  ```..If you want
+00000850: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+00000860: 676f 6f67 6c65 2064 6570 656e 6465 6e63  google dependenc
+00000870: 6965 7320 6173 7765 6c6c 2075 7365 0a0a  ies aswell use..
+00000880: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
+00000890: 6e73 7461 6c6c 2074 6869 7073 7465 725b  nstall thipster[
+000008a0: 676f 6f67 6c65 5d0a 6060 600a 0a54 6865  google].```..The
+000008b0: 206c 6973 7420 6f66 2061 7661 696c 6162   list of availab
+000008c0: 6c65 2076 6572 7369 6f6e 7320 6361 6e20  le versions can 
+000008d0: 6265 2066 6f75 6e64 206f 6e20 5b50 7950  be found on [PyP
+000008e0: 495d 2868 7474 7073 3a2f 2f70 7970 692e  I](https://pypi.
+000008f0: 6f72 672f 7072 6f6a 6563 742f 7468 6970  org/project/thip
+00000900: 7374 6572 2f29 2e0a 0a23 2320 5573 6167  ster/)...## Usag
+00000910: 650a 0a59 6f75 2063 616e 2075 7365 2054  e..You can use T
+00000920: 4869 7073 7465 7220 696e 2074 776f 2077  Hipster in two w
+00000930: 6179 733a 0a2d 2042 7920 6c65 7665 7261  ays:.- By levera
+00000940: 6769 6e67 2074 6865 205b 5448 6970 7374  ging the [THipst
+00000950: 6572 2043 4c49 5d28 6874 7470 733a 2f2f  er CLI](https://
+00000960: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
+00000970: 7465 722f 5448 6970 7374 6572 2d63 6c69  ter/THipster-cli
+00000980: 290a 2d20 4279 2064 6972 6563 746c 7920  ).- By directly 
+00000990: 7573 696e 6720 7468 6520 5b54 4869 7073  using the [THips
+000009a0: 7465 7220 5079 7468 6f6e 2070 6163 6b61  ter Python packa
+000009b0: 6765 5d28 6874 7470 733a 2f2f 7079 7069  ge](https://pypi
+000009c0: 2e6f 7267 2f70 726f 6a65 6374 2f74 6869  .org/project/thi
+000009d0: 7073 7465 722f 2920 696e 2079 6f75 7220  pster/) in your 
+000009e0: 6f77 6e20 636f 6465 0a0a 4d61 696e 2066  own code..Main f
+000009f0: 6561 7475 7265 3a0a 2d20 4765 6e65 7261  eature:.- Genera
+00000a00: 7465 2054 6572 7261 666f 726d 2066 696c  te Terraform fil
+00000a10: 6573 2066 726f 6d20 6120 5941 4d4c 2b4a  es from a YAML+J
+00000a20: 494e 4a41 206f 7220 5448 4950 5320 6669  INJA or THIPS fi
+00000a30: 6c65 3a0a 6060 6070 7974 686f 6e0a 6672  le:.```python.fr
+00000a40: 6f6d 2074 6869 7073 7465 7220 696d 706f  om thipster impo
+00000a50: 7274 2045 6e67 696e 6520 6173 2054 6869  rt Engine as Thi
+00000a60: 7073 7465 7245 6e67 696e 650a 6672 6f6d  psterEngine.from
+00000a70: 2074 6869 7073 7465 722e 6175 7468 2069   thipster.auth i
+00000a80: 6d70 6f72 7420 476f 6f67 6c65 0a66 726f  mport Google.fro
+00000a90: 6d20 7468 6970 7374 6572 2e70 6172 7365  m thipster.parse
+00000aa0: 7220 696d 706f 7274 2050 6172 7365 7246  r import ParserF
+00000ab0: 6163 746f 7279 0a66 726f 6d20 7468 6970  actory.from thip
+00000ac0: 7374 6572 2e72 6570 6f73 6974 6f72 7920  ster.repository 
+00000ad0: 696d 706f 7274 2047 6974 6875 6252 6570  import GithubRep
+00000ae0: 6f0a 6672 6f6d 2074 6869 7073 7465 722e  o.from thipster.
+00000af0: 7465 7272 6166 6f72 6d20 696d 706f 7274  terraform import
+00000b00: 2054 6572 7261 666f 726d 0a0a 2320 6372   Terraform..# cr
+00000b10: 6561 7465 206e 6577 2054 4869 7073 7465  eate new THipste
+00000b20: 7220 656e 6769 6e65 0a65 6e67 696e 6520  r engine.engine 
+00000b30: 3d20 5468 6970 7374 6572 456e 6769 6e65  = ThipsterEngine
+00000b40: 2850 6172 7365 7246 6163 746f 7279 2829  (ParserFactory()
+00000b50: 2c20 4769 7468 7562 5265 706f 2827 5448  , GithubRepo('TH
+00000b60: 6970 7374 6572 2f6d 6f64 656c 7327 292c  ipster/models'),
+00000b70: 2047 6f6f 676c 652c 2054 6572 7261 666f   Google, Terrafo
+00000b80: 726d 2829 290a 0a23 2067 656e 6572 6174  rm())..# generat
+00000b90: 6520 5465 7272 6166 6f72 6d20 6669 6c65  e Terraform file
+00000ba0: 7320 616e 6420 706c 616e 2066 726f 6d20  s and plan from 
+00000bb0: 6120 5941 4d4c 2b4a 494e 4a41 2066 696c  a YAML+JINJA fil
+00000bc0: 650a 7465 7272 6166 6f72 6d5f 706c 616e  e.terraform_plan
+00000bd0: 203d 2065 6e67 696e 652e 7275 6e28 2770   = engine.run('p
+00000be0: 6174 682f 746f 2f66 696c 652f 6f72 2f64  ath/to/file/or/d
+00000bf0: 6972 6563 746f 7279 2729 0a70 7269 6e74  irectory').print
+00000c00: 2874 6572 7261 666f 726d 5f70 6c61 6e29  (terraform_plan)
+00000c10: 0a60 6060 0a0a 2323 2048 6f77 2074 6f20  .```..## How to 
+00000c20: 7465 7374 2074 6865 2073 6f66 7477 6172  test the softwar
+00000c30: 650a 0a54 6f20 7275 6e20 7468 6520 7465  e..To run the te
+00000c40: 7374 732c 2079 6f75 2063 616e 2075 7365  sts, you can use
+00000c50: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00000c60: 6f6d 6d61 6e64 3a0a 0a60 6060 636f 6e73  ommand:..```cons
+00000c70: 6f6c 650a 7069 7020 696e 7374 616c 6c20  ole.pip install 
+00000c80: 2d65 202e 5b74 6573 745d 0a70 7974 6573  -e .[test].pytes
+00000c90: 7420 7465 7374 730a 6060 600a 0a23 2320  t tests.```..## 
+00000ca0: 4b6e 6f77 6e20 6973 7375 6573 0a0a 416c  Known issues..Al
+00000cb0: 6c20 6b6e 6f77 6e20 6973 7375 6573 2c20  l known issues, 
+00000cc0: 6275 6773 2c20 616e 6420 6665 6174 7572  bugs, and featur
+00000cd0: 6520 7265 7175 6573 7473 2061 7265 2074  e requests are t
+00000ce0: 7261 636b 6564 2069 6e20 7468 6520 5b49  racked in the [I
+00000cf0: 7373 7565 2074 7261 636b 6572 5d28 6874  ssue tracker](ht
+00000d00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000d10: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00000d20: 6572 2f69 7373 7565 7329 2e0a 0a23 2320  er/issues)...## 
+00000d30: 4765 7474 696e 6720 6865 6c70 0a0a 4966  Getting help..If
+00000d40: 2079 6f75 2068 6176 6520 7175 6573 7469   you have questi
+00000d50: 6f6e 732c 2063 6f6e 6365 726e 732c 2062  ons, concerns, b
+00000d60: 7567 2072 6570 6f72 7473 2c20 6574 632c  ug reports, etc,
+00000d70: 2070 6c65 6173 6520 6669 6c65 2061 6e20   please file an 
+00000d80: 6973 7375 6520 696e 2074 6869 7320 7265  issue in this re
+00000d90: 706f 7369 746f 7279 2773 205b 4973 7375  pository's [Issu
+00000da0: 6520 7472 6163 6b65 725d 2868 7474 7073  e tracker](https
+00000db0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5448  ://github.com/TH
+00000dc0: 6970 7374 6572 2f54 4869 7073 7465 722f  ipster/THipster/
+00000dd0: 6973 7375 6573 292e 0a0a 2323 2047 6574  issues)...## Get
+00000de0: 7469 6e67 2069 6e76 6f6c 7665 640a 0a54  ting involved..T
+00000df0: 6f20 696e 7374 616c 6c20 7468 6520 7072  o install the pr
+00000e00: 6f6a 6563 7420 666f 7220 6465 7665 6c6f  oject for develo
+00000e10: 706d 656e 742c 2079 6f75 2063 616e 2075  pment, you can u
+00000e20: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00000e30: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 636f   command:..```co
+00000e40: 6e73 6f6c 650a 7069 7020 696e 7374 616c  nsole.pip instal
+00000e50: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
+00000e60: 732e 7478 7420 2626 2070 6970 2069 6e73  s.txt && pip ins
+00000e70: 7461 6c6c 202d 6520 2e5b 6465 762c 7465  tall -e .[dev,te
+00000e80: 7374 2c64 6f63 2c67 6f6f 676c 655d 0a70  st,doc,google].p
+00000e90: 7265 2d63 6f6d 6d69 7420 696e 7374 616c  re-commit instal
+00000ea0: 6c20 2626 2070 7265 2d63 6f6d 6d69 7420  l && pre-commit 
+00000eb0: 7275 6e20 2d2d 616c 6c2d 6669 6c65 730a  run --all-files.
+00000ec0: 6060 600a 0a46 6f72 206d 6f72 6520 696e  ```..For more in
+00000ed0: 666f 726d 6174 696f 6e20 6f6e 2068 6f77  formation on how
+00000ee0: 2074 6f20 6865 6c70 206f 7574 2c20 706c   to help out, pl
+00000ef0: 6561 7365 2063 6865 636b 2074 6865 205b  ease check the [
+00000f00: 434f 4e54 5249 4255 5449 4e47 5d28 6874  CONTRIBUTING](ht
+00000f10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000f20: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00000f30: 6572 2f62 6c6f 622f 6d61 696e 2f43 4f4e  er/blob/main/CON
+00000f40: 5452 4942 5554 494e 472e 6d64 2920 6669  TRIBUTING.md) fi
+00000f50: 6c65 2e0a 0a23 2320 4f70 656e 2073 6f75  le...## Open sou
+00000f60: 7263 6520 6c69 6365 6e73 696e 6720 696e  rce licensing in
+00000f70: 666f 0a31 2e20 5b4c 4943 454e 5345 5d28  fo.1. [LICENSE](
+00000f80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000f90: 6f6d 2f54 4869 7073 7465 722f 5448 6970  om/THipster/THip
+00000fa0: 7374 6572 2f62 6c6f 622f 6d61 696e 2f4c  ster/blob/main/L
+00000fb0: 4943 454e 5345 290a 322e 205b 4346 5042  ICENSE).2. [CFPB
+00000fc0: 2053 6f75 7263 6520 436f 6465 2050 6f6c   Source Code Pol
+00000fd0: 6963 795d 2868 7474 7073 3a2f 2f67 6974  icy](https://git
+00000fe0: 6875 622e 636f 6d2f 6366 7062 2f73 6f75  hub.com/cfpb/sou
+00000ff0: 7263 652d 636f 6465 2d70 6f6c 6963 792f  rce-code-policy/
+00001000: 290a 0a23 2320 4372 6564 6974 7320 616e  )..## Credits an
+00001010: 6420 7265 6665 7265 6e63 6573 0a0a 312e  d references..1.
+00001020: 2050 726f 6a65 6374 7320 7468 6174 2069   Projects that i
+00001030: 6e73 7069 7265 6420 796f 750a 2020 2020  nspired you.    
+00001040: 2d20 5b41 5753 2041 7070 6c69 6361 7469  - [AWS Applicati
+00001050: 6f6e 2043 6f6d 706f 7365 725d 2868 7474  on Composer](htt
+00001060: 7073 3a2f 2f61 7773 2e61 6d61 7a6f 6e2e  ps://aws.amazon.
+00001070: 636f 6d2f 6170 706c 6963 6174 696f 6e2d  com/application-
+00001080: 636f 6d70 6f73 6572 2f3f 6e63 313d 685f  composer/?nc1=h_
+00001090: 6c73 290a 322e 2052 656c 6174 6564 2070  ls).2. Related p
+000010a0: 726f 6a65 6374 730a 2020 2020 2d20 5b57  rojects.    - [W
+000010b0: 696e 6720 5072 6f67 7261 6d6d 696e 6720  ing Programming 
+000010c0: 4c61 6e67 7561 6765 5d28 6874 7470 733a  Language](https:
+000010d0: 2f2f 7777 772e 7769 6e67 6c61 6e67 2e69  //www.winglang.i
+000010e0: 6f2f 290a                                o/).
```

### Comparing `thipster-0.16.6/README.md` & `thipster-0.16.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,217 +1,323 @@
-00000000: 2320 5448 6970 7374 6572 0a0a 5448 6970  # THipster..THip
-00000010: 7374 6572 2069 7320 6120 746f 6f6c 2064  ster is a tool d
-00000020: 6564 6963 6174 6564 2074 6f20 7369 6d70  edicated to simp
-00000030: 6c69 6679 696e 6720 7468 6520 6469 6666  lifying the diff
-00000040: 6963 756c 7479 2061 7373 6f63 6961 7465  iculty associate
-00000050: 6420 7769 7468 2077 7269 7469 6e67 2054  d with writing T
-00000060: 6572 7261 666f 726d 2066 696c 6573 2e0a  erraform files..
-00000070: 4974 2061 6c6c 6f77 7320 7573 6572 7320  It allows users 
-00000080: 746f 2077 7269 7465 2069 6e66 7261 7374  to write infrast
-00000090: 7275 6374 7572 6520 6173 2063 6f64 6520  ructure as code 
-000000a0: 696e 2061 2073 696d 706c 6966 6965 6420  in a simplified 
-000000b0: 666f 726d 6174 2c20 7573 696e 6720 6569  format, using ei
-000000c0: 7468 6572 2059 414d 4c20 2877 6974 6820  ther YAML (with 
-000000d0: 4a49 4e4a 4129 206f 7220 7468 6520 6465  JINJA) or the de
-000000e0: 6469 6361 7465 6420 5468 6970 7374 6572  dicated Thipster
-000000f0: 2044 534c 2e0a 0a57 7269 7474 656e 2065   DSL...Written e
-00000100: 6e74 6972 656c 7920 696e 2050 7974 686f  ntirely in Pytho
-00000110: 6e2c 2069 7420 6c65 7665 7261 6765 7320  n, it leverages 
-00000120: 7468 6520 5079 7468 6f6e 2043 444b 2066  the Python CDK f
-00000130: 6f72 2054 6572 7261 666f 726d 2074 6f20  or Terraform to 
-00000140: 6372 6561 7465 2054 6572 7261 666f 726d  create Terraform
-00000150: 2066 696c 6573 2061 6e64 2061 7070 6c79   files and apply
-00000160: 2074 6865 6d20 746f 2074 6865 2063 686f   them to the cho
-00000170: 7365 6e20 7072 6f76 6964 6572 2e0a 0a23  sen provider...#
-00000180: 2320 5465 6368 6e6f 6c6f 6779 2053 7461  # Technology Sta
-00000190: 636b 0a57 7269 7474 656e 2069 6e20 5079  ck.Written in Py
-000001a0: 7468 6f6e 2033 2e31 312c 2074 6869 7073  thon 3.11, thips
-000001b0: 7465 7220 6973 2064 6573 6967 6e65 6420  ter is designed 
-000001c0: 6173 2061 2070 7974 686f 6e20 7061 636b  as a python pack
-000001d0: 6167 652c 2074 6f20 6265 2075 7365 6420  age, to be used 
-000001e0: 6569 7468 6572 2061 7320 6120 7374 616e  either as a stan
-000001f0: 6461 6c6f 6e65 2074 6f6f 6c2c 206f 7220  dalone tool, or 
-00000200: 6173 2061 206d 6f64 756c 6520 696e 7369  as a module insi
-00000210: 6465 2061 2072 756e 6e69 6e67 2070 726f  de a running pro
-00000220: 6365 7373 206c 696b 6520 6120 4349 2f43  cess like a CI/C
-00000230: 4420 7069 7065 6c69 6e65 2e0a 0a23 2320  D pipeline...## 
-00000240: 5072 6f6a 6563 7420 5374 6174 7573 0a54  Project Status.T
-00000250: 4869 7073 7465 7220 6973 2063 7572 7265  Hipster is curre
-00000260: 6e74 6c79 2069 6e20 616e 2061 6374 6976  ntly in an activ
-00000270: 6520 6465 7665 6c6f 706d 656e 7420 7374  e development st
-00000280: 6174 652e 2049 6620 796f 7520 7761 6e74  ate. If you want
-00000290: 2074 6f20 6b6e 6f77 206d 6f72 652c 2070   to know more, p
-000002a0: 6c65 6173 6520 6368 6563 6b20 7468 6520  lease check the 
-000002b0: 5b43 4841 4e47 454c 4f47 5d28 6874 7470  [CHANGELOG](http
-000002c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-000002d0: 4869 7073 7465 722f 5448 6970 7374 6572  Hipster/THipster
-000002e0: 2f62 6c6f 622f 6d61 696e 2f43 4841 4e47  /blob/main/CHANG
-000002f0: 454c 4f47 2e6d 6429 2066 6f72 206d 6f72  ELOG.md) for mor
-00000300: 6520 6465 7461 696c 732e 0a0a 2323 2044  e details...## D
-00000310: 6570 656e 6465 6e63 6965 730a 0a49 6e20  ependencies..In 
-00000320: 6f72 6465 7220 746f 2075 7365 7220 5448  order to user TH
-00000330: 6970 7374 6572 2c20 796f 7520 7769 6c6c  ipster, you will
-00000340: 206e 6565 6420 746f 2068 6176 6520 7468   need to have th
-00000350: 6520 666f 6c6c 6f77 696e 6720 696e 7374  e following inst
-00000360: 616c 6c65 643a 0a2d 205b 5079 7468 6f6e  alled:.- [Python
-00000370: 5d28 6874 7470 733a 2f2f 7777 772e 7079  ](https://www.py
-00000380: 7468 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61  thon.org/downloa
-00000390: 6473 2f29 2028 332e 3131 2b29 0a2d 205b  ds/) (3.11+).- [
-000003a0: 7069 7065 6e76 5d28 6874 7470 733a 2f2f  pipenv](https://
-000003b0: 7069 7065 6e76 2e70 7970 612e 696f 2f65  pipenv.pypa.io/e
-000003c0: 6e2f 6c61 7465 7374 2f29 2076 3230 3231  n/latest/) v2021
-000003d0: 2e35 2b0a 2d20 5b54 6572 7261 666f 726d  .5+.- [Terraform
-000003e0: 2043 4c49 5d28 6874 7470 733a 2f2f 6465   CLI](https://de
-000003f0: 7665 6c6f 7065 722e 6861 7368 6963 6f72  veloper.hashicor
-00000400: 702e 636f 6d2f 7465 7272 6166 6f72 6d2f  p.com/terraform/
-00000410: 7475 746f 7269 616c 732f 6177 732d 6765  tutorials/aws-ge
-00000420: 742d 7374 6172 7465 642f 696e 7374 616c  t-started/instal
-00000430: 6c2d 636c 6929 2028 312e 322b 290a 2d20  l-cli) (1.2+).- 
-00000440: 5b4e 6f64 652e 6a73 5d28 6874 7470 733a  [Node.js](https:
-00000450: 2f2f 6e6f 6465 6a73 2e6f 7267 2f29 2061  //nodejs.org/) a
-00000460: 6e64 206e 706d 2076 3136 2b2e 0a0a 2323  nd npm v16+...##
-00000470: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a54   Installation..T
-00000480: 6f20 7573 6520 5448 6970 7374 6572 2c20  o use THipster, 
-00000490: 796f 7520 6361 6e20 7369 6d70 6c79 2069  you can simply i
-000004a0: 6e73 7461 6c6c 2074 6865 2070 6163 6b61  nstall the packa
-000004b0: 6765 2077 6974 6820 7069 703a 0a0a 6060  ge with pip:..``
-000004c0: 6063 6f6e 736f 6c65 0a70 6970 2069 6e73  `console.pip ins
-000004d0: 7461 6c6c 2074 6869 7073 7465 720a 6060  tall thipster.``
-000004e0: 600a 0a49 6620 796f 7520 7761 6e74 2074  `..If you want t
-000004f0: 6f20 696e 7374 616c 6c20 7468 6520 676f  o install the go
-00000500: 6f67 6c65 2064 6570 656e 6465 6e63 6965  ogle dependencie
-00000510: 7320 6173 7765 6c6c 2075 7365 0a0a 6060  s aswell use..``
-00000520: 6063 6f6e 736f 6c65 0a70 6970 2069 6e73  `console.pip ins
-00000530: 7461 6c6c 2074 6869 7073 7465 725b 676f  tall thipster[go
-00000540: 6f67 6c65 5d0a 6060 600a 0a54 6865 206c  ogle].```..The l
-00000550: 6973 7420 6f66 2061 7661 696c 6162 6c65  ist of available
-00000560: 2076 6572 7369 6f6e 7320 6361 6e20 6265   versions can be
-00000570: 2066 6f75 6e64 206f 6e20 5b50 7950 495d   found on [PyPI]
-00000580: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00000590: 672f 7072 6f6a 6563 742f 7468 6970 7374  g/project/thipst
-000005a0: 6572 2f29 2e0a 0a23 2320 5573 6167 650a  er/)...## Usage.
-000005b0: 0a59 6f75 2063 616e 2075 7365 2054 4869  .You can use THi
-000005c0: 7073 7465 7220 696e 2074 776f 2077 6179  pster in two way
-000005d0: 733a 0a2d 2042 7920 6c65 7665 7261 6769  s:.- By leveragi
-000005e0: 6e67 2074 6865 205b 5448 6970 7374 6572  ng the [THipster
-000005f0: 2043 4c49 5d28 6874 7470 733a 2f2f 6769   CLI](https://gi
-00000600: 7468 7562 2e63 6f6d 2f54 4869 7073 7465  thub.com/THipste
-00000610: 722f 5448 6970 7374 6572 2d63 6c69 290a  r/THipster-cli).
-00000620: 2d20 4279 2064 6972 6563 746c 7920 7573  - By directly us
-00000630: 696e 6720 7468 6520 5b54 4869 7073 7465  ing the [THipste
-00000640: 7220 5079 7468 6f6e 2070 6163 6b61 6765  r Python package
-00000650: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-00000660: 7267 2f70 726f 6a65 6374 2f74 6869 7073  rg/project/thips
-00000670: 7465 722f 2920 696e 2079 6f75 7220 6f77  ter/) in your ow
-00000680: 6e20 636f 6465 0a0a 4d61 696e 2066 6561  n code..Main fea
-00000690: 7475 7265 3a0a 2d20 4765 6e65 7261 7465  ture:.- Generate
-000006a0: 2054 6572 7261 666f 726d 2066 696c 6573   Terraform files
-000006b0: 2066 726f 6d20 6120 5941 4d4c 2b4a 494e   from a YAML+JIN
-000006c0: 4a41 206f 7220 5448 4950 5320 6669 6c65  JA or THIPS file
-000006d0: 3a0a 6060 6070 7974 686f 6e0a 6672 6f6d  :.```python.from
-000006e0: 2074 6869 7073 7465 7220 696d 706f 7274   thipster import
-000006f0: 2045 6e67 696e 6520 6173 2054 6869 7073   Engine as Thips
-00000700: 7465 7245 6e67 696e 650a 6672 6f6d 2074  terEngine.from t
-00000710: 6869 7073 7465 722e 6175 7468 2069 6d70  hipster.auth imp
-00000720: 6f72 7420 476f 6f67 6c65 0a66 726f 6d20  ort Google.from 
-00000730: 7468 6970 7374 6572 2e70 6172 7365 7220  thipster.parser 
-00000740: 696d 706f 7274 2050 6172 7365 7246 6163  import ParserFac
-00000750: 746f 7279 0a66 726f 6d20 7468 6970 7374  tory.from thipst
-00000760: 6572 2e72 6570 6f73 6974 6f72 7920 696d  er.repository im
-00000770: 706f 7274 2047 6974 6875 6252 6570 6f0a  port GithubRepo.
-00000780: 6672 6f6d 2074 6869 7073 7465 722e 7465  from thipster.te
-00000790: 7272 6166 6f72 6d20 696d 706f 7274 2054  rraform import T
-000007a0: 6572 7261 666f 726d 0a0a 2320 6372 6561  erraform..# crea
-000007b0: 7465 206e 6577 2054 4869 7073 7465 7220  te new THipster 
-000007c0: 656e 6769 6e65 0a65 6e67 696e 6520 3d20  engine.engine = 
-000007d0: 5468 6970 7374 6572 456e 6769 6e65 2850  ThipsterEngine(P
-000007e0: 6172 7365 7246 6163 746f 7279 2829 2c20  arserFactory(), 
-000007f0: 4769 7468 7562 5265 706f 2827 5448 6970  GithubRepo('THip
-00000800: 7374 6572 2f6d 6f64 656c 7327 292c 2047  ster/models'), G
-00000810: 6f6f 676c 652c 2054 6572 7261 666f 726d  oogle, Terraform
-00000820: 2829 290a 0a23 2067 656e 6572 6174 6520  ())..# generate 
-00000830: 5465 7272 6166 6f72 6d20 6669 6c65 7320  Terraform files 
-00000840: 616e 6420 706c 616e 2066 726f 6d20 6120  and plan from a 
-00000850: 5941 4d4c 2b4a 494e 4a41 2066 696c 650a  YAML+JINJA file.
-00000860: 7465 7272 6166 6f72 6d5f 706c 616e 203d  terraform_plan =
-00000870: 2065 6e67 696e 652e 7275 6e28 2770 6174   engine.run('pat
-00000880: 682f 746f 2f66 696c 652f 6f72 2f64 6972  h/to/file/or/dir
-00000890: 6563 746f 7279 2729 0a70 7269 6e74 2874  ectory').print(t
-000008a0: 6572 7261 666f 726d 5f70 6c61 6e29 0a60  erraform_plan).`
-000008b0: 6060 0a0a 2323 2048 6f77 2074 6f20 7465  ``..## How to te
-000008c0: 7374 2074 6865 2073 6f66 7477 6172 650a  st the software.
-000008d0: 0a54 6f20 7275 6e20 7468 6520 7465 7374  .To run the test
-000008e0: 732c 2079 6f75 2063 616e 2075 7365 2074  s, you can use t
-000008f0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00000900: 6d61 6e64 3a0a 0a60 6060 636f 6e73 6f6c  mand:..```consol
-00000910: 650a 7069 7020 696e 7374 616c 6c20 2d65  e.pip install -e
-00000920: 202e 5b74 6573 745d 0a70 7974 6573 7420   .[test].pytest 
-00000930: 7465 7374 730a 6060 600a 0a23 2320 4b6e  tests.```..## Kn
-00000940: 6f77 6e20 6973 7375 6573 0a0a 416c 6c20  own issues..All 
-00000950: 6b6e 6f77 6e20 6973 7375 6573 2c20 6275  known issues, bu
-00000960: 6773 2c20 616e 6420 6665 6174 7572 6520  gs, and feature 
-00000970: 7265 7175 6573 7473 2061 7265 2074 7261  requests are tra
-00000980: 636b 6564 2069 6e20 7468 6520 5b49 7373  cked in the [Iss
-00000990: 7565 2074 7261 636b 6572 5d28 6874 7470  ue tracker](http
-000009a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-000009b0: 4869 7073 7465 722f 5448 6970 7374 6572  Hipster/THipster
-000009c0: 2f69 7373 7565 7329 2e0a 0a23 2320 4765  /issues)...## Ge
-000009d0: 7474 696e 6720 6865 6c70 0a0a 4966 2079  tting help..If y
-000009e0: 6f75 2068 6176 6520 7175 6573 7469 6f6e  ou have question
-000009f0: 732c 2063 6f6e 6365 726e 732c 2062 7567  s, concerns, bug
-00000a00: 2072 6570 6f72 7473 2c20 6574 632c 2070   reports, etc, p
-00000a10: 6c65 6173 6520 6669 6c65 2061 6e20 6973  lease file an is
-00000a20: 7375 6520 696e 2074 6869 7320 7265 706f  sue in this repo
-00000a30: 7369 746f 7279 2773 205b 4973 7375 6520  sitory's [Issue 
-00000a40: 7472 6163 6b65 725d 2868 7474 7073 3a2f  tracker](https:/
-00000a50: 2f67 6974 6875 622e 636f 6d2f 5448 6970  /github.com/THip
-00000a60: 7374 6572 2f54 4869 7073 7465 722f 6973  ster/THipster/is
-00000a70: 7375 6573 292e 0a0a 2323 2047 6574 7469  sues)...## Getti
-00000a80: 6e67 2069 6e76 6f6c 7665 640a 0a54 6f20  ng involved..To 
-00000a90: 696e 7374 616c 6c20 7468 6520 7072 6f6a  install the proj
-00000aa0: 6563 7420 666f 7220 6465 7665 6c6f 706d  ect for developm
-00000ab0: 656e 742c 2079 6f75 2063 616e 2075 7365  ent, you can use
-00000ac0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00000ad0: 6f6d 6d61 6e64 3a0a 0a60 6060 636f 6e73  ommand:..```cons
-00000ae0: 6f6c 650a 7069 7020 696e 7374 616c 6c20  ole.pip install 
-00000af0: 2d72 2072 6571 7569 7265 6d65 6e74 732e  -r requirements.
-00000b00: 7478 7420 2626 2070 6970 2069 6e73 7461  txt && pip insta
-00000b10: 6c6c 202d 6520 2e5b 6465 762c 7465 7374  ll -e .[dev,test
-00000b20: 2c64 6f63 2c67 6f6f 676c 655d 0a70 7265  ,doc,google].pre
-00000b30: 2d63 6f6d 6d69 7420 696e 7374 616c 6c20  -commit install 
-00000b40: 2626 2070 7265 2d63 6f6d 6d69 7420 7275  && pre-commit ru
-00000b50: 6e20 2d2d 616c 6c2d 6669 6c65 730a 6060  n --all-files.``
-00000b60: 600a 0a46 6f72 206d 6f72 6520 696e 666f  `..For more info
-00000b70: 726d 6174 696f 6e20 6f6e 2068 6f77 2074  rmation on how t
-00000b80: 6f20 6865 6c70 206f 7574 2c20 706c 6561  o help out, plea
-00000b90: 7365 2063 6865 636b 2074 6865 205b 434f  se check the [CO
-00000ba0: 4e54 5249 4255 5449 4e47 5d28 6874 7470  NTRIBUTING](http
-00000bb0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00000bc0: 4869 7073 7465 722f 5448 6970 7374 6572  Hipster/THipster
-00000bd0: 2f62 6c6f 622f 6d61 696e 2f43 4f4e 5452  /blob/main/CONTR
-00000be0: 4942 5554 494e 472e 6d64 2920 6669 6c65  IBUTING.md) file
-00000bf0: 2e0a 0a23 2320 4f70 656e 2073 6f75 7263  ...## Open sourc
-00000c00: 6520 6c69 6365 6e73 696e 6720 696e 666f  e licensing info
-00000c10: 0a31 2e20 5b4c 4943 454e 5345 5d28 6874  .1. [LICENSE](ht
-00000c20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000c30: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
-00000c40: 6572 2f62 6c6f 622f 6d61 696e 2f4c 4943  er/blob/main/LIC
-00000c50: 454e 5345 290a 322e 205b 4346 5042 2053  ENSE).2. [CFPB S
-00000c60: 6f75 7263 6520 436f 6465 2050 6f6c 6963  ource Code Polic
-00000c70: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00000c80: 622e 636f 6d2f 6366 7062 2f73 6f75 7263  b.com/cfpb/sourc
-00000c90: 652d 636f 6465 2d70 6f6c 6963 792f 290a  e-code-policy/).
-00000ca0: 0a23 2320 4372 6564 6974 7320 616e 6420  .## Credits and 
-00000cb0: 7265 6665 7265 6e63 6573 0a0a 312e 2050  references..1. P
-00000cc0: 726f 6a65 6374 7320 7468 6174 2069 6e73  rojects that ins
-00000cd0: 7069 7265 6420 796f 750a 2020 2020 2d20  pired you.    - 
-00000ce0: 5b41 5753 2041 7070 6c69 6361 7469 6f6e  [AWS Application
-00000cf0: 2043 6f6d 706f 7365 725d 2868 7474 7073   Composer](https
-00000d00: 3a2f 2f61 7773 2e61 6d61 7a6f 6e2e 636f  ://aws.amazon.co
-00000d10: 6d2f 6170 706c 6963 6174 696f 6e2d 636f  m/application-co
-00000d20: 6d70 6f73 6572 2f3f 6e63 313d 685f 6c73  mposer/?nc1=h_ls
-00000d30: 290a 322e 2052 656c 6174 6564 2070 726f  ).2. Related pro
-00000d40: 6a65 6374 730a 2020 2020 2d20 5b57 696e  jects.    - [Win
-00000d50: 6720 5072 6f67 7261 6d6d 696e 6720 4c61  g Programming La
-00000d60: 6e67 7561 6765 5d28 6874 7470 733a 2f2f  nguage](https://
-00000d70: 7777 772e 7769 6e67 6c61 6e67 2e69 6f2f  www.winglang.io/
-00000d80: 290a                                     ).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 6970  : 2.1.Name: thip
+00000020: 7374 6572 0a56 6572 7369 6f6e 3a20 302e  ster.Version: 0.
+00000030: 3136 2e37 0a53 756d 6d61 7279 3a20 5448  16.7.Summary: TH
+00000040: 6970 7374 6572 2069 7320 6120 746f 6f6c  ipster is a tool
+00000050: 2064 6564 6963 6174 6564 2074 6f20 7369   dedicated to si
+00000060: 6d70 6c69 6679 696e 6720 7468 6520 6469  mplifying the di
+00000070: 6666 6963 756c 7479 2061 7373 6f63 6961  fficulty associa
+00000080: 7465 6420 7769 7468 2077 7269 7469 6e67  ted with writing
+00000090: 2054 6572 7261 666f 726d 2066 696c 6573   Terraform files
+000000a0: 2e20 4974 2061 6c6c 6f77 7320 7573 6572  . It allows user
+000000b0: 7320 746f 2077 7269 7465 2069 6e66 7261  s to write infra
+000000c0: 7374 7275 6374 7572 6520 6173 2063 6f64  structure as cod
+000000d0: 6520 696e 2061 2073 696d 706c 6966 6965  e in a simplifie
+000000e0: 6420 666f 726d 6174 2c20 7573 696e 6720  d format, using 
+000000f0: 6569 7468 6572 2059 414d 4c20 2877 6974  either YAML (wit
+00000100: 6820 4a49 4e4a 4129 206f 7220 7468 6520  h JINJA) or the 
+00000110: 6465 6469 6361 7465 6420 5468 6970 7374  dedicated Thipst
+00000120: 6572 2044 534c 2e0a 486f 6d65 2d70 6167  er DSL..Home-pag
+00000130: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
+00000140: 622e 636f 6d2f 5448 6970 7374 6572 2f54  b.com/THipster/T
+00000150: 4869 7073 7465 720a 446f 776e 6c6f 6164  Hipster.Download
+00000160: 2d55 524c 3a20 6874 7470 733a 2f2f 6769  -URL: https://gi
+00000170: 7468 7562 2e63 6f6d 2f54 4869 7073 7465  thub.com/THipste
+00000180: 722f 5448 6970 7374 6572 2e67 6974 0a4b  r/THipster.git.K
+00000190: 6579 776f 7264 733a 2074 6869 7073 7465  eywords: thipste
+000001a0: 722c 7465 7272 6166 6f72 6d2c 696e 6672  r,terraform,infr
+000001b0: 6173 7472 7563 7475 7265 2c69 6e66 7261  astructure,infra
+000001c0: 7374 7275 6374 7572 652d 6173 2d63 6f64  structure-as-cod
+000001d0: 652c 6961 632c 6765 6e65 7261 746f 722c  e,iac,generator,
+000001e0: 6473 6c2c 7961 6d6c 0a43 6c61 7373 6966  dsl,yaml.Classif
+000001f0: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
+00000200: 2053 7461 7475 7320 3a3a 2031 202d 2050   Status :: 1 - P
+00000210: 6c61 6e6e 696e 670a 436c 6173 7369 6669  lanning.Classifi
+00000220: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000230: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000240: 6f6e 203a 3a20 332e 3131 0a43 6c61 7373  on :: 3.11.Class
+00000250: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000260: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000270: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
+00000280: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000290: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000002a0: 2049 6e64 6570 656e 6465 6e74 0a44 6573   Independent.Des
+000002b0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000002c0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000002d0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+000002e0: 7472 613a 2074 6573 740a 5072 6f76 6964  tra: test.Provid
+000002f0: 6573 2d45 7874 7261 3a20 6465 760a 5072  es-Extra: dev.Pr
+00000300: 6f76 6964 6573 2d45 7874 7261 3a20 646f  ovides-Extra: do
+00000310: 630a 5072 6f76 6964 6573 2d45 7874 7261  c.Provides-Extra
+00000320: 3a20 676f 6f67 6c65 0a4c 6963 656e 7365  : google.License
+00000330: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000340: 2320 5448 6970 7374 6572 0a0a 5448 6970  # THipster..THip
+00000350: 7374 6572 2069 7320 6120 746f 6f6c 2064  ster is a tool d
+00000360: 6564 6963 6174 6564 2074 6f20 7369 6d70  edicated to simp
+00000370: 6c69 6679 696e 6720 7468 6520 6469 6666  lifying the diff
+00000380: 6963 756c 7479 2061 7373 6f63 6961 7465  iculty associate
+00000390: 6420 7769 7468 2077 7269 7469 6e67 2054  d with writing T
+000003a0: 6572 7261 666f 726d 2066 696c 6573 2e0a  erraform files..
+000003b0: 4974 2061 6c6c 6f77 7320 7573 6572 7320  It allows users 
+000003c0: 746f 2077 7269 7465 2069 6e66 7261 7374  to write infrast
+000003d0: 7275 6374 7572 6520 6173 2063 6f64 6520  ructure as code 
+000003e0: 696e 2061 2073 696d 706c 6966 6965 6420  in a simplified 
+000003f0: 666f 726d 6174 2c20 7573 696e 6720 6569  format, using ei
+00000400: 7468 6572 2059 414d 4c20 2877 6974 6820  ther YAML (with 
+00000410: 4a49 4e4a 4129 206f 7220 7468 6520 6465  JINJA) or the de
+00000420: 6469 6361 7465 6420 5468 6970 7374 6572  dicated Thipster
+00000430: 2044 534c 2e0a 0a57 7269 7474 656e 2065   DSL...Written e
+00000440: 6e74 6972 656c 7920 696e 2050 7974 686f  ntirely in Pytho
+00000450: 6e2c 2069 7420 6c65 7665 7261 6765 7320  n, it leverages 
+00000460: 7468 6520 5079 7468 6f6e 2043 444b 2066  the Python CDK f
+00000470: 6f72 2054 6572 7261 666f 726d 2074 6f20  or Terraform to 
+00000480: 6372 6561 7465 2054 6572 7261 666f 726d  create Terraform
+00000490: 2066 696c 6573 2061 6e64 2061 7070 6c79   files and apply
+000004a0: 2074 6865 6d20 746f 2074 6865 2063 686f   them to the cho
+000004b0: 7365 6e20 7072 6f76 6964 6572 2e0a 0a3c  sen provider...<
+000004c0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000004d0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+000004e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000004f0: 5448 6970 7374 6572 2f54 4869 7073 7465  THipster/THipste
+00000500: 722f 626c 6f62 2f6d 6169 6e2f 4c49 4345  r/blob/main/LICE
+00000510: 4e53 4522 2074 6172 6765 743d 225f 626c  NSE" target="_bl
+00000520: 616e 6b22 2061 6c74 3d22 4c69 6365 6e73  ank" alt="Licens
+00000530: 6522 3e0a 2020 2020 3c69 6d67 2073 7263  e">.    <img src
+00000540: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000550: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000560: 6c69 6365 6e73 652f 5448 6970 7374 6572  license/THipster
+00000570: 2f54 4869 7073 7465 7222 2061 6c74 3d22  /THipster" alt="
+00000580: 4c69 6365 6e73 6522 3e0a 2020 3c2f 613e  License">.  </a>
+00000590: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+000005a0: 733a 2f2f 7468 6970 7374 6572 2e72 6561  s://thipster.rea
+000005b0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000005c0: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
+000005d0: 6573 7422 2074 6172 6765 743d 225f 626c  est" target="_bl
+000005e0: 616e 6b22 2061 6c74 3d22 5265 6164 2074  ank" alt="Read t
+000005f0: 6865 2064 6f63 7320 646f 6375 6d65 6e74  he docs document
+00000600: 6174 696f 6e22 3e0a 2020 2020 3c69 6d67  ation">.    <img
+00000610: 2073 7263 3d22 6874 7470 733a 2f2f 7265   src="https://re
+00000620: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00000630: 6f6a 6563 7473 2f74 6869 7073 7465 722f  ojects/thipster/
+00000640: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000650: 6174 6573 7422 2061 6c74 3d22 5265 6164  atest" alt="Read
+00000660: 2074 6865 2064 6f63 7320 646f 6375 6d65   the docs docume
+00000670: 6e74 6174 696f 6e22 3e0a 2020 3c2f 613e  ntation">.  </a>
+00000680: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000690: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000006a0: 6a65 6374 2f74 6869 7073 7465 722f 2220  ject/thipster/" 
+000006b0: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
+000006c0: 616c 743d 2250 7950 6920 7061 636b 6167  alt="PyPi packag
+000006d0: 6522 3e0a 2020 2020 3c69 6d67 2073 7263  e">.    <img src
+000006e0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000006f0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000700: 7468 6970 7374 6572 3f63 6f6c 6f72 3d62  thipster?color=b
+00000710: 7269 6768 7467 7265 656e 266c 6162 656c  rightgreen&label
+00000720: 3d70 7970 6925 3230 7061 636b 6167 6522  =pypi%20package"
+00000730: 2061 6c74 3d22 5061 636b 6167 6520 7665   alt="Package ve
+00000740: 7273 696f 6e22 3e0a 2020 3c2f 613e 0a20  rsion">.  </a>. 
+00000750: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000760: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000770: 6374 2f74 6869 7073 7465 722f 2220 7461  ct/thipster/" ta
+00000780: 7267 6574 3d22 5f62 6c61 6e6b 2220 616c  rget="_blank" al
+00000790: 743d 2250 7950 6920 7061 636b 6167 6522  t="PyPi package"
+000007a0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+000007b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000007c0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+000007d0: 7273 696f 6e73 2f74 6869 7073 7465 723f  rsions/thipster?
+000007e0: 636f 6c6f 723d 6272 6967 6874 6772 6565  color=brightgree
+000007f0: 6e22 2061 6c74 3d22 5375 7070 6f72 7465  n" alt="Supporte
+00000800: 6420 5079 7468 6f6e 2076 6572 7369 6f6e  d Python version
+00000810: 7322 3e0a 2020 3c2f 613e 0a3c 2f70 3e0a  s">.  </a>.</p>.
+00000820: 0a23 2320 5465 6368 6e6f 6c6f 6779 2053  .## Technology S
+00000830: 7461 636b 0a57 7269 7474 656e 2069 6e20  tack.Written in 
+00000840: 5079 7468 6f6e 2033 2e31 312c 2074 6869  Python 3.11, thi
+00000850: 7073 7465 7220 6973 2064 6573 6967 6e65  pster is designe
+00000860: 6420 6173 2061 2070 7974 686f 6e20 7061  d as a python pa
+00000870: 636b 6167 652c 2074 6f20 6265 2075 7365  ckage, to be use
+00000880: 6420 6569 7468 6572 2061 7320 6120 7374  d either as a st
+00000890: 616e 6461 6c6f 6e65 2074 6f6f 6c2c 206f  andalone tool, o
+000008a0: 7220 6173 2061 206d 6f64 756c 6520 696e  r as a module in
+000008b0: 7369 6465 2061 2072 756e 6e69 6e67 2070  side a running p
+000008c0: 726f 6365 7373 206c 696b 6520 6120 4349  rocess like a CI
+000008d0: 2f43 4420 7069 7065 6c69 6e65 2e0a 0a23  /CD pipeline...#
+000008e0: 2320 5072 6f6a 6563 7420 5374 6174 7573  # Project Status
+000008f0: 0a54 4869 7073 7465 7220 6973 2063 7572  .THipster is cur
+00000900: 7265 6e74 6c79 2069 6e20 616e 2061 6374  rently in an act
+00000910: 6976 6520 6465 7665 6c6f 706d 656e 7420  ive development 
+00000920: 7374 6174 652e 2049 6620 796f 7520 7761  state. If you wa
+00000930: 6e74 2074 6f20 6b6e 6f77 206d 6f72 652c  nt to know more,
+00000940: 2070 6c65 6173 6520 6368 6563 6b20 7468   please check th
+00000950: 6520 5b43 4841 4e47 454c 4f47 5d28 6874  e [CHANGELOG](ht
+00000960: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000970: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00000980: 6572 2f62 6c6f 622f 6d61 696e 2f43 4841  er/blob/main/CHA
+00000990: 4e47 454c 4f47 2e6d 6429 2066 6f72 206d  NGELOG.md) for m
+000009a0: 6f72 6520 6465 7461 696c 732e 0a0a 2323  ore details...##
+000009b0: 2044 6570 656e 6465 6e63 6965 730a 0a49   Dependencies..I
+000009c0: 6e20 6f72 6465 7220 746f 2075 7365 7220  n order to user 
+000009d0: 5448 6970 7374 6572 2c20 796f 7520 7769  THipster, you wi
+000009e0: 6c6c 206e 6565 6420 746f 2068 6176 6520  ll need to have 
+000009f0: 7468 6520 666f 6c6c 6f77 696e 6720 696e  the following in
+00000a00: 7374 616c 6c65 643a 0a2d 205b 5079 7468  stalled:.- [Pyth
+00000a10: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
+00000a20: 7079 7468 6f6e 2e6f 7267 2f64 6f77 6e6c  python.org/downl
+00000a30: 6f61 6473 2f29 2028 332e 3131 2b29 0a2d  oads/) (3.11+).-
+00000a40: 205b 7069 7065 6e76 5d28 6874 7470 733a   [pipenv](https:
+00000a50: 2f2f 7069 7065 6e76 2e70 7970 612e 696f  //pipenv.pypa.io
+00000a60: 2f65 6e2f 6c61 7465 7374 2f29 2076 3230  /en/latest/) v20
+00000a70: 3231 2e35 2b0a 2d20 5b54 6572 7261 666f  21.5+.- [Terrafo
+00000a80: 726d 2043 4c49 5d28 6874 7470 733a 2f2f  rm CLI](https://
+00000a90: 6465 7665 6c6f 7065 722e 6861 7368 6963  developer.hashic
+00000aa0: 6f72 702e 636f 6d2f 7465 7272 6166 6f72  orp.com/terrafor
+00000ab0: 6d2f 7475 746f 7269 616c 732f 6177 732d  m/tutorials/aws-
+00000ac0: 6765 742d 7374 6172 7465 642f 696e 7374  get-started/inst
+00000ad0: 616c 6c2d 636c 6929 2028 312e 322b 290a  all-cli) (1.2+).
+00000ae0: 2d20 5b4e 6f64 652e 6a73 5d28 6874 7470  - [Node.js](http
+00000af0: 733a 2f2f 6e6f 6465 6a73 2e6f 7267 2f29  s://nodejs.org/)
+00000b00: 2061 6e64 206e 706d 2076 3136 2b2e 0a0a   and npm v16+...
+00000b10: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
+00000b20: 0a54 6f20 7573 6520 5448 6970 7374 6572  .To use THipster
+00000b30: 2c20 796f 7520 6361 6e20 7369 6d70 6c79  , you can simply
+00000b40: 2069 6e73 7461 6c6c 2074 6865 2070 6163   install the pac
+00000b50: 6b61 6765 2077 6974 6820 7069 703a 0a0a  kage with pip:..
+00000b60: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
+00000b70: 6e73 7461 6c6c 2074 6869 7073 7465 720a  nstall thipster.
+00000b80: 6060 600a 0a49 6620 796f 7520 7761 6e74  ```..If you want
+00000b90: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+00000ba0: 676f 6f67 6c65 2064 6570 656e 6465 6e63  google dependenc
+00000bb0: 6965 7320 6173 7765 6c6c 2075 7365 0a0a  ies aswell use..
+00000bc0: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
+00000bd0: 6e73 7461 6c6c 2074 6869 7073 7465 725b  nstall thipster[
+00000be0: 676f 6f67 6c65 5d0a 6060 600a 0a54 6865  google].```..The
+00000bf0: 206c 6973 7420 6f66 2061 7661 696c 6162   list of availab
+00000c00: 6c65 2076 6572 7369 6f6e 7320 6361 6e20  le versions can 
+00000c10: 6265 2066 6f75 6e64 206f 6e20 5b50 7950  be found on [PyP
+00000c20: 495d 2868 7474 7073 3a2f 2f70 7970 692e  I](https://pypi.
+00000c30: 6f72 672f 7072 6f6a 6563 742f 7468 6970  org/project/thip
+00000c40: 7374 6572 2f29 2e0a 0a23 2320 5573 6167  ster/)...## Usag
+00000c50: 650a 0a59 6f75 2063 616e 2075 7365 2054  e..You can use T
+00000c60: 4869 7073 7465 7220 696e 2074 776f 2077  Hipster in two w
+00000c70: 6179 733a 0a2d 2042 7920 6c65 7665 7261  ays:.- By levera
+00000c80: 6769 6e67 2074 6865 205b 5448 6970 7374  ging the [THipst
+00000c90: 6572 2043 4c49 5d28 6874 7470 733a 2f2f  er CLI](https://
+00000ca0: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
+00000cb0: 7465 722f 5448 6970 7374 6572 2d63 6c69  ter/THipster-cli
+00000cc0: 290a 2d20 4279 2064 6972 6563 746c 7920  ).- By directly 
+00000cd0: 7573 696e 6720 7468 6520 5b54 4869 7073  using the [THips
+00000ce0: 7465 7220 5079 7468 6f6e 2070 6163 6b61  ter Python packa
+00000cf0: 6765 5d28 6874 7470 733a 2f2f 7079 7069  ge](https://pypi
+00000d00: 2e6f 7267 2f70 726f 6a65 6374 2f74 6869  .org/project/thi
+00000d10: 7073 7465 722f 2920 696e 2079 6f75 7220  pster/) in your 
+00000d20: 6f77 6e20 636f 6465 0a0a 4d61 696e 2066  own code..Main f
+00000d30: 6561 7475 7265 3a0a 2d20 4765 6e65 7261  eature:.- Genera
+00000d40: 7465 2054 6572 7261 666f 726d 2066 696c  te Terraform fil
+00000d50: 6573 2066 726f 6d20 6120 5941 4d4c 2b4a  es from a YAML+J
+00000d60: 494e 4a41 206f 7220 5448 4950 5320 6669  INJA or THIPS fi
+00000d70: 6c65 3a0a 6060 6070 7974 686f 6e0a 6672  le:.```python.fr
+00000d80: 6f6d 2074 6869 7073 7465 7220 696d 706f  om thipster impo
+00000d90: 7274 2045 6e67 696e 6520 6173 2054 6869  rt Engine as Thi
+00000da0: 7073 7465 7245 6e67 696e 650a 6672 6f6d  psterEngine.from
+00000db0: 2074 6869 7073 7465 722e 6175 7468 2069   thipster.auth i
+00000dc0: 6d70 6f72 7420 476f 6f67 6c65 0a66 726f  mport Google.fro
+00000dd0: 6d20 7468 6970 7374 6572 2e70 6172 7365  m thipster.parse
+00000de0: 7220 696d 706f 7274 2050 6172 7365 7246  r import ParserF
+00000df0: 6163 746f 7279 0a66 726f 6d20 7468 6970  actory.from thip
+00000e00: 7374 6572 2e72 6570 6f73 6974 6f72 7920  ster.repository 
+00000e10: 696d 706f 7274 2047 6974 6875 6252 6570  import GithubRep
+00000e20: 6f0a 6672 6f6d 2074 6869 7073 7465 722e  o.from thipster.
+00000e30: 7465 7272 6166 6f72 6d20 696d 706f 7274  terraform import
+00000e40: 2054 6572 7261 666f 726d 0a0a 2320 6372   Terraform..# cr
+00000e50: 6561 7465 206e 6577 2054 4869 7073 7465  eate new THipste
+00000e60: 7220 656e 6769 6e65 0a65 6e67 696e 6520  r engine.engine 
+00000e70: 3d20 5468 6970 7374 6572 456e 6769 6e65  = ThipsterEngine
+00000e80: 2850 6172 7365 7246 6163 746f 7279 2829  (ParserFactory()
+00000e90: 2c20 4769 7468 7562 5265 706f 2827 5448  , GithubRepo('TH
+00000ea0: 6970 7374 6572 2f6d 6f64 656c 7327 292c  ipster/models'),
+00000eb0: 2047 6f6f 676c 652c 2054 6572 7261 666f   Google, Terrafo
+00000ec0: 726d 2829 290a 0a23 2067 656e 6572 6174  rm())..# generat
+00000ed0: 6520 5465 7272 6166 6f72 6d20 6669 6c65  e Terraform file
+00000ee0: 7320 616e 6420 706c 616e 2066 726f 6d20  s and plan from 
+00000ef0: 6120 5941 4d4c 2b4a 494e 4a41 2066 696c  a YAML+JINJA fil
+00000f00: 650a 7465 7272 6166 6f72 6d5f 706c 616e  e.terraform_plan
+00000f10: 203d 2065 6e67 696e 652e 7275 6e28 2770   = engine.run('p
+00000f20: 6174 682f 746f 2f66 696c 652f 6f72 2f64  ath/to/file/or/d
+00000f30: 6972 6563 746f 7279 2729 0a70 7269 6e74  irectory').print
+00000f40: 2874 6572 7261 666f 726d 5f70 6c61 6e29  (terraform_plan)
+00000f50: 0a60 6060 0a0a 2323 2048 6f77 2074 6f20  .```..## How to 
+00000f60: 7465 7374 2074 6865 2073 6f66 7477 6172  test the softwar
+00000f70: 650a 0a54 6f20 7275 6e20 7468 6520 7465  e..To run the te
+00000f80: 7374 732c 2079 6f75 2063 616e 2075 7365  sts, you can use
+00000f90: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00000fa0: 6f6d 6d61 6e64 3a0a 0a60 6060 636f 6e73  ommand:..```cons
+00000fb0: 6f6c 650a 7069 7020 696e 7374 616c 6c20  ole.pip install 
+00000fc0: 2d65 202e 5b74 6573 745d 0a70 7974 6573  -e .[test].pytes
+00000fd0: 7420 7465 7374 730a 6060 600a 0a23 2320  t tests.```..## 
+00000fe0: 4b6e 6f77 6e20 6973 7375 6573 0a0a 416c  Known issues..Al
+00000ff0: 6c20 6b6e 6f77 6e20 6973 7375 6573 2c20  l known issues, 
+00001000: 6275 6773 2c20 616e 6420 6665 6174 7572  bugs, and featur
+00001010: 6520 7265 7175 6573 7473 2061 7265 2074  e requests are t
+00001020: 7261 636b 6564 2069 6e20 7468 6520 5b49  racked in the [I
+00001030: 7373 7565 2074 7261 636b 6572 5d28 6874  ssue tracker](ht
+00001040: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001050: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00001060: 6572 2f69 7373 7565 7329 2e0a 0a23 2320  er/issues)...## 
+00001070: 4765 7474 696e 6720 6865 6c70 0a0a 4966  Getting help..If
+00001080: 2079 6f75 2068 6176 6520 7175 6573 7469   you have questi
+00001090: 6f6e 732c 2063 6f6e 6365 726e 732c 2062  ons, concerns, b
+000010a0: 7567 2072 6570 6f72 7473 2c20 6574 632c  ug reports, etc,
+000010b0: 2070 6c65 6173 6520 6669 6c65 2061 6e20   please file an 
+000010c0: 6973 7375 6520 696e 2074 6869 7320 7265  issue in this re
+000010d0: 706f 7369 746f 7279 2773 205b 4973 7375  pository's [Issu
+000010e0: 6520 7472 6163 6b65 725d 2868 7474 7073  e tracker](https
+000010f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5448  ://github.com/TH
+00001100: 6970 7374 6572 2f54 4869 7073 7465 722f  ipster/THipster/
+00001110: 6973 7375 6573 292e 0a0a 2323 2047 6574  issues)...## Get
+00001120: 7469 6e67 2069 6e76 6f6c 7665 640a 0a54  ting involved..T
+00001130: 6f20 696e 7374 616c 6c20 7468 6520 7072  o install the pr
+00001140: 6f6a 6563 7420 666f 7220 6465 7665 6c6f  oject for develo
+00001150: 706d 656e 742c 2079 6f75 2063 616e 2075  pment, you can u
+00001160: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00001170: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 636f   command:..```co
+00001180: 6e73 6f6c 650a 7069 7020 696e 7374 616c  nsole.pip instal
+00001190: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
+000011a0: 732e 7478 7420 2626 2070 6970 2069 6e73  s.txt && pip ins
+000011b0: 7461 6c6c 202d 6520 2e5b 6465 762c 7465  tall -e .[dev,te
+000011c0: 7374 2c64 6f63 2c67 6f6f 676c 655d 0a70  st,doc,google].p
+000011d0: 7265 2d63 6f6d 6d69 7420 696e 7374 616c  re-commit instal
+000011e0: 6c20 2626 2070 7265 2d63 6f6d 6d69 7420  l && pre-commit 
+000011f0: 7275 6e20 2d2d 616c 6c2d 6669 6c65 730a  run --all-files.
+00001200: 6060 600a 0a46 6f72 206d 6f72 6520 696e  ```..For more in
+00001210: 666f 726d 6174 696f 6e20 6f6e 2068 6f77  formation on how
+00001220: 2074 6f20 6865 6c70 206f 7574 2c20 706c   to help out, pl
+00001230: 6561 7365 2063 6865 636b 2074 6865 205b  ease check the [
+00001240: 434f 4e54 5249 4255 5449 4e47 5d28 6874  CONTRIBUTING](ht
+00001250: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001260: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00001270: 6572 2f62 6c6f 622f 6d61 696e 2f43 4f4e  er/blob/main/CON
+00001280: 5452 4942 5554 494e 472e 6d64 2920 6669  TRIBUTING.md) fi
+00001290: 6c65 2e0a 0a23 2320 4f70 656e 2073 6f75  le...## Open sou
+000012a0: 7263 6520 6c69 6365 6e73 696e 6720 696e  rce licensing in
+000012b0: 666f 0a31 2e20 5b4c 4943 454e 5345 5d28  fo.1. [LICENSE](
+000012c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000012d0: 6f6d 2f54 4869 7073 7465 722f 5448 6970  om/THipster/THip
+000012e0: 7374 6572 2f62 6c6f 622f 6d61 696e 2f4c  ster/blob/main/L
+000012f0: 4943 454e 5345 290a 322e 205b 4346 5042  ICENSE).2. [CFPB
+00001300: 2053 6f75 7263 6520 436f 6465 2050 6f6c   Source Code Pol
+00001310: 6963 795d 2868 7474 7073 3a2f 2f67 6974  icy](https://git
+00001320: 6875 622e 636f 6d2f 6366 7062 2f73 6f75  hub.com/cfpb/sou
+00001330: 7263 652d 636f 6465 2d70 6f6c 6963 792f  rce-code-policy/
+00001340: 290a 0a23 2320 4372 6564 6974 7320 616e  )..## Credits an
+00001350: 6420 7265 6665 7265 6e63 6573 0a0a 312e  d references..1.
+00001360: 2050 726f 6a65 6374 7320 7468 6174 2069   Projects that i
+00001370: 6e73 7069 7265 6420 796f 750a 2020 2020  nspired you.    
+00001380: 2d20 5b41 5753 2041 7070 6c69 6361 7469  - [AWS Applicati
+00001390: 6f6e 2043 6f6d 706f 7365 725d 2868 7474  on Composer](htt
+000013a0: 7073 3a2f 2f61 7773 2e61 6d61 7a6f 6e2e  ps://aws.amazon.
+000013b0: 636f 6d2f 6170 706c 6963 6174 696f 6e2d  com/application-
+000013c0: 636f 6d70 6f73 6572 2f3f 6e63 313d 685f  composer/?nc1=h_
+000013d0: 6c73 290a 322e 2052 656c 6174 6564 2070  ls).2. Related p
+000013e0: 726f 6a65 6374 730a 2020 2020 2d20 5b57  rojects.    - [W
+000013f0: 696e 6720 5072 6f67 7261 6d6d 696e 6720  ing Programming 
+00001400: 4c61 6e67 7561 6765 5d28 6874 7470 733a  Language](https:
+00001410: 2f2f 7777 772e 7769 6e67 6c61 6e67 2e69  //www.winglang.i
+00001420: 6f2f 290a                                o/).
```

### Comparing `thipster-0.16.6/pyproject.toml` & `thipster-0.16.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -26,7 +26,15 @@
 major_on_zero = false
 
 [pytest]
 mock_use_standalone_module = true
 
 [tool.ruff]
 exclude = ["__init__.py"]
+select = [
+    "F",
+    "E",
+    "W",
+    "I",
+    "UP",
+    "C90",
+]
```

### Comparing `thipster-0.16.6/setup.py` & `thipster-0.16.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-__version__ = '0.16.6'
+__version__ = '0.16.7'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
 
@@ -15,17 +15,29 @@
         {'name': 'gsuquet', 'email': 'gsuquet@ippon.fr'},
     ],
     description='THipster is a tool dedicated to simplifying the difficulty associated \
 with writing Terraform files. It allows users to write infrastructure as code in a \
 simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.',
     long_description=readme,
     long_description_content_type='text/markdown',
+    keywords=[
+        'thipster',
+        'terraform',
+        'infrastructure',
+        'infrastructure-as-code',
+        'iac',
+        'generator',
+        'dsl',
+        'yaml',
+    ],
     classifiers=[
         'Development Status :: 1 - Planning',
-        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.11',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
     ],
 
     download_url='https://github.com/THipster/THipster.git',
     url='https://github.com/THipster/THipster',
 
     version=__version__,
     install_requires=required,
```

### Comparing `thipster-0.16.6/tests/engine/test_engine.py` & `thipster-0.16.7/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/engine/test_generation.py` & `thipster-0.16.7/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.16.7/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 
 import pytest
 
 import thipster.engine.parsed_file as pf
 from thipster.parser import DSLParser
-from thipster.parser.dsl_parser.exceptions import DSLParserPathNotFound
-from thipster.parser.dsl_parser.token import TOKENTYPES as TT
 from thipster.parser.dsl_parser.exceptions import (
+    DSLArithmeticException,
     DSLConditionException,
+    DSLParserPathNotFound,
     DSLSyntaxException,
     DSLUnexpectedEOF,
-    DSLArithmeticException,
 )
+from thipster.parser.dsl_parser.token import TOKENTYPES as TT
 
 from ...test_tools import create_dir
 
 
 def test_get_files():
     path_input = 'test'
     _destroy_dir = create_dir(
```

### Comparing `thipster-0.16.6/tests/parser/dsl_parser/test_ast.py` & `thipster-0.16.7/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.16.7/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/parser/dsl_parser/test_token.py` & `thipster-0.16.7/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.16.7/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/parser/test_ParserFactory.py` & `thipster-0.16.7/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/parser/test_YAMLParser.py` & `thipster-0.16.7/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/parser/test_parsedfile.py` & `thipster-0.16.7/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/test_e2e.py` & `thipster-0.16.7/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/tests/test_tools.py` & `thipster-0.16.7/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/auth/google.py` & `thipster-0.16.7/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/engine/engine.py` & `thipster-0.16.7/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/engine/i_parser.py` & `thipster-0.16.7/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/engine/i_repository.py` & `thipster-0.16.7/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/engine/i_terraform.py` & `thipster-0.16.7/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/engine/parsed_file.py` & `thipster-0.16.7/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/engine/resource_model.py` & `thipster-0.16.7/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/helpers.py` & `thipster-0.16.7/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/ast.py` & `thipster-0.16.7/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.16.7/thipster/parser/dsl_parser/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from thipster.engine import THipsterException
 from thipster.engine.parsed_file import Position
+
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
 class DSLParserBaseException(THipsterException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
```

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.16.7/thipster/parser/dsl_parser/interpreter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import thipster.engine.parsed_file as pf
 import thipster.parser.dsl_parser.ast as ast
 
 from .exceptions import (
+    DSLArithmeticException,
     DSLParserVariableAlreadyUsed,
     DSLParserVariableNotDeclared,
-    DSLArithmeticException,
 )
 from .token import TOKENTYPES as TT
 
 
 class Interpreter():
     """Interpreter class for the DSL Parser
```

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/lexer.py` & `thipster-0.16.7/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.16.7/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/parser.py` & `thipster-0.16.7/thipster/parser/dsl_parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         files = {}
 
         if os.path.isdir(path):
             for content in os.listdir(path):
                 files.update(DSLParser.__getfiles(f'{path}/{content}'))
 
         if os.path.isfile(path):
-            with open(path, 'r') as f:
+            with open(path) as f:
                 files.update({path: f.read()})
 
                 f.close()
 
         return files
 
     @classmethod
```

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/token.py` & `thipster-0.16.7/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.16.7/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/parser/parser_factory.py` & `thipster-0.16.7/thipster/parser/parser_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
-from thipster.engine import I_Parser
-from thipster.engine import THipsterException
+from thipster.engine import I_Parser, THipsterException
 from thipster.engine.parsed_file import ParsedFile
+
 from .dsl_parser import DSLParser
 from .yaml_parser import YAMLParser
 
 
 def _noParser(pathExtension):
     class noParser():
         def run(path):
```

### Comparing `thipster-0.16.6/thipster/parser/yaml_parser.py` & `thipster-0.16.7/thipster/parser/yaml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 
 import yaml
 from jinja2 import Environment, FileSystemLoader
-from thipster.engine import THipsterException
 
 import thipster.engine.parsed_file as pf
-from thipster.engine import I_Parser
+from thipster.engine import I_Parser, THipsterException
 
 
 class YAMLParserBaseException(THipsterException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
```

### Comparing `thipster-0.16.6/thipster/repository/github.py` & `thipster-0.16.7/thipster/repository/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """GithubRepo.py module
 """
 
 import requests
 
 from .exceptions import ModelNotFoundError
-
 from .json import JSONRepo
 
 
 class GithubRepo(JSONRepo):
     """Class representing a GitHub resources Repository
 
     JSON Models of resources and services offered by supported cloud providers are
```

### Comparing `thipster-0.16.6/thipster/repository/json.py` & `thipster-0.16.7/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/terraform/cdk.py` & `thipster-0.16.7/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster/terraform/exceptions.py` & `thipster-0.16.7/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.6/thipster.egg-info/PKG-INFO` & `thipster-0.16.7/thipster.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 6970  : 2.1.Name: thip
 00000020: 7374 6572 0a56 6572 7369 6f6e 3a20 302e  ster.Version: 0.
-00000030: 3136 2e36 0a53 756d 6d61 7279 3a20 5448  16.6.Summary: TH
+00000030: 3136 2e37 0a53 756d 6d61 7279 3a20 5448  16.7.Summary: TH
 00000040: 6970 7374 6572 2069 7320 6120 746f 6f6c  ipster is a tool
 00000050: 2064 6564 6963 6174 6564 2074 6f20 7369   dedicated to si
 00000060: 6d70 6c69 6679 696e 6720 7468 6520 6469  mplifying the di
 00000070: 6666 6963 756c 7479 2061 7373 6f63 6961  fficulty associa
 00000080: 7465 6420 7769 7468 2077 7269 7469 6e67  ted with writing
 00000090: 2054 6572 7261 666f 726d 2066 696c 6573   Terraform files
 000000a0: 2e20 4974 2061 6c6c 6f77 7320 7573 6572  . It allows user
@@ -18,239 +18,306 @@
 00000110: 6465 6469 6361 7465 6420 5468 6970 7374  dedicated Thipst
 00000120: 6572 2044 534c 2e0a 486f 6d65 2d70 6167  er DSL..Home-pag
 00000130: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000140: 622e 636f 6d2f 5448 6970 7374 6572 2f54  b.com/THipster/T
 00000150: 4869 7073 7465 720a 446f 776e 6c6f 6164  Hipster.Download
 00000160: 2d55 524c 3a20 6874 7470 733a 2f2f 6769  -URL: https://gi
 00000170: 7468 7562 2e63 6f6d 2f54 4869 7073 7465  thub.com/THipste
-00000180: 722f 5448 6970 7374 6572 2e67 6974 0a43  r/THipster.git.C
-00000190: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-000001a0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-000001b0: 2031 202d 2050 6c61 6e6e 696e 670a 436c   1 - Planning.Cl
-000001c0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000001d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001e0: 3a20 5079 7468 6f6e 0a44 6573 6372 6970  : Python.Descrip
-000001f0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00000200: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00000210: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000220: 2074 6573 740a 5072 6f76 6964 6573 2d45   test.Provides-E
-00000230: 7874 7261 3a20 6465 760a 5072 6f76 6964  xtra: dev.Provid
-00000240: 6573 2d45 7874 7261 3a20 646f 630a 5072  es-Extra: doc.Pr
-00000250: 6f76 6964 6573 2d45 7874 7261 3a20 676f  ovides-Extra: go
-00000260: 6f67 6c65 0a4c 6963 656e 7365 2d46 696c  ogle.License-Fil
-00000270: 653a 204c 4943 454e 5345 0a0a 2320 5448  e: LICENSE..# TH
-00000280: 6970 7374 6572 0a0a 5448 6970 7374 6572  ipster..THipster
-00000290: 2069 7320 6120 746f 6f6c 2064 6564 6963   is a tool dedic
-000002a0: 6174 6564 2074 6f20 7369 6d70 6c69 6679  ated to simplify
-000002b0: 696e 6720 7468 6520 6469 6666 6963 756c  ing the difficul
-000002c0: 7479 2061 7373 6f63 6961 7465 6420 7769  ty associated wi
-000002d0: 7468 2077 7269 7469 6e67 2054 6572 7261  th writing Terra
-000002e0: 666f 726d 2066 696c 6573 2e0a 4974 2061  form files..It a
-000002f0: 6c6c 6f77 7320 7573 6572 7320 746f 2077  llows users to w
-00000300: 7269 7465 2069 6e66 7261 7374 7275 6374  rite infrastruct
-00000310: 7572 6520 6173 2063 6f64 6520 696e 2061  ure as code in a
-00000320: 2073 696d 706c 6966 6965 6420 666f 726d   simplified form
-00000330: 6174 2c20 7573 696e 6720 6569 7468 6572  at, using either
-00000340: 2059 414d 4c20 2877 6974 6820 4a49 4e4a   YAML (with JINJ
-00000350: 4129 206f 7220 7468 6520 6465 6469 6361  A) or the dedica
-00000360: 7465 6420 5468 6970 7374 6572 2044 534c  ted Thipster DSL
-00000370: 2e0a 0a57 7269 7474 656e 2065 6e74 6972  ...Written entir
-00000380: 656c 7920 696e 2050 7974 686f 6e2c 2069  ely in Python, i
-00000390: 7420 6c65 7665 7261 6765 7320 7468 6520  t leverages the 
-000003a0: 5079 7468 6f6e 2043 444b 2066 6f72 2054  Python CDK for T
-000003b0: 6572 7261 666f 726d 2074 6f20 6372 6561  erraform to crea
-000003c0: 7465 2054 6572 7261 666f 726d 2066 696c  te Terraform fil
-000003d0: 6573 2061 6e64 2061 7070 6c79 2074 6865  es and apply the
-000003e0: 6d20 746f 2074 6865 2063 686f 7365 6e20  m to the chosen 
-000003f0: 7072 6f76 6964 6572 2e0a 0a23 2320 5465  provider...## Te
-00000400: 6368 6e6f 6c6f 6779 2053 7461 636b 0a57  chnology Stack.W
-00000410: 7269 7474 656e 2069 6e20 5079 7468 6f6e  ritten in Python
-00000420: 2033 2e31 312c 2074 6869 7073 7465 7220   3.11, thipster 
-00000430: 6973 2064 6573 6967 6e65 6420 6173 2061  is designed as a
-00000440: 2070 7974 686f 6e20 7061 636b 6167 652c   python package,
-00000450: 2074 6f20 6265 2075 7365 6420 6569 7468   to be used eith
-00000460: 6572 2061 7320 6120 7374 616e 6461 6c6f  er as a standalo
-00000470: 6e65 2074 6f6f 6c2c 206f 7220 6173 2061  ne tool, or as a
-00000480: 206d 6f64 756c 6520 696e 7369 6465 2061   module inside a
-00000490: 2072 756e 6e69 6e67 2070 726f 6365 7373   running process
-000004a0: 206c 696b 6520 6120 4349 2f43 4420 7069   like a CI/CD pi
-000004b0: 7065 6c69 6e65 2e0a 0a23 2320 5072 6f6a  peline...## Proj
-000004c0: 6563 7420 5374 6174 7573 0a54 4869 7073  ect Status.THips
-000004d0: 7465 7220 6973 2063 7572 7265 6e74 6c79  ter is currently
-000004e0: 2069 6e20 616e 2061 6374 6976 6520 6465   in an active de
-000004f0: 7665 6c6f 706d 656e 7420 7374 6174 652e  velopment state.
-00000500: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
-00000510: 6b6e 6f77 206d 6f72 652c 2070 6c65 6173  know more, pleas
-00000520: 6520 6368 6563 6b20 7468 6520 5b43 4841  e check the [CHA
-00000530: 4e47 454c 4f47 5d28 6874 7470 733a 2f2f  NGELOG](https://
-00000540: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
-00000550: 7465 722f 5448 6970 7374 6572 2f62 6c6f  ter/THipster/blo
-00000560: 622f 6d61 696e 2f43 4841 4e47 454c 4f47  b/main/CHANGELOG
-00000570: 2e6d 6429 2066 6f72 206d 6f72 6520 6465  .md) for more de
-00000580: 7461 696c 732e 0a0a 2323 2044 6570 656e  tails...## Depen
-00000590: 6465 6e63 6965 730a 0a49 6e20 6f72 6465  dencies..In orde
-000005a0: 7220 746f 2075 7365 7220 5448 6970 7374  r to user THipst
-000005b0: 6572 2c20 796f 7520 7769 6c6c 206e 6565  er, you will nee
-000005c0: 6420 746f 2068 6176 6520 7468 6520 666f  d to have the fo
-000005d0: 6c6c 6f77 696e 6720 696e 7374 616c 6c65  llowing installe
-000005e0: 643a 0a2d 205b 5079 7468 6f6e 5d28 6874  d:.- [Python](ht
-000005f0: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000600: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
-00000610: 2028 332e 3131 2b29 0a2d 205b 7069 7065   (3.11+).- [pipe
-00000620: 6e76 5d28 6874 7470 733a 2f2f 7069 7065  nv](https://pipe
-00000630: 6e76 2e70 7970 612e 696f 2f65 6e2f 6c61  nv.pypa.io/en/la
-00000640: 7465 7374 2f29 2076 3230 3231 2e35 2b0a  test/) v2021.5+.
-00000650: 2d20 5b54 6572 7261 666f 726d 2043 4c49  - [Terraform CLI
-00000660: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00000670: 7065 722e 6861 7368 6963 6f72 702e 636f  per.hashicorp.co
-00000680: 6d2f 7465 7272 6166 6f72 6d2f 7475 746f  m/terraform/tuto
-00000690: 7269 616c 732f 6177 732d 6765 742d 7374  rials/aws-get-st
-000006a0: 6172 7465 642f 696e 7374 616c 6c2d 636c  arted/install-cl
-000006b0: 6929 2028 312e 322b 290a 2d20 5b4e 6f64  i) (1.2+).- [Nod
-000006c0: 652e 6a73 5d28 6874 7470 733a 2f2f 6e6f  e.js](https://no
-000006d0: 6465 6a73 2e6f 7267 2f29 2061 6e64 206e  dejs.org/) and n
-000006e0: 706d 2076 3136 2b2e 0a0a 2323 2049 6e73  pm v16+...## Ins
-000006f0: 7461 6c6c 6174 696f 6e0a 0a54 6f20 7573  tallation..To us
-00000700: 6520 5448 6970 7374 6572 2c20 796f 7520  e THipster, you 
-00000710: 6361 6e20 7369 6d70 6c79 2069 6e73 7461  can simply insta
-00000720: 6c6c 2074 6865 2070 6163 6b61 6765 2077  ll the package w
-00000730: 6974 6820 7069 703a 0a0a 6060 6063 6f6e  ith pip:..```con
-00000740: 736f 6c65 0a70 6970 2069 6e73 7461 6c6c  sole.pip install
-00000750: 2074 6869 7073 7465 720a 6060 600a 0a49   thipster.```..I
-00000760: 6620 796f 7520 7761 6e74 2074 6f20 696e  f you want to in
-00000770: 7374 616c 6c20 7468 6520 676f 6f67 6c65  stall the google
-00000780: 2064 6570 656e 6465 6e63 6965 7320 6173   dependencies as
-00000790: 7765 6c6c 2075 7365 0a0a 6060 6063 6f6e  well use..```con
-000007a0: 736f 6c65 0a70 6970 2069 6e73 7461 6c6c  sole.pip install
-000007b0: 2074 6869 7073 7465 725b 676f 6f67 6c65   thipster[google
-000007c0: 5d0a 6060 600a 0a54 6865 206c 6973 7420  ].```..The list 
-000007d0: 6f66 2061 7661 696c 6162 6c65 2076 6572  of available ver
-000007e0: 7369 6f6e 7320 6361 6e20 6265 2066 6f75  sions can be fou
-000007f0: 6e64 206f 6e20 5b50 7950 495d 2868 7474  nd on [PyPI](htt
-00000800: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000810: 6f6a 6563 742f 7468 6970 7374 6572 2f29  oject/thipster/)
-00000820: 2e0a 0a23 2320 5573 6167 650a 0a59 6f75  ...## Usage..You
-00000830: 2063 616e 2075 7365 2054 4869 7073 7465   can use THipste
-00000840: 7220 696e 2074 776f 2077 6179 733a 0a2d  r in two ways:.-
-00000850: 2042 7920 6c65 7665 7261 6769 6e67 2074   By leveraging t
-00000860: 6865 205b 5448 6970 7374 6572 2043 4c49  he [THipster CLI
-00000870: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000880: 2e63 6f6d 2f54 4869 7073 7465 722f 5448  .com/THipster/TH
-00000890: 6970 7374 6572 2d63 6c69 290a 2d20 4279  ipster-cli).- By
-000008a0: 2064 6972 6563 746c 7920 7573 696e 6720   directly using 
-000008b0: 7468 6520 5b54 4869 7073 7465 7220 5079  the [THipster Py
-000008c0: 7468 6f6e 2070 6163 6b61 6765 5d28 6874  thon package](ht
-000008d0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-000008e0: 726f 6a65 6374 2f74 6869 7073 7465 722f  roject/thipster/
-000008f0: 2920 696e 2079 6f75 7220 6f77 6e20 636f  ) in your own co
-00000900: 6465 0a0a 4d61 696e 2066 6561 7475 7265  de..Main feature
-00000910: 3a0a 2d20 4765 6e65 7261 7465 2054 6572  :.- Generate Ter
-00000920: 7261 666f 726d 2066 696c 6573 2066 726f  raform files fro
-00000930: 6d20 6120 5941 4d4c 2b4a 494e 4a41 206f  m a YAML+JINJA o
-00000940: 7220 5448 4950 5320 6669 6c65 3a0a 6060  r THIPS file:.``
-00000950: 6070 7974 686f 6e0a 6672 6f6d 2074 6869  `python.from thi
-00000960: 7073 7465 7220 696d 706f 7274 2045 6e67  pster import Eng
-00000970: 696e 6520 6173 2054 6869 7073 7465 7245  ine as ThipsterE
-00000980: 6e67 696e 650a 6672 6f6d 2074 6869 7073  ngine.from thips
-00000990: 7465 722e 6175 7468 2069 6d70 6f72 7420  ter.auth import 
-000009a0: 476f 6f67 6c65 0a66 726f 6d20 7468 6970  Google.from thip
-000009b0: 7374 6572 2e70 6172 7365 7220 696d 706f  ster.parser impo
-000009c0: 7274 2050 6172 7365 7246 6163 746f 7279  rt ParserFactory
-000009d0: 0a66 726f 6d20 7468 6970 7374 6572 2e72  .from thipster.r
-000009e0: 6570 6f73 6974 6f72 7920 696d 706f 7274  epository import
-000009f0: 2047 6974 6875 6252 6570 6f0a 6672 6f6d   GithubRepo.from
-00000a00: 2074 6869 7073 7465 722e 7465 7272 6166   thipster.terraf
-00000a10: 6f72 6d20 696d 706f 7274 2054 6572 7261  orm import Terra
-00000a20: 666f 726d 0a0a 2320 6372 6561 7465 206e  form..# create n
-00000a30: 6577 2054 4869 7073 7465 7220 656e 6769  ew THipster engi
-00000a40: 6e65 0a65 6e67 696e 6520 3d20 5468 6970  ne.engine = Thip
-00000a50: 7374 6572 456e 6769 6e65 2850 6172 7365  sterEngine(Parse
-00000a60: 7246 6163 746f 7279 2829 2c20 4769 7468  rFactory(), Gith
-00000a70: 7562 5265 706f 2827 5448 6970 7374 6572  ubRepo('THipster
-00000a80: 2f6d 6f64 656c 7327 292c 2047 6f6f 676c  /models'), Googl
-00000a90: 652c 2054 6572 7261 666f 726d 2829 290a  e, Terraform()).
-00000aa0: 0a23 2067 656e 6572 6174 6520 5465 7272  .# generate Terr
-00000ab0: 6166 6f72 6d20 6669 6c65 7320 616e 6420  aform files and 
-00000ac0: 706c 616e 2066 726f 6d20 6120 5941 4d4c  plan from a YAML
-00000ad0: 2b4a 494e 4a41 2066 696c 650a 7465 7272  +JINJA file.terr
-00000ae0: 6166 6f72 6d5f 706c 616e 203d 2065 6e67  aform_plan = eng
-00000af0: 696e 652e 7275 6e28 2770 6174 682f 746f  ine.run('path/to
-00000b00: 2f66 696c 652f 6f72 2f64 6972 6563 746f  /file/or/directo
-00000b10: 7279 2729 0a70 7269 6e74 2874 6572 7261  ry').print(terra
-00000b20: 666f 726d 5f70 6c61 6e29 0a60 6060 0a0a  form_plan).```..
-00000b30: 2323 2048 6f77 2074 6f20 7465 7374 2074  ## How to test t
-00000b40: 6865 2073 6f66 7477 6172 650a 0a54 6f20  he software..To 
-00000b50: 7275 6e20 7468 6520 7465 7374 732c 2079  run the tests, y
-00000b60: 6f75 2063 616e 2075 7365 2074 6865 2066  ou can use the f
-00000b70: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00000b80: 3a0a 0a60 6060 636f 6e73 6f6c 650a 7069  :..```console.pi
-00000b90: 7020 696e 7374 616c 6c20 2d65 202e 5b74  p install -e .[t
-00000ba0: 6573 745d 0a70 7974 6573 7420 7465 7374  est].pytest test
-00000bb0: 730a 6060 600a 0a23 2320 4b6e 6f77 6e20  s.```..## Known 
-00000bc0: 6973 7375 6573 0a0a 416c 6c20 6b6e 6f77  issues..All know
-00000bd0: 6e20 6973 7375 6573 2c20 6275 6773 2c20  n issues, bugs, 
-00000be0: 616e 6420 6665 6174 7572 6520 7265 7175  and feature requ
-00000bf0: 6573 7473 2061 7265 2074 7261 636b 6564  ests are tracked
-00000c00: 2069 6e20 7468 6520 5b49 7373 7565 2074   in the [Issue t
-00000c10: 7261 636b 6572 5d28 6874 7470 733a 2f2f  racker](https://
-00000c20: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
-00000c30: 7465 722f 5448 6970 7374 6572 2f69 7373  ter/THipster/iss
-00000c40: 7565 7329 2e0a 0a23 2320 4765 7474 696e  ues)...## Gettin
-00000c50: 6720 6865 6c70 0a0a 4966 2079 6f75 2068  g help..If you h
-00000c60: 6176 6520 7175 6573 7469 6f6e 732c 2063  ave questions, c
-00000c70: 6f6e 6365 726e 732c 2062 7567 2072 6570  oncerns, bug rep
-00000c80: 6f72 7473 2c20 6574 632c 2070 6c65 6173  orts, etc, pleas
-00000c90: 6520 6669 6c65 2061 6e20 6973 7375 6520  e file an issue 
-00000ca0: 696e 2074 6869 7320 7265 706f 7369 746f  in this reposito
-00000cb0: 7279 2773 205b 4973 7375 6520 7472 6163  ry's [Issue trac
-00000cc0: 6b65 725d 2868 7474 7073 3a2f 2f67 6974  ker](https://git
-00000cd0: 6875 622e 636f 6d2f 5448 6970 7374 6572  hub.com/THipster
-00000ce0: 2f54 4869 7073 7465 722f 6973 7375 6573  /THipster/issues
-00000cf0: 292e 0a0a 2323 2047 6574 7469 6e67 2069  )...## Getting i
-00000d00: 6e76 6f6c 7665 640a 0a54 6f20 696e 7374  nvolved..To inst
-00000d10: 616c 6c20 7468 6520 7072 6f6a 6563 7420  all the project 
-00000d20: 666f 7220 6465 7665 6c6f 706d 656e 742c  for development,
-00000d30: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00000d40: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000d50: 6e64 3a0a 0a60 6060 636f 6e73 6f6c 650a  nd:..```console.
-00000d60: 7069 7020 696e 7374 616c 6c20 2d72 2072  pip install -r r
-00000d70: 6571 7569 7265 6d65 6e74 732e 7478 7420  equirements.txt 
-00000d80: 2626 2070 6970 2069 6e73 7461 6c6c 202d  && pip install -
-00000d90: 6520 2e5b 6465 762c 7465 7374 2c64 6f63  e .[dev,test,doc
-00000da0: 2c67 6f6f 676c 655d 0a70 7265 2d63 6f6d  ,google].pre-com
-00000db0: 6d69 7420 696e 7374 616c 6c20 2626 2070  mit install && p
-00000dc0: 7265 2d63 6f6d 6d69 7420 7275 6e20 2d2d  re-commit run --
-00000dd0: 616c 6c2d 6669 6c65 730a 6060 600a 0a46  all-files.```..F
-00000de0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00000df0: 696f 6e20 6f6e 2068 6f77 2074 6f20 6865  ion on how to he
-00000e00: 6c70 206f 7574 2c20 706c 6561 7365 2063  lp out, please c
-00000e10: 6865 636b 2074 6865 205b 434f 4e54 5249  heck the [CONTRI
-00000e20: 4255 5449 4e47 5d28 6874 7470 733a 2f2f  BUTING](https://
-00000e30: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
-00000e40: 7465 722f 5448 6970 7374 6572 2f62 6c6f  ter/THipster/blo
-00000e50: 622f 6d61 696e 2f43 4f4e 5452 4942 5554  b/main/CONTRIBUT
-00000e60: 494e 472e 6d64 2920 6669 6c65 2e0a 0a23  ING.md) file...#
-00000e70: 2320 4f70 656e 2073 6f75 7263 6520 6c69  # Open source li
-00000e80: 6365 6e73 696e 6720 696e 666f 0a31 2e20  censing info.1. 
-00000e90: 5b4c 4943 454e 5345 5d28 6874 7470 733a  [LICENSE](https:
-00000ea0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 4869  //github.com/THi
-00000eb0: 7073 7465 722f 5448 6970 7374 6572 2f62  pster/THipster/b
-00000ec0: 6c6f 622f 6d61 696e 2f4c 4943 454e 5345  lob/main/LICENSE
-00000ed0: 290a 322e 205b 4346 5042 2053 6f75 7263  ).2. [CFPB Sourc
-00000ee0: 6520 436f 6465 2050 6f6c 6963 795d 2868  e Code Policy](h
-00000ef0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000f00: 6d2f 6366 7062 2f73 6f75 7263 652d 636f  m/cfpb/source-co
-00000f10: 6465 2d70 6f6c 6963 792f 290a 0a23 2320  de-policy/)..## 
-00000f20: 4372 6564 6974 7320 616e 6420 7265 6665  Credits and refe
-00000f30: 7265 6e63 6573 0a0a 312e 2050 726f 6a65  rences..1. Proje
-00000f40: 6374 7320 7468 6174 2069 6e73 7069 7265  cts that inspire
-00000f50: 6420 796f 750a 2020 2020 2d20 5b41 5753  d you.    - [AWS
-00000f60: 2041 7070 6c69 6361 7469 6f6e 2043 6f6d   Application Com
-00000f70: 706f 7365 725d 2868 7474 7073 3a2f 2f61  poser](https://a
-00000f80: 7773 2e61 6d61 7a6f 6e2e 636f 6d2f 6170  ws.amazon.com/ap
-00000f90: 706c 6963 6174 696f 6e2d 636f 6d70 6f73  plication-compos
-00000fa0: 6572 2f3f 6e63 313d 685f 6c73 290a 322e  er/?nc1=h_ls).2.
-00000fb0: 2052 656c 6174 6564 2070 726f 6a65 6374   Related project
-00000fc0: 730a 2020 2020 2d20 5b57 696e 6720 5072  s.    - [Wing Pr
-00000fd0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000fe0: 6765 5d28 6874 7470 733a 2f2f 7777 772e  ge](https://www.
-00000ff0: 7769 6e67 6c61 6e67 2e69 6f2f 290a       winglang.io/).
+00000180: 722f 5448 6970 7374 6572 2e67 6974 0a4b  r/THipster.git.K
+00000190: 6579 776f 7264 733a 2074 6869 7073 7465  eywords: thipste
+000001a0: 722c 7465 7272 6166 6f72 6d2c 696e 6672  r,terraform,infr
+000001b0: 6173 7472 7563 7475 7265 2c69 6e66 7261  astructure,infra
+000001c0: 7374 7275 6374 7572 652d 6173 2d63 6f64  structure-as-cod
+000001d0: 652c 6961 632c 6765 6e65 7261 746f 722c  e,iac,generator,
+000001e0: 6473 6c2c 7961 6d6c 0a43 6c61 7373 6966  dsl,yaml.Classif
+000001f0: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
+00000200: 2053 7461 7475 7320 3a3a 2031 202d 2050   Status :: 1 - P
+00000210: 6c61 6e6e 696e 670a 436c 6173 7369 6669  lanning.Classifi
+00000220: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000230: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000240: 6f6e 203a 3a20 332e 3131 0a43 6c61 7373  on :: 3.11.Class
+00000250: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000260: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000270: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
+00000280: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000290: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000002a0: 2049 6e64 6570 656e 6465 6e74 0a44 6573   Independent.Des
+000002b0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000002c0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000002d0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+000002e0: 7472 613a 2074 6573 740a 5072 6f76 6964  tra: test.Provid
+000002f0: 6573 2d45 7874 7261 3a20 6465 760a 5072  es-Extra: dev.Pr
+00000300: 6f76 6964 6573 2d45 7874 7261 3a20 646f  ovides-Extra: do
+00000310: 630a 5072 6f76 6964 6573 2d45 7874 7261  c.Provides-Extra
+00000320: 3a20 676f 6f67 6c65 0a4c 6963 656e 7365  : google.License
+00000330: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000340: 2320 5448 6970 7374 6572 0a0a 5448 6970  # THipster..THip
+00000350: 7374 6572 2069 7320 6120 746f 6f6c 2064  ster is a tool d
+00000360: 6564 6963 6174 6564 2074 6f20 7369 6d70  edicated to simp
+00000370: 6c69 6679 696e 6720 7468 6520 6469 6666  lifying the diff
+00000380: 6963 756c 7479 2061 7373 6f63 6961 7465  iculty associate
+00000390: 6420 7769 7468 2077 7269 7469 6e67 2054  d with writing T
+000003a0: 6572 7261 666f 726d 2066 696c 6573 2e0a  erraform files..
+000003b0: 4974 2061 6c6c 6f77 7320 7573 6572 7320  It allows users 
+000003c0: 746f 2077 7269 7465 2069 6e66 7261 7374  to write infrast
+000003d0: 7275 6374 7572 6520 6173 2063 6f64 6520  ructure as code 
+000003e0: 696e 2061 2073 696d 706c 6966 6965 6420  in a simplified 
+000003f0: 666f 726d 6174 2c20 7573 696e 6720 6569  format, using ei
+00000400: 7468 6572 2059 414d 4c20 2877 6974 6820  ther YAML (with 
+00000410: 4a49 4e4a 4129 206f 7220 7468 6520 6465  JINJA) or the de
+00000420: 6469 6361 7465 6420 5468 6970 7374 6572  dicated Thipster
+00000430: 2044 534c 2e0a 0a57 7269 7474 656e 2065   DSL...Written e
+00000440: 6e74 6972 656c 7920 696e 2050 7974 686f  ntirely in Pytho
+00000450: 6e2c 2069 7420 6c65 7665 7261 6765 7320  n, it leverages 
+00000460: 7468 6520 5079 7468 6f6e 2043 444b 2066  the Python CDK f
+00000470: 6f72 2054 6572 7261 666f 726d 2074 6f20  or Terraform to 
+00000480: 6372 6561 7465 2054 6572 7261 666f 726d  create Terraform
+00000490: 2066 696c 6573 2061 6e64 2061 7070 6c79   files and apply
+000004a0: 2074 6865 6d20 746f 2074 6865 2063 686f   them to the cho
+000004b0: 7365 6e20 7072 6f76 6964 6572 2e0a 0a3c  sen provider...<
+000004c0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000004d0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+000004e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000004f0: 5448 6970 7374 6572 2f54 4869 7073 7465  THipster/THipste
+00000500: 722f 626c 6f62 2f6d 6169 6e2f 4c49 4345  r/blob/main/LICE
+00000510: 4e53 4522 2074 6172 6765 743d 225f 626c  NSE" target="_bl
+00000520: 616e 6b22 2061 6c74 3d22 4c69 6365 6e73  ank" alt="Licens
+00000530: 6522 3e0a 2020 2020 3c69 6d67 2073 7263  e">.    <img src
+00000540: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000550: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000560: 6c69 6365 6e73 652f 5448 6970 7374 6572  license/THipster
+00000570: 2f54 4869 7073 7465 7222 2061 6c74 3d22  /THipster" alt="
+00000580: 4c69 6365 6e73 6522 3e0a 2020 3c2f 613e  License">.  </a>
+00000590: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+000005a0: 733a 2f2f 7468 6970 7374 6572 2e72 6561  s://thipster.rea
+000005b0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000005c0: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
+000005d0: 6573 7422 2074 6172 6765 743d 225f 626c  est" target="_bl
+000005e0: 616e 6b22 2061 6c74 3d22 5265 6164 2074  ank" alt="Read t
+000005f0: 6865 2064 6f63 7320 646f 6375 6d65 6e74  he docs document
+00000600: 6174 696f 6e22 3e0a 2020 2020 3c69 6d67  ation">.    <img
+00000610: 2073 7263 3d22 6874 7470 733a 2f2f 7265   src="https://re
+00000620: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00000630: 6f6a 6563 7473 2f74 6869 7073 7465 722f  ojects/thipster/
+00000640: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000650: 6174 6573 7422 2061 6c74 3d22 5265 6164  atest" alt="Read
+00000660: 2074 6865 2064 6f63 7320 646f 6375 6d65   the docs docume
+00000670: 6e74 6174 696f 6e22 3e0a 2020 3c2f 613e  ntation">.  </a>
+00000680: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000690: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000006a0: 6a65 6374 2f74 6869 7073 7465 722f 2220  ject/thipster/" 
+000006b0: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
+000006c0: 616c 743d 2250 7950 6920 7061 636b 6167  alt="PyPi packag
+000006d0: 6522 3e0a 2020 2020 3c69 6d67 2073 7263  e">.    <img src
+000006e0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000006f0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000700: 7468 6970 7374 6572 3f63 6f6c 6f72 3d62  thipster?color=b
+00000710: 7269 6768 7467 7265 656e 266c 6162 656c  rightgreen&label
+00000720: 3d70 7970 6925 3230 7061 636b 6167 6522  =pypi%20package"
+00000730: 2061 6c74 3d22 5061 636b 6167 6520 7665   alt="Package ve
+00000740: 7273 696f 6e22 3e0a 2020 3c2f 613e 0a20  rsion">.  </a>. 
+00000750: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000760: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000770: 6374 2f74 6869 7073 7465 722f 2220 7461  ct/thipster/" ta
+00000780: 7267 6574 3d22 5f62 6c61 6e6b 2220 616c  rget="_blank" al
+00000790: 743d 2250 7950 6920 7061 636b 6167 6522  t="PyPi package"
+000007a0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+000007b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000007c0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+000007d0: 7273 696f 6e73 2f74 6869 7073 7465 723f  rsions/thipster?
+000007e0: 636f 6c6f 723d 6272 6967 6874 6772 6565  color=brightgree
+000007f0: 6e22 2061 6c74 3d22 5375 7070 6f72 7465  n" alt="Supporte
+00000800: 6420 5079 7468 6f6e 2076 6572 7369 6f6e  d Python version
+00000810: 7322 3e0a 2020 3c2f 613e 0a3c 2f70 3e0a  s">.  </a>.</p>.
+00000820: 0a23 2320 5465 6368 6e6f 6c6f 6779 2053  .## Technology S
+00000830: 7461 636b 0a57 7269 7474 656e 2069 6e20  tack.Written in 
+00000840: 5079 7468 6f6e 2033 2e31 312c 2074 6869  Python 3.11, thi
+00000850: 7073 7465 7220 6973 2064 6573 6967 6e65  pster is designe
+00000860: 6420 6173 2061 2070 7974 686f 6e20 7061  d as a python pa
+00000870: 636b 6167 652c 2074 6f20 6265 2075 7365  ckage, to be use
+00000880: 6420 6569 7468 6572 2061 7320 6120 7374  d either as a st
+00000890: 616e 6461 6c6f 6e65 2074 6f6f 6c2c 206f  andalone tool, o
+000008a0: 7220 6173 2061 206d 6f64 756c 6520 696e  r as a module in
+000008b0: 7369 6465 2061 2072 756e 6e69 6e67 2070  side a running p
+000008c0: 726f 6365 7373 206c 696b 6520 6120 4349  rocess like a CI
+000008d0: 2f43 4420 7069 7065 6c69 6e65 2e0a 0a23  /CD pipeline...#
+000008e0: 2320 5072 6f6a 6563 7420 5374 6174 7573  # Project Status
+000008f0: 0a54 4869 7073 7465 7220 6973 2063 7572  .THipster is cur
+00000900: 7265 6e74 6c79 2069 6e20 616e 2061 6374  rently in an act
+00000910: 6976 6520 6465 7665 6c6f 706d 656e 7420  ive development 
+00000920: 7374 6174 652e 2049 6620 796f 7520 7761  state. If you wa
+00000930: 6e74 2074 6f20 6b6e 6f77 206d 6f72 652c  nt to know more,
+00000940: 2070 6c65 6173 6520 6368 6563 6b20 7468   please check th
+00000950: 6520 5b43 4841 4e47 454c 4f47 5d28 6874  e [CHANGELOG](ht
+00000960: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000970: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00000980: 6572 2f62 6c6f 622f 6d61 696e 2f43 4841  er/blob/main/CHA
+00000990: 4e47 454c 4f47 2e6d 6429 2066 6f72 206d  NGELOG.md) for m
+000009a0: 6f72 6520 6465 7461 696c 732e 0a0a 2323  ore details...##
+000009b0: 2044 6570 656e 6465 6e63 6965 730a 0a49   Dependencies..I
+000009c0: 6e20 6f72 6465 7220 746f 2075 7365 7220  n order to user 
+000009d0: 5448 6970 7374 6572 2c20 796f 7520 7769  THipster, you wi
+000009e0: 6c6c 206e 6565 6420 746f 2068 6176 6520  ll need to have 
+000009f0: 7468 6520 666f 6c6c 6f77 696e 6720 696e  the following in
+00000a00: 7374 616c 6c65 643a 0a2d 205b 5079 7468  stalled:.- [Pyth
+00000a10: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
+00000a20: 7079 7468 6f6e 2e6f 7267 2f64 6f77 6e6c  python.org/downl
+00000a30: 6f61 6473 2f29 2028 332e 3131 2b29 0a2d  oads/) (3.11+).-
+00000a40: 205b 7069 7065 6e76 5d28 6874 7470 733a   [pipenv](https:
+00000a50: 2f2f 7069 7065 6e76 2e70 7970 612e 696f  //pipenv.pypa.io
+00000a60: 2f65 6e2f 6c61 7465 7374 2f29 2076 3230  /en/latest/) v20
+00000a70: 3231 2e35 2b0a 2d20 5b54 6572 7261 666f  21.5+.- [Terrafo
+00000a80: 726d 2043 4c49 5d28 6874 7470 733a 2f2f  rm CLI](https://
+00000a90: 6465 7665 6c6f 7065 722e 6861 7368 6963  developer.hashic
+00000aa0: 6f72 702e 636f 6d2f 7465 7272 6166 6f72  orp.com/terrafor
+00000ab0: 6d2f 7475 746f 7269 616c 732f 6177 732d  m/tutorials/aws-
+00000ac0: 6765 742d 7374 6172 7465 642f 696e 7374  get-started/inst
+00000ad0: 616c 6c2d 636c 6929 2028 312e 322b 290a  all-cli) (1.2+).
+00000ae0: 2d20 5b4e 6f64 652e 6a73 5d28 6874 7470  - [Node.js](http
+00000af0: 733a 2f2f 6e6f 6465 6a73 2e6f 7267 2f29  s://nodejs.org/)
+00000b00: 2061 6e64 206e 706d 2076 3136 2b2e 0a0a   and npm v16+...
+00000b10: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
+00000b20: 0a54 6f20 7573 6520 5448 6970 7374 6572  .To use THipster
+00000b30: 2c20 796f 7520 6361 6e20 7369 6d70 6c79  , you can simply
+00000b40: 2069 6e73 7461 6c6c 2074 6865 2070 6163   install the pac
+00000b50: 6b61 6765 2077 6974 6820 7069 703a 0a0a  kage with pip:..
+00000b60: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
+00000b70: 6e73 7461 6c6c 2074 6869 7073 7465 720a  nstall thipster.
+00000b80: 6060 600a 0a49 6620 796f 7520 7761 6e74  ```..If you want
+00000b90: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+00000ba0: 676f 6f67 6c65 2064 6570 656e 6465 6e63  google dependenc
+00000bb0: 6965 7320 6173 7765 6c6c 2075 7365 0a0a  ies aswell use..
+00000bc0: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
+00000bd0: 6e73 7461 6c6c 2074 6869 7073 7465 725b  nstall thipster[
+00000be0: 676f 6f67 6c65 5d0a 6060 600a 0a54 6865  google].```..The
+00000bf0: 206c 6973 7420 6f66 2061 7661 696c 6162   list of availab
+00000c00: 6c65 2076 6572 7369 6f6e 7320 6361 6e20  le versions can 
+00000c10: 6265 2066 6f75 6e64 206f 6e20 5b50 7950  be found on [PyP
+00000c20: 495d 2868 7474 7073 3a2f 2f70 7970 692e  I](https://pypi.
+00000c30: 6f72 672f 7072 6f6a 6563 742f 7468 6970  org/project/thip
+00000c40: 7374 6572 2f29 2e0a 0a23 2320 5573 6167  ster/)...## Usag
+00000c50: 650a 0a59 6f75 2063 616e 2075 7365 2054  e..You can use T
+00000c60: 4869 7073 7465 7220 696e 2074 776f 2077  Hipster in two w
+00000c70: 6179 733a 0a2d 2042 7920 6c65 7665 7261  ays:.- By levera
+00000c80: 6769 6e67 2074 6865 205b 5448 6970 7374  ging the [THipst
+00000c90: 6572 2043 4c49 5d28 6874 7470 733a 2f2f  er CLI](https://
+00000ca0: 6769 7468 7562 2e63 6f6d 2f54 4869 7073  github.com/THips
+00000cb0: 7465 722f 5448 6970 7374 6572 2d63 6c69  ter/THipster-cli
+00000cc0: 290a 2d20 4279 2064 6972 6563 746c 7920  ).- By directly 
+00000cd0: 7573 696e 6720 7468 6520 5b54 4869 7073  using the [THips
+00000ce0: 7465 7220 5079 7468 6f6e 2070 6163 6b61  ter Python packa
+00000cf0: 6765 5d28 6874 7470 733a 2f2f 7079 7069  ge](https://pypi
+00000d00: 2e6f 7267 2f70 726f 6a65 6374 2f74 6869  .org/project/thi
+00000d10: 7073 7465 722f 2920 696e 2079 6f75 7220  pster/) in your 
+00000d20: 6f77 6e20 636f 6465 0a0a 4d61 696e 2066  own code..Main f
+00000d30: 6561 7475 7265 3a0a 2d20 4765 6e65 7261  eature:.- Genera
+00000d40: 7465 2054 6572 7261 666f 726d 2066 696c  te Terraform fil
+00000d50: 6573 2066 726f 6d20 6120 5941 4d4c 2b4a  es from a YAML+J
+00000d60: 494e 4a41 206f 7220 5448 4950 5320 6669  INJA or THIPS fi
+00000d70: 6c65 3a0a 6060 6070 7974 686f 6e0a 6672  le:.```python.fr
+00000d80: 6f6d 2074 6869 7073 7465 7220 696d 706f  om thipster impo
+00000d90: 7274 2045 6e67 696e 6520 6173 2054 6869  rt Engine as Thi
+00000da0: 7073 7465 7245 6e67 696e 650a 6672 6f6d  psterEngine.from
+00000db0: 2074 6869 7073 7465 722e 6175 7468 2069   thipster.auth i
+00000dc0: 6d70 6f72 7420 476f 6f67 6c65 0a66 726f  mport Google.fro
+00000dd0: 6d20 7468 6970 7374 6572 2e70 6172 7365  m thipster.parse
+00000de0: 7220 696d 706f 7274 2050 6172 7365 7246  r import ParserF
+00000df0: 6163 746f 7279 0a66 726f 6d20 7468 6970  actory.from thip
+00000e00: 7374 6572 2e72 6570 6f73 6974 6f72 7920  ster.repository 
+00000e10: 696d 706f 7274 2047 6974 6875 6252 6570  import GithubRep
+00000e20: 6f0a 6672 6f6d 2074 6869 7073 7465 722e  o.from thipster.
+00000e30: 7465 7272 6166 6f72 6d20 696d 706f 7274  terraform import
+00000e40: 2054 6572 7261 666f 726d 0a0a 2320 6372   Terraform..# cr
+00000e50: 6561 7465 206e 6577 2054 4869 7073 7465  eate new THipste
+00000e60: 7220 656e 6769 6e65 0a65 6e67 696e 6520  r engine.engine 
+00000e70: 3d20 5468 6970 7374 6572 456e 6769 6e65  = ThipsterEngine
+00000e80: 2850 6172 7365 7246 6163 746f 7279 2829  (ParserFactory()
+00000e90: 2c20 4769 7468 7562 5265 706f 2827 5448  , GithubRepo('TH
+00000ea0: 6970 7374 6572 2f6d 6f64 656c 7327 292c  ipster/models'),
+00000eb0: 2047 6f6f 676c 652c 2054 6572 7261 666f   Google, Terrafo
+00000ec0: 726d 2829 290a 0a23 2067 656e 6572 6174  rm())..# generat
+00000ed0: 6520 5465 7272 6166 6f72 6d20 6669 6c65  e Terraform file
+00000ee0: 7320 616e 6420 706c 616e 2066 726f 6d20  s and plan from 
+00000ef0: 6120 5941 4d4c 2b4a 494e 4a41 2066 696c  a YAML+JINJA fil
+00000f00: 650a 7465 7272 6166 6f72 6d5f 706c 616e  e.terraform_plan
+00000f10: 203d 2065 6e67 696e 652e 7275 6e28 2770   = engine.run('p
+00000f20: 6174 682f 746f 2f66 696c 652f 6f72 2f64  ath/to/file/or/d
+00000f30: 6972 6563 746f 7279 2729 0a70 7269 6e74  irectory').print
+00000f40: 2874 6572 7261 666f 726d 5f70 6c61 6e29  (terraform_plan)
+00000f50: 0a60 6060 0a0a 2323 2048 6f77 2074 6f20  .```..## How to 
+00000f60: 7465 7374 2074 6865 2073 6f66 7477 6172  test the softwar
+00000f70: 650a 0a54 6f20 7275 6e20 7468 6520 7465  e..To run the te
+00000f80: 7374 732c 2079 6f75 2063 616e 2075 7365  sts, you can use
+00000f90: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00000fa0: 6f6d 6d61 6e64 3a0a 0a60 6060 636f 6e73  ommand:..```cons
+00000fb0: 6f6c 650a 7069 7020 696e 7374 616c 6c20  ole.pip install 
+00000fc0: 2d65 202e 5b74 6573 745d 0a70 7974 6573  -e .[test].pytes
+00000fd0: 7420 7465 7374 730a 6060 600a 0a23 2320  t tests.```..## 
+00000fe0: 4b6e 6f77 6e20 6973 7375 6573 0a0a 416c  Known issues..Al
+00000ff0: 6c20 6b6e 6f77 6e20 6973 7375 6573 2c20  l known issues, 
+00001000: 6275 6773 2c20 616e 6420 6665 6174 7572  bugs, and featur
+00001010: 6520 7265 7175 6573 7473 2061 7265 2074  e requests are t
+00001020: 7261 636b 6564 2069 6e20 7468 6520 5b49  racked in the [I
+00001030: 7373 7565 2074 7261 636b 6572 5d28 6874  ssue tracker](ht
+00001040: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001050: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00001060: 6572 2f69 7373 7565 7329 2e0a 0a23 2320  er/issues)...## 
+00001070: 4765 7474 696e 6720 6865 6c70 0a0a 4966  Getting help..If
+00001080: 2079 6f75 2068 6176 6520 7175 6573 7469   you have questi
+00001090: 6f6e 732c 2063 6f6e 6365 726e 732c 2062  ons, concerns, b
+000010a0: 7567 2072 6570 6f72 7473 2c20 6574 632c  ug reports, etc,
+000010b0: 2070 6c65 6173 6520 6669 6c65 2061 6e20   please file an 
+000010c0: 6973 7375 6520 696e 2074 6869 7320 7265  issue in this re
+000010d0: 706f 7369 746f 7279 2773 205b 4973 7375  pository's [Issu
+000010e0: 6520 7472 6163 6b65 725d 2868 7474 7073  e tracker](https
+000010f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5448  ://github.com/TH
+00001100: 6970 7374 6572 2f54 4869 7073 7465 722f  ipster/THipster/
+00001110: 6973 7375 6573 292e 0a0a 2323 2047 6574  issues)...## Get
+00001120: 7469 6e67 2069 6e76 6f6c 7665 640a 0a54  ting involved..T
+00001130: 6f20 696e 7374 616c 6c20 7468 6520 7072  o install the pr
+00001140: 6f6a 6563 7420 666f 7220 6465 7665 6c6f  oject for develo
+00001150: 706d 656e 742c 2079 6f75 2063 616e 2075  pment, you can u
+00001160: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00001170: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 636f   command:..```co
+00001180: 6e73 6f6c 650a 7069 7020 696e 7374 616c  nsole.pip instal
+00001190: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
+000011a0: 732e 7478 7420 2626 2070 6970 2069 6e73  s.txt && pip ins
+000011b0: 7461 6c6c 202d 6520 2e5b 6465 762c 7465  tall -e .[dev,te
+000011c0: 7374 2c64 6f63 2c67 6f6f 676c 655d 0a70  st,doc,google].p
+000011d0: 7265 2d63 6f6d 6d69 7420 696e 7374 616c  re-commit instal
+000011e0: 6c20 2626 2070 7265 2d63 6f6d 6d69 7420  l && pre-commit 
+000011f0: 7275 6e20 2d2d 616c 6c2d 6669 6c65 730a  run --all-files.
+00001200: 6060 600a 0a46 6f72 206d 6f72 6520 696e  ```..For more in
+00001210: 666f 726d 6174 696f 6e20 6f6e 2068 6f77  formation on how
+00001220: 2074 6f20 6865 6c70 206f 7574 2c20 706c   to help out, pl
+00001230: 6561 7365 2063 6865 636b 2074 6865 205b  ease check the [
+00001240: 434f 4e54 5249 4255 5449 4e47 5d28 6874  CONTRIBUTING](ht
+00001250: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001260: 2f54 4869 7073 7465 722f 5448 6970 7374  /THipster/THipst
+00001270: 6572 2f62 6c6f 622f 6d61 696e 2f43 4f4e  er/blob/main/CON
+00001280: 5452 4942 5554 494e 472e 6d64 2920 6669  TRIBUTING.md) fi
+00001290: 6c65 2e0a 0a23 2320 4f70 656e 2073 6f75  le...## Open sou
+000012a0: 7263 6520 6c69 6365 6e73 696e 6720 696e  rce licensing in
+000012b0: 666f 0a31 2e20 5b4c 4943 454e 5345 5d28  fo.1. [LICENSE](
+000012c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000012d0: 6f6d 2f54 4869 7073 7465 722f 5448 6970  om/THipster/THip
+000012e0: 7374 6572 2f62 6c6f 622f 6d61 696e 2f4c  ster/blob/main/L
+000012f0: 4943 454e 5345 290a 322e 205b 4346 5042  ICENSE).2. [CFPB
+00001300: 2053 6f75 7263 6520 436f 6465 2050 6f6c   Source Code Pol
+00001310: 6963 795d 2868 7474 7073 3a2f 2f67 6974  icy](https://git
+00001320: 6875 622e 636f 6d2f 6366 7062 2f73 6f75  hub.com/cfpb/sou
+00001330: 7263 652d 636f 6465 2d70 6f6c 6963 792f  rce-code-policy/
+00001340: 290a 0a23 2320 4372 6564 6974 7320 616e  )..## Credits an
+00001350: 6420 7265 6665 7265 6e63 6573 0a0a 312e  d references..1.
+00001360: 2050 726f 6a65 6374 7320 7468 6174 2069   Projects that i
+00001370: 6e73 7069 7265 6420 796f 750a 2020 2020  nspired you.    
+00001380: 2d20 5b41 5753 2041 7070 6c69 6361 7469  - [AWS Applicati
+00001390: 6f6e 2043 6f6d 706f 7365 725d 2868 7474  on Composer](htt
+000013a0: 7073 3a2f 2f61 7773 2e61 6d61 7a6f 6e2e  ps://aws.amazon.
+000013b0: 636f 6d2f 6170 706c 6963 6174 696f 6e2d  com/application-
+000013c0: 636f 6d70 6f73 6572 2f3f 6e63 313d 685f  composer/?nc1=h_
+000013d0: 6c73 290a 322e 2052 656c 6174 6564 2070  ls).2. Related p
+000013e0: 726f 6a65 6374 730a 2020 2020 2d20 5b57  rojects.    - [W
+000013f0: 696e 6720 5072 6f67 7261 6d6d 696e 6720  ing Programming 
+00001400: 4c61 6e67 7561 6765 5d28 6874 7470 733a  Language](https:
+00001410: 2f2f 7777 772e 7769 6e67 6c61 6e67 2e69  //www.winglang.i
+00001420: 6f2f 290a                                o/).
```

### Comparing `thipster-0.16.6/thipster.egg-info/SOURCES.txt` & `thipster-0.16.7/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

