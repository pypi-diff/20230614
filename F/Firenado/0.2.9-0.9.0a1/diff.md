# Comparing `tmp/Firenado-0.2.9.tar.gz` & `tmp/Firenado-0.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Firenado-0.2.9.tar", last modified: Sun Apr  4 00:22:57 2021, max compression
+gzip compressed data, was "Firenado-0.9.0a1.tar", last modified: Tue Jun  6 15:02:38 2023, max compression
```

## Comparing `Firenado-0.2.9.tar` & `Firenado-0.9.0a1.tar`

### file list

```diff
@@ -1,97 +1,107 @@
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.015006 Firenado-0.2.9/
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.003006 Firenado-0.2.9/Firenado.egg-info/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     5363 2021-04-04 00:22:56.000000 Firenado-0.2.9/Firenado.egg-info/PKG-INFO
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2319 2021-04-04 00:22:56.000000 Firenado-0.2.9/Firenado.egg-info/SOURCES.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        1 2021-04-04 00:22:56.000000 Firenado-0.2.9/Firenado.egg-info/dependency_links.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       72 2021-04-04 00:22:56.000000 Firenado-0.2.9/Firenado.egg-info/entry_points.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      258 2021-04-04 00:22:56.000000 Firenado-0.2.9/Firenado.egg-info/requires.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       15 2021-04-04 00:22:56.000000 Firenado-0.2.9/Firenado.egg-info/top_level.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    11349 2020-02-29 17:12:35.000000 Firenado-0.2.9/LICENSE
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      593 2021-03-14 16:46:20.000000 Firenado-0.2.9/MANIFEST.in
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5363 2021-04-04 00:22:57.015006 Firenado-0.2.9/PKG-INFO
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3249 2019-01-26 05:48:04.000000 Firenado-0.2.9/README.md
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3118 2019-01-26 05:48:04.000000 Firenado-0.2.9/README.rst
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.005006 Firenado-0.2.9/firenado/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      938 2021-04-04 00:11:25.000000 Firenado-0.2.9/firenado/__init__.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.006006 Firenado-0.2.9/firenado/bin/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      740 2019-01-19 15:51:14.000000 Firenado-0.2.9/firenado/bin/firenado-cli.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.006006 Firenado-0.2.9/firenado/components/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      759 2019-01-19 15:51:14.000000 Firenado-0.2.9/firenado/components/__init__.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.006006 Firenado-0.2.9/firenado/components/firenado/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.2.9/firenado/components/firenado/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      872 2016-09-08 01:38:40.000000 Firenado-0.2.9/firenado/components/firenado/component.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1063 2016-09-08 01:38:40.000000 Firenado-0.2.9/firenado/components/firenado/handlers.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.007006 Firenado-0.2.9/firenado/components/firenado/templates/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4008 2016-08-29 15:57:57.000000 Firenado-0.2.9/firenado/components/firenado/templates/info.html
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.007006 Firenado-0.2.9/firenado/components/static_maps/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.2.9/firenado/components/static_maps/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4137 2018-08-25 00:58:30.000000 Firenado-0.2.9/firenado/components/static_maps/component.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.007006 Firenado-0.2.9/firenado/components/toolbox/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-11-26 15:05:30.000000 Firenado-0.2.9/firenado/components/toolbox/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      831 2016-11-26 15:05:30.000000 Firenado-0.2.9/firenado/components/toolbox/component.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1675 2020-06-18 21:24:15.000000 Firenado-0.2.9/firenado/components/toolbox/uimodules.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.008006 Firenado-0.2.9/firenado/conf/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4706 2021-04-03 04:19:30.000000 Firenado-0.2.9/firenado/conf/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1091 2020-02-29 17:12:35.000000 Firenado-0.2.9/firenado/conf/firenado.yml
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    17663 2021-04-03 04:28:11.000000 Firenado-0.2.9/firenado/config.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    13422 2021-03-25 17:25:45.000000 Firenado-0.2.9/firenado/data.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    12800 2021-04-03 04:43:35.000000 Firenado-0.2.9/firenado/launcher.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.009006 Firenado-0.2.9/firenado/management/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      738 2019-05-18 04:12:04.000000 Firenado-0.2.9/firenado/management/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1993 2020-02-29 17:12:35.000000 Firenado-0.2.9/firenado/management/commands.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8578 2021-03-23 17:02:47.000000 Firenado-0.2.9/firenado/management/management.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6791 2021-03-23 16:54:01.000000 Firenado-0.2.9/firenado/management/tasks.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.001006 Firenado-0.2.9/firenado/management/templates/
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.010006 Firenado-0.2.9/firenado/management/templates/help/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      160 2016-09-08 01:38:40.000000 Firenado-0.2.9/firenado/management/templates/help/app_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      119 2018-11-03 23:08:57.000000 Firenado-0.2.9/firenado/management/templates/help/header.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       46 2016-09-08 01:38:40.000000 Firenado-0.2.9/firenado/management/templates/help/init_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      252 2018-11-03 23:09:50.000000 Firenado-0.2.9/firenado/management/templates/help/main_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      117 2017-06-19 04:13:32.000000 Firenado-0.2.9/firenado/management/templates/help/project_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      241 2020-02-29 17:12:35.000000 Firenado-0.2.9/firenado/management/templates/help/random_command_help.txt
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.011006 Firenado-0.2.9/firenado/management/templates/project/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      224 2018-11-21 07:38:12.000000 Firenado-0.2.9/firenado/management/templates/project/app.py.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      691 2016-09-10 17:22:04.000000 Firenado-0.2.9/firenado/management/templates/project/firenado.yml.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      212 2018-11-21 07:38:12.000000 Firenado-0.2.9/firenado/management/templates/project/handlers.py.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       54 2016-09-08 01:38:40.000000 Firenado-0.2.9/firenado/management/templates/project/init_command_help.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    14559 2021-03-28 01:47:35.000000 Firenado-0.2.9/firenado/schedule.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     5276 2021-03-23 16:37:05.000000 Firenado-0.2.9/firenado/security.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4230 2021-03-23 16:37:05.000000 Firenado-0.2.9/firenado/service.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    21993 2021-03-25 19:17:05.000000 Firenado-0.2.9/firenado/session.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    22004 2021-03-25 19:16:32.000000 Firenado-0.2.9/firenado/tornadoweb.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      847 2021-03-23 16:46:58.000000 Firenado-0.2.9/firenado/uimodules.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.012006 Firenado-0.2.9/firenado/util/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-02-29 17:12:35.000000 Firenado-0.2.9/firenado/util/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1084 2019-05-18 04:12:19.000000 Firenado-0.2.9/firenado/util/argparse_util.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3468 2020-09-11 14:09:30.000000 Firenado-0.2.9/firenado/util/sqlalchemy_util.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      920 2019-05-18 04:12:04.000000 Firenado-0.2.9/firenado/util/url_util.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.012006 Firenado-0.2.9/requirements/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       62 2020-07-28 14:20:19.000000 Firenado-0.2.9/requirements/all.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       49 2021-04-03 04:22:18.000000 Firenado-0.2.9/requirements/basic.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       15 2020-02-29 17:12:35.000000 Firenado-0.2.9/requirements/pexpect.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       28 2021-04-03 04:23:04.000000 Firenado-0.2.9/requirements/redis.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       17 2021-04-03 04:23:04.000000 Firenado-0.2.9/requirements/schedule.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       18 2021-04-03 04:23:04.000000 Firenado-0.2.9/requirements/sqlalchemy.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      102 2021-04-04 00:22:57.015006 Firenado-0.2.9/setup.cfg
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3780 2021-03-14 16:45:56.000000 Firenado-0.2.9/setup.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.014006 Firenado-0.2.9/tests/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2156 2021-03-23 16:49:01.000000 Firenado-0.2.9/tests/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1865 2021-03-23 17:02:58.000000 Firenado-0.2.9/tests/components_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     9805 2021-03-23 16:50:16.000000 Firenado-0.2.9/tests/conf_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1903 2021-03-23 17:03:37.000000 Firenado-0.2.9/tests/config_test.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2816 2021-03-25 16:38:16.000000 Firenado-0.2.9/tests/data_test.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.014006 Firenado-0.2.9/tests/features/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2019-05-18 04:12:19.000000 Firenado-0.2.9/tests/features/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1021 2020-03-17 14:16:49.000000 Firenado-0.2.9/tests/features/environment.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.014006 Firenado-0.2.9/tests/features/steps/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-03-17 14:16:49.000000 Firenado-0.2.9/tests/features/steps/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2410 2020-03-17 14:16:49.000000 Firenado-0.2.9/tests/features/steps/launcher.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1793 2021-03-25 03:55:31.000000 Firenado-0.2.9/tests/runtests.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2073 2021-03-23 17:04:21.000000 Firenado-0.2.9/tests/security_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     7065 2021-03-23 17:04:45.000000 Firenado-0.2.9/tests/service_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4925 2021-03-23 17:06:32.000000 Firenado-0.2.9/tests/session_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6025 2021-03-23 17:08:06.000000 Firenado-0.2.9/tests/tornadoweb_test.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2021-04-04 00:22:57.015006 Firenado-0.2.9/tests/util/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2018-07-08 04:28:25.000000 Firenado-0.2.9/tests/util/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3289 2021-03-23 17:10:03.000000 Firenado-0.2.9/tests/util/sqlalchemy_util_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1895 2021-03-23 17:10:31.000000 Firenado-0.2.9/tests/util/url_util_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.280004 Firenado-0.9.0a1/Firenado.egg-info/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5202 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2539 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/SOURCES.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/dependency_links.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       71 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/entry_points.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      238 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/requires.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       15 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/top_level.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    11361 2022-01-22 03:40:14.000000 Firenado-0.9.0a1/LICENSE
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      593 2021-03-14 16:46:20.000000 Firenado-0.9.0a1/MANIFEST.in
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5202 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/PKG-INFO
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3789 2022-04-15 16:36:51.000000 Firenado-0.9.0a1/README.md
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3118 2019-01-26 05:48:04.000000 Firenado-0.9.0a1/README.rst
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.282004 Firenado-0.9.0a1/firenado/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1079 2023-06-06 14:40:55.000000 Firenado-0.9.0a1/firenado/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3895 2023-06-05 20:36:53.000000 Firenado-0.9.0a1/firenado/_pexpect_async_patch.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/bin/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2022-08-03 17:33:42.000000 Firenado-0.9.0a1/firenado/bin/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      752 2022-12-01 17:39:50.000000 Firenado-0.9.0a1/firenado/bin/firenado-cli.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      727 2022-08-30 19:14:45.000000 Firenado-0.9.0a1/firenado/bin/firenado-cli1.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/cli/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       31 2022-08-30 19:14:45.000000 Firenado-0.9.0a1/firenado/cli/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      620 2022-03-19 18:33:11.000000 Firenado-0.9.0a1/firenado/cli/commands.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      194 2022-08-30 18:49:41.000000 Firenado-0.9.0a1/firenado/cli/root.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/components/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      759 2019-01-19 15:51:14.000000 Firenado-0.9.0a1/firenado/components/__init__.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/components/firenado/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/firenado/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      872 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/firenado/component.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1063 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/firenado/handlers.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.284004 Firenado-0.9.0a1/firenado/components/firenado/templates/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4008 2016-08-29 15:57:57.000000 Firenado-0.9.0a1/firenado/components/firenado/templates/info.html
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.284004 Firenado-0.9.0a1/firenado/components/static_maps/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/static_maps/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4137 2018-08-25 00:58:30.000000 Firenado-0.9.0a1/firenado/components/static_maps/component.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.284004 Firenado-0.9.0a1/firenado/components/toolbox/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-11-26 15:05:30.000000 Firenado-0.9.0a1/firenado/components/toolbox/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      831 2016-11-26 15:05:30.000000 Firenado-0.9.0a1/firenado/components/toolbox/component.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1961 2021-12-06 00:51:41.000000 Firenado-0.9.0a1/firenado/components/toolbox/uimodules.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.285004 Firenado-0.9.0a1/firenado/conf/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4774 2022-08-30 18:49:41.000000 Firenado-0.9.0a1/firenado/conf/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1092 2022-12-23 19:35:46.000000 Firenado-0.9.0a1/firenado/conf/firenado.yml
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    17831 2023-01-30 02:41:12.000000 Firenado-0.9.0a1/firenado/config.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    15458 2023-06-06 03:00:02.000000 Firenado-0.9.0a1/firenado/data.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    14990 2023-06-05 20:54:46.000000 Firenado-0.9.0a1/firenado/launcher.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.285004 Firenado-0.9.0a1/firenado/management/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      738 2019-05-18 04:12:04.000000 Firenado-0.9.0a1/firenado/management/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1993 2020-02-29 17:12:35.000000 Firenado-0.9.0a1/firenado/management/commands.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8627 2022-04-16 02:07:19.000000 Firenado-0.9.0a1/firenado/management/management.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6791 2022-04-13 19:58:05.000000 Firenado-0.9.0a1/firenado/management/tasks.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.278004 Firenado-0.9.0a1/firenado/management/templates/
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.286004 Firenado-0.9.0a1/firenado/management/templates/help/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      160 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/management/templates/help/app_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      119 2018-11-03 23:08:57.000000 Firenado-0.9.0a1/firenado/management/templates/help/header.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       46 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/management/templates/help/init_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      252 2018-11-03 23:09:50.000000 Firenado-0.9.0a1/firenado/management/templates/help/main_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      117 2017-06-19 04:13:32.000000 Firenado-0.9.0a1/firenado/management/templates/help/project_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      241 2020-02-29 17:12:35.000000 Firenado-0.9.0a1/firenado/management/templates/help/random_command_help.txt
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.286004 Firenado-0.9.0a1/firenado/management/templates/project/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      224 2018-11-21 07:38:12.000000 Firenado-0.9.0a1/firenado/management/templates/project/app.py.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      691 2016-09-10 17:22:04.000000 Firenado-0.9.0a1/firenado/management/templates/project/firenado.yml.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      212 2018-11-21 07:38:12.000000 Firenado-0.9.0a1/firenado/management/templates/project/handlers.py.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       54 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/management/templates/project/init_command_help.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    15364 2022-04-16 01:20:31.000000 Firenado-0.9.0a1/firenado/schedule.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    10107 2022-12-18 22:48:38.000000 Firenado-0.9.0a1/firenado/security.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4906 2023-01-30 02:42:51.000000 Firenado-0.9.0a1/firenado/service.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    22717 2023-03-01 19:37:22.000000 Firenado-0.9.0a1/firenado/session.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6160 2023-06-06 03:01:08.000000 Firenado-0.9.0a1/firenado/sqlalchemy.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4608 2022-11-12 06:31:24.000000 Firenado-0.9.0a1/firenado/testing.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    21715 2023-05-19 18:16:54.000000 Firenado-0.9.0a1/firenado/tornadoweb.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      847 2021-03-23 16:46:58.000000 Firenado-0.9.0a1/firenado/uimodules.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.287004 Firenado-0.9.0a1/firenado/util/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-02-29 17:12:35.000000 Firenado-0.9.0a1/firenado/util/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1084 2019-05-18 04:12:19.000000 Firenado-0.9.0a1/firenado/util/argparse_util.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      939 2023-06-06 01:39:44.000000 Firenado-0.9.0a1/firenado/util/sqlalchemy_util.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      920 2019-05-18 04:12:04.000000 Firenado-0.9.0a1/firenado/util/url_util.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.288004 Firenado-0.9.0a1/requirements/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       62 2020-07-28 14:20:19.000000 Firenado-0.9.0a1/requirements/all.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       29 2023-06-05 21:13:20.000000 Firenado-0.9.0a1/requirements/basic.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       15 2022-07-23 21:52:18.000000 Firenado-0.9.0a1/requirements/pexpect.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       28 2022-07-23 21:51:27.000000 Firenado-0.9.0a1/requirements/redis.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       16 2022-12-23 19:45:17.000000 Firenado-0.9.0a1/requirements/schedule.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       19 2023-06-06 03:02:10.000000 Firenado-0.9.0a1/requirements/sqlalchemy.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      103 2023-06-06 15:02:38.291004 Firenado-0.9.0a1/setup.cfg
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3716 2023-06-05 21:12:00.000000 Firenado-0.9.0a1/setup.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.289004 Firenado-0.9.0a1/tests/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2180 2022-08-30 18:19:09.000000 Firenado-0.9.0a1/tests/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2010 2022-12-18 22:09:16.000000 Firenado-0.9.0a1/tests/components_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     9962 2022-04-20 03:19:42.000000 Firenado-0.9.0a1/tests/conf_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1903 2021-03-23 17:03:37.000000 Firenado-0.9.0a1/tests/config_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5212 2022-12-18 22:07:05.000000 Firenado-0.9.0a1/tests/data_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.289004 Firenado-0.9.0a1/tests/features/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2019-05-18 04:12:19.000000 Firenado-0.9.0a1/tests/features/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1021 2020-03-17 14:16:49.000000 Firenado-0.9.0a1/tests/features/environment.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/tests/features/steps/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-03-17 14:16:49.000000 Firenado-0.9.0a1/tests/features/steps/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1037 2022-07-22 14:57:31.000000 Firenado-0.9.0a1/tests/features/steps/cli.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2403 2022-04-16 02:44:17.000000 Firenado-0.9.0a1/tests/features/steps/launcher.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1802 2022-12-18 22:01:58.000000 Firenado-0.9.0a1/tests/runtests.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3095 2023-06-05 20:59:34.000000 Firenado-0.9.0a1/tests/security_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8036 2023-06-06 02:55:20.000000 Firenado-0.9.0a1/tests/service_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     5182 2022-12-24 04:00:43.000000 Firenado-0.9.0a1/tests/session_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     8874 2023-06-06 02:56:41.000000 Firenado-0.9.0a1/tests/sqlalchemy_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6025 2021-03-23 17:08:06.000000 Firenado-0.9.0a1/tests/tornadoweb_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/tests/util/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2018-07-08 04:28:25.000000 Firenado-0.9.0a1/tests/util/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1895 2021-03-23 17:10:31.000000 Firenado-0.9.0a1/tests/util/url_util_test.py
```

### Comparing `Firenado-0.2.9/Firenado.egg-info/PKG-INFO` & `Firenado-0.9.0a1/Firenado.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,133 +1,170 @@
 Metadata-Version: 2.1
 Name: Firenado
-Version: 0.2.9
+Version: 0.9.0a1
 Summary: Firenado is a python web framework based on Tornado web framework/server.
 Home-page: https://github.com/candango/firenado
-Author: Flavio Garcia
+Author: Flávio Gonçalves Garcia
 Author-email: piraz@candango.org
-Maintainer: Flavio Garcia
+Maintainer: Flávio Gonçalves Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
-Description: # Firenado Framework 
-        
-        **master:** [![Build Status](https://travis-ci.org/candango/firenado.svg?branch=master)](https://travis-ci.org/candango/firenado)
-        [![Code Health](https://landscape.io/github/candango/firenado/master/landscape.svg?style=flat)](https://landscape.io/github/candango/firenado/master)
-        [![Documentation Status](https://readthedocs.org/projects/firenado/badge/?version=latest)](https://readthedocs.org/projects/firenado/?badge=latest)
-        
-        **develop:** [![Build Status develop](https://travis-ci.org/candango/firenado.svg?branch=develop)](https://travis-ci.org/candango/firenado)
-        [![Code Health](https://landscape.io/github/candango/firenado/develop/landscape.svg?style=flat)](https://landscape.io/github/candango/firenado/develop)
-        [![Documentation Status](https://readthedocs.org/projects/firenado/badge/?version=develop)](http://firenado.readthedocs.org/en/develop/?badge=develop)
-        
-        
-        ## Introduction
-        
-        Firenado is a Python web framework that encapsulates and extends
-        [Tornado](http://www.tornadoweb.org) organizing the application in
-        components also adding a server side session layer, yaml based configuration
-        files as other features common that will help developers building web
-        applications and services.
-        
-        Firenado is a web framework that extends the original Tornado Web framework
-        adding new features like loose couple components, server side session layer, 
-        yaml based configuration files and more.
-        
-        ## Installation
-        
-        Installing Firenado will only force the installation of pyyaml, Tornado and
-        six. We call it the basic installation:
-        
-        ```
-        pip install firenado
-        ```
-        
-        It is possible to install extra packages as redis-py, sqlalchemy and pexpect.
-        
-        To install only redis-py:
-        
-        ```
-        pip install firenado[redis]
-        ```
-        
-        Complete installation:
-        
-        ```
-        pip install firenado[pexpect, redis, sqlalchemy]
-        ```
-        
-        ## Usage
-        
-        Creating and running a new application:
-        
-        ```shell
-        firenado project init helloworld
-        cd helloworld
-        firenado app run
-        ```
-        
-        An application will be created with the redis based session engine
-        and a redis data source linked to the session.
-        
-        Firenado won't install redis-py so it is necessary to inform the extra
-        requirement parameter or install it separately. It is possible to change 
-        the session to a file based engine or disable the session engine completely.
-        
-        In order to change the session type to file go to helloworld/conf/firenado.yml
-        and change the session definition to:
-        
-        ```yaml
-        # Session types could be:
-        # file or redis.
-        session:
-          type: file
-          enabled: true
-          # Redis session handler configuration
-          #data:
-          #  source: session
-          # File session handler related configuration
-          path: /tmp
-        ```
-        
-        If your helloworld project isn't located in the python path just go 
-        helloworld/conf/firenado.yml and changed it to:
-        
-        ```yaml
-        app:
-          component: helloworld
-          data:
-            sources:
-                # Set here references from sources defined on data.sources
-                - session
-          pythonpath: ..
-          port: 8888
-        ```
-        
-        ## Support
-        
-        Firenado is one of [Candango Open Source Group](http://www.candango.org/projects/) initiatives. It is available under
-        the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
-        
-        This web site and all documentation is licensed under [Creative
-        Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: redis
 Provides-Extra: pexpect
 Provides-Extra: schedule
 Provides-Extra: sqlalchemy
+License-File: LICENSE
+
+# Firenado Framework 
+
+[![Latest PyPI version](https://img.shields.io/pypi/v/firenado.svg)](https://pypi.org/project/firenado/)
+[![Number of PyPI downloads](https://img.shields.io/pypi/dm/firenado.svg)](https://pypi.org/project/firenado/#files)
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Ffirenado%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/firenado/goto)
+[![GitHub license](https://img.shields.io/github/license/candango/firenado)](https://github.com/candango/firenado/blob/develop/LICENSE)
+
+## Introduction
+
+Firenado is a Python web framework that encapsulates and extends
+[Tornado](http://www.tornadoweb.org) organizing the application in
+components also adding a server side session layer, yaml based configuration
+files as other features common that will help developers building web
+applications and services.
+
+Firenado is a web framework that extends the original Tornado Web framework
+adding new features like loose couple components, server side session layer, 
+yaml based configuration files and more.
+
+## Installation
+
+Installing Firenado will only force the installation of pyyaml, Tornado and
+six. We call it the basic installation:
+
+```
+pip install firenado
+```
+
+It is possible to install extra packages as redis-py, sqlalchemy and pexpect.
+
+Installing only redis-py:
+
+```
+pip install firenado[redis]
+```
+
+Installing only redis-py:
+
+```
+pip install firenado[sqlalchemy pexpect]
+```
+
+Installing only redis (redis-py, hiredis):
+
+```
+pip install firenado[sqlalchemy pexpect]
+```
+
+Installing redis and schedule(croniter):
+
+```
+pip install firenado[redis schedule]
+```
+
+Complete installation(what it is being the case, everytime):
+
+```
+pip install firenado[all]
+```
+
+> In the future, the installation logic will be inverted. Redis and pexpect
+> will be added by default, and disabling them using optional parameters.
+>
+> The sqlalchemy and schedule(croniter) optionals will remain as is.
+>
+> With that change if you want just add schedule to the redis and pexpect:
+>
+> ``` pip install firenado[schedule] ```
+>
+> Maybe you want an agent with scheduled features and no redis:
+>
+> ``` pip install firenado[schedule noredis] ```
+>
+> Or don't need ProcessLaucher but sqlalchemy support:
+>
+> ``` pip install firenado[sqlalchemy nopexpect] ```
+>
+> See: #401
+
+## Usage
+
+Creating and running a new application:
+
+```shell
+firenado project init helloworld
+cd helloworld
+firenado app run
+```
+
+An application will be created with the redis based session engine
+and a redis data source linked to the session.
+
+Firenado won't install redis-py so it is necessary to inform the extra
+requirement parameter or install it separately. It is possible to change 
+the session to a file based engine or disable the session engine completely.
+
+In order to change the session type to file go to helloworld/conf/firenado.yml
+and change the session definition to:
+
+```yaml
+# Session types could be:
+# file or redis.
+session:
+  type: file
+  enabled: true
+  # Redis session handler configuration
+  #data:
+  #  source: session
+  # File session handler related configuration
+  path: /tmp
+```
+
+If your helloworld project isn't located in the python path just go 
+helloworld/conf/firenado.yml and changed it to:
+
+```yaml
+app:
+  component: helloworld
+  data:
+    sources:
+        # Set here references from sources defined on data.sources
+        - session
+  pythonpath: ..
+  port: 8888
+```
+
+## Support
+
+Firenado is one of [Candango Open Source Group
+](http://www.candango.org/projects/) initiatives. It is available under
+the [Apache License, Version 2.0
+](http://www.apache.org/licenses/LICENSE-2.0.html).
+
+This web site and all documentation is licensed under [Creative
+Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/Firenado.egg-info/SOURCES.txt` & `Firenado-0.9.0a1/Firenado.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,32 @@
 Firenado.egg-info/PKG-INFO
 Firenado.egg-info/SOURCES.txt
 Firenado.egg-info/dependency_links.txt
 Firenado.egg-info/entry_points.txt
 Firenado.egg-info/requires.txt
 Firenado.egg-info/top_level.txt
 firenado/__init__.py
+firenado/_pexpect_async_patch.py
 firenado/config.py
 firenado/data.py
 firenado/launcher.py
 firenado/schedule.py
 firenado/security.py
 firenado/service.py
 firenado/session.py
+firenado/sqlalchemy.py
+firenado/testing.py
 firenado/tornadoweb.py
 firenado/uimodules.py
+firenado/bin/__init__.py
 firenado/bin/firenado-cli.py
+firenado/bin/firenado-cli1.py
+firenado/cli/__init__.py
+firenado/cli/commands.py
+firenado/cli/root.py
 firenado/components/__init__.py
 firenado/components/firenado/__init__.py
 firenado/components/firenado/component.py
 firenado/components/firenado/handlers.py
 firenado/components/firenado/templates/info.html
 firenado/components/static_maps/__init__.py
 firenado/components/static_maps/component.py
@@ -62,15 +70,16 @@
 tests/conf_test.py
 tests/config_test.py
 tests/data_test.py
 tests/runtests.py
 tests/security_test.py
 tests/service_test.py
 tests/session_test.py
+tests/sqlalchemy_test.py
 tests/tornadoweb_test.py
 tests/features/__init__.py
 tests/features/environment.py
 tests/features/steps/__init__.py
+tests/features/steps/cli.py
 tests/features/steps/launcher.py
 tests/util/__init__.py
-tests/util/sqlalchemy_util_test.py
 tests/util/url_util_test.py
```

### Comparing `Firenado-0.2.9/LICENSE` & `Firenado-0.9.0a1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2015-2020 Flavio Garcia
+   Copyright 2015-2022 Flávio Gonçalves Garcia
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/MANIFEST.in` & `Firenado-0.9.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/PKG-INFO` & `Firenado-0.9.0a1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,133 +1,170 @@
 Metadata-Version: 2.1
 Name: Firenado
-Version: 0.2.9
+Version: 0.9.0a1
 Summary: Firenado is a python web framework based on Tornado web framework/server.
 Home-page: https://github.com/candango/firenado
-Author: Flavio Garcia
+Author: Flávio Gonçalves Garcia
 Author-email: piraz@candango.org
-Maintainer: Flavio Garcia
+Maintainer: Flávio Gonçalves Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
-Description: # Firenado Framework 
-        
-        **master:** [![Build Status](https://travis-ci.org/candango/firenado.svg?branch=master)](https://travis-ci.org/candango/firenado)
-        [![Code Health](https://landscape.io/github/candango/firenado/master/landscape.svg?style=flat)](https://landscape.io/github/candango/firenado/master)
-        [![Documentation Status](https://readthedocs.org/projects/firenado/badge/?version=latest)](https://readthedocs.org/projects/firenado/?badge=latest)
-        
-        **develop:** [![Build Status develop](https://travis-ci.org/candango/firenado.svg?branch=develop)](https://travis-ci.org/candango/firenado)
-        [![Code Health](https://landscape.io/github/candango/firenado/develop/landscape.svg?style=flat)](https://landscape.io/github/candango/firenado/develop)
-        [![Documentation Status](https://readthedocs.org/projects/firenado/badge/?version=develop)](http://firenado.readthedocs.org/en/develop/?badge=develop)
-        
-        
-        ## Introduction
-        
-        Firenado is a Python web framework that encapsulates and extends
-        [Tornado](http://www.tornadoweb.org) organizing the application in
-        components also adding a server side session layer, yaml based configuration
-        files as other features common that will help developers building web
-        applications and services.
-        
-        Firenado is a web framework that extends the original Tornado Web framework
-        adding new features like loose couple components, server side session layer, 
-        yaml based configuration files and more.
-        
-        ## Installation
-        
-        Installing Firenado will only force the installation of pyyaml, Tornado and
-        six. We call it the basic installation:
-        
-        ```
-        pip install firenado
-        ```
-        
-        It is possible to install extra packages as redis-py, sqlalchemy and pexpect.
-        
-        To install only redis-py:
-        
-        ```
-        pip install firenado[redis]
-        ```
-        
-        Complete installation:
-        
-        ```
-        pip install firenado[pexpect, redis, sqlalchemy]
-        ```
-        
-        ## Usage
-        
-        Creating and running a new application:
-        
-        ```shell
-        firenado project init helloworld
-        cd helloworld
-        firenado app run
-        ```
-        
-        An application will be created with the redis based session engine
-        and a redis data source linked to the session.
-        
-        Firenado won't install redis-py so it is necessary to inform the extra
-        requirement parameter or install it separately. It is possible to change 
-        the session to a file based engine or disable the session engine completely.
-        
-        In order to change the session type to file go to helloworld/conf/firenado.yml
-        and change the session definition to:
-        
-        ```yaml
-        # Session types could be:
-        # file or redis.
-        session:
-          type: file
-          enabled: true
-          # Redis session handler configuration
-          #data:
-          #  source: session
-          # File session handler related configuration
-          path: /tmp
-        ```
-        
-        If your helloworld project isn't located in the python path just go 
-        helloworld/conf/firenado.yml and changed it to:
-        
-        ```yaml
-        app:
-          component: helloworld
-          data:
-            sources:
-                # Set here references from sources defined on data.sources
-                - session
-          pythonpath: ..
-          port: 8888
-        ```
-        
-        ## Support
-        
-        Firenado is one of [Candango Open Source Group](http://www.candango.org/projects/) initiatives. It is available under
-        the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
-        
-        This web site and all documentation is licensed under [Creative
-        Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: redis
 Provides-Extra: pexpect
 Provides-Extra: schedule
 Provides-Extra: sqlalchemy
+License-File: LICENSE
+
+# Firenado Framework 
+
+[![Latest PyPI version](https://img.shields.io/pypi/v/firenado.svg)](https://pypi.org/project/firenado/)
+[![Number of PyPI downloads](https://img.shields.io/pypi/dm/firenado.svg)](https://pypi.org/project/firenado/#files)
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Ffirenado%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/firenado/goto)
+[![GitHub license](https://img.shields.io/github/license/candango/firenado)](https://github.com/candango/firenado/blob/develop/LICENSE)
+
+## Introduction
+
+Firenado is a Python web framework that encapsulates and extends
+[Tornado](http://www.tornadoweb.org) organizing the application in
+components also adding a server side session layer, yaml based configuration
+files as other features common that will help developers building web
+applications and services.
+
+Firenado is a web framework that extends the original Tornado Web framework
+adding new features like loose couple components, server side session layer, 
+yaml based configuration files and more.
+
+## Installation
+
+Installing Firenado will only force the installation of pyyaml, Tornado and
+six. We call it the basic installation:
+
+```
+pip install firenado
+```
+
+It is possible to install extra packages as redis-py, sqlalchemy and pexpect.
+
+Installing only redis-py:
+
+```
+pip install firenado[redis]
+```
+
+Installing only redis-py:
+
+```
+pip install firenado[sqlalchemy pexpect]
+```
+
+Installing only redis (redis-py, hiredis):
+
+```
+pip install firenado[sqlalchemy pexpect]
+```
+
+Installing redis and schedule(croniter):
+
+```
+pip install firenado[redis schedule]
+```
+
+Complete installation(what it is being the case, everytime):
+
+```
+pip install firenado[all]
+```
+
+> In the future, the installation logic will be inverted. Redis and pexpect
+> will be added by default, and disabling them using optional parameters.
+>
+> The sqlalchemy and schedule(croniter) optionals will remain as is.
+>
+> With that change if you want just add schedule to the redis and pexpect:
+>
+> ``` pip install firenado[schedule] ```
+>
+> Maybe you want an agent with scheduled features and no redis:
+>
+> ``` pip install firenado[schedule noredis] ```
+>
+> Or don't need ProcessLaucher but sqlalchemy support:
+>
+> ``` pip install firenado[sqlalchemy nopexpect] ```
+>
+> See: #401
+
+## Usage
+
+Creating and running a new application:
+
+```shell
+firenado project init helloworld
+cd helloworld
+firenado app run
+```
+
+An application will be created with the redis based session engine
+and a redis data source linked to the session.
+
+Firenado won't install redis-py so it is necessary to inform the extra
+requirement parameter or install it separately. It is possible to change 
+the session to a file based engine or disable the session engine completely.
+
+In order to change the session type to file go to helloworld/conf/firenado.yml
+and change the session definition to:
+
+```yaml
+# Session types could be:
+# file or redis.
+session:
+  type: file
+  enabled: true
+  # Redis session handler configuration
+  #data:
+  #  source: session
+  # File session handler related configuration
+  path: /tmp
+```
+
+If your helloworld project isn't located in the python path just go 
+helloworld/conf/firenado.yml and changed it to:
+
+```yaml
+app:
+  component: helloworld
+  data:
+    sources:
+        # Set here references from sources defined on data.sources
+        - session
+  pythonpath: ..
+  port: 8888
+```
+
+## Support
+
+Firenado is one of [Candango Open Source Group
+](http://www.candango.org/projects/) initiatives. It is available under
+the [Apache License, Version 2.0
+](http://www.apache.org/licenses/LICENSE-2.0.html).
+
+This web site and all documentation is licensed under [Creative
+Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/README.md` & `Firenado-0.9.0a1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # Firenado Framework 
 
-**master:** [![Build Status](https://travis-ci.org/candango/firenado.svg?branch=master)](https://travis-ci.org/candango/firenado)
-[![Code Health](https://landscape.io/github/candango/firenado/master/landscape.svg?style=flat)](https://landscape.io/github/candango/firenado/master)
-[![Documentation Status](https://readthedocs.org/projects/firenado/badge/?version=latest)](https://readthedocs.org/projects/firenado/?badge=latest)
-
-**develop:** [![Build Status develop](https://travis-ci.org/candango/firenado.svg?branch=develop)](https://travis-ci.org/candango/firenado)
-[![Code Health](https://landscape.io/github/candango/firenado/develop/landscape.svg?style=flat)](https://landscape.io/github/candango/firenado/develop)
-[![Documentation Status](https://readthedocs.org/projects/firenado/badge/?version=develop)](http://firenado.readthedocs.org/en/develop/?badge=develop)
-
+[![Latest PyPI version](https://img.shields.io/pypi/v/firenado.svg)](https://pypi.org/project/firenado/)
+[![Number of PyPI downloads](https://img.shields.io/pypi/dm/firenado.svg)](https://pypi.org/project/firenado/#files)
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Ffirenado%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/firenado/goto)
+[![GitHub license](https://img.shields.io/github/license/candango/firenado)](https://github.com/candango/firenado/blob/develop/LICENSE)
 
 ## Introduction
 
 Firenado is a Python web framework that encapsulates and extends
 [Tornado](http://www.tornadoweb.org) organizing the application in
 components also adding a server side session layer, yaml based configuration
 files as other features common that will help developers building web
@@ -28,26 +24,63 @@
 
 ```
 pip install firenado
 ```
 
 It is possible to install extra packages as redis-py, sqlalchemy and pexpect.
 
-To install only redis-py:
+Installing only redis-py:
 
 ```
 pip install firenado[redis]
 ```
 
-Complete installation:
+Installing only redis-py:
+
+```
+pip install firenado[sqlalchemy pexpect]
+```
+
+Installing only redis (redis-py, hiredis):
+
+```
+pip install firenado[sqlalchemy pexpect]
+```
+
+Installing redis and schedule(croniter):
 
 ```
-pip install firenado[pexpect, redis, sqlalchemy]
+pip install firenado[redis schedule]
 ```
 
+Complete installation(what it is being the case, everytime):
+
+```
+pip install firenado[all]
+```
+
+> In the future, the installation logic will be inverted. Redis and pexpect
+> will be added by default, and disabling them using optional parameters.
+>
+> The sqlalchemy and schedule(croniter) optionals will remain as is.
+>
+> With that change if you want just add schedule to the redis and pexpect:
+>
+> ``` pip install firenado[schedule] ```
+>
+> Maybe you want an agent with scheduled features and no redis:
+>
+> ``` pip install firenado[schedule noredis] ```
+>
+> Or don't need ProcessLaucher but sqlalchemy support:
+>
+> ``` pip install firenado[sqlalchemy nopexpect] ```
+>
+> See: #401
+
 ## Usage
 
 Creating and running a new application:
 
 ```shell
 firenado project init helloworld
 cd helloworld
@@ -89,12 +122,14 @@
         - session
   pythonpath: ..
   port: 8888
 ```
 
 ## Support
 
-Firenado is one of [Candango Open Source Group](http://www.candango.org/projects/) initiatives. It is available under
-the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
+Firenado is one of [Candango Open Source Group
+](http://www.candango.org/projects/) initiatives. It is available under
+the [Apache License, Version 2.0
+](http://www.apache.org/licenses/LICENSE-2.0.html).
 
 This web site and all documentation is licensed under [Creative
 Commons 3.0](http://creativecommons.org/licenses/by/3.0/).
```

### Comparing `Firenado-0.2.9/README.rst` & `Firenado-0.9.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/__init__.py` & `Firenado-0.9.0a1/firenado/components/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-# -*- coding: UTF-8 -*-
+#!/usr/bin/env python
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2019 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-"""The Firenado Framework"""
-
-__author__ = "Flavio Garcia <piraz@candango.org>"
-__version__ = (0, 2, 9)
-__licence__ = "Apache License V2.0"
-
-
-def get_version():
-    return ".".join(map(str, __version__))
-
-
-def get_author():
-    return __author__.split(" <")[0]
-
-
-def get_author_email():
-    return __author__.split(" <")[1][:-1]
+from .firenado.component import FirenadoComponent
+from .static_maps.component import StaticMapsComponent
+from .toolbox.component import ToolboxComponent
```

### Comparing `Firenado-0.2.9/firenado/bin/firenado-cli.py` & `Firenado-0.9.0a1/firenado/bin/firenado-cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2019 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/components/__init__.py` & `Firenado-0.9.0a1/firenado/cli/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-#!/usr/bin/env python
+# -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2019 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .firenado.component import FirenadoComponent
-from .static_maps.component import StaticMapsComponent
-from .toolbox.component import ToolboxComponent
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/components/firenado/component.py` & `Firenado-0.9.0a1/firenado/components/firenado/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/components/firenado/handlers.py` & `Firenado-0.9.0a1/firenado/components/firenado/handlers.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/components/firenado/templates/info.html` & `Firenado-0.9.0a1/firenado/components/firenado/templates/info.html`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/components/static_maps/component.py` & `Firenado-0.9.0a1/firenado/components/static_maps/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/components/toolbox/component.py` & `Firenado-0.9.0a1/firenado/components/toolbox/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/conf/__init__.py` & `Firenado-0.9.0a1/firenado/conf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,20 @@
 session['prefix'] = "firenado:session"
 session['purge_limit'] = 500
 session['redis'] = {}
 session['redis']['data'] = {}
 session['redis']['data']['source'] = ""
 session['type'] = ""
 
+taskio_conf = {}
+
 if HAS_LIB_CONFIG_FILE:
     lib_config = load_yaml_file(LIB_CONFIG_FILE)
     _config.process_config(sys.modules[__name__], lib_config)
+    taskio_conf = load_yaml_file(LIB_CONFIG_FILE)
 
 if HAS_SYS_CONFIG_FILE:
     sys_config = load_yaml_file(SYS_CONFIG_FILE)
     _config.process_config(sys.modules[__name__], sys_config)
 
 if HAS_APP_CONFIG_FILE:
     app_config = load_yaml_file(APP_CONFIG_FILE)
```

### Comparing `Firenado-0.2.9/firenado/conf/firenado.yml` & `Firenado-0.9.0a1/firenado/conf/firenado.yml`

 * *Files 10% similar despite different names*

```diff
@@ -35,11 +35,11 @@
       class: firenado.session.FileSessionHandler
     - name: redis
       class: firenado.session.RedisSessionHandler
   encoders:
     - name: json
       class: firenado.session.JsonSessionEncoder
     - name: pickle
-      class: firenado.session.PickeSessionEncoder
+      class: firenado.session.PickleSessionEncoder
   id_generators:
     - name: default
       function: firenado.session.generate_session_id
```

### Comparing `Firenado-0.2.9/firenado/config.py` & `Firenado-0.9.0a1/firenado/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -54,14 +54,15 @@
     app['types'] = {}
     app['types']['tornado'] = {}
     app['types']['tornado']['name'] = "tornado"
     app['types']['tornado']['launcher'] = {}
     app['types']['tornado']['launcher']['class'] = "TornadoLauncher"
     app['types']['tornado']['launcher']['module'] = "firenado.launcher"
     app['url_root_path'] = None
+    app['xheaders'] = None
     # Wait before shutdown is on seconds
     app['wait_before_shutdown'] = 0
     return app
 
 
 def get_config_from_package(package):
     """ Breaks a package string in module and class.
@@ -199,15 +200,15 @@
                 if not os.path.isabs(file):
                     file = os.path.abspath(
                         os.path.join(config.APP_CONFIG_PATH, file)
                     )
                 if not os.path.exists(file):
                     logger.critical("The file %s doesn't exists. Please check"
                                     "your apps definition and inform a valid "
-                                    "file." % file)
+                                    "file.", file)
                     sysexits.exit_fatal(sysexits.EX_CONFIG)
                 file_app_config = load_yaml_file(file)
                 if "app" in file_app_config:
                     process_app_config_section(config.apps[name],
                                                file_app_config['app'])
             else:
                 process_app_config_section(config.apps[name], app_config)
@@ -218,15 +219,15 @@
     if config.current_app_name is None:
         for app in config.apps:
             config.current_app_name = app
             break
     if config.current_app_name in config.apps:
         config.app = config.apps[config.current_app_name].app
     else:
-        logger.critical("The application %s is not defined." %
+        logger.critical("The application %s is not defined.",
                         config.current_app_name)
         sysexits.exit_fatal(sysexits.EX_CONFIG)
 
 
 def process_app_config_section(config, app_config):
     """ Processes the app section from a configuration data dict.
 
@@ -241,16 +242,17 @@
     if 'data' in app_config:
         if 'sources' in app_config['data']:
             config.app['data']['sources'] = app_config['data']['sources']
     if 'id' in app_config:
         config.app['id'] = app_config['id']
     if 'login' in app_config:
         if 'urls' in app_config['login']:
-            for url in app_config['login']['urls']:
-                config.app['login']['urls'][url['name']] = url['value']
+            if app_config['login']['urls']:
+                for url in app_config['login']['urls']:
+                    config.app['login']['urls'][url['name']] = url['value']
     if 'pythonpath' in app_config:
         config.app['pythonpath'] = app_config['pythonpath']
     if 'port' in app_config:
         config.app['port'] = app_config['port']
     if 'process' in app_config:
         if 'num_processes' in app_config['process']:
             config.app['process']['num_processes'] = app_config[
@@ -273,14 +275,16 @@
     if 'type' in app_config:
         config.app['type'] = app_config['type']
     if 'types' in app_config:
         for app_type in app_config['types']:
             app_type['launcher'] = get_config_from_package(
                 app_type['launcher'])
             config.app['types'][app_type['name']] = app_type
+    if 'xheaders' in app_config:
+        config.app['xheaders'] = app_config['xheaders']
     if 'wait_before_shutdown' in app_config:
         config.app['wait_before_shutdown'] = app_config['wait_before_shutdown']
 
 
 def process_components_config_section(config, components_config):
     """ Processes the components section from a configuration data dict.
 
@@ -423,10 +427,10 @@
     if 'purge_limit' in session_config:
         config.session['purge_limit'] = session_config['purge_limit']
     if 'encoder' in session_config:
         if session_config['encoder'] in config.session['encoders']:
             config.session['encoder'] = session_config['encoder']
         else:
             logger = logging.getLogger(__name__)
-            logger.critical("The session encoder \"{}\" is not defined."
-                            "".format(session_config['encoder']))
+            logger.critical("The session encoder \"%s\" is not defined.",
+                            session_config['encoder'])
             sysexits.exit_fatal(sysexits.EX_CONFIG)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/data.py` & `Firenado-0.9.0a1/firenado/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: UTF-8 -*-
-#
-# Copyright 2015-2021 Flavio Goncalves Garcia
+# Copyright 2015-2023 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -35,28 +33,28 @@
             return method(self, *args, **kwargs)
         return wrapper
     return f_wrapper
 
 
 class DataConnectedMixin(object):
     """ Data connected objects has data sources. This mixin prepares an
-    object to to have data sources set to it and retrieved from it.
+    object to have data sources set to it and retrieved from it.
 
     Example:
     >>> class MyClass(..., DataConnectedMixin):
     """
 
     @property
     def data_sources(self):
         """ Returns all connectors registered to the data connected instance.
         """
         return get_data_sources(self, '__data_sources')
 
     def get_data_source(self, name):
-        """ Returns a data source by it's name.
+        """ Returns a data source by its name.
         """
         return self.data_sources[name]
 
     def set_data_source(self, name, data_source):
         """ Add a data source to the data sources collection.
         """
         self.data_sources[name] = data_source
@@ -96,16 +94,18 @@
 class RedisConnector(Connector):
     """ Connects a redis database to a data connected instance.
     """
 
     def __init__(self, data_connected):
         self.__connection = None
         super(RedisConnector, self).__init__(data_connected)
+        self.__name = None
 
-    def configure(self, conf):
+    def configure(self, name, conf):
+        self.__name = name
         logger.info("Connecting to redis using the configuration: %s.", conf)
         import redis
         redis_conf = dict()
         redis_conf.update(conf)
         redis_conf.pop("connector")
         # TODO Handle connection error
         self.__connection = redis.Redis(**redis_conf)
@@ -130,79 +130,86 @@
                 if key in ['db', 'port']:
                     db_conf[key] = int(conf[key])
                 db_conf[key] = conf[key]
         return db_conf
 
 
 class SqlalchemyConnector(Connector):
-    """ Connects a sqlalchemy engine to a data connected instance. Sqlalchemy
-    support a big variety of relational database backends. The connection
-    returned by this handler contains a engine and session created by
-    sqlalchemy and the database backend name.
+    from sqlalchemy.orm import Session
+    """ Connects a sqlalchemy engine to a data connected instance.
+    Sqlalchemy support a big variety of relational database backends. The
+    connection returned by this handler contains an engine and session created
+    by sqlalchemy and the database backend name.
     """
 
     def __init__(self, data_connected):
         super(SqlalchemyConnector, self).__init__(data_connected)
+        self.__name = None
         self.__connection = {
             'backend': None,
             'session': {
                 'autoflush': True,
-                'autocommit': False,
                 'expire_on_commit': True,
                 'info': None
             }
         }
         self.__engine = None
 
-    def configure(self, conf):
+    def configure(self, name, conf):
+        self.__name = name
         from sqlalchemy import create_engine
         from sqlalchemy import exc, event, select
         # We will set the isolation level to READ UNCOMMITTED by default
         # to avoid the "cache" effect sqlalchemy has without this option.
         # Solution from: http://bit.ly/2bDq0Nv
         # TODO: Get the isolation level from data source conf
         engine_params = {
             'isolation_level': "READ UNCOMMITTED"
         }
 
         if "backend" in conf:
             if conf['backend'] == 'mysql':
                 # Setting connection default connection timeout for mysql
                 # backends as suggested on http://bit.ly/2bvOLxs
-                # TODO: ignore this if pool_recycle is defined on conf
                 engine_params['pool_recycle'] = 3600
 
         if "future" in conf:
             if conf['future']:
                 engine_params['future'] = True
 
         if "pool" in conf:
-            if "size" in conf['pool']:
-                engine_params['pool_size'] = conf['pool']['size']
-            if "max_overflow" in conf['pool']:
-                engine_params['max_overflow'] = conf['pool']['max_overflow']
             if "class" in conf['pool']:
                 engine_params['pool_class'] = conf['pool']['class']
                 if isinstance(engine_params['pool_class'], str):
                     engine_params['pool_class'] = config.get_from_string(
                         engine_params['pool_class'])
+            if "isolation_level" in conf['pool']:
+                engine_params['isolation_level'] = conf['pool'][
+                    'isolation_level']
+            if "max_overflow" in conf['pool']:
+                engine_params['max_overflow'] = conf['pool']['max_overflow']
+            if "pool_recycle" in conf['pool']:
+                engine_params['pool_recycle'] = conf['pool']['pool_recycle']
+            if "size" in conf['pool']:
+                engine_params['pool_size'] = conf['pool']['size']
 
         if "session" in conf:
             if "autoflush" in conf['session']:
                 self.__connection['session']['autoflush'] = conf['session'][
                     'autoflush']
-            if "autocommit" in conf['session']:
-                self.__connection['session']['autocommit'] = conf['session'][
-                    'autocommit']
             if "expire_on_commit" in conf['session']:
                 self.__connection['session']['expire_on_commit'] = conf[
                     'session']['expire_on_commit']
             if "info" in conf['session']:
                 self.__connection['session']['info'] = conf['session']['info']
 
+        if "url" not in conf:
+            logger.error("It is not possible to create sqlalchemy engine"
+                         "for %s datasource. Configuration: %s.", self.__name,
+                         conf)
         self.__engine = create_engine(conf['url'], **engine_params)
 
         @event.listens_for(self.__engine, "engine_connect")
         def ping_connection(connection, branch):
             # Adding ping connection event handler as described at the
             # pessimistic disconnect section of: http://bit.ly/2c8Sm2t
             logger.debug("Pinging sqlalchemy connection.")
@@ -217,15 +224,15 @@
             save_should_close_with_result = connection.should_close_with_result
             connection.should_close_with_result = False
             try:
                 # run a SELECT 1.   use a core select() so that
                 # the SELECT of a scalar value without a table is
                 # appropriately formatted for the backend
                 logger.debug("Testing sqlalchemy connection.")
-                connection.scalar(select([1]))
+                connection.scalar(select(1))
             except exc.DBAPIError as err:
                 logger.warning(err)
                 logger.warning("Firenado will try to reestablish the data "
                                "source connection.")
                 # catch SQLAlchemy's DBAPIError, which is a wrapper
                 # for the DBAPI's exception.  It includes a
                 # .connection_invalidated attribute which specifies if this
@@ -239,17 +246,16 @@
                     # connections are discarded.
                     connection.scalar(select([1]))
                     logger.warning("Data source connection reestablished.")
                 else:
                     raise
             finally:
                 # restore "close with result"
-                connection.should_close_with_result = \
-                    save_should_close_with_result
-
+                connection.should_close_with_result = (
+                    save_should_close_with_result)
         logger.info("Connecting to the database using the engine: %s.",
                     self.__engine)
         self.__connection['backend'] = conf['backend']
         # will just happen during the handler execution
 
     def get_connection(self):
         return self.__connection
@@ -258,20 +264,31 @@
         from sqlalchemy.exc import OperationalError
         try:
             self.__engine.connect()
         except OperationalError as op_error:
             logger.fatal("Error trying to connect to database: %s", op_error)
             sys.exit(errno.ECONNREFUSED)
 
-    def get_a_session(self, autoflush=True, autocommit=False,
-                      expire_on_commit=True, info=None):
-        from firenado.util.sqlalchemy_util import Session
-        Session.configure(bind=self.__engine, autoflush=autoflush,
-                          autocommit=autocommit,
-                          expire_on_commit=expire_on_commit, info=info)
+    def get_a_session(self, **kwargs) -> Session:
+        """ Return a session bind to the datasource engine.
+
+        Default parameters based on: https://bit.ly/3MjWDzF
+        :param dict kwargs:
+        :key bool autoflush: Default to True
+        :key bool expire_on_commit: Default to False
+        :key dict info: Default to None
+        :return Session:
+        """
+        autoflush = kwargs.get("autoflush", True)
+        expire_on_commit = kwargs.get("expire_on_commit", True)
+        info = kwargs.get("info")
+
+        from sqlalchemy.orm import sessionmaker
+        Session = sessionmaker(bind=self.__engine, autoflush=autoflush,
+                               expire_on_commit=expire_on_commit, info=info)
         return Session()
 
     @property
     def backend(self):
         return self.__connection['backend']
 
     @property
@@ -284,59 +301,89 @@
 
     def process_config(self, conf):
         db_conf = {
             'type': 'sqlalchemy',
         }
         for key in conf:
             # TODO Handle other properties and create the url if needed.
-            if key in ["future", "pool" "session", "url"]:
-                db_conf[key] = conf[key]
+            if key in ["db", "database", "dialect", "driver", "future", "host",
+                       "pass", "password", "pool", "port", "session", "url",
+                       "user", "username"]:
+                index = key
+                if index == "db":
+                    index = "database"
+                if index == "user":
+                    index = "username"
+                if index == "pass":
+                    index = "password"
+                db_conf[index] = conf[key]
         # TODO: Handler errors here
-        db_conf['backend'] = db_conf['url'].split(':')[0].split('+')[0]
+        if "url" in db_conf:
+            db_conf['backend'] = db_conf['url'].split(':')[0].split('+')[0]
+        else:
+            url = ""
+            if "dialect" in db_conf:
+                db_conf['backend'] = db_conf['dialect']
+                url = "%s" % db_conf.pop("dialect")
+                if "driver" in db_conf:
+                    url = "%s+%s" % (url, db_conf.pop("driver"))
+            if "username" in db_conf:
+                url = "%s://%s" % (url, db_conf.pop("username"))
+                if "password" in db_conf:
+                    from urllib.parse import quote
+                    url = "%s:%s" % (url, quote(db_conf.pop("password")))
+            if "host" in db_conf:
+                url = "%s@%s" % (url, db_conf.pop("host"))
+                if "port" in db_conf:
+                    url = "%s:%s" % (url, db_conf.pop("port"))
+            if "database" in db_conf:
+                url = "%s/%s" % (url, db_conf.pop("database"))
+            db_conf['url'] = url
         return db_conf
 
 
-def config_to_data_source(conf, data_connected):
-    """ Convert a data source conf to it's respective data source. We need
+def config_to_data_source(name, conf, data_connected):
+    """ Convert a data source conf to its respective data source. We need
     a data connected to use while instantiating the data source.
+    :param name: Datasource name
     :param conf: A data source confuration item
     :param data_connected: A data connected object
     :return: Connector
     """
     connector_conf = firenado.conf.data['connectors'][conf['connector']]
     # TODO: Test if handler was returned None. An error occurred.
     handler_class = config.get_from_module(connector_conf['module'],
                                            connector_conf['class'])
     data_source_instance = handler_class(data_connected)
     conf = data_source_instance.process_config(conf)
-    data_source_instance.configure(conf)
+    data_source_instance.configure(name, conf)
     return data_source_instance
 
 
 def configure_data_sources(data_sources, data_connected):
     """ Configure all data sources from configuration and set to the data
     connected.
     :param data_sources: List of data sources to be configured
     :param data_connected: Data connected object where the data sources will
     be configured.
     """
     if isinstance(data_sources, str):
         if data_sources in firenado.conf.data['sources']:
             logger.debug("Found data source [%s] in the list. Preceding with "
-                         "the configuration process." % data_sources)
+                         "the configuration process.", data_sources)
             conf = firenado.conf.data['sources'][data_sources]
-            data_source_instance = config_to_data_source(conf,
-                                                         data_connected)
+            data_source_instance = config_to_data_source(
+                data_sources, conf, data_connected)
             data_connected.set_data_source(data_sources, data_source_instance)
         else:
             logger.fatal("It was not possible to find [%s] in the list of "
                          "available data sources. Please fix the firenado "
                          "configuration file. Sometimes that could be only a "
                          "typo in one of app data sources to be created. Look "
-                         "at app.data.sources list." % data_sources)
+                         "at app.data.sources list.", data_sources)
             sys.exit(errno.ENOKEY)
         # TODO: Testing the connection
         # Without that the error will just happen during the handler execution
     elif isinstance(data_sources, list):
         for data_source in data_sources:
             configure_data_sources(data_source, data_connected)
     # TODO Throw an error here if it is not string or list
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/launcher.py` & `Firenado-0.9.0a1/firenado/launcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 
 from cartola import sysexits
 import firenado.conf
 from importlib import reload
 import logging
 import os
 import sys
-from tornado import gen
+import warnings
 
 logger = logging.getLogger(__name__)
 
 
 class FirenadoLauncher(object):
 
     def __init__(self, **settings):
@@ -66,33 +66,67 @@
         for handler in logging.root.handlers[:]:
             # clearing loggers, solution from: https://bit.ly/2yTchyx
             logging.root.removeHandler(handler)
         logging.basicConfig(level=firenado.conf.log['level'],
                             format=firenado.conf.log['format'])
 
     def load(self):
-        return None
+        raise NotImplementedError()
 
     def launch(self):
-        return None
+        raise NotImplementedError()
+
+    def shutdown(self):
+        raise NotImplementedError()
+
+
+def expect_list_mp(self, pattern_list, timeout=-1, searchwindowsize=-1,
+                   async_=False, **kw):
+    from pexpect import Expecter, searcher_re
+    '''This takes a list of compiled regular expressions and returns the
+    index into the pattern_list that matched the child output. The list may
+    also contain EOF or TIMEOUT(which are not compiled regular
+    expressions). This method is similar to the expect() method except that
+    expect_list() does not recompile the pattern list on every call. This
+    may help if you are trying to optimize for speed, otherwise just use
+    the expect() method.  This is called by expect().
+
+
+    Like :meth:`expect`, passing ``async_=True`` will make this return an
+    asyncio coroutine.
+    '''
+    if timeout == -1:
+        timeout = self.timeout
+    if 'async' in kw:
+        async_ = kw.pop('async')
+    if kw:
+        raise TypeError("Unknown keyword arguments: {}".format(kw))
+
+    exp = Expecter(self, searcher_re(pattern_list), searchwindowsize)
+    if async_:
+        from ._pexpect_async_patch import expect_async
+        return expect_async(exp, timeout)
+    else:
+        return exp.expect_loop(timeout)
 
 
 class ProcessLauncher(FirenadoLauncher):
     try:
         import pexpect
         process = None  # type: pexpect.spawn
     except ImportError:
         logger.debug("The pexpect module ins't isn't installed. Consider "
                      "installing it in order to launch applications using "
                      "ProcessLauncher.")
 
     def __init__(self, **settings):
-        super(ProcessLauncher, self).__init__(**settings)
+        super().__init__(**settings)
         self.process = None
         self.process_callback = None
+        self.process_callback_time = 100
         self.logfile = settings.get("logfile", None)
         self.command = None
         self.response = None
 
     def load(self):
         firenado_script = os.path.join(firenado.conf.ROOT, "bin",
                                        "firenado-cli.py")
@@ -108,49 +142,52 @@
             if self.port is not None:
                 port_parameter = "--port=%s" % self.port
                 self.command = "%s %s" % (self.command, port_parameter)
         else:
             socket_parameter = "--port=%s" % self.socket
             self.command = "%s %s" % (self.command, socket_parameter)
 
-    @gen.coroutine
-    def read_process(self):
+    async def read_process(self):
         import pexpect
         self.process_callback.stop()
         try:
             # Simple way to catch everything is wait for a new line:
             #
-            yield self.process.expect("\n", async_=True)
+            await self.process.expect("\n", async_=True)
         except pexpect.TIMEOUT:
-            logger.warning("Reached timeout")
-            pass
+            logger.debug("Reached timeout, getting back in the loop.")
         self.process_callback.start()
 
-    @gen.coroutine
-    def launch(self):
-        import pexpect
-        import tornado.ioloop
-        logger.info("Launching %s" % self.command)
-        parameters = {
-            'command': self.command,
-            'encoding': "utf-8"
-        }
-        if self.logfile is not None:
-            parameters['logfile'] = self.logfile
-        self.process = pexpect.spawn(**parameters)
-        yield self.process.expect(
-            [r"[Firenado server started successfully].*"], async_=True)
-        self.process_callback = tornado.ioloop.PeriodicCallback(
-            self.read_process,
-            400
-        )
-        self.process_callback.start()
+    async def launch(self):
+        with warnings.catch_warnings():
+            import pexpect
+            import tornado.ioloop
+            logger.info("Launching %s", self.command)
+            parameters = {
+                'command': self.command,
+                'encoding': "utf-8"
+            }
+            if self.dir:
+                parameters['cwd'] = self.dir
+            if self.logfile is not None:
+                parameters['logfile'] = self.logfile
+            self.process = pexpect.spawn(**parameters)
+            self.process.expect_list = expect_list_mp.__get__(self.process,
+                                                              pexpect.spawn)
+            warnings.simplefilter("ignore")
+            await self.process.expect(
+                [r"[Firenado server started successfully].*"], async_=True)
+            self.process_callback = tornado.ioloop.PeriodicCallback(
+                self.read_process,
+                self.process_callback_time
+            )
+            self.process_callback.start()
 
     def send(self, line):
-        logger.info("Sending line {}".format(line))
+        logger.info("Sending line %s", line)
         self.process.sendline(line)
 
     def shutdown(self):
         logger.warning("Shutting down process launcher.")
         self.process.terminate(force=True)
 
     def is_alive(self):
@@ -184,24 +221,35 @@
         import signal
         import tornado.httpserver
         signal.signal(signal.SIGTERM, self.sig_handler)
         signal.signal(signal.SIGINT, self.sig_handler)
         if os.name == "posix":
             signal.signal(signal.SIGTSTP, self.sig_handler)
         self.http_server = tornado.httpserver.HTTPServer(self.application)
+        if firenado.conf.app['xheaders'] is not None and type(
+                firenado.conf.app['xheaders']) == bool:
+            logger.debug("Setting http server xheaders as %s.",
+                         firenado.conf.app['xheaders'])
+            self.http_server.xheaders = firenado.conf.app['xheaders']
+        if firenado.conf.app['xheaders'] is not None and type(
+                firenado.conf.app['xheaders']) != bool:
+            logger.warning("The xheaders defined in the application section"
+                           "must be bool instead of %s. Ignoring the "
+                           "configuration item.",
+                           type(firenado.conf.app['xheaders']).__name__)
         listening_count = 0
         listening_what = "socket"
         if firenado.conf.app['socket'] or self.socket:
             from tornado.netutil import bind_unix_socket
             socket_path = firenado.conf.app['socket']
             if self.socket:
                 socket_path = self.socket
             socket = bind_unix_socket(socket_path)
             self.http_server.add_socket(socket)
-            logger.info("Firenado listening at socket ""%s" %
+            logger.info("Firenado listening at socket %s",
                         socket.getsockname())
             listening_count += 1
         else:
             listening_what = "addresses:port"
             if len(self.addresses):
                 for address in self.addresses:
                     if self.add_sockets(self.port, address):
@@ -209,25 +257,25 @@
             else:
                 if self.add_sockets(self.port):
                     listening_count += 1
         if listening_count:
             if listening_count > 1:
                 listening_what = "%ss" % listening_what
             logger.info("Firenado server started successfully. Listening at %s"
-                        " %s." % (listening_count, listening_what))
+                        " %s.", listening_count, listening_what)
             if firenado.conf.app['process']['num_processes'] is not None:
                 import tornado.process
                 num_processes = firenado.conf.app['process']['num_processes']
                 max_restarts = firenado.conf.app['process']['max_restarts']
                 num_processes_alert = num_processes
                 if num_processes == 0:
                     num_processes_alert = ("0 (assuming %s as cpu count)" %
                                            tornado.process.cpu_count())
                 logger.info("Tornado set to start %s processes with %s max "
-                            "restarts." % (num_processes_alert, max_restarts))
+                            "restarts.", num_processes_alert, max_restarts)
                 tornado.process.fork_processes(num_processes, max_restarts)
             tornado.ioloop.IOLoop.current().start()
         else:
             logger.critical("Firenado unable to start.")
             sysexits.exit_fatal(sysexits.EX_SOFTWARE)
 
     def sig_handler(self, sig, _):
@@ -236,86 +284,81 @@
         :param _: Frame is not being used
         """
         import tornado.ioloop
         from tornado.process import task_id
         tid = task_id()
         pid = os.getpid()
         if tid is None:
-            logger.warning("main process (pid %s) caught signal: %s" %
-                           (pid, sig))
+            logger.warning("main process (pid %s) caught signal: %s", pid, sig)
         else:
-            logger.warning("child %s (pid %s) caught signal: %s" %
-                           (tid, pid, sig))
+            logger.warning("child %s (pid %s) caught signal: %s", tid, pid,
+                           sig)
         tornado.ioloop.IOLoop.current().add_callback_from_signal(self.shutdown)
 
     def add_sockets(self, port, address=None):
         from socket import gaierror
         try:
             from tornado.netutil import bind_sockets
             if address:
                 sockets = bind_sockets(port, address.strip())
             else:
                 sockets = bind_sockets(port)
                 address = "127.0.0.1"
             self.http_server.add_sockets(sockets)
-            logger.info("Firenado listening at http://%s:%s." %
-                        (address.strip(), port))
+            logger.info("Firenado listening at http://%s:%s.", address.strip(),
+                        port)
             return True
         except gaierror as error:
-            logger.error("Firenado failed to listen at http://%s:%s."
-                         % (address.strip(), port))
+            logger.error("Firenado failed to listen at http://%s:%s.",
+                         address.strip(), port)
         except OSError as error:
-            logger.error("Firenado failed to listen at http://%s:%s. "
-                         "Check if another process is listening at "
-                         "this port or if you provided a dns name and"
-                         "the correspondent ip in the addresses"
-                         "configuration or if the machine owns the ip "
-                         "Fireando will start to listen." %
-                         (address, port))
+            logger.error("Firenado failed to listen at http://%s:%s. Check if "
+                         "another process is listening at this port or if you "
+                         "provided a dns name and the correspondent ip in the "
+                         "addresses configuration or if the machine owns the "
+                         "ip Fireando will start to listen.", address, port)
         return False
 
     def shutdown(self):
         import time
         import tornado.ioloop
         from tornado.process import task_id
         tid = task_id()
         pid = os.getpid()
         if tid is None:
-            logger.info("main process (pid %s): stopping http server" % pid)
+            logger.info("main process (pid %s): stopping http server.", pid)
         else:
-            logger.info("child %s (pid %s): stopping http server" % (tid, pid))
+            logger.info("child %s (pid %s): stopping http server.", tid, pid)
         for key, component in self.application.components.items():
             component.shutdown()
         self.http_server.stop()
 
         io_loop = tornado.ioloop.IOLoop.current()
 
         if self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN == 0:
             io_loop.stop()
             if tid is None:
-                logger.info("main process (pid %s): application is down" % pid)
+                logger.info("main process (pid %s): application is down", pid)
             else:
-                logger.info("child %s (pid %s): application is down" %
-                            (tid, pid))
+                logger.info("child %s (pid %s): application is down", tid, pid)
         else:
             if tid is None:
                 logger.info("main process (pid %s): shutdown in %s seconds "
-                            "..." %
-                            (pid, self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN))
+                            "...", pid, self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN)
             else:
-                logger.info("child %s (pid %s): shutdown in %s seconds ..." %
-                            (tid, pid, self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN))
+                logger.info("child %s (pid %s): shutdown in %s seconds ...",
+                            tid, pid, self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN)
             deadline = time.time() + self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN
 
             def stop_loop():
                 now = time.time()
                 if now < deadline:
                     io_loop.add_timeout(now + 1, stop_loop)
                 else:
                     io_loop.stop()
                     if tid is None:
                         logger.info("main process (pid %s): application is "
-                                    "down" % pid)
+                                    "down", pid)
                     else:
-                        logger.info("child %s (pid %s): application is down" %
-                                    (tid, pid))
+                        logger.info("child %s (pid %s): application is down",
+                                    tid, pid)
             stop_loop()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/management/__init__.py` & `Firenado-0.9.0a1/firenado/management/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/management/commands.py` & `Firenado-0.9.0a1/firenado/management/commands.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/management/management.py` & `Firenado-0.9.0a1/firenado/management/management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,19 +30,18 @@
 command_categories = dict()
 
 
 def run_from_command_line():
     """ Run Firenado's management commands from a command line
     """
     for commands_conf in firenado.conf.management['commands']:
-        logger.debug("Loading %s commands from %s." % (
-            commands_conf['name'],
-            commands_conf['module']
-        ))
-        exec('import %s' % commands_conf['module'])
+        logger.debug("Loading %s commands from %s.", commands_conf['name'],
+                     commands_conf['module'])
+        # from https://stackoverflow.com/a/19221024/2887989
+        __import__(commands_conf['module'])
     command_index = 1
     for arg in sys.argv[1:]:
         command_index += 1
         if arg[0] != "-":
             break
     parser = FirenadoArgumentParser(prog=os.path.split(sys.argv[0])[1],
                                     add_help=False)
@@ -50,14 +49,15 @@
     parser.add_argument("command", default="help", help="Command to executed")
 
     try:
         namespace = parser.parse_args(sys.argv[1:command_index])
         if not command_exists(namespace.command):
             show_command_line_usage(parser)
         else:
+
             run_command(namespace.command, sys.argv[command_index-1:])
     except FirenadoArgumentError:
         show_command_line_usage(parser, True)
 
 
 def get_command_header(parser, usage_message="", usage=False):
     """ Return the command line header
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/management/tasks.py` & `Firenado-0.9.0a1/firenado/management/tasks.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/management/templates/project/firenado.yml.txt` & `Firenado-0.9.0a1/firenado/management/templates/project/firenado.yml.txt`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/schedule.py` & `Firenado-0.9.0a1/firenado/schedule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .tornadoweb import TornadoComponent
-from cartola import config, sysexits
+from cartola import config, exception, sysexits
 from datetime import datetime, timedelta
 import logging
 import sys
 import tornado.ioloop
 
 logger = logging.getLogger(__name__)
 
@@ -37,19 +37,20 @@
                  "instead of installing croniter directly to avoid any "
                  "version compatibility error.\n The croniter package"
                  "installed by extras was tested with firenado and no errors "
                  "are expected during the execution.")
     sys.exit(sysexits.EX_FATAL_ERROR)
 
 
-def next_from_cron(cron):
-    """ Return next schedule run offset from now to the time of execution
+def next_from_cron(cron: str) -> datetime:
+    """ Return a datatetime object with the next execution based on the informed
+    cron string and the current time.
 
-    :param cron: The cron string
-    :return:
+    :param str cron: The cron string
+    :return datetime: A datetime object with the next execution
     """
     iterator = croniter(cron, datetime.now())
     return iterator.get_next(datetime)
 
 
 class Scheduler(object):
 
@@ -68,89 +69,97 @@
         self._jobs = {}
         self._interval = kwargs.get("interval", 1000)
         self._name = None
         self.component = component
         self._periodic_callback = None
 
     @property
+    def app_component(self) -> TornadoComponent:
+        """ Shortcut to self.component.app_component
+
+        :return: TornadoComponent
+        """
+        return self.component.app_component
+
+    @property
     def id(self):
         return self._id
 
     @property
     def jobs(self):
         return [job for _, job in self._jobs.items()]
 
     @property
     def name(self):
         return self._name
 
     @property
-    def can_run(self):
+    def can_run(self) -> bool:
+        """ Indicates if the scheduler can run
+        """
         return self._can_run
 
     def add_job(self, job):
-        logger.debug("Adding job %s into the scheduler [id: %s, name: %s]." %
-                     (job.id, self.id, self.name))
+        logger.debug("Adding job %s into the scheduler [id: %s, name: %s].",
+                     job.id, self.id, self.name)
         self._jobs[job.id] = job
 
     def get_job(self, job_id):
         return self._jobs.get(job_id)
 
     def initialize(self, **kwargs):
         self._id = kwargs.get("id")
         self._name = kwargs.get("name")
-        logger.debug("Initializing scheduler [id: %s, name: %s]." % (
-            self.id, self.name))
+        logger.debug("Initializing scheduler [id: %s, name: %s].", self.id,
+                     self.name)
 
     def load_jobs(self):
         raise NotImplementedError
 
     def remove_job(self, job_id):
-        logger.debug("Removing job %s from the scheduler [id: %s, name: %s]."
-                     % (job_id, self.id, self.name))
+        logger.debug("Removing job %s from the scheduler [id: %s, name: %s].",
+                     job_id, self.id, self.name)
         job = self.get_job(job_id)
         if job is None:
             return None
         del(self._jobs[job_id])
         return job.id
 
     def run(self):
         self.load_jobs()
-        logger.debug("Scheduler [id: %s, name: %s] interval set to %sms." %
-                     (self.id, self.name, self._interval))
+        logger.debug("Scheduler [id: %s, name: %s] interval set to %sms.",
+                     self.id, self.name, self._interval)
         self._periodic_callback = tornado.ioloop.PeriodicCallback(
             self._manage_jobs, self._interval)
         self._periodic_callback.start()
 
     def _manage_jobs(self):
-        logger.debug("Scheduler [id: %s, name: %s] managing jobs." %
-                     (self.id, self.name))
+        logger.debug("Scheduler [id: %s, name: %s] managing jobs.", self.id,
+                     self.name)
         logger.debug("Scheduler [id: %s, name: %s] stopping periodic callback."
-                     % (self.id, self.name))
+                     , self.id, self.name)
         self._periodic_callback.stop()
         for job in self.jobs:
             if not job.already_scheduled:
                 logger.debug("Job %s from Scheduler [id: %s, name: %s] isn't "
-                             "scheduled yet." % (job.hard_id, self.id,
-                                                 self.name))
+                             "scheduled yet.", job.hard_id, self.id, self.name)
                 if job.must_schedule:
-                    logger.debug(
-                        "Job %s from Scheduler [id: %s, name: %s] must be "
-                        "scheduled to run at %s." % (
-                            job.hard_id, self.id, self.name, job.next_run))
+                    logger.debug("Job %s from Scheduler [id: %s, name: %s] "
+                                 "must be scheduled to run at %s.",
+                                 job.hard_id, self.id, self.name, job.next_run)
                     job.schedule()
             else:
-                logger.debug("Job %s from Scheduler [id: %s, name: %s] already"
-                             "scheduled." % (job.hard_id, self.id,
-                                             self.name))
+                logger.debug("Job %s from Scheduler [id: %s, name: %s] "
+                             "already scheduled.", job.hard_id, self.id,
+                             self.name)
 
-        logger.debug("Scheduler [id: %s, name: %s] ending of managing jobs." %
-                     (self.id, self.name))
+        logger.debug("Scheduler [id: %s, name: %s] ending of managing jobs.",
+                     self.id, self.name)
         logger.debug("Scheduler [id: %s, name: %s] starting periodic callback."
-                     % (self.id, self.name))
+                     , self.id, self.name)
         self._periodic_callback.start()
 
 
 class ConfScheduler(Scheduler):
 
     def __init__(self, scheduled_component, **kwargs):
         super(ConfScheduler, self).__init__(scheduled_component, **kwargs)
@@ -169,18 +178,18 @@
                         job_conf['class'])
                 if job_resolved_class is None:
                     logger.warning("Firenado Scheduled Job Error:\n    The "
                                    "scheduled class job %s was not found "
                                    "in the file:\n        %s\n    Job id: %s"
                                    "\n    Scheduler: [id: %s, name: %s]"
                                    "\n        Config: %s\n"
-                                   "\n    Please fix this issue.\n" %
-                                   (job_conf['class'],
-                                    self.component.get_complete_config_file(),
-                                    job_id, self.id, self.name, job_conf))
+                                   "\n    Please fix this issue.\n",
+                                   job_conf['class'],
+                                   self.component.get_complete_config_file(),
+                                   job_id, self.id, self.name, job_conf)
                 else:
                     if job_id is None:
                         logger.warning(
                             "Firenado Scheduled Job Error:\n    The "
                             "scheduled job id not defined in the "
                             "file:\n        %s"
                             "\n    Scheduler: [id: %s, name: %s]"
@@ -194,35 +203,35 @@
                             logger.warning(
                                 "Firenado Scheduled Job Error:\n    The "
                                 "scheduled must have a cron or date or "
                                 "interval defined in the file:\n        %s\n  "
                                 "  Job id: %s\n    Scheduler: [id: %s, "
                                 "name: %s]\n        Config: %s\n"
                                 "\n    Please define either a cron string or "
-                                "date.\n" %
-                                (self.component.get_complete_config_file(),
-                                 job_id, self.id, self.name, job_conf))
+                                "date.\n",
+                                self.component.get_complete_config_file(),
+                                job_id, self.id, self.name, job_conf)
                         else:
                             self.add_job(job_resolved_class(self, **job_conf))
 
     def initialize(self):
         has_error = False
         if self._conf is None:
             logger.warning("It is not possible to initialize the scheduler "
                            "because the configuration is missing.")
             has_error = True
         if "id" not in self._conf:
             logger.warning("It is not possible to initialize the scheduler "
                            "because id is missing in the configuration "
-                           "provided.\n Config: %s" % self._conf)
+                           "provided.\n Config: %s", self._conf)
             has_error = True
         if "name" not in self._conf:
             logger.warning("It is not possible to initialize the scheduler "
                            "because name is missing in the configuration "
-                           "provided.\n Config: %s" % self._conf)
+                           "provided.\n Config: %s", self._conf)
             has_error = True
 
         if not has_error:
             self._can_run = True
             super(ConfScheduler, self).initialize(**self._conf)
 
         if "interval" in self._conf:
@@ -236,14 +245,26 @@
         self._id = kwargs.get('id')
         self._date = kwargs.get('date')
         self._cron = kwargs.get('cron')
         self._interval = kwargs.get('interval')
         self._periodic_callback = None
 
     @property
+    def component(self) -> "ScheduledTornadoComponent":
+        """ Return scheduler's component
+        """
+        return self._scheduler.component
+
+    @property
+    def app_component(self) -> TornadoComponent:
+        """ Shortcut to  self.component.app_component
+        """
+        return self.component.app_component
+
+    @property
     def id(self):
         return self._id
 
     @property
     def hard_id(self):
         return "%s:%s:%s" % (self._id, self.__class__.__name__, id(self))
 
@@ -277,40 +298,43 @@
     @property
     def must_schedule(self):
         return self.next_interval > 0
 
     def schedule(self):
         next_interval = self.next_interval
         logger.debug("Job %s from Scheduler [id: %s, name: %s] scheduled to "
-                     "run at next interval of %sms." % (self.hard_id,
-                                                        self._scheduler.id,
-                                                        self._scheduler.name,
-                                                        self.next_interval))
+                     "run at next interval of %sms.", self.hard_id,
+                     self._scheduler.id, self._scheduler.name,
+                     self.next_interval)
         self._periodic_callback = tornado.ioloop.PeriodicCallback(
             self._run_job, next_interval)
         self._periodic_callback.start()
 
     async def _run_job(self):
         """ Run the job
         :return None:
         """
         self._periodic_callback.stop()
-        logger.debug(
-            "Running job %s from Scheduler [id: %s, name: %s]." % (
-                self.hard_id, self._scheduler.id, self._scheduler.name))
-        future = self.run()
-        if future is not None:
-            logger.debug(
-                "Running job %s from Scheduler [id: %s, name: %s] "
-                "asynchronously. " % (self.hard_id, self._scheduler.id,
-                                      self._scheduler.name))
-            await future
-        logger.debug(
-            "Job %s removed from Scheduler [id: %s, name: %s]" % (
-                self.hard_id, self._scheduler.id, self._scheduler.name))
+        logger.debug("Running job %s from Scheduler [id: %s, name: %s].",
+                     self.hard_id, self._scheduler.id, self._scheduler.name)
+        try:
+            future = self.run()
+            if future:
+                logger.debug("Running job %s from Scheduler [id: %s, name: "
+                             "%s] asynchronously.", self.hard_id,
+                             self._scheduler.id, self._scheduler.name)
+                await future
+        except:
+            logger.error("A non handled exception was cough while running the "
+                         "job %s:", self.hard_id,
+                         exc_info=exception.full_exc_info())
+            logger.error("Please handle the exception to fix the job "
+                         "execution and avoid breaking the scheduler.")
+        logger.debug("Job %s removed from Scheduler [id: %s, name: %s]",
+                     self.hard_id, self._scheduler.id, self._scheduler.name)
         self._periodic_callback = None
         return
 
     def run(self):
         pass
 
 
@@ -337,27 +361,26 @@
         if name in self.schedulers:
             return self.schedulers[name]
         return None
 
     def _config_schedule_component(self):
         if "interval" in self.schedule_conf():
             self._interval = self.conf['interval']
-        logger.debug("Scheduled component %s interval set to %sms." %
-                     (self.name, self._interval))
+        logger.debug("Scheduled component %s interval set to %sms.", self.name,
+                     self._interval)
         if "schedulers" in self.schedule_conf():
-            logger.debug("Initializing %s schedulers." % self.name)
+            logger.debug("Initializing %s schedulers.", self.name)
             self._initialize_schedulers()
         else:
             logger.warning("No scheduler was defined in the scheduled "
                            "component %s.\n\n%s\n* It is necessary either "
                            "define schedulers or scheduler loaders in the \n*"
                            " %s config file. \n* %s-- Firenado scheduled "
-                           "component\n%s\n" %
-                           (self.name, "*" * 70,
-                            self.get_config_file(), " " * 37, "*" * 70))
+                           "component\n%s\n", self.name, "*" * 70,
+                           self.get_config_file(), " " * 37, "*" * 70)
 
     def _initialize_schedulers(self):
         for scheduler_conf in self.conf['schedulers']:
             scheduler = ConfScheduler(self, interval=self._interval,
                                       conf=scheduler_conf)
             scheduler.initialize()
             if scheduler.can_run:
@@ -366,12 +389,12 @@
 
     def schedule_conf(self):
         return self.conf
 
     def initialize(self):
         if self.has_conf:
             logger.debug("Configuration file found. Starting scheduled "
-                         "component %s initialization." % self.name)
+                         "component %s initialization.", self.name)
             self._config_schedule_component()
         else:
             logger.warning("No configuration file was found. Scheduled"
                            "component %s won't initialize")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/service.py` & `Firenado-0.9.0a1/firenado/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .sqlalchemy import with_session
 import functools
 import importlib
+import logging
 
 
-class FirenadoService(object):
+logger = logging.getLogger(__name__)
+
+
+class FirenadoService:
     """ Base class to handle services. A Firenado service is usually connected
     to a handler or a service.
     The developer can add extra configuration using the configuration_service
     method and can get a data source from the data connected instance using
     either get_data_sources or get_data_source methods.
     """
 
@@ -67,14 +72,23 @@
         invert_op = getattr(self.consumer, "get_data_connected", None)
         if callable(invert_op):
             return self.consumer.get_data_connected()
         return self.consumer.data_connected
 
 
 def served_by(service, attribute_name=None):
+    import warnings
+    warnings.warn(
+        "The \"firenado.service.served_by\" function is depreciated. "
+        "Please use firenado.service.with_service instead.",
+        DeprecationWarning, 2)
+    return with_service(service, attribute_name)
+
+
+def with_service(service, attribute_name=None):
     """ Decorator that connects a service to a service consumer.
     """
 
     def f_wrapper(method):
         @functools.wraps(method)
         def wrapper(self, *args, **kwargs):
             if isinstance(service, str):
@@ -110,7 +124,16 @@
                     must_set_service = True
             if must_set_service:
                 setattr(self, service_attribute, service_class(self))
             return method(self, *args, **kwargs)
 
         return wrapper
     return f_wrapper
+
+
+def sessionned(*args, **kwargs):
+    import warnings
+    warnings.warn(
+        "The \"firenado.service.sessioned\" module is depreciated. "
+        "Please use firenado.sqlalchemy.with_session  instead.",
+        DeprecationWarning, 2)
+    return with_session(*args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/session.py` & `Firenado-0.9.0a1/firenado/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from cartola import fs, security
-import firenado.conf
-from firenado.config import get_class_from_config
 import functools
 import logging
 import os
+
 import tornado
 import tornado.ioloop
 import tornado.web
+from cartola.fs import read as fs_read
+from cartola.fs import touch as fs_touch
+from cartola.fs import write as fs_write
+from cartola.security import random_string
+
+import firenado.conf
+from firenado.config import get_class_from_config
 
 logger = logging.getLogger(__name__)
 
 
 class SessionEngine(object):
-    """SessionEngine provides session support to an application.
+    """Provides session support to an application.
     """
 
     def __init__(self, session_aware_instance):
         self.session_aware_instance = None
         self.session_handler = None
         self.session_callback = None
         self.callback_time = None
         self.callback_hiccup = firenado.conf.session['callback_hiccup'] * 1000
-
-        # TODO: By the way session could be disabled. How do we 
-        # handle that?
+        # TODO: By the way session could be disabled. How to handle that?
         # TODO: check if session type exists. Maybe disable it if type is not
         # defined. We need to inform the error here
         if firenado.conf.session['enabled']:
             # Transforming session callback time to milliseconds.
             self.callback_time = firenado.conf.session['callback_time'] * 1000
             logging.debug("Session periodic callback will be set with time of "
                           "%sms." % self.callback_time)
@@ -70,15 +73,15 @@
             encoder_class = get_class_from_config(
                 firenado.conf.session['encoders'][
                     firenado.conf.session['encoder']
                 ]
             )
             self.session_encoder = encoder_class()
 
-    def get_session(self, request_handler):
+    async def get_session(self, request_handler):
         """Returns a valid session object. This session is handler by the
         session handler defined on the application configuration. """
         if firenado.conf.session['enabled']:
             session = Session(self)
             cookie_created_on_request = False
             session_id = SessionHandler.get_session_id_cookie(request_handler)
             if session_id is None:
@@ -95,53 +98,56 @@
                     session = self.__renew_session(request_handler)
             if not cookie_created_on_request:
                 session_data = self.decode_session_data(
                     self.session_handler.read_stored_session(session_id))
                 session = Session(self, session_data, session_id)
             return session
 
-    def store_session(self, request_handler):
+    async def store_session(self, request_handler):
         """Sends the session data to be stored by the session handler defined
         on the application configuration. """
         if firenado.conf.session['enabled']:
             session_id = request_handler.session.id
-            # If session was destroyed than we gonna handle it differently
+            # If session was destroyed than we're going to handle it
+            # differently
             # If session id is None than ignored (it is probably a redirect
             # leftover from security)
             if session_id is not None:
                 if not request_handler.session.is_destroyed():
                     encoded_session_data = self.encode_session_data(
                         request_handler.session.get_data())
+                    params = request_handler.session.get_params()
                     if request_handler.session.is_changed():
                         self.session_handler.write_stored_session(
                             session_id,
-                            encoded_session_data
+                            encoded_session_data,
+                            **params
                         )
                 else:
                     # Generating a new session
                     logger.debug("Dispatching session %s destruction to the "
-                                 "session handler." % session_id)
+                                 "session handler.", session_id)
                     self.session_handler.destroy_stored_session(session_id)
 
     def encode_session_data(self, data):
         return self.session_encoder.encode(data)
 
     def decode_session_data(self, data):
         return self.session_encoder.decode(data)
 
     def get_session_aware_instance(self):
         return self.session_aware_instance
 
     def set_purge_normal(self):
         self.session_callback.callback_time = self.callback_time
-        logger.debug("No hiccups. Callback in %sms." % self.callback_time)
+        logger.debug("No hiccups. Callback in %sms.", self.callback_time)
 
     def set_purge_hiccup(self):
         self.session_callback.callback_time = self.callback_hiccup
-        logger.warning("Purge hiccup in %sms." % self.callback_hiccup)
+        logger.warning("Purge hiccup in %sms.", self.callback_hiccup)
 
     def __renew_session(self, request_handler):
         if firenado.conf.session['enabled']:
             session = Session(self)
             session_id = SessionHandler.create_session_id_cookie(
                 request_handler)
             session.id = session_id
@@ -175,14 +181,15 @@
 
 class Session(object):
 
     def __init__(self, engine, data=None, sess_id=None):
         self.__engine = engine
         self.id = sess_id
         self.__data = {} if data is None else data
+        self.__params = {}
         self.__destroyed = False
         self.__changed = False
 
     def clear(self):
         """ Clear all data stored into the session. This is not 
         renewing/creating a new session id. If you want that use 
         session.destroy() """
@@ -203,14 +210,18 @@
             return self.__data[key]
         return None
 
     def get_data(self):
         self.__lock_if_destroyed()
         return self.__data.copy()
 
+    def get_params(self):
+        self.__lock_if_destroyed()
+        return self.__params.copy()
+
     def has(self, key):
         self.__lock_if_destroyed()
         """ Returns if session data has some data stored by a given key. """
         return key in self.__data
 
     def delete(self, key):
         self.__lock_if_destroyed()
@@ -226,50 +237,54 @@
     def is_changed(self):
         return self.__changed
 
     def __lock_if_destroyed(self):
         if self.is_destroyed():
             raise SessionDestroyedError()
 
-    def set(self, key, value):
+    def set(self, key, value, **kwargs):
         """ Set a value into the session data labeled by a given key """
         self.__lock_if_destroyed()
         self.__data[key] = value
+        self.__params[key] = kwargs
         self.__changed = True
 
 
 class SessionDestroyedError(tornado.web.HTTPError):
 
-    def __init__(self, status_code, log_message=None, *args, **kwargs):
-        message = "The session was destroyed. It is necessary a renew the " \
-                  "session before use it again."
+    def __init__(self, status_code=500, log_message=None, *args, **kwargs):
+        message = ("The session is already destroyed. It is necessary to renew"
+                   " the session before using it again."
+                   if log_message is None else log_message)
         super(SessionDestroyedError, self).__init__(
-            505, message, *args, **kwargs)
+            status_code, message, *args, **kwargs)
 
 
-class SessionHandler(object):
+class SessionHandler:
+
+    life_time: int
 
     def __init__(self, engine):
         self.engine = engine
         self.settings = {}
 
     def create_session(self, session_id, data):
-        pass
+        raise NotImplementedError
 
     def read_stored_session(self, session_id):
-        pass
+        raise NotImplementedError
 
-    def write_stored_session(self, session_id, data):
-        pass
+    def write_stored_session(self, session_id, data, **kwargs):
+        raise NotImplementedError
 
     def destroy_stored_session(self, session_id):
-        pass
+        raise NotImplementedError
 
     def purge_expired_sessions(self):
-        pass
+        raise NotImplementedError
 
     @staticmethod
     def create_session_id_cookie(request_handler):
         session_id = SessionHandler.__generate_session_id()
         if 'cookie_secret' in request_handler.application.settings:
             settings = SessionHandler.__session_id_cookie_settings(secret=True)
             expires_days = settings.pop('expires_days')
@@ -313,15 +328,15 @@
 
     @staticmethod
     def __generate_session_id():
         """
         Retrieves the session id generator function from the configuration.
 
         It is possible for a developer create a new session id generator
-        function and and use it here.
+        function and use it here.
 
         Returns:
             A probably unique session id.
         """
         session_id_generator = get_class_from_config(
             firenado.conf.session['id_generators'][
                 firenado.conf.app['session']['id_generator']
@@ -335,36 +350,41 @@
         session_engine_instance = session_engine_class(obj)
         setattr(obj, session_engine_attribute, session_engine_instance)
     return getattr(obj, session_engine_attribute)
 
 
 def read(method):
     @functools.wraps(method)
-    def wrapper(self, *args, **kwargs):
+    async def wrapper(self, *args, **kwargs):
         if firenado.conf.session['enabled']:
-            session = self.application.session_engine.get_session(self)
+            session = await self.application.session_engine.get_session(self)
             self.session = session
             logging.debug("Reading session %s." % self.session.id)
         return method(self, *args, **kwargs)
     return wrapper
 
 
 def write(method):
     @functools.wraps(method)
     def wrapper(self, *args, **kwargs):
+        async def write_session_callback():
+            logging.debug("Writing session %s." % self.session.id)
+            await self.application.session_engine.store_session(self)
+
         retval = method(self, *args, **kwargs)
         if firenado.conf.session['enabled']:
             if self.session is None:
                 logging.error("The handler session is None. Something wrong"
                               " happened during the handler execution. The"
                               " current handler status is: %s." %
                               self.get_status())
             else:
-                logging.debug("Writing session %s." % self.session.id)
-                self.application.session_engine.store_session(self)
+                tornado.ioloop.IOLoop.current().add_callback(
+                    callback=write_session_callback
+                )
         return retval
     return wrapper
 
 
 class FileSessionHandler(SessionHandler):
     """
     Session handler that deals with file data stored in files.
@@ -387,76 +407,73 @@
             self.path = firenado.conf.TMP_APP_PATH
 
     def create_session(self, session_id, data):
         # TODO: What could possibly go wrong here? Let's handle it!
         if os.path.exists(firenado.conf.session['file']['path']):
             session_file = os.path.join(self.path,
                                         self.__get_filename(session_id))
-            fs.touch(session_file)
+            fs_touch(session_file)
             self.write_stored_session(session_id, data)
 
     def read_stored_session(self, session_id):
         import binascii
         session_file = os.path.join(self.path, self.__get_filename(session_id))
-        timed_data = fs.read(session_file)
+        timed_data = fs_read(session_file)
         return binascii.unhexlify(timed_data.split("--")[0])
 
-    def write_stored_session(self, session_id, data):
+    def write_stored_session(self, session_id, data, **kwargs):
         import binascii
         import time
         timed_data = "%s--%s" % (binascii.hexlify(data).decode("ascii"),
                                  int(time.time()))
         session_file = os.path.join(self.path, self.__get_filename(session_id))
-        fs.write(session_file, timed_data)
+        fs_write(session_file, timed_data)
 
     def destroy_stored_session(self, session_id):
-        logger.debug("Destroying session %s." % session_id)
+        logger.debug("Destroying session %s.", session_id)
         try:
             session_file = os.path.join(
                 self.path,
                 self.__get_filename(session_id)
             )
             os.remove(session_file)
-            logger.debug("Session %s destroyed." % session_id)
+            logger.debug("Session %s destroyed.", session_id)
         except OSError:
             # TODO Why we are deleting the session file twice?
             pass
 
     def purge_expired_sessions(self):
         import time
         """ A file session contains a data separated by --
         The first part is the hexadecimal representation of the encoded session
         data. Second is the epoch of the last write.
         If current epoch - file epoch is lower than the session life time then
         we need to delete this file.
         """
         logger.debug("File handler looking for expired sessions.")
         self.engine.session_callback.stop()
-        logging.debug("Session periodic callback stopped by the file "
-                      "handler.")
+        logger.debug("Session periodic callback stopped by the file handler.")
         purge_count = 0
         purge_hiccup = False
         for dirname, dirnames, filenames in os.walk(self.path):
             for filename in filenames:
                 file_path = os.path.join(self.path, filename)
                 sess_id = filename.split(".")[0].split("_")[-1]
-                timed_data = fs.read(file_path)
+                timed_data = fs_read(file_path)
                 last_write = timed_data.split("--")[1]
                 age = int(time.time()) - int(last_write)
                 if age > self.life_time:
                     logging.debug("Session %s is expired. Removing file "
                                   "from the session path." % sess_id)
                     os.remove(file_path)
                     purge_count += 1
             if purge_count == firenado.conf.session['purge_limit']:
                 purge_hiccup = True
-                logger.warning(
-                    "Expired 500 sessions. Exiting the call and waiting for "
-                    "purge hiccup."
-                )
+                logger.warning("Expired 500 sessions. Exiting the call and "
+                               "waiting for purge hiccup.")
                 break
         if purge_hiccup:
             self.engine.set_purge_hiccup()
         else:
             self.engine.set_purge_normal()
         self.engine.session_callback.start()
         logging.debug("Session periodic callback resumed by the file "
@@ -468,16 +485,17 @@
 
     def __get_filename(self, session_id):
         return 'firenado_%s.sess' % session_id
 
 
 class RedisSessionHandler(SessionHandler):
     """
-    Session handler that deals with file data stored  in a redis database.
+    A session handler that deals with data stored in a redis database.
     """
+
     def __init__(self, engine):
         SessionHandler.__init__(self, engine)
         self.data_source = None
 
     def configure(self):
         self.life_time = firenado.conf.session['life_time']
         self.data_source = (
@@ -490,24 +508,24 @@
         self.write_stored_session(session_id, data)
 
     def read_stored_session(self, session_id):
         key = self.__get_key(session_id)
         self.data_source.get_connection().expire(key, self.life_time)
         return self.data_source.get_connection().get(key)
 
-    def write_stored_session(self, session_id, data):
+    def write_stored_session(self, session_id, data, **kwargs):
         key = self.__get_key(session_id)
         self.data_source.get_connection().set(key, data)
         self.data_source.get_connection().expire(key, self.life_time)
 
     def destroy_stored_session(self, session_id):
-        logger.debug("Destroying session %s." % session_id)
+        logger.debug("Destroying session %s.", session_id)
         key = self.__get_key(session_id)
         self.data_source.get_connection().delete(key)
-        logger.debug("Session %s destroyed." % session_id)
+        logger.debug("Session %s destroyed.", session_id)
 
     def purge_expired_sessions(self):
         """ On Redis we don't destroy expired sessions per-se.
         If a session has no ttl we just reset an expiration value to it.
         """
         logger.debug("Redis handler looking for sessions without ttl.")
         self.engine.session_callback.stop()
@@ -515,25 +533,22 @@
                       "handler.")
         keys = self.data_source.get_connection().keys(self.__get_key("*"))
         purge_count = 0
         purge_hiccup = False
         for key in keys:
             ttl = self.data_source.get_connection().ttl(key)
             if ttl == -1:
-                logger.warning(
-                    "Session %s without ttl. Setting expiration now." % key
-                )
+                logger.warning("Session %s without ttl. Setting expiration "
+                               "now.", key)
                 self.data_source.get_connection().expire(key, self.life_time)
                 purge_count += 1
                 if purge_count == firenado.conf.session['purge_limit']:
                     purge_hiccup = True
-                    logger.warning(
-                        "Set ttl to 500 sessions. Exiting the call and waiting"
-                        " for purge hiccup."
-                    )
+                    logger.warning("Set ttl to 500 sessions. Exiting the call"
+                                   " and waiting for purge hiccup.")
                     break
         if purge_hiccup:
             self.engine.set_purge_hiccup()
         else:
             self.engine.set_purge_normal()
         self.engine.session_callback.start()
         logging.debug("Session periodic callback resumed by the redis "
@@ -561,15 +576,15 @@
     def encode(self, data):
         return data
 
     def decode(self, data):
         return data
 
 
-class PickeSessionEncoder(SessionEncoder):
+class PickleSessionEncoder(SessionEncoder):
 
     def encode(self, data):
         import pickle
         return pickle.dumps(data, 2)
 
     def decode(self, data):
         import pickle
@@ -590,8 +605,8 @@
 def generate_session_id():
     """
     Default firenado session id generator
 
     Returns:
         A random string containing digits, upper and lower characters
     """
-    return security.random_string(64)
+    return random_string(64)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/tornadoweb.py` & `Firenado-0.9.0a1/firenado/tornadoweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -59,15 +59,15 @@
     request = HTTPRequest(url, method=method)
     if form_urlencoded:
         request.headers.add("Content-Type",
                             "application/x-www-form-urlencoded")
     return request
 
 
-class TornadoErrorHandler(object):
+class TornadoErrorHandler:
 
     def __init__(self, host):
         self._host = host
 
     @property
     def host(self):
         return self._host
@@ -89,15 +89,15 @@
 
 class TornadoApplication(tornado.web.Application, data.DataConnectedMixin,
                          session.SessionEnginedMixin):
     """ Firenado basic Tornado application.
     """
 
     def __init__(self, default_host="", transforms=None, **settings):
-        logger.debug('Wiring application located at %s.' %
+        logger.debug("Wiring application located at %s.",
                      firenado.conf.APP_ROOT_PATH)
         self.components = {}
         settings.update(firenado.conf.app['settings'])
         handlers = []
         ui_modules = []
         data.configure_data_sources(firenado.conf.app['data']['sources'], self)
         self.__load_components()
@@ -148,27 +148,31 @@
         if firenado.conf.app['url_root_path'] is not None:
             from .util.url_util import rooted_path
             for idx, handler in enumerate(handlers):
                 handler_list = list(handler)
                 handler_list[0] = rooted_path(
                     firenado.conf.app['url_root_path'], handler_list[0])
                 handlers[idx] = tuple(handler_list)
-        tornado.web.Application.__init__(self, handlers=handlers,
-                                         default_host=default_host,
-                                         transforms=transforms, **settings)
+        super().__init__(handlers=handlers, default_host=default_host,
+                         transforms=transforms, **settings)
         logger.debug("Checking if session is enabled.")
         if firenado.conf.session['enabled']:
             logger.debug("Session is enabled. Starting session engine.")
             # This is forcing the session engine to be created from the get-go
             # an assert will be use to call it and check if is not none.
             assert self.session_engine is not None
         else:
             logger.debug("Session is disabled.")
 
-    def get_app_component(self):
+    def get_app_component(self) -> "TornadoComponent":
+        """ Return the component set as the application component at the
+        app config.
+
+        :return: TornadoComponent
+        """
         return self.components[firenado.conf.app['component']]
 
     def __load_components(self):
         """ Loads all enabled components registered from the components
         config section.
         """
         for key, value in firenado.conf.components.items():
@@ -180,25 +184,24 @@
                     if filename is not None:
                         self.components[key].conf = load_yaml_file(filename)
                         self.components[key].process_config()
                         self.components[key].has_conf = True
                     else:
                         logger.debug("Failed to find the file for the "
                                      "component %s at %s. Component's "
-                                     "filename returned is %s." % (
-                                        key, firenado.conf.APP_CONFIG_PATH,
-                                        self.components[key].get_config_file())
-                                     )
+                                     "filename returned is %s.", key,
+                                     firenado.conf.APP_CONFIG_PATH,
+                                     self.components[key].get_config_file())
         # Initializing enabled components after the load.
         for key, value in firenado.conf.components.items():
             if value['enabled']:
                 self.components[key].initialize()
 
 
-class TornadoComponent(object):
+class TornadoComponent:
     """ Firenado applications are organized in components. A component could be
     an application or something that can be distributed as an add-on or a
     plugin.
     """
 
     def __init__(self, name, application):
         self.name = name
@@ -221,15 +224,15 @@
 
     def get_error_handler(self) -> TornadoErrorHandler:
         """Return a `TornadoErrorHandler` here to provide a different error
         handling than the tornado's default. If the error handler is
         implemented at the component, all handlers will use it as default. If a
         handler implements the `get_error_handler` method, it will be used
         instead of the one implemented at the component."""
-        pass
+        return None
 
     def is_current_app(self):
         if not firenado.conf.is_multi_app:
             return True
         if firenado.conf.current_app_name == self.name:
             return True
         return False
@@ -324,35 +327,36 @@
 class SessionHandler:
     """ Set the stage for a handler with session. The session per-se will be
     managed by the ComponentHandler that extends SessionHandler.
     """
 
     def __init__(self):
         self.session = None
+        self.skip_auth = False
 
     def authenticated(self):
         """ Returns if the current user is authenticated. If the current user
         is set then we consider authenticated.
 
         :return: bool True is current user is set
         """
         return self.current_user is not None
 
 
 class ComponentHandler(SessionHandler):
-    """ This mixing will define a handler with components and session.
+    """ This mixin will define a handler with components and session.
     ComponentHandler is the base of what a Firenado handler should be and it
     will be used to unify TornadoHandler and TornadoWebSocketHandler logic.
     Other functionalities will be implemented in TemplateHandler that assumes
     the handler being applied to is also a ComponentHandler.
     """
 
     def __init__(self, **kwargs):
+        super().__init__()
         self.component = None
-        SessionHandler.__init__(self)
 
     def initialize(self, component):
         self.component = component
 
     def get_data_connected(self):
         return self.application
 
@@ -363,20 +367,23 @@
         :param Any kwargs:
         :return:
         """
         error_handler = self.get_error_handler()
         if error_handler is None:
             error_handler = self.component.get_error_handler()
         if error_handler is None:
-            super(TornadoHandler, self).write_error(status_code, **kwargs)
+            super().write_error(status_code, **kwargs)
         else:
             error_handler.handle_error(self, status_code, **kwargs)
 
     @session.read
     def prepare(self):
+        if hasattr(self, "authenticate"):
+            if self.authenticate and hasattr(self.authenticate, '__call__'):
+                self.authenticate()
         self.component.before_request(self)
         self.before_request()
 
     @session.write
     def on_finish(self):
         self.after_request()
         self.component.after_request(self)
@@ -398,15 +405,15 @@
         pass
 
     def get_error_handler(self) -> TornadoErrorHandler:
         """Return a `TornadoErrorHandler` here to provide a different error
         handling than the tornado's default. If the error handler is
         implemented at the handler, it will be used instead of the one
         implemented at the component."""
-        pass
+        return None
 
     def before_request(self):
         """Called at the beginning of a request before  `get`/`post`/etc.
 
         Override this method to perform common initialization regardless
         of the request method.
 
@@ -422,19 +429,24 @@
         until the ``Awaitable`` is done.
 
         .. versionadded:: 0.1.10
            Asynchronous support.
         """
         pass
 
+    def get_rooted_path(self, path):
+        from .util.url_util import rooted_path
+        root = firenado.conf.app['url_root_path']
+        return rooted_path(root, path)
+
 
 class TemplateHandler:
-    """ Deals with all aspects related to templates. The mixin will assume
-    it was applied to a ComponentHandler so we can resolve and deal with
-    templates defined in the same component or other components from the
+    """ Deals with all aspects related to templates. This mixin will assume
+    it was applied to a ComponentHandler. It will resolve and deal with
+    templates defined in the same component or other components of an
     application.
     """
 
     def __init__(self):
         self.__template_variables = dict()
 
     @property
@@ -468,15 +480,15 @@
 
         By default, we use the ``template_path`` application setting.
         Return None to load templates relative to the calling file.
         """
         if self.component is None:
             # This is the default behaviour provided by Tornado.
             # No components on the request no fancy template path.
-            return super(TornadoHandler, self).get_template_path()
+            return super().get_template_path()
         else:
             return self.component.get_template_path()
 
     def get_firenado_template_path(self):
         """Override to customize the firenado template path for each handler.
 
         By default, we use the ``firenado_template_path`` application setting.
@@ -498,58 +510,41 @@
             # autoescape=None means "no escaping", so we have to be sure
             # to only pass this kwarg if the user asked for it.
             kwargs['autoescape'] = settings['autoescape']
         return FirenadoComponentLoader(
             template_path, component=self.component, **kwargs)
 
 
-class WebUtilHandler:
-    """ Holds everything else related to web utilities.
-    """
-
-    def is_mobile(self):
-        from mobiledetect import MobileDetect
-        if 'User-Agent' in self.request.headers:
-            return MobileDetect(
-                useragent=self.request.headers['User-Agent']
-            ).is_mobile()
-        return False
-
-    def get_rooted_path(self, path):
-        from .util.url_util import rooted_path
-        root = firenado.conf.app['url_root_path']
-        return rooted_path(root, path)
-
-
-class TornadoHandler(ComponentHandler, TemplateHandler, WebUtilHandler,
+class TornadoHandler(ComponentHandler, TemplateHandler,
                      tornado.web.RequestHandler):
     """ Base request handler to be used on a Firenado application.
     It provides session and handles component paths.
     """
+
     def __init__(self, application, request, **kwargs):
         ComponentHandler.__init__(self, **kwargs)
         TemplateHandler.__init__(self)
         tornado.web.RequestHandler.__init__(self, application, request,
                                             **kwargs)
 
 
 class TornadoWebSocketHandler(ComponentHandler, TemplateHandler,
-                              WebUtilHandler,
                               tornado.websocket.WebSocketHandler):
 
     def __init__(self, application, request, **kwargs):
         ComponentHandler.__init__(self, **kwargs)
         TemplateHandler.__init__(self)
         tornado.websocket.WebSocketHandler.__init__(
             self, application, request, **kwargs)
 
 
 class FirenadoComponentLoader(Loader):
     """ A template loader that loads from a single root directory.
     """
+
     def __init__(self, root_directory, component=None, **kwargs):
         # TODO: Check if we should alter/use the root_directory value
         # here or on the resolve_path method.
         self.component = component
         super(FirenadoComponentLoader, self).__init__(root_directory, **kwargs)
 
     def resolve_path(self, name, parent_path=None):
@@ -557,20 +552,19 @@
         another component is being referenced. The component template will be
         resolved and passed to the original Tornado resolve_path method.
 
         :param name: The template name
         :param parent_path: The template parent path
         :return: Tornado resolve_path result.
         """
-        logger.debug("Resolving template %s." % name)
+        logger.debug("Resolving template %s.", name)
         name_resolved = name
         if ':' in name:
             name_x = name.split(':')
             component_name = name_x[0]
             name_resolved = os.path.join(
                 self.component.application.components[
                     component_name].get_template_path(), name_x[-1])
         if name != name_resolved:
-            logger.debug("Template %s resolved at %s." % (name, name_resolved))
+            logger.debug("Template %s resolved at %s.", name, name_resolved)
 
-        return super(FirenadoComponentLoader,
-                     self).resolve_path(name_resolved, parent_path)
+        return super().resolve_path(name_resolved, parent_path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/firenado/uimodules.py` & `Firenado-0.9.0a1/firenado/uimodules.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/util/argparse_util.py` & `Firenado-0.9.0a1/firenado/util/argparse_util.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/firenado/util/url_util.py` & `Firenado-0.9.0a1/firenado/util/url_util.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/setup.py` & `Firenado-0.9.0a1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,30 +42,28 @@
         # pr stands for parsed_requirement
         return [str(pr.requirement) for pr in requirements]
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-# We still running: python setup.py sdist upload --repository=testpypi
-# Twine isn't handling long_descriptions as per:
-# https://github.com/pypa/twine/issues/262
 setup(
     name="Firenado",
     version=firenado.get_version(),
     description="Firenado is a python web framework based on Tornado web "
                 "framework/server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license=firenado.__licence__,
     author=firenado.get_author(),
     author_email=firenado.get_author_email(),
     maintainer=firenado.get_author(),
     maintainer_email=firenado.get_author_email(),
     install_requires=resolve_requires("requirements/basic.txt"),
+    python_requires=">= 3.7",
     extras_require={
         'all': resolve_requires("requirements/all.txt"),
         'redis': resolve_requires("requirements/redis.txt"),
         'pexpect': resolve_requires("requirements/pexpect.txt"),
         'schedule': resolve_requires("requirements/schedule.txt"),
         'sqlalchemy': resolve_requires("requirements/sqlalchemy.txt"),
     },
@@ -76,18 +74,19 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Environment :: Web Environment",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP :: WSGI",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     scripts=["firenado/bin/firenado-cli.py"],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/tests/__init__.py` & `Firenado-0.9.0a1/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,26 +36,26 @@
         import logging
         for handler in logging.root.handlers[:]:
             # clearing loggers, solution from: https://bit.ly/2yTchyx
             logging.root.removeHandler(handler)
     return test_app_dirname
 
 
-def chdir_app(app_name, dir=None):
+def chdir_app(app_name, directory=None):
     """ Change to the application directory located at the resource directory
     for conf tests.
 
     The conf resources directory is firenado/tests/resources/conf.
 
     :param app_name: The application name
-    :param dir: The directory to be changed
+    :param directory: The directory to be changed
     """
     import firenado.conf
 
     test_dirname, filename = os.path.split(os.path.abspath(__file__))
-    if dir:
+    if directory:
         test_app_dirname = os.path.join(test_dirname, 'resources',
-                                        dir, app_name)
+                                        directory, app_name)
     else:
         test_app_dirname = os.path.join(test_dirname, 'resources', app_name)
     os.chdir(test_app_dirname)
     reload(firenado.conf)
```

### Comparing `Firenado-0.2.9/tests/components_test.py` & `Firenado-0.9.0a1/tests/components_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#!/usr/bin/env python
+# -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,35 +16,38 @@
 
 import unittest
 
 import firenado.conf
 from firenado.config import get_class_from_config
 from tests import chdir_app
 from firenado.tornadoweb import TornadoApplication
+import warnings
 
 chdir_app('file', 'session')
 
 
 class StaticMapsTestCase(unittest.TestCase):
-    """ Case that tests an Firenado application after being loaded from its
+    """ Case that tests a Firenado application after being loaded from its
     configuration file.
     """
 
     def setUp(self):
         """ Application configuration file will be read and components will be
         loaded.
         """
-        chdir_app('file', 'session')
-        self.application = TornadoApplication()
-        self.session_handler_config = firenado.conf.session[
-            'handlers'][firenado.conf.session['type']]
-        self.session_handler_config = firenado.conf.session[
-            'handlers'][firenado.conf.session['type']]
-        self.session_handler_class = get_class_from_config(
-            self.session_handler_config)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            chdir_app('file', 'session')
+            self.application = TornadoApplication()
+            self.session_handler_config = firenado.conf.session[
+                'handlers'][firenado.conf.session['type']]
+            self.session_handler_config = firenado.conf.session[
+                'handlers'][firenado.conf.session['type']]
+            self.session_handler_class = get_class_from_config(
+                self.session_handler_config)
 
     def test_application_session_handler(self):
         """ Checks if the session handler loaded is the same the session
         handler defined.
         """
         app_session_handler_class = \
             self.application.session_engine.session_handler.__class__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/tests/conf_test.py` & `Firenado-0.9.0a1/tests/conf_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,14 @@
     """ Case that tests an Firenado application after being loaded from its
     configuration file.
     """
 
     def test_conf_root(self):
         """ Test if Firenado root matches the upper directory relative to the
         current one. """
-        import os
-        current_path = os.path.dirname(os.path.realpath(__file__))
-        firenado_root = ("%s" % os.sep).join(current_path.split(os.sep)[:-1])
-        self.assertEqual(firenado_root, firenado.conf.ROOT)
-
-    def test_conf_root(self):
-        """ Test if Firenado root matches the upper directory relative to the
-        current one. """
         current_path = os.path.dirname(os.path.realpath(__file__))
         firenado_root = ("%s" % os.sep).join(current_path.split(os.sep)[:-1])
         firenado_root = os.path.join(firenado_root, "firenado")
         self.assertEqual(firenado_root, firenado.conf.ROOT)
 
     def test_firenado_config_file_default_value(self):
         """ Test if the default Firenado config file value will be "firenado".
@@ -191,15 +183,15 @@
     def test_root_url_slash_none(self):
         """ Test if the root path with a slash in the front will be returned
         without it was set on the app configuration.
         """
         chdir_app("root_url_slash_none", "conf")
         self.assertEqual(None,  firenado.conf.app['url_root_path'])
 
-    def test_static_path(self):
+    def test_static_url_prefix(self):
         """ If static url prefix is defined on the app configuration.
         """
         chdir_app("yml", "conf")
         self.assertEqual("yml_static_url_prefix",
                           firenado.conf.app['static_url_prefix'])
 
     def test_session_type_file(self):
@@ -226,14 +218,28 @@
     def test_session_name_custom(self):
         """ Checks if the session name will be defined as in the config file
         """
         chdir_app("redis", "session")
         self.assertEqual(firenado.conf.session['enabled'], True)
         self.assertEqual(firenado.conf.session['name'], "REDISSESSID")
 
+    def test_data_source_pool(self):
+        """ Checks if the data source pool is set correctly
+        """
+        chdir_app("data", "conf")
+        self.assertEqual(
+            firenado.conf.data['sources']['mysql']['pool']['size'],
+            10)
+        self.assertEqual(
+            firenado.conf.data['sources']['mysql']['pool']['max_overflow'],
+            10)
+        self.assertEqual(
+            firenado.conf.data['sources']['mysql']['pool']['isolation_level'],
+            "REPEATABLE READ")
+
 
 class MultiAppTestCase(unittest.TestCase):
     """ Case that tests multi app configuration.
     """
 
     def test_multi_app_true(self):
         """ Checks if the application is multi app
```

### Comparing `Firenado-0.2.9/tests/config_test.py` & `Firenado-0.9.0a1/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/tests/features/environment.py` & `Firenado-0.9.0a1/tests/features/environment.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/tests/features/steps/launcher.py` & `Firenado-0.9.0a1/tests/features/steps/launcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     await context.launcher.launch()
     await gen.sleep(1)
     context.tester.assertTrue(context.launcher.is_alive())
 
 
 @when("The application is running correctly at {port} port")
 @async_run_until_complete
-async def step_we_launch_application_using_process_launcher(context, port):
+async def step_application_running_correctly_at_port(context, port):
     http_client = AsyncHTTPClient()
     try:
         response = await http_client.fetch("http://localhost:%s" %
                                            port)
     except Exception as e:
         print("Error: %s" % e)
         context.tester.assertTrue(False)
```

### Comparing `Firenado-0.2.9/tests/runtests.py` & `Firenado-0.9.0a1/tests/runtests.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 from tests import (components_test, conf_test, config_test, data_test,
-                   security_test, service_test, session_test, tornadoweb_test)
-from tests.util import sqlalchemy_util_test, url_util_test
+                   security_test, service_test, session_test, sqlalchemy_test,
+                   tornadoweb_test)
+from tests.util import url_util_test
 
 
 def suite():
     testLoader = unittest.TestLoader()
     alltests = unittest.TestSuite()
     alltests.addTests(testLoader.loadTestsFromModule(components_test))
     alltests.addTests(testLoader.loadTestsFromModule(conf_test))
     alltests.addTests(testLoader.loadTestsFromModule(config_test))
     alltests.addTests(testLoader.loadTestsFromModule(data_test))
     alltests.addTests(testLoader.loadTestsFromModule(security_test))
     alltests.addTests(testLoader.loadTestsFromModule(service_test))
     alltests.addTests(testLoader.loadTestsFromModule(session_test))
+    alltests.addTests(testLoader.loadTestsFromModule(sqlalchemy_test))
     alltests.addTests(testLoader.loadTestsFromModule(tornadoweb_test))
-    alltests.addTests(testLoader.loadTestsFromModule(sqlalchemy_util_test))
     alltests.addTests(testLoader.loadTestsFromModule(url_util_test))
     return alltests
 
 
 if __name__ == "__main__":
     runner = unittest.TextTestRunner(verbosity=3)
     result = runner.run(suite())
```

### Comparing `Firenado-0.2.9/tests/service_test.py` & `Firenado-0.9.0a1/tests/service_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,184 +1,227 @@
-#!/usr/bin/env python
-#
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from firenado.data import DataConnectedMixin
-from firenado.service import served_by, FirenadoService
+from firenado.service import with_service, FirenadoService
 import unittest
 
 
-class MockServiceDataConnected(FirenadoService):
+class TestableServiceDataConnected(FirenadoService):
     """ Serves a data connected method directly.
     When decorating a data connected directly the service must return the
     consumer.
     """
     pass
 
 
-class MockDataConnected(DataConnectedMixin):
+class TestableSession(object):
+
+    def __init__(self, data_source):
+        self._data_source = data_source
+        self._oppened = True
+
+    @property
+    def data_source(self):
+        return self._data_source
+
+    @property
+    def is_oppened(self):
+        return self._oppened
+
+    @property
+    def name(self):
+        return self.data_source.resolve_session()
+
+    def close(self):
+        self._oppened = False
+
+
+class TestableDataSource(object):
+
+    def __init__(self, name):
+        self._name = name
+
+    @property
+    def name(self):
+        return self._name
+
+    @property
+    def session(self):
+        return TestableSession(self)
+
+    @property
+    def session_resolved_string(self):
+        return "Session resolved from data source"
+
+    def resolve_session(self):
+        return "%s: %s" % (self.session_resolved_string, self.name)
+
+
+class TestableDataConnected(DataConnectedMixin):
     """ Data connected mock object. This object holds the data sources to be
     used in the test cases.
     """
 
+    testable_service_data_connected: TestableServiceDataConnected
+
     def __init__(self):
-        self.data_sources['datasource1'] = 'DataSource1'
-        self.data_sources['datasource2'] = 'DataSource2'
+        self.data_sources['datasource1'] = TestableDataSource("DataSource1")
+        self.data_sources['datasource2'] = TestableDataSource("DataSource2")
 
-    @served_by(MockServiceDataConnected)
+    @with_service(TestableServiceDataConnected)
     def get_service_data_sources_directly(self):
-        return self.mock_service_data_connected.get_data_sources()
+        return self.testable_service_data_connected.get_data_sources()
 
 
-class MockTestService(FirenadoService):
+class TestableService(FirenadoService):
     """ Service that decorates the instance to be served directly and
     indirectly thought MockTestServiceRecursion.
     When decorating directly data connected and data sources will be returned
     in one interaction.
     When decorating indirectly MockTestServiceRecursion will be used to return
     the data connected instance and data sources.
     """
     pass
 
 
-class MockTestServiceRecursion(FirenadoService):
-    """ Service that decorates the instance to be served and will be used
-    to return the data connected and data sources when MockTestService
-    delegates to during the recursive test.
+class RecursiveService(FirenadoService):
+    """ This service will be used to return the data connected reference
+    and data source, during the recursive test, delegating to MockTestService.
     """
 
-    @served_by(MockTestService)
+    testable_service: TestableService
+
+    @with_service(TestableService)
     def get_service_data_sources_recursively(self):
-        return self.mock_test_service.get_data_sources()
+        return self.testable_service.get_data_sources()
 
-    @served_by(MockTestService)
+    @with_service(TestableService)
     def get_data_connected_recursively(self):
-        return self.mock_test_service.data_connected
+        return self.testable_service.data_connected
 
 
 class ServedByInstance(object):
-    """ Class that has methods that will be decorated with the served_by
-    decorator.
+    """ Class with methods to be decorated with the served_by decorator.
     """
 
+    testable_service: TestableService
+    recursive_service: RecursiveService
+
     def __init__(self, data_connected):
         self.data_connected = data_connected
 
-    @served_by(MockTestService)
+    @with_service(TestableService)
     def do_served_by_class(self):
-        """
-        This method will be decorated with served_by with the class reference
+        """ Method to be decorated with served_by with a class reference
         """
         pass
 
-    @served_by('tests.service_test.MockTestService')
+    @with_service("tests.service_test.TestableService")
     def do_served_by_string(self):
-        """
-        This method will be decorated with served_by with the class as string
+        """ Method to be decorated with served_by with a string as class
+        reference
         """
         pass
 
-    @served_by(MockTestService)
+    @with_service(TestableService)
     def get_service_data_connected(self):
-        return self.mock_test_service.data_connected
+        return self.testable_service.data_connected
 
-    @served_by(MockTestServiceRecursion)
+    @with_service(RecursiveService)
     def get_service_data_connected_recursively(self):
-        return (self.mock_test_service_recursion.
-                get_data_connected_recursively())
+        return (self.recursive_service.get_data_connected_recursively())
 
-    @served_by(MockTestService)
+    @with_service(TestableService)
     def get_service_data_sources(self):
         """ This method returns the data sources from the data connected
         instance of this class. The method is returned by the service defined
         on the served_by decorator. Here there is no recursion once
         MockTestService is directly serving the ServiceByInstance.
         """
-        return self.mock_test_service.get_data_sources()
+        return self.testable_service.get_data_sources()
 
-    @served_by(MockTestServiceRecursion)
+    @with_service(RecursiveService)
     def get_service_data_sources_recursively(self):
-        """ Same as get_service_data_sources but the a service will be serving
-        the service defined here and then access the data sources
+        """ Same as get_service_data_sources but service will be serving
+        another service defined here and then access the data sources
         """
-        return (self.mock_test_service_recursion.
-                get_service_data_sources_recursively())
+        return (self.recursive_service.get_service_data_sources_recursively())
 
     def get_data_connected(self):
         return self.data_connected
 
 
 class ServiceTestCase(unittest.TestCase):
 
     def setUp(self):
         """ Setting up an object that has firenado.core.service.served_by
         decorators on some methods.
         """
-        self.data_connected_instance = MockDataConnected()
+        self.data_connected_instance = TestableDataConnected()
         self.served_by_instance = ServedByInstance(
             self.data_connected_instance)
 
     def test_served_by_class_reference(self):
-        self.assertFalse(hasattr(self.served_by_instance, 'mock_test_service'))
+        self.assertFalse(hasattr(self.served_by_instance, 'testable_service'))
         self.served_by_instance.do_served_by_class()
-        self.assertTrue(hasattr(self.served_by_instance, 'mock_test_service'))
+        self.assertTrue(hasattr(self.served_by_instance, 'testable_service'))
         self.assertTrue(isinstance(
-            self.served_by_instance.mock_test_service, MockTestService))
+            self.served_by_instance.testable_service, TestableService))
 
     def test_served_by_class_name_string(self):
-        self.assertFalse(hasattr(self.served_by_instance, 'mock_test_service'))
+        self.assertFalse(hasattr(self.served_by_instance, 'testable_service'))
         self.served_by_instance.do_served_by_string()
-        self.assertTrue(hasattr(self.served_by_instance, 'mock_test_service'))
+        self.assertTrue(hasattr(self.served_by_instance, 'testable_service'))
         self.assertEqual(
-            self.served_by_instance.mock_test_service.__class__.__name__,
-            MockTestService.__name__)
+            self.served_by_instance.testable_service.__class__.__name__,
+            TestableService.__name__)
 
     def test_data_connected_from_service(self):
         data_connected = self.served_by_instance.get_data_connected()
         self.assertEqual(data_connected, self.data_connected_instance)
 
     def test_data_connected_from_service_recursively(self):
         data_connected = (self.served_by_instance.
                           get_service_data_connected_recursively())
         self.assertEqual(data_connected, self.data_connected_instance)
 
     def test_data_connected_from_service_none(self):
-        mock_service = MockTestService(None)
-        data_connected = mock_service.data_connected
+        service = TestableService(None)
+        data_connected = service.data_connected
         self.assertIsNone(data_connected)
 
     def test_get_data_source_from_service(self):
         data_sources = self.served_by_instance.get_service_data_sources()
         self.assertTrue(len(data_sources) == 2)
-        self.assertEqual(data_sources['datasource1'], "DataSource1")
-        self.assertEqual(data_sources['datasource2'], "DataSource2")
+        self.assertEqual(data_sources['datasource1'].name, "DataSource1")
+        self.assertEqual(data_sources['datasource2'].name, "DataSource2")
 
     def test_get_data_source_from_data_connected(self):
         data_sources = (self.data_connected_instance.
                         get_service_data_sources_directly())
         self.assertTrue(len(data_sources) == 2)
-        self.assertEqual(data_sources['datasource1'], "DataSource1")
-        self.assertEqual(data_sources['datasource2'], "DataSource2")
+        self.assertEqual(data_sources['datasource1'].name, "DataSource1")
+        self.assertEqual(data_sources['datasource2'].name, "DataSource2")
 
     def test_get_data_source_from_service_recursively(self):
         data_sources = (self.served_by_instance.
                         get_service_data_sources_recursively())
         self.assertTrue(len(data_sources) == 2)
-        self.assertEqual(data_sources['datasource1'], "DataSource1")
-        self.assertEqual(data_sources['datasource2'], "DataSource2")
+        self.assertEqual(data_sources['datasource1'].name, "DataSource1")
+        self.assertEqual(data_sources['datasource2'].name, "DataSource2")
 
     def test_get_data_source_from_service_none(self):
-        mock_service = MockTestService(None)
-        data_sources = mock_service.get_data_sources()
+        service = TestableService(None)
+        data_sources = service.get_data_sources()
         self.assertIsNone(data_sources)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/tests/session_test.py` & `Firenado-0.9.0a1/tests/session_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#!/usr/bin/env python
+# -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2022 Flávio Gonçalves Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,33 +15,36 @@
 # limitations under the License.
 
 import firenado.conf
 from firenado.config import get_class_from_config
 from firenado.tornadoweb import TornadoApplication
 from tests import chdir_app
 import unittest
+import warnings
 
 
 class FileSessionTestCase(unittest.TestCase):
-    """ Case that tests an Firenado application after being loaded from its
+    """ Case that tests a Firenado application after being loaded from its
     configuration file.
     """
 
     def setUp(self):
         """ Application configuration file will be read and components will be
         loaded.
         """
         chdir_app("file", "session")
-        self.application = TornadoApplication()
-        self.session_handler_config = firenado.conf.session[
-            'handlers'][firenado.conf.session['type']]
-        self.session_handler_config = firenado.conf.session[
-            'handlers'][firenado.conf.session['type']]
-        self.session_handler_class = get_class_from_config(
-            self.session_handler_config)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            self.application = TornadoApplication()
+            self.session_handler_config = firenado.conf.session[
+                'handlers'][firenado.conf.session['type']]
+            self.session_handler_config = firenado.conf.session[
+                'handlers'][firenado.conf.session['type']]
+            self.session_handler_class = get_class_from_config(
+                self.session_handler_config)
 
     def test_defaults_session_parameters(self):
         """ Checks default session parameters on the configuration
         session section
         """
         self.assertEqual(firenado.conf.session['life_time'], 1800)
         self.assertEqual(firenado.conf.session['callback_time'], 120)
@@ -55,26 +58,29 @@
             self.session_handler_class
         )
 
     def test_session_type_file(self):
         """ Checks if test component was loaded correctly by the application
         __init__ method.
         """
-        application = TornadoApplication()
-        session_handler_config = firenado.conf.session[
-            'handlers'][firenado.conf.session['type']]
-        session_handler_class = get_class_from_config(session_handler_config)
-        self.assertEqual(application.session_engine.session_handler.__class__,
-                         session_handler_class)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            application = TornadoApplication()
+            session_handler_config = firenado.conf.session[
+                'handlers'][firenado.conf.session['type']]
+            session_handler_class = get_class_from_config(
+                session_handler_config)
+            self.assertEqual(
+                application.session_engine.session_handler.__class__,
+                session_handler_class)
 
 
 class RedisSessionTestCase(unittest.TestCase):
-    """ Case that tests an Firenado application after being loaded from its
-    configuration file.
-    """
+    """ Tests a Firenado application after being loaded from its configuration
+    file. """
 
     def setUp(self):
         """ Application configuration file will be read and components will be
         loaded.
         """
         chdir_app("redis", "session")
 
@@ -95,22 +101,22 @@
 
 class EncodersSessionTestCase(unittest.TestCase):
 
     def test_pickle_session_encoder(self):
         """ Checks if the pickle session encoder will keep a dict structure
         and values intact after encoding and decoding it.
         """
-        from firenado.session import PickeSessionEncoder
+        from firenado.session import PickleSessionEncoder
         my_dict = {
             'value1': "My value1",
             'value2': {
                 'value3': "My value3",
             }
         }
-        encoder = PickeSessionEncoder()
+        encoder = PickleSessionEncoder()
         encoded_data = encoder.encode(my_dict)
         decoded_data = encoder.decode(encoded_data)
         self.assertEqual(decoded_data['value1'], my_dict['value1'])
         self.assertEqual(decoded_data['value2']['value3'],
                          my_dict['value2']['value3'])
 
     def test_json_session_encoder(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Firenado-0.2.9/tests/tornadoweb_test.py` & `Firenado-0.9.0a1/tests/tornadoweb_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.2.9/tests/util/url_util_test.py` & `Firenado-0.9.0a1/tests/util/url_util_test.py`

 * *Files identical despite different names*

