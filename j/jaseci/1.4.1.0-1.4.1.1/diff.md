# Comparing `tmp/jaseci-1.4.1.0.tar.gz` & `tmp/jaseci-1.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci-1.4.1.0.tar", last modified: Wed Jun  7 18:24:54 2023, max compression
+gzip compressed data, was "jaseci-1.4.1.1.tar", last modified: Wed Jun 14 19:22:28 2023, max compression
```

## Comparing `jaseci-1.4.1.0.tar` & `jaseci-1.4.1.1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/cli_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/book_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/cli_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/tests/test_jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/extens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.723014 jaseci-1.4.1.0/jaseci/extens/act_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/jaseci.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/std.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.723014 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/std_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_file_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_mail_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_net_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_zlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/extens/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/actions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/alias_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/jac_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/jsorc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/master_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/super_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/extens/api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/webhook_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/extens/svc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/elastic_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/kube_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/mail_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/prome_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/redis_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/stripe_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/task_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/jac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/architype_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    66659 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/sentinel_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/interpreter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/walker_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/ast_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/jac_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/ir/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/ast_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/codegen_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/ir_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/printer_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/pt_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/stats_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac.g4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/jac_parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/jacLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/jacListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/jacParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/jsci_vm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/disasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/inst_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/op_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/test_codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/jac_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/jac_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/machine_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jac/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/book_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/test_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/test_lang_14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jsorc/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/jsorc_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/jsorc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/live_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jsorc/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/database.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/elastic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/prometheus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/remote_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jsorc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/tests/test_jsorc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/prim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/ability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/architype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/obj_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/super_master.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/jaseci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/jac_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/jac_test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_jac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/jaseci/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/jaseci/utils/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/actions_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/actions_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/actions_state.py
--rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/gprof2dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/id_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/book_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/cli_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/tests/test_jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/extens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.242444 jaseci-1.4.1.1/jaseci/extens/act_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/jaseci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.246444 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/std_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_mail_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_net_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_zlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.250444 jaseci-1.4.1.1/jaseci/extens/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/alias_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/jsorc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/master_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/super_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.254444 jaseci-1.4.1.1/jaseci/extens/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/webhook_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.254444 jaseci-1.4.1.1/jaseci/extens/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/elastic_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/kube_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/prome_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/redis_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/stripe_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.254444 jaseci-1.4.1.1/jaseci/jac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/architype_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66659 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/sentinel_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/interpreter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/walker_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/ast_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/jac_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/ir/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/ast_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/codegen_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/ir_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/printer_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/pt_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/stats_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac.g4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/jac_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/jacLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/jacListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/jacParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/jsci_vm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/inst_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/op_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/test_codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/jac_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/jac_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/machine_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jac/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/book_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/test_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/test_lang_14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jsorc/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/jsorc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/jsorc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/live_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jsorc/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/database.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/elastic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/prometheus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/remote_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jsorc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/tests/test_jsorc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.270445 jaseci-1.4.1.1/jaseci/prim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/architype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/obj_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/super_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/jaseci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/jac_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/jac_test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_jac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/jaseci/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/jaseci/utils/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/actions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/actions_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/actions_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/gprof2dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/id_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/setup.py
```

### Comparing `jaseci-1.4.1.0/LICENSE` & `jaseci-1.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/__init__.py` & `jaseci-1.4.1.1/jaseci/__init__.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/cli_tools/book_tools.py` & `jaseci-1.4.1.1/jaseci/cli_tools/book_tools.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/cli_tools/jsctl.py` & `jaseci-1.4.1.1/jaseci/cli_tools/jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/cli_tools/tests/test_jsctl.py` & `jaseci-1.4.1.1/jaseci/cli_tools/tests/test_jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/date.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/elastic.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/file.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/file.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/jaseci.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/jaseci.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/net.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/net.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/rand.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/rand.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/regex.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/request.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/request.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/std.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/stripe.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/stripe.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/std_test_code.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/std_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_date.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_elastic.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_file_lib.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_file_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_mail_lib.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_mail_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_net_lib.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_net_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_regex.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std_lib.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_url.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_vector.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_webtool.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_zlib.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_zlib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/url.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/vector.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/webtool.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/act_lib/zip.py` & `jaseci-1.4.1.1/jaseci/extens/act_lib/zip.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/actions_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/alias_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/alias_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/architype_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/config_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/config_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/global_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/graph_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/interface.py` & `jaseci-1.4.1.1/jaseci/extens/api/interface.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/jac_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/jac_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/jsorc_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/jsorc_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/logger_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/master_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/master_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/object_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/prometheus_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/queue_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/sentinel_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/super_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/super_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_architype_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_global_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_graph_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_logger_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_object_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_sentinel_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_user_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/tests/test_walker_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/tests/test_walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/user_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/walker_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/api/webhook_api.py` & `jaseci-1.4.1.1/jaseci/extens/api/webhook_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/elastic_svc.py` & `jaseci-1.4.1.1/jaseci/extens/svc/elastic_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/kube_svc.py` & `jaseci-1.4.1.1/jaseci/extens/svc/kube_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/mail_svc.py` & `jaseci-1.4.1.1/jaseci/extens/svc/mail_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/prome_svc.py` & `jaseci-1.4.1.1/jaseci/extens/svc/prome_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/redis_svc.py` & `jaseci-1.4.1.1/jaseci/extens/svc/redis_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/stripe_svc.py` & `jaseci-1.4.1.1/jaseci/extens/svc/stripe_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/task_svc.py` & `jaseci-1.4.1.1/jaseci/extens/svc/task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/extens/svc/tasks.py` & `jaseci-1.4.1.1/jaseci/extens/svc/tasks.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/interpreter/architype_interp.py` & `jaseci-1.4.1.1/jaseci/jac/interpreter/architype_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/interpreter/interp.py` & `jaseci-1.4.1.1/jaseci/jac/interpreter/interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/interpreter/sentinel_interp.py` & `jaseci-1.4.1.1/jaseci/jac/interpreter/sentinel_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/interpreter/tests/test_interp.py` & `jaseci-1.4.1.1/jaseci/jac/interpreter/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/interpreter/walker_interp.py` & `jaseci-1.4.1.1/jaseci/jac/interpreter/walker_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/ast.py` & `jaseci-1.4.1.1/jaseci/jac/ir/ast.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/ast_builder.py` & `jaseci-1.4.1.1/jaseci/jac/ir/ast_builder.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/jac_code.py` & `jaseci-1.4.1.1/jaseci/jac/ir/jac_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/passes/codegen_pass.py` & `jaseci-1.4.1.1/jaseci/jac/ir/passes/codegen_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/passes/ir_pass.py` & `jaseci-1.4.1.1/jaseci/jac/ir/passes/ir_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/passes/printer_pass.py` & `jaseci-1.4.1.1/jaseci/jac/ir/passes/printer_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/passes/pt_prune_pass.py` & `jaseci-1.4.1.1/jaseci/jac/ir/passes/pt_prune_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/ir/passes/schedule.py` & `jaseci-1.4.1.1/jaseci/jac/ir/passes/schedule.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jac.g4` & `jaseci-1.4.1.1/jaseci/jac/jac.g4`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jac_parse/jacLexer.py` & `jaseci-1.4.1.1/jaseci/jac/jac_parse/jacLexer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jac_parse/jacListener.py` & `jaseci-1.4.1.1/jaseci/jac/jac_parse/jacListener.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jac_parse/jacParser.py` & `jaseci-1.4.1.1/jaseci/jac/jac_parse/jacParser.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jac_set.py` & `jaseci-1.4.1.1/jaseci/jac/jac_set.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jsci_vm/disasm.py` & `jaseci-1.4.1.1/jaseci/jac/jsci_vm/disasm.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jsci_vm/inst_ptr.py` & `jaseci-1.4.1.1/jaseci/jac/jsci_vm/inst_ptr.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jsci_vm/machine.py` & `jaseci-1.4.1.1/jaseci/jac/jsci_vm/machine.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jsci_vm/op_codes.py` & `jaseci-1.4.1.1/jaseci/jac/jsci_vm/op_codes.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/test_codegen.py` & `jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/machine/jac_scope.py` & `jaseci-1.4.1.1/jaseci/jac/machine/jac_scope.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/machine/jac_value.py` & `jaseci-1.4.1.1/jaseci/jac/machine/jac_value.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/machine/machine_state.py` & `jaseci-1.4.1.1/jaseci/jac/machine/machine_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/tests/book_code.py` & `jaseci-1.4.1.1/jaseci/jac/tests/book_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/tests/test_book.py` & `jaseci-1.4.1.1/jaseci/jac/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jac/tests/test_lang_14.py` & `jaseci-1.4.1.1/jaseci/jac/tests/test_lang_14.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/jsorc.py` & `jaseci-1.4.1.1/jaseci/jsorc/jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/jsorc_settings.py` & `jaseci-1.4.1.1/jaseci/jsorc/jsorc_settings.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/jsorc_utils.py` & `jaseci-1.4.1.1/jaseci/jsorc/jsorc_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/live_actions.py` & `jaseci-1.4.1.1/jaseci/jsorc/live_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/manifests/database.yaml` & `jaseci-1.4.1.1/jaseci/jsorc/manifests/database.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/manifests/elastic.yaml` & `jaseci-1.4.1.1/jaseci/jsorc/manifests/elastic.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/manifests/prometheus.yaml` & `jaseci-1.4.1.1/jaseci/jsorc/manifests/prometheus.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/manifests/redis.yaml` & `jaseci-1.4.1.1/jaseci/jsorc/manifests/redis.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/memory.py` & `jaseci-1.4.1.1/jaseci/jsorc/memory.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/redis.py` & `jaseci-1.4.1.1/jaseci/jsorc/redis.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/remote_actions.py` & `jaseci-1.4.1.1/jaseci/jsorc/remote_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/tests/test_actions.py` & `jaseci-1.4.1.1/jaseci/jsorc/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/jsorc/tests/test_jsorc.py` & `jaseci-1.4.1.1/jaseci/jsorc/tests/test_jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/ability.py` & `jaseci-1.4.1.1/jaseci/prim/ability.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/architype.py` & `jaseci-1.4.1.1/jaseci/prim/architype.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/edge.py` & `jaseci-1.4.1.1/jaseci/prim/edge.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/element.py` & `jaseci-1.4.1.1/jaseci/prim/element.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/graph.py` & `jaseci-1.4.1.1/jaseci/prim/graph.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/master.py` & `jaseci-1.4.1.1/jaseci/prim/master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/node.py` & `jaseci-1.4.1.1/jaseci/prim/node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/obj_mixins.py` & `jaseci-1.4.1.1/jaseci/prim/obj_mixins.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/sentinel.py` & `jaseci-1.4.1.1/jaseci/prim/sentinel.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/super_master.py` & `jaseci-1.4.1.1/jaseci/prim/super_master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/prim/walker.py` & `jaseci-1.4.1.1/jaseci/prim/walker.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/infer.py` & `jaseci-1.4.1.1/jaseci/tests/infer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/jac_test_code.py` & `jaseci-1.4.1.1/jaseci/tests/jac_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/jac_test_progs.py` & `jaseci-1.4.1.1/jaseci/tests/jac_test_progs.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/test_core.py` & `jaseci-1.4.1.1/jaseci/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/test_jac.py` & `jaseci-1.4.1.1/jaseci/tests/test_jac.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/test_node.py` & `jaseci-1.4.1.1/jaseci/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/test_progs.py` & `jaseci-1.4.1.1/jaseci/tests/test_progs.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/test_stack.py` & `jaseci-1.4.1.1/jaseci/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/tests/test_stripe.py` & `jaseci-1.4.1.1/jaseci/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/actions/actions_manager.py` & `jaseci-1.4.1.1/jaseci/utils/actions/actions_manager.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/actions/actions_optimizer.py` & `jaseci-1.4.1.1/jaseci/utils/actions/actions_optimizer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/actions/actions_state.py` & `jaseci-1.4.1.1/jaseci/utils/actions/actions_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/gprof2dot.py` & `jaseci-1.4.1.1/jaseci/utils/gprof2dot.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/id_list.py` & `jaseci-1.4.1.1/jaseci/utils/id_list.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/json_handler.py` & `jaseci-1.4.1.1/jaseci/utils/json_handler.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/log_utils.py` & `jaseci-1.4.1.1/jaseci/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/test_core.py` & `jaseci-1.4.1.1/jaseci/utils/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci/utils/utils.py` & `jaseci-1.4.1.1/jaseci/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/jaseci.egg-info/SOURCES.txt` & `jaseci-1.4.1.1/jaseci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.0/setup.py` & `jaseci-1.4.1.1/setup.py`

 * *Files identical despite different names*

