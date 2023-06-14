# Comparing `tmp/bullmq-0.5.3.tar.gz` & `tmp/bullmq-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.5.3.tar", last modified: Tue Jun 13 16:46:50 2023, max compression
+gzip compressed data, was "bullmq-0.5.4.tar", last modified: Wed Jun 14 14:01:52 2023, max compression
```

## Comparing `bullmq-0.5.3.tar` & `bullmq-0.5.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.098966 bullmq-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 16:46:50.098966 bullmq-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-13 16:44:57.000000 bullmq-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.094966 bullmq-0.5.3/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 16:46:47.000000 bullmq-0.5.3/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.098966 bullmq-0.5.3/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/addJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/changePriority-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getState-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/pause-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/promote-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.098966 bullmq-0.5.3/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.094966 bullmq-0.5.3/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-13 16:46:50.098966 bullmq-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 16:44:57.000000 bullmq-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.110907 bullmq-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-14 14:01:52.110907 bullmq-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-14 14:00:25.000000 bullmq-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.102907 bullmq-0.5.4/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 14:01:50.000000 bullmq-0.5.4/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.106907 bullmq-0.5.4/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/changePriority-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getState-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/pause-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/promote-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.110907 bullmq-0.5.4/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.102907 bullmq-0.5.4/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 14:01:52.110907 bullmq-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-14 14:00:25.000000 bullmq-0.5.4/setup.py
```

### Comparing `bullmq-0.5.3/PKG-INFO` & `bullmq-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.3
+Version: 0.5.4
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.3/README.md` & `bullmq-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/backoffs.py` & `bullmq-0.5.4/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/addJob-8.lua` & `bullmq-0.5.4/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/changeDelay-3.lua` & `bullmq-0.5.4/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/changePriority-4.lua` & `bullmq-0.5.4/bullmq/commands/changePriority-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.5.4/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/drain-4.lua` & `bullmq-0.5.4/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/getCounts-1.lua` & `bullmq-0.5.4/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/getRanges-1.lua` & `bullmq-0.5.4/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/getState-7.lua` & `bullmq-0.5.4/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/getStateV2-7.lua` & `bullmq-0.5.4/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/isFinished-3.lua` & `bullmq-0.5.4/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-0.5.4/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.5.4/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/moveToActive-9.lua` & `bullmq-0.5.4/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.5.4/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.5.4/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.5.4/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/obliterate-2.lua` & `bullmq-0.5.4/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/promote-6.lua` & `bullmq-0.5.4/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/removeJob-1.lua` & `bullmq-0.5.4/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.5.4/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/reprocessJob-6.lua` & `bullmq-0.5.4/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/retryJob-8.lua` & `bullmq-0.5.4/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/commands/retryJobs-6.lua` & `bullmq-0.5.4/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/event_emitter.py` & `bullmq-0.5.4/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/job.py` & `bullmq-0.5.4/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/queue.py` & `bullmq-0.5.4/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/scripts.py` & `bullmq-0.5.4/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/timer.py` & `bullmq-0.5.4/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/types/job_options.py` & `bullmq-0.5.4/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/types/worker_options.py` & `bullmq-0.5.4/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq/worker.py` & `bullmq-0.5.4/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/bullmq.egg-info/PKG-INFO` & `bullmq-0.5.4/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.3
+Version: 0.5.4
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.3/bullmq.egg-info/SOURCES.txt` & `bullmq-0.5.4/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.3/setup.py` & `bullmq-0.5.4/setup.py`

 * *Files identical despite different names*

