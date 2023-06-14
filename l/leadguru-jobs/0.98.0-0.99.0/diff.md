# Comparing `tmp/leadguru_jobs-0.98.0.tar.gz` & `tmp/leadguru_jobs-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leadguru_jobs-0.98.0.tar", last modified: Fri Aug 20 14:34:28 2021, max compression
+gzip compressed data, was "leadguru_jobs-0.99.0.tar", last modified: Tue Aug 24 09:23:09 2021, max compression
```

## Comparing `leadguru_jobs-0.98.0.tar` & `leadguru_jobs-0.99.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2021-08-20 14:34:28.254751 leadguru_jobs-0.98.0/
--rw-rw-rw-   0        0        0       65 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/MANIFEST.in
--rw-rw-rw-   0        0        0      904 2021-08-20 14:34:28.254751 leadguru_jobs-0.98.0/PKG-INFO
--rw-rw-rw-   0        0        0     2091 2021-08-16 12:43:36.000000 leadguru_jobs-0.98.0/README.md
-drwxrwxrwx   0        0        0        0 2021-08-20 14:34:28.111117 leadguru_jobs-0.98.0/leadguru_jobs.egg-info/
--rw-rw-rw-   0        0        0      904 2021-08-20 14:34:28.000000 leadguru_jobs-0.98.0/leadguru_jobs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2021-08-20 14:34:28.000000 leadguru_jobs-0.98.0/leadguru_jobs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-20 14:34:28.000000 leadguru_jobs-0.98.0/leadguru_jobs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-08-20 14:34:27.000000 leadguru_jobs-0.98.0/leadguru_jobs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       89 2021-08-20 14:34:28.000000 leadguru_jobs-0.98.0/leadguru_jobs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-08-20 14:34:28.000000 leadguru_jobs-0.98.0/leadguru_jobs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-08-20 14:34:28.157160 leadguru_jobs-0.98.0/lgt_jobs/
--rw-rw-rw-   0        0        0     2974 2021-08-09 09:42:20.000000 leadguru_jobs-0.98.0/lgt_jobs/__init__.py
--rw-rw-rw-   0        0        0     1281 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/lgt_jobs/basejobs.py
--rw-rw-rw-   0        0        0      874 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/lgt_jobs/env.py
-drwxrwxrwx   0        0        0        0 2021-08-20 14:34:28.244575 leadguru_jobs-0.98.0/lgt_jobs/jobs/
--rw-rw-rw-   0        0        0        0 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/__init__.py
--rw-rw-rw-   0        0        0     1295 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/analytics.py
--rw-rw-rw-   0        0        0      852 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/archive_leads.py
--rw-rw-rw-   0        0        0     2078 2021-08-16 12:43:36.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/bot_stats_update.py
--rw-rw-rw-   0        0        0     1608 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/bots_creds_update.py
--rw-rw-rw-   0        0        0     5439 2021-07-01 09:17:12.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/chat_history.py
--rw-rw-rw-   0        0        0     1819 2021-08-09 09:42:20.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/conversation_replied.py
--rw-rw-rw-   0        0        0     2116 2021-08-09 09:42:20.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/reactions_added.py
--rw-rw-rw-   0        0        0     2099 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/restart_bots.py
--rw-rw-rw-   0        0        0     1942 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/restart_dedicated_bots.py
--rw-rw-rw-   0        0        0     5150 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/update_slack_profile.py
--rw-rw-rw-   0        0        0     2031 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/user_bots_creds_update.py
--rw-rw-rw-   0        0        0     2790 2021-08-17 11:07:39.000000 leadguru_jobs-0.98.0/lgt_jobs/jobs/user_limits_update.py
--rw-rw-rw-   0        0        0     5229 2021-08-09 09:42:20.000000 leadguru_jobs-0.98.0/lgt_jobs/k8client.py
--rw-rw-rw-   0        0        0     2260 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/lgt_jobs/main.py
--rw-rw-rw-   0        0        0     1091 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/lgt_jobs/runner.py
--rw-rw-rw-   0        0        0      534 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/lgt_jobs/simple_job.py
--rw-rw-rw-   0        0        0     1382 2021-06-30 10:30:51.000000 leadguru_jobs-0.98.0/lgt_jobs/smtp.py
--rw-rw-rw-   0        0        0      737 2021-08-20 14:34:28.261758 leadguru_jobs-0.98.0/setup.cfg
--rw-rw-rw-   0        0        0     1900 2021-08-20 14:31:22.000000 leadguru_jobs-0.98.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-20 14:34:28.253751 leadguru_jobs-0.98.0/tests/
--rw-rw-rw-   0        0        0        0 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1238 2021-06-07 09:23:28.000000 leadguru_jobs-0.98.0/tests/job_data_test.py
+drwxrwxrwx   0        0        0        0 2021-08-24 09:23:09.616936 leadguru_jobs-0.99.0/
+-rw-rw-rw-   0        0        0       65 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      904 2021-08-24 09:23:09.616936 leadguru_jobs-0.99.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2021-08-16 12:43:36.000000 leadguru_jobs-0.99.0/README.md
+drwxrwxrwx   0        0        0        0 2021-08-24 09:23:09.462795 leadguru_jobs-0.99.0/leadguru_jobs.egg-info/
+-rw-rw-rw-   0        0        0      904 2021-08-24 09:23:09.000000 leadguru_jobs-0.99.0/leadguru_jobs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2021-08-24 09:23:09.000000 leadguru_jobs-0.99.0/leadguru_jobs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-24 09:23:09.000000 leadguru_jobs-0.99.0/leadguru_jobs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-08-24 09:23:08.000000 leadguru_jobs-0.99.0/leadguru_jobs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       89 2021-08-24 09:23:09.000000 leadguru_jobs-0.99.0/leadguru_jobs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2021-08-24 09:23:09.000000 leadguru_jobs-0.99.0/leadguru_jobs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-08-24 09:23:09.515843 leadguru_jobs-0.99.0/lgt_jobs/
+-rw-rw-rw-   0        0        0     2974 2021-08-09 09:42:20.000000 leadguru_jobs-0.99.0/lgt_jobs/__init__.py
+-rw-rw-rw-   0        0        0     1281 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/lgt_jobs/basejobs.py
+-rw-rw-rw-   0        0        0      874 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/lgt_jobs/env.py
+drwxrwxrwx   0        0        0        0 2021-08-24 09:23:09.608928 leadguru_jobs-0.99.0/lgt_jobs/jobs/
+-rw-rw-rw-   0        0        0        0 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/__init__.py
+-rw-rw-rw-   0        0        0     1295 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/analytics.py
+-rw-rw-rw-   0        0        0      852 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/archive_leads.py
+-rw-rw-rw-   0        0        0     2078 2021-08-16 12:43:36.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/bot_stats_update.py
+-rw-rw-rw-   0        0        0     1608 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/bots_creds_update.py
+-rw-rw-rw-   0        0        0     5439 2021-07-01 09:17:12.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/chat_history.py
+-rw-rw-rw-   0        0        0     1819 2021-08-09 09:42:20.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/conversation_replied.py
+-rw-rw-rw-   0        0        0     2116 2021-08-09 09:42:20.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/reactions_added.py
+-rw-rw-rw-   0        0        0     2099 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/restart_bots.py
+-rw-rw-rw-   0        0        0     1942 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/restart_dedicated_bots.py
+-rw-rw-rw-   0        0        0     5150 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/update_slack_profile.py
+-rw-rw-rw-   0        0        0     2031 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/user_bots_creds_update.py
+-rw-rw-rw-   0        0        0     2790 2021-08-17 11:07:39.000000 leadguru_jobs-0.99.0/lgt_jobs/jobs/user_limits_update.py
+-rw-rw-rw-   0        0        0     5229 2021-08-09 09:42:20.000000 leadguru_jobs-0.99.0/lgt_jobs/k8client.py
+-rw-rw-rw-   0        0        0     2260 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/lgt_jobs/main.py
+-rw-rw-rw-   0        0        0     1091 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/lgt_jobs/runner.py
+-rw-rw-rw-   0        0        0      534 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/lgt_jobs/simple_job.py
+-rw-rw-rw-   0        0        0     1382 2021-06-30 10:30:51.000000 leadguru_jobs-0.99.0/lgt_jobs/smtp.py
+-rw-rw-rw-   0        0        0      737 2021-08-24 09:23:09.617936 leadguru_jobs-0.99.0/setup.cfg
+-rw-rw-rw-   0        0        0     1900 2021-08-20 14:31:22.000000 leadguru_jobs-0.99.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-24 09:23:09.615935 leadguru_jobs-0.99.0/tests/
+-rw-rw-rw-   0        0        0        0 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1238 2021-06-07 09:23:28.000000 leadguru_jobs-0.99.0/tests/job_data_test.py
```

### Comparing `leadguru_jobs-0.98.0/PKG-INFO` & `leadguru_jobs-0.99.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leadguru_jobs
-Version: 0.98.0
+Version: 0.99.0
 Summary: LGT jobs builds
 Home-page: UNKNOWN
 Author-email: developer@leadguru.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `leadguru_jobs-0.98.0/README.md` & `leadguru_jobs-0.99.0/README.md`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/leadguru_jobs.egg-info/PKG-INFO` & `leadguru_jobs-0.99.0/leadguru_jobs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leadguru-jobs
-Version: 0.98.0
+Version: 0.99.0
 Summary: LGT jobs builds
 Home-page: UNKNOWN
 Author-email: developer@leadguru.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `leadguru_jobs-0.98.0/leadguru_jobs.egg-info/SOURCES.txt` & `leadguru_jobs-0.99.0/leadguru_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/__init__.py` & `leadguru_jobs-0.99.0/lgt_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/basejobs.py` & `leadguru_jobs-0.99.0/lgt_jobs/basejobs.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/env.py` & `leadguru_jobs-0.99.0/lgt_jobs/env.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/analytics.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/analytics.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/archive_leads.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/archive_leads.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/bot_stats_update.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/bot_stats_update.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/bots_creds_update.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/bots_creds_update.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/chat_history.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/chat_history.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/conversation_replied.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/conversation_replied.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/reactions_added.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/reactions_added.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/restart_bots.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/restart_bots.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/restart_dedicated_bots.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/restart_dedicated_bots.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/update_slack_profile.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/update_slack_profile.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/user_bots_creds_update.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/user_bots_creds_update.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/jobs/user_limits_update.py` & `leadguru_jobs-0.99.0/lgt_jobs/jobs/user_limits_update.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/k8client.py` & `leadguru_jobs-0.99.0/lgt_jobs/k8client.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/main.py` & `leadguru_jobs-0.99.0/lgt_jobs/main.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/runner.py` & `leadguru_jobs-0.99.0/lgt_jobs/runner.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/simple_job.py` & `leadguru_jobs-0.99.0/lgt_jobs/simple_job.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/lgt_jobs/smtp.py` & `leadguru_jobs-0.99.0/lgt_jobs/smtp.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/setup.cfg` & `leadguru_jobs-0.99.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/setup.py` & `leadguru_jobs-0.99.0/setup.py`

 * *Files identical despite different names*

### Comparing `leadguru_jobs-0.98.0/tests/job_data_test.py` & `leadguru_jobs-0.99.0/tests/job_data_test.py`

 * *Files identical despite different names*

