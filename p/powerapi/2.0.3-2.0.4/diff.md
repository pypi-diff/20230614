# Comparing `tmp/powerapi-2.0.3.tar.gz` & `tmp/powerapi-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerapi-2.0.3.tar", last modified: Tue Apr 25 14:42:30 2023, max compression
+gzip compressed data, was "powerapi-2.0.4.tar", last modified: Wed Jun 14 09:43:35 2023, max compression
```

## Comparing `powerapi-2.0.3.tar` & `powerapi-2.0.4.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.830734 powerapi-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-25 14:42:12.000000 powerapi-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-25 14:42:30.830734 powerapi-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-25 14:42:12.000000 powerapi-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/socket_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi/backend_supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/backend_supervisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/backend_supervisor/backend_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.814734 powerapi-2.0.3/powerapi/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/base_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/csvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/direct_prometheus_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/file_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/opentsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/prometheus_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/socket_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/virtiofs_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/dispatch_rule/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/hwpc_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/power_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/procfs_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/simple_dispatch_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/blocking_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/route_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/dispatcher/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/filter/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/abstract_cpu_dram_formula.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/formula/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/simple/simple_formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/simple/simple_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/poison_pill_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/start_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/puller/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/puller_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/puller/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/simple/simple_puller_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/simple/simple_puller_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/pusher/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/pusher_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/pusher/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/control_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/formula_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/hwpc_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/power_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/procfs_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/report_modifier/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report_modifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report_modifier/libvirt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report_modifier/report_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/stat_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-25 14:42:12.000000 powerapi-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:42:30.830734 powerapi-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-14 09:43:24.000000 powerapi-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-14 09:43:35.955064 powerapi-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-14 09:43:24.000000 powerapi-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.939064 powerapi-2.0.4/powerapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/socket_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/backend_supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/backend_supervisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/backend_supervisor/backend_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/common_cli_parsing_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18482 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/parsing_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/base_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/csvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/direct_prometheus_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/opentsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/prometheus_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/socket_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/virtiofs_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/dispatch_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/hwpc_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/power_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/procfs_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/simple_dispatch_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/blocking_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/dispatcher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/route_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/dispatcher/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/abstract_cpu_dram_formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/formula_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/formula/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/simple/simple_formula_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/simple/simple_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/poison_pill_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/start_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/puller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/puller_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/puller/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/simple/simple_puller_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/simple/simple_puller_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/pusher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/pusher_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/pusher/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/control_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/formula_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/hwpc_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/power_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/procfs_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/report_modifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report_modifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report_modifier/libvirt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report_modifier/report_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/stat_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.939064 powerapi-2.0.4/powerapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-14 09:43:24.000000 powerapi-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:43:35.955064 powerapi-2.0.4/setup.cfg
```

### Comparing `powerapi-2.0.3/LICENSE` & `powerapi-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/PKG-INFO` & `powerapi-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.0.3
+Version: 2.0.4
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerapi Version: 2.0.3 Summary: PowerAPI is a
+Metadata-Version: 2.1 Name: powerapi Version: 2.0.4 Summary: PowerAPI is a
 middleware toolkit for building software-defined power meters. Author-email:
 PowerAPI Staff
 inria.fr> License: BSD-3-Clause Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org Project-URL:
 repository, https://github.com/powerapi-ng/powerapi Keywords:
 powerapi,energy,power-meter,green-computing Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `powerapi-2.0.3/README.md` & `powerapi-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/__init__.py` & `powerapi-2.0.4/powerapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
```

### Comparing `powerapi-2.0.3/powerapi/actor/__init__.py` & `powerapi-2.0.4/powerapi/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/actor/actor.py` & `powerapi-2.0.4/powerapi/actor/actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/actor/socket_interface.py` & `powerapi-2.0.4/powerapi/actor/socket_interface.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/actor/state.py` & `powerapi-2.0.4/powerapi/actor/state.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/actor/supervisor.py` & `powerapi-2.0.4/powerapi/actor/supervisor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/backend_supervisor/__init__.py` & `powerapi-2.0.4/powerapi/backend_supervisor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/backend_supervisor/backend_supervisor.py` & `powerapi-2.0.4/powerapi/backend_supervisor/backend_supervisor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/cli/__init__.py` & `powerapi-2.0.4/powerapi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/cli/config_validator.py` & `powerapi-2.0.4/powerapi/cli/config_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging
 import os
 
 from typing import Dict
 
+from powerapi.exception import MissingArgumentException, NotAllowedArgumentValueException, FileDoesNotExistException
+
 
 class ConfigValidator:
     """
     Validate powerapi config and initialize missing default values
     """
     @staticmethod
     def validate(config: Dict):
@@ -44,54 +46,51 @@
         """
         if 'verbose' not in config:
             config['verbose'] = logging.NOTSET
         if 'stream' not in config:
             config['stream'] = False
         if 'output' not in config:
             logging.error("no output configuration found")
-            return False
+            raise MissingArgumentException(argument_name='output')
 
         for output_type in config['output']:
             output_config = config['output'][output_type]
             if 'model' not in output_config:
                 output_config['model'] = 'HWPCReport'
             if 'name' not in output_config:
                 output_config['name'] = 'default_pusher'
 
         if 'input' not in config:
             logging.error("no input configuration found")
-            return False
+            raise MissingArgumentException(argument_name='input')
 
         for input_id in config['input']:
             input_config = config['input'][input_id]
             if input_config['type'] == 'csv' \
                     and ('files' not in input_config or input_config['files'] is None or len(input_config['files']) == 0):
                 logging.error("no files parameter found for csv input")
-                return False
+                raise MissingArgumentException(argument_name='files')
 
             if input_config['type'] == 'csv' and config['stream']:
                 logging.error("stream mode cannot be used for csv input")
-                return False
+                raise NotAllowedArgumentValueException("Stream mode cannot be used for csv input")
 
             if 'model' not in input_config:
                 input_config['model'] = 'PowerReport'
             if 'name' not in input_config:
                 input_config['name'] = 'default_puller'
 
-        if not ConfigValidator._validate_input(config):
-            return False
-        return True
+        ConfigValidator._validate_input(config)
 
     @staticmethod
     def _validate_input(config: Dict):
         for key, input_config in config['input'].items():
             if input_config['type'] == 'csv':
                 list_of_files = input_config['files']
 
                 if isinstance(list_of_files, str):
                     list_of_files = input_config['files'].split(",")
                     config['input'][key]['files'] = list_of_files
 
                 for file_name in list_of_files:
                     if not os.access(file_name, os.R_OK):
-                        return False
-        return True
+                        raise FileDoesNotExistException(file_name=file_name)
```

### Comparing `powerapi-2.0.3/powerapi/cli/generator.py` & `powerapi-2.0.4/powerapi/cli/generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 import logging
 import os
 import sys
 from typing import Dict, Type
 
 from powerapi.actor import Actor
 from powerapi.database.influxdb2 import InfluxDB2
-from powerapi.exception import PowerAPIException
+from powerapi.exception import PowerAPIException, ModelNameAlreadyUsed, DatabaseNameDoesNotExist, ModelNameDoesNotExist, \
+    DatabaseNameAlreadyUsed
 from powerapi.filter import Filter
 from powerapi.report import HWPCReport, PowerReport, ControlReport, ProcfsReport, Report, FormulaReport
 from powerapi.database import MongoDB, CsvDB, InfluxDB, OpenTSDB, SocketDB, PrometheusDB, DirectPrometheusDB, \
     VirtioFSDB, FileDB
 from powerapi.puller import PullerActor
 from powerapi.pusher import PusherActor
 
@@ -77,15 +78,15 @@
         ...
     }
     """
 
     def __init__(self, component_group_name):
         self.component_group_name = component_group_name
 
-    def generate(self, main_config: Dict) -> Dict[str, Type[Actor]]:
+    def generate(self, main_config: dict) -> Dict[str, Type[Actor]]:
         """
         Generate an actor class and actor start message from config dict
         """
         if self.component_group_name not in main_config:
             raise PowerAPIException('Configuration error : no ' + self.component_group_name + ' specified')
 
         actors = {}
@@ -99,139 +100,101 @@
                 msg = 'Configuration error : argument ' + exn.args[0]
                 msg += ' needed with output ' + component_type
                 print(msg, file=sys.stderr)
                 raise PowerAPIException(msg) from exn
 
         return actors
 
-    def _gen_actor(self, component_config: Dict, main_config: Dict, component_name: str) -> Type[Actor]:
+    def _gen_actor(self, component_config: dict, main_config: dict, component_name: str) -> Type[Actor]:
         raise NotImplementedError()
 
 
-class ModelNameAlreadyUsed(PowerAPIException):
-    """
-    Exception raised when attempting to add to a DBActorGenerator a model factory with a name already bound to another
-    model factory in the DBActorGenerator
-    """
-
-    def __init__(self, model_name):
-        PowerAPIException.__init__(self)
-        self.model_name = model_name
-
-
-class DatabaseNameAlreadyUsed(PowerAPIException):
-    """
-    Exception raised when attempting to add to a DBActorGenerator a database factory with a name already bound to
-    another database factory in the DBActorGenerator
-    """
-
-    def __init__(self, database_name):
-        PowerAPIException.__init__(self)
-        self.database_name = database_name
-
-
-class ModelNameDoesNotExist(PowerAPIException):
-    """
-    Exception raised when attempting to remove to a DBActorGenerator a model factory with a name that is not bound to
-    another model factory in the DBActorGenerator
-    """
-
-    def __init__(self, model_name):
-        PowerAPIException.__init__(self)
-        self.model_name = model_name
-
-
-class DatabaseNameDoesNotExist(PowerAPIException):
-    """
-    Exception raised when attempting to remove to a DBActorGenerator a database factory with a name that is not bound to
-    another database factory in the DBActorGenerator
-    """
-
-    def __init__(self, database_name):
-        PowerAPIException.__init__(self)
-        self.database_name = database_name
-
-
-def gen_tag_list(db_config: Dict):
+def gen_tag_list(db_config: dict):
     """
     Generate tag list from tag string
     """
     if 'tags' not in db_config:
         return []
     return db_config['tags'].split(',')
 
 
-class SimpleGenerator(Generator):
+class BaseGenerator(Generator):
     """
-    Generate Simple Actor class and Simple Start message from config
+    Generate an Actor and Start message from config
     """
 
     def __init__(self, component_group_name: str):
         Generator.__init__(self, component_group_name)
         self.report_classes = {
             'HWPCReport': HWPCReport,
             'PowerReport': PowerReport
         }
 
-    def _gen_actor(self, component_config: Dict, main_config: Dict, component_name: str):
+    def _gen_actor(self, component_config: dict, main_config: dict, component_name: str):
         model = self._get_report_class(component_config[COMPONENT_MODEL_KEY], component_config)
         component_config[COMPONENT_MODEL_KEY] = model
 
         actor = self._actor_factory(component_name, main_config, component_config)
         return actor
 
-    def _get_report_class(self, model_name, component_config):
+    def _get_report_class(self, model_name: str, component_config: dict):
         if model_name not in self.report_classes:
             raise PowerAPIException(f'Configuration error: model type {model_name} unknown')
 
         return self.report_classes[component_config[COMPONENT_MODEL_KEY]]
 
-    def _actor_factory(self, actor_name: str, main_config: Dict, component_config: Dict):
+    def _actor_factory(self, actor_name: str, main_config: dict, component_config: dict):
         raise NotImplementedError
 
 
-class DBActorGenerator(SimpleGenerator):
+class DBActorGenerator(BaseGenerator):
     """
     ActorGenerator that initialise the start message with a database from config
     """
 
     def __init__(self, component_group_name: str):
-        SimpleGenerator.__init__(self, component_group_name)
+        BaseGenerator.__init__(self, component_group_name)
         self.report_classes['FormulaReport'] = FormulaReport
         self.report_classes['ControlReport'] = ControlReport
         self.report_classes['ProcfsReport'] = ProcfsReport
 
         self.db_factory = {
-            'mongodb': lambda db_config: MongoDB(db_config['model'], db_config['uri'], db_config['db'],
-                                                 db_config['collection']),
+            'mongodb': lambda db_config: MongoDB(report_type=db_config['model'], uri=db_config['uri'],
+                                                 db_name=db_config['db'], collection_name=db_config['collection']),
             'socket': lambda db_config: SocketDB(db_config['model'], db_config['port']),
-            'csv': lambda db_config: CsvDB(db_config['model'], gen_tag_list(db_config),
+            'csv': lambda db_config: CsvDB(report_type=db_config['model'], tags=gen_tag_list(db_config),
                                            current_path=os.getcwd() if 'directory' not in db_config else db_config[
                                                'directory'],
                                            files=[] if 'files' not in db_config else db_config['files']),
-            'influxdb': lambda db_config: InfluxDB(db_config['model'], db_config['uri'], db_config['port'],
-                                                   db_config['db'], gen_tag_list(db_config)),
-            'influxdb2': lambda db_config: InfluxDB2(db_config['model'], db_config['uri'], db_config['org'],
-                                                     db_config['db'], db_config['token'], gen_tag_list(db_config),
+            'influxdb': lambda db_config: InfluxDB(report_type=db_config['model'], uri=db_config['uri'],
+                                                   port=db_config['port'], db_name=db_config['db'],
+                                                   tags=gen_tag_list(db_config)),
+            'influxdb2': lambda db_config: InfluxDB2(report_type=db_config['model'], url=db_config['uri'],
+                                                     org=db_config['org'],
+                                                     bucket_name=db_config['db'], token=db_config['token'],
+                                                     tags=gen_tag_list(db_config),
                                                      port=None if 'port' not in db_config else db_config['port']),
-            'opentsdb': lambda db_config: OpenTSDB(db_config['model'], db_config['uri'], db_config['port'],
-                                                   db_config['metric_name']),
-            'prom': lambda db_config: PrometheusDB(db_config['model'], db_config['port'], db_config['uri'],
-                                                   db_config['metric_name'],
-                                                   db_config['metric_description'], db_config['aggregation_period'],
-                                                   gen_tag_list(db_config)),
-            'direct_prom': lambda db_config: DirectPrometheusDB(db_config['model'], db_config['port'], db_config['uri'],
-                                                                db_config['metric_name'],
-                                                                db_config['metric_description'],
-                                                                gen_tag_list(db_config)),
-            'virtiofs': lambda db_config: VirtioFSDB(db_config['model'], db_config['vm_name_regexp'],
-                                                     db_config['root_directory_name'],
-                                                     db_config['vm_directory_name_prefix'],
-                                                     db_config['vm_directory_name_suffix']),
-            'filedb': lambda db_config: FileDB(db_config['model'], db_config['filename'])
+            'opentsdb': lambda db_config: OpenTSDB(report_type=db_config['model'], host=db_config['uri'],
+                                                   port=db_config['port'], metric_name=db_config['metric_name']),
+            'prom': lambda db_config: PrometheusDB(report_type=db_config['model'], port=db_config['port'],
+                                                   address=db_config['uri'], metric_name=db_config['metric_name'],
+                                                   metric_description=db_config['metric_description'],
+                                                   aggregation_periode=db_config['aggregation_period'],
+                                                   tags=gen_tag_list(db_config)),
+            'direct_prom': lambda db_config: DirectPrometheusDB(report_type=db_config['model'], port=db_config['port'],
+                                                                address=db_config['uri'],
+                                                                metric_name=db_config['metric_name'],
+                                                                metric_description=db_config['metric_description'],
+                                                                tags=gen_tag_list(db_config)),
+            'virtiofs': lambda db_config: VirtioFSDB(report_type=db_config['model'],
+                                                     vm_name_regexp=db_config['vm_name_regexp'],
+                                                     root_directory_name=db_config['root_directory_name'],
+                                                     vm_directory_name_prefix=db_config['vm_directory_name_prefix'],
+                                                     vm_directory_name_suffix=db_config['vm_directory_name_suffix']),
+            'filedb': lambda db_config: FileDB(report_type=db_config['model'], filename=db_config['filename'])
         }
 
     def remove_report_class(self, model_name: str):
         """
         remove a Model from generator
         """
         if model_name not in self.report_classes:
@@ -258,64 +221,70 @@
         """
         add a database to generator
         """
         if db_name in self.db_factory:
             raise DatabaseNameAlreadyUsed(db_name)
         self.db_factory[db_name] = db_factory_function
 
-    def _generate_db(self, db_name: str, component_config: Dict):
+    def _generate_db(self, db_name: str, component_config: dict):
         if db_name not in self.db_factory:
             msg = 'Configuration error : database type ' + db_name + ' unknown'
             print(msg, file=sys.stderr)
             raise PowerAPIException(msg)
         else:
             return self.db_factory[db_name](component_config)
 
-    def _gen_actor(self, component_config: Dict, main_config: Dict, actor_name: str):
+    def _gen_actor(self, component_config: dict, main_config: dict, actor_name: str):
         model = self._get_report_class(component_config[COMPONENT_MODEL_KEY], component_config)
         component_config[COMPONENT_MODEL_KEY] = model
         database_manager = self._generate_db(component_config[COMPONENT_TYPE_KEY], component_config)
         component_config[COMPONENT_DB_MANAGER_KEY] = database_manager
 
         actor = self._actor_factory(actor_name, main_config, component_config)
         return actor
 
 
 class PullerGenerator(DBActorGenerator):
     """
     Generate Puller Actor class and Puller start message from config
     """
 
-    def __init__(self, report_filter: Filter, report_modifier_list=[]):
+    def __init__(self, report_filter: Filter, report_modifier_list=None):
         DBActorGenerator.__init__(self, 'input')
         self.report_filter = report_filter
+
+        if report_modifier_list is None:
+            report_modifier_list = []
         self.report_modifier_list = report_modifier_list
 
-    def _actor_factory(self, actor_name: str, main_config, component_config: Dict):
+    def _actor_factory(self, actor_name: str, main_config, component_config: dict):
         return PullerActor(name=actor_name, database=component_config[COMPONENT_DB_MANAGER_KEY],
                            report_filter=self.report_filter, stream_mode=main_config[GENERAL_CONF_STREAM_MODE_KEY],
                            report_modifier_list=self.report_modifier_list,
                            report_model=component_config[COMPONENT_MODEL_KEY],
                            level_logger=logging.DEBUG if main_config[GENERAL_CONF_VERBOSE_KEY] else logging.INFO)
 
 
 COMPONENT_NUMBER_OF_REPORTS_TO_SEND_KEY = 'number_of_reports_to_send'
 
 
-class SimplePullerGenerator(SimpleGenerator):
+class SimplePullerGenerator(BaseGenerator):
     """
     Generate Simple Puller Actor class and Simple Puller start message from config
     """
 
-    def __init__(self, report_filter, report_modifier_list=[]):
-        SimpleGenerator.__init__(self, 'input')
+    def __init__(self, report_filter, report_modifier_list=None):
+        BaseGenerator.__init__(self, 'input')
         self.report_filter = report_filter
+
+        if report_modifier_list is None:
+            report_modifier_list = []
         self.report_modifier_list = report_modifier_list
 
-    def _actor_factory(self, actor_name: str, main_config: Dict, component_config: Dict):
+    def _actor_factory(self, actor_name: str, main_config: dict, component_config: dict):
         return SimplePullerActor(name=actor_name, report_filter=self.report_filter,
                                  number_of_reports_to_send=component_config[COMPONENT_NUMBER_OF_REPORTS_TO_SEND_KEY],
                                  report_type_to_send=component_config[COMPONENT_MODEL_KEY])
 
 
 COMPONENT_NUMBER_OF_REPORTS_TO_STORE_KEY = 'number_of_reports_to_store'
 
@@ -324,47 +293,47 @@
     """
     Generate Pusher actor and Pusher start message from config
     """
 
     def __init__(self):
         DBActorGenerator.__init__(self, 'output')
 
-    def _actor_factory(self, actor_name: str, main_config: Dict, component_config: Dict):
+    def _actor_factory(self, actor_name: str, main_config: dict, component_config: dict):
         if 'max_buffer_size' in component_config.keys():
             return PusherActor(name=actor_name, report_model=component_config[COMPONENT_MODEL_KEY],
                                database=component_config[COMPONENT_DB_MANAGER_KEY],
                                max_size=component_config[COMPONENT_DB_MAX_BUFFER_SIZE])
 
         return PusherActor(name=actor_name, report_model=component_config[COMPONENT_MODEL_KEY],
                            database=component_config[COMPONENT_DB_MANAGER_KEY],
                            level_logger=logging.DEBUG if main_config[GENERAL_CONF_VERBOSE_KEY] else logging.INFO)
 
 
-class SimplePusherGenerator(SimpleGenerator):
+class SimplePusherGenerator(BaseGenerator):
     """
     Generate Simple Pusher actor and Simple Pusher start message from config
     """
 
     def __init__(self):
-        SimpleGenerator.__init__(self, 'output')
+        BaseGenerator.__init__(self, 'output')
 
-    def _actor_factory(self, actor_name: str, main_config: Dict, component_config: Dict):
+    def _actor_factory(self, actor_name: str, main_config: dict, component_config: dict):
         return SimplePusherActor(name=actor_name,
                                  number_of_reports_to_store=component_config['number_of_reports_to_store'])
 
 
 class ReportModifierGenerator:
     """
     Generate Report modifier list from config
     """
 
     def __init__(self):
         self.factory = {'libvirt_mapper': lambda config: LibvirtMapper(config['uri'], config['domain_regexp'])}
 
-    def generate(self, config: Dict):
+    def generate(self, config: dict):
         """
         Generate Report modifier list from config
         """
         report_modifier_list = []
         if 'report_modifier' not in config:
             return []
         for report_modifier_name in config['report_modifier'].keys():
```

### Comparing `powerapi-2.0.3/powerapi/cli/parser.py` & `powerapi-2.0.4/powerapi/cli/config_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,377 +24,305 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import getopt
 import sys
-from copy import deepcopy
+from typing import Any, Callable
 
-from powerapi.exception import PowerAPIException
+from powerapi.exception import AlreadyAddedArgumentException, UnknownArgException, \
+    MissingValueException, BadContextException, TooManyArgumentNamesException, NoNameSpecifiedForSubgroupException, \
+    SubgroupAlreadyExistException, SubgroupParserWithoutNameArgumentException, BadTypeException, \
+    MissingArgumentException, SameLengthArgumentNamesException
+from powerapi.utils.cli import find_longest_string_in_list, remove_first_characters, string_to_bool
 
 
-def _extract_minus(arg):
-    if len(arg) > 2:
-        return arg[2:]
-    return arg[1]
-
-
-def _cast_argument_value(arg_name, val, action):
-    if not action.is_flag:
-        try:
-            return action.arg_type(val)
-        except ValueError as exn:
-            raise BadTypeException(arg_name, action.arg_type) from exn
-    return val
-
-
-def _find_longest_name(names):
-    max_len = 0
-    longest_name = ''
-    for name in names:
-        if len(name) > max_len:
-            longest_name = name
-            max_len = len(name)
-    return longest_name
-
-
-#############
-# EXCEPTION #
-#############
-class ParserException(PowerAPIException):
-    """
-    Base Exception for parser error
-    """
-    def __init__(self, argument_name):
-        PowerAPIException.__init__(self)
-        self.argument_name = argument_name
-
-
-class NoNameSpecifiedForComponentException(ParserException):
-    """
-    Exception raised when attempting to parse substring thant describe a component which not contains the component name
-    """
-
-
-class ComponentAlreadyExistException(ParserException):
-    """
-    Exception raised when attempting to parse a substring to create a component with a name that already exist
-    """
-
-
-class SubParserWithoutNameArgumentException(PowerAPIException):
-    """
-    Exception raised when a subparser without argument name is added to a parser
-    """
-
-
-class TooManyArgumentNamesException(ParserException):
-    """
-    Exception raised when attemtping to add an argument with too much names
-
-    """
-    def __init__(self, argument_name):
-        ParserException.__init__(self, argument_name)
-
-
-class AlreadyAddedArgumentException(ParserException):
-    """
-    Exception raised when attempting to add an argument to a parser that already
-    have this argument
-
-    """
-    def __init__(self, argument_name):
-        ParserException.__init__(self, argument_name)
-        self.msg = 'Parser already contain an argument ' + argument_name
-
-
-class AlreadyAddedSubparserException(ParserException):
-    """
-    Exception raised when attempting to add an argument to a parser that already
-    have this argument
-
-    """
-    def __init__(self, argument_name):
-        ParserException.__init__(self, argument_name)
-        self.msg = 'Parser already contain SubParser with name ' + argument_name
-
-
-class MissingArgumentException(ParserException):
-    """
-    Exception raised when a mandatory argument is missing
-    """
-
-    def __init__(self, argument_name):
-        ParserException.__init__(self, argument_name)
-        self.msg = 'Argument ' + argument_name + ' is missing'
-
-
-class MissingValueException(ParserException):
-    """
-    Exception raised when an argument that require a value is caught without
-    its value
-
-    """
-    def __init__(self, argument_name):
-        ParserException.__init__(self, argument_name)
-        self.msg = 'Argument ' + argument_name + ' require a value'
-
-
-class UnknowArgException(ParserException):
-    """
-    Exception raised when the parser catch an argument that it can't handle
-
-    """
-    def __init__(self, argument_name):
-        ParserException.__init__(self, argument_name)
-        self.msg = 'Unknow argument ' + argument_name
-
-
-class BadTypeException(ParserException):
-    """
-    Exception raised when an argument is parsed with a value of an incorrect type
+def store_val(arg: str, val: Any, args: list, acc: dict):
     """
-    def __init__(self, argument_name, arg_type):
-        ParserException.__init__(self, argument_name)
-        self.msg = argument_name + " expect " + arg_type.__name__
-
-
-class BadContextException(ParserException):
-    """
-    Exception raised when the parser catch an argument that it can't handle in
-    the current context
-    """
-    def __init__(self, argument_name, context_list):
-        ParserException.__init__(self, argument_name)
-        self.context_list = context_list
-        self.msg = 'argument ' + argument_name + 'not used in the correct context\nUse it with the following arguments :'
-        for main_arg_name, context_name in context_list:
-            self.msg += '\n  --' + main_arg_name + ' ' + context_name
-
-
-#################
-# ACTION LAMBDA #
-#################
-def store_val(arg, val, args, acc):
-    """
-    lambda that store the value of the argument on the parser result
+    Action that stores the value of the argument on the parser result
 
     """
     if val == '':
         val = None
 
     acc[arg] = val
     return args, acc
 
 
-def store_true(arg, _, args, acc):
+def store_true(arg: str, _, args: list, acc: dict):
     """
-    lambda that store a True boolean value on the parser result
+    Action that stores a True boolean value on the parser result
 
     """
     acc[arg] = True
     return args, acc
 
 
-class ParserAction:
+class ConfigurationArgument:
     """
-    Action binded to an argument
+    Argument provided by a formula configuration.
     """
-    def __init__(self, name_list, is_flag, action, default_value, help_str, arg_type):
-        self.name_list = name_list
+
+    def __init__(self, names: list, is_flag: bool, default_value: Any, help_text: str, argument_type: type,
+                 is_mandatory: bool, action: Callable = None):
+        self.names = names
         self.is_flag = is_flag
-        self.action = action
         self.default_value = default_value
-        self.help_str = help_str
-        self.arg_type = arg_type
-
-
-class SubParserGroup:
-    """"""
-    def __init__(self, group_name, help_str=''):
-        self.group_name = group_name
-        self.help_str = help_str
-        self.subparsers = {}
-
-    def contains(self, name):
-        """"""
-        return name in self.subparsers
-
-    def add_subparser(self, name, subparser):
-        """"""
-        self.subparsers[name] = subparser
-
-    def get_subparser(self, name):
-        """"""
-        return self.subparsers[name]
+        self.help_text = help_text
+        self.type = argument_type
+        self.is_mandatory = is_mandatory
+        self.action = action
 
-    def __iter__(self):
-        return iter(self.subparsers.items())
+    def __eq__(self, arg):
+        names_ok = True
 
-    def get_help(self):
-        """
-        return help string
-        """
-        s = self.group_name + ' details :\n'
-        for subparser_name, subparser in self.subparsers.items():
-            s += '  --' + self.group_name + ' ' + subparser_name + ':\n'
-            s += subparser.get_help()
-            s += '\n'
+        for current_name in self.names:
+            names_ok = current_name in arg.names
 
-        return s
+        return names_ok and len(self.names) == len(arg.names) and self.is_flag == arg.is_flag and \
+            self.type == arg.type and self.default_value == arg.default_value and \
+            self.help_text == arg.help_text and self.is_mandatory == arg.is_mandatory
 
 
-class Parser:
+class BaseConfigParser:
     """"""
     def __init__(self):
-        self.actions = {}
-        self.default_values = {}
-        self.action_list = []
+        self.arguments = {}
 
-    def add_argument(self, *names, flag=False, action=store_val, default=None,
-                     help='', type=str):
+    def add_argument(self, *names, is_flag: bool = False, action: Callable = store_val, default_value: Any = None,
+                     help_text: str = '', argument_type: type = str, is_mandatory: bool = False):
         """add an optional argument to the parser that will activate an action
 
-        :param str *names: names of the optional argument that will be bind to
+        :param str names: names of the optional argument that will be bind to
                            the action (could be long or short name)
 
-        :param bool flag: True if the argument doesn't require to be followed
+        :param bool is_flag: True if the argument doesn't require to be followed
                            by a value
 
-        :param lambda action: action that will be executed when the argument is
+        :param Callable action: action that will be executed when the argument is
                               caught by the parser. the lambda take 4 parameters
                               (the name of the argument caught by the parser,
                               the value attached to this argument, the current
                               list of arguments that is parsed by the parser and
                               the parser result) and return a list of token and
                               a parser result(dict)
 
-        :param default: the default value attached to this argument
+        :param default_value: the default value attached to this argument
 
-        :param str help: string that describe the argument
+        :param str help_text: text that describe the argument
 
-        :param type type: type of the value that the argument must catch
+        :param type argument_type: type of the value that the argument must catch
+
+        :param bool is_mandatory: True if the argument is required
 
         :raise AlreadyAddedArgumentException: when attempting to add an
                                                argument that already have been
                                                added to this parser
 
         """
-        parser_action = ParserAction(list(names), flag, action, default, help, type)
-
         for name in names:
-            if name in self.actions:
+            if name in self.arguments:
                 raise AlreadyAddedArgumentException(name)
-            self.actions[name] = parser_action
-
-        action_name = _find_longest_name(names)
 
-        if default is not None:
-            self.default_values[action_name] = default
+        argument = ConfigurationArgument(names=list(names), is_flag=is_flag, action=action,
+                                         default_value=default_value, help_text=help_text,
+                                         argument_type=argument_type, is_mandatory=is_mandatory)
 
-        self.action_list.append(parser_action)
+        for name in names:
+            self.arguments[name] = argument
 
-    def _get_action_list_str(self, indent):
-        s = ''
-        for action in self.action_list:
-            s += indent + ', '.join(map(lambda x: '-' + x if len(x) == 1 else '--' + x, action.name_list))
-            s += ' : ' + action.help_str + '\n'
-        return s
+    def _get_default_arguments_values(self):
+        default_values = {}
+        for _, argument in self.arguments.items():
+            if argument.default_value is not None:
+                argument_name = find_longest_string_in_list(argument.names)
+                if argument_name not in default_values:
+                    default_values[argument_name] = argument.default_value
+
+        return default_values
+
+    def _get_arguments_str(self, indent: str) -> str:
+        already_added_argument = []
+        arguments_str_representation = ''
+        for _, argument in self.arguments.items():
+            if argument not in already_added_argument:
+                arguments_str_representation += indent + ', '.join(map(lambda x: '-' + x if len(x) == 1 else '--' + x, argument.names))
+                arguments_str_representation += ' : ' + argument.help_text + '\n'
+                already_added_argument.append(argument)
+        return arguments_str_representation
 
-    def _unknow_argument_behaviour(self, arg_name, val, args, acc):
+    def _unknown_argument_behaviour(self, arg_name: str, val: Any, args: list, acc: dict):
         raise NotImplementedError()
 
-    def _parse(self, args, acc):
+    def _parse(self, args: list, acc: dict) -> (list, dict):
 
-        while args != []:
+        while args:
             arg, val = args.pop(0)
-            if arg not in self.actions:
+            if arg not in self.arguments:
                 args.insert(0, (arg, val))
-                return self._unknow_argument_behaviour(arg, val, args, acc)
+                return self._unknown_argument_behaviour(arg, val, args, acc)
 
-            action = self.actions[arg]
+            argument = self.arguments[arg]
 
-            arg_long_name = _find_longest_name(action.name_list)
-            val = _cast_argument_value(arg_long_name, val, action)
+            arg_long_name = find_longest_string_in_list(argument.names)
+            val = cast_argument_value(arg_long_name, val, argument)
 
-            args, acc = action.action(arg_long_name, val, args, acc)
+            args, acc = argument.action(arg_long_name, val, args, acc)
 
         return args, acc
 
+    def _get_mandatory_arguments(self) -> list:
+        """
+        Return the list of mandatory arguments
+        """
+        mand_args = []
+        for _, argument in self.arguments.items():
+            if argument.is_mandatory and argument not in mand_args:
+                mand_args.append(argument)
+        return mand_args
+
+    def get_arguments(self):
+        """ Get the parser arguments """
+        return self.arguments
+
+    def validate(self, conf: dict) -> dict:
+        """
+            Check that mandatory arguments are present in the provided configuration.
+            It also defines default values if any for arguments that are not defined in the configuration
+        """
+        # Check that all the mandatory arguments are present
+        mandatory_args = self._get_mandatory_arguments()
+        for arg in mandatory_args:
+            is_present = False
+            for arg_name in arg.names:
+                if arg_name in conf:
+                    is_present = True
+                    break
+            if not is_present:
+                raise MissingArgumentException(str(arg.names))
+
+        # Define default values for no defined arguments if they are specified
+        for argument_name, argument_definition in self.arguments.items():
+            is_defined = False
+            for name in argument_definition.names:
+                if name in conf:
+                    is_defined = True
+                    break
+            if not is_defined and argument_definition.default_value is not None:
+                conf[argument_name] = argument_definition.default_value
+
+        return conf
+
+
+class SubgroupParserGroup:
+    """"""
+    def __init__(self, group_name: str, help_text: str = ''):
+        self.group_name = group_name
+        self.help_text = help_text
+        self.subparsers = {}
+
+    def contains(self, name: str):
+        """"""
+        return name in self.subparsers
+
+    def add_subgroup_parser(self, name: str, subparser: BaseConfigParser):
+        """"""
+        self.subparsers[name] = subparser
+
+    def get_subgroup_parser(self, name: str) -> BaseConfigParser:
+        """"""
+        return self.subparsers[name]
+
+    def __iter__(self):
+        return iter(self.subparsers.items())
+
+    def get_help(self) -> str:
+        """
+        return help string
+        """
+        help_str = self.group_name + ' details :\n'
+        for subparser_name, subparser in self.subparsers.items():
+            help_str += '  --' + self.group_name + ' ' + subparser_name + ':\n'
+            help_str += subparser.get_help()
+            help_str += '\n'
+
+        return help_str
+
 
-class ComponentSubParser(Parser):
+class SubgroupConfigParser(BaseConfigParser):
     """"""
-    def __init__(self, name):
-        Parser.__init__(self)
+    def __init__(self, name: str):
+        BaseConfigParser.__init__(self)
         self.name = name
 
-    def _unknow_argument_behaviour(self, arg_name, val, args, acc):
+    def _unknown_argument_behaviour(self, arg_name: str, val: Any, args: list,
+                                    acc: dict):
         return args, acc
 
-    def subparse(self, token_list):
+    def parse(self, token_list: list) -> (list, dict):
         """
-        Parse the given token list until an unknow argument is caught
+        Parse the given token list until an unknown argument is caught
 
         :param list token_list: the token list currently parsed
 
         :result: the current result of the parser
 
         :return (list, dict): a tuple containing the token list without the
                               parsed argument and the result of the parsing
 
         """
-        local_result = deepcopy(self.default_values)
-        if token_list == []:
+        local_result = self._get_default_arguments_values()
+        if not token_list:
             return token_list, local_result
 
         return self._parse(token_list, local_result)
 
-    def get_help(self):
+    def get_help(self) -> str:
         """
         return help string
         """
-        return self._get_action_list_str('    ')
+        return self._get_arguments_str('    ')
 
 
-class MainParser(Parser):
+class RootConfigParser(BaseConfigParser):
     """"""
-    def __init__(self, help_arg=True):
+    def __init__(self, help_arg: bool = True):
         """
         :param bool help_arg: if True, add a -h/--help argument that display help
         """
-        Parser.__init__(self)
+        BaseConfigParser.__init__(self)
         self.short_arg = ''
         self.long_arg = []
-        self.subparsers_group = {}
+        self.subgroup_parsers = {}
 
         self.help_arg = help_arg
         if help_arg:
-            self.add_argument('h', 'help', flag=True, action=None)
+            self.add_argument('h', 'help', is_flag=True, argument_type=bool)
 
     def get_help(self):
         """
         return help string
         """
         s = 'main arguments:\n'
-        s += self._get_action_list_str('  ')
+        s += self._get_arguments_str('  ')
         s += '\n'
 
-        for _, subparser_group in self.subparsers_group.items():
+        for _, subparser_group in self.subgroup_parsers.items():
             s += subparser_group.get_help()
 
         return s
 
-    def parse(self, args):
+    def parse(self, args: list) -> dict:
         """
-        :param str args: string that contains the arguments and their values
+        :param list args: list that contains the arguments and their values
 
-        :return dict:
+        :return dict: Dictionary that contains the arguments with its associated values extracted from args
 
-        :raise UnknowArgException: when the parser catch catch an argument that
+        :raise UnknownArgException: when the parser catch an argument that
                                    this parser can't handle
 
         :raise BadContextException: when an argument that the parser can't
                                     handle in the current context is caught
 
         :raise MissingValueException: when an argument that require a value is
                                       caught without its value
@@ -402,138 +330,141 @@
         :raise BadTypeException: when an argument is parsed with a value of an
                                  incorrect type
         """
         try:
             args, _ = getopt.getopt(args, self.short_arg, self.long_arg)
         except getopt.GetoptError as exn:
             if 'recognized' in exn.msg:
-                raise UnknowArgException(exn.opt) from exn
+                raise UnknownArgException(exn.opt) from exn
             elif 'requires' in exn.msg:
                 raise MissingValueException(exn.opt) from exn
 
-        # retirer les moins
-        args = list(map(lambda x: (_extract_minus(x[0]), x[1]), args))
+        # remove minus
+        args = list(map(lambda x: (remove_first_characters(x[0]), x[1]), args))
 
         # verify if help argument exists in args
-
         if self.help_arg:
             for arg_name, _ in args:
                 if arg_name in ('h', 'help'):
                     print(self.get_help())
                     sys.exit(0)
 
-        acc = deepcopy(self.default_values)
+        acc = self._get_default_arguments_values()
 
         args, acc = self._parse(args, acc)
 
         return acc
 
-    def _unknow_argument_behaviour(self, arg_name, val, args, acc):
+    def parse_config_dict(self, conf: dict) -> dict:
+        """
+        Return a configuration dict that has all the arguments' names in the long form.
+        If an argument does not exist, a UnknownArgException is raised
+        """
+        conf_with_long_names = {}
+
+        for current_argument_name in conf:
+            if current_argument_name not in self.arguments:
+                raise UnknownArgException(current_argument_name)
+            current_argument = self.arguments[current_argument_name]
+            longest_argument_name = find_longest_string_in_list(current_argument.names)
+
+            conf_with_long_names[longest_argument_name] = conf[current_argument_name]
+
+        return conf_with_long_names
+
+    def _unknown_argument_behaviour(self, arg_name: str, val: Any, args: list,
+                                    acc: dict):
         good_contexts = []
-        for main_arg_name, subparser_group in self.subparsers_group.items():
+        for main_arg_name, subparser_group in self.subgroup_parsers.items():
             for subparser_name, subparser in subparser_group:
-                if arg_name in subparser.actions:
+                if arg_name in subparser.arguments:
                     good_contexts.append((main_arg_name, subparser_name))
         raise BadContextException(arg_name, good_contexts)
 
-    def _add_argument_names(self, names, is_flag):
+    def _add_argument_names(self, names: list, is_flag: bool):
 
         if len(names) > 2:
             raise TooManyArgumentNamesException(names[2])
 
         if len(names) > 1 and len(names[0]) == len(names[1]):
-            raise TooManyArgumentNamesException(names[1])
+            raise SameLengthArgumentNamesException(names[1])
 
-        def gen_name(name):
-            if len(name) == 1:
-                return name + ('' if is_flag else ':')
-            return name + ('' if is_flag else '=')
+        def add_suffix_to_argument_name_if_required(current_name):
+            if len(current_name) == 1:
+                return current_name + ('' if is_flag else ':')
+            return current_name + ('' if is_flag else '=')
 
         for name in names:
             if len(name) == 1:
-                self.short_arg += gen_name(name)
+                self.short_arg += add_suffix_to_argument_name_if_required(name)
             else:
-                self.long_arg.append(gen_name(name))
-
-    def add_argument(self, *names, flag=False, action=store_val, default=None, help='', type=str):
-        Parser.add_argument(self, *names, flag=flag, action=action, default=default, help=help, type=type)
-        self._add_argument_names(names, flag)
-
-    def add_component_subparser(self, component_type, subparser, help_str=''):
-        """
-        Add a subparser that will be used by the argument *component_name*
+                self.long_arg.append(add_suffix_to_argument_name_if_required(name))
 
-        :param str component_type:
-        :param ComponentSubParser subparser:
+    def add_argument(self, *names, is_flag: bool = False, action: Callable = store_val, default_value: Any = None,
+                     help_text: str = '', argument_type: type = str, is_mandatory: bool = False):
+        self._add_argument_names(list(names), is_flag)
+        BaseConfigParser.add_argument(self, *names, is_flag=is_flag, action=action, default_value=default_value,
+                                      help_text=help_text, argument_type=argument_type, is_mandatory=is_mandatory)
+
+    def add_subgroup_parser(self, subgroup_type: str, subgroup_parser: SubgroupConfigParser, help_text: str = ''):
+        """
+        Add a subparser that will be used by the argument *group_name*
+        The group must contain a name action
+        :param str subgroup_type: the group type
+        :param SubgroupConfigParser subgroup_parser: The subgroup parser
+        :param str help_text: help text related to the parser
 
         :raise AlreadyAddedArgumentException: when attempting to add an
                                               argument that already have been
                                               added to this parser
         """
-        def _action(arg, val, args, acc):
+        def _action(arg: str, val: Any, args: list, acc: dict):
             if arg not in acc:
                 acc[arg] = {}
 
-            subparser = self.subparsers_group[arg].get_subparser(val)
-            args, subparse_result = subparser.subparse(args)
+            parser = self.subgroup_parsers[arg].get_subgroup_parser(val)
+            args, parse_result = parser.parse(args)
 
-            acc[arg][subparser.name] = subparse_result
-            # acc[arg] = subparse_result
-            return args, acc
+            if 'name' not in parse_result:
+                raise NoNameSpecifiedForSubgroupException(subgroup_type)
 
-        if component_type not in self.subparsers_group:
-            self.subparsers_group[component_type] = SubParserGroup(component_type, help_str=help_str)
-            self.add_argument(component_type, action=_action, help=help_str)
-        else:
-            if self.subparsers_group[component_type].contains(subparser.name):
-                raise AlreadyAddedArgumentException(subparser.name)
+            subgroup_name = parse_result['name']
+            del parse_result['name']
 
-        self.subparsers_group[component_type].add_subparser(subparser.name, subparser)
+            if subgroup_name in acc[arg]:
+                raise SubgroupAlreadyExistException(subgroup_name)
 
-        for action_name, action in subparser.actions.items():
-            self._add_argument_names([action_name], action.is_flag)
-
-    def add_actor_subparser(self, component_type, subparser, help_str=''):
-        """
-        Add a subparser that will be used by the argument *component_name*
-        The component must contain a name action
-        :param str component_type:
-        :param ComponentSubParser subparser:
-
-        :raise AlreadyAddedArgumentException: when attempting to add an
-                                              argument that already have been
-                                              added to this parser
-        """
-        def _action(arg, val, args, acc):
-            if arg not in acc:
-                acc[arg] = {}
-
-            subparser = self.subparsers_group[arg].get_subparser(val)
-            args, subparse_result = subparser.subparse(args)
-
-            if 'name' not in subparse_result:
-                raise NoNameSpecifiedForComponentException(component_type)
-
-            component_name = subparse_result['name']
-            del subparse_result['name']
-
-            if component_name in acc[arg]:
-                raise ComponentAlreadyExistException(component_name)
-
-            acc[arg][component_name] = subparse_result
-            acc[arg][component_name]['type'] = subparser.name
+            acc[arg][subgroup_name] = parse_result
+            acc[arg][subgroup_name]['type'] = parser.name
 
             return args, acc
 
-        if 'name' not in subparser.actions:
-            raise SubParserWithoutNameArgumentException()
-        if component_type not in self.subparsers_group:
-            self.subparsers_group[component_type] = SubParserGroup(component_type, help_str=help_str)
-            self.add_argument(component_type, action=_action, help=help_str)
+        if 'name' not in subgroup_parser.arguments:
+            raise SubgroupParserWithoutNameArgumentException()
+        if subgroup_type not in self.subgroup_parsers:
+            self.subgroup_parsers[subgroup_type] = SubgroupParserGroup(subgroup_type, help_text=help_text)
+            self.add_argument(subgroup_type, action=_action, help_text=help_text)
         else:
-            if self.subparsers_group[component_type].contains(subparser.name):
-                raise AlreadyAddedArgumentException(subparser.name)
+            if self.subgroup_parsers[subgroup_type].contains(subgroup_parser.name):
+                raise AlreadyAddedArgumentException(subgroup_parser.name)
 
-        self.subparsers_group[component_type].add_subparser(subparser.name, subparser)
+        self.subgroup_parsers[subgroup_type].add_subgroup_parser(subgroup_parser.name, subgroup_parser)
 
-        for action_name, action in subparser.actions.items():
+        for action_name, action in subgroup_parser.arguments.items():
             self._add_argument_names([action_name], action.is_flag)
+
+
+def cast_argument_value(arg_name: str, val: Any, argument: ConfigurationArgument):
+    """
+    Cast the given value to argument.type
+    :param str arg_name: The argument name
+    :param Any val: Current value given to the argument
+    :argument ConfigurationAgument argument: The argument definition
+    """
+    if not argument.is_flag:
+        try:
+            if argument.type is bool and isinstance(val, str):
+                return string_to_bool(val)
+            return argument.type(val)
+        except ValueError as exn:
+            raise BadTypeException(arg_name, argument.type) from exn
+    return val
```

### Comparing `powerapi-2.0.3/powerapi/cli/tools.py` & `powerapi-2.0.4/powerapi/cli/common_cli_parsing_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,395 +25,394 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import sys
 
-from powerapi.cli.config_parser import MainConfigParser, SubConfigParser
-from powerapi.cli.parser import store_true
-from powerapi.cli.parser import MissingValueException
-from powerapi.cli.parser import BadTypeException, BadContextException
-from powerapi.cli.parser import UnknowArgException
+from powerapi.cli.parsing_manager import RootConfigParsingManager, SubgroupConfigParsingManager
+from powerapi.cli.config_parser import store_true
+from powerapi.cli.config_parser import MissingValueException
+from powerapi.exception import BadTypeException, BadContextException, UnknownArgException
 
 
 def extract_file_names(arg, val, args, acc):
     """
     action used to convert string from --files parameter into a list of file name
     """
     acc[arg] = val.split(",")
     return args, acc
 
 
-class CommonCLIParser(MainConfigParser):
+class CommonCLIParsingManager(RootConfigParsingManager):
     """
     PowerAPI basic config parser
     """
 
     def __init__(self):
-        MainConfigParser.__init__(self)
+        RootConfigParsingManager.__init__(self)
 
-        self.add_argument(
+        self.add_argument_to_cli_parser(
             "v",
             "verbose",
-            flag=True,
+            is_flag=True,
             action=store_true,
-            default=False,
-            help="enable verbose mode",
+            default_value=False,
+            help_text="enable verbose mode",
         )
-        self.add_argument(
+        self.add_argument_to_cli_parser(
             "s",
             "stream",
-            flag=True,
+            is_flag=True,
             action=store_true,
-            default=False,
-            help="enable stream mode",
+            default_value=False,
+            help_text="enable stream mode",
         )
 
-        subparser_libvirt_mapper_modifier = SubConfigParser("libvirt_mapper")
-        subparser_libvirt_mapper_modifier.add_argument(
-            "u", "uri", help="libvirt daemon uri", default=""
+        subparser_libvirt_mapper_modifier = SubgroupConfigParsingManager("libvirt_mapper")
+        subparser_libvirt_mapper_modifier.add_argument_to_cli_parser(
+            "u", "uri", help_text="libvirt daemon uri", default_value=""
         )
-        subparser_libvirt_mapper_modifier.add_argument(
+        subparser_libvirt_mapper_modifier.add_argument_to_cli_parser(
             "d",
             "domain_regexp",
-            help="regexp used to extract domain from cgroup string",
+            help_text="regexp used to extract domain from cgroup string",
         )
-        subparser_libvirt_mapper_modifier.add_argument("n", "name", help="")
-        self.add_subparser(
+        subparser_libvirt_mapper_modifier.add_argument_to_cli_parser("n", "name", help_text="")
+        self.add_subgroup_parser(
             "report_modifier",
             subparser_libvirt_mapper_modifier,
-            help="Specify a report modifier to change input report values : --report_modifier ARG1 ARG2 ...",
+            help_text="Specify a report modifier to change input report values : --report_modifier ARG1 ARG2 ...",
         )
 
-        subparser_mongo_input = SubConfigParser("mongodb")
-        subparser_mongo_input.add_argument("u", "uri", help="specify MongoDB uri")
-        subparser_mongo_input.add_argument(
+        subparser_mongo_input = SubgroupConfigParsingManager("mongodb")
+        subparser_mongo_input.add_argument_to_cli_parser("u", "uri", help_text="specify MongoDB uri")
+        subparser_mongo_input.add_argument_to_cli_parser(
             "d",
             "db",
-            help="specify MongoDB database name",
+            help_text="specify MongoDB database name",
         )
-        subparser_mongo_input.add_argument(
-            "c", "collection", help="specify MongoDB database collection"
+        subparser_mongo_input.add_argument_to_cli_parser(
+            "c", "collection", help_text="specify MongoDB database collection"
         )
-        subparser_mongo_input.add_argument(
-            "n", "name", help="specify puller name", default="puller_mongodb"
+        subparser_mongo_input.add_argument_to_cli_parser(
+            "n", "name", help_text="specify puller name", default_value="puller_mongodb"
         )
-        subparser_mongo_input.add_argument(
+        subparser_mongo_input.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be stored in the database",
-            default="HWPCReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="HWPCReport",
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "input",
             subparser_mongo_input,
-            help="specify a database input : --db_input database_name ARG1 ARG2 ... ",
+            help_text="specify a database input : --db_input database_name ARG1 ARG2 ... ",
         )
 
-        subparser_socket_input = SubConfigParser("socket")
-        subparser_socket_input.add_argument(
-            "p", "port", type=int, help="specify port to bind the socket"
+        subparser_socket_input = SubgroupConfigParsingManager("socket")
+        subparser_socket_input.add_argument_to_cli_parser(
+            "p", "port", argument_type=int, help_text="specify port to bind the socket"
         )
-        subparser_socket_input.add_argument(
-            "n", "name", help="specify puller name", default="puller_socket"
+        subparser_socket_input.add_argument_to_cli_parser(
+            "n", "name", help_text="specify puller name", default_value="puller_socket"
         )
-        subparser_socket_input.add_argument(
+        subparser_socket_input.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be sent through the socket",
-            default="HWPCReport",
+            help_text="specify data type that will be sent through the socket",
+            default_value="HWPCReport",
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "input",
             subparser_socket_input,
-            help="specify a database input : --db_input database_name ARG1 ARG2 ... ",
+            help_text="specify a database input : --db_input database_name ARG1 ARG2 ... ",
         )
 
-        subparser_csv_input = SubConfigParser("csv")
-        subparser_csv_input.add_argument(
+        subparser_csv_input = SubgroupConfigParsingManager("csv")
+        subparser_csv_input.add_argument_to_cli_parser(
             "f",
             "files",
-            help="specify input csv files with this format : file1,file2,file3",
+            help_text="specify input csv files with this format : file1,file2,file3",
             action=extract_file_names,
-            default=[],
+            default_value=[],
         )
-        subparser_csv_input.add_argument(
+        subparser_csv_input.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be storen in the database",
-            default="HWPCReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="HWPCReport",
         )
-        subparser_csv_input.add_argument(
-            "n", "name", help="specify puller name", default="puller_csv"
+        subparser_csv_input.add_argument_to_cli_parser(
+            "n", "name", help_text="specify puller name", default_value="puller_csv"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "input",
             subparser_csv_input,
-            help="specify a database input : --db_input database_name ARG1 ARG2 ... ",
+            help_text="specify a database input : --db_input database_name ARG1 ARG2 ... ",
         )
 
-        subparser_file_input = SubConfigParser("filedb")
-        subparser_file_input.add_argument(
+        subparser_file_input = SubgroupConfigParsingManager("filedb")
+        subparser_file_input.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be stored in the database",
-            default="HWPCReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="HWPCReport",
         )
-        subparser_file_input.add_argument("f", "filename", help="specify file name")
-        subparser_file_input.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_filedb"
+        subparser_file_input.add_argument_to_cli_parser("f", "filename", help_text="specify file name")
+        subparser_file_input.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_filedb"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "input",
             subparser_file_input,
-            help="specify a database input : --db_input database_name ARG1 ARG2 ... ",
+            help_text="specify a database input : --db_input database_name ARG1 ARG2 ... ",
         )
 
-        subparser_file_output = SubConfigParser("filedb")
-        subparser_file_output.add_argument(
+        subparser_file_output = SubgroupConfigParsingManager("filedb")
+        subparser_file_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be stored in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
-        subparser_file_output.add_argument("f", "filename", help="specify file name")
-        subparser_file_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_filedb"
+        subparser_file_output.add_argument_to_cli_parser("f", "filename", help_text="specify file name")
+        subparser_file_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_filedb"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_file_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ...",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ...",
         )
 
-        subparser_virtiofs_output = SubConfigParser("virtiofs")
-        help = "regexp used to extract vm name from report."
-        help += "The regexp must match the name of the target in the HWPC-report and a group must"
-        subparser_virtiofs_output.add_argument("r", "vm_name_regexp", help=help)
-        subparser_virtiofs_output.add_argument(
+        subparser_virtiofs_output = SubgroupConfigParsingManager("virtiofs")
+        help_text = "regexp used to extract vm name from report."
+        help_text += "The regexp must match the name of the target in the HWPC-report and a group must"
+        subparser_virtiofs_output.add_argument_to_cli_parser("r", "vm_name_regexp", help_text=help_text)
+        subparser_virtiofs_output.add_argument_to_cli_parser(
             "d",
             "root_directory_name",
-            help="directory where VM directory will be stored",
+            help_text="directory where VM directory will be stored",
         )
-        subparser_virtiofs_output.add_argument(
+        subparser_virtiofs_output.add_argument_to_cli_parser(
             "p",
             "vm_directory_name_prefix",
-            help="first part of the VM directory name",
-            default="",
+            help_text="first part of the VM directory name",
+            default_value="",
         )
-        subparser_virtiofs_output.add_argument(
+        subparser_virtiofs_output.add_argument_to_cli_parser(
             "s",
             "vm_directory_name_suffix",
-            help="last part of the VM directory name",
-            default="",
+            help_text="last part of the VM directory name",
+            default_value="",
         )
-        subparser_virtiofs_output.add_argument(
+        subparser_virtiofs_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be storen in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
-        subparser_virtiofs_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_virtiofs"
+        subparser_virtiofs_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_virtiofs"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_virtiofs_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ...",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ...",
         )
 
-        subparser_mongo_output = SubConfigParser("mongodb")
-        subparser_mongo_output.add_argument("u", "uri", help="specify MongoDB uri")
-        subparser_mongo_output.add_argument(
-            "d", "db", help="specify MongoDB database name"
+        subparser_mongo_output = SubgroupConfigParsingManager("mongodb")
+        subparser_mongo_output.add_argument_to_cli_parser("u", "uri", help_text="specify MongoDB uri")
+        subparser_mongo_output.add_argument_to_cli_parser(
+            "d", "db", help_text="specify MongoDB database name"
         )
-        subparser_mongo_output.add_argument(
-            "c", "collection", help="specify MongoDB database collection"
+        subparser_mongo_output.add_argument_to_cli_parser(
+            "c", "collection", help_text="specify MongoDB database collection"
         )
 
-        subparser_mongo_output.add_argument(
+        subparser_mongo_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be stored in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
-        subparser_mongo_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_mongodb"
+        subparser_mongo_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_mongodb"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_mongo_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ...",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ...",
         )
 
-        subparser_prom_output = SubConfigParser("prom")
-        subparser_prom_output.add_argument("t", "tags", help="specify report tags")
-        subparser_prom_output.add_argument("u", "uri", help="specify server uri")
-        subparser_prom_output.add_argument(
-            "p", "port", help="specify server port", type=int
+        subparser_prom_output = SubgroupConfigParsingManager("prom")
+        subparser_prom_output.add_argument_to_cli_parser("t", "tags", help_text="specify report tags")
+        subparser_prom_output.add_argument_to_cli_parser("u", "uri", help_text="specify server uri")
+        subparser_prom_output.add_argument_to_cli_parser(
+            "p", "port", help_text="specify server port", argument_type=int
         )
-        subparser_prom_output.add_argument(
-            "M", "metric_name", help="specify metric name"
+        subparser_prom_output.add_argument_to_cli_parser(
+            "M", "metric_name", help_text="specify metric name"
         )
-        subparser_prom_output.add_argument(
+        subparser_prom_output.add_argument_to_cli_parser(
             "d",
             "metric_description",
-            help="specify metric description",
-            default="energy consumption",
+            help_text="specify metric description",
+            default_value="energy consumption",
         )
-        help = "specify number of second for the value must be aggregated before compute statistics on them"
-        subparser_prom_output.add_argument(
-            "A", "aggregation_period", help=help, default=15, type=int
+        help_text = "specify number of second for the value must be aggregated before compute statistics on them"
+        subparser_prom_output.add_argument_to_cli_parser(
+            "A", "aggregation_period", help_text=help_text, default_value=15, argument_type=int
         )
 
-        subparser_prom_output.add_argument(
+        subparser_prom_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be storen in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
-        subparser_prom_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_prom"
+        subparser_prom_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_prom"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_prom_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ...",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ...",
         )
 
-        subparser_direct_prom_output = SubConfigParser("direct_prom")
-        subparser_direct_prom_output.add_argument(
-            "t", "tags", help="specify report tags"
+        subparser_direct_prom_output = SubgroupConfigParsingManager("direct_prom")
+        subparser_direct_prom_output.add_argument_to_cli_parser(
+            "t", "tags", help_text="specify report tags"
         )
-        subparser_direct_prom_output.add_argument("a", "uri", help="specify server uri")
-        subparser_direct_prom_output.add_argument(
-            "p", "port", help="specify server port", type=int
+        subparser_direct_prom_output.add_argument_to_cli_parser("a", "uri", help_text="specify server uri")
+        subparser_direct_prom_output.add_argument_to_cli_parser(
+            "p", "port", help_text="specify server port", argument_type=int
         )
-        subparser_direct_prom_output.add_argument(
-            "M", "metric_name", help="speify metric name"
+        subparser_direct_prom_output.add_argument_to_cli_parser(
+            "M", "metric_name", help_text="specify metric name"
         )
-        subparser_direct_prom_output.add_argument(
+        subparser_direct_prom_output.add_argument_to_cli_parser(
             "d",
             "metric_description",
-            help="specify metric description",
-            default="energy consumption",
+            help_text="specify metric description",
+            default_value="energy consumption",
         )
-        subparser_direct_prom_output.add_argument(
+        subparser_direct_prom_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be storen in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
-        subparser_direct_prom_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_prom"
+        subparser_direct_prom_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_prom"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_direct_prom_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ...",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ...",
         )
 
-        subparser_csv_output = SubConfigParser("csv")
-        subparser_csv_output.add_argument(
+        subparser_csv_output = SubgroupConfigParsingManager("csv")
+        subparser_csv_output.add_argument_to_cli_parser(
             "d",
             "directory",
-            help="specify directory where where output  csv files will be writen",
+            help_text="specify directory where where output  csv files will be writen",
         )
-        subparser_csv_output.add_argument(
+        subparser_csv_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be stored in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
 
-        subparser_csv_output.add_argument("t", "tags", help="specify report tags")
-        subparser_csv_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_csv"
+        subparser_csv_output.add_argument_to_cli_parser("t", "tags", help_text="specify report tags")
+        subparser_csv_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_csv"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_csv_output,
-            help="specify a database outpout : --db_output database_name ARG1 ARG2 ... ",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ... ",
         )
 
-        subparser_influx_output = SubConfigParser("influxdb")
-        subparser_influx_output.add_argument("u", "uri", help="specify InfluxDB uri")
-        subparser_influx_output.add_argument("t", "tags", help="specify report tags")
-        subparser_influx_output.add_argument(
-            "d", "db", help="specify InfluxDB database name"
+        subparser_influx_output = SubgroupConfigParsingManager("influxdb")
+        subparser_influx_output.add_argument_to_cli_parser("u", "uri", help_text="specify InfluxDB uri")
+        subparser_influx_output.add_argument_to_cli_parser("t", "tags", help_text="specify report tags")
+        subparser_influx_output.add_argument_to_cli_parser(
+            "d", "db", help_text="specify InfluxDB database name"
         )
-        subparser_influx_output.add_argument(
-            "p", "port", help="specify InfluxDB connection port", type=int
+        subparser_influx_output.add_argument_to_cli_parser(
+            "p", "port", help_text="specify InfluxDB connection port", argument_type=int
         )
-        subparser_influx_output.add_argument(
+        subparser_influx_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be storen in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
-        subparser_influx_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_influxdb"
+        subparser_influx_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_influxdb"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_influx_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ... ",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ... ",
         )
 
-        subparser_opentsdb_output = SubConfigParser("opentsdb")
-        subparser_opentsdb_output.add_argument("u", "uri", help="specify openTSDB host")
-        subparser_opentsdb_output.add_argument(
-            "p", "port", help="specify openTSDB connection port", type=int
+        subparser_opentsdb_output = SubgroupConfigParsingManager("opentsdb")
+        subparser_opentsdb_output.add_argument_to_cli_parser("u", "uri", help_text="specify openTSDB host")
+        subparser_opentsdb_output.add_argument_to_cli_parser(
+            "p", "port", help_text="specify openTSDB connection port", argument_type=int
         )
-        subparser_opentsdb_output.add_argument(
-            "metric_name", help="specify metric name"
+        subparser_opentsdb_output.add_argument_to_cli_parser(
+            "metric_name", help_text="specify metric name"
         )
 
-        subparser_opentsdb_output.add_argument(
+        subparser_opentsdb_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be stored in the database",
-            default="PowerReport",
+            help_text="specify data type that will be stored in the database",
+            default_value="PowerReport",
         )
-        subparser_opentsdb_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_opentsdb"
+        subparser_opentsdb_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_opentsdb"
         )
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_opentsdb_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ... ",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ... ",
         )
 
-        subparser_influx2_output = SubConfigParser("influxdb2")
-        subparser_influx2_output.add_argument("u", "uri", help="specify InfluxDB uri")
-        subparser_influx2_output.add_argument("t", "tags", help="specify report tags")
-        subparser_influx2_output.add_argument("k", "token", help="specify token for accessing the database")
-        subparser_influx2_output.add_argument("g", "org", help="specify organisation for accessing the database")
+        subparser_influx2_output = SubgroupConfigParsingManager("influxdb2")
+        subparser_influx2_output.add_argument_to_cli_parser("u", "uri", help_text="specify InfluxDB uri")
+        subparser_influx2_output.add_argument_to_cli_parser("t", "tags", help_text="specify report tags")
+        subparser_influx2_output.add_argument_to_cli_parser("k", "token", help_text="specify token for accessing the database")
+        subparser_influx2_output.add_argument_to_cli_parser("g", "org", help_text="specify organisation for accessing the database")
 
-        subparser_influx2_output.add_argument(
-            "d", "db", help="specify InfluxDB database name"
+        subparser_influx2_output.add_argument_to_cli_parser(
+            "d", "db", help_text="specify InfluxDB database name"
         )
-        subparser_influx2_output.add_argument(
-            "p", "port", help="specify InfluxDB connection port", type=int
+        subparser_influx2_output.add_argument_to_cli_parser(
+            "p", "port", help_text="specify InfluxDB connection port", argument_type=int
         )
-        subparser_influx2_output.add_argument(
+        subparser_influx2_output.add_argument_to_cli_parser(
             "m",
             "model",
-            help="specify data type that will be store in the database",
-            default="PowerReport",
+            help_text="specify data type that will be store in the database",
+            default_value="PowerReport",
         )
-        subparser_influx2_output.add_argument(
-            "n", "name", help="specify pusher name", default="pusher_influxdb2"
+        subparser_influx2_output.add_argument_to_cli_parser(
+            "n", "name", help_text="specify pusher name", default_value="pusher_influxdb2"
         )
 
-        self.add_subparser(
+        self.add_subgroup_parser(
             "output",
             subparser_influx2_output,
-            help="specify a database output : --db_output database_name ARG1 ARG2 ... ",
+            help_text="specify a database output : --db_output database_name ARG1 ARG2 ... ",
         )
 
     def parse_argv(self):
         """ """
         try:
             return self.parse(sys.argv[1:])
 
@@ -421,16 +420,16 @@
             msg = "CLI error : argument " + exn.argument_name + " : expect a value"
             print(msg, file=sys.stderr)
 
         except BadTypeException as exn:
             msg = "Configuration error : " + exn.msg
             print(msg, file=sys.stderr)
 
-        except UnknowArgException as exn:
-            msg = "CLI error : unknow argument " + exn.argument_name
+        except UnknownArgException as exn:
+            msg = "CLI error : unknown argument " + exn.argument_name
             print(msg, file=sys.stderr)
 
         except BadContextException as exn:
             msg = "CLI error : argument " + exn.argument_name
             msg += " not used in the correct context\nUse it with the following arguments :"
             for main_arg_name, context_name in exn.context_list:
                 msg += "\n  --" + main_arg_name + " " + context_name
```

### Comparing `powerapi-2.0.3/powerapi/database/__init__.py` & `powerapi-2.0.4/powerapi/database/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from powerapi.database.base_db import BaseDB, IterDB, DBError
 from powerapi.database.csvdb import CsvDB, CsvBadFilePathError
 from powerapi.database.csvdb import CsvBadCommonKeysError, HeaderAreNotTheSameError
 from powerapi.database.mongodb import MongoDB, MongoBadDBError
 from powerapi.database.opentsdb import OpenTSDB, CantConnectToOpenTSDBException
 from powerapi.database.influxdb import InfluxDB, CantConnectToInfluxDBException
+from powerapi.database.influxdb2 import InfluxDB2
 from powerapi.database.prometheus_db import PrometheusDB
 from powerapi.database.virtiofs_db import VirtioFSDB
 from powerapi.database.direct_prometheus_db import DirectPrometheusDB
 from powerapi.database.socket_db import SocketDB
 from powerapi.database.file_db import FileDB
```

### Comparing `powerapi-2.0.3/powerapi/database/base_db.py` & `powerapi-2.0.4/powerapi/database/base_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/csvdb.py` & `powerapi-2.0.4/powerapi/database/csvdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/direct_prometheus_db.py` & `powerapi-2.0.4/powerapi/database/direct_prometheus_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/file_db.py` & `powerapi-2.0.4/powerapi/database/file_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/influxdb.py` & `powerapi-2.0.4/powerapi/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/influxdb2.py` & `powerapi-2.0.4/powerapi/database/influxdb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,26 +33,27 @@
 try:
     from influxdb_client import InfluxDBClient, WriteOptions
     from influxdb_client.client.write_api import SYNCHRONOUS
 except ImportError:
     logging.getLogger().info("influx-client2 is not installed.")
 
 from powerapi.report import Report
+from powerapi.exception import MissingArgumentException
 from .base_db import BaseDB, DBError
 
 
 class CantConnectToInfluxDBException(DBError):
     """
         Exception raised to notify that connection to the influx database is impossible
     """
 
 
 class InfluxDB2(BaseDB):
     """
-        InfluxDB2 class herited from BaseDB
+        InfluxDB2 class is a subclass of BaseDB
 
         Allow to handle a InfluxDB database in reading or writing.
     """
 
     def __init__(self, report_type: Type[Report], url: str, org: str, bucket_name: str, token: str, tags: List[str],
                  port=None):
         """
@@ -68,14 +69,16 @@
         BaseDB.__init__(self, report_type)
         self.uri = url
 
         # We check if the URL has the port or not
         parsed_url = urlparse(url)
         if parsed_url.port is None and port is not None:
             self.uri += ':' + port.__str__()
+        elif parsed_url.port is None and port is None:
+            raise MissingArgumentException('port')
 
         self.org = org
         self.token = token
         self.bucket_name = bucket_name
         self.tags = tags
 
         self.client = None
```

### Comparing `powerapi-2.0.3/powerapi/database/mongodb.py` & `powerapi-2.0.4/powerapi/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/opentsdb.py` & `powerapi-2.0.4/powerapi/database/opentsdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/prometheus_db.py` & `powerapi-2.0.4/powerapi/database/prometheus_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/socket_db.py` & `powerapi-2.0.4/powerapi/database/socket_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/database/virtiofs_db.py` & `powerapi-2.0.4/powerapi/database/virtiofs_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatch_rule/__init__.py` & `powerapi-2.0.4/powerapi/dispatch_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatch_rule/dispatch_rule.py` & `powerapi-2.0.4/powerapi/dispatch_rule/dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatch_rule/hwpc_dispatch_rule.py` & `powerapi-2.0.4/powerapi/dispatch_rule/hwpc_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatch_rule/power_dispatch_rule.py` & `powerapi-2.0.4/powerapi/dispatch_rule/power_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatch_rule/procfs_dispatch_rule.py` & `powerapi-2.0.4/powerapi/dispatch_rule/procfs_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatch_rule/simple_dispatch_rule.py` & `powerapi-2.0.4/powerapi/dispatch_rule/simple_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/__init__.py` & `powerapi-2.0.4/powerapi/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/blocking_detector.py` & `powerapi-2.0.4/powerapi/dispatcher/blocking_detector.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/dispatcher_actor.py` & `powerapi-2.0.4/powerapi/dispatcher/dispatcher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/handlers.py` & `powerapi-2.0.4/powerapi/dispatcher/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/route_table.py` & `powerapi-2.0.4/powerapi/dispatcher/route_table.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/simple/__init__.py` & `powerapi-2.0.4/powerapi/dispatcher/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_actor.py` & `powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_handlers.py` & `powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/exception.py` & `powerapi-2.0.4/powerapi/utils/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,31 +23,45 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import collections.abc as collections
+import datetime
 
-class PowerAPIException(Exception):
+
+def timestamp_to_datetime(timestamp):
     """
-    PowerAPIException base class
+    Create datetime from a timestamp value
+
+    :param int timestamp:
+    :rtype: datetime.datetime
     """
-    def __init__(self, *args: object):
-        Exception.__init__(self, args)
+    return datetime.datetime.fromtimestamp(timestamp / 1000)
 
 
-class PowerAPIExceptionWithMessage(PowerAPIException):
-    """
-    PowerAPIException base class
+def datetime_to_timestamp(date):
     """
+    Cast a datetime object to a simple timestamp
 
-    def __init__(self, msg):
-        PowerAPIException.__init__(self)
-        self.msg = msg
+    :param datetime.datetime date:
+    :rtype: int
+    """
+    return int(datetime.datetime.timestamp(date) * 1000)
 
 
-class BadInputData(PowerAPIException):
+def dict_merge(dict1, dict2):
     """
-    Exception raised when the data read in input are not
-    in the good format
+    Recursive dict merge, act like dict.update() but update
+    all level and not only top-level.
+
+    :param dict dict1:
+    :param dict dict2:
+
     """
+    for key, value in dict2.items():
+        if (key in dict1 and isinstance(dict1[key], dict) and isinstance(dict2[key], collections.Mapping)):
+            dict_merge(dict1[key], dict2[key])
+        else:
+            dict1[key] = value
```

### Comparing `powerapi-2.0.3/powerapi/filter/__init__.py` & `powerapi-2.0.4/powerapi/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/filter/filter.py` & `powerapi-2.0.4/powerapi/filter/filter.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/formula/__init__.py` & `powerapi-2.0.4/powerapi/formula/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/formula/abstract_cpu_dram_formula.py` & `powerapi-2.0.4/powerapi/formula/abstract_cpu_dram_formula.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/formula/formula_actor.py` & `powerapi-2.0.4/powerapi/formula/formula_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/formula/handlers.py` & `powerapi-2.0.4/powerapi/formula/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/formula/simple/__init__.py` & `powerapi-2.0.4/powerapi/formula/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/formula/simple/simple_formula_actor.py` & `powerapi-2.0.4/powerapi/formula/simple/simple_formula_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/formula/simple/simple_handlers.py` & `powerapi-2.0.4/powerapi/formula/simple/simple_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/handler/__init__.py` & `powerapi-2.0.4/powerapi/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/handler/handler.py` & `powerapi-2.0.4/powerapi/handler/handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/handler/poison_pill_message_handler.py` & `powerapi-2.0.4/powerapi/handler/poison_pill_message_handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/handler/start_handler.py` & `powerapi-2.0.4/powerapi/handler/start_handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/message.py` & `powerapi-2.0.4/powerapi/message.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/puller/__init__.py` & `powerapi-2.0.4/powerapi/puller/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/puller/handlers.py` & `powerapi-2.0.4/powerapi/puller/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/puller/puller_actor.py` & `powerapi-2.0.4/powerapi/puller/puller_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/puller/simple/__init__.py` & `powerapi-2.0.4/powerapi/puller/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/puller/simple/simple_puller_actor.py` & `powerapi-2.0.4/powerapi/puller/simple/simple_puller_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/puller/simple/simple_puller_handlers.py` & `powerapi-2.0.4/powerapi/puller/simple/simple_puller_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/pusher/__init__.py` & `powerapi-2.0.4/powerapi/pusher/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/pusher/handlers.py` & `powerapi-2.0.4/powerapi/pusher/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/pusher/pusher_actor.py` & `powerapi-2.0.4/powerapi/pusher/pusher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/pusher/simple/__init__.py` & `powerapi-2.0.4/powerapi/pusher/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_actor.py` & `powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_handlers.py` & `powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report/__init__.py` & `powerapi-2.0.4/powerapi/report/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report/control_report.py` & `powerapi-2.0.4/powerapi/report/control_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report/formula_report.py` & `powerapi-2.0.4/powerapi/report/formula_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report/hwpc_report.py` & `powerapi-2.0.4/powerapi/report/hwpc_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report/power_report.py` & `powerapi-2.0.4/powerapi/report/power_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report/procfs_report.py` & `powerapi-2.0.4/powerapi/report/procfs_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report/report.py` & `powerapi-2.0.4/powerapi/report/report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report_modifier/__init__.py` & `powerapi-2.0.4/powerapi/report_modifier/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report_modifier/libvirt_mapper.py` & `powerapi-2.0.4/powerapi/report_modifier/libvirt_mapper.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/report_modifier/report_modifier.py` & `powerapi-2.0.4/powerapi/report_modifier/report_modifier.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/utils/__init__.py` & `powerapi-2.0.4/powerapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/utils/json_stream.py` & `powerapi-2.0.4/powerapi/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/utils/stat_buffer.py` & `powerapi-2.0.4/powerapi/utils/stat_buffer.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/utils/sync.py` & `powerapi-2.0.4/powerapi/utils/sync.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/utils/tree.py` & `powerapi-2.0.4/powerapi/utils/tree.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/powerapi/utils/utils.py` & `powerapi-2.0.4/powerapi/utils/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2021, INRIA
-# Copyright (c) 2021, University of Lille
+# Copyright (c) 2023, INRIA
+# Copyright (c) 2023, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,45 +23,36 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import collections.abc as collections
-import datetime
-
-
-def timestamp_to_datetime(timestamp):
+def remove_first_characters(arg: str):
     """
-    Create datetime from a timestamp value
-
-    :param int timestamp:
-    :rtype: datetime.datetime
+    Remove the two first characters of arg if it has more than 2 characters, otherwise, it removes only the first one.
+    :param str arg: The string to remove the first characters
     """
-    return datetime.datetime.fromtimestamp(timestamp / 1000)
+    if len(arg) > 2:
+        return arg[2:]
+    return arg[1]
 
 
-def datetime_to_timestamp(date):
+def find_longest_string_in_list(string_list: list):
     """
-    Cast a datetime object to a simple timestamp
-
-    :param datetime.datetime date:
-    :rtype: int
+    Find the largest string contained in the given list
+    :param list string_list: List of strings
     """
-    return int(datetime.datetime.timestamp(date) * 1000)
+    max_len = 0
+    longest_string = ''
+    for name in string_list:
+        if len(name) > max_len:
+            longest_string = name
+            max_len = len(name)
+    return longest_string
 
 
-def dict_merge(dict1, dict2):
+def string_to_bool(bool_value: str):
     """
-    Recursive dict merge, act like dict.update() but update
-    all level and not only top-level.
-
-    :param dict dict1:
-    :param dict dict2:
-
+    Transforms a str to bool according to their content
     """
-    for key, value in dict2.items():
-        if (key in dict1 and isinstance(dict1[key], dict) and isinstance(dict2[key], collections.Mapping)):
-            dict_merge(dict1[key], dict2[key])
-        else:
-            dict1[key] = value
+    return bool_value.lower() in ("yes", "true", "t", "1")
```

### Comparing `powerapi-2.0.3/powerapi.egg-info/PKG-INFO` & `powerapi-2.0.4/powerapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.0.3
+Version: 2.0.4
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerapi Version: 2.0.3 Summary: PowerAPI is a
+Metadata-Version: 2.1 Name: powerapi Version: 2.0.4 Summary: PowerAPI is a
 middleware toolkit for building software-defined power meters. Author-email:
 PowerAPI Staff
 inria.fr> License: BSD-3-Clause Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org Project-URL:
 repository, https://github.com/powerapi-ng/powerapi Keywords:
 powerapi,energy,power-meter,green-computing Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `powerapi-2.0.3/powerapi.egg-info/SOURCES.txt` & `powerapi-2.0.4/powerapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 powerapi/actor/actor.py
 powerapi/actor/socket_interface.py
 powerapi/actor/state.py
 powerapi/actor/supervisor.py
 powerapi/backend_supervisor/__init__.py
 powerapi/backend_supervisor/backend_supervisor.py
 powerapi/cli/__init__.py
+powerapi/cli/common_cli_parsing_manager.py
 powerapi/cli/config_parser.py
 powerapi/cli/config_validator.py
 powerapi/cli/generator.py
-powerapi/cli/parser.py
-powerapi/cli/tools.py
+powerapi/cli/parsing_manager.py
 powerapi/database/__init__.py
 powerapi/database/base_db.py
 powerapi/database/csvdb.py
 powerapi/database/direct_prometheus_db.py
 powerapi/database/file_db.py
 powerapi/database/influxdb.py
 powerapi/database/influxdb2.py
@@ -80,12 +80,13 @@
 powerapi/report/power_report.py
 powerapi/report/procfs_report.py
 powerapi/report/report.py
 powerapi/report_modifier/__init__.py
 powerapi/report_modifier/libvirt_mapper.py
 powerapi/report_modifier/report_modifier.py
 powerapi/utils/__init__.py
+powerapi/utils/cli.py
 powerapi/utils/json_stream.py
 powerapi/utils/stat_buffer.py
 powerapi/utils/sync.py
 powerapi/utils/tree.py
 powerapi/utils/utils.py
```

### Comparing `powerapi-2.0.3/powerapi.egg-info/requires.txt` & `powerapi-2.0.4/powerapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.3/pyproject.toml` & `powerapi-2.0.4/pyproject.toml`

 * *Files identical despite different names*

