# Comparing `tmp/girder-jobs-3.1.9.dev6.tar.gz` & `tmp/girder-jobs-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-jobs-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:52 2022, max compression
+gzip compressed data, was "dist/girder-jobs-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:52 2022, max compression
```

## Comparing `girder-jobs-3.1.9.dev6.tar` & `girder-jobs-3.1.9.dev8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22898 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/models/job.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/collections/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      227 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/collections/JobCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/collections/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/models/JobModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/models/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/stylesheets/jobListWidget.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/adminViewMenuItem.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/headerUserViewMenu.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobCheckBoxContent.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2232 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobDetailsWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1940 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobListWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobsGraphWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      399 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/AdminView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2192 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/CheckBoxMenu.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/HeaderUserView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4906 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/JobDetailsWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8414 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/JobGraphWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12083 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/JobListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8304 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/timeChartConfig.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11782 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/timingHistoryChartConfig.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/JobStatus.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      642 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1195 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2077 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8965 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/girder_jobs/job_rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1802 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/girder_jobs.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21567 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/plugin_tests/jobsSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24912 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/plugin_tests/jobs_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/plugin_tests/local_job_impl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       49 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-02-23 16:09:15.000000 girder-jobs-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:52.000000 girder-jobs-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22898 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/models/job.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/collections/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      227 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/collections/JobCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/collections/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/models/JobModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/models/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/stylesheets/jobListWidget.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/adminViewMenuItem.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/headerUserViewMenu.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobCheckBoxContent.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2232 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobDetailsWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1940 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobListWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobsGraphWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      399 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/AdminView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2192 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/CheckBoxMenu.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/HeaderUserView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4906 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/JobDetailsWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8414 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/JobGraphWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12083 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/JobListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8304 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/timeChartConfig.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11782 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/timingHistoryChartConfig.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/JobStatus.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      642 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1195 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2077 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8965 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/girder_jobs/job_rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1802 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/girder_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21567 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/plugin_tests/jobsSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24912 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/plugin_tests/jobs_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/plugin_tests/local_job_impl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       49 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-02-23 17:41:16.000000 girder-jobs-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:52.000000 girder-jobs-3.1.9.dev8/setup.cfg
```

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/models/job.py` & `girder-jobs-3.1.9.dev8/girder_jobs/models/job.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/models/JobModel.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/models/JobModel.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/stylesheets/jobListWidget.styl` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/stylesheets/jobListWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobDetailsWidget.pug` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobDetailsWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobList.pug` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobList.pug`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/templates/jobListWidget.pug` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/templates/jobListWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/CheckBoxMenu.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/CheckBoxMenu.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/HeaderUserView.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/JobDetailsWidget.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/JobDetailsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/JobGraphWidget.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/JobGraphWidget.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/JobListWidget.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/JobListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/timeChartConfig.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/timeChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/views/timingHistoryChartConfig.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/views/timingHistoryChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/JobStatus.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/JobStatus.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/package.json` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/web_client/routes.js` & `girder-jobs-3.1.9.dev8/girder_jobs/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/__init__.py` & `girder-jobs-3.1.9.dev8/girder_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/constants.py` & `girder-jobs-3.1.9.dev8/girder_jobs/constants.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs/job_rest.py` & `girder-jobs-3.1.9.dev8/girder_jobs/job_rest.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs.egg-info/PKG-INFO` & `girder-jobs-3.1.9.dev8/girder_jobs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-jobs
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: A general purpose plugin for managing offline jobs.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#jobs
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-jobs-3.1.9.dev6/girder_jobs.egg-info/SOURCES.txt` & `girder-jobs-3.1.9.dev8/girder_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/plugin_tests/jobsSpec.js` & `girder-jobs-3.1.9.dev8/plugin_tests/jobsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/plugin_tests/jobs_test.py` & `girder-jobs-3.1.9.dev8/plugin_tests/jobs_test.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/setup.py` & `girder-jobs-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.1.9.dev6/PKG-INFO` & `girder-jobs-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-jobs
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: A general purpose plugin for managing offline jobs.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#jobs
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

