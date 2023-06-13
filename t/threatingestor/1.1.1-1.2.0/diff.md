# Comparing `tmp/threatingestor-1.1.1.tar.gz` & `tmp/threatingestor-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threatingestor-1.1.1.tar", last modified: Fri May 19 13:52:08 2023, max compression
+gzip compressed data, was "threatingestor-1.2.0.tar", last modified: Tue Jun 13 23:49:49 2023, max compression
```

## Comparing `threatingestor-1.1.1.tar` & `threatingestor-1.2.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-05-19 13:52:08.307836 threatingestor-1.1.1/
--rw-r--r--   0 azazel     (501) staff       (20)    18046 2023-04-26 13:26:17.000000 threatingestor-1.1.1/LICENSE
--rw-r--r--   0 azazel     (501) staff       (20)       92 2023-04-26 13:27:18.000000 threatingestor-1.1.1/MANIFEST.in
--rw-r--r--   0 azazel     (501) staff       (20)     8311 2023-05-19 13:52:08.307587 threatingestor-1.1.1/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)     7320 2023-04-26 13:27:18.000000 threatingestor-1.1.1/README.md
--rw-r--r--   0 azazel     (501) staff       (20)      184 2023-04-26 13:26:17.000000 threatingestor-1.1.1/requirements-testing.txt
--rw-r--r--   0 azazel     (501) staff       (20)      144 2023-04-26 13:41:52.000000 threatingestor-1.1.1/requirements.txt
--rw-r--r--   0 azazel     (501) staff       (20)       38 2023-05-19 13:52:08.307876 threatingestor-1.1.1/setup.cfg
--rw-r--r--   0 azazel     (501) staff       (20)     2082 2023-05-19 13:52:04.000000 threatingestor-1.1.1/setup.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-05-19 13:52:08.302070 threatingestor-1.1.1/tests/
--rw-r--r--   0 azazel     (501) staff       (20)    18861 2023-05-11 15:27:40.000000 threatingestor-1.1.1/tests/test_artifacts.py
--rw-r--r--   0 azazel     (501) staff       (20)     8942 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_config.py
--rw-r--r--   0 azazel     (501) staff       (20)     2468 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_ingestor.py
--rw-r--r--   0 azazel     (501) staff       (20)     7191 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators.py
--rw-r--r--   0 azazel     (501) staff       (20)     4234 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_abstract_json.py
--rw-r--r--   0 azazel     (501) staff       (20)      562 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     1069 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_csv.py
--rw-r--r--   0 azazel     (501) staff       (20)     4728 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_misp.py
--rw-r--r--   0 azazel     (501) staff       (20)     1397 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_mysql.py
--rw-r--r--   0 azazel     (501) staff       (20)     3486 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_sqlite.py
--rw-r--r--   0 azazel     (501) staff       (20)     4051 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     2112 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_threatkb.py
--rw-r--r--   0 azazel     (501) staff       (20)     3465 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_operators_twitter.py
--rw-r--r--   0 azazel     (501) staff       (20)     6991 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources.py
--rw-r--r--   0 azazel     (501) staff       (20)      834 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources_beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     3899 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources_git.py
--rw-r--r--   0 azazel     (501) staff       (20)     3283 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources_github.py
--rw-r--r--   0 azazel     (501) staff       (20)     2118 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources_json.py
--rw-r--r--   0 azazel     (501) staff       (20)      893 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources_sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     6382 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources_twitter.py
--rw-r--r--   0 azazel     (501) staff       (20)     2653 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_sources_web.py
--rw-r--r--   0 azazel     (501) staff       (20)     1089 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_state.py
--rw-r--r--   0 azazel     (501) staff       (20)      459 2023-04-26 13:26:17.000000 threatingestor-1.1.1/tests/test_whitelist.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-05-19 13:52:08.302764 threatingestor-1.1.1/threatingestor/
--rw-r--r--   0 azazel     (501) staff       (20)     6885 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)    10377 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/artifacts.py
--rw-r--r--   0 azazel     (501) staff       (20)     5490 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/config.py
--rw-r--r--   0 azazel     (501) staff       (20)      221 2023-04-26 13:26:17.000000 threatingestor-1.1.1/threatingestor/exceptions.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-05-19 13:52:08.304100 threatingestor-1.1.1/threatingestor/extras/
--rw-r--r--   0 azazel     (501) staff       (20)        0 2023-04-26 13:26:17.000000 threatingestor-1.1.1/threatingestor/extras/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)     1227 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/extras/fswatcher.py
--rw-r--r--   0 azazel     (501) staff       (20)     1116 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/extras/pasteprocessor.py
--rw-r--r--   0 azazel     (501) staff       (20)     4918 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/extras/queueworker.py
--rw-r--r--   0 azazel     (501) staff       (20)     2899 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/extras/webapp.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-05-19 13:52:08.305229 threatingestor-1.1.1/threatingestor/operators/
--rw-r--r--   0 azazel     (501) staff       (20)     2846 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)      929 2023-04-26 13:26:17.000000 threatingestor-1.1.1/threatingestor/operators/abstract_json.py
--rw-r--r--   0 azazel     (501) staff       (20)     1129 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     1076 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/csv.py
--rw-r--r--   0 azazel     (501) staff       (20)     4881 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/misp.py
--rw-r--r--   0 azazel     (501) staff       (20)     3584 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/mysql.py
--rw-r--r--   0 azazel     (501) staff       (20)     2296 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/sqlite.py
--rw-r--r--   0 azazel     (501) staff       (20)     1390 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     3278 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/threatkb.py
--rw-r--r--   0 azazel     (501) staff       (20)     2078 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/operators/twitter.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-05-19 13:52:08.307391 threatingestor-1.1.1/threatingestor/sources/
--rw-r--r--   0 azazel     (501) staff       (20)     6931 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)     1654 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/abstract_json.py
--rw-r--r--   0 azazel     (501) staff       (20)     1303 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/beanstalk.py
--rw-r--r--   0 azazel     (501) staff       (20)     3646 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/git.py
--rw-r--r--   0 azazel     (501) staff       (20)     2235 2023-04-26 13:26:17.000000 threatingestor-1.1.1/threatingestor/sources/github.py
--rw-r--r--   0 azazel     (501) staff       (20)     1634 2023-04-26 13:26:17.000000 threatingestor-1.1.1/threatingestor/sources/github_gist.py
--rw-r--r--   0 azazel     (501) staff       (20)     2775 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/image.py
--rw-r--r--   0 azazel     (501) staff       (20)     3441 2023-05-18 16:29:09.000000 threatingestor-1.1.1/threatingestor/sources/rss.py
--rw-r--r--   0 azazel     (501) staff       (20)     2927 2023-05-18 15:04:20.000000 threatingestor-1.1.1/threatingestor/sources/sitemap.py
--rw-r--r--   0 azazel     (501) staff       (20)     1133 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/sqs.py
--rw-r--r--   0 azazel     (501) staff       (20)     6447 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/twitter.py
--rw-r--r--   0 azazel     (501) staff       (20)     4249 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/twitter_follow_links.py
--rw-r--r--   0 azazel     (501) staff       (20)     1442 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/sources/web.py
--rw-r--r--   0 azazel     (501) staff       (20)     1252 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/state.py
--rw-r--r--   0 azazel     (501) staff       (20)      848 2023-04-26 13:27:18.000000 threatingestor-1.1.1/threatingestor/whitelist.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-05-19 13:52:08.303458 threatingestor-1.1.1/threatingestor.egg-info/
--rw-r--r--   0 azazel     (501) staff       (20)     8311 2023-05-19 13:52:08.000000 threatingestor-1.1.1/threatingestor.egg-info/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)     2091 2023-05-19 13:52:08.000000 threatingestor-1.1.1/threatingestor.egg-info/SOURCES.txt
--rw-r--r--   0 azazel     (501) staff       (20)        1 2023-05-19 13:52:08.000000 threatingestor-1.1.1/threatingestor.egg-info/dependency_links.txt
--rw-r--r--   0 azazel     (501) staff       (20)       55 2023-05-19 13:52:08.000000 threatingestor-1.1.1/threatingestor.egg-info/entry_points.txt
--rw-r--r--   0 azazel     (501) staff       (20)      503 2023-05-19 13:52:08.000000 threatingestor-1.1.1/threatingestor.egg-info/requires.txt
--rw-r--r--   0 azazel     (501) staff       (20)       15 2023-05-19 13:52:08.000000 threatingestor-1.1.1/threatingestor.egg-info/top_level.txt
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-13 23:49:49.180675 threatingestor-1.2.0/
+-rw-r--r--   0 azazel     (501) staff       (20)    18046 2023-04-26 13:26:17.000000 threatingestor-1.2.0/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)       92 2023-04-26 13:27:18.000000 threatingestor-1.2.0/MANIFEST.in
+-rw-r--r--   0 azazel     (501) staff       (20)     8932 2023-06-13 23:49:49.180471 threatingestor-1.2.0/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     7942 2023-06-13 23:47:30.000000 threatingestor-1.2.0/README.md
+-rw-r--r--   0 azazel     (501) staff       (20)      184 2023-04-26 13:26:17.000000 threatingestor-1.2.0/requirements-testing.txt
+-rw-r--r--   0 azazel     (501) staff       (20)      144 2023-06-07 19:31:24.000000 threatingestor-1.2.0/requirements.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2023-06-13 23:49:49.180720 threatingestor-1.2.0/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     2082 2023-06-13 23:49:31.000000 threatingestor-1.2.0/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-13 23:49:49.175360 threatingestor-1.2.0/tests/
+-rw-r--r--   0 azazel     (501) staff       (20)    18861 2023-06-02 05:27:17.000000 threatingestor-1.2.0/tests/test_artifacts.py
+-rw-r--r--   0 azazel     (501) staff       (20)     8942 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_config.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2468 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_ingestor.py
+-rw-r--r--   0 azazel     (501) staff       (20)     7191 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4234 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_abstract_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)      562 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1069 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_csv.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4728 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_misp.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1397 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_mysql.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3486 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_sqlite.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4051 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2112 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_threatkb.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3465 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_operators_twitter.py
+-rw-r--r--   0 azazel     (501) staff       (20)     6991 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_sources.py
+-rw-r--r--   0 azazel     (501) staff       (20)      834 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_sources_beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3899 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_sources_git.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3283 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_sources_github.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2118 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_sources_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)      893 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_sources_sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     6382 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_sources_twitter.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2659 2023-06-13 23:47:30.000000 threatingestor-1.2.0/tests/test_sources_web.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1089 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_state.py
+-rw-r--r--   0 azazel     (501) staff       (20)      459 2023-04-26 13:26:17.000000 threatingestor-1.2.0/tests/test_whitelist.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-13 23:49:49.176277 threatingestor-1.2.0/threatingestor/
+-rw-r--r--   0 azazel     (501) staff       (20)     6885 2023-06-12 18:39:12.000000 threatingestor-1.2.0/threatingestor/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)    10377 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/artifacts.py
+-rw-r--r--   0 azazel     (501) staff       (20)     5490 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/config.py
+-rw-r--r--   0 azazel     (501) staff       (20)      221 2023-04-26 13:26:17.000000 threatingestor-1.2.0/threatingestor/exceptions.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-13 23:49:49.177606 threatingestor-1.2.0/threatingestor/extras/
+-rw-r--r--   0 azazel     (501) staff       (20)        0 2023-04-26 13:26:17.000000 threatingestor-1.2.0/threatingestor/extras/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1227 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/extras/fswatcher.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1116 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/extras/pasteprocessor.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4918 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/extras/queueworker.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2899 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/extras/webapp.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-13 23:49:49.178694 threatingestor-1.2.0/threatingestor/operators/
+-rw-r--r--   0 azazel     (501) staff       (20)     2846 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)      929 2023-04-26 13:26:17.000000 threatingestor-1.2.0/threatingestor/operators/abstract_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1129 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1076 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/csv.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4881 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/misp.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3584 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/mysql.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2296 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/sqlite.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1390 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3278 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/threatkb.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2078 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/operators/twitter.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-13 23:49:49.180262 threatingestor-1.2.0/threatingestor/sources/
+-rw-r--r--   0 azazel     (501) staff       (20)     6931 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1654 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/abstract_json.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1303 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/sources/beanstalk.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3646 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/git.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2235 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/github.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1634 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/github_gist.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2775 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/image.py
+-rw-r--r--   0 azazel     (501) staff       (20)     3441 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/rss.py
+-rw-r--r--   0 azazel     (501) staff       (20)     2483 2023-06-13 23:47:30.000000 threatingestor-1.2.0/threatingestor/sources/sitemap.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1133 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/sources/sqs.py
+-rw-r--r--   0 azazel     (501) staff       (20)     6447 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/twitter.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4249 2023-06-12 19:30:09.000000 threatingestor-1.2.0/threatingestor/sources/twitter_follow_links.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1135 2023-06-13 23:47:30.000000 threatingestor-1.2.0/threatingestor/sources/virustotal.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1682 2023-06-13 23:47:30.000000 threatingestor-1.2.0/threatingestor/sources/web.py
+-rw-r--r--   0 azazel     (501) staff       (20)     1252 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/state.py
+-rw-r--r--   0 azazel     (501) staff       (20)      848 2023-04-26 13:27:18.000000 threatingestor-1.2.0/threatingestor/whitelist.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-13 23:49:49.177074 threatingestor-1.2.0/threatingestor.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     8932 2023-06-13 23:49:49.000000 threatingestor-1.2.0/threatingestor.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     2128 2023-06-13 23:49:49.000000 threatingestor-1.2.0/threatingestor.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2023-06-13 23:49:49.000000 threatingestor-1.2.0/threatingestor.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       55 2023-06-13 23:49:49.000000 threatingestor-1.2.0/threatingestor.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)      503 2023-06-13 23:49:49.000000 threatingestor-1.2.0/threatingestor.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       15 2023-06-13 23:49:49.000000 threatingestor-1.2.0/threatingestor.egg-info/top_level.txt
```

### Comparing `threatingestor-1.1.1/LICENSE` & `threatingestor-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/PKG-INFO` & `threatingestor-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threatingestor
-Version: 1.1.1
+Version: 1.2.0
 Summary: Extract and aggregate IOCs from threat feeds.
 Home-page: https://github.com/InQuest/ThreatIngestor
 Author: InQuest Labs
 Author-email: labs@inquest.net
 License: GPL
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -175,7 +175,15 @@
 FROM ubuntu:18.04
 ...
 # RUN apt-get install tesseract-ocr -y
 ...
 # RUN pip3 install opencv-python pytesseract numpy
 ...
 ```
+
+### Extra Scripts
+
+Some scripts are now provided to help with your local configuration of ThreatIngestor.
+
+| Script                | Description                                                                                                 | Example                          |
+|-----------------------|-------------------------------------------------------------------------------------------------------------|----------------------------------|
+| `scripts/validate.py` | This script validates your YAML syntax and checks that you have the bare minimum required by ThreatIngestor | `python3 validate.py config.yml` |
```

### Comparing `threatingestor-1.1.1/README.md` & `threatingestor-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -144,8 +144,16 @@
 ```
 FROM ubuntu:18.04
 ...
 # RUN apt-get install tesseract-ocr -y
 ...
 # RUN pip3 install opencv-python pytesseract numpy
 ...
-```
+```
+
+### Extra Scripts
+
+Some scripts are now provided to help with your local configuration of ThreatIngestor.
+
+| Script                | Description                                                                                                 | Example                          |
+|-----------------------|-------------------------------------------------------------------------------------------------------------|----------------------------------|
+| `scripts/validate.py` | This script validates your YAML syntax and checks that you have the bare minimum required by ThreatIngestor | `python3 validate.py config.yml` |
```

### Comparing `threatingestor-1.1.1/setup.py` & `threatingestor-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 if not isinstance(extra_requires, list):
     print("requirements-testing.txt was not parsed correctly.")
     extra_requires = []
 
 
 setup(
     name='threatingestor',
-    version='1.1.1',
+    version='1.2.0',
     include_package_data=True,
     install_requires=requires,
     extras_require={
         'twitter': ['twitter'],
         'rss': ['feedparser'],
         'misp': ['PyMISP'],
         'threatkb': ['threatkb'],
```

### Comparing `threatingestor-1.1.1/tests/test_artifacts.py` & `threatingestor-1.2.0/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_config.py` & `threatingestor-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_ingestor.py` & `threatingestor-1.2.0/tests/test_ingestor.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators.py` & `threatingestor-1.2.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_abstract_json.py` & `threatingestor-1.2.0/tests/test_operators_abstract_json.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_beanstalk.py` & `threatingestor-1.2.0/tests/test_operators_beanstalk.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_csv.py` & `threatingestor-1.2.0/tests/test_operators_csv.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_misp.py` & `threatingestor-1.2.0/tests/test_operators_misp.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_mysql.py` & `threatingestor-1.2.0/tests/test_operators_mysql.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_sqlite.py` & `threatingestor-1.2.0/tests/test_operators_sqlite.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_sqs.py` & `threatingestor-1.2.0/tests/test_operators_sqs.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_threatkb.py` & `threatingestor-1.2.0/tests/test_operators_threatkb.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_operators_twitter.py` & `threatingestor-1.2.0/tests/test_operators_twitter.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources.py` & `threatingestor-1.2.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources_beanstalk.py` & `threatingestor-1.2.0/tests/test_sources_beanstalk.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources_git.py` & `threatingestor-1.2.0/tests/test_sources_git.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources_github.py` & `threatingestor-1.2.0/tests/test_sources_github.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources_json.py` & `threatingestor-1.2.0/tests/test_sources_json.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources_sqs.py` & `threatingestor-1.2.0/tests/test_sources_sqs.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources_twitter.py` & `threatingestor-1.2.0/tests/test_sources_twitter.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/tests/test_sources_web.py` & `threatingestor-1.2.0/tests/test_sources_web.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import unittest
-
 import httpretty
 
 import threatingestor.sources.web
 
-
 class TestWeb(unittest.TestCase):
 
     def setUp(self):
         self.web = threatingestor.sources.web.Plugin('myweb', 'http://example.mock/list.txt')
 
     @httpretty.activate
     def test_run_with_200(self):
@@ -18,15 +16,15 @@
                 adding_headers={
                     'Last-Modified': 'test',
                     'Etag': '"test"'
                 })
 
         saved_state, artifacts = self.web.run(None)
         self.assertIn('http://example.com/test', [str(x) for x in artifacts])
-        self.assertEqual(saved_state, 'test;"test"')
+        self.assertEqual(saved_state, 'test;"test";200')
 
     @httpretty.activate
     def test_run_with_304(self):
         httpretty.register_uri(httpretty.HEAD, "http://example.mock/list.txt",
                                status=304)
 
         saved_state, artifacts = self.web.run('test;"test"')
@@ -52,15 +50,15 @@
                 body='http://example.com/test',
                 adding_headers={
                     'Etag': '"test"'
                 })
 
         saved_state, artifacts = self.web.run(None)
         self.assertIn('http://example.com/test', [str(x) for x in artifacts])
-        self.assertEqual(saved_state, 'None;"test"')
+        self.assertEqual(saved_state, 'None;"test";200')
 
     @httpretty.activate
     def test_run_with_200_and_no_state_headers(self):
         httpretty.register_uri(httpretty.HEAD, "http://example.mock/list.txt")
         httpretty.register_uri(httpretty.GET, "http://example.mock/list.txt",
                 body='http://example.com/test')
```

### Comparing `threatingestor-1.1.1/tests/test_state.py` & `threatingestor-1.2.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/__init__.py` & `threatingestor-1.2.0/threatingestor/__init__.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/artifacts.py` & `threatingestor-1.2.0/threatingestor/artifacts.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/config.py` & `threatingestor-1.2.0/threatingestor/config.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/extras/fswatcher.py` & `threatingestor-1.2.0/threatingestor/extras/fswatcher.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/extras/pasteprocessor.py` & `threatingestor-1.2.0/threatingestor/extras/pasteprocessor.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/extras/queueworker.py` & `threatingestor-1.2.0/threatingestor/extras/queueworker.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/extras/webapp.py` & `threatingestor-1.2.0/threatingestor/extras/webapp.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/__init__.py` & `threatingestor-1.2.0/threatingestor/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/abstract_json.py` & `threatingestor-1.2.0/threatingestor/operators/abstract_json.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/beanstalk.py` & `threatingestor-1.2.0/threatingestor/operators/beanstalk.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/csv.py` & `threatingestor-1.2.0/threatingestor/operators/csv.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/misp.py` & `threatingestor-1.2.0/threatingestor/operators/misp.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/mysql.py` & `threatingestor-1.2.0/threatingestor/operators/mysql.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/sqlite.py` & `threatingestor-1.2.0/threatingestor/operators/sqlite.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/sqs.py` & `threatingestor-1.2.0/threatingestor/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/threatkb.py` & `threatingestor-1.2.0/threatingestor/operators/threatkb.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/operators/twitter.py` & `threatingestor-1.2.0/threatingestor/operators/twitter.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/__init__.py` & `threatingestor-1.2.0/threatingestor/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/abstract_json.py` & `threatingestor-1.2.0/threatingestor/sources/abstract_json.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/beanstalk.py` & `threatingestor-1.2.0/threatingestor/sources/beanstalk.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/git.py` & `threatingestor-1.2.0/threatingestor/sources/git.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/github.py` & `threatingestor-1.2.0/threatingestor/sources/github.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/github_gist.py` & `threatingestor-1.2.0/threatingestor/sources/github_gist.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/image.py` & `threatingestor-1.2.0/threatingestor/sources/image.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/rss.py` & `threatingestor-1.2.0/threatingestor/sources/rss.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/sqs.py` & `threatingestor-1.2.0/threatingestor/sources/sqs.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/twitter.py` & `threatingestor-1.2.0/threatingestor/sources/twitter.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/twitter_follow_links.py` & `threatingestor-1.2.0/threatingestor/sources/twitter_follow_links.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/sources/web.py` & `threatingestor-1.2.0/threatingestor/sources/web.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,41 +8,46 @@
         self.name = name
         self.url = url
 
 
     def run(self, saved_state):
         # Read saved state and set HTTP headers.
         headers = {}
+        
         if saved_state:
             # If both last modified and etag, set both.
             # Otherwise just interpret the whole field as last modified.
             last_modified = saved_state
 
             if len(saved_state.split(';')) == 2:
                 last_modified, etag = saved_state.split(';')
                 headers['If-None-Match'] = etag
 
             headers['If-Modified-Since'] = last_modified
+        
+        if not saved_state:
+            saved_state = ""
 
         # Send head first to check 304.
         response = requests.head(self.url, headers=headers)
 
-        # If not modified, return immediately.
-        if response.status_code == 304:
+        # If not modified, return immediately
+        if "304" in saved_state or response.status_code == 304:
+            saved_state = ';'.join([str(response.headers.get('Last-Modified')), 'N/A', str(response.status_code)])
             return saved_state, []
 
         # Otherwise, do the full request.
         response = requests.get(self.url, headers=headers)
 
         # Form saved state.
         last_modified = response.headers.get('Last-Modified')
         etag = response.headers.get('Etag')
 
         if etag:
-            saved_state = ';'.join([str(last_modified), etag])
+            saved_state = ';'.join([str(last_modified), etag, str(response.status_code)])
         else:
             saved_state = last_modified
 
         # Process text.
         artifact_list = self.process_element(response.text, self.url, include_nonobfuscated=True)
 
         return saved_state, artifact_list
```

### Comparing `threatingestor-1.1.1/threatingestor/state.py` & `threatingestor-1.2.0/threatingestor/state.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor/whitelist.py` & `threatingestor-1.2.0/threatingestor/whitelist.py`

 * *Files identical despite different names*

### Comparing `threatingestor-1.1.1/threatingestor.egg-info/PKG-INFO` & `threatingestor-1.2.0/threatingestor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threatingestor
-Version: 1.1.1
+Version: 1.2.0
 Summary: Extract and aggregate IOCs from threat feeds.
 Home-page: https://github.com/InQuest/ThreatIngestor
 Author: InQuest Labs
 Author-email: labs@inquest.net
 License: GPL
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -175,7 +175,15 @@
 FROM ubuntu:18.04
 ...
 # RUN apt-get install tesseract-ocr -y
 ...
 # RUN pip3 install opencv-python pytesseract numpy
 ...
 ```
+
+### Extra Scripts
+
+Some scripts are now provided to help with your local configuration of ThreatIngestor.
+
+| Script                | Description                                                                                                 | Example                          |
+|-----------------------|-------------------------------------------------------------------------------------------------------------|----------------------------------|
+| `scripts/validate.py` | This script validates your YAML syntax and checks that you have the bare minimum required by ThreatIngestor | `python3 validate.py config.yml` |
```

### Comparing `threatingestor-1.1.1/threatingestor.egg-info/SOURCES.txt` & `threatingestor-1.2.0/threatingestor.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -62,8 +62,9 @@
 threatingestor/sources/github_gist.py
 threatingestor/sources/image.py
 threatingestor/sources/rss.py
 threatingestor/sources/sitemap.py
 threatingestor/sources/sqs.py
 threatingestor/sources/twitter.py
 threatingestor/sources/twitter_follow_links.py
+threatingestor/sources/virustotal.py
 threatingestor/sources/web.py
```

