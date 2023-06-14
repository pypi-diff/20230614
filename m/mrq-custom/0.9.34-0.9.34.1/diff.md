# Comparing `tmp/mrq-custom-0.9.34.tar.gz` & `tmp/mrq-custom-0.9.34.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrq-custom-0.9.34.tar", last modified: Wed May 17 13:44:25 2023, max compression
+gzip compressed data, was "mrq-custom-0.9.34.1.tar", last modified: Wed May 17 14:02:38 2023, max compression
```

## Comparing `mrq-custom-0.9.34.tar` & `mrq-custom-0.9.34.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.742194 mrq-custom-0.9.34/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1083 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/LICENSE
--rw-r--r--   0 ghabrielv   (501) staff       (20)      145 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/MANIFEST.in
--rw-r--r--   0 ghabrielv   (501) staff       (20)     9261 2023-05-17 13:44:25.741461 mrq-custom-0.9.34/PKG-INFO
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8270 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/README.md
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.679951 mrq-custom-0.9.34/mrq/
--rw-r--r--   0 ghabrielv   (501) staff       (20)       12 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     7500 2023-05-16 19:30:24.000000 mrq-custom-0.9.34/mrq/agent.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.681877 mrq-custom-0.9.34/mrq/basetasks/
--rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/basetasks/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/basetasks/cleaning.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2167 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/basetasks/indexes.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3901 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/basetasks/orchestrator.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     5813 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/basetasks/utils.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.683269 mrq-custom-0.9.34/mrq/bin/
--rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/bin/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      857 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/bin/mrq_agent.py
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     2229 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/bin/mrq_run.py
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1509 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/bin/mrq_worker.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    18048 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/config.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8222 2023-05-17 13:39:52.000000 mrq-custom-0.9.34/mrq/context.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.684302 mrq-custom-0.9.34/mrq/dashboard/
--rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    11412 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/app.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.685021 mrq-custom-0.9.34/mrq/dashboard/static/
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.689773 mrq-custom-0.9.34/mrq/dashboard/static/bin/
--rw-r--r--   0 ghabrielv   (501) staff       (20)   469976 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/0.bundle.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2943 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/bundle.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.691707 mrq-custom-0.9.34/mrq/dashboard/static/css/
--rw-r--r--   0 ghabrielv   (501) staff       (20)   123361 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/css/bootstrap-theme.min.css
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3694 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/css/datatables.css
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)      367 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/css/jquery.circliful.css
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1453 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/css/mrq-dashboard.css
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.693908 mrq-custom-0.9.34/mrq/dashboard/static/fonts/
--rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.698471 mrq-custom-0.9.34/mrq/dashboard/static/images/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1406 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/images/favicon-old.ico
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1579 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/images/favicon.ico
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/images/sort_asc.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/images/sort_asc_disabled.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/images/sort_both.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/images/sort_desc.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/images/sort_desc_disabled.png
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.701046 mrq-custom-0.9.34/mrq/dashboard/static/js/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2620 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/app.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4947 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/main.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)       84 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/models.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3977 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/router.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.710051 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/
--rw-r--r--   0 ghabrielv   (501) staff       (20)    19967 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/backbone.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     9618 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/backbone.queryparams.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    55258 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/bootstrap.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    29110 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/bootstrap.min.js
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     7045 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/datatables.bs3.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    83614 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3096 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery.circliful.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    70857 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    43246 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    26050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/moment.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    80376 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/require.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    14643 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/underscore.min.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.719286 mrq-custom-0.9.34/mrq/dashboard/static/js/views/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/agents.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.722362 mrq-custom-0.9.34/mrq/dashboard/static/js/views/generic/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     6664 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/generic/datatablepage.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4645 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/generic/page.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4697 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/index.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4107 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/io.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    15498 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/jobs.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     5180 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/queues.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4263 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/root.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2211 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/scheduledjobs.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2360 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/status.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2873 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/taskexceptions.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2235 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/taskpaths.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)      879 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/workergroups.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     6884 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/js/views/workers.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)      562 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/package.json
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1484 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/static/webpack.config.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.727209 mrq-custom-0.9.34/mrq/dashboard/templates/
--rw-r--r--   0 ghabrielv   (501) staff       (20)    17348 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/templates/index.html
--rw-r--r--   0 ghabrielv   (501) staff       (20)    43302 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/templates/library.html
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1388 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/dashboard/utils.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1638 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/exceptions.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      918 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/helpers.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    25667 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/job.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3573 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/logger.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    15471 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/monkey.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     6460 2023-05-04 14:04:25.000000 mrq-custom-0.9.34/mrq/processes.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8652 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/queue.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8586 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/queue_raw.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4991 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/queue_regular.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2251 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/redishelpers.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4982 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/scheduler.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3326 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/subpool.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      737 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/supervisor.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      663 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/task.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/mrq/utils.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)       88 2023-05-17 13:42:49.000000 mrq-custom-0.9.34/mrq/version.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    24931 2023-05-16 19:30:24.000000 mrq-custom-0.9.34/mrq/worker.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 13:44:25.739797 mrq-custom-0.9.34/mrq_custom.egg-info/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     9261 2023-05-17 13:44:25.000000 mrq-custom-0.9.34/mrq_custom.egg-info/PKG-INFO
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3821 2023-05-17 13:44:25.000000 mrq-custom-0.9.34/mrq_custom.egg-info/SOURCES.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-17 13:44:25.000000 mrq-custom-0.9.34/mrq_custom.egg-info/dependency_links.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      160 2023-05-17 13:44:25.000000 mrq-custom-0.9.34/mrq_custom.egg-info/entry_points.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-09 15:38:54.000000 mrq-custom-0.9.34/mrq_custom.egg-info/not-zip-safe
--rw-r--r--   0 ghabrielv   (501) staff       (20)      169 2023-05-17 13:44:25.000000 mrq-custom-0.9.34/mrq_custom.egg-info/requires.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)        4 2023-05-17 13:44:25.000000 mrq-custom-0.9.34/mrq_custom.egg-info/top_level.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      268 2023-05-16 19:30:24.000000 mrq-custom-0.9.34/requirements-base.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/requirements-dashboard.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      337 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/requirements-dev.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/requirements-heroku.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      205 2023-05-09 16:04:20.000000 mrq-custom-0.9.34/requirements.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)       38 2023-05-17 13:44:25.742554 mrq-custom-0.9.34/setup.cfg
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3036 2023-03-10 20:48:18.000000 mrq-custom-0.9.34/setup.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:38.024497 mrq-custom-0.9.34.1/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1083 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/LICENSE
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      145 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/MANIFEST.in
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     9263 2023-05-17 14:02:38.023863 mrq-custom-0.9.34.1/PKG-INFO
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8270 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/README.md
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.952586 mrq-custom-0.9.34.1/mrq/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       12 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     7500 2023-05-16 19:30:24.000000 mrq-custom-0.9.34.1/mrq/agent.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.955764 mrq-custom-0.9.34.1/mrq/basetasks/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/basetasks/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/basetasks/cleaning.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2167 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/basetasks/indexes.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3901 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/basetasks/orchestrator.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     5813 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/basetasks/utils.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.958580 mrq-custom-0.9.34.1/mrq/bin/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/bin/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      857 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/bin/mrq_agent.py
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     2229 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/bin/mrq_run.py
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1509 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/bin/mrq_worker.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    18048 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/config.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8238 2023-05-17 13:59:54.000000 mrq-custom-0.9.34.1/mrq/context.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.960567 mrq-custom-0.9.34.1/mrq/dashboard/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    11412 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/app.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.961813 mrq-custom-0.9.34.1/mrq/dashboard/static/
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.975186 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)   469976 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/0.bundle.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2943 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/bundle.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.978871 mrq-custom-0.9.34.1/mrq/dashboard/static/css/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)   123361 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/css/bootstrap-theme.min.css
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3694 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/css/datatables.css
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)      367 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/css/jquery.circliful.css
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1453 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/css/mrq-dashboard.css
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.981520 mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.985840 mrq-custom-0.9.34.1/mrq/dashboard/static/images/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1406 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/images/favicon-old.ico
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1579 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/images/favicon.ico
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_asc.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_asc_disabled.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_both.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_desc.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_desc_disabled.png
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:37.988885 mrq-custom-0.9.34.1/mrq/dashboard/static/js/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2620 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/app.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4947 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/main.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       84 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/models.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3977 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/router.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:38.000117 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    19967 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/backbone.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     9618 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/backbone.queryparams.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    55258 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/bootstrap.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    29110 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/bootstrap.min.js
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     7045 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/datatables.bs3.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    83614 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3096 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery.circliful.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    70857 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    43246 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    26050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/moment.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    80376 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/require.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    14643 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/underscore.min.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:38.006783 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/agents.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:38.008277 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/generic/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     6664 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/generic/datatablepage.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4645 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/generic/page.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4697 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/index.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4107 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/io.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    15498 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/jobs.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     5180 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/queues.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4263 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/root.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2211 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/scheduledjobs.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2360 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/status.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2873 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/taskexceptions.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2235 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/taskpaths.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      879 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/workergroups.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     6884 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/workers.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      562 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/package.json
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1484 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/static/webpack.config.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:38.010873 mrq-custom-0.9.34.1/mrq/dashboard/templates/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    17348 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/templates/index.html
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    43302 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/templates/library.html
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1388 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/dashboard/utils.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1638 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/exceptions.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      918 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/helpers.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    25667 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/job.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3573 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/logger.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    15471 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/monkey.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     6460 2023-05-04 14:04:25.000000 mrq-custom-0.9.34.1/mrq/processes.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8652 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/queue.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8586 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/queue_raw.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4991 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/queue_regular.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2251 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/redishelpers.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4982 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/scheduler.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3326 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/subpool.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      737 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/supervisor.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      663 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/task.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8050 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/mrq/utils.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       90 2023-05-17 14:01:11.000000 mrq-custom-0.9.34.1/mrq/version.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    24931 2023-05-16 19:30:24.000000 mrq-custom-0.9.34.1/mrq/worker.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-17 14:02:38.022955 mrq-custom-0.9.34.1/mrq_custom.egg-info/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     9263 2023-05-17 14:02:37.000000 mrq-custom-0.9.34.1/mrq_custom.egg-info/PKG-INFO
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3821 2023-05-17 14:02:37.000000 mrq-custom-0.9.34.1/mrq_custom.egg-info/SOURCES.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-17 14:02:37.000000 mrq-custom-0.9.34.1/mrq_custom.egg-info/dependency_links.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      160 2023-05-17 14:02:37.000000 mrq-custom-0.9.34.1/mrq_custom.egg-info/entry_points.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-09 15:38:54.000000 mrq-custom-0.9.34.1/mrq_custom.egg-info/not-zip-safe
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      169 2023-05-17 14:02:37.000000 mrq-custom-0.9.34.1/mrq_custom.egg-info/requires.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        4 2023-05-17 14:02:37.000000 mrq-custom-0.9.34.1/mrq_custom.egg-info/top_level.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      268 2023-05-16 19:30:24.000000 mrq-custom-0.9.34.1/requirements-base.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/requirements-dashboard.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      337 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/requirements-dev.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/requirements-heroku.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      205 2023-05-09 16:04:20.000000 mrq-custom-0.9.34.1/requirements.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       38 2023-05-17 14:02:38.024674 mrq-custom-0.9.34.1/setup.cfg
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3036 2023-03-10 20:48:18.000000 mrq-custom-0.9.34.1/setup.py
```

### Comparing `mrq-custom-0.9.34/LICENSE` & `mrq-custom-0.9.34.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/PKG-INFO` & `mrq-custom-0.9.34.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrq-custom
-Version: 0.9.34
+Version: 0.9.34.1
 Summary: A simple yet powerful distributed worker task queue in Python
 Home-page: http://github.com/pricingassistant/mrq
 Author: Pricing Assistant
 Author-email: contact@pricingassistant.com
 License: MIT
 Keywords: worker,task,distributed,queue,asynchronous,redis,mongodb,job,processing,gevent
 Platform: any
```

### Comparing `mrq-custom-0.9.34/README.md` & `mrq-custom-0.9.34.1/README.md`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/agent.py` & `mrq-custom-0.9.34.1/mrq/agent.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/basetasks/cleaning.py` & `mrq-custom-0.9.34.1/mrq/basetasks/cleaning.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/basetasks/indexes.py` & `mrq-custom-0.9.34.1/mrq/basetasks/indexes.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/basetasks/orchestrator.py` & `mrq-custom-0.9.34.1/mrq/basetasks/orchestrator.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/basetasks/utils.py` & `mrq-custom-0.9.34.1/mrq/basetasks/utils.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/bin/mrq_agent.py` & `mrq-custom-0.9.34.1/mrq/bin/mrq_agent.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/bin/mrq_run.py` & `mrq-custom-0.9.34.1/mrq/bin/mrq_run.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/bin/mrq_worker.py` & `mrq-custom-0.9.34.1/mrq/bin/mrq_worker.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/config.py` & `mrq-custom-0.9.34.1/mrq/config.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/context.py` & `mrq-custom-0.9.34.1/mrq/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                 max_connections=int(config.get("redis_max_connections")),
                 timeout=int(config.get("redis_timeout")),
                 decode_responses=False,
                 connection_class=connection_class
             )
 
             if redis_url.scheme == "rediss":
-                connection_class = pyredisconnection.SSLConnection
+                redis_params["connection_class"] = pyredisconnection.SSLConnection
                 redis_params["ssl_cert_reqs"] = "none"
 
             redis_pool = pyredis.BlockingConnectionPool(**redis_params)
 
             log.info("%s: Connecting to Redis at %s..." %
                      (attr, redis_url.hostname))
```

### Comparing `mrq-custom-0.9.34/mrq/dashboard/app.py` & `mrq-custom-0.9.34.1/mrq/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/0.bundle.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/0.bundle.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/bundle.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/bundle.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf` & `mrq-custom-0.9.34.1/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/css/bootstrap-theme.min.css` & `mrq-custom-0.9.34.1/mrq/dashboard/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/css/datatables.css` & `mrq-custom-0.9.34.1/mrq/dashboard/static/css/datatables.css`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/css/mrq-dashboard.css` & `mrq-custom-0.9.34.1/mrq/dashboard/static/css/mrq-dashboard.css`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot` & `mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg` & `mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf` & `mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff` & `mrq-custom-0.9.34.1/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/images/favicon-old.ico` & `mrq-custom-0.9.34.1/mrq/dashboard/static/images/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/images/favicon.ico` & `mrq-custom-0.9.34.1/mrq/dashboard/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/images/sort_asc.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/images/sort_asc_disabled.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/images/sort_both.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/images/sort_desc.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/images/sort_desc_disabled.png` & `mrq-custom-0.9.34.1/mrq/dashboard/static/images/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/app.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/app.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/main.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/main.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/router.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/router.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/backbone.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/backbone.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/backbone.queryparams.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/backbone.queryparams.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/bootstrap.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/bootstrap.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/datatables.bs3.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/datatables.bs3.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery.circliful.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery.circliful.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/moment.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/moment.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/require.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/require.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/vendor/underscore.min.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/vendor/underscore.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/agents.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/agents.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/generic/datatablepage.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/generic/datatablepage.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/generic/page.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/generic/page.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/index.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/index.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/io.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/io.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/jobs.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/jobs.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/queues.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/queues.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/root.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/root.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/scheduledjobs.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/scheduledjobs.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/status.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/status.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/taskexceptions.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/taskexceptions.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/taskpaths.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/taskpaths.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/workergroups.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/workergroups.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/js/views/workers.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/js/views/workers.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/package.json` & `mrq-custom-0.9.34.1/mrq/dashboard/static/package.json`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/static/webpack.config.js` & `mrq-custom-0.9.34.1/mrq/dashboard/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/templates/index.html` & `mrq-custom-0.9.34.1/mrq/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/templates/library.html` & `mrq-custom-0.9.34.1/mrq/dashboard/templates/library.html`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/dashboard/utils.py` & `mrq-custom-0.9.34.1/mrq/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/exceptions.py` & `mrq-custom-0.9.34.1/mrq/exceptions.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/helpers.py` & `mrq-custom-0.9.34.1/mrq/helpers.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/job.py` & `mrq-custom-0.9.34.1/mrq/job.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/logger.py` & `mrq-custom-0.9.34.1/mrq/logger.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/monkey.py` & `mrq-custom-0.9.34.1/mrq/monkey.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/processes.py` & `mrq-custom-0.9.34.1/mrq/processes.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/queue.py` & `mrq-custom-0.9.34.1/mrq/queue.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/queue_raw.py` & `mrq-custom-0.9.34.1/mrq/queue_raw.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/queue_regular.py` & `mrq-custom-0.9.34.1/mrq/queue_regular.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/redishelpers.py` & `mrq-custom-0.9.34.1/mrq/redishelpers.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/scheduler.py` & `mrq-custom-0.9.34.1/mrq/scheduler.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/subpool.py` & `mrq-custom-0.9.34.1/mrq/subpool.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/supervisor.py` & `mrq-custom-0.9.34.1/mrq/supervisor.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/task.py` & `mrq-custom-0.9.34.1/mrq/task.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/utils.py` & `mrq-custom-0.9.34.1/mrq/utils.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq/worker.py` & `mrq-custom-0.9.34.1/mrq/worker.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/mrq_custom.egg-info/PKG-INFO` & `mrq-custom-0.9.34.1/mrq_custom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrq-custom
-Version: 0.9.34
+Version: 0.9.34.1
 Summary: A simple yet powerful distributed worker task queue in Python
 Home-page: http://github.com/pricingassistant/mrq
 Author: Pricing Assistant
 Author-email: contact@pricingassistant.com
 License: MIT
 Keywords: worker,task,distributed,queue,asynchronous,redis,mongodb,job,processing,gevent
 Platform: any
```

### Comparing `mrq-custom-0.9.34/mrq_custom.egg-info/SOURCES.txt` & `mrq-custom-0.9.34.1/mrq_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.34/setup.py` & `mrq-custom-0.9.34.1/setup.py`

 * *Files identical despite different names*

