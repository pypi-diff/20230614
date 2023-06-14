# Comparing `tmp/etm-dgraham-5.0.7.tar.gz` & `tmp/etm-dgraham-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.0.7.tar", last modified: Thu Jun  8 12:38:43 2023, max compression
+gzip compressed data, was "etm-dgraham-5.0.8.tar", last modified: Wed Jun 14 00:21:08 2023, max compression
```

## Comparing `etm-dgraham-5.0.7.tar` & `etm-dgraham-5.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.760417 etm-dgraham-5.0.7/
--rw-r--r--   0 dag        (501) staff       (20)     2361 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-08 12:38:43.760237 etm-dgraham-5.0.7/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.7/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.7/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.7/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.754487 etm-dgraham-5.0.7/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.756811 etm-dgraham-5.0.7/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.7/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.7/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.7/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.7/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   280674 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.7/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.7/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    98299 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.758654 etm-dgraham-5.0.7/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.7/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.7/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-08 12:38:43.760473 etm-dgraham-5.0.7/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.7/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.758751 etm-dgraham-5.0.7/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.7/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.759629 etm-dgraham-5.0.7/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.7/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.7/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.7/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.526338 etm-dgraham-5.0.8/
+-rw-r--r--   0 dag        (501) staff       (20)     2463 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   129624 2023-06-14 00:21:08.526166 etm-dgraham-5.0.8/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   128712 2023-06-08 20:23:17.000000 etm-dgraham-5.0.8/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.8/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.8/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.518404 etm-dgraham-5.0.8/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.522472 etm-dgraham-5.0.8/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.0.8/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.8/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.8/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.8/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   282318 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37350 2023-06-08 15:18:02.000000 etm-dgraham-5.0.8/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.8/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    98133 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.524513 etm-dgraham-5.0.8/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   129624 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.8/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.8/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-14 00:21:08.526380 etm-dgraham-5.0.8/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.8/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.524608 etm-dgraham-5.0.8/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.8/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.525551 etm-dgraham-5.0.8/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.8/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.8/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.8/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.0.7/CHANGES.txt` & `etm-dgraham-5.0.8/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,83 @@
-Recent tagged changes as of 2023-06-08T08:38:27.324898-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.0.7) Daniel Graham
+Recent tagged changes as of 2023-06-13T20:17:48.417919-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.0.8) Daniel Graham
+    1f587d1 2023-06-13 20:17:48 -0400
+    Tagged version 5.0.8. Only display and allow completion of jthe
+    jobs of the oldest unfinished instance of a repeating task.
+
+- 6 days ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
 
-- 3 days ago (tag: 5.0.6) Daniel Graham
+- 8 days ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
-- 3 days ago (tag: 5.0.5) Daniel Graham
+- 9 days ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
-- 3 days ago (tag: 5.0.4) Daniel Graham
+- 9 days ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
-- 4 days ago (tag: 5.0.3) Daniel Graham
+- 9 days ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
-- 4 days ago (tag: 5.0.2) Daniel Graham
+- 9 days ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 4 days ago (tag: 5.0.1) Daniel Graham
+- 9 days ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
-- 5 days ago (tag: 5.0.0) Daniel Graham
+- 11 days ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
 
-- 12 days ago (tag: 4.12.9) Daniel Graham
+- 2 weeks ago (tag: 4.12.9) Daniel Graham
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
 
-- 13 days ago (tag: 4.12.8) Daniel Graham
+- 3 weeks ago (tag: 4.12.8) Daniel Graham
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
 
-- 2 weeks ago (tag: 4.12.7) Daniel Graham
+- 3 weeks ago (tag: 4.12.7) Daniel Graham
     442ff98 2023-05-25 13:53:52 -0400
     Tagged version 4.12.7.
 
-- 2 weeks ago (tag: 4.12.6) Daniel Graham
+- 3 weeks ago (tag: 4.12.6) Daniel Graham
     3da7332 2023-05-23 14:01:37 -0400
     Tagged version 4.12.6.
 
 - 3 weeks ago (tag: 4.12.5) Daniel Graham
     f0c24d8 2023-05-21 15:08:06 -0400
     Tagged version 4.12.5.
 
 - 3 weeks ago (tag: 4.12.4) Daniel Graham
     15b3333 2023-05-20 14:33:40 -0400
     Tagged version 4.12.4.
 
-- 3 weeks ago (tag: 4.12.3) Daniel Graham
+- 4 weeks ago (tag: 4.12.3) Daniel Graham
     dd49fda 2023-05-17 12:24:12 -0400
     Tagged version 4.12.3.
 
-- 3 weeks ago (tag: 4.12.2) Daniel Graham
+- 4 weeks ago (tag: 4.12.2) Daniel Graham
     2a304a3 2023-05-17 09:34:05 -0400
     Tagged version 4.12.2.
 
-- 3 weeks ago (tag: 4.12.1) Daniel Graham
+- 4 weeks ago (tag: 4.12.1) Daniel Graham
     68005b7 2023-05-15 14:20:25 -0400
     Tagged version 4.12.1. Added display for all-day events to busy
     view
 
 - 4 weeks ago (tag: 4.12.0) Daniel Graham
     ce2ab09 2023-05-13 12:46:39 -0400
     Tagged version 4.12.0. Added engaged view
 
-- 4 weeks ago (tag: 4.11.18) Daniel Graham
+- 5 weeks ago (tag: 4.11.18) Daniel Graham
     cd5482a 2023-05-11 12:20:48 -0400
     Tagged version 4.11.18.
-
-- 4 weeks ago (tag: 4.11.17) Daniel Graham
-    8a02515 2023-05-09 10:14:28 -0400
-    Tagged version 4.11.17.
```

### Comparing `etm-dgraham-5.0.7/PKG-INFO` & `etm-dgraham-5.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.7
+Version: 5.0.8
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -920,15 +920,15 @@
 The recommended workflow for updating reminders is first
 to perfect the query to be certain that it lists just the
 items you want to update. Then press 'q' and the 'up'
 cursor key to restore the previous query, add ' | ' and
 the update command you want with its arguments.
 
 WARNING: Since the results may not be reversible, consider
-backing up your 'db.json' database before using update
+backing up your 'etm.json' database before using update
 commands. This simple query, e.g., would PERMANENTLY DELETE
 ALL YOUR REMINDERS:
 
     query exists itemtype | remove
 
 
 [↺ contents](#contents)
@@ -1139,15 +1139,15 @@
 
 [↺ contents](#contents)
 
 ## Mobile access to your reminders {#mobile}
 
 The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
 
-* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary.
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary. A width of 46, for example, works well for an iPhone in portrait mode.
 
 * `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
 
 By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
 
 Here is a screen shot from an iPhone of an illustrative `current.txt`:
 
@@ -1431,17 +1431,17 @@
 
 Whatever *home* directory you choose, running etm for the first time will add the following to that directory.
 
         etm home directory/
             backups/
             logs/
             cfg.yaml
-            db.json
+            etm.json
 
-Here `cfg.yaml` is your user configuration file and `db.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `db.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
+Here `cfg.yaml` is your user configuration file and `etm.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `etm.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
 
 The file `cfg.yaml` can be edited and the options are documented in the file.
 See [configuration](#configuration) for details.
 
 [↺ contents](#contents)
 
 ### Timers {#timers}
@@ -1584,15 +1584,15 @@
 
 - The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is scheduled to be completed.
     - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the scheduled time.
     - Tasks with `@s` date entry are regarded as past due after the due date and are displayed in *Agenda View* on the due date after all items with datetimes.
     - Tasks that are past due are also displayed in *Agenda View* on the current date using the type character `<` with an indication of the number of days that the task is past due.
 - Tasks without an `@s` entry are to be completed when possible and are sometimes called *todos*. They are regarded as *next* items in the *Getting Things Done* terminology and are displayed in *Do Next* view grouped by @l (location/context).
 - Tasks with an `@r` (repeat) or an `@+` entry can have an `@o` (overdue) setting.
-	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. This is the default when no `@o` entry is given.
+	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. The default when no `@o` entry is given is `@o k`.
 	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
 	- `@o s`: skip. Like 'keep' with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
 
 	    Furthermore, if the options setting `limit_skip_display` were true, then only the first instance of such a task would be displayed in agenda view. E.g., with the `limit_skip_display` setting true, then for the task
 
 			- meds @s +0d @r d &h 8,14,20 @o s
 
@@ -1759,15 +1759,15 @@
 *  @h: history. (for repeating tasks, a list of the most recent completion datetimes)
 *  @i: index. forward slash delimited string. E.g., client/project/activity
 *  @j*: job summary. string, optionally followed by job &key entries
 *  @k*: doc_id. connect this reminder to the one corresponding to doc_id.
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
-*  @o: overdue. character from (r) restart, (s) skip, (k) keep, (p) preserve
+*  @o: overdue. character from (r) restart, (s) skip, (k) keep. Defaults to (k) keep.
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
 *  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
@@ -2041,20 +2041,20 @@
     # unreadable after the change.
 
     omit_extent:
     # A list of calendar names. Events with @c entries belonging to this
     # list will only have their starting times displayed in agenda view
     # and will neither appear nor cause conflicts in busy view.
 
-    keep_current: [0, 47]
+    keep_current: [0, 46]
     # A list of two, non-negative integers for "weeks" and "width". If
     # weeks is positive, the agenda for that integer number of weeks
     # starting with the current week will be written to "current.txt" in
     # your etm home directory and updated when necessary. The format will
-    # be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+    # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
     # in portrait mode. You could, for example, create a link to
     # "current.txt" in a pCloud or GoogleDrive folder and always have access
     # to your current agenda on your mobile device.
 
     keep_next: false
     # true or false. If true, the 'do next' view will be written to
     # "next.txt" in your etm home directory. As with "current.txt", a link
@@ -2338,23 +2338,22 @@
 		v: /usr/bin/say -v "Alex" "{summary}, {when}"
 
 
 [↺ contents](#contents)
 
 ### data storage {#data-storage}
 
-All *etm* reminders are stored in the text file `db.json` in your etm home directory using the wonderful *TinyDB* package. This *json* file is human readable but not easily editable. When you start *etm* for the first time, this file will have no entries:
+All *etm* reminders are stored in the text file `etm.json` in your etm home directory using the wonderful *TinyDB* package. [Prior to etm 5.0.0, the data storage file was named `db.json`. The format and name changed slightly with that version.] This *json* file is human readable but not easily editable. When you start *etm* for the first time, this file will have no entries:
 
 	{
 	"items": {},
 	"archive": {}
 	}
 
-Note that to *json* this is a hash/dictionary with two keys: "items" and "archive". Both have empty hashes/dictionaries as values.
-
+To *json* this is a hash/dictionary with two keys: "items" and "archive". Both have empty hashes/dictionaries as values.
 Add a first reminder to take out the trash on Mondays
 
 	- trash @s 2019-12-21 @r w &w mo
 
 at 10:26am on Dec 21, 2019 EST and the file would change to
 
 	{
```

### Comparing `etm-dgraham-5.0.7/README.md` & `etm-dgraham-5.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -896,15 +896,15 @@
 The recommended workflow for updating reminders is first
 to perfect the query to be certain that it lists just the
 items you want to update. Then press 'q' and the 'up'
 cursor key to restore the previous query, add ' | ' and
 the update command you want with its arguments.
 
 WARNING: Since the results may not be reversible, consider
-backing up your 'db.json' database before using update
+backing up your 'etm.json' database before using update
 commands. This simple query, e.g., would PERMANENTLY DELETE
 ALL YOUR REMINDERS:
 
     query exists itemtype | remove
 
 
 [↺ contents](#contents)
@@ -1115,15 +1115,15 @@
 
 [↺ contents](#contents)
 
 ## Mobile access to your reminders {#mobile}
 
 The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
 
-* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary.
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary. A width of 46, for example, works well for an iPhone in portrait mode.
 
 * `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
 
 By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
 
 Here is a screen shot from an iPhone of an illustrative `current.txt`:
 
@@ -1407,17 +1407,17 @@
 
 Whatever *home* directory you choose, running etm for the first time will add the following to that directory.
 
         etm home directory/
             backups/
             logs/
             cfg.yaml
-            db.json
+            etm.json
 
-Here `cfg.yaml` is your user configuration file and `db.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `db.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
+Here `cfg.yaml` is your user configuration file and `etm.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `etm.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
 
 The file `cfg.yaml` can be edited and the options are documented in the file.
 See [configuration](#configuration) for details.
 
 [↺ contents](#contents)
 
 ### Timers {#timers}
@@ -1560,15 +1560,15 @@
 
 - The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is scheduled to be completed.
     - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the scheduled time.
     - Tasks with `@s` date entry are regarded as past due after the due date and are displayed in *Agenda View* on the due date after all items with datetimes.
     - Tasks that are past due are also displayed in *Agenda View* on the current date using the type character `<` with an indication of the number of days that the task is past due.
 - Tasks without an `@s` entry are to be completed when possible and are sometimes called *todos*. They are regarded as *next* items in the *Getting Things Done* terminology and are displayed in *Do Next* view grouped by @l (location/context).
 - Tasks with an `@r` (repeat) or an `@+` entry can have an `@o` (overdue) setting.
-	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. This is the default when no `@o` entry is given.
+	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. The default when no `@o` entry is given is `@o k`.
 	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
 	- `@o s`: skip. Like 'keep' with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
 
 	    Furthermore, if the options setting `limit_skip_display` were true, then only the first instance of such a task would be displayed in agenda view. E.g., with the `limit_skip_display` setting true, then for the task
 
 			- meds @s +0d @r d &h 8,14,20 @o s
 
@@ -1735,15 +1735,15 @@
 *  @h: history. (for repeating tasks, a list of the most recent completion datetimes)
 *  @i: index. forward slash delimited string. E.g., client/project/activity
 *  @j*: job summary. string, optionally followed by job &key entries
 *  @k*: doc_id. connect this reminder to the one corresponding to doc_id.
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
-*  @o: overdue. character from (r) restart, (s) skip, (k) keep, (p) preserve
+*  @o: overdue. character from (r) restart, (s) skip, (k) keep. Defaults to (k) keep.
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
 *  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
@@ -2017,20 +2017,20 @@
     # unreadable after the change.
 
     omit_extent:
     # A list of calendar names. Events with @c entries belonging to this
     # list will only have their starting times displayed in agenda view
     # and will neither appear nor cause conflicts in busy view.
 
-    keep_current: [0, 47]
+    keep_current: [0, 46]
     # A list of two, non-negative integers for "weeks" and "width". If
     # weeks is positive, the agenda for that integer number of weeks
     # starting with the current week will be written to "current.txt" in
     # your etm home directory and updated when necessary. The format will
-    # be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+    # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
     # in portrait mode. You could, for example, create a link to
     # "current.txt" in a pCloud or GoogleDrive folder and always have access
     # to your current agenda on your mobile device.
 
     keep_next: false
     # true or false. If true, the 'do next' view will be written to
     # "next.txt" in your etm home directory. As with "current.txt", a link
@@ -2314,23 +2314,22 @@
 		v: /usr/bin/say -v "Alex" "{summary}, {when}"
 
 
 [↺ contents](#contents)
 
 ### data storage {#data-storage}
 
-All *etm* reminders are stored in the text file `db.json` in your etm home directory using the wonderful *TinyDB* package. This *json* file is human readable but not easily editable. When you start *etm* for the first time, this file will have no entries:
+All *etm* reminders are stored in the text file `etm.json` in your etm home directory using the wonderful *TinyDB* package. [Prior to etm 5.0.0, the data storage file was named `db.json`. The format and name changed slightly with that version.] This *json* file is human readable but not easily editable. When you start *etm* for the first time, this file will have no entries:
 
 	{
 	"items": {},
 	"archive": {}
 	}
 
-Note that to *json* this is a hash/dictionary with two keys: "items" and "archive". Both have empty hashes/dictionaries as values.
-
+To *json* this is a hash/dictionary with two keys: "items" and "archive". Both have empty hashes/dictionaries as values.
 Add a first reminder to take out the trash on Mondays
 
 	- trash @s 2019-12-21 @r w &w mo
 
 at 10:26am on Dec 21, 2019 EST and the file would change to
 
 	{
```

### Comparing `etm-dgraham-5.0.7/bump.py` & `etm-dgraham-5.0.8/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/docs/index_konnections.md` & `etm-dgraham-5.0.8/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/docs/index_usedtime.md` & `etm-dgraham-5.0.8/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/docs/multiple_timers.md` & `etm-dgraham-5.0.8/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etm/__main__.py` & `etm-dgraham-5.0.8/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etm/data.py` & `etm-dgraham-5.0.8/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etm/ical.py` & `etm-dgraham-5.0.8/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etm/make_examples.py` & `etm-dgraham-5.0.8/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etm/model.py` & `etm-dgraham-5.0.8/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,22 +74,35 @@
 DBARCH = None
 ETMDB = None
 data = None
 # NOTE: view.main() will override ampm using the configuration setting
 ampm = True
 logger = None
 
-def sortdt(dt):
-    # assumes dt is either a date or a datetime
-    try:
-        # this works if dt is a datetime
-        return dt.format("YYYYMMDDHHmm")
-    except:
-        # this works if dt is a date by providing 00 for HH and mm
-        return dt.format("YYYYMMDD0000")
+active_tasks = {}
+
+# def sortdt(dt):
+#     # assumes dt is either a date or a datetime
+#     if isinstance(dt, pendulum.Date):
+#         dt = date_to_datetime(dt)
+#     elif isinstance(dt, pendulum.Period):
+#         dt = dt.end
+#     try:
+#         # this works if dt is a datetime
+#         return dt.format("YYYYMMDDHHmm")
+#     except:
+#         # this works if dt is a date by providing 00 for HH and mm
+#         return dt.format("YYYYMMDD0000")
+
+def sortprd(prd, start=True):
+    # assumes prd is a pendulum.Period
+    if start:
+        return prd.start.format("YYYYMMDDHHmm")
+    else:
+        return prd.end.format("YYYYMMDDHHmm")
 
 
 
 PHONE_REGEX = re.compile(r'[0-9]{10}@.*')
 KONNECT_REGEX = re.compile(r'^.+:\s+(\d+)\s*$')
 
 # The style sheet for terminal output
@@ -783,14 +796,15 @@
         # deleting an @+ or adding an @- NOT changing @s!
 
         # What to do about history? Make history a hash with done keys and
         # lists of (done-due) or ZERO periods as values. Show competed on due
         # date with period.days in right hand column if 2nd component is not
         # ZERO. Why list of period values? done's resolution is one minute so
         # more than one completion might be attributed to the same minute.
+        global active_tasks
 
         save_item = False
         self.item_hsh = self.db.get(doc_id=item_id)
         self.doc_id = item_id
         self.created = self.item_hsh['created']
         completion_entry = pendulum.period(completed_datetime, due_datetime) if due_datetime else pendulum.period(completed_datetime, completed_datetime)
         if job_id:
@@ -812,14 +826,17 @@
                         if 'r' in self.item_hsh:
                             for i in range(len(self.item_hsh['r'])):
                                 if 'c' in self.item_hsh['r'][i] and self.item_hsh['r'][i]['c'] > 0:
                                     self.item_hsh['r'][i]['c'] -= 1
                                     break
                         self.item_hsh['s'] = nxt
                         self.item_hsh.setdefault('h', []).append(completion_entry)
+                        if self.doc_id in active_tasks:
+                            del active_tasks[self.doc_id]
+
                         save_item = True
                     else:  # finished last instance
                         self.item_hsh['f'] = completion_entry
                         save_item = True
 
         else:
             # no jobs
@@ -870,15 +887,15 @@
                 # only truncate completions for infinitely repeating tasks
                 for rr in self.item_hsh.get('r', {}):
                     if 'c' in rr or 'u' in rr:
                         # we have a count or an until: keep all completions
                         ok = False
                 if ok:
                     sh = self.item_hsh['h']
-                    sh.sort(key=sortdt)
+                    sh.sort(key=sortprd)
                     self.item_hsh['h'] = sh[-num_finished:]
 
             self.item_hsh['created'] = self.created
             self.item_hsh['modified'] = pendulum.now('local')
             # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
             self.do_update()
             return True
@@ -1575,14 +1592,16 @@
     >>> timestamp("13/16/16 2p")
     (False, 'invalid time-stamp: 13/16/16 2p')
     """
     if isinstance(arg, pendulum.DateTime):
         return True, arg
     elif isinstance(arg, pendulum.Date):
         return True, date_to_datetime(arg)
+    elif isinstance(arg, pendulum.Period):
+        return True, arg
     try:
         # res = parse(arg).strftime(ETMFMT)
         res = parse(arg)
     except:
         return False, 'invalid time-stamp: {}'.format(arg)
     return True, res
 
@@ -2198,14 +2217,18 @@
         self.used_details2id = {}
         self.effort_details = {}
         self.currMonth()
         self.completions = []
         self.konnections_from = {}
         self.konnections_to = {}
         self.konnected = []
+
+        # for repeating tasks with jobs - only one can be active
+        # self.active_tasks = [] # ids of repeating tasks with jobs
+
         if os.path.exists(timers_file):
             with open(timers_file, 'rb') as fn:
                 self.timers = pickle.load(fn)
             self.active_timer = None
             for x in self.timers:
                 if self.timers[x][0] == 'p':
                     self.active_timer = x
@@ -3767,15 +3790,15 @@
 {% endif %}\
 {% if 'h' in h and h['h'] %}
 @h {{ nowrap(prdlst2str(h['h'])) }} \
 {%- endif %}\
 {%- set ls = namespace(found=false) -%}\
 {%- set location -%}\
 {%- for k in ['l', 'm', 'g', 'x', 'p'] -%}\
-{%- if k in h %}@{{ k }} {{ h[k] }}{% set ls.found = true %} {% endif -%}\
+{%- if k in h %} @{{ k }} {{ h[k] }}{% set ls.found = true %} {% endif -%}\
 {%- endfor -%}\
 {%- endset -%}\
 {%- if ls.found -%}\
 {{ nowrap(location) }} \
 {% endif -%}\
 {%- if 'r' in h -%}\
 {%- for x in h['r'] -%}\
@@ -3874,15 +3897,15 @@
 {% endif %}\
 {% if 'h' in h and h['h'] %}
 @h {{ prdlst2str(h['h']) }} \
 {%- endif %}\
 {%- set ls = namespace(found=false) -%}\
 {%- set location -%}\
 {%- for k in ['l', 'm', 'g', 'x', 'p'] -%}\
-{%- if k in h %}@{{ k }} {{ h[k] }}{% set ls.found = true %} {% endif -%}\
+{%- if k in h %} @{{ k }} {{ h[k] }}{% set ls.found = true %} {% endif -%}\
 {%- endfor -%}\
 {%- endset -%}\
 {%- if ls.found -%}\
 {{ wrap(location) }} \
 {% endif -%}\
 {%- if 'r' in h -%}\
 {%- for x in h['r'] -%}\
@@ -4775,15 +4798,15 @@
     if not (
         isinstance(dtstart, pendulum.DateTime)
         or isinstance(dtstart, pendulum.Date)
     ):
         return []
     # This should not be necessary since the data store decodes dates as datetimes
     if isinstance(dtstart, pendulum.Date) and not isinstance(dtstart, pendulum.DateTime):
-        dtstart = pendulum.datetime(year=dtstart.year, month=dtstart.month, day=dtstart.day, hour=0, minute=0)
+        dtstart = pendulum.datetime(year=dtstart.year, month=dtstart.month, day=dtstart.day, hour=0, minute=0, tz='local')
         startdst = None
         using_dates = True
     else:
         using_dates = False
         # for discarding daylight saving time differences in repetitions
         try:
             startdst = dtstart.dst()
@@ -5527,14 +5550,15 @@
 
     wkday_fmt = "ddd D MMM" if settings['dayfirst'] else "ddd MMM D"
     dirty = False
     width = shutil.get_terminal_size()[0] - 3
     summary_width = width - 7 - 16
     ampm = settings['ampm']
     rhc_width = 15 if ampm else 11
+    num_remaining = ""
 
     today = pendulum.today()
     tomorrow = today + DAY
     inbox_fmt = today.format("YYYYMMDD    ")   # first
     pastdue_fmt = today.format("YYYYMMDD^^^^") # after all day and timed
     begby_fmt = today.format("YYYYMMDD~~~~")   # after past due
 
@@ -5665,19 +5689,21 @@
                     else: # k or p
                         relevant = rset.after(today, inc=True)
                         already_done = [x.end for x in item.get('h', [])]
                         # relevant will be the first instance after 12am today
                         # it will be the @s entry for the updated repeating item
                         # these are @s entries for the instances to be preserved
                         between = rset.between(dtstart, today-ONEMIN, inc=True)
-                        remaining = [x for x in between if x not in already_done]
+                        remaining = [x for x in between if x not in already_done and x != dtstart]
                         # once instances have been created, between will be empty until
                         # the current date falls after item['s'] and relevant is reset
-                        summary = f"{item['summary']} ({len(remaining)})"
-                        if dtstart.date() < today.date():
+                        num_remaining = f"({len(remaining)})" if remaining else ""
+                        sum_abbr = item['summary'][:summary_width]
+                        summary = f"{sum_abbr} {num_remaining}"
+                        if dtstart.date() < today.date() and 'j' not in item:
                             pastdue.append([(dtstart.date() - today.date()).days, summary, item.doc_id, None, None])
                 else:
                     # get the first instance after today
                     try:
                         relevant = rset.after(today, inc=True)
                     except Exception as e:
                         logger.error(f"error processing {item}; {repr(e)}")
@@ -5759,32 +5785,33 @@
         if 'j' in item and 'f' not in item:
             # jobs only for the relevant instance of unfinished tasks
             for job in item['j']:
                 job_id = job.get('i')
                 if 'f' in job:
                     continue
                 # adjust job starting time if 's' in job
-                job_summary = job.get('summary', '')
-                jobstart = relevant - job.get('s', ZERO)
-                if jobstart.date() < today.date():
+                job_summary = f"{job.get('summary', '')[:summary_width]} {num_remaining}"
+                jobstart = dtstart - job.get('s', ZERO)
+                if jobstart.date() < today.date() and job.get('status', None) == '-':
                     pastdue_jobs = True
                     pastdue.append([(jobstart.date() - today.date()).days, job_summary, item.doc_id, job_id, None])
                 if 'b' in job:
                     days = int(job['b']) * DAY
                     if today + DAY <= jobstart <= tomorrow + days:
                         beginbys.append([(jobstart.date() - today.date()).days, job_summary, item.doc_id, job_id, None])
                 if 'a' in job:
                     for alert in job['a']:
                         for td in alert[0]:
                             if today <= jobstart - td <= tomorrow:
                                 alerts.append([dtstart - td, dtstart, alert[1], '-', job['summary'], item.doc_id, job_id, None])
 
         id2relevant[item.doc_id] = relevant
 
-        if item['itemtype'] == '-' and 'f' not in item and not pastdue_jobs and relevant.date() < today.date():
+        # if item['itemtype'] == '-' and 'f' not in item and relevant.date() < today.date():
+        if item['itemtype'] == '-' and 'f' not in item and 'j' not in item and relevant.date() < today.date():
             pastdue.append([(relevant.date() - today.date()).days, summary, item.doc_id, None, None])
 
     inbox.sort()
     pastdue.sort()
     beginbys.sort()
     alerts.sort()
     # alerts: alert datetime, start datetime, commands, summary, doc_id
@@ -5797,17 +5824,18 @@
         flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         current.append({'id': item[2], 'job': None, 'instance': None, 'sort': (inbox_fmt, 1), 'week': week, 'day': day, 'columns': ['!', item[1], flags, rhc, doc_id]})
 
     for item in pastdue:
         item_0 = str(item[0]) if item[0] in item else ""
         rhc = item_0.center(rhc_width, ' ')
         doc_id = item[2]
+        job_id = item[3] if item[3] else ""
         flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         try:
-            current.append({'id': item[2], 'job': item[3], 'instance': item[4], 'sort': (pastdue_fmt, 2, item[0]), 'week': week, 'day': day, 'columns': ['<', item[1], flags, rhc, doc_id]})
+            current.append({'id': item[2], 'job': item[3], 'instance': item[4], 'sort': (pastdue_fmt, 2, item[0]), 'week': week, 'day': day, 'columns': ['<', item[1], flags, rhc, (doc_id, item[4], item[3])]})
         except Exception as e:
             logger.warning(f"could not append item: {item}; e: {e}")
 
     for item in beginbys:
         if item[0] in item:
             item_0 = str(item[0]) if item[0] <= 0 else f"+{item[0]}"
         else:
@@ -6680,15 +6708,15 @@
 
 def wkday2row(wkday):
     # week day number in 1, ..., 7 to row number in busy view
     # 1 -> 5, ..., 6 -> 15, 0 -> 17  (pendulum thinks Sunday is first)
     return 3+ 2*wkday if wkday else 17
 
 def schedule(db, yw=getWeekNum(), current=[], now=pendulum.now(), weeks_before=0, weeks_after=0, pinned_list=[], link_list=[], konnect_list=[], timers={}):
-    global current_hsh
+    global current_hsh, active_tasks
     wkday_fmt = "ddd D MMM" if settings['dayfirst'] else "ddd MMM D"
     timer_schedule = TimeIt('***SCHEDULE***')
     #
 
     width = shutil.get_terminal_size()[0]-3
     compact = False
     weeks_after = settings['keep_current'][0]
@@ -6759,14 +6787,18 @@
     busy_details = {}
     week2day2busy = {}
     week2day2allday = {}
 
     #XXX main loop begins
     todayYMD = now.format("YYYYMMDD")
     tomorrowYMD = (now + 1*DAY).format("YYYYMMDD")
+
+    # Only display one active instance of a repeating task with jobs
+    repeating_with_jobs_ids = []
+
     for item in db:
         if item.get('itemtype', None) == None:
             logger.error(f"itemtype missing from {item}")
             continue
         if item['itemtype'] in "!?":
             continue
 
@@ -6853,16 +6885,17 @@
                     if 'f' in job:
                         # FIXME
                         d.append([job['f'].start, job_summary, doc_id, job['i']])
             if d:
                 for row in d:
                     dt = row[0]
                     if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
-                        dt = pendulum.parse(dt.format("YYYYMMDD"), tz='local')
-                        dt.set(hour=23, minute=59, second=59)
+                        # dt = pendulum.parse(dt.format("YYYYMMDD"), tz='local')
+                        dt = pendulum.datetime(dt.year, dt.month, dt.day, tz='local')
+                        # dt.set(hour=23, minute=59, second=59)
 
                     rhc = str(row[3]) if len(row) > 3 else ""
                     if dt < aft_dt or dt > bef_dt:
                         continue
 
                     done.append(
                             {
@@ -6917,16 +6950,30 @@
                 tmp_summary = set_summary(item['summary'], item['s'], dt, freq)
                 week2day2allday[week][dayofweek][1].append(f"{item['itemtype']} {tmp_summary}")
 
             if 'r' in item:
                 freq = item['r'][0].get('r', 'y')
             else:
                 freq = 'y'
+
             instance = dt if '+' in item or 'r' in item else None
+
             if 'j' in item:
+
+                # repeating task with jobs
+
+                if instance:
+                    if doc_id in active_tasks and active_tasks[doc_id] != instance:
+                            continue
+
+
+                    else:
+                        active_tasks[doc_id] = instance
+
+
                 for job in item['j']:
                     if 'f' in job:
                         continue
                     job_summary = job.get('summary', '')
                     jobstart = dt - job.get('s', ZERO)
                     job_id = job.get('i', None)
                     job_sort = str(job_id)
```

### Comparing `etm-dgraham-5.0.7/etm/options.py` & `etm-dgraham-5.0.8/etm/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     dayfirst = "false"
     beginbusy = 7
     updates_interval = 0
     locale = "en_US"
     vi_mode = "false"
     secret = randomString(10)
     omit_extent = ""
-    keep_current = [0, 47]
+    keep_current = [0, 46]
     keep_next = "false"
     archive_after = 0
     refresh_interval = 60
     num_finished = 0
     limit_skip_display = "true"
     connecting_dots = "false"
     usedtime_minutes = 1
@@ -295,15 +295,15 @@
 # and will neither appear nor cause conflicts in busy view.
 
 keep_current: {keep_current}
 # A list of two, non-negative integers for "weeks" and "width". If
 # weeks is positive, the agenda for that integer number of weeks
 # starting with the current week will be written to "current.txt" in
 # your etm home directory and updated when necessary. The format will
-# be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+# be scaled to fit "width". A width of 46, e.g, fits an iPhone display
 # in portrait mode. You could, for example, create a link to
 # "current.txt" in a pCloud or GoogleDrive folder and always have access
 # to your current agenda on your mobile device.
 
 keep_next: {keep_next}
 # true or false. If true, the 'do next' view will be written to
 # "next.txt" in your etm home directory. As with "current.txt", a link
@@ -725,22 +725,24 @@
                 new['window_colors'] = tmp
 
             if new['window_colors']:
                 self.settings_hsh['window_colors'] = dict2yaml(new['window_colors'])
                 self.settings['window_colors'].update(new['window_colors'])
 
         if 'keep_current' in new and not isinstance(new['keep_current'], list):
+            weeks, width = self.settings['keep_current']
             if isinstance(new['keep_current'], int):
                 weeks = new['keep_current']
-            elif isinstance(new['keep_current'], bool):
-                weeks = 3 if new['keep_current'] else 0
+            elif isinstance(new['keep_current'], bool) and not new['keep_current']:
+                weeks = 0
             else:
                 weeks = 0
-            changed.append(f"Converting 'keep_current' from {new['keep_current']} to [{weeks}, 50]")
-            new['keep_current'] = [weeks, 50]
+            # use default width
+            changed.append(f"Converting 'keep_current' from {new['keep_current']} to [{weeks}, {width}]")
+            new['keep_current'] = [weeks, width]
 
         if not locale_regex.match(new['locale']):
             tmp = new['locale']
             new['locale'] = self.settings['locale']
             changed.append(f"retaining default for 'locale': {self.settings['locale']}. The provided setting, {tmp}, does have the required format.")
```

### Comparing `etm-dgraham-5.0.7/etm/report.py` & `etm-dgraham-5.0.8/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etm/view.py` & `etm-dgraham-5.0.8/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1389,15 +1389,14 @@
 
     if bad:
         logger.error(f"unrecognized alert commands: {bad}")
 
 
 async def event_handler():
     global current_datetime
-    logger.debug(f"current_datetime: {current_datetime}")
     # check for updates every interval minutes
     interval = settings.get('updates_interval', 0)
     refresh_interval = settings.get('refresh_interval', 60)
     minutes = 0
     try:
         while True:
             now = pendulum.now('local')
@@ -1499,29 +1498,27 @@
         active_part = inactive_part = ('class:status', "")
 
     return [ active_part, inactive_part,  ('class:status',  f"{dataview.active_view} {inbasket}{update_status.get_status()}"), ]
 
 def openWithDefault(path):
     if " " in path:
         parts = qsplit(path)
-        logger.debug(f"path: {path}\n    Popen args: {parts}")
         if parts:
             # wrapper to catch 'Exception Ignored' messages
             output = io.StringIO()
             with contextlib.redirect_stderr(output):
                 # the pid business is evidently needed to avoid waiting
                 pid = subprocess.Popen(parts, stdin=subprocess.DEVNULL, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL).pid
                 res = output.getvalue()
                 if res:
                     logger.error(f"caught by contextlib:\n'{res}'")
 
 
     else:
         path = os.path.normpath(os.path.expanduser(path))
-        logger.debug(f"path: {path}")
         sys_platform = platform.system()
         if platform.system() == 'Darwin':       # macOS
             subprocess.run(('open', path), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         elif platform.system() == 'Windows':    # Windows
             os.startfile(path)
         else:                                   # linux
             subprocess.run(('xdg-open', path), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
@@ -2138,32 +2135,31 @@
 @bindings.add('F', filter=is_viewing_or_details & is_item_view)
 def do_finish(*event):
 
     doc_id, instance, job = dataview.get_row_details(text_area.document.cursor_position_row)
     if not doc_id:
         return
 
-    logger.debug(f"doc_id: {doc_id}; instance: {instance}; job: {job}")
-
     hsh = DBITEM.get(doc_id=doc_id)
     has_timer = doc_id in dataview.timers
     timer_warning = " and\nits associated timer" if has_timer else ""
     repeating = 'r' in hsh or '+' in hsh
 
     between = []
     due = ""
 
     title = "Finish"
-    if instance:
+    if instance and instance != model.date_to_datetime(hsh['s']):
         need = 2
         between = [hsh['s'], instance]
-        values = [
-            f"{format_datetime(hsh['s'])[1]} (oldest)",
-            f"{format_datetime(instance)[1]} (selected)",
-            ]
+        if instance != hsh['s']:
+            values = [
+                f"{format_datetime(hsh['s'])[1]} (oldest)",
+                f"{format_datetime(instance)[1]} (selected)",
+                ]
 
         values_list = []
         count = -1
         for x in values:
             count += 1
             values_list.append(f"    {count}: {x}")
 
@@ -2178,19 +2174,18 @@
 the completion datetime to use?
 number : datetime\
         """
         entry = "1 : now"
         due = ""
 
 
-    elif repeating:
+    elif repeating and between:
         already_done = [x.end for x in hsh.get('h', [])]
         need = 2
         between = [x[0] for x in model.item_instances(hsh, model.date_to_datetime(hsh['s']), pendulum.now().replace(hour=0, minute=0, second=0, microsecond=0)) if x[0] not in already_done]
-        logger.debug(f"between: {between}")
         values_list = []
         # values.append( (0, format_datetime(between[0][0])[1]) )
         count = -1
         for x in between:
             count += 1
             values_list.append(f"   {count}: {format_datetime(x)[1]}")
```

### Comparing `etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.7
+Version: 5.0.8
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -920,15 +920,15 @@
 The recommended workflow for updating reminders is first
 to perfect the query to be certain that it lists just the
 items you want to update. Then press 'q' and the 'up'
 cursor key to restore the previous query, add ' | ' and
 the update command you want with its arguments.
 
 WARNING: Since the results may not be reversible, consider
-backing up your 'db.json' database before using update
+backing up your 'etm.json' database before using update
 commands. This simple query, e.g., would PERMANENTLY DELETE
 ALL YOUR REMINDERS:
 
     query exists itemtype | remove
 
 
 [↺ contents](#contents)
@@ -1139,15 +1139,15 @@
 
 [↺ contents](#contents)
 
 ## Mobile access to your reminders {#mobile}
 
 The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
 
-* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary.
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary. A width of 46, for example, works well for an iPhone in portrait mode.
 
 * `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
 
 By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
 
 Here is a screen shot from an iPhone of an illustrative `current.txt`:
 
@@ -1431,17 +1431,17 @@
 
 Whatever *home* directory you choose, running etm for the first time will add the following to that directory.
 
         etm home directory/
             backups/
             logs/
             cfg.yaml
-            db.json
+            etm.json
 
-Here `cfg.yaml` is your user configuration file and `db.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `db.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
+Here `cfg.yaml` is your user configuration file and `etm.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `etm.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
 
 The file `cfg.yaml` can be edited and the options are documented in the file.
 See [configuration](#configuration) for details.
 
 [↺ contents](#contents)
 
 ### Timers {#timers}
@@ -1584,15 +1584,15 @@
 
 - The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is scheduled to be completed.
     - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the scheduled time.
     - Tasks with `@s` date entry are regarded as past due after the due date and are displayed in *Agenda View* on the due date after all items with datetimes.
     - Tasks that are past due are also displayed in *Agenda View* on the current date using the type character `<` with an indication of the number of days that the task is past due.
 - Tasks without an `@s` entry are to be completed when possible and are sometimes called *todos*. They are regarded as *next* items in the *Getting Things Done* terminology and are displayed in *Do Next* view grouped by @l (location/context).
 - Tasks with an `@r` (repeat) or an `@+` entry can have an `@o` (overdue) setting.
-	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. This is the default when no `@o` entry is given.
+	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. The default when no `@o` entry is given is `@o k`.
 	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
 	- `@o s`: skip. Like 'keep' with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
 
 	    Furthermore, if the options setting `limit_skip_display` were true, then only the first instance of such a task would be displayed in agenda view. E.g., with the `limit_skip_display` setting true, then for the task
 
 			- meds @s +0d @r d &h 8,14,20 @o s
 
@@ -1759,15 +1759,15 @@
 *  @h: history. (for repeating tasks, a list of the most recent completion datetimes)
 *  @i: index. forward slash delimited string. E.g., client/project/activity
 *  @j*: job summary. string, optionally followed by job &key entries
 *  @k*: doc_id. connect this reminder to the one corresponding to doc_id.
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
-*  @o: overdue. character from (r) restart, (s) skip, (k) keep, (p) preserve
+*  @o: overdue. character from (r) restart, (s) skip, (k) keep. Defaults to (k) keep.
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
 *  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
@@ -2041,20 +2041,20 @@
     # unreadable after the change.
 
     omit_extent:
     # A list of calendar names. Events with @c entries belonging to this
     # list will only have their starting times displayed in agenda view
     # and will neither appear nor cause conflicts in busy view.
 
-    keep_current: [0, 47]
+    keep_current: [0, 46]
     # A list of two, non-negative integers for "weeks" and "width". If
     # weeks is positive, the agenda for that integer number of weeks
     # starting with the current week will be written to "current.txt" in
     # your etm home directory and updated when necessary. The format will
-    # be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+    # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
     # in portrait mode. You could, for example, create a link to
     # "current.txt" in a pCloud or GoogleDrive folder and always have access
     # to your current agenda on your mobile device.
 
     keep_next: false
     # true or false. If true, the 'do next' view will be written to
     # "next.txt" in your etm home directory. As with "current.txt", a link
@@ -2338,23 +2338,22 @@
 		v: /usr/bin/say -v "Alex" "{summary}, {when}"
 
 
 [↺ contents](#contents)
 
 ### data storage {#data-storage}
 
-All *etm* reminders are stored in the text file `db.json` in your etm home directory using the wonderful *TinyDB* package. This *json* file is human readable but not easily editable. When you start *etm* for the first time, this file will have no entries:
+All *etm* reminders are stored in the text file `etm.json` in your etm home directory using the wonderful *TinyDB* package. [Prior to etm 5.0.0, the data storage file was named `db.json`. The format and name changed slightly with that version.] This *json* file is human readable but not easily editable. When you start *etm* for the first time, this file will have no entries:
 
 	{
 	"items": {},
 	"archive": {}
 	}
 
-Note that to *json* this is a hash/dictionary with two keys: "items" and "archive". Both have empty hashes/dictionaries as values.
-
+To *json* this is a hash/dictionary with two keys: "items" and "archive". Both have empty hashes/dictionaries as values.
 Add a first reminder to take out the trash on Mondays
 
 	- trash @s 2019-12-21 @r w &w mo
 
 at 10:26am on Dec 21, 2019 EST and the file would change to
 
 	{
```

### Comparing `etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.0.8/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etmlogo.png` & `etm-dgraham-5.0.8/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etmlogo_small.png` & `etm-dgraham-5.0.8/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/etmview_agenda.png` & `etm-dgraham-5.0.8/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/namedcolors.py` & `etm-dgraham-5.0.8/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/new.png` & `etm-dgraham-5.0.8/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/setup.py` & `etm-dgraham-5.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/test/test_parser.py` & `etm-dgraham-5.0.8/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/utilities/colons_to_slashes.py` & `etm-dgraham-5.0.8/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/utilities/etm_in` & `etm-dgraham-5.0.8/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/utilities/inbasket` & `etm-dgraham-5.0.8/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.7/utilities/open_in_mutt` & `etm-dgraham-5.0.8/utilities/open_in_mutt`

 * *Files identical despite different names*

