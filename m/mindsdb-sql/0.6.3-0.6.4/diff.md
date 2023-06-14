# Comparing `tmp/mindsdb_sql-0.6.3.tar.gz` & `tmp/mindsdb_sql-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.6.3.tar", last modified: Thu Jun  8 19:18:28 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.6.4.tar", last modified: Wed Jun 14 12:56:56 2023, max compression
```

## Comparing `mindsdb_sql-0.6.3.tar` & `mindsdb_sql-0.6.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/
--rw-rw-rw-   0        0        0      535 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     7245 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1195 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1343 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     2287 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3260 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      567 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1593 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0     3136 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     2407 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      769 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1818 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
--rw-rw-rw-   0        0        0     1595 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2078 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1201 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     5361 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1534 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      704 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      713 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      737 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
--rw-rw-rw-   0        0        0      692 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      708 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0     1313 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
--rw-rw-rw-   0        0        0      223 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0      359 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8140 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    44911 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29491 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6226 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21382 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    50304 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21344 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8276 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    13228 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    20561 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5282 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/__init__.py
--rw-rw-rw-   0        0        0      776 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ast.py
--rw-rw-rw-   0        0        0    11910 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_base_lexer.py
--rw-rw-rw-   0        0        0      223 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_base_sql.py
--rw-rw-rw-   0        0        0     1480 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_create.py
--rw-rw-rw-   0        0        0     2481 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ddl.py
--rw-rw-rw-   0        0        0     1075 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_delete.py
--rw-rw-rw-   0        0        0     1094 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_describe.py
--rw-rw-rw-   0        0        0     2426 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_insert.py
--rw-rw-rw-   0        0        0     6945 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_misc_sql_queries.py
--rw-rw-rw-   0        0        0     3625 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_common_table_expression.py
--rw-rw-rw-   0        0        0    24799 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_operations.py
--rw-rw-rw-   0        0        0    45563 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_structure.py
--rw-rw-rw-   0        0        0    13620 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_show.py
--rw-rw-rw-   0        0        0     3114 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_union.py
--rw-rw-rw-   0        0        0     2462 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_update.py
--rw-rw-rw-   0        0        0      514 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_use.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_chatbots.py
--rw-rw-rw-   0        0        0      605 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_file.py
--rw-rw-rw-   0        0        0     4203 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_integration.py
--rw-rw-rw-   0        0        0     6617 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_predictor.py
--rw-rw-rw-   0        0        0     2651 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_view.py
--rw-rw-rw-   0        0        0      520 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_dataset.py
--rw-rw-rw-   0        0        0      861 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_datasource.py
--rw-rw-rw-   0        0        0      866 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_integration.py
--rw-rw-rw-   0        0        0     1708 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_predictor.py
--rw-rw-rw-   0        0        0     1824 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_evaluate.py
--rw-rw-rw-   0        0        0     1339 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_finetune_predictor.py
--rw-rw-rw-   0        0        0     2056 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_jobs.py
--rw-rw-rw-   0        0        0     1587 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_ml_engine.py
--rw-rw-rw-   0        0        0     2242 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_retrain_predictor.py
--rw-rw-rw-   0        0        0     3572 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_selects.py
--rw-rw-rw-   0        0        0     1226 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_show_mindsdb.py
--rw-rw-rw-   0        0        0      959 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_timeseries.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/__init__.py
--rw-rw-rw-   0        0        0      714 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_lexer.py
--rw-rw-rw-   0        0        0     3050 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_render/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_render/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_render/test_sqlalchemyrender.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/
+-rw-rw-rw-   0        0        0      535 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7245 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1195 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1343 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     2287 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3260 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      567 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1593 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0     3196 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     2407 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      769 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
+-rw-rw-rw-   0        0        0     1595 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2078 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1201 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     5361 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1534 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      704 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      713 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      737 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
+-rw-rw-rw-   0        0        0      692 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      708 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0      359 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8140 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    44911 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29491 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6226 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21382 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    51397 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21394 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8517 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    13228 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    20561 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-06-14 12:56:55.000000 mindsdb_sql-0.6.4/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5282 2023-06-14 12:56:55.000000 mindsdb_sql-0.6.4/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 12:56:55.000000 mindsdb_sql-0.6.4/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-14 12:56:55.000000 mindsdb_sql-0.6.4/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-14 12:56:55.000000 mindsdb_sql-0.6.4/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      843 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/tests/test_parser/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/__init__.py
+-rw-rw-rw-   0        0        0      776 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_ast.py
+-rw-rw-rw-   0        0        0    11910 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_base_lexer.py
+-rw-rw-rw-   0        0        0      223 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_base_sql.py
+-rw-rw-rw-   0        0        0     1480 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_create.py
+-rw-rw-rw-   0        0        0     2481 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_ddl.py
+-rw-rw-rw-   0        0        0     1075 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_delete.py
+-rw-rw-rw-   0        0        0     1094 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_describe.py
+-rw-rw-rw-   0        0        0     2426 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_insert.py
+-rw-rw-rw-   0        0        0     6945 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_misc_sql_queries.py
+-rw-rw-rw-   0        0        0     3625 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_select_common_table_expression.py
+-rw-rw-rw-   0        0        0    24799 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_select_operations.py
+-rw-rw-rw-   0        0        0    45563 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_select_structure.py
+-rw-rw-rw-   0        0        0    13620 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_show.py
+-rw-rw-rw-   0        0        0     3114 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_union.py
+-rw-rw-rw-   0        0        0     2462 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_update.py
+-rw-rw-rw-   0        0        0      514 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_use.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_chatbots.py
+-rw-rw-rw-   0        0        0      605 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_file.py
+-rw-rw-rw-   0        0        0     4203 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_integration.py
+-rw-rw-rw-   0        0        0     6617 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_predictor.py
+-rw-rw-rw-   0        0        0     2651 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_view.py
+-rw-rw-rw-   0        0        0      520 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_dataset.py
+-rw-rw-rw-   0        0        0      861 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_datasource.py
+-rw-rw-rw-   0        0        0      866 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_integration.py
+-rw-rw-rw-   0        0        0     1708 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_predictor.py
+-rw-rw-rw-   0        0        0     1824 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_evaluate.py
+-rw-rw-rw-   0        0        0     1339 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_finetune_predictor.py
+-rw-rw-rw-   0        0        0     2056 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_jobs.py
+-rw-rw-rw-   0        0        0     1587 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_ml_engine.py
+-rw-rw-rw-   0        0        0     2242 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_retrain_predictor.py
+-rw-rw-rw-   0        0        0     3572 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_selects.py
+-rw-rw-rw-   0        0        0     1226 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_show_mindsdb.py
+-rw-rw-rw-   0        0        0      959 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_timeseries.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mysql/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mysql/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mysql/test_mysql_lexer.py
+-rw-rw-rw-   0        0        0     3050 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_parser/test_mysql/test_mysql_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:56:56.000000 mindsdb_sql-0.6.4/tests/test_render/
+-rw-rw-rw-   0        0        0        0 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_render/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-06-14 12:56:24.000000 mindsdb_sql-0.6.4/tests/test_render/test_sqlalchemyrender.py
```

### Comparing `mindsdb_sql-0.6.3/PKG-INFO` & `mindsdb_sql-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb_sql
-Version: 0.6.3
+Version: 0.6.4
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.3/README.md` & `mindsdb_sql-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/__init__.py` & `mindsdb_sql-0.6.4/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/__init__.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,51 +18,55 @@
 
 RESERVED_KEYWORDS = {
     'PERSIST', 'IF', 'EXISTS', 'NULLS', 'FIRST', 'LAST',
     'ORDER', 'BY', 'GROUP', 'PARTITION'
 }
 
 
+def get_reserved_words():
+    from mindsdb_sql.parser.lexer import SQLLexer
+    from mindsdb_sql.parser.dialects.mindsdb.lexer import MindsDBLexer
+
+    reserved = RESERVED_KEYWORDS
+    for word in SQLLexer.tokens | MindsDBLexer.tokens:
+        if '_' not in word:
+            # exclude combinations
+            reserved.add(word)
+    return reserved
+
+
 class Identifier(ASTNode):
     def __init__(self, path_str=None, parts=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         assert path_str or parts, "Either path_str or parts must be provided for an Identifier"
         assert not (path_str and parts), "Provide either path_str or parts, but not both"
         if isinstance(path_str, Star) and not parts:
             parts = [Star()]
 
         if path_str and not parts:
             parts = path_str_to_parts(path_str)
         assert isinstance(parts, list)
         self.parts = parts
 
-        from mindsdb_sql.parser.lexer import SQLLexer
-        from mindsdb_sql.parser.dialects.mindsdb.lexer import MindsDBLexer
-
-        self.reserved = RESERVED_KEYWORDS
-        for word in SQLLexer.tokens | MindsDBLexer.tokens:
-            if '_' not in word:
-                # exclude combinations
-                self.reserved.add(word)
-
     @classmethod
     def from_path_str(self, value, *args, **kwargs):
         parts = path_str_to_parts(value)
         return Identifier(parts=parts, *args, **kwargs)
 
     def parts_to_str(self):
         out_parts = []
+        reserved_words = get_reserved_words()
         for part in self.parts:
             if isinstance(part, Star):
                 part = str(part)
             else:
                 if (
                     not no_wrap_identifier_regex.fullmatch(part)
                     or
-                    part.upper() in self.reserved
+                    part.upper() in reserved_words
                 ):
                     part = f'`{part}`'
 
             out_parts.append(part)
         return '.'.join(out_parts)
 
     def to_tree(self, *args, level=0, **kwargs):
```

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/chatbot.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/chatbot.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/evaluate.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.6.4/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.6.4/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.6.4/mindsdb_sql/planner/query_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import copy
 from collections import defaultdict
 from mindsdb_sql.exceptions import PlanningException
 from mindsdb_sql.parser import ast
 from mindsdb_sql.parser.ast import (Select, Identifier, Join, Star, BinaryOperation, Constant, OrderBy,
                                     BetweenOperation, Union, NullConstant, CreateTable, Function, Insert,
-                                    Update, NativeQuery, Parameter)
+                                    Update, NativeQuery, Parameter, Delete)
 
 from mindsdb_sql.parser.dialects.mindsdb.latest import Latest
 from mindsdb_sql.planner.steps import (FetchDataframeStep, ProjectStep, JoinStep, ApplyPredictorStep,
                                        ApplyPredictorRowStep, FilterStep, GroupByStep, LimitOffsetStep, OrderByStep,
                                        UnionStep, MapReduceStep, MultipleSteps, ApplyTimeseriesPredictorStep,
-                                       GetPredictorColumns, SaveToTable, InsertToTable, UpdateToTable, SubSelectStep)
+                                       GetPredictorColumns, SaveToTable, InsertToTable, UpdateToTable, SubSelectStep,
+                                       DeleteStep)
 from mindsdb_sql.planner.ts_utils import (validate_ts_where_condition, find_time_filter, replace_time_filter,
                                           find_and_remove_time_filter)
 from mindsdb_sql.planner.utils import (disambiguate_predictor_column_identifier,
                                        get_deepest_select,
                                        recursively_extract_column_values,
                                        recursively_check_join_identifiers_for_ambiguity,
                                        query_traversal)
@@ -216,14 +217,35 @@
 
                 elif integration is not None:
                     integrations.add(integration)
 
         utils.query_traversal(query, find_predictors)
         return {'mdb_entities': mdb_entities, 'integrations': integrations, 'predictors': predictors}
 
+    def get_nested_selects_plan_fnc(self, main_integration, force=False):
+        # returns function for traversal over query and inject fetch data query instead of subselects
+        def find_selects(node, **kwargs):
+            if isinstance(node, Select):
+                query_info2 = self.get_query_info(node)
+                if force or (
+                        len(query_info2['integrations']) > 1 or
+                        main_integration not in query_info2['integrations'] or
+                        len(query_info2['mdb_entities']) > 0
+                ):
+                    # need to execute in planner
+
+                    node.parentheses = False
+                    last_step = self.plan_select(node)
+                    node2 = Parameter(last_step.result)
+
+                    return node2
+
+        return find_selects
+
+
     def plan_select_identifier(self, query):
         query_info = self.get_query_info(query)
 
         if len(query_info['integrations']) == 0 and len(query_info['predictors']) >= 1:
             # select from predictor
             return self.plan_select_from_predictor(query)
         elif len(query_info['integrations']) == 1 and len(query_info['mdb_entities']) == 0:
@@ -231,31 +253,17 @@
             int_name = list(query_info['integrations'])[0]
             if self.integrations.get(int_name, {}).get('class_type') != 'api':
                 # one integration without predictors, send all query to integration
                 return self.plan_integration_select(query)
 
         # find subselects
         main_integration, _ = self.resolve_database_table(query.from_table)
+        is_api_db = self.integrations.get(main_integration, {}).get('class_type') == 'api'
 
-        def find_selects(node, **kwargs):
-            if isinstance(node, Select):
-                query_info2 = self.get_query_info(node)
-                if (
-                        len(query_info2['integrations']) > 1 or
-                        main_integration not in query_info2['integrations'] or
-                        len(query_info2['mdb_entities']) > 0
-                ):
-                    # need to execute in planner
-
-                    node.parentheses = False
-                    last_step = self.plan_select(node)
-                    node2 = Parameter(last_step.result)
-
-                    return node2
-
+        find_selects = self.get_nested_selects_plan_fnc(main_integration, force=is_api_db)
         query.targets = utils.query_traversal(query.targets, find_selects)
         utils.query_traversal(query.where, find_selects)
 
         if len(query_info['predictors']) >= 1:
             # select from predictor
             return self.plan_select_from_predictor(query)
         else:
@@ -1089,33 +1097,48 @@
         else:
             self.plan.add_step(InsertToTable(
                 table=table,
                 query=query,
             ))
 
     def plan_update(self, query):
-        if query.from_select is None:
-            raise PlanningException(f'Support only insert from select')
-
-        integration_name = query.table.parts[0]
+        last_step = None
+        if query.from_select is not None:
+            integration_name = query.table.parts[0]
+            last_step = self.plan_select(query.from_select, integration=integration_name)
 
         # plan sub-select first
-        last_step = self.plan_select(query.from_select, integration=integration_name)
-
         update_command = copy.deepcopy(query)
         # clear subselect
         update_command.from_select = None
 
         table = query.table
         self.plan.add_step(UpdateToTable(
             table=table,
             dataframe=last_step,
             update_command=update_command
         ))
 
+    def plan_delete(self, query: Delete):
+
+        # find subselects
+        main_integration, _ = self.resolve_database_table(query.table)
+
+        is_api_db = self.integrations.get(main_integration, {}).get('class_type') == 'api'
+
+        find_selects = self.get_nested_selects_plan_fnc(main_integration, force=is_api_db)
+        utils.query_traversal(query.where, find_selects)
+
+        self.prepare_integration_select(main_integration, query.where)
+
+        return self.plan.add_step(DeleteStep(
+            table=query.table,
+            where=query.where
+        ))
+
     def plan_select(self, query, integration=None):
         from_table = query.from_table
 
         if isinstance(from_table, Identifier):
             return self.plan_select_identifier(query)
         elif isinstance(from_table, Select):
             return self.plan_nested_select(query)
@@ -1170,14 +1193,16 @@
             self.plan_union(query)
         elif isinstance(query, CreateTable):
             self.plan_create_table(query)
         elif isinstance(query, Insert):
             self.plan_insert(query)
         elif isinstance(query, Update):
             self.plan_update(query)
+        elif isinstance(query, Delete):
+            self.plan_delete(query)
         else:
             raise PlanningException(f'Unsupported query type {type(query)}')
 
         return self.plan
 
     def prepare_steps(self, query):
         statement_planner = PreparedStatementPlanner(self)
```

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.6.4/mindsdb_sql/planner/query_prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,14 +515,15 @@
 
         if (
                 isinstance(query, ast.Select)
                 or isinstance(query, ast.Union)
                 or isinstance(query, ast.CreateTable)
                 or isinstance(query, ast.Insert)
                 or isinstance(query, ast.Update)
+                or isinstance(query, ast.Delete)
         ):
             return self.plan_query(query)
         else:
             return []
 
     def plan_query(self, query):
         # use v1 planner
```

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.6.4/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.6.4/mindsdb_sql/planner/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,22 @@
         """Fills table with content of dataframe"""
         super().__init__(*args, **kwargs)
         self.table = table
         self.dataframe = dataframe
         self.update_command = update_command
 
 
+class DeleteStep(PlanStep):
+    def __init__(self, table, where, *args, **kwargs):
+        """Fills table with content of dataframe"""
+        super().__init__(*args, **kwargs)
+        self.table = table
+        self.where = where
+
+
 class SubSelectStep(PlanStep):
     def __init__(self, query, dataframe, table_name=None, *args, **kwargs):
         """Performs select from dataframe"""
         super().__init__(*args, **kwargs)
         self.query = query
         self.dataframe = dataframe
         self.table_name = table_name
```

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.6.4/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/planner/utils.py` & `mindsdb_sql-0.6.4/mindsdb_sql/planner/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.6.4/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql.egg-info/PKG-INFO` & `mindsdb_sql-0.6.4/mindsdb_sql.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb-sql
-Version: 0.6.3
+Version: 0.6.4
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.3/mindsdb_sql.egg-info/SOURCES.txt` & `mindsdb_sql-0.6.4/mindsdb_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/setup.py` & `mindsdb_sql-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ast.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_ast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_base_lexer.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_base_lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_create.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ddl.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_ddl.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_delete.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_describe.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_insert.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_misc_sql_queries.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_misc_sql_queries.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_common_table_expression.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_select_common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_operations.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_select_operations.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_structure.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_select_structure.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_show.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_union.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_update.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_use.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_base_sql/test_use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_chatbots.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_chatbots.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_file.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_integration.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_predictor.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_view.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_dataset.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_datasource.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_integration.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_predictor.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_evaluate.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_finetune_predictor.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_finetune_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_jobs.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_jobs.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_ml_engine.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_retrain_predictor.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_retrain_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_selects.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_selects.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_show_mindsdb.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_show_mindsdb.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_timeseries.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mindsdb/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_lexer.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mysql/test_mysql_lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_parser.py` & `mindsdb_sql-0.6.4/tests/test_parser/test_mysql/test_mysql_parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.3/tests/test_render/test_sqlalchemyrender.py` & `mindsdb_sql-0.6.4/tests/test_render/test_sqlalchemyrender.py`

 * *Files identical despite different names*

