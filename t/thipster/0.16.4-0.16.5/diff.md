# Comparing `tmp/thipster-0.16.4.tar.gz` & `tmp/thipster-0.16.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.16.4.tar", last modified: Mon Jun 12 08:42:39 2023, max compression
+gzip compressed data, was "thipster-0.16.5.tar", last modified: Tue Jun 13 13:41:22 2023, max compression
```

## Comparing `thipster-0.16.4.tar` & `thipster-0.16.5.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:42:36.000000 thipster-0.16.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:42:36.000000 thipster-0.16.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:42:39.701296 thipster-0.16.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-12 08:42:36.000000 thipster-0.16.4/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:42:36.000000 thipster-0.16.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:42:36.000000 thipster-0.16.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:42:39.701296 thipster-0.16.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1490 2023-06-12 08:42:37.000000 thipster-0.16.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3214 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6924 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13387 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19129 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6417 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1688 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.734442 thipster-0.16.5/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-13 13:41:19.000000 thipster-0.16.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-13 13:41:19.000000 thipster-0.16.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-13 13:41:22.734442 thipster-0.16.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-13 13:41:19.000000 thipster-0.16.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-13 13:41:19.000000 thipster-0.16.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-13 13:41:19.000000 thipster-0.16.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 13:41:22.734442 thipster-0.16.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-13 13:41:20.000000 thipster-0.16.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.726442 thipster-0.16.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.730442 thipster-0.16.5/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.730442 thipster-0.16.5/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.730442 thipster-0.16.5/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14904 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4315 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-13 13:41:19.000000 thipster-0.16.5/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.730442 thipster-0.16.5/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.730442 thipster-0.16.5/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.734442 thipster-0.16.5/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.734442 thipster-0.16.5/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.734442 thipster-0.16.5/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10271 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13387 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19129 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.734442 thipster-0.16.5/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.734442 thipster-0.16.5/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18962 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-13 13:41:19.000000 thipster-0.16.5/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 13:41:22.730442 thipster-0.16.5/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-13 13:41:22.000000 thipster-0.16.5/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-06-13 13:41:22.000000 thipster-0.16.5/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 13:41:22.000000 thipster-0.16.5/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-13 13:41:22.000000 thipster-0.16.5/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-13 13:41:22.000000 thipster-0.16.5/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.16.4/LICENSE` & `thipster-0.16.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/PKG-INFO` & `thipster-0.16.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.4
+Version: 0.16.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.16.4/README.md` & `thipster-0.16.5/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/pyproject.toml` & `thipster-0.16.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/tests/engine/test_engine.py` & `thipster-0.16.5/tests/engine/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,16 @@
 
 
 def create_file(filename: str, content: str, dirname: str = 'test'):
     if not os.path.isdir(dirname):
         os.mkdir(dirname)
     dirname = os.path.abspath(dirname)
 
-    file = open(f'{dirname}/{filename}', 'w')
-    file.write(content)
-    file.close()
+    with open(f'{dirname}/{filename}', 'w') as f:
+        f.write(content)
 
 
 def test_engine_calls():
     parser = MockParser()
     repository = MockRepository()
     auth = MockAuth()
     terraform = MockTerraform()
```

### Comparing `thipster-0.16.4/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.16.5/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,39 +8,15 @@
 from thipster.parser.dsl_parser.token import TOKENTYPES as TT
 from thipster.parser.dsl_parser.token_parser import (
     DSLConditionException,
     DSLSyntaxException,
     DSLUnexpectedEOF,
 )
 
-
-def create_dir(dirname: str, files: dict[str, str]):
-    if not os.path.isdir(dirname):
-        os.mkdir(dirname)
-
-    dirname = os.path.abspath(dirname)
-    for name, content in files.items():
-        create_file(name, content, dirname)
-
-    def destroy_files():
-        for content in os.listdir(dirname):
-            os.remove(f'{dirname}/{content}')
-        os.rmdir(dirname)
-
-    return destroy_files
-
-
-def create_file(filename: str, content: str, dirname: str = 'test'):
-    if not os.path.isdir(dirname):
-        os.mkdir(dirname)
-    dirname = os.path.abspath(dirname)
-
-    file = open(f'{dirname}/{filename}', 'w')
-    file.write(content)
-    file.close()
+from ...test_tools import create_dir
 
 
 def test_get_files():
     path_input = 'test'
     _destroy_dir = create_dir(
         path_input,
         {f'test_file{i}.thips': 'content' for i in range(1, 4)},
@@ -568,15 +544,15 @@
 def __test_syntax_error(
     mocker, input: str, ln: int, col: int,
     expected: str, got: str,
 ):
 
     exc_info = __test_parser_raises(mocker, input, DSLSyntaxException)
 
-    exp = str(' or '.join(list(map(lambda x: str(x), expected))))\
+    exp = str(' or '.join(list(map(str, expected))))\
         if isinstance(expected, list) else str(expected.value)
 
     assert str(exc_info.value) == f'(File : \
 {os.getcwd()}/test/test_file.thips, Ln {str(ln)}, Col {str(col)}) :\n\t\
 Syntax error : Expected {exp}, got {str(got.value)}'
```

### Comparing `thipster-0.16.4/tests/parser/dsl_parser/test_ast.py` & `thipster-0.16.5/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.16.5/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/tests/parser/dsl_parser/test_token.py` & `thipster-0.16.5/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.16.5/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/tests/parser/test_ParserFactory.py` & `thipster-0.16.5/tests/parser/test_ParserFactory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,11 @@
-import os
-
 from thipster.engine.parsed_file import ParsedFile
 from thipster.parser import ParserFactory
 
-
-def create_dir(dirname: str, files: dict[str, str]):
-    if not os.path.isdir(dirname):
-        os.mkdir(dirname)
-
-    dirname = os.path.abspath(dirname)
-    for name, content in files.items():
-        create_file(name, content, dirname)
-
-    def destroy_files():
-        for content in os.listdir(dirname):
-            os.remove(f'{dirname}/{content}')
-        os.rmdir(dirname)
-
-    return destroy_files
-
-
-def create_file(filename: str, content: str, dirname: str = 'test'):
-    if not os.path.isdir(dirname):
-        os.mkdir(dirname)
-    dirname = os.path.abspath(dirname)
-
-    file = open(f'{dirname}/{filename}', 'w')
-    file.write(content)
-    file.close()
+from ..test_tools import create_dir
 
 
 def __test_file(files: str):
     path_input = 'test'
     _destroy_dir = create_dir(
         path_input,
         files,
```

### Comparing `thipster-0.16.4/tests/parser/test_YAMLParser.py` & `thipster-0.16.5/tests/parser/test_YAMLParser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,26 @@
-import os
-
 import pytest
 
 import thipster.engine.parsed_file as pf
 from thipster.parser import YAMLParser
 from thipster.parser.yaml_parser import YAMLParserNoName
 
+from ..test_tools import create_dir
+
 
 def __test_parser_raises(mocker, input: str, exception: Exception)\
         -> pytest.ExceptionInfo:
     with pytest.raises(exception) as exc_info:
         __test_file(
             file=input,
         )
 
     return exc_info
 
 
-def create_dir(dirname: str, files: dict[str, str]):
-    if not os.path.isdir(dirname):
-        os.mkdir(dirname)
-
-    dirname = os.path.abspath(dirname)
-    for name, content in files.items():
-        create_file(name, content, dirname)
-
-    def destroy_files():
-        for content in os.listdir(dirname):
-            os.remove(f'{dirname}/{content}')
-        os.rmdir(dirname)
-
-    return destroy_files
-
-
-def create_file(filename: str, content: str, dirname: str = 'test'):
-    if not os.path.isdir(dirname):
-        os.mkdir(dirname)
-    dirname = os.path.abspath(dirname)
-
-    file = open(f'{dirname}/{filename}', 'w')
-    file.write(content)
-    file.close()
-
-
 def __test_file(file: str):
     path_input = 'test'
     _destroy_dir = create_dir(
         path_input,
         {
             'test_file.yaml':
             file,
```

### Comparing `thipster-0.16.4/tests/parser/test_parsedfile.py` & `thipster-0.16.5/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/auth/google.py` & `thipster-0.16.5/thipster/auth/google.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,15 @@
     """Authenticate to Google Cloud Platform (GCP) projects
 
     To use this module, you need to have a GCP account and a project created.
     You also need to have gcloud installed : https://cloud.google.com/sdk/docs/install
     Then login using glcloud : gcloud auth application-default login
     """
 
-    def __init__(self) -> None:
-        return GoogleAuth
-
-    def authenticate(app):
+    def authenticate(self, app):
         """Generates the google provider block for the Terraform CDK
 
         Parameters
         ----------
         app: Construct
             CDK Construct where the provider is created
```

### Comparing `thipster-0.16.4/thipster/engine/engine.py` & `thipster-0.16.5/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/engine/i_parser.py` & `thipster-0.16.5/thipster/engine/i_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from abc import ABC, abstractmethod
+from abc import ABC, abstractclassmethod
 
 from thipster.engine.parsed_file import ParsedFile
 
 
 class I_Parser(ABC):
     """Parser module interface
     """
-    @abstractmethod
-    def run(self, path: str) -> ParsedFile:
+    @abstractclassmethod
+    def run(cls, path: str) -> ParsedFile:
         """Abstract run method
 
         Parameters
         ----------
         path : str
             The path of the filesor directory to be processed
```

### Comparing `thipster-0.16.4/thipster/engine/i_repository.py` & `thipster-0.16.5/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/engine/i_terraform.py` & `thipster-0.16.5/thipster/engine/i_terraform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from abc import ABC, abstractmethod
+from abc import ABC, abstractclassmethod
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 
+from .i_auth import I_Auth
+
 
 class I_Terraform(ABC):
     """Terraform module interface
     """
-    @abstractmethod
-    def apply(self, plan_file_path: str | None = None):
+    @abstractclassmethod
+    def apply(cls, plan_file_path: str | None = None):
         """Apply generated terraform code
 
         Parameters
         ----------
         plan_file_path : str, optional
             Path to plan file, by default None
 
@@ -20,16 +22,19 @@
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement apply()')
 
-    @abstractmethod
-    def generate(self, file: pf.ParsedFile, models: dict[str, rm.ResourceModel]):
+    @abstractclassmethod
+    def generate(
+        cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
+        _authenticator: I_Auth,
+    ):
         """Generates Terraform code from parsed file and models
 
         Parameters
         ----------
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
         models : dict[str, rm.ResourceModel]
@@ -39,28 +44,28 @@
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement generate()')
 
-    @abstractmethod
-    def init(self):
+    @abstractclassmethod
+    def init(cls):
         """Init Terraform for generated terraform code
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement generate()')
 
-    @abstractmethod
-    def plan(self):
+    @abstractclassmethod
+    def plan(cls):
         """Get plan from generated terraform code
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
```

### Comparing `thipster-0.16.4/thipster/engine/parsed_file.py` & `thipster-0.16.5/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/engine/resource_model.py` & `thipster-0.16.5/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/helpers.py` & `thipster-0.16.5/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/ast.py` & `thipster-0.16.5/thipster/parser/dsl_parser/ast.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         for v in values:
             if isinstance(v, list):
                 self.__value.extend(v)
             else:
                 self.__value.append(v)
 
     def __str__(self) -> str:
-        return f"<STRING-EXPR {' '.join(list(map(lambda x : str(x), self.__value)))}>"
+        return f"<STRING-EXPR {' '.join(list(map(str, self.__value)))}>"
 
     @property
     def values(self) -> list[Node]:
         return self.__value
 
     def accept(self, visitor):
         return visitor.visitStringExpr(self)
@@ -265,15 +265,15 @@
 
 class DictNode(ValueNode):
     def __init__(self, value: list[ParameterNode]) -> None:
         super().__init__()
         self.__value = value
 
     def __str__(self) -> str:
-        return f"<DICT {' '.join(list(map(lambda x : str(x), self.__value)))}>"
+        return f"<DICT {' '.join(list(map(str, self.__value)))}>"
 
     @property
     def value(self):
         return self.__value
 
     def accept(self, visitor):
         return visitor.visitDict(self)
@@ -297,15 +297,15 @@
 
 class ListNode(ValueNode):
     def __init__(self, value: list[ValueNode]) -> None:
         super().__init__()
         self.__value = value
 
     def __str__(self) -> str:
-        return f"<LIST {' '.join(list(map(lambda x : str(x), self.__value)))}>"
+        return f"<LIST {' '.join(list(map(str, self.__value)))}>"
 
     @property
     def value(self):
         return self.__value
 
     def accept(self, visitor):
         return visitor.visitList(self)
@@ -434,15 +434,15 @@
         super().__init__()
         self.__resources = []
 
     def add(self, item: ResourceNode | IfNode | AmountNode) -> None:
         self.__resources.append(item)
 
     def __str__(self) -> str:
-        return '\n'.join(list(map(lambda x: str(x), self.__resources)))
+        return '\n'.join(list(map(str, self.__resources)))
 
     @property
     def resources(self) -> list[ResourceNode]:
         return self.__resources
 
     def accept(self, visitor):
         return visitor.visitFile(self)
```

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.16.5/thipster/parser/dsl_parser/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     @property
     def message(self) -> str:
         if type(self.expected) is TT:
             return f"""{str(self.token.position)} :\n\tSyntax error : Expected \
 {str(self.expected.value)}, got {str(self.token.tokenType)}"""
         else:
             return f"""{str(self.token.position)} :\n\tSyntax error : Expected \
-{str(' or '.join(list(map(lambda x : str(x), self.expected))))}, got {
+{str(' or '.join(list(map(str, self.expected))))}, got {
     str(self.token.tokenType)}"""
 
 
 class DSLConditionException(DSLParserBaseException):
     def __init__(self, token: Token, *args: object) -> None:
         super().__init__(*args)
         self.token = token
```

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.16.5/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/lexer.py` & `thipster-0.16.5/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.16.5/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/parser.py` & `thipster-0.16.5/thipster/parser/dsl_parser/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from .interpreter import Interpreter
 from .lexer import Lexer
 from .token_parser import TokenParser
 
 
 class DSLParser(I_Parser):
 
-    def __getfiles(path: str) -> dict[str, str]:
+    @classmethod
+    def __getfiles(cls, path: str) -> dict[str, str]:
         """Recursively get all files in the requested directory and its sudirectories
         Can be run on a path file aswell
 
         Parameters
         ----------
         path: str
             Path to run this function into
@@ -41,15 +42,16 @@
             with open(path, 'r') as f:
                 files.update({path: f.read()})
 
                 f.close()
 
         return files
 
-    def run(path: str) -> ParsedFile:
+    @classmethod
+    def run(cls, path: str) -> ParsedFile:
         """Run the DSLParser
 
         Parameters
         ----------
         path: str
             Path to run the parser into
```

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/token.py` & `thipster-0.16.5/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.16.5/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/parser/parser_factory.py` & `thipster-0.16.5/thipster/parser/parser_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,48 @@
 from thipster.engine import I_Parser
 from thipster.engine import THipsterException
 from thipster.engine.parsed_file import ParsedFile
 from .dsl_parser import DSLParser
 from .yaml_parser import YAMLParser
 
 
+def _noParser(pathExtension):
+    class noParser():
+        def run(path):
+            raise Exception(f'{pathExtension} files can\'t be parsed')
+
+    return noParser
+
+
 class ParserPathNotFound(THipsterException):
-    def __init__(self, path, *args: object) -> None:
+    def __init__(cls, path, *args: object) -> None:
         super().__init__(*args)
 
-        self.__path = path
+        cls.__path = path
 
     @property
-    def message(self) -> str:
-        return f'Path not found : {self.__path}'
+    def message(cls) -> str:
+        return f'Path not found : {cls.__path}'
 
 
 class ParserFactory(I_Parser):
 
     __parsers = {
         '.yaml': YAMLParser,
         '.yml': YAMLParser,
         '.jinja': YAMLParser,
         '.thips': DSLParser,
     }
 
-    def addParser(parser: I_Parser, extensions: list[str]):
-        ParserFactory.__parsers.update({e: parser for e in extensions})
+    @classmethod
+    def addParser(cls, parser: I_Parser, extensions: list[str]):
+        cls.__parsers.update({e: parser for e in extensions})
 
-    def __getfiles(self, path: str) -> list[str]:
+    @classmethod
+    def __getfiles(cls, path: str) -> list[str]:
         """Recursively get all files names in the requested directory and its\
               sudirectories
         Can be run on a path file aswell
 
         Parameters
         ----------
         path: str
@@ -51,50 +61,45 @@
         if not os.path.exists(path):
             raise ParserPathNotFound(path)
 
         files = []
 
         if os.path.isdir(path):
             for content in os.listdir(path):
-                files += self.__getfiles(f'{path}/{content}')
+                files += cls.__getfiles(f'{path}/{content}')
 
         if os.path.isfile(path):
             return [path]
 
         return files
 
-    def __noParser(self, pathExtension):
-        class noParser():
-            def run(path):
-                raise Exception(f'{pathExtension} files can\'t be parsed')
-
-        return noParser
-
-    def run(self, path: str) -> ParsedFile:
+    @classmethod
+    def run(cls, path: str) -> ParsedFile:
         """Run the ParserFactory
 
         Parameters
         ----------
         path: str
             Path to run the parser into
 
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
-        files = self.__getfiles(path)
+        files = cls.__getfiles(path)
 
         res = ParsedFile()
         for file in files:
-            parsedFile = self.__getParser(file).run(file)
+            parsedFile = cls.__getParser(file).run(file)
             res.resources += parsedFile.resources
 
         return res
 
-    def __getParser(self, path) -> I_Parser:
+    @classmethod
+    def __getParser(cls, path) -> I_Parser:
 
         _, pathExtension = os.path.splitext(path)
 
-        return ParserFactory.__parsers.get(
-            pathExtension, self.__noParser(pathExtension),
+        return cls.__parsers.get(
+            pathExtension, _noParser(pathExtension),
         )
```

### Comparing `thipster-0.16.4/thipster/parser/yaml_parser.py` & `thipster-0.16.5/thipster/parser/yaml_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
     @property
     def message(self) -> str:
         return f'No name for resource : {self.resource}'
 
 
 class YAMLParser(I_Parser):
-
-    def __getfiles(path: str) -> list[str]:
+    @classmethod
+    def __getfiles(cls, path: str) -> list[str]:
         """Recursively get all files names in the requested directory and its\
               sudirectories
         Can be run on a path file aswell
 
         Parameters
         ----------
         path: str
@@ -55,57 +55,62 @@
         if not os.path.exists(path):
             raise YAMLParserPathNotFound(path)
 
         files = []
 
         if os.path.isdir(path):
             for content in os.listdir(path):
-                files += YAMLParser.__getfiles(f'{path}/{content}')
+                files += cls.__getfiles(f'{path}/{content}')
 
         if os.path.isfile(path):
             return [path]
 
         return files
 
-    def run(path: str) -> pf.ParsedFile:
+    @classmethod
+    def run(cls, path: str) -> pf.ParsedFile:
         """Run the YAMLParser
 
         Parameters
         ----------
         path: str
             Path to run the parser into
 
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
         try:
-            files = YAMLParser.__getfiles(path)
+            files = cls.__getfiles(path)
             parsedFile = pf.ParsedFile()
 
             for file in files:
                 filedir, filename = os.path.split(file)
 
-                environment = Environment(loader=FileSystemLoader(filedir))
+                environment = Environment(
+                    loader=FileSystemLoader(filedir),
+                    autoescape=True,
+                )
                 template = environment.get_template(filename)
                 rendered = template.render()
                 content = yaml.safe_load(rendered)
 
-                parsedFile.resources += YAMLParser.__convert(content)
+                parsedFile.resources += cls.__convert(content)
 
             return parsedFile
         except yaml.YAMLError as exc:
             raise exc
         except YAMLParserBaseException as e:
             raise e
         except Exception as e:
             raise e
 
-    def __convert(file: dict) -> list[pf.ParsedResource]:
+    @classmethod
+    def __convert(cls, file: dict) -> list[pf.ParsedResource]:
         """Converts a dictionnary into a list of ParsedResources
 
         Parameters
         ----------
         file: dict
             Dict to convert
 
@@ -122,34 +127,35 @@
                     if 'name' in res:
                         name = res['name']
                         del res['name']
                     else:
                         raise YAMLParserNoName(key)
 
                     resources.append(
-                        YAMLParser.__get_resource(
+                        cls.__get_resource(
                             content=res, resourceType=key, name=name,
                         ),
                     )
             elif type(val) == dict:
                 if 'name' in val:
                     name = val['name']
                     del val['name']
                 else:
                     raise YAMLParserNoName(key)
 
                 resources.append(
-                    YAMLParser.__get_resource(
+                    cls.__get_resource(
                         content=val, resourceType=key, name=name,
                     ),
                 )
 
         return resources
 
-    def __get_resource(content: dict, resourceType: str, name: str)\
+    @classmethod
+    def __get_resource(cls, content: dict, resourceType: str, name: str)\
             -> pf.ParsedResource:
         """Converts a dict in a ParsedResource
 
         Parameters
         ----------
         content: dict
             Dict of attributes of the resource
@@ -162,24 +168,25 @@
         -------
         ParsedResource
             A ParsedResource object with the content of the dict
         """
         attr = []
 
         for key, val in content.items():
-            attr.append(YAMLParser.__get__attr(key, val))
+            attr.append(cls.__get__attr(key, val))
 
         return pf.ParsedResource(
             type=resourceType,
             name=name,
             position=None,
             attributes=attr,
         )
 
-    def __get__attr(name: str, value: object) -> pf.ParsedAttribute:
+    @classmethod
+    def __get__attr(cls, name: str, value: object) -> pf.ParsedAttribute:
         """Converts an object in a ParsedAttribute
 
         Parameters
         ----------
         value: object
             Object to convert
         name: str
@@ -187,27 +194,28 @@
 
         Returns
         -------
         ParsedResource
             A ParsedAttribute object with wanted value type
         """
         if type(value) == dict:
-            val = YAMLParser.__get_dict(value)
+            val = cls.__get_dict(value)
         elif type(value) == list:
-            val = YAMLParser.__get_list(value)
+            val = cls.__get_list(value)
         else:
             val = pf.ParsedLiteral(value)
 
         return pf.ParsedAttribute(
             name=name,
             value=val,
             position=None,
         )
 
-    def __get_dict(input: dict) -> pf.ParsedDict:
+    @classmethod
+    def __get_dict(cls, input: dict) -> pf.ParsedDict:
         """Converts a dict into a list of ParsedDict
 
         Parameters
         ----------
         input: dict
             Dict to convert
 
@@ -215,19 +223,20 @@
         -------
         ParsedDict
             Converted dict
         """
         attr = []
 
         for key, val in input.items():
-            attr.append(YAMLParser.__get__attr(key, val))
+            attr.append(cls.__get__attr(key, val))
 
         return pf.ParsedDict(attr)
 
-    def __get_list(input: list) -> pf.ParsedList:
+    @classmethod
+    def __get_list(cls, input: list) -> pf.ParsedList:
         """Converts a dictionnary into a ParsedList
 
         Parameters
         ----------
         input: list
             List to convert
 
@@ -236,12 +245,12 @@
         ParsedList
             Converted list
         """
         attr = []
 
         for val in input:
             if isinstance(val, dict):
-                attr.append(YAMLParser.__get_dict(val))
+                attr.append(cls.__get_dict(val))
             else:
                 attr.append(pf.ParsedLiteral(val))
 
         return pf.ParsedList(attr)
```

### Comparing `thipster-0.16.4/thipster/repository/github.py` & `thipster-0.16.5/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/repository/json.py` & `thipster-0.16.5/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster/terraform/cdk.py` & `thipster-0.16.5/thipster/terraform/cdk.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     _models = []
     _parent_resources_stack = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = Logger(__name__)
 
-    def apply(self, plan_file_path: str | None = None):
+    @classmethod
+    def apply(cls, plan_file_path: str | None = None):
         """Applies generated Terraform plan
 
         Parameters
         ----------
         plan_file_path : str, optional
             path to the plan file, default None
 
@@ -38,121 +39,129 @@
         str
             Terraform apply output
         """
         t = Terraform()
         _, stdout, stderr = t.apply(plan_file_path)
         return stdout + stderr
 
+    @classmethod
     def generate(
-        self, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
-        _auth: I_Auth,
+        cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
+        _authenticator: I_Auth,
     ):
         """Generate Terraform file from given parsed file and models
 
         Parameters
         ----------
         file : pf.ParsedFile
             parsedFile object to transform
         models : dict[str, rm.ResourceModel]
             associated models
         _auth : I_Auth
             authenticator to use
         """
-        CDK._created_resources = {}
-        CDK._models = models
-        CDK._parent_resources_stack = []
+        cls._created_resources = {}
+        cls._models = models
+        cls._parent_resources_stack = []
 
         # Init CDK
         app = App()
 
         f_position = file.resources[0].position
         file_name = f_position.fileName if f_position else 'thipster_infrastructure'
 
-        CDK._logger.debug('Creating tf code for file %s', file_name)
+        cls._logger.debug('Creating tf code for file %s', file_name)
 
         # Declare new stack in CDK
         class _ResourceStack(TerraformStack):
             def __init__(self, scope: Construct, ns: str):
                 super().__init__(scope, ns)
 
-                _auth.authenticate(self)
+                _authenticator.authenticate(self)
 
                 for resource in file.resources:
-                    res = CDK._create_resource_from_resource(
+                    res = _create_resource_from_resource(
                         self,
                         resource=resource,
                     )
 
-                    CDK._created_resources[f'{resource.type}/{resource.name}'] = res.id
+                    cls._created_resources[f'{resource.type}/{resource.name}'] = res.id
 
         _ResourceStack(app, file_name)
 
         # Synth files
         app.synth()
 
-        self.__dirs = [
+        output_directories = [
             f'{app.outdir}/stacks/{c.node.path}' for c in app.node.children
         ]
 
-        CDK._logger.info('Created %s terraform file(s)', len(self.__dirs))
+        CDK._logger.info(
+            'Created %s terraform file(s)',
+            len(output_directories),
+        )
 
         # Move files
-        for dirname in self.__dirs:
+        for dirname in output_directories:
             shutil.move(
                 os.path.join(os.getcwd(), dirname, 'cdk.tf.json'),
                 os.path.join(os.getcwd(), 'thipster.tf.json'),
             )
 
         # Delete cdktf.out directory
             for content in os.listdir(os.path.join(os.getcwd(), dirname)):
                 os.remove(f'{dirname}/{content}')
             os.rmdir(dirname)
         for content in os.listdir(os.path.join(os.getcwd(), 'cdktf.out')):
             d = f'cdktf.out/{content}'
             os.rmdir(d) if os.path.isdir(d) else os.remove(d)
         os.rmdir('cdktf.out')
 
-    def init(self):
+    @classmethod
+    def init(cls):
         """Initilize terraform
 
         Returns
         -------
         str
             Terraform init output
         """
         t = Terraform()
         _, stdout, stderr = t.init()
         return stdout + stderr
 
-    def plan(self):
+    @classmethod
+    def plan(cls):
         """Get plan from generated terraform code
 
         Returns
         -------
         str
             Terraform plan output
         """
         t = Terraform()
         _, stdout, stderr = t.plan(out='thipster.tfplan')
         return stdout + stderr
 
-    def _pip_install(package: str):
+    @classmethod
+    def _pip_install(cls, package: str):
         """Install a package if it wasn't already installed by thipster
 
         Parameters
         ----------
         package : str
             package to install
         """
         if package not in sys.modules:
             subprocess.check_call(
                 [sys.executable, '-m', 'pip', 'install', '-qqq', package],
             )
 
-    def _import(package_name: str, module_name: str, class_name: str) -> type:
+    @classmethod
+    def _import(cls, package_name: str, module_name: str, class_name: str) -> type:
         """Import a class from any package
 
         Parameters
         ----------
         package_name : str
             package that contains the class
         module_name : str
@@ -166,464 +175,474 @@
             the imported class
         """
         module = importlib.import_module(f'{package_name}.{module_name}')
         class_ = getattr(module, class_name)
 
         return class_
 
-    def _create_default_resource(
-        self, resource_type: str, parent_name: str | None = None,
-        no_modif: bool = True, no_dependencies: bool = False,
-    ):
-        """Create a resource with all default values
 
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        resource_type : str
-            type of the resource to create
-        parent_name : str, optional
-            name of its parent, default None
-        no_modif : bool, optional
-            if True, raise errors if resource can't be created with default values, \
+def _create_default_resource(
+    resource_self, resource_type: str, parent_name: str | None = None,
+    no_modif: bool = True, no_dependencies: bool = False,
+):
+    """Create a resource with all default values
+
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    resource_type : str
+        type of the resource to create
+    parent_name : str, optional
+        name of its parent, default None
+    no_modif : bool, optional
+        if True, raise errors if resource can't be created with default values, \
 default False
-        no_dependencies : bool, optional
-            if True, create the default dependencies, default False
-
-        Returns
-        -------
-        (type, str, dict[str, object]) :
-            all the information needed to instantiate the class with default values
-        """
-        # Checks for cyclic dependency
-        if resource_type in CDK._parent_resources_stack:
-            CDK._logger.error(
-                '%s already present in parent Stack', resource_type,
-            )
-            raise cdk_exceptions.CDKCyclicDependencies(
-                CDK._parent_resources_stack,
-            )
-
-        CDK._parent_resources_stack.append(resource_type)
-
-        model = CDK._models[resource_type]
-
-        attributes = copy.deepcopy(model.attributes)
+    no_dependencies : bool, optional
+        if True, create the default dependencies, default False
 
-        for a in CDK._inherited_attributes:
-            if a.name in attributes.keys():
-                attributes[a.name].default = rm.Model_Literal(a.value)
+    Returns
+    -------
+    (type, str, dict[str, object]) :
+        all the information needed to instantiate the class with default values
+    """
+    # Checks for cyclic dependency
+    if resource_type in CDK._parent_resources_stack:
+        CDK._logger.error(
+            '%s already present in parent Stack', resource_type,
+        )
+        raise cdk_exceptions.CDKCyclicDependencies(
+            CDK._parent_resources_stack,
+        )
 
-            else:
-                attributes[a.name] = rm.Model_Attribute(
-                    cdk_name=a.name,
-                    default=rm.Model_Literal(a.value),
-                )
+    CDK._parent_resources_stack.append(resource_type)
 
-        # Checks that all attributes have a default value
-        if (
-            no_modif
-            and not all(map(lambda x: x.default is not None, attributes.values()))
-        ):
-            raise cdk_exceptions.CDKMissingAttributeInDependency(resource_type)
-
-        # Import package and class
-        CDK._pip_install(model.cdk_provider)
-        resource_class = CDK._import(
-            model.cdk_provider, model.cdk_module, model.cdk_name,
-        )
-
-        # Process name + default values
-        dependencies = copy.deepcopy(model.dependencies)
-        resource_args = {}
-
-        name = f'{parent_name}-{uuid.uuid4()}'
-        if model.name_key:
-            resource_args[model.name_key] = name
-
-        for attribute_name, attribute_value in attributes.items():
-
-            if not no_dependencies and attribute_name in dependencies:
-
-                CDK._check_explicit_dependency(
-                    self, resource_args, dependencies[attribute_name]['resource'],
-                    attribute_value.default, attribute_name,
-                )
+    model = CDK._models[resource_type]
 
-                del dependencies[attribute_name]
+    attributes = copy.deepcopy(model.attributes)
 
-            if attribute_name in model.attributes:
-                resource_args[attribute_value.cdk_name] = attribute_value.default
+    for a in CDK._inherited_attributes:
+        if a.name in attributes.keys():
+            attributes[a.name].default = rm.Model_Literal(a.value)
 
-        # Create default defendencies if needed
-        if not no_dependencies:
-            CDK._generate_default_dependencies(
-                self, dependencies, model, resource_args, parent_name,
+        else:
+            attributes[a.name] = rm.Model_Attribute(
+                cdk_name=a.name,
+                default=rm.Model_Literal(a.value),
             )
 
-        CDK._logger.debug('Created default %s named %s', resource_class, name)
-
-        return (resource_class, name, resource_args)
-
-    def _create_resource(self, resource_args: object, resource_type: str = None):
-        """Create a resource with the given values
-
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        resource_args : object
-            data source to create the resource
-        resource_type : str, optional
-            type of the resource to create, default None
-
-        Returns
-        -------
-        object :
-            the created resource
-        """
-
-        if isinstance(resource_args, pf.ParsedResource):
-            return CDK._create_resource_from_resource(self, resource_args)
-
-        return CDK._create_resource_from_args(self, resource_type, resource_args)
-
-    def _create_resource_from_args(
-        self, resource_type: str, input_args: list[pf.ParsedAttribute] | None,
+    # Checks that all attributes have a default value
+    if (
+        no_modif
+        and not all(map(lambda x: x.default is not None, attributes.values()))
     ):
-        """Create a resource from a list of ParsedAttributes
+        raise cdk_exceptions.CDKMissingAttributeInDependency(resource_type)
 
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        resource_type : str, optional
-            type of the resource to create, default None
-        input_args : list[ParsedAttribute]
-            data source to create the resource
+    # Import package and class
+    CDK._pip_install(model.cdk_provider)
+    resource_class = CDK._import(
+        model.cdk_provider, model.cdk_module, model.cdk_name,
+    )
 
-        Returns
-        -------
-        object :
-            the created resource
-        """
-        resource_class, resource_name, resource_args = CDK._create_default_resource(
-            self,
-            resource_type,
-            no_modif=False,
-            no_dependencies=True,
-        )
-        model = CDK._models[resource_type]
-
-        # Process attributes
-        dependencies = copy.deepcopy(model.dependencies)
-
-        def attributes(attribute_list):
-            for attribute in attribute_list:
-                if attribute.name and model.name_key:
-                    resource_args[model.name_key] = attribute.name
+    # Process name + default values
+    dependencies = copy.deepcopy(model.dependencies)
+    resource_args = {}
 
-                CDK._process_attribute(
-                    self, model, attribute, resource_args, dependencies,
-                )
+    name = f'{parent_name}-{uuid.uuid4()}'
+    if model.name_key:
+        resource_args[model.name_key] = name
+
+    for attribute_name, attribute_value in attributes.items():
 
-        attributes(input_args)
-        attributes(CDK._inherited_attributes)
+        if not no_dependencies and attribute_name in dependencies:
 
-        CDK._inherited_attributes += input_args
-        CDK._generate_default_dependencies(
-            self, dependencies, model, resource_args, resource_name,
-        )
-        CDK._inherited_attributes = CDK._inherited_attributes[
-            :-len(
-                input_args,
+            _check_explicit_dependency(
+                resource_self, resource_args, dependencies[attribute_name]['resource'],
+                attribute_value.default, attribute_name,
             )
-        ]
 
-        # Create resource
-        CDK._parent_resources_stack.remove(resource_type)
+            del dependencies[attribute_name]
+
+        if attribute_name in model.attributes:
+            resource_args[attribute_value.cdk_name] = attribute_value.default
 
-        CDK._logger.debug(
-            'Created default %s named %s',
-            resource_class, resource_name,
-        )
-
-        if not model.name_key:
-            return resource_class(**resource_args)
-        return resource_class(self, resource_name, **resource_args)
-
-    def _create_resource_from_resource(self, resource: pf.ParsedResource):
-        # Create resource with default values
-        resource_class, _, resource_args = CDK._create_default_resource(
-            self,
-            resource.type,
-            no_modif=False,
-            no_dependencies=True,
+    # Create default defendencies if needed
+    if not no_dependencies:
+        _generate_default_dependencies(
+            resource_self, dependencies, model, resource_args, parent_name,
         )
-        """Create a resource from a list of ParsedAttributes
 
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        resource : ParsedResource
-            data source to create the resource
+    CDK._logger.debug('Created default %s named %s', resource_class, name)
 
-        Returns
-        -------
-        object :
-            the created resource
-        """
-        model = CDK._models[resource.type]
+    return (resource_class, name, resource_args)
 
-        if model.name_key:
-            resource_args[model.name_key] = resource.name
 
-        # Process attributes
-        dependencies = copy.deepcopy(model.dependencies)
+def _create_resource(resource_self, resource_args: object, resource_type: str = None):
+    """Create a resource with the given values
 
-        def attributes(attribute_list):
-            for attribute in attribute_list:
-                CDK._process_attribute(
-                    self,
-                    model,
-                    attribute,
-                    resource_args,
-                    dependencies,
-                )
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    resource_args : object
+        data source to create the resource
+    resource_type : str, optional
+        type of the resource to create, default None
+
+    Returns
+    -------
+    object :
+        the created resource
+    """
+
+    if isinstance(resource_args, pf.ParsedResource):
+        return _create_resource_from_resource(resource_self, resource_args)
+
+    return _create_resource_from_args(resource_self, resource_type, resource_args)
+
+
+def _create_resource_from_args(
+    resource_self, resource_type: str, input_args: list[pf.ParsedAttribute] | None,
+):
+    """Create a resource from a list of ParsedAttributes
+
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    resource_type : str, optional
+        type of the resource to create, default None
+    input_args : list[ParsedAttribute]
+        data source to create the resource
+
+    Returns
+    -------
+    object :
+        the created resource
+    """
+    resource_class, resource_name, resource_args = _create_default_resource(
+        resource_self,
+        resource_type,
+        no_modif=False,
+        no_dependencies=True,
+    )
+    model = CDK._models[resource_type]
+
+    # Process attributes
+    dependencies = copy.deepcopy(model.dependencies)
+
+    def attributes(attribute_list):
+        for attribute in attribute_list:
+            if attribute.name and model.name_key:
+                resource_args[model.name_key] = attribute.name
+
+            _process_attribute(
+                resource_self, model, attribute, resource_args, dependencies,
+            )
+
+    attributes(input_args)
+    attributes(CDK._inherited_attributes)
+
+    CDK._inherited_attributes += input_args
+    _generate_default_dependencies(
+        resource_self, dependencies, model, resource_args, resource_name,
+    )
+    CDK._inherited_attributes = CDK._inherited_attributes[
+        :-len(
+            input_args,
+        )
+    ]
 
-        attributes(resource.attributes)
-        attributes(CDK._inherited_attributes)
+    # Create resource
+    CDK._parent_resources_stack.remove(resource_type)
 
-        CDK._inherited_attributes += resource.attributes
-        CDK._generate_default_dependencies(
-            self, dependencies, model, resource_args, resource.name,
-        )
-        CDK._inherited_attributes = CDK._inherited_attributes[
-            :-len(
-                resource.attributes,
+    CDK._logger.debug(
+        'Created default %s named %s',
+        resource_class, resource_name,
+    )
+
+    if not model.name_key:
+        return resource_class(**resource_args)
+    return resource_class(resource_self, resource_name, **resource_args)
+
+
+def _create_resource_from_resource(resource_self, resource: pf.ParsedResource):
+    # Create resource with default values
+    resource_class, _, resource_args = _create_default_resource(
+        resource_self,
+        resource.type,
+        no_modif=False,
+        no_dependencies=True,
+    )
+    """Create a resource from a list of ParsedAttributes
+
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    resource : ParsedResource
+        data source to create the resource
+
+    Returns
+    -------
+    object :
+        the created resource
+    """
+    model = CDK._models[resource.type]
+
+    if model.name_key:
+        resource_args[model.name_key] = resource.name
+
+    # Process attributes
+    dependencies = copy.deepcopy(model.dependencies)
+
+    def attributes(attribute_list):
+        for attribute in attribute_list:
+            _process_attribute(
+                resource_self,
+                model,
+                attribute,
+                resource_args,
+                dependencies,
             )
-        ]
 
-        # Create resource
-        CDK._parent_resources_stack.remove(resource.type)
+    attributes(resource.attributes)
+    attributes(CDK._inherited_attributes)
 
-        CDK._logger.debug(
-            'Created resource %s named %s',
-            resource_class, resource.name,
+    CDK._inherited_attributes += resource.attributes
+    _generate_default_dependencies(
+        resource_self, dependencies, model, resource_args, resource.name,
+    )
+    CDK._inherited_attributes = CDK._inherited_attributes[
+        :-len(
+            resource.attributes,
         )
+    ]
 
-        return resource_class(self, resource.name, **resource_args)
-
-    def _process_attribute(
-        self,
-        model: rm.ResourceModel,
-        attribute: pf.ParsedAttribute,
-        resource_args: dict[str, object],
-        dependencies: dict[str, dict[str, object]] | None,
-    ):
-        """Process an attribute
-
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        model : ResourceModel
-            model of the resource that is being created
-        attribute : ParsedAttribute
-            attribute to handle
-        resource_args : object
-            data source needed to create the resource
-        dependencies : dict[str, dict[str, object]]
-            dependencies needed to create the resource
-        """
-        if attribute.name in dependencies:
-            CDK._check_explicit_dependency(
-                self, resource_args, dependencies[attribute.name]['resource'],
-                attribute.value, attribute.name,
-            )
-            del dependencies[attribute.name]
-            return
+    # Create resource
+    CDK._parent_resources_stack.remove(resource.type)
 
-        # Checks if attribute is an internal object
-        if attribute.name in model.internal_objects:
-            resource_args = CDK._create_internal_object(
-                self,
-                attribute.name,
-                model.internal_objects[attribute.name],
-                attribute.value,
-                resource_args,
-            )
-            return
-
-        # Checks if attribute is expected as an attibute
-        if attribute.name not in model.attributes:
-            return
+    CDK._logger.debug(
+        'Created resource %s named %s',
+        resource_class, resource.name,
+    )
+
+    return resource_class(resource_self, resource.name, **resource_args)
+
+
+def _process_attribute(
+    resource_self,
+    model: rm.ResourceModel,
+    attribute: pf.ParsedAttribute,
+    resource_args: dict[str, object],
+    dependencies: dict[str, dict[str, object]] | None,
+):
+    """Process an attribute
+
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    model : ResourceModel
+        model of the resource that is being created
+    attribute : ParsedAttribute
+        attribute to handle
+    resource_args : object
+        data source needed to create the resource
+    dependencies : dict[str, dict[str, object]]
+        dependencies needed to create the resource
+    """
+    if attribute.name in dependencies:
+        _check_explicit_dependency(
+            resource_self, resource_args, dependencies[attribute.name]['resource'],
+            attribute.value, attribute.name,
+        )
+        del dependencies[attribute.name]
+        return
 
-        # Processes list attribute
-        attribute_value = attribute.value
-        if model.attributes[attribute.name].is_list:
-            if type(attribute.value) is list:
-                attribute_value = [i.value for i in attribute.value]
-            else:
-                attribute_value = [attribute.value]
-
-        # Sets attribute value
-        resource_args[model.attributes[attribute.name].cdk_name] = attribute_value
-
-    def _generate_default_dependencies(
-            self,
-            dependencies,
-            model: rm.ResourceModel,
+    # Checks if attribute is an internal object
+    if attribute.name in model.internal_objects:
+        _create_internal_object(
+            resource_self,
+            attribute.name,
+            model.internal_objects[attribute.name],
+            attribute.value,
             resource_args,
-            resource_name,
-    ):
-        """Generate default dependencies and internal objects in a resource
-
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        dependencies :
-            list of dependencies to create
-        model : str
-            model of the resource that is being created
-        resource_args : _type_
-            data source needed to create the resource
-        resource_name : dict
-            name of the resource that is being created
-        """
-        # Create missing dependencies
-        for dependency_name, dependency_object in dependencies.items():
-            CDK._create_dependency(
-                self, dependency_name, dependency_object, resource_args, resource_name,
-            )
+        )
+        return
 
-        # Create default internal objects if needed
-        for internal_object_name, internal_object in model.internal_objects.items():
-            if internal_object_name not in resource_args:
-                for default_args_json in internal_object['defaults']:
-
-                    # Transform in list of ParsedAttributes
-                    default_args = []
-                    for arg_key, arg_value in default_args_json.items():
-                        default_args.append(
-                            pf.ParsedAttribute(
-                                arg_key, None, pf.ParsedLiteral(arg_value),
-                            ),
-                        )
+    # Checks if attribute is expected as an attibute
+    if attribute.name not in model.attributes:
+        return
 
-                    CDK._create_internal_object(
-                        self,
-                        internal_object_name,
-                        model.internal_objects[internal_object_name],
-                        default_args,
-                        resource_args,
-                    )
+    # Processes list attribute
+    attribute_value = attribute.value
+    if model.attributes[attribute.name].is_list:
+        if type(attribute.value) is list:
+            attribute_value = [i.value for i in attribute.value]
+        else:
+            attribute_value = [attribute.value]
+
+    # Sets attribute value
+    resource_args[model.attributes[attribute.name].cdk_name] = attribute_value
 
-    def _create_internal_object(
-        self,
-        name: str,
-        internal_object_model,
-        internal_object_args,
-        resource_args: dict,
-    ):
-        """Create an internal object in a resource
 
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        name : str
-            name of the internal object
-        internal_object_model : ResourceModel
-            model of the internal object
-        internal_object_args : object
-            data source to create the internal object
-        resource_args : dict
-            data source needed to create the resource
-        """
-        internal_object_type = internal_object_model['var_type'] \
-            if 'var_type' in internal_object_model else 'Unknown'
+def _generate_default_dependencies(
+        resource_self,
+        dependencies,
+        model: rm.ResourceModel,
+        resource_args,
+        resource_name,
+):
+    """Generate default dependencies and internal objects in a resource
+
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    dependencies :
+        list of dependencies to create
+    model : str
+        model of the resource that is being created
+    resource_args : _type_
+        data source needed to create the resource
+    resource_name : dict
+        name of the resource that is being created
+    """
+    # Create missing dependencies
+    for dependency_name, dependency_object in dependencies.items():
+        _create_dependency(
+            resource_self, dependency_name,
+            dependency_object, resource_args, resource_name,
+        )
 
-        if internal_object_type.startswith('list'):
-            if name not in resource_args:
-                resource_args[name] = []
+    # Create default internal objects if needed
+    for internal_object_name, internal_object in model.internal_objects.items():
+        if internal_object_name not in resource_args:
+            for default_args_json in internal_object['defaults']:
+
+                # Transform in list of ParsedAttributes
+                default_args = []
+                for arg_key, arg_value in default_args_json.items():
+                    default_args.append(
+                        pf.ParsedAttribute(
+                            arg_key, None, pf.ParsedLiteral(arg_value),
+                        ),
+                    )
 
-            if isinstance(internal_object_args, list) \
-                    and isinstance(internal_object_args[0], pf.ParsedDict):
+                _create_internal_object(
+                    resource_self,
+                    internal_object_name,
+                    model.internal_objects[internal_object_name],
+                    default_args,
+                    resource_args,
+                )
 
-                for internalObject in internal_object_args:
-                    res = CDK._create_resource(
-                        self,
-                        internalObject.value,
-                        internal_object_model['resource'],
-                    )
-                    resource_args[name] += [res]
 
-                return
+def _create_internal_object(
+    resource_self,
+    name: str,
+    internal_object_model,
+    internal_object_args,
+    resource_args: dict,
+):
+    """Create an internal object in a resource
+
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    name : str
+        name of the internal object
+    internal_object_model : ResourceModel
+        model of the internal object
+    internal_object_args : object
+        data source to create the internal object
+    resource_args : dict
+        data source needed to create the resource
+    """
+    internal_object_type = internal_object_model['var_type'] \
+        if 'var_type' in internal_object_model else 'Unknown'
+
+    if internal_object_type.startswith('list'):
+        if name not in resource_args:
+            resource_args[name] = []
+
+        if isinstance(internal_object_args, list) \
+                and isinstance(internal_object_args[0], pf.ParsedDict):
+
+            for internalObject in internal_object_args:
+                res = _create_resource(
+                    resource_self,
+                    internalObject.value,
+                    internal_object_model['resource'],
+                )
+                resource_args[name] += [res]
 
-            res = CDK._create_resource(
-                self,
-                internal_object_args,
-                internal_object_model['resource'],
-            )
-            resource_args[name] += [res]
             return
 
-        res = CDK._create_resource(
-            self,
+        res = _create_resource(
+            resource_self,
             internal_object_args,
             internal_object_model['resource'],
         )
-        resource_args[name] = res
-
+        resource_args[name] += [res]
         return
 
-    def _create_dependency(self, dep_name, dep_value, resource_args, parent_name):
-        """Create an internal object in a resource
-
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        dep_name : str
-            name of the dependency
-        dep_value : ResourceModel
-            model of the dependency
-        resource_args : dict
-            data source needed to create the resource
-        parent_name : str
-            name of its parent
-        """
-        class_, class_name, class_attributes = CDK._create_default_resource(
-            self, dep_value['resource'], parent_name,
+    res = _create_resource(
+        resource_self,
+        internal_object_args,
+        internal_object_model['resource'],
+    )
+    resource_args[name] = res
+
+    return
+
+
+def _create_dependency(resource_self, dep_name, dep_value, resource_args, parent_name):
+    """Create an internal object in a resource
+
+    Parameters
+    ----------
+    self : _ResourceStack
+        Terraform CDK stack that contains the resource
+    dep_name : str
+        name of the dependency
+    dep_value : ResourceModel
+        model of the dependency
+    resource_args : dict
+        data source needed to create the resource
+    parent_name : str
+        name of its parent
+    """
+    class_, class_name, class_attributes = _create_default_resource(
+        resource_self, dep_value['resource'], parent_name,
+    )
+
+    id = class_(resource_self, class_name, **class_attributes).id
+    if dep_name:
+        resource_args[dep_name] = id
+
+    CDK._parent_resources_stack.remove(dep_value['resource'])
+
+
+def _check_explicit_dependency(
+    resource_self, resource_args, dependency_type, dependency_value, attribute_name,
+):
+    created_name = f'{dependency_type}/'\
+        f'{dependency_value}'
+
+    # Checks if attribute is an explicit dependency
+    if created_name not in CDK._created_resources.keys():
+
+        if isinstance(dependency_value, str):
+            raise cdk_exceptions.CDKDependencyNotDeclared(
+                attribute_name, dependency_value,
+            )
+
+        # Creates explicit dependency
+        _create_dependency(
+            resource_self, attribute_name, dependency_value,
+            resource_args, attribute_name,
         )
 
-        id = class_(self, class_name, **class_attributes).id
-        if dep_name:
-            resource_args[dep_name] = id
-
-        CDK._parent_resources_stack.remove(dep_value['resource'])
-
-    def _check_explicit_dependency(
-        self, resource_args, dependency_type, dependency_value, attribute_name,
-    ):
-        created_name = f'{dependency_type}/'\
-            f'{dependency_value}'
-
-        # Checks if attribute is an explicit dependency
-        if created_name not in CDK._created_resources.keys():
-
-            if isinstance(dependency_value, str):
-                raise cdk_exceptions.CDKDependencyNotDeclared(
-                    attribute_name, dependency_value,
-                )
-
-            # Creates explicit dependency
-            CDK._create_dependency(
-                self, attribute_name, dependency_value,
-                resource_args, attribute_name,
-            )
-
-        resource_args[attribute_name] = CDK._created_resources[created_name]
+    resource_args[attribute_name] = CDK._created_resources[created_name]
```

### Comparing `thipster-0.16.4/thipster/terraform/exceptions.py` & `thipster-0.16.5/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.4/thipster.egg-info/PKG-INFO` & `thipster-0.16.5/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.4
+Version: 0.16.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.16.4/thipster.egg-info/SOURCES.txt` & `thipster-0.16.5/thipster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 tests/__init__.py
 tests/test_e2e.py
+tests/test_tools.py
 tests/engine/__init__.py
 tests/engine/test_engine.py
+tests/engine/test_generation.py
 tests/parser/__init__.py
 tests/parser/test_ParserFactory.py
 tests/parser/test_YAMLParser.py
 tests/parser/test_parsedfile.py
 tests/parser/dsl_parser/__init__.py
 tests/parser/dsl_parser/test_DSLparser.py
 tests/parser/dsl_parser/test_ast.py
```

