# Comparing `tmp/genocide-90.tar.gz` & `tmp/genocide-91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genocide-90.tar", last modified: Tue Dec 13 11:55:51 2022, max compression
+gzip compressed data, was "genocide-91.tar", last modified: Wed Jan  4 08:35:39 2023, max compression
```

## Comparing `genocide-90.tar` & `genocide-91.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.161976 genocide-90/
--rw-r--r--   0 bart      (1000) bart      (1000)     2756 2022-12-13 11:55:51.161976 genocide-90/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1854 2022-12-13 09:26:23.000000 genocide-90/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.149976 genocide-90/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     3043 2022-12-13 09:26:23.000000 genocide-90/bin/genocide
--rwxr-xr-x   0 bart      (1000) bart      (1000)      868 2022-12-13 09:26:23.000000 genocide-90/bin/genocidecmd
--rwxr-xr-x   0 bart      (1000) bart      (1000)      226 2022-12-13 09:26:23.000000 genocide-90/bin/genocidectl
--rwxr-xr-x   0 bart      (1000) bart      (1000)      420 2022-12-13 09:26:23.000000 genocide-90/bin/genocided
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.157976 genocide-90/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)   180711 2022-12-13 09:26:23.000000 genocide-90/docs/ECHAabilify.png
--rw-r--r--   0 bart      (1000) bart      (1000)   193757 2022-12-13 09:26:23.000000 genocide-90/docs/ECHAclozapine.png
--rw-r--r--   0 bart      (1000) bart      (1000)   197697 2022-12-13 09:26:23.000000 genocide-90/docs/ECHAhaldol.png
--rw-r--r--   0 bart      (1000) bart      (1000)   232313 2022-12-13 09:26:23.000000 genocide-90/docs/ECHAzyprexa.png
--rw-r--r--   0 bart      (1000) bart      (1000)   245670 2022-12-13 09:26:23.000000 genocide-90/docs/OTP1.png
--rw-r--r--   0 bart      (1000) bart      (1000)   238095 2022-12-13 09:26:23.000000 genocide-90/docs/OTP2.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.157976 genocide-90/docs/_static/
--rw-r--r--   0 bart      (1000) bart      (1000)      785 2022-12-13 09:26:23.000000 genocide-90/docs/_static/genocide.css
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.157976 genocide-90/docs/_templates/
--rw-r--r--   0 bart      (1000) bart      (1000)      309 2022-12-13 09:26:23.000000 genocide-90/docs/_templates/base.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      543 2022-12-13 09:26:23.000000 genocide-90/docs/_templates/class.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      849 2022-12-13 09:26:23.000000 genocide-90/docs/_templates/module.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1295 2022-12-13 09:26:23.000000 genocide-90/docs/about.rst
--rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2022-12-13 09:26:23.000000 genocide-90/docs/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     3107 2022-12-13 09:26:23.000000 genocide-90/docs/conf.py
--rw-r--r--   0 bart      (1000) bart      (1000)   192133 2022-12-13 09:26:23.000000 genocide-90/docs/elverbatim.png
--rw-r--r--   0 bart      (1000) bart      (1000)      660 2022-12-13 09:26:23.000000 genocide-90/docs/evidence.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    47740 2022-12-13 09:26:23.000000 genocide-90/docs/genocide.png
--rw-r--r--   0 bart      (1000) bart      (1000)    21988 2022-12-13 09:26:23.000000 genocide-90/docs/genocide3.png
--rw-r--r--   0 bart      (1000) bart      (1000)      474 2022-12-13 09:26:23.000000 genocide-90/docs/guilty.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1460 2022-12-13 09:26:23.000000 genocide-90/docs/index.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    69979 2022-12-13 09:26:23.000000 genocide-90/docs/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   228393 2022-12-13 09:26:23.000000 genocide-90/docs/kamer.png
--rw-r--r--   0 bart      (1000) bart      (1000)     3015 2022-12-13 09:39:28.000000 genocide-90/docs/manual.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.157976 genocide-90/docs/pdf/
--rw-r--r--   0 bart      (1000) bart      (1000)   238330 2022-12-13 09:26:23.000000 genocide-90/docs/pdf/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   236671 2022-12-13 09:26:23.000000 genocide-90/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   257079 2022-12-13 09:26:23.000000 genocide-90/docs/pdf/Elements-of-Crimes.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    41559 2022-12-13 09:26:23.000000 genocide-90/docs/pdf/Kamer.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   323490 2022-12-13 09:26:23.000000 genocide-90/docs/pdf/Rome-Statute.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   571580 2022-12-13 09:26:23.000000 genocide-90/docs/pdf/Rules-of-Procedure-and-Evidence.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    50044 2022-12-13 09:26:23.000000 genocide-90/docs/pdf/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)     2121 2022-12-13 09:26:23.000000 genocide-90/docs/reconsider.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2290 2022-12-13 09:26:23.000000 genocide-90/docs/request.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      162 2022-12-13 09:26:23.000000 genocide-90/docs/requirements.txt
--rw-r--r--   0 bart      (1000) bart      (1000)   179869 2022-12-13 09:26:23.000000 genocide-90/docs/skull.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   125074 2022-12-13 09:26:23.000000 genocide-90/docs/skullagain.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   139659 2022-12-13 09:26:23.000000 genocide-90/docs/skullnr.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   144090 2022-12-13 09:26:23.000000 genocide-90/docs/skullnr2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      506 2022-12-13 09:26:23.000000 genocide-90/docs/source.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   234877 2022-12-13 09:26:23.000000 genocide-90/docs/verbatim2.png
--rw-r--r--   0 bart      (1000) bart      (1000)    71457 2022-12-13 09:26:23.000000 genocide-90/docs/whitetxt4.png
--rw-r--r--   0 bart      (1000) bart      (1000)     1138 2022-12-13 09:26:23.000000 genocide-90/docs/writings.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.157976 genocide-90/files/
--rw-r--r--   0 bart      (1000) bart      (1000)      368 2022-12-13 09:26:23.000000 genocide-90/files/genocide.service
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.161976 genocide-90/genocide/
--rw-r--r--   0 bart      (1000) bart      (1000)     2144 2022-12-13 09:26:23.000000 genocide-90/genocide/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2654 2022-12-13 09:26:23.000000 genocide-90/genocide/cmds.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6790 2022-12-13 09:26:23.000000 genocide-90/genocide/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)    18751 2022-12-13 09:26:23.000000 genocide-90/genocide/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17719 2022-12-13 09:26:23.000000 genocide-90/genocide/model.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11380 2022-12-13 09:26:23.000000 genocide-90/genocide/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2393 2022-12-13 09:27:55.000000 genocide-90/genocide/request.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7393 2022-12-13 09:26:23.000000 genocide-90/genocide/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)      152 2022-12-13 09:26:23.000000 genocide-90/genocide/run.py
--rw-r--r--   0 bart      (1000) bart      (1000)      215 2022-12-13 09:26:23.000000 genocide-90/genocide/slogan.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2812 2022-12-13 09:26:23.000000 genocide-90/genocide/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1791 2022-12-13 09:26:23.000000 genocide-90/genocide/util.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.161976 genocide-90/genocide.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2756 2022-12-13 11:55:51.000000 genocide-90/genocide.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1499 2022-12-13 11:55:51.000000 genocide-90/genocide.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2022-12-13 11:55:51.000000 genocide-90/genocide.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        9 2022-12-13 11:55:51.000000 genocide-90/genocide.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2022-12-13 11:55:51.000000 genocide-90/genocide.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2022-12-13 11:55:51.161976 genocide-90/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)     1651 2022-12-13 09:41:31.000000 genocide-90/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2022-12-13 11:55:51.161976 genocide-90/test/
--rw-r--r--   0 bart      (1000) bart      (1000)      915 2022-12-13 09:26:23.000000 genocide-90/test/test_bus.py
--rw-r--r--   0 bart      (1000) bart      (1000)      266 2022-12-13 09:26:23.000000 genocide-90/test/test_dbs.py
--rw-r--r--   0 bart      (1000) bart      (1000)      274 2022-12-13 09:26:23.000000 genocide-90/test/test_evt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      284 2022-12-13 09:26:23.000000 genocide-90/test/test_hdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      249 2022-12-13 09:26:23.000000 genocide-90/test/test_irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      299 2022-12-13 09:26:23.000000 genocide-90/test/test_mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5792 2022-12-13 09:26:23.000000 genocide-90/test/test_obj.py
--rw-r--r--   0 bart      (1000) bart      (1000)      277 2022-12-13 09:26:23.000000 genocide-90/test/test_rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)      309 2022-12-13 09:26:23.000000 genocide-90/test/test_thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)      307 2022-12-13 09:26:23.000000 genocide-90/test/test_tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1382 2022-12-13 09:26:23.000000 genocide-90/test/test_zcmd.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.220839 genocide-91/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2756 2023-01-04 08:35:39.220839 genocide-91/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1854 2022-12-28 13:01:52.000000 genocide-91/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.208839 genocide-91/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     4842 2023-01-03 18:22:07.000000 genocide-91/bin/genocide
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     1778 2023-01-03 21:06:27.000000 genocide-91/bin/genocidecmd
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      226 2023-01-01 15:12:39.000000 genocide-91/bin/genocidectl
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      436 2023-01-03 18:24:56.000000 genocide-91/bin/genocided
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.216839 genocide-91/docs/
+-rw-r--r--   0 bart      (1000) bart      (1000)   180711 2022-12-28 13:01:52.000000 genocide-91/docs/ECHAabilify.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   193757 2022-12-28 13:01:52.000000 genocide-91/docs/ECHAclozapine.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   197697 2022-12-28 13:01:52.000000 genocide-91/docs/ECHAhaldol.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   232313 2022-12-28 13:01:52.000000 genocide-91/docs/ECHAzyprexa.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   245670 2022-12-28 13:01:52.000000 genocide-91/docs/OTP1.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   238095 2022-12-28 13:01:52.000000 genocide-91/docs/OTP2.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.216839 genocide-91/docs/_static/
+-rw-r--r--   0 bart      (1000) bart      (1000)      785 2022-12-28 13:01:52.000000 genocide-91/docs/_static/genocide.css
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.216839 genocide-91/docs/_templates/
+-rw-r--r--   0 bart      (1000) bart      (1000)      309 2022-12-28 13:01:52.000000 genocide-91/docs/_templates/base.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      543 2022-12-28 13:01:52.000000 genocide-91/docs/_templates/class.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      896 2023-01-03 20:17:27.000000 genocide-91/docs/_templates/module.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1287 2023-01-02 00:14:34.000000 genocide-91/docs/about.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2022-12-28 13:01:52.000000 genocide-91/docs/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)     3208 2023-01-03 18:45:58.000000 genocide-91/docs/conf.py
+-rw-r--r--   0 bart      (1000) bart      (1000)   192133 2022-12-28 13:01:52.000000 genocide-91/docs/elverbatim.png
+-rw-r--r--   0 bart      (1000) bart      (1000)      533 2023-01-02 01:57:31.000000 genocide-91/docs/evidence.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    47740 2022-12-28 13:01:52.000000 genocide-91/docs/genocide.png
+-rw-r--r--   0 bart      (1000) bart      (1000)    21988 2022-12-28 13:01:52.000000 genocide-91/docs/genocide3.png
+-rw-r--r--   0 bart      (1000) bart      (1000)      388 2023-01-03 18:53:38.000000 genocide-91/docs/guilty.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2069 2023-01-03 18:47:07.000000 genocide-91/docs/index.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    69979 2022-12-28 13:01:52.000000 genocide-91/docs/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   228393 2022-12-28 13:01:52.000000 genocide-91/docs/kamer.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     2900 2023-01-03 18:53:19.000000 genocide-91/docs/manual.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.216839 genocide-91/docs/pdf/
+-rw-r--r--   0 bart      (1000) bart      (1000)   238330 2022-12-28 13:01:52.000000 genocide-91/docs/pdf/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   236671 2022-12-28 13:01:52.000000 genocide-91/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   257079 2022-12-28 13:01:52.000000 genocide-91/docs/pdf/Elements-of-Crimes.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    41559 2022-12-28 13:01:52.000000 genocide-91/docs/pdf/Kamer.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   323490 2022-12-28 13:01:52.000000 genocide-91/docs/pdf/Rome-Statute.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   571580 2022-12-28 13:01:52.000000 genocide-91/docs/pdf/Rules-of-Procedure-and-Evidence.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    50044 2022-12-28 13:01:52.000000 genocide-91/docs/pdf/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)     2026 2023-01-03 18:53:26.000000 genocide-91/docs/reconsider.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2302 2023-01-01 16:15:30.000000 genocide-91/docs/request.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   179869 2022-12-28 13:01:52.000000 genocide-91/docs/skull.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   125074 2022-12-28 13:01:52.000000 genocide-91/docs/skullagain.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   139659 2022-12-28 13:01:52.000000 genocide-91/docs/skullnr.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   144090 2022-12-28 13:01:52.000000 genocide-91/docs/skullnr2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      808 2023-01-03 18:47:55.000000 genocide-91/docs/source.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   234877 2022-12-28 13:01:52.000000 genocide-91/docs/verbatim2.png
+-rw-r--r--   0 bart      (1000) bart      (1000)    71457 2022-12-28 13:01:52.000000 genocide-91/docs/whitetxt4.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     1047 2023-01-03 18:53:46.000000 genocide-91/docs/writings.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.216839 genocide-91/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)      344 2023-01-03 20:43:34.000000 genocide-91/files/genocide.service
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.216839 genocide-91/genocide/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1741 2023-01-03 18:36:49.000000 genocide-91/genocide/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3374 2023-01-01 15:11:29.000000 genocide-91/genocide/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2776 2023-01-01 15:11:29.000000 genocide-91/genocide/message.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.220839 genocide-91/genocide/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      149 2023-01-03 19:37:52.000000 genocide-91/genocide/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      253 2023-01-03 19:44:53.000000 genocide-91/genocide/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16407 2023-01-03 18:19:13.000000 genocide-91/genocide/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1074 2023-01-03 19:46:07.000000 genocide-91/genocide/modules/krn.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17670 2023-01-03 19:45:17.000000 genocide-91/genocide/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2429 2023-01-03 19:42:41.000000 genocide-91/genocide/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7313 2023-01-02 12:26:41.000000 genocide-91/genocide/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1519 2023-01-03 16:04:40.000000 genocide-91/genocide/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1635 2023-01-01 16:42:13.000000 genocide-91/genocide/modules/usr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    13147 2023-01-03 19:44:11.000000 genocide-91/genocide/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2181 2023-01-02 13:35:02.000000 genocide-91/genocide/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3840 2023-01-01 15:11:29.000000 genocide-91/genocide/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1599 2023-01-03 19:44:24.000000 genocide-91/genocide/usersdb.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.216839 genocide-91/genocide.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2756 2023-01-04 08:35:39.000000 genocide-91/genocide.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1586 2023-01-04 08:35:39.000000 genocide-91/genocide.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-01-04 08:35:39.000000 genocide-91/genocide.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        9 2023-01-04 08:35:39.000000 genocide-91/genocide.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-01-04 08:35:39.000000 genocide-91/genocide.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-01-04 08:35:39.220839 genocide-91/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)     1665 2023-01-03 19:48:52.000000 genocide-91/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-04 08:35:39.220839 genocide-91/test/
+-rw-r--r--   0 bart      (1000) bart      (1000)      915 2022-12-28 13:01:52.000000 genocide-91/test/test_bus.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      267 2023-01-01 16:19:37.000000 genocide-91/test/test_dbs.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      274 2023-01-02 14:04:43.000000 genocide-91/test/test_evt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      284 2022-12-28 13:01:52.000000 genocide-91/test/test_hdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      257 2023-01-03 18:37:57.000000 genocide-91/test/test_irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5797 2023-01-01 16:21:35.000000 genocide-91/test/test_obj.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      285 2023-01-03 18:38:09.000000 genocide-91/test/test_rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      310 2023-01-01 16:22:16.000000 genocide-91/test/test_thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      308 2023-01-01 16:22:25.000000 genocide-91/test/test_tmr.py
```

### Comparing `genocide-90/PKG-INFO` & `genocide-91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genocide
-Version: 90
+Version: 91
 Summary: @KarimKhanQC reconsider OTP-CR-117/19
 Home-page: https://github.com/bthate/genocide
 Author: Bart Thate
 Author-email: bthate67@gmail.com
 License: Public Domain
 Description: | **Information and Evidence Unit**
         | **Office of the Prosecutor**
```

### Comparing `genocide-90/README.rst` & `genocide-91/README.rst`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/ECHAabilify.png` & `genocide-91/docs/ECHAabilify.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/ECHAclozapine.png` & `genocide-91/docs/ECHAclozapine.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/ECHAhaldol.png` & `genocide-91/docs/ECHAhaldol.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/ECHAzyprexa.png` & `genocide-91/docs/ECHAzyprexa.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/OTP1.png` & `genocide-91/docs/OTP1.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/OTP2.png` & `genocide-91/docs/OTP2.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/_static/genocide.css` & `genocide-91/docs/_static/genocide.css`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/_templates/class.rst` & `genocide-91/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/_templates/module.rst` & `genocide-91/docs/_templates/module.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .. _{{ fullname }}:
 
-.. raw:: html
-
-    <br><br>
-    <center><b>
-
-
 .. title:: {{ fullname }}
 
+.. raw:: html
+
+    <center>
+    <h3>
+    <b>
 
-**{{ fullname }}**
+{{ fullname }} 
 
 .. raw:: html
 
     </b>
+    </h3>
     </center>
     <br>
 
 .. automodule:: {{ fullname }}
     :members:
 
     {% block exceptions %}
@@ -27,15 +27,14 @@
     .. autosummary::
     {% for item in exceptions %}
         {{ item }}
     {%- endfor %}
     {% endif %}
     {% endblock %}
 
-
     {% block classes %}
     {% if classes %}
     .. rubric:: classes
 
     .. autosummary:: 
     {% for item in classes %}
         {{ item }}
@@ -52,9 +51,10 @@
         {{ item }}
     {%- endfor %}
     {% endif %}
     {% endblock %}
 
     .. raw:: html
 
-       <br><br>
+       <br><br><br><br>
 
+.. currentmodule:: {{ fullname }}
```

### Comparing `genocide-90/docs/about.rst` & `genocide-91/docs/about.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 .. _about:
 
 .. raw:: html
 
-     <br><br>
+    <br>
 
 .. title:: About
 
 
 .. image:: skullagain.jpg
     :width: 100%
     :target: manual.html
 
-
 .. raw:: html
 
+     <center>
+     <i>By law, with the use of poison, killing, torturing, castrating, destroying, in whole or in part, all elderly and all handicapped (Wzd), all criminals (Wfz) and all psychiatric patients (WvGGZ) here in the Netherlands.</i>
      </center>
      <br>
-     <center><i>By law, with the use of poison, killing, torturing, castrating, destroying, in whole or in part, all elderly and all handicapped (Wzd), all criminals (Wfz) and all psychiatric patients (WvGGZ) here in the Netherlands.</i></center>
-     <br>
-
 
-In 2018 i informed the king of the netherlands that what he calls medicine in his "care" laws are not medicine but poison. Proof of these medicine being poison were shown to the king, who's (personal) kabinet wrote back that "the king took note of what i have written".
+In 2018 i :ref:`informed <informed>` the king of the netherlands that what he calls medicine in his "care" laws are not medicine but poison. Proof of these medicine being poison were shown to the king, who's (personal) kabinet wrote back that "the king took note of what i have written".
 
 Using poison makes the care laws used in the netherlands to provide care to elderly and handicapped, criminals and psychiatric patients not care laws but genocide laws with which the king is killing groups of the population by giving them poison instead of medicine in the "care" they are forced to undergo.
 
-I :ref:`wrote <writings>` the prosecutor asking for an arrest of the king (make him stop), the prosecutor decided to call it a "no basis to proceed". It requires a :ref:`basis to prosecute <reconsider>` of the prosecutor to get the king in his cell and his genocide, thereby, stopped.
+I :ref:`wrote <writings>` the prosecutor asking for an arrest of the king (make him stop), the prosecutor decided to call it a "no basis to proceed". It requires a :ref:`basis to prosecute <home>` of the prosecutor to get the king in his cell and his genocide, thereby, stopped.
```

### Comparing `genocide-90/docs/bevestigd.jpg` & `genocide-91/docs/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/conf.py` & `genocide-91/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# GENOCIDE OTP-CR-117/19
+# GCID OTP-CR-117/19
 # -*- coding: utf-8 -*-
 #
 
 
-"@KarimKhanQC reconsider OTP-CR-117/19 - http://pypi.org/project/genocide"
+"Reconsider OTP-CR-117/19"
 
 
 __name__ = "genocide"
-__version__ = "89"
+__version__ = "91"
 
 
 import doctest
 import os
 import sys
 import unittest
 
 
 curdir = os.getcwd()
 
 
-sys.path.insert(0, os.path.join(curdir))
-sys.path.insert(0, os.path.join(curdir, ".."))
 sys.path.insert(0, os.path.join(curdir, "..", ".."))
+sys.path.insert(0, os.path.join(curdir, ".."))
+sys.path.insert(0, os.path.join(curdir))
 
 
 # -- Options for GENERIC output ---------------------------------------------
 
 
 project = __name__
 master_doc = 'index'
 version = '%s' % __version__
 release = '%s' % __version__
-language = ''
+language = 'en'
 today = ''
 today_fmt = '%B %d, %Y'
 needs_sphinx='1.7'
 exclude_patterns = ['_build', '_templates', '_source', 'Thumbs.db', '.DS_Store']
 source_suffix = '.rst'
 source_encoding = 'utf-8-sig'
 modindex_common_prefix = [""]
@@ -54,15 +54,15 @@
     'sphinx.ext.githubpages'
 ]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 
-html_title = '@KarimKhanQC reconsider OTP-CR-117/19 - http://pypi.org/project/genocide'
+html_title = "Reconsider OTP-CR-117/19"
 html_style = 'genocide.css'
 html_static_path = ["_static"]
 html_css_files = ["genocide.css",]
 html_short_title = "GENOCIDE %s" % __version__
 html_sidebars = {
     '**': [
         'about.html',
@@ -79,15 +79,15 @@
     'github_banner': False,
     'logo': 'skull.jpg',
     'link': '#000',
     'link_hover': '#000',
     'nosidebar': True,
     'show_powered_by': False,
     'show_relbar_top': False,
-    'sidebar_width': 0,
+    'sidebar_width': 10,
 }
 html_favicon = "skull.jpg"
 html_extra_path = []
 html_last_updated_fmt = '%Y-%b-%d'
 html_additional_pages = {}
 html_domain_indices = False
 html_use_index = True
@@ -102,20 +102,34 @@
 
 intersphinx_mapping = {
                        'python': ('https://docs.python.org/3', 'objects.inv'),
                        'sphinx': ('http://sphinx.pocoo.org/', None),
                       }
 intersphinx_cache_limit=1
 
+
 rst_prolog = '''.. image:: genocide.png
     :width: 100%
     :height: 2.2cm
     :target: index.html
+
 '''
+rst_epilog = '''.. raw:: html
+
+    <br>
+    <center>
+    <b>
+
+:ref:`home <home>` - :ref:`manual <manual>` - :ref:`source <source>` - :ref:`about <about>`
 
+.. raw:: html
+
+    </b>
+    </center>
+'''
 autosummary_generate=True
 autodoc_default_flags=['members', 'undoc-members', 'private-members', "imported-members"]
 autodoc_member_order='groupwise'
 autodoc_docstring_signature=True
 autoclass_content="class"
 doctest_global_setup=""
 doctest_global_cleanup=""
```

### Comparing `genocide-90/docs/elverbatim.png` & `genocide-91/docs/elverbatim.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/evidence.rst` & `genocide-91/docs/evidence.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,16 @@
 .. _evidence:
 
-.. raw:: html
-
-     <br><br>
-
 .. title:: Evidence
 
+.. _haldol:
 
 .. raw:: html
 
-
-    <center>
-    <b>
-    E V I D E N C E
-    </b>
-    </center>
-    <br>
-
-
-.. _haldol:
-
+  <br>
 
 **haldol**
 
 
 .. raw:: html
 
   <br>
@@ -80,11 +67,7 @@
 .. raw:: html
 
   <br>
 
 .. image:: ECHAabilify.png
      :width: 100%
 
-.. raw:: html
-
-  <br><br>
-
```

### Comparing `genocide-90/docs/genocide.png` & `genocide-91/docs/genocide.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/genocide3.png` & `genocide-91/docs/genocide3.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/index.rst` & `genocide-91/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,130 @@
 00000000: 2e2e 205f 686f 6d65 3a0a 0a2e 2e20 7261  .. _home:.... ra
-00000010: 773a 3a20 6874 6d6c 0a0a 2020 2020 3c62  w:: html..    <b
-00000020: 723e 0a0a 2e2e 2074 6974 6c65 3a3a 204f  r>.... title:: O
-00000030: 5450 2d43 522d 3131 372f 3139 0a0a 0a2e  TP-CR-117/19....
-00000040: 2e20 696d 6167 653a 3a20 736b 756c 6c61  . image:: skulla
-00000050: 6761 696e 2e6a 7067 0a20 2020 203a 7769  gain.jpg.    :wi
-00000060: 6474 683a 2031 3030 250a 2020 2020 3a74  dth: 100%.    :t
-00000070: 6172 6765 743a 206d 616e 7561 6c2e 6874  arget: manual.ht
-00000080: 6d6c 0a0a 0a2e 2e20 7261 773a 3a20 6874  ml..... raw:: ht
-00000090: 6d6c 0a0a 2020 2020 203c 6365 6e74 6572  ml..     <center
-000000a0: 3e3c 693e 4279 206c 6177 2c20 7769 7468  ><i>By law, with
-000000b0: 2074 6865 2075 7365 206f 6620 706f 6973   the use of pois
-000000c0: 6f6e 2c20 6b69 6c6c 696e 672c 2074 6f72  on, killing, tor
-000000d0: 7475 7269 6e67 2c20 6361 7374 7261 7469  turing, castrati
-000000e0: 6e67 2c20 6465 7374 726f 7969 6e67 2c20  ng, destroying, 
-000000f0: 696e 2077 686f 6c65 206f 7220 696e 2070  in whole or in p
-00000100: 6172 742c 2061 6c6c 2065 6c64 6572 6c79  art, all elderly
-00000110: 2061 6e64 2061 6c6c 2068 616e 6469 6361   and all handica
-00000120: 7070 6564 2028 577a 6429 2c20 616c 6c20  pped (Wzd), all 
-00000130: 6372 696d 696e 616c 7320 2857 667a 2920  criminals (Wfz) 
-00000140: 616e 6420 616c 6c20 7073 7963 6869 6174  and all psychiat
-00000150: 7269 6320 7061 7469 656e 7473 2028 5776  ric patients (Wv
-00000160: 4747 5a29 2068 6572 6520 696e 2074 6865  GGZ) here in the
-00000170: 204e 6574 6865 726c 616e 6473 2e3c 2f69   Netherlands.</i
-00000180: 3e3c 2f63 656e 7465 723e 0a20 2020 2020  ></center>.     
-00000190: 3c62 723e 0a0a 0a49 6e20 3230 3138 2069  <br>...In 2018 i
-000001a0: 203a 7265 663a 6069 6e66 6f72 6d65 6420   :ref:`informed 
-000001b0: 3c69 6e66 6f72 6d65 643e 6020 7468 6520  <informed>` the 
-000001c0: 6b69 6e67 206f 6620 7468 6520 6e65 7468  king of the neth
-000001d0: 6572 6c61 6e64 7320 7468 6174 2077 6861  erlands that wha
-000001e0: 7420 6865 2063 616c 6c73 206d 6564 6963  t he calls medic
-000001f0: 696e 6520 696e 2068 6973 2022 6361 7265  ine in his "care
-00000200: 2220 6c61 7773 2061 7265 206e 6f74 206d  " laws are not m
-00000210: 6564 6963 696e 6520 6275 7420 706f 6973  edicine but pois
-00000220: 6f6e 2e20 5072 6f6f 6620 6f66 2074 6865  on. Proof of the
-00000230: 7365 206d 6564 6963 696e 6520 6265 696e  se medicine bein
-00000240: 6720 706f 6973 6f6e 2077 6572 6520 7368  g poison were sh
-00000250: 6f77 6e20 746f 2074 6865 206b 696e 672c  own to the king,
-00000260: 2077 686f 2773 2028 7065 7273 6f6e 616c   who's (personal
-00000270: 2920 6b61 6269 6e65 7420 7772 6f74 6520  ) kabinet wrote 
-00000280: 6261 636b 2074 6861 7420 2274 6865 206b  back that "the k
-00000290: 696e 6720 746f 6f6b 206e 6f74 6520 6f66  ing took note of
-000002a0: 2077 6861 7420 6920 6861 7665 2077 7269   what i have wri
-000002b0: 7474 656e 222e 0a0a 5573 696e 6720 706f  tten"...Using po
-000002c0: 6973 6f6e 206d 616b 6573 2074 6865 2063  ison makes the c
-000002d0: 6172 6520 6c61 7773 2075 7365 6420 696e  are laws used in
-000002e0: 2074 6865 206e 6574 6865 726c 616e 6473   the netherlands
-000002f0: 2074 6f20 7072 6f76 6964 6520 6361 7265   to provide care
-00000300: 2074 6f20 656c 6465 726c 7920 616e 6420   to elderly and 
-00000310: 6861 6e64 6963 6170 7065 642c 2063 7269  handicapped, cri
-00000320: 6d69 6e61 6c73 2061 6e64 2070 7379 6368  minals and psych
-00000330: 6961 7472 6963 2070 6174 6965 6e74 7320  iatric patients 
-00000340: 6e6f 7420 6361 7265 206c 6177 7320 6275  not care laws bu
-00000350: 7420 6765 6e6f 6369 6465 206c 6177 7320  t genocide laws 
-00000360: 7769 7468 2077 6869 6368 2074 6865 206b  with which the k
-00000370: 696e 6720 6973 206b 696c 6c69 6e67 2067  ing is killing g
-00000380: 726f 7570 7320 6f66 2074 6865 2070 6f70  roups of the pop
-00000390: 756c 6174 696f 6e20 6279 2067 6976 696e  ulation by givin
-000003a0: 6720 7468 656d 2070 6f69 736f 6e20 696e  g them poison in
-000003b0: 7374 6561 6420 6f66 206d 6564 6963 696e  stead of medicin
-000003c0: 6520 696e 2074 6865 2022 6361 7265 2220  e in the "care" 
-000003d0: 7468 6579 2061 7265 2066 6f72 6365 6420  they are forced 
-000003e0: 746f 2075 6e64 6572 676f 2e0a 0a49 203a  to undergo...I :
-000003f0: 7265 663a 6077 726f 7465 203c 7772 6974  ref:`wrote <writ
-00000400: 696e 6773 3e60 2074 6865 2070 726f 7365  ings>` the prose
-00000410: 6375 746f 7220 6173 6b69 6e67 2066 6f72  cutor asking for
-00000420: 2061 6e20 6172 7265 7374 206f 6620 7468   an arrest of th
-00000430: 6520 6b69 6e67 2028 6d61 6b65 2068 696d  e king (make him
-00000440: 2073 746f 7029 2c20 7468 6520 7072 6f73   stop), the pros
-00000450: 6563 7574 6f72 2064 6563 6964 6564 2074  ecutor decided t
-00000460: 6f20 6361 6c6c 2069 7420 6120 226e 6f20  o call it a "no 
-00000470: 6261 7369 7320 746f 2070 726f 6365 6564  basis to proceed
-00000480: 222e 2049 7420 7265 7175 6972 6573 2061  ". It requires a
-00000490: 203a 7265 663a 6062 6173 6973 2074 6f20   :ref:`basis to 
-000004a0: 7072 6f73 6563 7574 6520 3c72 6563 6f6e  prosecute <recon
-000004b0: 7369 6465 723e 6020 6f66 2074 6865 2070  sider>` of the p
-000004c0: 726f 7365 6375 746f 7220 746f 2067 6574  rosecutor to get
-000004d0: 2074 6865 206b 696e 6720 696e 2068 6973   the king in his
-000004e0: 2063 656c 6c20 616e 6420 6869 7320 6765   cell and his ge
-000004f0: 6e6f 6369 6465 2c20 7468 6572 6562 792c  nocide, thereby,
-00000500: 2073 746f 7070 6564 2e0a 0a2e 2e20 7261   stopped..... ra
-00000510: 773a 3a20 6874 6d6c 0a0a 2020 2020 203c  w:: html..     <
-00000520: 6272 3e0a 2020 2020 203c 6365 6e74 6572  br>.     <center
-00000530: 3e3c 623e 404b 6172 696d 4b68 616e 5143  ><b>@KarimKhanQC
-00000540: 2072 6563 6f6e 7369 6465 7220 3c61 2068   reconsider <a h
-00000550: 7265 663d 2272 6563 6f6e 7369 6465 722e  ref="reconsider.
-00000560: 6874 6d6c 223e 4f54 502d 4352 2d31 3137  html">OTP-CR-117
-00000570: 2f31 393c 2f61 3e2e 3c2f 623e 3c2f 6365  /19</a>.</b></ce
-00000580: 6e74 6572 3e0a 0a0a 2e2e 2074 6f63 7472  nter>..... toctr
-00000590: 6565 3a3a 0a20 2020 203a 6869 6464 656e  ee::.    :hidden
-000005a0: 3a0a 2020 2020 3a67 6c6f 623a 0a0a 2020  :.    :glob:..  
-000005b0: 2020 2a0a                                  *.
+00000010: 773a 3a20 6874 6d6c 0a0a 2020 2020 203c  w:: html..     <
+00000020: 6272 3e3c 6272 3e0a 0a2e 2e20 7469 746c  br><br>.... titl
+00000030: 653a 3a20 4f54 502d 4352 2d31 3137 2f31  e:: OTP-CR-117/1
+00000040: 390a 0a0a 7c20 2a2a 496e 666f 726d 6174  9...| **Informat
+00000050: 696f 6e20 616e 6420 4576 6964 656e 6365  ion and Evidence
+00000060: 2055 6e69 742a 2a0a 7c20 2a2a 4f66 6669   Unit**.| **Offi
+00000070: 6365 206f 6620 7468 6520 5072 6f73 6563  ce of the Prosec
+00000080: 7574 6f72 2a2a 0a7c 202a 2a50 6f73 7420  utor**.| **Post 
+00000090: 4f66 6669 6365 2042 6f78 2031 3935 3139  Office Box 19519
+000000a0: 2a2a 0a7c 202a 2a32 3530 3020 434d 2054  **.| **2500 CM T
+000000b0: 6865 2048 6167 7565 2a2a 0a7c 202a 2a54  he Hague**.| **T
+000000c0: 6865 204e 6574 6865 726c 616e 6473 2a2a  he Netherlands**
+000000d0: 0a7c 200a 0a48 656c 6c6f 204f 6666 6963  .| ..Hello Offic
+000000e0: 6520 6f66 2074 6865 2050 726f 7365 6375  e of the Prosecu
+000000f0: 746f 722c 0a0a 6920 7772 6974 6520 796f  tor,..i write yo
+00000100: 7520 696e 2074 6865 2063 6f6e 7465 7874  u in the context
+00000110: 206f 6620 636f 6d6d 756e 6963 6174 696f   of communicatio
+00000120: 6e73 2061 6e64 2063 6c61 696d 7320 756e  ns and claims un
+00000130: 6465 7220 6172 742e 3135 206f 6620 0a74  der art.15 of .t
+00000140: 6865 2052 6f6d 6520 5374 6174 7574 652e  he Rome Statute.
+00000150: 2069 2077 616e 7420 746f 2069 6e66 6f72   i want to infor
+00000160: 6d20 7468 6520 7072 6f73 6563 7574 6f72  m the prosecutor
+00000170: 2074 6861 7420 7468 6520 6b69 6e67 206f   that the king o
+00000180: 6620 7468 6520 0a6e 6574 6865 726c 616e  f the .netherlan
+00000190: 6473 2061 6e64 2068 6973 2067 6f76 6572  ds and his gover
+000001a0: 6e6d 656e 7420 6172 6520 636f 6d6d 6974  nment are commit
+000001b0: 696e 6720 3320 6f66 2074 6865 2035 2063  ing 3 of the 5 c
+000001c0: 7269 6d65 7320 6465 6669 6e65 6420 0a69  rimes defined .i
+000001d0: 6e20 7468 6520 526f 6d65 2053 7461 7475  n the Rome Statu
+000001e0: 7465 2e0a 0a54 6865 2064 7574 6368 2067  te...The dutch g
+000001f0: 6f76 6572 6e6d 656e 7420 6861 7320 696e  overnment has in
+00000200: 7472 6f64 7563 6564 2074 6872 6565 206e  troduced three n
+00000210: 6577 2066 6f72 6365 6420 6361 7265 206c  ew forced care l
+00000220: 6177 732c 2074 6865 2057 667a 200a 2877  aws, the Wfz .(w
+00000230: 6574 2066 6f72 656e 7369 7363 6865 207a  et forensische z
+00000240: 6f72 6729 2066 6f72 2063 7269 6d69 6e61  org) for crimina
+00000250: 6c73 2c20 7468 6520 5776 4747 5a20 2857  ls, the WvGGZ (W
+00000260: 6574 2076 6572 706c 6963 6874 6520 4747  et verplichte GG
+00000270: 5a29 2066 6f72 200a 7468 6520 6469 7374  Z) for .the dist
+00000280: 7572 6265 6420 616e 6420 6164 6469 6374  urbed and addict
+00000290: 6564 2061 6e64 2074 6865 2057 7a64 2028  ed and the Wzd (
+000002a0: 5765 7420 7a6f 7267 2065 6e20 6477 616e  Wet zorg en dwan
+000002b0: 6729 2066 6f72 2074 6865 200a 6861 6e64  g) for the .hand
+000002c0: 6963 6170 7065 642e 0a0a 426f 7468 2074  icapped...Both t
+000002d0: 6865 2063 6861 6d62 6572 2073 7567 6765  he chamber sugge
+000002e0: 7374 696e 6720 7468 6573 6520 6c61 7773  sting these laws
+000002f0: 2074 6f20 7468 6520 6b69 6e67 2061 6e64   to the king and
+00000300: 2074 6865 206b 696e 6720 6869 6d73 656c   the king himsel
+00000310: 6620 0a68 6176 6520 6265 656e 2069 6e66  f .have been inf
+00000320: 6f72 6d65 6420 6162 6f75 7420 7468 6520  ormed about the 
+00000330: 6661 6374 2074 6865 2074 6865 2073 7562  fact the the sub
+00000340: 7374 616e 6365 7320 6164 6d69 6e69 7374  stances administ
+00000350: 6572 6564 2075 6e64 6572 200a 7468 6573  ered under .thes
+00000360: 6520 6c61 7773 2061 7265 2070 726f 7665  e laws are prove
+00000370: 6e20 746f 2062 6520 706f 6973 6f6e 2e0a  n to be poison..
+00000380: 200a 5468 6572 6520 6973 2070 726f 6f66   .There is proof
+00000390: 2074 6865 206d 6564 6963 6174 696f 6e20   the medication 
+000003a0: 7573 6564 2069 6e20 666f 7263 6564 2074  used in forced t
+000003b0: 7265 6174 656d 656e 7473 2069 6e20 7468  reatements in th
+000003c0: 6520 0a6e 6574 6865 726c 616e 6473 2061  e .netherlands a
+000003d0: 7265 2070 6f69 736f 6e2c 2073 6565 2063  re poison, see c
+000003e0: 6f70 6965 7320 6f66 2074 6865 2045 4348  opies of the ECH
+000003f0: 4120 3c60 4575 726f 7065 616e 2043 6865  A <`European Che
+00000400: 6d69 6361 6c20 4167 656e 6379 603e 0a77  mical Agency`>.w
+00000410: 6562 7369 7465 2066 6f72 3a0a 0a28 3129  ebsite for:..(1)
+00000420: 203a 7265 663a 6068 616c 646f 6c20 3c68   :ref:`haldol <h
+00000430: 616c 646f 6c3e 600a 2832 2920 3a72 6566  aldol>`.(2) :ref
+00000440: 3a60 636c 6f7a 6170 696e 6520 3c63 6c6f  :`clozapine <clo
+00000450: 7a61 7069 6e65 3e60 0a28 3329 203a 7265  zapine>`.(3) :re
+00000460: 663a 607a 7970 7265 7861 203c 7a79 7072  f:`zyprexa <zypr
+00000470: 6578 613e 600a 2834 2920 3a72 6566 3a60  exa>`.(4) :ref:`
+00000480: 6162 696c 6966 7920 3c61 6269 6c69 6679  abilify <abilify
+00000490: 3e60 0a0a 5769 7468 2074 6865 206d 6173  >`..With the mas
+000004a0: 7320 7363 616c 6520 746f 7274 7572 6520  s scale torture 
+000004b0: 7769 7468 2070 6f69 736f 6e20 7468 6520  with poison the 
+000004c0: 6b69 6e67 206f 6620 7468 6520 6e65 7468  king of the neth
+000004d0: 6572 6c61 6e64 7320 616e 6420 0a68 6973  erlands and .his
+000004e0: 2063 6861 6d62 6572 3a0a 0a28 3129 206b   chamber:..(1) k
+000004f0: 696c 6c73 0a28 3229 2064 6f65 7320 6772  ills.(2) does gr
+00000500: 6176 6520 626f 6469 6c79 2061 6e64 206d  ave bodily and m
+00000510: 656e 7461 6c20 6861 726d 0a28 3329 206d  ental harm.(3) m
+00000520: 616b 6573 2069 6d70 6f74 656e 740a 0a6f  akes impotent..o
+00000530: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00000540: 7669 6374 696d 2067 726f 7570 7320 6865  victim groups he
+00000550: 7265 2069 6e20 7468 6520 4e65 7468 6572  re in the Nether
+00000560: 6c61 6e64 733a 0a0a 2831 2920 7665 7273  lands:..(1) vers
+00000570: 6c61 6166 6465 6e20 2861 6464 6963 7473  laafden (addicts
+00000580: 290a 2832 2920 6265 6a61 6172 6465 6e20  ).(2) bejaarden 
+00000590: 2865 6c64 6572 6c79 290a 2833 2920 6767  (elderly).(3) gg
+000005a0: 7a20 7061 7469 656e 7465 6e20 2870 7379  z patienten (psy
+000005b0: 6368 6961 7472 6963 2070 6174 6965 6e74  chiatric patient
+000005c0: 7329 0a28 3429 2063 7269 6d69 6e65 6c65  s).(4) criminele
+000005d0: 6e20 2863 7269 6d69 6e69 616c 7329 0a28  n (criminials).(
+000005e0: 3529 2067 6568 616e 6469 6361 7074 656e  5) gehandicapten
+000005f0: 2028 6861 6e64 6963 6170 7065 6429 0a0a   (handicapped)..
+00000600: 5369 6e63 6520 7468 6520 6d65 6d62 6572  Since the member
+00000610: 7320 6f66 2074 6865 203a 7265 663a 6063  s of the :ref:`c
+00000620: 6861 6d62 6572 203c 6368 616d 6265 723e  hamber <chamber>
+00000630: 6020 616e 6420 7468 6520 3a72 6566 3a60  ` and the :ref:`
+00000640: 6b69 6e67 203c 6b69 6e67 3e60 0a77 6572  king <king>`.wer
+00000650: 6520 6177 6172 6520 7468 6174 2074 6865  e aware that the
+00000660: 7365 206d 6564 6963 696e 6520 6172 6520  se medicine are 
+00000670: 706f 6973 6f6e 2061 7420 7468 6520 7469  poison at the ti
+00000680: 6d65 2074 6865 7920 766f 7465 6420 666f  me they voted fo
+00000690: 7220 7468 6973 206c 6177 0a61 6e64 2074  r this law.and t
+000006a0: 6865 2064 6179 2074 6865 2057 667a 206c  he day the Wfz l
+000006b0: 6177 2074 6f6f 6b20 6566 6665 6374 2028  aw took effect (
+000006c0: 312d 312d 3230 3139 292c 2069 2061 736b  1-1-2019), i ask
+000006d0: 2074 6865 2070 726f 7365 6375 746f 7220   the prosecutor 
+000006e0: 746f 0a70 726f 7365 6375 7465 2074 6865  to.prosecute the
+000006f0: 206b 696e 6720 666f 7220 6d61 6b69 6e67   king for making
+00000700: 2074 6865 2063 6f6d 6d69 7469 6e67 206f   the commiting o
+00000710: 6620 7468 6520 6162 6f76 6520 6d65 6e74  f the above ment
+00000720: 696f 6e65 6420 6372 696d 6573 0a28 6b69  ioned crimes.(ki
+00000730: 6c6c 696e 672c 2074 6f72 7475 7265 2061  lling, torture a
+00000740: 6e64 2069 6d70 6f74 656e 7420 6d61 6b69  nd impotent maki
+00000750: 6e67 2920 706f 7373 6962 6c65 2068 6572  ng) possible her
+00000760: 6520 696e 2074 6865 206e 6574 6865 726c  e in the netherl
+00000770: 616e 6473 2069 6e0a 7468 6520 686f 7065  ands in.the hope
+00000780: 2074 6861 7420 6974 2073 746f 7073 2074   that it stops t
+00000790: 6865 206d 6173 7320 746f 7274 7572 6520  he mass torture 
+000007a0: 7769 7468 2070 6f69 736f 6e20 7468 6520  with poison the 
+000007b0: 6b69 6e67 206f 6620 7468 6520 0a6e 6574  king of the .net
+000007c0: 6865 726c 616e 6473 2061 6e64 2068 6973  herlands and his
+000007d0: 2067 6f76 6572 6e6d 656e 7420 6172 6520   government are 
+000007e0: 646f 696e 672e 0a0a 0a2e 2e20 746f 6374  doing...... toct
+000007f0: 7265 653a 3a0a 2020 2020 3a68 6964 6465  ree::.    :hidde
+00000800: 6e3a 0a20 2020 203a 676c 6f62 3a0a 0a20  n:.    :glob:.. 
+00000810: 2020 202a 0a                                *.
```

### Comparing `genocide-90/docs/informed.jpg` & `genocide-91/docs/informed.jpg`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/kamer.png` & `genocide-91/docs/kamer.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/manual.rst` & `genocide-91/docs/manual.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,135 +1,124 @@
 .. _manual:
 
-.. raw:: html
-
-     <br><br>
-
 .. title:: Manual
 
 
 .. raw:: html
 
-
-    <center>
-    <b>
-    M A N U A L
-    </b>
-    </center>
-    <br>
+     <br><br>
 
 
 **NAME**
 
- @KarimKhanQC reconsider OTP-CR-117/19
-
+ | ``GENOCIDE`` - reconsider ``OTP-CR-117/19``
 
 **SYNOPSIS**
 
  | ``genocidectl <cmd> [key=value] [key==value]``
 
 
 **DESCRIPTION**
 
- **GENOCIDE** holds evidence that king netherlands is doing a genocide, a 
+ ``GENOCIDE`` is a solid, non hackable bot, that runs under systemd as a 
+ 24/7 background service starts after reboot and is intended to be programmable
+ in a static, only code, no popen, no user imports and no reading modules from
+ a directory, way. It can show genocide and suicide stats of king netherlands
+ his genocide into a IRC channel, display rss feeds and log simple text
+ messages, source is :ref:`here <source>`.
+
+ ``GENOCIDE`` holds evidence that king netherlands is doing a genocide, a 
  written :ref:`response <king>` where king netherlands confirmed taking note
  of “what i have written”, namely :ref:`proof <evidence>` that medicine he
  uses in treatement laws like zyprexa, haldol, abilify and clozapine are poison
  that make impotent, is both physical (contracted muscles) and mental (let 
  people hallucinate) torture and kills members of the victim groups. 
 
- **GENOCIDE** contains :ref:`correspondence <writings>` with the
+ ``GENOCIDE`` contains :ref:`correspondence <writings>` with the
  International Criminal Court, asking for arrest of the king of the 
  netherlands, for the genocide he is committing with his new treatement laws.
  Current status is an outside the jurisdiction judgement of the prosecutor 
- which requires a :ref:`reconsider <reconsider>` to have the king actually
+ which requires a :ref:`reconsider <home>` to have the king actually
  arrested.
 
- **GENOCIDE** is a solid, non hackable bot, that runs under systemd as a 
- 24/7 background service starts after reboot and is intended to be programmable
- in a static, only code, no popen, no user imports and no reading modules from
- a directory, way. It can show genocide and suicide stats of king netherlands
- his genocide into a IRC channel, display rss feeds and log simple text
- messages, source is :ref:`here <source>`.
-
 **INSTALL**
 
-  | ``sudo pip3 install genocide``
-  |
+
+ | ``sudo python3 -m pip install genocide``
+ | ``sudo systemctl enable /usr/local/genocide/genocide.service --now``
+
 
 **CONFIGURATION**
 
+
  use sudo, ``genocidectl`` needs root privileges
 
- **irc**
 
-  | ``genocidectl cfg server=<server>``
-  | ``genocidectl channel=<channel>``
-  | ``genocidectl cfg nick=<nick> port=<port>``
-  |  
-  | ``(*) default is #genocide on localhost``
-  |
+ ``irc``
+
+  | ``genocidectl cfg server=<server> channel=<channel> nick=<nick>``
+  
+  | ``(*) default channel/server is #genocide on localhost``
 
- **sasl**
+ ``sasl``
 
   | ``genocidectl pwd <nickservnick> <nickservpass>``
   | ``genocidectl cfg password=<outputfrompwd>``
-  |
 
- **users**
+ ``users``
 
   | ``genocidectl cfg users=True``
   | ``genocidectl met <userhost>``
-  |
 
- **rss**
+ ``rss``
 
   | ``genocidectl rss <url>``
-  |
 
- **24/7**
+ ``24/7``
+
+  | ``systemctl enable /usr/local/genocide/genocide.service --now``
 
-  | ``systemctl enable <servicefile> --now``
-  |
-  | ``* /usr/local/share/genocide/genocide.service``
 
 **COMMANDS**
 
  ::
 
   cmd - commands
   cfg - irc configuration
   dlt - remove a user
   dpl - sets display items
   ftc - runs a fetching batch
   fnd - find objects 
-  flt - list of bus listeners
+  flt - list of instances registered to the bus
   log - log some text
   mdl - genocide model
   met - add a user
   mre - displays cached output, channel wise.
   nck - changes nick on irc
   now - genocide stats
-  pwd - create SASL passwd from nickserv creds
+  pwd - combines nickserv name/password into a sasl password
   rem - removes a rss feed
   req - request to the prosecutor
   rss - add a feed
   slg - slogan
   thr - show the running threads
   tpc - put genocide stats into topic
-  trt - torture definition
 
 
 **FILES**
 
+
  | ``/usr/local/share/doc/genocide/*``
- | ``/usr/local/share/genocide/genocide.service``
- |
+ | ``/usr/local/genocide/``
+
 
 **AUTHOR**
 
- | Bart Thate 
- |
+
+ Bart Thate 
+
 
 **COPYRIGHT**
 
- **GENOCIDE** is placed in the Public Domain.
+
+ ``GENOCIDE`` is placed in the Public Domain.
+
```

### Comparing `genocide-90/docs/pdf/EM_T04_OTP-CR-117_19.pdf` & `genocide-91/docs/pdf/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf` & `genocide-91/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/pdf/Elements-of-Crimes.pdf` & `genocide-91/docs/pdf/Elements-of-Crimes.pdf`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/pdf/Kamer.pdf` & `genocide-91/docs/pdf/Kamer.pdf`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/pdf/Rome-Statute.pdf` & `genocide-91/docs/pdf/Rome-Statute.pdf`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/pdf/Rules-of-Procedure-and-Evidence.pdf` & `genocide-91/docs/pdf/Rules-of-Procedure-and-Evidence.pdf`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/pdf/bevestigd.pdf` & `genocide-91/docs/pdf/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/reconsider.rst` & `genocide-91/docs/reconsider.rst`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,14 @@
 .. raw:: html
 
      <br><br>
 
 .. title:: Reconsider
 
 
-.. raw:: html
-
-
-    <center>
-    <b>
-    R E C O N S I D E R
-    </b>
-    </center>
-    <br>
-
-
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
```

### Comparing `genocide-90/docs/request.rst` & `genocide-91/docs/request.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 .. _request:
 
 .. raw:: html
 
-     <br><br>
+     <br>
 
 .. title:: Request
 
 
 .. raw:: html
 
-
     <center>
     <b>
-    R E Q U E S T
+
+**R E Q U E S T**
+
+.. raw:: html
+
     </b>
     </center>
     <br>
 
 
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
```

### Comparing `genocide-90/docs/skull.jpg` & `genocide-91/docs/skull.jpg`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/skullagain.jpg` & `genocide-91/docs/skullagain.jpg`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/skullnr.jpg` & `genocide-91/docs/skullnr.jpg`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/skullnr2.jpg` & `genocide-91/docs/skullnr2.jpg`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/verbatim2.png` & `genocide-91/docs/verbatim2.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/whitetxt4.png` & `genocide-91/docs/whitetxt4.png`

 * *Files identical despite different names*

### Comparing `genocide-90/docs/writings.rst` & `genocide-91/docs/writings.rst`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,14 @@
 .. raw:: html
 
      <br><br>
 
 .. title:: Writings
 
 
-.. raw:: html
-
-
-    <center>
-    <b>
-    W R I T I N G S
-    </b>
-    </center>
-    <br>
-
-
 **email 1**
 
 |
 
 | **From**: Bart Thate <bthate@dds.nl>
 | **To**: otp.informationdesk@icc-cpi.int
 | **Subject**: Information that the king of the netherlands is aware that the medicine administered with the use of new defines laws are proven to be poison and is commiting 3 of 5 genocide crimes on parts of the population here in the netherlands
```

### Comparing `genocide-90/genocide/cmds.py` & `genocide-91/genocide/modules/sts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,61 @@
 # This file is placed in the Public Domain.
-# pylint: disable=E1101,R0903,C0115,C0116
+# pylint: disable=C0115,C0116,C0301,E1101,E0402
 
 
-"command"
+"runtime information"
 
 
+import os
 import threading
 import time
 
 
-from genocide.handler import Bus, Command
-from genocide.object import Class, Object, find, fntime, save, update
-from genocide.run import starttime
-from genocide.thread import name
-from genocide.util import elapsed
-
+from .. import Bus, Object, elapsed, name, update
+from .. import modules as gmod
 
 def __dir__():
     return (
-            'Log',
-            'Todo',
-            'cmd',
             'flt',
-            'log',
-            'tdo',
+            'mod',
             'thr',
             'upt'
            )
 
 
-class Log(Object):
-
-    def __init__(self):
-        Object.__init__(self)
-        self.txt = ""
-
-
-Class.add(Log)
-
-
-class Todo(Log):
-
-    pass
-
-
-Class.add(Todo)
-
-
-def cmd(event):
-    event.reply(",".join(sorted(Command.cmd)))
+starttime = time.time()
 
 
 def flt(event):
     try:
         index = int(event.args[0])
         event.reply(Bus.objs[index])
         return
     except (KeyError, TypeError, IndexError, ValueError):
         pass
     event.reply(" | ".join([name(o) for o in Bus.objs]))
 
 
-def log(event):
-    if not event.rest:
-        nmr = 0
-        for obj in find("log"):
-            event.reply("%s %s %s" % (
-                                      nmr,
-                                      obj.txt,
-                                      elapsed(time.time() - fntime(obj.__fnm__)))
-                                     )
-            nmr += 1
-        return
-    obj = Log()
-    obj.txt = event.rest
-    save(obj)
-    event.done()
-
-
-def tdo(event):
-    if not event.rest:
-        nmr = 0
-        for obj in find("todo"):
-            event.reply("%s %s %s" % (
-                                      nmr,
-                                      obj.txt,
-                                      elapsed(time.time() - fntime(obj.__fnm__))
-                                     ))
-            nmr += 1
-        return
-    obj = Todo()
-    obj.txt = event.rest
-    save(obj)
-    event.done()
+def mod(event):
+    path = gmod.__path__[0]
+    event.reply(",".join([x[:-3] for x in os.listdir(path) if not (x.startswith("_") or x.endswith("~"))]))
 
 
 def thr(event):
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
         if str(thread).startswith("<_"):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, "sleep", None):
             uptime = obj.sleep - int(time.time() - obj.state["latest"])
         else:
-            uptime = int(time.time() - obj.starttime)
-        result.append((uptime, thread.getName()))
+            uptime = int(time.time() - starttime)
+        result.append((uptime, thread.name))
     res = []
     for uptime, txt in sorted(result, key=lambda x: x[0]):
         res.append("%s/%s" % (txt, elapsed(uptime)))
     if res:
         event.reply(" ".join(res))
     else:
         event.reply("no threads running")
```

### Comparing `genocide-90/genocide/irc.py` & `genocide-91/genocide/modules/irc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,R0201,C0413,R0902,R0903,W0201,W0613
-# pylint: disable=E1101,R0912,R0915,R0904,W0221
+# pylint: disable=E1101,R0912,R0915,R0904,W0221,E0402
 
 
-"irc"
+"internet relay chat"
 
 
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from genocide.object import Class, Default, Object
-from genocide.object import keys, last, printable
-from genocide.object import edit, fntime, find, save, update
-from genocide.object import locked, register
-from genocide.handler import Command, Event, Handler
-from genocide.thread import launch
-from genocide.util import elapsed
+from .. import Class, Command, Default, Event, Handler, Object, Users
+from .. import edit, keys, last, printable, save
+from .. import launch, locked, register
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
             'cfg',
-            'dlt',
             'init',
-            'met',
             'mre',
             'pwd'
            )
 
 
 __all__ = __dir__()
 
 
 NAME = "genocide"
-REALNAME = '@KarimKhanQC reconsider OTP-CR-117/19 - http://pypi.org/project/genocide'
+REALNAME = "@KarimKhanQC reconsider OTP-CR-117/19"
+
 
 saylock = _thread.allocate_lock()
 
 
 def init():
     irc = IRC()
     irc.start()
@@ -209,15 +204,15 @@
         self.register("AUTHENTICATE", self.auth)
         self.register("CAP", self.cap)
         self.register("ERROR", self.error)
         self.register("LOG", self.log)
         self.register("NOTICE", self.notice)
         self.register("PRIVMSG", self.privmsg)
         self.register("QUIT", self.quit)
-        #self.register("command", Command.handle)
+        self.register("command", Command.handle)
 
     def announce(self, txt):
         for channel in self.channels:
             self.say(channel, txt)
 
     def auth(self, event):
         time.sleep(1.0)
@@ -523,15 +518,15 @@
         assert self.cfg.server
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.connected.clear()
         self.joined.clear()
         Output.start(self)
-        Handler.start(self)
+        launch(Handler.start, self)
         launch(
                self.doconnect,
                self.cfg.server,
                self.cfg.nick,
                int(self.cfg.port or "6667")
               )
         if not self.keeprunning:
@@ -541,71 +536,14 @@
         try:
             self.sock.shutdown(2)
         except OSError:
             pass
         Handler.stop(self)
 
 
-class Users(Object):
-
-    @staticmethod
-    def allowed(origin, perm):
-        perm = perm.upper()
-        user = Users.get_user(origin)
-        val = False
-        if user and perm in user.perms:
-            val = True
-        return val
-
-    @staticmethod
-    def delete(origin, perm):
-        res = False
-        for user in Users.get_users(origin):
-            try:
-                user.perms.remove(perm)
-                save(user)
-                res = True
-            except ValueError:
-                pass
-        return res
-
-    @staticmethod
-    def get_users(origin=""):
-        selector = {"user": origin}
-        return find("user", selector)
-
-    @staticmethod
-    def get_user(origin):
-        users = list(Users.get_users(origin))
-        res = None
-        if len(users) > 0:
-            res = users[-1][-1]
-        return res
-
-    @staticmethod
-    def perm(origin, permission):
-        user = Users.get_user(origin)
-        if not user:
-            raise NoUser(origin)
-        if permission.upper() not in user.perms:
-            user.perms.append(permission.upper())
-            save(user)
-        return user
-
-
-class User(Object):
-
-    def __init__(self, val=None):
-        super().__init__()
-        self.user = ""
-        self.perms = []
-        if val:
-            update(self, val)
-
-
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(printable(
                               config,
                               keys(config),
@@ -613,45 +551,14 @@
                              )
     else:
         edit(config, event.sets)
         save(config)
         event.done()
 
 
-def dlt(event):
-    if not event.args:
-        event.reply("dlt <username>")
-        return
-    selector = {"user": event.args[0]}
-    for obj in find("user", selector):
-        obj.__deleted__ = True
-        save(obj)
-        event.done()
-        break
-
-
-def met(event):
-    if not event.rest:
-        nmr = 0
-        for obj in find("user"):
-            event.reply("%s %s %s %s" % (
-                                         nmr,
-                                         obj.user,
-                                         obj.perms,
-                                         elapsed(time.time() - fntime(obj.__fnm__)))
-                                        )
-            nmr += 1
-        return
-    user = User()
-    user.user = event.rest
-    user.perms = ["USER"]
-    save(user)
-    event.done()
-
-
 def mre(event):
     if not event.channel:
         event.reply("channel is not set.")
         return
     bot = event.bot()
     if "cache" not in dir(bot):
         event.reply("bot is missing cache")
@@ -675,8 +582,7 @@
     enc = txt.encode("ascii")
     base = base64.b64encode(enc)
     dcd = base.decode("ascii")
     event.reply(dcd)
 
 
 Class.add(Config)
-Class.add(User)
```

### Comparing `genocide-90/genocide/model.py` & `genocide-91/genocide/modules/mdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # This file is placed in the Public Domain.
-# pylint: disable=E1101,C0116,C0301,W0613,R1710
+# pylint: disable=E1101,C0116,C0301,W0613,R1710,E0402
 
 
-"model"
+"dutch genocide model"
 
 
 import datetime
 import time
 
 
-from genocide.object import Object,  keys
-from genocide.handler import Bus, Event
-from genocide.thread import Repeater, launch
-from genocide.util import elapsed
+from genocide import Bus, Event, Object, Repeater
+from genocide import elapsed, keys, launch
 
 
 def __dir__():
     return (
         "init",
         "mdl",
         "now"
@@ -400,15 +398,15 @@
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
         txt += "%s: %s " % (getalias(name), nrtimes)
     txt += " http://genocide.rtfd.io"
-    Bus.announce(txt)
+    event.reply(txt)
 
 
 def mdl(event):
     name = event.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
@@ -420,15 +418,15 @@
                                                                nrtimes,
                                                                getalias(name),
                                                                thisday,
                                                                nrday,
                                                                nryear,
                                                                elapsed(needed)
                                                               )
-        Bus.announce(txt)
+        event.reply(txt)
 
 
 def tpc(event):
     txt = "%ss " % elapsed(time.time() - STARTTIME)
     for name in sorted(oorzaken, key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         delta = time.time() - STARTTIME
```

### Comparing `genocide-90/genocide/object.py` & `genocide-91/genocide/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,52 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0112,C0115,C0116,W0613,W0108,R0903
 
 
-"object"
+"""objects
+
+
+this module contains a big Object class that provides a clean, no methods,
+namespace for json data to be read into. this is necessary so that methods
+don't get overwritten by __dict__ updating and, without methods defined on
+the object, is easily being updated from a on disk stored json (dict).
+
+basic usage is this:
+
+>>> import genocide
+>>> o = genocide.Object()
+>>> o.key = "value"
+>>> o.key
+'value'
+
+Some hidden methods are provided, methods are factored out into functions
+like get, items, keys, register, set, update and values.
+
+load/save from/to disk:
+
+>>> from genocide import Object, load, save
+>>> o = Object()
+>>> o.key = "value"
+>>> p = save(o)
+>>> oo = Object()
+>>> load(oo, p)
+>>> oo.key
+'value'
+
+big Objects can be searched with database functions and uses read-only files
+to improve persistence and a type in filename for reconstruction:
+
+>>> from genocide import Object, save
+>>> o = Object()
+>>> save(o)  # doctest: +ELLIPSIS
+'genocide.objects.Object/...'
+
+great for giving objects peristence by having their state stored in files.
+
+"""
 
 
 import datetime
 import json
 import os
 import pathlib
 import time
@@ -33,18 +73,20 @@
             'hook',
             'items',
             'keys',
             'kind',
             'last',
             'load',
             'loads',
+            'locked',
             'match',
             'printable',
             'register',
             'save',
+            'spl',
             'update',
             'values',
             'write'
            )
 
 
 __all__ = __dir__()
@@ -86,15 +128,17 @@
         self.__fnm__ = os.path.join(
             kind(self),
             str(uuid.uuid4().hex),
             os.sep.join(str(datetime.datetime.now()).split()),
         )
         if args:
             val = args[0]
-            if isinstance(val, zip):
+            if isinstance(val, list):
+                update(self, dict(val))
+            elif isinstance(val, zip):
                 update(self, dict(val))
             elif isinstance(val, dict):
                 update(self, val)
             elif isinstance(val, Object):
                 update(self, vars(val))
         if kwargs:
             self.__dict__.update(kwargs)
@@ -169,16 +213,16 @@
         value = getattr(obj, key, None)
         if not value:
             continue
         if " object at " in str(value):
             continue
         txt = ""
         if plain:
-            txt = str(value)
-        elif isinstance(value, str) and len(value.split()) >= 2:
+            value = str(value)
+        if isinstance(value, str) and len(value.split()) >= 2:
             txt = '%s="%s"' % (key, value)
         else:
             txt = '%s=%s' % (key, value)
         res.append(txt)
     txt = " ".join(res)
     return txt.strip()
 
@@ -394,16 +438,18 @@
     result = []
     for nme in names:
         res = Db.find(nme, selector, index, timed, deleted)
         result.extend(res)
     return sorted(result, key=lambda x: fntime(x.__fnm__))
 
 
-def last(obj):
-    ooo = Db.last(kind(obj))
+def last(obj, selector=None):
+    if selector is None:
+        selector = {}
+    ooo = Db.last(kind(obj), selector)
     if ooo:
         update(obj, ooo)
         obj.__fnm__ = ooo.__fnm__
 
 
 def match(otp, selector=None):
     names = Class.full(otp)
@@ -415,15 +461,18 @@
     return None
 
 
 def search(obj, selector):
     res = False
     select = Object(selector)
     for key, value in items(select):
-        val = getattr(obj, key)
+        try:
+            val = getattr(obj, key)
+        except AttributeError:
+            continue
         if str(value) in str(val):
             res = True
             break
     return res
 
 
 class Class:
@@ -466,14 +515,26 @@
         return Wd.workdir
 
     @staticmethod
     def getpath(path):
         return os.path.join(Wd.get(), "store", path)
 
     @staticmethod
+    def moddir():
+        mdr = os.path.join(Wd.get(), "mod")
+        cdir(mdr)
+        return mdr
+
+    @staticmethod
+    def nmdir():
+        mdr = os.path.join(Wd.get(), "notmod")
+        cdir(mdr)
+        return mdr
+
+    @staticmethod
     def set(path):
         Wd.workdir = path
 
     @staticmethod
     def storedir():
         sdr =  os.path.join(Wd.get(), "store", '')
         cdir(sdr)
@@ -488,16 +549,26 @@
                 continue
             if fnm not in res:
                 res.append(fnm)
         return res
 
 
 def cdir(path):
-    if not os.path.isdir(path):
+    path = os.path.abspath(path)
+    fname = path.split(os.sep)[-1]
+    if fname.count(":") == 2:
         path = os.path.dirname(path)
     ppp = pathlib.Path(path)
     ppp.mkdir(parents=True, exist_ok=True)
 
 
+def spl(txt):
+    try:
+        res = txt.split(",")
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
+
+
 Class.add(Object)
 Class.add(Default)
```

### Comparing `genocide-90/genocide/request.py` & `genocide-91/genocide/modules/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0114,C0115,C0116
 
 
-"""| **Information and Evidence Unit**
+"""@KarimKhanQC reconsider OTP-CR-117/19
+
+
+| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 
 Hello Office of the Prosecutor,
@@ -74,9 +77,9 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
-def request(event):
+def req(event):
     event.reply(__doc__)
```

### Comparing `genocide-90/genocide/rss.py` & `genocide-91/genocide/modules/rss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=R0903,C0115,C0116
+# pylint: disable=E1121,R0903,C0115,C0116,E0402
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -13,21 +13,18 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from genocide.object import Class, Db, Default, Object, write
-from genocide.object import find, fntime, last, printable, save
-from genocide.object import edit, register, update
-from genocide.handler import Bus
-from genocide.run import Cfg
-from genocide.thread import Repeater, launch
-from genocide.util import elapsed, spl
+from genocide import Bus, Cfg, Class, Db, Default, Object, Repeater
+from genocide import find, fntime, last, printable, save, spl
+from genocide import edit, register, update, write
+from genocide import elapsed, launch
 
 
 def __dir__():
     return (
         "Feed",
         "Fetcher",
         "Rss",
@@ -292,15 +289,16 @@
         if not nrs:
             event.reply("no rss feed found.")
         return
     url = event.args[0]
     if "http" not in url:
         event.reply("i need an url")
         return
-    res = list(find("rss", {"rss": url}))
+    dbs = Db()
+    res = dbs.last("rss", {"rss": url})
     if res:
         event.reply("already got %s" % url)
         return
     feed = Rss()
     feed.rss = event.args[0]
     save(feed)
     event.done()
```

### Comparing `genocide-90/genocide/thread.py` & `genocide-91/genocide/threads.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file is placed in the Public Domain.
-# pylint: disable=R,C,W,C0302
+# pylint: disable=C0112,C0115,C0116,R0902
 
 
-"thread"
+"threads"
 
 
-import os
 import queue
 import threading
 import time
 import types
 
 
 def __dir__():
     return (
             'Thread',
             'Timer',
             'Repeater',
+            'elapsed',
             'launch',
             'name'
-           ) 
+           )
 
 
 __all__ = __dir__()
 
 
 class Thread(threading.Thread):
 
@@ -55,18 +55,19 @@
         return self._result
 
     def run(self) -> None:
         ""
         func, args = self.queue.get()
         if args:
             self._evt = args[0]
+            if "txt" in self._evt:
+                self.name = self._evt.txt
         self.starttime = time.time()
         self._result = func(*args)
 
-
 class Timer:
 
     def __init__(self, sleep, func, *args, thrname=None):
         super().__init__()
         self.args = args
         self.func = func
         self.sleep = sleep
@@ -100,14 +101,55 @@
 
     def run(self):
         thr = launch(self.start)
         super().run()
         return thr
 
 
+def elapsed(seconds, short=True):
+    txt = ""
+    nsec = float(seconds)
+    if nsec < 1:
+        return f"{nsec:.4f}s"
+    year = 365*24*60*60
+    week = 7*24*60*60
+    nday = 24*60*60
+    hour = 60*60
+    minute = 60
+    years = int(nsec/year)
+    nsec -= years*year
+    weeks = int(nsec/week)
+    nsec -= weeks*week
+    nrdays = int(nsec/nday)
+    nsec -= nrdays*nday
+    hours = int(nsec/hour)
+    nsec -= hours*hour
+    minutes = int(nsec/minute)
+    nsec -= int(minute*minutes)
+    sec = int(nsec)
+    if years:
+        txt += "%sy" % years
+    if weeks:
+        nrdays += weeks * 7
+    if nrdays:
+        txt += "%sd" % nrdays
+    if years and short and txt:
+        return txt.strip()
+    if hours:
+        txt += "%sh" % hours
+    if minutes:
+        txt += "%sm" % minutes
+    if sec:
+        txt += "%ss" % sec
+    else:
+        txt += "0s"
+    txt = txt.strip()
+    return txt
+
+
 def launch(func, *args, **kwargs):
     thrname = kwargs.get("name", name(func))
     thr = Thread(func, thrname, *args)
     thr.start()
     return thr
 
 
@@ -118,9 +160,9 @@
     if "__self__" in dir(obj):
         return "%s.%s" % (obj.__self__.__class__.__name__, obj.__name__)
     if "__class__" in dir(obj) and "__name__" in dir(obj):
         return "%s.%s" % (obj.__class__.__name__, obj.__name__)
     if "__class__" in dir(obj):
         return obj.__class__.__name__
     if "__name__" in dir(obj):
-        return obj.__name__
+        return "%s.%s" % (obj.__class__.__name__, obj.__name__)
     return None
```

### Comparing `genocide-90/genocide.egg-info/PKG-INFO` & `genocide-91/genocide.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genocide
-Version: 90
+Version: 91
 Summary: @KarimKhanQC reconsider OTP-CR-117/19
 Home-page: https://github.com/bthate/genocide
 Author: Bart Thate
 Author-email: bthate67@gmail.com
 License: Public Domain
 Description: | **Information and Evidence Unit**
         | **Office of the Prosecutor**
```

### Comparing `genocide-90/genocide.egg-info/SOURCES.txt` & `genocide-91/genocide.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 docs/guilty.rst
 docs/index.rst
 docs/informed.jpg
 docs/kamer.png
 docs/manual.rst
 docs/reconsider.rst
 docs/request.rst
-docs/requirements.txt
 docs/skull.jpg
 docs/skullagain.jpg
 docs/skullnr.jpg
 docs/skullnr2.jpg
 docs/source.rst
 docs/verbatim2.png
 docs/whitetxt4.png
@@ -42,34 +41,36 @@
 docs/pdf/Elements-of-Crimes.pdf
 docs/pdf/Kamer.pdf
 docs/pdf/Rome-Statute.pdf
 docs/pdf/Rules-of-Procedure-and-Evidence.pdf
 docs/pdf/bevestigd.pdf
 files/genocide.service
 genocide/__init__.py
-genocide/cmds.py
 genocide/handler.py
-genocide/irc.py
-genocide/model.py
-genocide/object.py
-genocide/request.py
-genocide/rss.py
-genocide/run.py
-genocide/slogan.py
-genocide/thread.py
-genocide/util.py
+genocide/message.py
+genocide/objects.py
+genocide/runtime.py
+genocide/threads.py
+genocide/usersdb.py
 genocide.egg-info/PKG-INFO
 genocide.egg-info/SOURCES.txt
 genocide.egg-info/dependency_links.txt
 genocide.egg-info/top_level.txt
 genocide.egg-info/zip-safe
+genocide/modules/__init__.py
+genocide/modules/cmd.py
+genocide/modules/irc.py
+genocide/modules/krn.py
+genocide/modules/mdl.py
+genocide/modules/req.py
+genocide/modules/rss.py
+genocide/modules/sts.py
+genocide/modules/usr.py
 test/test_bus.py
 test/test_dbs.py
 test/test_evt.py
 test/test_hdl.py
 test/test_irc.py
-test/test_mdl.py
 test/test_obj.py
 test/test_rss.py
 test/test_thr.py
-test/test_tmr.py
-test/test_zcmd.py
+test/test_tmr.py
```

### Comparing `genocide-90/setup.py` & `genocide-91/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,27 +24,27 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name='genocide',
-    version='90',
+    version='91',
     url='https://github.com/bthate/genocide',
     author='Bart Thate',
     author_email='bthate67@gmail.com', 
     description="@KarimKhanQC reconsider OTP-CR-117/19",
     long_description=read(),
     long_description_content_type='text/x-rst',
     license='Public Domain',
-    packages=["genocide"],
+    packages=["genocide", "genocide.modules"],
     zip_safe=True,
     include_package_data=True,
     data_files=[
-                ("share/genocide", ["files/genocide.service",]),
+                ("genocide", ["files/genocide.service",]),
                 ("share/doc/genocide", uploadlist("docs")),
                 ("share/doc/genocide/pdf", uploadlist("docs/pdf")),
                 ("share/doc/genocide/_static", uploadlist("docs/_static")),
                 ("share/doc/genocide/_templates", uploadlist("docs/_templates")),
                ],
     scripts=["bin/genocide", "bin/genocidecmd", "bin/genocidectl", "bin/genocided"],
     classifiers=['Development Status :: 3 - Alpha',
```

### Comparing `genocide-90/test/test_bus.py` & `genocide-91/test/test_bus.py`

 * *Files identical despite different names*

### Comparing `genocide-90/test/test_obj.py` & `genocide-91/test/test_obj.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 
 import json
 import os
 import unittest
 
 
-from genocide.object import Object, Wd, items, keys, register, update, values
-from genocide.object import edit, kind, load, save
-from genocide.object import ObjectDecoder, ObjectEncoder
-from genocide.object import printable
+from genocide.objects import Object, Wd, items, keys, register, update, values
+from genocide.objects import edit, kind, load, save
+from genocide.objects import ObjectDecoder, ObjectEncoder
+from genocide.objects import printable
 
 
 Wd.workdir = ".test"
 
 
 VALIDJSON = '{"test": "bla"}'
 
@@ -153,15 +153,15 @@
         obj = Object()
         self.assertEqual(len(obj), 0)
 
     def test_module(self):
         self.assertTrue(Object().__module__, "op")
 
     def test_kind(self):
-        self.assertEqual(kind(Object()), "genocide.object.Object")
+        self.assertEqual(kind(Object()), "genocide.objects.Object")
 
     def test_repr(self):
         self.assertTrue(update(Object(),
                                {"key": "value"}).__repr__(), {"key": "value"})
 
     def test_setattr(self):
         obj = Object()
```

