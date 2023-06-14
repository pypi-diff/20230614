# Comparing `tmp/starrail-toolkit-0.6.9.tar.gz` & `tmp/starrail-toolkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.6.9.tar", last modified: Sun Jun  4 17:42:25 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.7.0.tar", last modified: Wed Jun 14 13:21:41 2023, max compression
```

## Comparing `starrail-toolkit-0.6.9.tar` & `starrail-toolkit-0.7.0.tar`

### file list

```diff
@@ -1,75 +1,80 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.614493 starrail-toolkit-0.6.9/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     6000 2023-06-04 17:42:25.614354 starrail-toolkit-0.6.9/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     5493 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-06-04 17:42:25.614531 starrail-toolkit-0.6.9/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.607913 starrail-toolkit-0.6.9/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.608364 starrail-toolkit-0.6.9/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3827 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.609546 starrail-toolkit-0.6.9/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6284 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1318 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/factory.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6566 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1080 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/migrate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     7702 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6287 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.609750 starrail-toolkit-0.6.9/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6752 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.610352 starrail-toolkit-0.6.9/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1916 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/config.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      304 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      645 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      576 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/common/thread.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.611080 starrail-toolkit-0.6.9/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    26369 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/unlock_fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3046 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.611580 starrail-toolkit-0.6.9/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2830 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/pie_chart.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.611872 starrail-toolkit-0.6.9/starrail/unlock/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/unlock/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/unlock/fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/unlock/service.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.612574 starrail-toolkit-0.6.9/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2459 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/utils/accounts.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.613387 starrail-toolkit-0.6.9/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     5198 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    10670 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/misc.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.614170 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     6000 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1785 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.878758 starrail-toolkit-0.7.0/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6008 2023-06-14 13:21:41.878560 starrail-toolkit-0.7.0/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5501 2023-06-14 13:20:38.000000 starrail-toolkit-0.7.0/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-06-14 13:21:41.878812 starrail-toolkit-0.7.0/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.868720 starrail-toolkit-0.7.0/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1939 2023-06-14 09:48:24.000000 starrail-toolkit-0.7.0/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.869320 starrail-toolkit-0.7.0/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3827 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.871111 starrail-toolkit-0.7.0/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6284 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1318 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/factory.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1164 2023-06-14 07:33:08.000000 starrail-toolkit-0.7.0/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6566 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1080 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/migrate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     7702 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6287 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.871376 starrail-toolkit-0.7.0/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     7233 2023-06-14 09:10:59.000000 starrail-toolkit-0.7.0/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.872320 starrail-toolkit-0.7.0/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1916 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      332 2023-06-14 09:10:36.000000 starrail-toolkit-0.7.0/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      679 2023-06-14 08:55:08.000000 starrail-toolkit-0.7.0/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      576 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gui/common/thread.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.873976 starrail-toolkit-0.7.0/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4456 2023-06-14 13:19:24.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/announcements.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-06-06 06:52:24.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    26369 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-06-13 09:01:52.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/unlock_fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3046 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.874734 starrail-toolkit-0.7.0/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2830 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/pie_chart.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.875019 starrail-toolkit-0.7.0/starrail/mihoyo/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-14 09:19:50.000000 starrail-toolkit-0.7.0/starrail/mihoyo/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      241 2023-06-14 09:35:53.000000 starrail-toolkit-0.7.0/starrail/mihoyo/api.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.875559 starrail-toolkit-0.7.0/starrail/unlock/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/unlock/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/unlock/fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/unlock/service.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.876529 starrail-toolkit-0.7.0/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2459 2023-06-04 14:27:29.000000 starrail-toolkit-0.7.0/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.877353 starrail-toolkit-0.7.0/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5302 2023-06-14 09:04:40.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    10871 2023-06-14 09:35:53.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1349 2023-06-14 10:04:01.000000 starrail-toolkit-0.7.0/starrail/utils/download.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-06-02 03:58:21.000000 starrail-toolkit-0.7.0/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      346 2023-06-14 07:36:34.000000 starrail-toolkit-0.7.0/starrail/utils/misc.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-06-14 13:20:08.000000 starrail-toolkit-0.7.0/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-14 13:21:41.878291 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6008 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1904 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-06-14 13:21:41.000000 starrail-toolkit-0.7.0/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.6.9/LICENSE` & `starrail-toolkit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/PKG-INFO` & `starrail-toolkit-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.6.9
+Version: 0.7.0
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,28 +17,27 @@
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
 ## 开发状态
 
+**近期考试&其他事情比较忙，更新延缓一周（自2023.6.12起）左右**
+
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.9    |    0.6.9     |   0.6.9   |   0.6.9    |
+|   0.6.9    |    0.7.0     |   0.7.0   |   0.6.9    |
 
-目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
+目前大部分计划中的 feature 已实现完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
-- [x] 支持更多的可设置选项
-- [x] 支持解锁120帧
-- [x] 支持以 SRGF 标准导出
-- [x] 支持以 SRGF 标准导入
-- [x] 支持手动设置 API URL
-- [x] 支持夜间模式
-- [x] 支持多用户切换
-- [x] 美化程序界面
+- [x] 获取官方公告
+- [ ] 支持配置 SToken 用于抽卡导出
+- [ ] 支持 UP 池计算
+- [ ] 开拓月历
+- [ ] 米游社信息相关
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
```

### Comparing `starrail-toolkit-0.6.9/README.md` & `starrail-toolkit-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
 ## 开发状态
 
+**近期考试&其他事情比较忙，更新延缓一周（自2023.6.12起）左右**
+
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.9    |    0.6.9     |   0.6.9   |   0.6.9    |
+|   0.6.9    |    0.7.0     |   0.7.0   |   0.6.9    |
 
-目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
+目前大部分计划中的 feature 已实现完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
-- [x] 支持更多的可设置选项
-- [x] 支持解锁120帧
-- [x] 支持以 SRGF 标准导出
-- [x] 支持以 SRGF 标准导入
-- [x] 支持手动设置 API URL
-- [x] 支持夜间模式
-- [x] 支持多用户切换
-- [x] 美化程序界面
+- [x] 获取官方公告
+- [ ] 支持配置 SToken 用于抽卡导出
+- [ ] 支持 UP 池计算
+- [ ] 开拓月历
+- [ ] 米游社信息相关
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
```

### Comparing `starrail-toolkit-0.6.9/setup.py` & `starrail-toolkit-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/__init__.py` & `starrail-toolkit-0.7.0/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/config.py` & `starrail-toolkit-0.7.0/starrail/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 
 from easydict import EasyDict
 
 userroot = os.path.abspath(os.path.expanduser('~'))
+srroot = os.path.join(userroot, '.starrail')
 
 
 class Configuration(EasyDict):
 
     def __init__(self, d=None, **kwargs):
         self.no_flush = True
         self.skip_keys = set()
@@ -34,32 +35,35 @@
                 for k in self.user_keys if k not in self.skip_keys
             }
             with open(self.config_path, 'w', encoding='utf-8') as fcfg:
                 json.dump(cfg, fcfg, indent=2)
 
 
 configuration = Configuration(
-    cache_dir=os.path.join(userroot, '.starrail'),
-    db_dir=os.path.join(userroot, '.starrail', 'database'),
-    config_path=os.path.join(userroot, '.starrail', 'config.json'),
-    account_record_path=os.path.join(userroot, '.starrail', 'accounts.json'),
+    cache_dir=srroot,
+    db_dir=os.path.join(srroot, 'database'),
+    config_path=os.path.join(srroot, 'config.json'),
+    account_record_path=os.path.join(srroot, 'accounts.json'),
+    res_cache_dir=os.path.join(srroot, 'cache'),
     check_update=True,
     locale='zhs',
     log_level='DEBUG',
 )
 configuration.set_skip_keys(
     'skip_keys', 'no_flush',
     'cache_dir', 'config_path', 'db_dir', 'account_record_path',
+    'res_cache_dir',
 )
 
 
 def init_config():
 
     os.makedirs(configuration.cache_dir, exist_ok=True)
     os.makedirs(configuration.db_dir, exist_ok=True)
+    os.makedirs(configuration.res_cache_dir, exist_ok=True)
 
     if os.path.isfile(configuration.config_path):
         with open(configuration.config_path, encoding='utf-8') as fcfg:
             custom_config = json.load(fcfg)
 
         configuration.update(custom_config)
     else:
```

### Comparing `starrail-toolkit-0.6.9/starrail/entry/cli.py` & `starrail-toolkit-0.7.0/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/entry/gui.py` & `starrail-toolkit-0.7.0/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/entry/setup.py` & `starrail-toolkit-0.7.0/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/autodet.py` & `starrail-toolkit-0.7.0/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/database.py` & `starrail-toolkit-0.7.0/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/factory.py` & `starrail-toolkit-0.7.0/starrail/gacha/factory.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/fetch.py` & `starrail-toolkit-0.7.0/starrail/gacha/fetch.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         r = requests.get(url, timeout=timeout)
         if 200 <= r.status_code < 300:
             content = r.content.decode('utf-8', errors='ignore')
             payload = json.loads(content)
             logger.debug(json.dumps(payload, ensure_ascii=False, indent=2))
             return payload, r.status_code
     except Exception:
-        traceback.print_exc()
+        logger.error(traceback.format_exc())
     return None, -1
 
 
 def fetch_text(url):
     try:
         r = requests.get(url)
         if 200 <= r.status_code < 300:
             content = r.content.decode('utf-8', errors='ignore')
             return content, r.status_code
     except Exception:
-        traceback.print_exc()
+        logger.error(traceback.format_exc())
     return None, -1
```

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/fileio.py` & `starrail-toolkit-0.7.0/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/migrate.py` & `starrail-toolkit-0.7.0/starrail/gacha/migrate.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/parse.py` & `starrail-toolkit-0.7.0/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/service.py` & `starrail-toolkit-0.7.0/starrail/gacha/service.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gacha/url.py` & `starrail-toolkit-0.7.0/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/application.py` & `starrail-toolkit-0.7.0/starrail/gui/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from qfluentwidgets import NavigationInterface, NavigationItemPosition
 from qframelesswindow import FramelessWindow
 
 from starrail.gui.common.config import qcfg
 from starrail.gui.common.icon import Icon
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.utils import checkUpdate
+from starrail.gui.interfaces.announcements import AnnouncementsInterface
 from starrail.gui.interfaces.gacha_sync import GachaSyncInterface
 from starrail.gui.interfaces.home import HomeInterface
 from starrail.gui.interfaces.setting import SettingInterface
 from starrail.gui.interfaces.unlock_fps import UnlockFpsInterface
 from starrail.gui.interfaces.users import UsersInterface
 from starrail.gui.widgets.title_bar import CustomTitleBar
 from starrail.utils import babelfish
@@ -60,14 +61,19 @@
         self.hBoxLayout = QHBoxLayout(self)
         self.widgetLayout = QHBoxLayout()
 
         self.stackWidget = StackedWidget(self)
         self.navigationInterface = NavigationInterface(self, True, True)
 
         self.homeInterface = HomeInterface(self)
+        self.announcementsInterface = AnnouncementsInterface(
+            babelfish.ui_announcements(),
+            babelfish.ui_announcements_desc(),
+            self,
+        )
         self.gachaSyncInterface = GachaSyncInterface(
             babelfish.ui_gacha_sync(),
             babelfish.ui_gacha_sync_desc(),
             self,
         )
         self.unlockFpsInterface = UnlockFpsInterface(
             babelfish.ui_unlock_fps(),
@@ -109,14 +115,22 @@
             babelfish.ui_welcome(),
             NavigationItemPosition.TOP,
         )
 
         self.navigationInterface.addSeparator()
 
         self.addSubInterface(
+            self.announcementsInterface,
+            'announcementInterface',
+            Icon.MEGAPHONE,
+            babelfish.ui_announcements(),
+            NavigationItemPosition.TOP,
+        )
+
+        self.addSubInterface(
             self.gachaSyncInterface,
             'gachaSyncInterface',
             qfluentwidgets.FluentIcon.SYNC,
             babelfish.ui_gacha_sync(),
             NavigationItemPosition.TOP,
         )
```

### Comparing `starrail-toolkit-0.6.9/starrail/gui/common/config.py` & `starrail-toolkit-0.7.0/starrail/gui/common/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.7.0/starrail/gui/common/stylesheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from qfluentwidgets import StyleSheetBase, Theme, qconfig
 
 
 class StyleSheet(StyleSheetBase, Enum):
     """ Style sheet  """
 
+    ANNOUNCEMENT = 'announcement'
     BASE_INTERFACE = 'base_interface'
     CHECK_UPDATE_DIALOG = 'check_update_dialog'
     GACHA_RECORD = 'gacha_record'
     HOME_INTERFACE = 'home_interface'
     LINK_CARD = 'link_card'
     RESULT_TABLE_WIDGET = 'result_table_widget'
     SETTING_INTERFACE = 'setting_interface'
```

### Comparing `starrail-toolkit-0.6.9/starrail/gui/common/thread.py` & `starrail-toolkit-0.7.0/starrail/gui/common/thread.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/common/utils.py` & `starrail-toolkit-0.7.0/starrail/gui/common/utils.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.7.0/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.7.0/starrail/gui/interfaces/gacha_sync.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.7.0/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.7.0/starrail/gui/interfaces/setting.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/interfaces/unlock_fps.py` & `starrail-toolkit-0.7.0/starrail/gui/interfaces/unlock_fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/interfaces/users.py` & `starrail-toolkit-0.7.0/starrail/gui/interfaces/users.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.7.0/starrail/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.7.0/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/widgets/pie_chart.py` & `starrail-toolkit-0.7.0/starrail/gui/widgets/pie_chart.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.7.0/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/unlock/fps.py` & `starrail-toolkit-0.7.0/starrail/unlock/fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/utils/accounts.py` & `starrail-toolkit-0.7.0/starrail/utils/accounts.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/utils/auto_update.py` & `starrail-toolkit-0.7.0/starrail/utils/auto_update.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.7.0/starrail/utils/babelfish/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 ui_3star_light_cone = dictionary.ui_3star_light_cone
 ui_4star_character = dictionary.ui_4star_character
 ui_4star_light_cone = dictionary.ui_4star_light_cone
 ui_5star_character = dictionary.ui_5star_character
 ui_5star_light_cone = dictionary.ui_5star_light_cone
 ui_about = dictionary.ui_about
 ui_about_this = dictionary.ui_about_this
+ui_announcements = dictionary.ui_announcements
+ui_announcements_desc = dictionary.ui_announcements_desc
 ui_arerage_warps_per_5star = dictionary.ui_arerage_warps_per_5star
 ui_auto = dictionary.ui_auto
 ui_average_warps_per_up = dictionary.ui_average_warps_per_up
 ui_cancel_update = dictionary.ui_cancel_update
 ui_check_update = dictionary.ui_check_update
 ui_check_update_at_start = dictionary.ui_check_update_at_start
 ui_check_update_at_start_desc = dictionary.ui_check_update_at_start_desc
```

### Comparing `starrail-toolkit-0.6.9/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.7.0/starrail/utils/babelfish/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,22 @@
 ui_3star_light_cone = _MS(en='Light Cone (3)', zhs='三星光锥')
 ui_4star_character = _MS(en='Character (4)', zhs='四星角色')
 ui_4star_light_cone = _MS(en='Light Cone (4)', zhs='四星光锥')
 ui_5star_character = _MS(en='Character (5)', zhs='五星角色')
 ui_5star_light_cone = _MS(en='Light Cone (5)', zhs='五星光锥')
 ui_about = _MS(en='About', zhs='关于')
 ui_about_this = _MS(en='About This Application', zhs='关于本软件')
+ui_announcements = _MS(
+    en='Announcements',
+    zhs='通知公告',
+)
+ui_announcements_desc = _MS(
+    en='The latest news about Honkai: Star Rail.',
+    zhs='有关星穹铁道的最新消息',
+)
 ui_arerage_warps_per_5star = _MS(
     en='Average warps per 5 star',
     zhs='五星平均抽数',
 )
 ui_auto = _MS(en='Auto', zhs='跟随系统设置')
 ui_average_warps_per_up = _MS(
     en='Average warps per up',
```

### Comparing `starrail-toolkit-0.6.9/starrail/utils/babelfish/locale.py` & `starrail-toolkit-0.7.0/starrail/utils/babelfish/locale.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.7.0/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail/utils/loggings.py` & `starrail-toolkit-0.7.0/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.9/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.7.0/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.6.9
+Version: 0.7.0
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,28 +17,27 @@
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
 ## 开发状态
 
+**近期考试&其他事情比较忙，更新延缓一周（自2023.6.12起）左右**
+
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.9    |    0.6.9     |   0.6.9   |   0.6.9    |
+|   0.6.9    |    0.7.0     |   0.7.0   |   0.6.9    |
 
-目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
+目前大部分计划中的 feature 已实现完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
-- [x] 支持更多的可设置选项
-- [x] 支持解锁120帧
-- [x] 支持以 SRGF 标准导出
-- [x] 支持以 SRGF 标准导入
-- [x] 支持手动设置 API URL
-- [x] 支持夜间模式
-- [x] 支持多用户切换
-- [x] 美化程序界面
+- [x] 获取官方公告
+- [ ] 支持配置 SToken 用于抽卡导出
+- [ ] 支持 UP 池计算
+- [ ] 开拓月历
+- [ ] 米游社信息相关
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
```

### Comparing `starrail-toolkit-0.6.9/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.7.0/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,31 +24,35 @@
 starrail/gui/common/__init__.py
 starrail/gui/common/config.py
 starrail/gui/common/icon.py
 starrail/gui/common/stylesheet.py
 starrail/gui/common/thread.py
 starrail/gui/common/utils.py
 starrail/gui/interfaces/__init__.py
+starrail/gui/interfaces/announcements.py
 starrail/gui/interfaces/base.py
 starrail/gui/interfaces/gacha_sync.py
 starrail/gui/interfaces/home.py
 starrail/gui/interfaces/setting.py
 starrail/gui/interfaces/unlock_fps.py
 starrail/gui/interfaces/users.py
 starrail/gui/widgets/__init__.py
 starrail/gui/widgets/dialog.py
 starrail/gui/widgets/link_card.py
 starrail/gui/widgets/pie_chart.py
 starrail/gui/widgets/title_bar.py
+starrail/mihoyo/__init__.py
+starrail/mihoyo/api.py
 starrail/unlock/__init__.py
 starrail/unlock/fps.py
 starrail/unlock/service.py
 starrail/utils/__init__.py
 starrail/utils/accounts.py
 starrail/utils/auto_update.py
+starrail/utils/download.py
 starrail/utils/loggings.py
 starrail/utils/misc.py
 starrail/utils/babelfish/__init__.py
 starrail/utils/babelfish/constants.py
 starrail/utils/babelfish/dictionary.py
 starrail/utils/babelfish/locale.py
 starrail/utils/babelfish/multilingual.py
```

