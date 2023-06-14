# Comparing `tmp/latch-2.9.5.tar.gz` & `tmp/latch-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch-2.9.5.tar", last modified: Sun Jan  8 00:47:57 2023, max compression
+gzip compressed data, was "latch-2.9.6.tar", last modified: Sun Jan  8 00:55:17 2023, max compression
```

## Comparing `latch-2.9.5.tar` & `latch-2.9.6.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:57.006574 latch-2.9.5/
--rw-r--r--   0 ayush      (504) staff       (20)     1048 2022-09-08 19:58:53.000000 latch-2.9.5/LICENSE
--rw-r--r--   0 ayush      (504) staff       (20)       70 2022-09-24 23:53:37.000000 latch-2.9.5/MANIFEST.in
--rw-r--r--   0 ayush      (504) staff       (20)      300 2023-01-08 00:47:57.005643 latch-2.9.5/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)     4585 2022-09-03 21:36:00.000000 latch-2.9.5/README.md
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.955342 latch-2.9.5/latch/
--rw-r--r--   0 ayush      (504) staff       (20)      684 2022-08-23 01:27:33.000000 latch-2.9.5/latch/__init__.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.958858 latch-2.9.5/latch/functions/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2022-07-03 00:46:15.000000 latch-2.9.5/latch/functions/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     2411 2022-09-14 20:35:53.000000 latch-2.9.5/latch/functions/messages.py
--rw-r--r--   0 ayush      (504) staff       (20)     6655 2022-12-08 16:17:55.000000 latch-2.9.5/latch/functions/operators.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.962861 latch-2.9.5/latch/resources/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2022-07-03 00:46:15.000000 latch-2.9.5/latch/resources/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     1588 2022-07-03 00:46:15.000000 latch-2.9.5/latch/resources/conditional.py
--rw-r--r--   0 ayush      (504) staff       (20)     1688 2022-07-21 20:42:07.000000 latch-2.9.5/latch/resources/launch_plan.py
--rw-r--r--   0 ayush      (504) staff       (20)     1184 2022-07-03 00:46:15.000000 latch-2.9.5/latch/resources/map_tasks.py
--rw-r--r--   0 ayush      (504) staff       (20)      320 2022-08-27 20:01:30.000000 latch-2.9.5/latch/resources/reference_workflow.py
--rw-r--r--   0 ayush      (504) staff       (20)     7770 2022-10-08 19:33:36.000000 latch-2.9.5/latch/resources/tasks.py
--rw-r--r--   0 ayush      (504) staff       (20)     2697 2022-12-29 21:24:58.000000 latch-2.9.5/latch/resources/workflow.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.965556 latch-2.9.5/latch/types/
--rw-r--r--   0 ayush      (504) staff       (20)      361 2022-10-19 17:16:20.000000 latch-2.9.5/latch/types/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     5432 2022-11-12 18:54:27.000000 latch-2.9.5/latch/types/directory.py
--rw-r--r--   0 ayush      (504) staff       (20)     5661 2022-12-05 20:46:41.000000 latch-2.9.5/latch/types/file.py
--rw-r--r--   0 ayush      (504) staff       (20)     1742 2022-07-30 22:37:39.000000 latch-2.9.5/latch/types/glob.py
--rw-r--r--   0 ayush      (504) staff       (20)     9856 2022-12-17 21:55:17.000000 latch-2.9.5/latch/types/metadata.py
--rw-r--r--   0 ayush      (504) staff       (20)      519 2022-08-17 02:25:21.000000 latch-2.9.5/latch/types/utils.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.967060 latch-2.9.5/latch/verified/
--rw-r--r--   0 ayush      (504) staff       (20)      151 2022-09-02 16:38:32.000000 latch-2.9.5/latch/verified/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     2223 2022-09-02 16:38:32.000000 latch-2.9.5/latch/verified/deseq2.py
--rw-r--r--   0 ayush      (504) staff       (20)      499 2022-09-02 16:38:32.000000 latch-2.9.5/latch/verified/pathway.py
--rw-r--r--   0 ayush      (504) staff       (20)     1857 2022-09-02 16:38:32.000000 latch-2.9.5/latch/verified/rnaseq.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.957595 latch-2.9.5/latch.egg-info/
--rw-r--r--   0 ayush      (504) staff       (20)      300 2023-01-08 00:47:56.000000 latch-2.9.5/latch.egg-info/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)     2798 2023-01-08 00:47:56.000000 latch-2.9.5/latch.egg-info/SOURCES.txt
--rw-r--r--   0 ayush      (504) staff       (20)        1 2023-01-08 00:47:56.000000 latch-2.9.5/latch.egg-info/dependency_links.txt
--rw-r--r--   0 ayush      (504) staff       (20)       46 2023-01-08 00:47:56.000000 latch-2.9.5/latch.egg-info/entry_points.txt
--rw-r--r--   0 ayush      (504) staff       (20)      322 2023-01-08 00:47:56.000000 latch-2.9.5/latch.egg-info/requires.txt
--rw-r--r--   0 ayush      (504) staff       (20)       22 2023-01-08 00:47:56.000000 latch-2.9.5/latch.egg-info/top_level.txt
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.970583 latch-2.9.5/latch_cli/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-28 22:18:08.000000 latch-2.9.5/latch_cli/__init__.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.973521 latch-2.9.5/latch_cli/auth/
--rw-r--r--   0 ayush      (504) staff       (20)      120 2022-06-28 22:18:08.000000 latch-2.9.5/latch_cli/auth/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)      778 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/auth/csrf.py
--rw-r--r--   0 ayush      (504) staff       (20)     6972 2022-09-03 21:36:00.000000 latch-2.9.5/latch_cli/auth/oauth2.py
--rw-r--r--   0 ayush      (504) staff       (20)     4221 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/auth/pkce.py
--rw-r--r--   0 ayush      (504) staff       (20)      708 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/auth/utils.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.974586 latch-2.9.5/latch_cli/centromere/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2022-11-12 18:54:27.000000 latch-2.9.5/latch_cli/centromere/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)    10258 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/centromere/ctx.py
--rw-r--r--   0 ayush      (504) staff       (20)     6916 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/centromere/utils.py
--rw-r--r--   0 ayush      (504) staff       (20)     2878 2022-07-16 21:32:35.000000 latch-2.9.5/latch_cli/click_utils.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.975649 latch-2.9.5/latch_cli/config/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-28 22:18:08.000000 latch-2.9.5/latch_cli/config/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     1969 2022-12-29 21:24:54.000000 latch-2.9.5/latch_cli/config/latch.py
--rw-r--r--   0 ayush      (504) staff       (20)     1515 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/config/user.py
--rw-r--r--   0 ayush      (504) staff       (20)      660 2022-12-06 01:45:17.000000 latch-2.9.5/latch_cli/constants.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.977754 latch-2.9.5/latch_cli/exceptions/
--rw-r--r--   0 ayush      (504) staff       (20)        1 2022-12-06 01:45:17.000000 latch-2.9.5/latch_cli/exceptions/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)       90 2022-12-06 01:45:17.000000 latch-2.9.5/latch_cli/exceptions/cache.py
--rw-r--r--   0 ayush      (504) staff       (20)      312 2022-12-06 01:45:17.000000 latch-2.9.5/latch_cli/exceptions/errors.py
--rw-r--r--   0 ayush      (504) staff       (20)     3887 2022-12-06 01:45:24.000000 latch-2.9.5/latch_cli/exceptions/handler.py
--rw-r--r--   0 ayush      (504) staff       (20)     5168 2022-12-29 21:24:54.000000 latch-2.9.5/latch_cli/exceptions/traceback.py
--rw-r--r--   0 ayush      (504) staff       (20)    15581 2023-01-05 22:31:16.000000 latch-2.9.5/latch_cli/main.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.986490 latch-2.9.5/latch_cli/services/
--rw-r--r--   0 ayush      (504) staff       (20)      256 2022-06-28 22:18:08.000000 latch-2.9.5/latch_cli/services/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)    11320 2023-01-03 21:18:16.000000 latch-2.9.5/latch_cli/services/cp.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.989955 latch-2.9.5/latch_cli/services/deprecated/
--rw-r--r--   0 ayush      (504) staff       (20)       69 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/deprecated/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     2061 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/deprecated/mkdir.py
--rw-r--r--   0 ayush      (504) staff       (20)     1607 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/deprecated/rm.py
--rw-r--r--   0 ayush      (504) staff       (20)     1848 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/deprecated/touch.py
--rw-r--r--   0 ayush      (504) staff       (20)     8266 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/execute.py
--rw-r--r--   0 ayush      (504) staff       (20)     1718 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/get.py
--rw-r--r--   0 ayush      (504) staff       (20)    19049 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/get_executions.py
--rw-r--r--   0 ayush      (504) staff       (20)    12305 2022-12-29 21:24:58.000000 latch-2.9.5/latch_cli/services/get_params.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.991119 latch-2.9.5/latch_cli/services/init/
--rw-r--r--   0 ayush      (504) staff       (20)       46 2022-09-03 21:36:00.000000 latch-2.9.5/latch_cli/services/init/__init__.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.992557 latch-2.9.5/latch_cli/services/init/assemble_and_sort/
--rw-r--r--   0 ayush      (504) staff       (20)     1019 2022-11-12 18:54:27.000000 latch-2.9.5/latch_cli/services/init/assemble_and_sort/Dockerfile
--rw-r--r--   0 ayush      (504) staff       (20)     2862 2022-09-03 21:36:00.000000 latch-2.9.5/latch_cli/services/init/assemble_and_sort/__init__.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.994744 latch-2.9.5/latch_cli/services/init/example_conda/
--rw-r--r--   0 ayush      (504) staff       (20)     1180 2022-11-12 18:54:27.000000 latch-2.9.5/latch_cli/services/init/example_conda/Dockerfile
--rw-r--r--   0 ayush      (504) staff       (20)     1463 2022-09-03 21:36:00.000000 latch-2.9.5/latch_cli/services/init/example_conda/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)        6 2022-09-03 21:36:00.000000 latch-2.9.5/latch_cli/services/init/example_conda/requirements.txt
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.995636 latch-2.9.5/latch_cli/services/init/example_r/
--rw-r--r--   0 ayush      (504) staff       (20)      859 2022-11-12 18:54:27.000000 latch-2.9.5/latch_cli/services/init/example_r/Dockerfile
--rw-r--r--   0 ayush      (504) staff       (20)     1742 2022-09-03 22:07:00.000000 latch-2.9.5/latch_cli/services/init/example_r/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     5433 2022-12-06 01:45:17.000000 latch-2.9.5/latch_cli/services/init/init.py
--rw-r--r--   0 ayush      (504) staff       (20)     7613 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/launch.py
--rw-r--r--   0 ayush      (504) staff       (20)    14288 2022-12-29 21:24:54.000000 latch-2.9.5/latch_cli/services/local_dev.py
--rw-r--r--   0 ayush      (504) staff       (20)     2726 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/login.py
--rw-r--r--   0 ayush      (504) staff       (20)     1633 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/ls.py
--rw-r--r--   0 ayush      (504) staff       (20)     1776 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/open_file.py
--rw-r--r--   0 ayush      (504) staff       (20)     6077 2023-01-05 22:31:16.000000 latch-2.9.5/latch_cli/services/preview.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:56.996822 latch-2.9.5/latch_cli/services/register/
--rw-r--r--   0 ayush      (504) staff       (20)      117 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/register/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)      226 2022-11-12 18:54:27.000000 latch-2.9.5/latch_cli/services/register/constants.py
--rw-r--r--   0 ayush      (504) staff       (20)    11538 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/register/register.py
--rw-r--r--   0 ayush      (504) staff       (20)     3611 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/register/utils.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:57.000550 latch-2.9.5/latch_cli/services/test_data/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2022-07-30 22:37:39.000000 latch-2.9.5/latch_cli/services/test_data/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)      741 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/test_data/ls.py
--rw-r--r--   0 ayush      (504) staff       (20)      997 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/test_data/remove.py
--rw-r--r--   0 ayush      (504) staff       (20)     2506 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/test_data/upload.py
--rw-r--r--   0 ayush      (504) staff       (20)     1237 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/test_data/utils.py
--rw-r--r--   0 ayush      (504) staff       (20)     4941 2022-12-05 20:46:41.000000 latch-2.9.5/latch_cli/services/workspace.py
--rw-r--r--   0 ayush      (504) staff       (20)     2922 2022-10-05 18:39:39.000000 latch-2.9.5/latch_cli/tinyrequests.py
--rw-r--r--   0 ayush      (504) staff       (20)     4307 2022-07-30 22:37:39.000000 latch-2.9.5/latch_cli/tui.py
--rw-r--r--   0 ayush      (504) staff       (20)     8464 2022-12-08 18:05:24.000000 latch-2.9.5/latch_cli/utils.py
--rw-r--r--   0 ayush      (504) staff       (20)       38 2023-01-08 00:47:57.006695 latch-2.9.5/setup.cfg
--rw-r--r--   0 ayush      (504) staff       (20)     1422 2023-01-08 00:47:33.000000 latch-2.9.5/setup.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-01-08 00:47:57.004892 latch-2.9.5/tests/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-28 22:18:08.000000 latch-2.9.5/tests/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)      555 2022-06-28 22:18:08.000000 latch-2.9.5/tests/fixtures.py
--rw-r--r--   0 ayush      (504) staff       (20)     6171 2022-12-16 07:22:06.000000 latch-2.9.5/tests/test_cli.py
--rw-r--r--   0 ayush      (504) staff       (20)     2993 2023-01-03 23:50:55.000000 latch-2.9.5/tests/test_launch.py
--rw-r--r--   0 ayush      (504) staff       (20)      140 2022-06-28 22:18:08.000000 latch-2.9.5/tests/test_login.py
--rw-r--r--   0 ayush      (504) staff       (20)      478 2022-06-28 22:18:08.000000 latch-2.9.5/tests/test_types.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.948491 latch-2.9.6/
+-rw-r--r--   0 kenny      (501) staff       (20)     1048 2022-10-18 23:53:25.000000 latch-2.9.6/LICENSE
+-rw-r--r--   0 kenny      (501) staff       (20)       70 2022-10-18 23:53:25.000000 latch-2.9.6/MANIFEST.in
+-rw-r--r--   0 kenny      (501) staff       (20)      300 2023-01-08 00:55:17.948053 latch-2.9.6/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)     4585 2022-10-18 23:53:25.000000 latch-2.9.6/README.md
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.912926 latch-2.9.6/latch/
+-rw-r--r--   0 kenny      (501) staff       (20)      684 2022-10-18 23:53:25.000000 latch-2.9.6/latch/__init__.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.916253 latch-2.9.6/latch/functions/
+-rw-r--r--   0 kenny      (501) staff       (20)        0 2022-10-18 23:53:25.000000 latch-2.9.6/latch/functions/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2411 2022-10-18 23:53:25.000000 latch-2.9.6/latch/functions/messages.py
+-rw-r--r--   0 kenny      (501) staff       (20)     6655 2022-12-03 23:56:43.000000 latch-2.9.6/latch/functions/operators.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.919132 latch-2.9.6/latch/resources/
+-rw-r--r--   0 kenny      (501) staff       (20)        0 2022-03-02 18:23:56.000000 latch-2.9.6/latch/resources/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1588 2022-10-18 23:53:25.000000 latch-2.9.6/latch/resources/conditional.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1688 2022-10-18 23:53:25.000000 latch-2.9.6/latch/resources/launch_plan.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1184 2022-10-18 23:53:25.000000 latch-2.9.6/latch/resources/map_tasks.py
+-rw-r--r--   0 kenny      (501) staff       (20)      320 2022-10-18 23:53:25.000000 latch-2.9.6/latch/resources/reference_workflow.py
+-rw-r--r--   0 kenny      (501) staff       (20)     7770 2023-01-06 20:17:02.000000 latch-2.9.6/latch/resources/tasks.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2697 2022-12-28 21:10:07.000000 latch-2.9.6/latch/resources/workflow.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.921584 latch-2.9.6/latch/types/
+-rw-r--r--   0 kenny      (501) staff       (20)      361 2022-10-21 01:26:11.000000 latch-2.9.6/latch/types/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)     5432 2022-11-16 16:46:12.000000 latch-2.9.6/latch/types/directory.py
+-rw-r--r--   0 kenny      (501) staff       (20)     5661 2022-12-03 23:56:43.000000 latch-2.9.6/latch/types/file.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1742 2022-10-18 23:53:25.000000 latch-2.9.6/latch/types/glob.py
+-rw-r--r--   0 kenny      (501) staff       (20)     9856 2022-12-28 21:10:07.000000 latch-2.9.6/latch/types/metadata.py
+-rw-r--r--   0 kenny      (501) staff       (20)      519 2022-10-18 23:53:25.000000 latch-2.9.6/latch/types/utils.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.923311 latch-2.9.6/latch/verified/
+-rw-r--r--   0 kenny      (501) staff       (20)      151 2022-10-18 23:53:25.000000 latch-2.9.6/latch/verified/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2223 2022-10-18 23:53:25.000000 latch-2.9.6/latch/verified/deseq2.py
+-rw-r--r--   0 kenny      (501) staff       (20)      499 2022-10-18 23:53:25.000000 latch-2.9.6/latch/verified/pathway.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1857 2022-10-18 23:53:25.000000 latch-2.9.6/latch/verified/rnaseq.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.915011 latch-2.9.6/latch.egg-info/
+-rw-r--r--   0 kenny      (501) staff       (20)      300 2023-01-08 00:55:17.000000 latch-2.9.6/latch.egg-info/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)     2798 2023-01-08 00:55:17.000000 latch-2.9.6/latch.egg-info/SOURCES.txt
+-rw-r--r--   0 kenny      (501) staff       (20)        1 2023-01-08 00:55:17.000000 latch-2.9.6/latch.egg-info/dependency_links.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       46 2023-01-08 00:55:17.000000 latch-2.9.6/latch.egg-info/entry_points.txt
+-rw-r--r--   0 kenny      (501) staff       (20)      322 2023-01-08 00:55:17.000000 latch-2.9.6/latch.egg-info/requires.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       22 2023-01-08 00:55:17.000000 latch-2.9.6/latch.egg-info/top_level.txt
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.926016 latch-2.9.6/latch_cli/
+-rw-r--r--   0 kenny      (501) staff       (20)        0 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/__init__.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.927936 latch-2.9.6/latch_cli/auth/
+-rw-r--r--   0 kenny      (501) staff       (20)      120 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/auth/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)      778 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/auth/csrf.py
+-rw-r--r--   0 kenny      (501) staff       (20)     6972 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/auth/oauth2.py
+-rw-r--r--   0 kenny      (501) staff       (20)     4221 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/auth/pkce.py
+-rw-r--r--   0 kenny      (501) staff       (20)      708 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/auth/utils.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.929022 latch-2.9.6/latch_cli/centromere/
+-rw-r--r--   0 kenny      (501) staff       (20)        0 2022-11-16 16:46:12.000000 latch-2.9.6/latch_cli/centromere/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)    10258 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/centromere/ctx.py
+-rw-r--r--   0 kenny      (501) staff       (20)     6916 2023-01-06 20:17:02.000000 latch-2.9.6/latch_cli/centromere/utils.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2878 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/click_utils.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.930147 latch-2.9.6/latch_cli/config/
+-rw-r--r--   0 kenny      (501) staff       (20)        0 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/config/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1969 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/config/latch.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1515 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/config/user.py
+-rw-r--r--   0 kenny      (501) staff       (20)      660 2022-12-06 01:34:32.000000 latch-2.9.6/latch_cli/constants.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.932159 latch-2.9.6/latch_cli/exceptions/
+-rw-r--r--   0 kenny      (501) staff       (20)        1 2022-12-06 01:34:32.000000 latch-2.9.6/latch_cli/exceptions/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)       90 2022-12-06 01:34:32.000000 latch-2.9.6/latch_cli/exceptions/cache.py
+-rw-r--r--   0 kenny      (501) staff       (20)      312 2022-12-06 01:34:32.000000 latch-2.9.6/latch_cli/exceptions/errors.py
+-rw-r--r--   0 kenny      (501) staff       (20)     3887 2022-12-06 01:57:22.000000 latch-2.9.6/latch_cli/exceptions/handler.py
+-rw-r--r--   0 kenny      (501) staff       (20)     5168 2022-12-16 23:49:28.000000 latch-2.9.6/latch_cli/exceptions/traceback.py
+-rw-r--r--   0 kenny      (501) staff       (20)    15581 2023-01-04 18:27:31.000000 latch-2.9.6/latch_cli/main.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.937976 latch-2.9.6/latch_cli/services/
+-rw-r--r--   0 kenny      (501) staff       (20)      256 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/services/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)    11320 2022-12-17 01:33:53.000000 latch-2.9.6/latch_cli/services/cp.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.939618 latch-2.9.6/latch_cli/services/deprecated/
+-rw-r--r--   0 kenny      (501) staff       (20)       69 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/deprecated/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2061 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/deprecated/mkdir.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1607 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/deprecated/rm.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1848 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/deprecated/touch.py
+-rw-r--r--   0 kenny      (501) staff       (20)     8266 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/execute.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1718 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/get.py
+-rw-r--r--   0 kenny      (501) staff       (20)    19049 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/get_executions.py
+-rw-r--r--   0 kenny      (501) staff       (20)    12305 2023-01-08 00:29:34.000000 latch-2.9.6/latch_cli/services/get_params.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.940313 latch-2.9.6/latch_cli/services/init/
+-rw-r--r--   0 kenny      (501) staff       (20)       46 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/services/init/__init__.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.941144 latch-2.9.6/latch_cli/services/init/assemble_and_sort/
+-rw-r--r--   0 kenny      (501) staff       (20)     1019 2022-11-16 16:46:12.000000 latch-2.9.6/latch_cli/services/init/assemble_and_sort/Dockerfile
+-rw-r--r--   0 kenny      (501) staff       (20)     2862 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/services/init/assemble_and_sort/__init__.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.942428 latch-2.9.6/latch_cli/services/init/example_conda/
+-rw-r--r--   0 kenny      (501) staff       (20)     1180 2022-11-16 16:46:12.000000 latch-2.9.6/latch_cli/services/init/example_conda/Dockerfile
+-rw-r--r--   0 kenny      (501) staff       (20)     1463 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/services/init/example_conda/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)        6 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/services/init/example_conda/requirements.txt
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.943063 latch-2.9.6/latch_cli/services/init/example_r/
+-rw-r--r--   0 kenny      (501) staff       (20)      859 2022-11-16 16:46:12.000000 latch-2.9.6/latch_cli/services/init/example_r/Dockerfile
+-rw-r--r--   0 kenny      (501) staff       (20)     1742 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/services/init/example_r/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)     5433 2022-12-06 01:34:32.000000 latch-2.9.6/latch_cli/services/init/init.py
+-rw-r--r--   0 kenny      (501) staff       (20)     7613 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/launch.py
+-rw-r--r--   0 kenny      (501) staff       (20)    14288 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/local_dev.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2726 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/login.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1633 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/ls.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1776 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/open_file.py
+-rw-r--r--   0 kenny      (501) staff       (20)     6077 2023-01-04 18:27:31.000000 latch-2.9.6/latch_cli/services/preview.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.944490 latch-2.9.6/latch_cli/services/register/
+-rw-r--r--   0 kenny      (501) staff       (20)      117 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/register/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)      226 2022-11-16 16:46:12.000000 latch-2.9.6/latch_cli/services/register/constants.py
+-rw-r--r--   0 kenny      (501) staff       (20)    11538 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/register/register.py
+-rw-r--r--   0 kenny      (501) staff       (20)     3611 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/register/utils.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.945892 latch-2.9.6/latch_cli/services/test_data/
+-rw-r--r--   0 kenny      (501) staff       (20)        0 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/services/test_data/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)      741 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/test_data/ls.py
+-rw-r--r--   0 kenny      (501) staff       (20)      997 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/test_data/remove.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2506 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/test_data/upload.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1237 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/test_data/utils.py
+-rw-r--r--   0 kenny      (501) staff       (20)     4941 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/services/workspace.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2922 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/tinyrequests.py
+-rw-r--r--   0 kenny      (501) staff       (20)     4307 2022-10-18 23:53:25.000000 latch-2.9.6/latch_cli/tui.py
+-rw-r--r--   0 kenny      (501) staff       (20)     8464 2022-12-03 23:56:43.000000 latch-2.9.6/latch_cli/utils.py
+-rw-r--r--   0 kenny      (501) staff       (20)       38 2023-01-08 00:55:17.948564 latch-2.9.6/setup.cfg
+-rw-r--r--   0 kenny      (501) staff       (20)     1422 2023-01-08 00:55:16.000000 latch-2.9.6/setup.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-01-08 00:55:17.947572 latch-2.9.6/tests/
+-rw-r--r--   0 kenny      (501) staff       (20)        0 2022-09-07 17:48:29.000000 latch-2.9.6/tests/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)      555 2022-09-07 17:48:29.000000 latch-2.9.6/tests/fixtures.py
+-rw-r--r--   0 kenny      (501) staff       (20)     6171 2022-12-17 01:33:53.000000 latch-2.9.6/tests/test_cli.py
+-rw-r--r--   0 kenny      (501) staff       (20)     2993 2023-01-04 18:27:31.000000 latch-2.9.6/tests/test_launch.py
+-rw-r--r--   0 kenny      (501) staff       (20)      140 2022-09-07 17:48:29.000000 latch-2.9.6/tests/test_login.py
+-rw-r--r--   0 kenny      (501) staff       (20)      478 2022-10-18 23:53:25.000000 latch-2.9.6/tests/test_types.py
```

### Comparing `latch-2.9.5/LICENSE` & `latch-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/README.md` & `latch-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/__init__.py` & `latch-2.9.6/latch/__init__.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/functions/messages.py` & `latch-2.9.6/latch/functions/messages.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/functions/operators.py` & `latch-2.9.6/latch/functions/operators.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/resources/conditional.py` & `latch-2.9.6/latch/resources/conditional.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/resources/launch_plan.py` & `latch-2.9.6/latch/resources/launch_plan.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/resources/map_tasks.py` & `latch-2.9.6/latch/resources/map_tasks.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/resources/tasks.py` & `latch-2.9.6/latch/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/resources/workflow.py` & `latch-2.9.6/latch/resources/workflow.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/types/directory.py` & `latch-2.9.6/latch/types/directory.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/types/file.py` & `latch-2.9.6/latch/types/file.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/types/glob.py` & `latch-2.9.6/latch/types/glob.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/types/metadata.py` & `latch-2.9.6/latch/types/metadata.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/types/utils.py` & `latch-2.9.6/latch/types/utils.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/verified/deseq2.py` & `latch-2.9.6/latch/verified/deseq2.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch/verified/rnaseq.py` & `latch-2.9.6/latch/verified/rnaseq.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch.egg-info/SOURCES.txt` & `latch-2.9.6/latch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/auth/csrf.py` & `latch-2.9.6/latch_cli/auth/csrf.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/auth/oauth2.py` & `latch-2.9.6/latch_cli/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/auth/pkce.py` & `latch-2.9.6/latch_cli/auth/pkce.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/auth/utils.py` & `latch-2.9.6/latch_cli/auth/utils.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/centromere/ctx.py` & `latch-2.9.6/latch_cli/centromere/ctx.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/centromere/utils.py` & `latch-2.9.6/latch_cli/centromere/utils.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/click_utils.py` & `latch-2.9.6/latch_cli/click_utils.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/config/latch.py` & `latch-2.9.6/latch_cli/config/latch.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/config/user.py` & `latch-2.9.6/latch_cli/config/user.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/constants.py` & `latch-2.9.6/latch_cli/constants.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/exceptions/handler.py` & `latch-2.9.6/latch_cli/exceptions/handler.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/exceptions/traceback.py` & `latch-2.9.6/latch_cli/exceptions/traceback.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/main.py` & `latch-2.9.6/latch_cli/main.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/cp.py` & `latch-2.9.6/latch_cli/services/cp.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/deprecated/mkdir.py` & `latch-2.9.6/latch_cli/services/deprecated/mkdir.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/deprecated/rm.py` & `latch-2.9.6/latch_cli/services/deprecated/rm.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/deprecated/touch.py` & `latch-2.9.6/latch_cli/services/deprecated/touch.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/execute.py` & `latch-2.9.6/latch_cli/services/execute.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/get.py` & `latch-2.9.6/latch_cli/services/get.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/get_executions.py` & `latch-2.9.6/latch_cli/services/get_executions.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/get_params.py` & `latch-2.9.6/latch_cli/services/get_params.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/init/assemble_and_sort/Dockerfile` & `latch-2.9.6/latch_cli/services/init/assemble_and_sort/Dockerfile`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/init/assemble_and_sort/__init__.py` & `latch-2.9.6/latch_cli/services/init/assemble_and_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/init/example_conda/Dockerfile` & `latch-2.9.6/latch_cli/services/init/example_conda/Dockerfile`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/init/example_conda/__init__.py` & `latch-2.9.6/latch_cli/services/init/example_conda/__init__.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/init/example_r/Dockerfile` & `latch-2.9.6/latch_cli/services/init/example_r/Dockerfile`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/init/example_r/__init__.py` & `latch-2.9.6/latch_cli/services/init/example_r/__init__.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/init/init.py` & `latch-2.9.6/latch_cli/services/init/init.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/launch.py` & `latch-2.9.6/latch_cli/services/launch.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/local_dev.py` & `latch-2.9.6/latch_cli/services/local_dev.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/login.py` & `latch-2.9.6/latch_cli/services/login.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/ls.py` & `latch-2.9.6/latch_cli/services/ls.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/open_file.py` & `latch-2.9.6/latch_cli/services/open_file.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/preview.py` & `latch-2.9.6/latch_cli/services/preview.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/register/register.py` & `latch-2.9.6/latch_cli/services/register/register.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/register/utils.py` & `latch-2.9.6/latch_cli/services/register/utils.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/test_data/ls.py` & `latch-2.9.6/latch_cli/services/test_data/ls.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/test_data/remove.py` & `latch-2.9.6/latch_cli/services/test_data/remove.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/test_data/upload.py` & `latch-2.9.6/latch_cli/services/test_data/upload.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/test_data/utils.py` & `latch-2.9.6/latch_cli/services/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/services/workspace.py` & `latch-2.9.6/latch_cli/services/workspace.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/tinyrequests.py` & `latch-2.9.6/latch_cli/tinyrequests.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/tui.py` & `latch-2.9.6/latch_cli/tui.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/latch_cli/utils.py` & `latch-2.9.6/latch_cli/utils.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/setup.py` & `latch-2.9.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         f"Latch SDK is only supported for Python version is {MIN_PYTHON_VERSION}+."
         f" Detected you are on version {CURRENT_PYTHON}, installation will not proceed!"
     )
     sys.exit(-1)
 
 setup(
     name="latch",
-    version="v2.9.5",
+    version="v2.9.6",
     author_email="kenny@latch.bio",
     description="The Latchbio SDK",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.8",
     entry_points={
         "console_scripts": [
@@ -34,15 +34,15 @@
         "requests>=2.28.1",
         "click>=8.0",
         "docker>=5.0",
         "paramiko>=2.11.0",
         "scp>=0.14.0",
         "boto3>=1.24.22",
         "tqdm>=4.63.0",
-        "lytekit==0.14.2",
+        "lytekit==0.14.8",
         "lytekitplugins-pods==0.4.0",
         "typing-extensions==4.3.0",
         "apscheduler==3.9.1",
         "uvloop==0.17.0",
         "websockets==10.3",
         "prompt-toolkit==3.0.33",
     ],
```

### Comparing `latch-2.9.5/tests/fixtures.py` & `latch-2.9.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/tests/test_cli.py` & `latch-2.9.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `latch-2.9.5/tests/test_launch.py` & `latch-2.9.6/tests/test_launch.py`

 * *Files identical despite different names*

