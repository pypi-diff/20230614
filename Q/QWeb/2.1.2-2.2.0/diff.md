# Comparing `tmp/QWeb-2.1.2.tar.gz` & `tmp/QWeb-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QWeb-2.1.2.tar", last modified: Thu Mar 23 15:22:26 2023, max compression
+gzip compressed data, was "QWeb-2.2.0.tar", last modified: Wed Jun 14 07:39:39 2023, max compression
```

## Comparing `QWeb-2.1.2.tar` & `QWeb-2.2.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 15:22:26.374562 QWeb-2.1.2/
--rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-2.1.2/LICENSE
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    10191 2023-03-23 15:22:26.375560 QWeb-2.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-23 15:22:26.385115 QWeb-2.1.2/QWeb/
--rw-rw-rw-   0        0        0     6450 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/__init__.py
--rw-rw-rw-   0        0        0     2267 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/__main__.py
--rw-rw-rw-   0        0        0      519 2023-03-23 15:22:26.386130 QWeb-2.1.2/QWeb/_version.py
--rw-rw-rw-   0        0        0      905 2022-10-17 07:43:06.000000 QWeb-2.1.2/QWeb/config.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:22:26.141006 QWeb-2.1.2/QWeb/internal/
--rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-2.1.2/QWeb/internal/__init__.py
--rw-rw-rw-   0        0        0    21882 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/actions.py
--rw-rw-rw-   0        0        0     3840 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/ajax.py
--rw-rw-rw-   0        0        0     1699 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/alert.py
--rw-rw-rw-   0        0        0     3689 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/blocks.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:22:26.188095 QWeb-2.1.2/QWeb/internal/browser/
--rw-rw-rw-   0        0        0     5495 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/browser/__init__.py
--rw-rw-rw-   0        0        0     1446 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/browser/android.py
--rw-rw-rw-   0        0        0     2626 2022-06-23 10:57:52.000000 QWeb-2.1.2/QWeb/internal/browser/bs_desktop.py
--rw-rw-rw-   0        0        0     1716 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/browser/bs_mobile.py
--rw-rw-rw-   0        0        0     5889 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/internal/browser/chrome.py
--rw-rw-rw-   0        0        0     4277 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/internal/browser/edge.py
--rw-rw-rw-   0        0        0     5140 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/internal/browser/firefox.py
--rw-rw-rw-   0        0        0     1888 2022-11-23 07:04:05.000000 QWeb-2.1.2/QWeb/internal/browser/ie.py
--rw-rw-rw-   0        0        0     1077 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/browser/safari.py
--rw-rw-rw-   0        0        0     6626 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/checkbox.py
--rw-rw-rw-   0        0        0     4118 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/config.py
--rw-rw-rw-   0        0        0     4379 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/config_defaults.py
--rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/cookies.py
--rw-rw-rw-   0        0        0     9085 2022-12-12 08:01:37.000000 QWeb-2.1.2/QWeb/internal/decorators.py
--rw-rw-rw-   0        0        0     5294 2022-12-02 06:15:00.000000 QWeb-2.1.2/QWeb/internal/download.py
--rw-rw-rw-   0        0        0     3241 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/dragdrop.py
--rw-rw-rw-   0        0        0     7808 2022-12-12 14:30:56.000000 QWeb-2.1.2/QWeb/internal/dropdown.py
--rw-rw-rw-   0        0        0    28249 2022-12-16 14:12:34.000000 QWeb-2.1.2/QWeb/internal/element.py
--rw-rw-rw-   0        0        0     3087 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/exceptions.py
--rw-rw-rw-   0        0        0     3463 2022-12-09 08:03:29.000000 QWeb-2.1.2/QWeb/internal/file.py
--rw-rw-rw-   0        0        0    11767 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/frame.py
--rw-rw-rw-   0        0        0     1960 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/internal/frame_checker.py
--rw-rw-rw-   0        0        0    20231 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/icon.py
--rw-rw-rw-   0        0        0    10703 2022-12-12 14:30:56.000000 QWeb-2.1.2/QWeb/internal/input_.py
--rw-rw-rw-   0        0        0     7244 2023-03-23 15:17:25.000000 QWeb-2.1.2/QWeb/internal/input_handler.py
--rw-rw-rw-   0        0        0    21040 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/internal/javascript.py
--rw-rw-rw-   0        0        0     9479 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/lists.py
--rw-rw-rw-   0        0        0     3194 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/meas.py
--rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-2.1.2/QWeb/internal/platform.py
--rw-rw-rw-   0        0        0    13330 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/screenshot.py
--rw-rw-rw-   0        0        0     6850 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/internal/search_strategy.py
--rw-rw-rw-   0        0        0     5531 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/internal/secrets.py
--rw-rw-rw-   0        0        0    15645 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/internal/table.py
--rw-rw-rw-   0        0        0    16851 2023-03-16 07:45:30.000000 QWeb-2.1.2/QWeb/internal/text.py
--rw-rw-rw-   0        0        0     1411 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/internal/user.py
--rw-rw-rw-   0        0        0    12833 2023-03-08 07:11:26.000000 QWeb-2.1.2/QWeb/internal/util.py
--rw-rw-rw-   0        0        0     4423 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/internal/window.py
--rw-rw-rw-   0        0        0     3321 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/internal/xhr.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:22:26.367524 QWeb-2.1.2/QWeb/keywords/
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.1.2/QWeb/keywords/__init__.py
--rw-rw-rw-   0        0        0     4238 2022-12-09 08:03:37.000000 QWeb-2.1.2/QWeb/keywords/ajax.py
--rw-rw-rw-   0        0        0     4920 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/alert.py
--rw-rw-rw-   0        0        0     5778 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/blocks.py
--rw-rw-rw-   0        0        0    18536 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/keywords/browser.py
--rw-rw-rw-   0        0        0    12960 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/checkbox.py
--rw-rw-rw-   0        0        0    36464 2023-03-23 15:17:25.000000 QWeb-2.1.2/QWeb/keywords/config.py
--rw-rw-rw-   0        0        0     2846 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/keywords/cookies.py
--rw-rw-rw-   0        0        0     2500 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/debug.py
--rw-rw-rw-   0        0        0     3998 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/download.py
--rw-rw-rw-   0        0        0     6268 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/keywords/dragdrop.py
--rw-rw-rw-   0        0        0    14590 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/dropdown.py
--rw-rw-rw-   0        0        0    27613 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/keywords/element.py
--rw-rw-rw-   0        0        0    12453 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/keywords/file.py
--rw-rw-rw-   0        0        0     4612 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/frame.py
--rw-rw-rw-   0        0        0     8675 2023-03-23 15:17:25.000000 QWeb-2.1.2/QWeb/keywords/icon.py
--rw-rw-rw-   0        0        0    35783 2023-02-03 08:50:04.000000 QWeb-2.1.2/QWeb/keywords/input_.py
--rw-rw-rw-   0        0        0     1908 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/javascript.py
--rw-rw-rw-   0        0        0     8703 2022-11-21 09:35:10.000000 QWeb-2.1.2/QWeb/keywords/lists.py
--rw-rw-rw-   0        0        0     2967 2022-06-23 10:57:52.000000 QWeb-2.1.2/QWeb/keywords/screenshot.py
--rw-rw-rw-   0        0        0     8486 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/search_strategy.py
--rw-rw-rw-   0        0        0    11958 2022-11-22 10:56:24.000000 QWeb-2.1.2/QWeb/keywords/table.py
--rw-rw-rw-   0        0        0    66393 2022-09-07 11:01:14.000000 QWeb-2.1.2/QWeb/keywords/text.py
--rw-rw-rw-   0        0        0    17540 2022-06-16 12:12:07.000000 QWeb-2.1.2/QWeb/keywords/window.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:22:25.968157 QWeb-2.1.2/QWeb.egg-info/
--rw-rw-rw-   0        0        0    10191 2023-03-23 15:22:25.000000 QWeb-2.1.2/QWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2039 2023-03-23 15:22:25.000000 QWeb-2.1.2/QWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 15:22:25.000000 QWeb-2.1.2/QWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-2.1.2/QWeb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      418 2023-03-23 15:22:25.000000 QWeb-2.1.2/QWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-23 15:22:25.000000 QWeb-2.1.2/QWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9400 2023-03-08 08:01:54.000000 QWeb-2.1.2/README.md
--rw-rw-rw-   0        0        0     1208 2023-03-23 15:22:26.382795 QWeb-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2663 2023-03-08 07:11:26.000000 QWeb-2.1.2/setup.py
--rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-2.1.2/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.150060 QWeb-2.2.0/
+-rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10191 2023-06-14 07:39:39.151056 QWeb-2.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.157669 QWeb-2.2.0/QWeb/
+-rw-rw-rw-   0        0        0     6450 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/__init__.py
+-rw-rw-rw-   0        0        0     2267 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/__main__.py
+-rw-rw-rw-   0        0        0      519 2023-06-14 07:39:39.159663 QWeb-2.2.0/QWeb/_version.py
+-rw-rw-rw-   0        0        0      905 2022-10-17 07:43:06.000000 QWeb-2.2.0/QWeb/config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.065395 QWeb-2.2.0/QWeb/internal/
+-rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-2.2.0/QWeb/internal/__init__.py
+-rw-rw-rw-   0        0        0    21882 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/actions.py
+-rw-rw-rw-   0        0        0     3840 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/ajax.py
+-rw-rw-rw-   0        0        0     1699 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/alert.py
+-rw-rw-rw-   0        0        0     3689 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/blocks.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.088005 QWeb-2.2.0/QWeb/internal/browser/
+-rw-rw-rw-   0        0        0     5495 2023-04-26 08:15:55.000000 QWeb-2.2.0/QWeb/internal/browser/__init__.py
+-rw-rw-rw-   0        0        0     1446 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/browser/android.py
+-rw-rw-rw-   0        0        0     2626 2022-06-23 10:57:52.000000 QWeb-2.2.0/QWeb/internal/browser/bs_desktop.py
+-rw-rw-rw-   0        0        0     1716 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/browser/bs_mobile.py
+-rw-rw-rw-   0        0        0     5889 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/browser/chrome.py
+-rw-rw-rw-   0        0        0     4277 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/browser/edge.py
+-rw-rw-rw-   0        0        0     5140 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/browser/firefox.py
+-rw-rw-rw-   0        0        0     1888 2022-11-23 07:04:05.000000 QWeb-2.2.0/QWeb/internal/browser/ie.py
+-rw-rw-rw-   0        0        0     1077 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/browser/safari.py
+-rw-rw-rw-   0        0        0     6626 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/checkbox.py
+-rw-rw-rw-   0        0        0     4118 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/config.py
+-rw-rw-rw-   0        0        0     4379 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/config_defaults.py
+-rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/cookies.py
+-rw-rw-rw-   0        0        0     9341 2023-06-12 09:33:39.000000 QWeb-2.2.0/QWeb/internal/decorators.py
+-rw-rw-rw-   0        0        0     5294 2022-12-02 06:15:00.000000 QWeb-2.2.0/QWeb/internal/download.py
+-rw-rw-rw-   0        0        0     3241 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/dragdrop.py
+-rw-rw-rw-   0        0        0     7808 2022-12-12 14:30:56.000000 QWeb-2.2.0/QWeb/internal/dropdown.py
+-rw-rw-rw-   0        0        0    28249 2022-12-16 14:12:34.000000 QWeb-2.2.0/QWeb/internal/element.py
+-rw-rw-rw-   0        0        0     3087 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/exceptions.py
+-rw-rw-rw-   0        0        0     3463 2022-12-09 08:03:29.000000 QWeb-2.2.0/QWeb/internal/file.py
+-rw-rw-rw-   0        0        0    11767 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/frame.py
+-rw-rw-rw-   0        0        0     1960 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/frame_checker.py
+-rw-rw-rw-   0        0        0    20231 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/icon.py
+-rw-rw-rw-   0        0        0    10703 2022-12-12 14:30:56.000000 QWeb-2.2.0/QWeb/internal/input_.py
+-rw-rw-rw-   0        0        0     7244 2023-03-23 15:17:25.000000 QWeb-2.2.0/QWeb/internal/input_handler.py
+-rw-rw-rw-   0        0        0    21040 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/javascript.py
+-rw-rw-rw-   0        0        0     9479 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/lists.py
+-rw-rw-rw-   0        0        0     3194 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/meas.py
+-rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/platform.py
+-rw-rw-rw-   0        0        0    13379 2023-06-06 09:19:52.000000 QWeb-2.2.0/QWeb/internal/screenshot.py
+-rw-rw-rw-   0        0        0     6850 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/search_strategy.py
+-rw-rw-rw-   0        0        0     5531 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/secrets.py
+-rw-rw-rw-   0        0        0    15645 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/table.py
+-rw-rw-rw-   0        0        0    16851 2023-03-16 07:45:30.000000 QWeb-2.2.0/QWeb/internal/text.py
+-rw-rw-rw-   0        0        0     1411 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/user.py
+-rw-rw-rw-   0        0        0    12833 2023-03-08 07:11:26.000000 QWeb-2.2.0/QWeb/internal/util.py
+-rw-rw-rw-   0        0        0     4423 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/window.py
+-rw-rw-rw-   0        0        0     3321 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/xhr.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.148055 QWeb-2.2.0/QWeb/keywords/
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.2.0/QWeb/keywords/__init__.py
+-rw-rw-rw-   0        0        0     4238 2022-12-09 08:03:37.000000 QWeb-2.2.0/QWeb/keywords/ajax.py
+-rw-rw-rw-   0        0        0     4920 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/alert.py
+-rw-rw-rw-   0        0        0     5778 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/blocks.py
+-rw-rw-rw-   0        0        0    18536 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/keywords/browser.py
+-rw-rw-rw-   0        0        0    12960 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/checkbox.py
+-rw-rw-rw-   0        0        0    36464 2023-03-23 15:17:25.000000 QWeb-2.2.0/QWeb/keywords/config.py
+-rw-rw-rw-   0        0        0     2846 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/cookies.py
+-rw-rw-rw-   0        0        0     2500 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/debug.py
+-rw-rw-rw-   0        0        0     3998 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/download.py
+-rw-rw-rw-   0        0        0     6268 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/dragdrop.py
+-rw-rw-rw-   0        0        0    14590 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/dropdown.py
+-rw-rw-rw-   0        0        0    27613 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/element.py
+-rw-rw-rw-   0        0        0    12453 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/keywords/file.py
+-rw-rw-rw-   0        0        0     4612 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/frame.py
+-rw-rw-rw-   0        0        0     8675 2023-03-23 15:17:25.000000 QWeb-2.2.0/QWeb/keywords/icon.py
+-rw-rw-rw-   0        0        0    38042 2023-06-12 09:33:39.000000 QWeb-2.2.0/QWeb/keywords/input_.py
+-rw-rw-rw-   0        0        0     1908 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/javascript.py
+-rw-rw-rw-   0        0        0     8703 2022-11-21 09:35:10.000000 QWeb-2.2.0/QWeb/keywords/lists.py
+-rw-rw-rw-   0        0        0     2967 2022-06-23 10:57:52.000000 QWeb-2.2.0/QWeb/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     8486 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/search_strategy.py
+-rw-rw-rw-   0        0        0    11958 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/table.py
+-rw-rw-rw-   0        0        0    66393 2022-09-07 11:01:14.000000 QWeb-2.2.0/QWeb/keywords/text.py
+-rw-rw-rw-   0        0        0    17540 2023-06-07 09:41:10.000000 QWeb-2.2.0/QWeb/keywords/window.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:39:38.965558 QWeb-2.2.0/QWeb.egg-info/
+-rw-rw-rw-   0        0        0    10191 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2039 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-2.2.0/QWeb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      418 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9400 2023-03-08 08:01:54.000000 QWeb-2.2.0/README.md
+-rw-rw-rw-   0        0        0     1208 2023-06-14 07:39:39.156056 QWeb-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2663 2023-06-14 07:12:14.000000 QWeb-2.2.0/setup.py
+-rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-2.2.0/versioneer.py
```

### Comparing `QWeb-2.1.2/LICENSE` & `QWeb-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/PKG-INFO` & `QWeb-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 2.1.2
+Version: 2.2.0
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `QWeb-2.1.2/QWeb/__init__.py` & `QWeb-2.2.0/QWeb/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/__main__.py` & `QWeb-2.2.0/QWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/config.py` & `QWeb-2.2.0/QWeb/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/actions.py` & `QWeb-2.2.0/QWeb/internal/actions.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/ajax.py` & `QWeb-2.2.0/QWeb/internal/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/alert.py` & `QWeb-2.2.0/QWeb/internal/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/blocks.py` & `QWeb-2.2.0/QWeb/internal/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/__init__.py` & `QWeb-2.2.0/QWeb/internal/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/android.py` & `QWeb-2.2.0/QWeb/internal/browser/android.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/bs_desktop.py` & `QWeb-2.2.0/QWeb/internal/browser/bs_desktop.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/bs_mobile.py` & `QWeb-2.2.0/QWeb/internal/browser/bs_mobile.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/chrome.py` & `QWeb-2.2.0/QWeb/internal/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/edge.py` & `QWeb-2.2.0/QWeb/internal/browser/edge.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/firefox.py` & `QWeb-2.2.0/QWeb/internal/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/ie.py` & `QWeb-2.2.0/QWeb/internal/browser/ie.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/browser/safari.py` & `QWeb-2.2.0/QWeb/internal/browser/safari.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/checkbox.py` & `QWeb-2.2.0/QWeb/internal/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/config.py` & `QWeb-2.2.0/QWeb/internal/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/config_defaults.py` & `QWeb-2.2.0/QWeb/internal/config_defaults.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/cookies.py` & `QWeb-2.2.0/QWeb/internal/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/decorators.py` & `QWeb-2.2.0/QWeb/internal/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,198 +1,199 @@
-# -*- coding: utf-8 -*-
-# --------------------------
-# Copyright © 2014 -            Qentinel Group.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ---------------------------
-from __future__ import annotations
-from types import MappingProxyType
-from typing import Callable, Any, Union
-
-import time
-from inspect import signature
-from functools import wraps
-from robot.utils import timestr_to_secs
-from robot.api import logger
-from selenium.common.exceptions import InvalidSelectorException, \
-    NoSuchElementException, StaleElementReferenceException, WebDriverException, \
-    UnexpectedAlertPresentException, InvalidSessionIdException
-from QWeb.keywords import config
-from QWeb.internal import frame
-from QWeb.internal.config_defaults import CONFIG, SHORT_DELAY, LONG_DELAY
-from QWeb.internal.exceptions import QWebElementNotFoundError, \
-    QWebStalingElementError, QWebDriverError, QWebTimeoutError, QWebValueError, \
-    QWebUnexpectedConditionError, QWebValueMismatchError, QWebSearchingMode, QWebUnexpectedAlert, \
-    QWebIconNotFoundError, QWebBrowserError, FATAL_MESSAGES
-
-
-# pylint: disable=too-many-statements
-# pylint: disable=too-many-branches
-def timeout_decorator(fn: Callable[..., Any]) -> Callable[..., Any]:
-
-    @wraps(fn)
-    def get_elements_from_dom_content(  # type: ignore[return] # pylint: disable=R1710
-            *args: Any, **kwargs: Any) -> Union[Callable[..., Any], int, bool, None]:
-        try:
-            args, kwargs, locator = _equal_sign_handler(args, kwargs, fn)
-            msg: Union[WebDriverException, QWebDriverError, QWebValueError, None] = None
-            params = signature(fn).parameters
-            args, kwargs = _args_to_kwargs(params, args, kwargs)
-            timeout = get_timeout(**kwargs)
-            logger.debug('Timeout is {} sec'.format(timeout))
-
-            try:
-                if 'go_to' not in str(fn) and 'switch_window' not in str(fn):
-                    frame.wait_page_loaded()
-            except UnexpectedAlertPresentException as e:
-                if not CONFIG["HandleAlerts"]:
-                    raise QWebUnexpectedAlert(str(e)) from e
-                logger.debug('Got {}. Trying to retry..'.format(e))
-                time.sleep(SHORT_DELAY)
-            start = time.time()
-            while time.time() < timeout + start:
-                try:
-                    kwargs['timeout'] = float(timeout + start - time.time())
-                    config.set_config('FrameTimeout', float(timeout + start - time.time()))
-                    return fn(*args, **kwargs)
-                except (QWebUnexpectedConditionError, QWebTimeoutError) as e:
-                    logger.debug('Got {}'.format(e))
-                except (InvalidSelectorException, NoSuchElementException, QWebElementNotFoundError,
-                        UnexpectedAlertPresentException, QWebStalingElementError,
-                        StaleElementReferenceException, QWebIconNotFoundError) as e:
-                    time.sleep(SHORT_DELAY)
-                    logger.debug('Got exception: {}. Trying to retry..'.format(e))
-                except InvalidSessionIdException as e:
-                    CONFIG.set_value("OSScreenshots", True)
-                    raise QWebBrowserError("Browser session lost. Did browser crash?") from e
-                except (WebDriverException, QWebDriverError) as e:
-                    if any(s in str(e) for s in FATAL_MESSAGES):
-                        CONFIG.set_value("OSScreenshots", True)
-                        raise QWebBrowserError(e)  # pylint: disable=W0707
-                    logger.debug('From timeout decorator: Webdriver exception. Retrying..')
-                    logger.debug(e)
-                    time.sleep(SHORT_DELAY)
-                    err = QWebDriverError
-                    msg = e
-                except QWebValueError as ve:
-                    logger.debug('Got QWebValueError: {}. Trying to retry..'.format(ve))
-                    err = QWebValueError  # type: ignore[assignment]
-                    msg = ve
-                    time.sleep(SHORT_DELAY)
-            if msg:
-                raise err(msg)
-            if 'count' in str(fn):
-                return 0
-            if 'is_text' in str(fn) or 'is_no_text' in str(fn):
-                return False
-            raise QWebElementNotFoundError('Unable to find element for locator {} in {} sec'.format(
-                locator, timeout))
-        except QWebSearchingMode:
-            pass
-
-    return get_elements_from_dom_content
-
-
-def timeout_decorator_for_actions(fn: Callable[..., Any]) -> Callable[..., Any]:
-
-    @wraps(fn)
-    def perform(*args: Any, **kwargs: Any) -> Callable[..., Any]:
-        params = signature(fn).parameters
-        args, kwargs = _args_to_kwargs(params, args, kwargs)
-        timeout = get_timeout(**kwargs)
-        err = None
-        msg = None
-        performed = False
-        logger.debug('time to run {}'.format(timeout))
-        start = time.time()
-        while time.time() < timeout + start:
-            try:
-                return fn(*args, **kwargs)
-            except QWebValueMismatchError as mismatch:
-                if 'text_appearance' not in str(fn) and 'get_or_compare_text' not in str(fn):
-                    err = QWebValueError
-                    msg = mismatch
-                logger.trace('Value mismatch: {}'.format(mismatch))
-                continue
-            except (QWebElementNotFoundError, UnexpectedAlertPresentException):
-                logger.debug('Not found')
-                time.sleep(SHORT_DELAY)
-            except QWebValueError as ve:
-                if performed:
-                    break
-                raise ve
-            except (QWebStalingElementError, StaleElementReferenceException) as S:
-                if 'execute_click' in str(fn) or 'text_appearance' in str(fn):
-                    logger.debug('Got staling element err from retry click.'
-                                 'Action is probably triggered.')
-                    raise QWebUnexpectedConditionError(S)  # pylint: disable=W0707
-                raise QWebStalingElementError('Staling element')  # pylint: disable=W0707
-            except (WebDriverException, QWebDriverError) as wde:
-                if 'alert' in str(fn):
-                    time.sleep(LONG_DELAY)
-                    logger.debug("Got webdriver exception..{}. Retrying..".format(wde))
-                    err = QWebDriverError  # type: ignore[assignment]
-                    msg = wde  # type: ignore[assignment]
-                else:
-                    raise QWebDriverError(wde)  # pylint: disable=W0707
-        if msg:
-            raise err(msg)  # type: ignore[misc]
-        raise QWebTimeoutError('Timeout exceeded')
-
-    return perform
-
-
-def get_timeout(**kwargs: Any) -> Union[int, float]:
-    timeout = timestr_to_secs(CONFIG["DefaultTimeout"])
-    if 'timeout' in kwargs:
-        if timestr_to_secs(kwargs['timeout']) != 0:
-            timeout = timestr_to_secs(kwargs['timeout'])
-    return timeout
-
-
-def _args_to_kwargs(params: MappingProxyType[str, Any], args: tuple,
-                    kwargs: dict) -> tuple[tuple, dict]:
-    if 'timeout' not in kwargs:
-        for i, p in enumerate(params.values()):
-            if p.name not in kwargs:
-                if len(args) > i:
-                    kwargs[p.name] = args[i]
-                else:
-                    kwargs[p.name] = p.default
-        args = tuple('')
-    return tuple(args), kwargs
-
-
-def _equal_sign_handler(args: Union[tuple, list], kwargs: dict,
-                        function_name: Union[str, Callable[..., Any]]) -> tuple[tuple, dict, str]:
-    try:
-        locator = args[0]
-    except IndexError:
-        for key, value in kwargs.items():
-            # if present any of these is always the first argument
-            # locator can be the 2nd arg but it is handled later on
-            if key in ('locator', 'xpath', 'steps', 'image', 'input_texts', 'input_values', 'text',
-                       'coordinates', 'texts_to_verify', 'url', 'title'):
-                locator = value
-                break
-        else:
-            # index can be unnamed first argument or named argument
-            locator = kwargs.get('index', None)
-
-        # The only decorated method with 'locator' as NOT the first argument
-        if str(function_name) == "scroll_to":
-            locator = kwargs.get('text_to_find', None)
-
-    if locator is None:
-        logger.console(f"args: {args}, \nkwargs: {kwargs}")
-        raise QWebElementNotFoundError("Use \\= instead of = in xpaths")
-    return tuple(args), kwargs, locator
+# -*- coding: utf-8 -*-
+# --------------------------
+# Copyright © 2014 -            Qentinel Group.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ---------------------------
+from __future__ import annotations
+from types import MappingProxyType
+from typing import Callable, Any, Union
+
+import time
+from inspect import signature
+from functools import wraps
+from robot.utils import timestr_to_secs
+from robot.api import logger
+from selenium.common.exceptions import InvalidSelectorException, \
+    NoSuchElementException, StaleElementReferenceException, WebDriverException, \
+    UnexpectedAlertPresentException, InvalidSessionIdException
+from QWeb.keywords import config
+from QWeb.internal import frame
+from QWeb.internal.config_defaults import CONFIG, SHORT_DELAY, LONG_DELAY
+from QWeb.internal.exceptions import QWebElementNotFoundError, \
+    QWebStalingElementError, QWebDriverError, QWebTimeoutError, QWebValueError, \
+    QWebUnexpectedConditionError, QWebValueMismatchError, QWebSearchingMode, QWebUnexpectedAlert, \
+    QWebIconNotFoundError, QWebBrowserError, FATAL_MESSAGES
+
+
+# pylint: disable=too-many-statements
+# pylint: disable=too-many-branches
+def timeout_decorator(fn: Callable[..., Any]) -> Callable[..., Any]:
+
+    @wraps(fn)
+    def get_elements_from_dom_content(  # type: ignore[return] # pylint: disable=R1710
+            *args: Any, **kwargs: Any) -> Union[Callable[..., Any], int, bool, None]:
+        try:
+            args, kwargs, locator = _equal_sign_handler(args, kwargs, fn)
+            msg: Union[WebDriverException, QWebDriverError, QWebValueError, None] = None
+            params = signature(fn).parameters
+            args, kwargs = _args_to_kwargs(params, args, kwargs)
+            timeout = get_timeout(**kwargs)
+            logger.debug('Timeout is {} sec'.format(timeout))
+
+            try:
+                if 'go_to' not in str(fn) and 'switch_window' not in str(fn):
+                    frame.wait_page_loaded()
+            except UnexpectedAlertPresentException as e:
+                if not CONFIG["HandleAlerts"]:
+                    raise QWebUnexpectedAlert(str(e)) from e
+                logger.debug('Got {}. Trying to retry..'.format(e))
+                time.sleep(SHORT_DELAY)
+            start = time.time()
+            while time.time() < timeout + start:
+                try:
+                    kwargs['timeout'] = float(timeout + start - time.time())
+                    config.set_config('FrameTimeout', float(timeout + start - time.time()))
+                    return fn(*args, **kwargs)
+                except (QWebUnexpectedConditionError, QWebTimeoutError) as e:
+                    logger.debug('Got {}'.format(e))
+                except (InvalidSelectorException, NoSuchElementException, QWebElementNotFoundError,
+                        UnexpectedAlertPresentException, QWebStalingElementError,
+                        StaleElementReferenceException, QWebIconNotFoundError) as e:
+                    time.sleep(SHORT_DELAY)
+                    logger.debug('Got exception: {}. Trying to retry..'.format(e))
+                except InvalidSessionIdException as e:
+                    CONFIG.set_value("OSScreenshots", True)
+                    raise QWebBrowserError("Browser session lost. Did browser crash?") from e
+                except (WebDriverException, QWebDriverError) as e:
+                    if any(s in str(e) for s in FATAL_MESSAGES):
+                        CONFIG.set_value("OSScreenshots", True)
+                        raise QWebBrowserError(e)  # pylint: disable=W0707
+                    logger.debug('From timeout decorator: Webdriver exception. Retrying..')
+                    logger.debug(e)
+                    time.sleep(SHORT_DELAY)
+                    err = QWebDriverError
+                    msg = e
+                except QWebValueError as ve:
+                    logger.debug('Got QWebValueError: {}. Trying to retry..'.format(ve))
+                    err = QWebValueError  # type: ignore[assignment]
+                    msg = ve
+                    time.sleep(SHORT_DELAY)
+            if msg:
+                # pylint: disable=used-before-assignment
+                raise err(msg)
+            if 'count' in str(fn):
+                return 0
+            if 'is_text' in str(fn) or 'is_no_text' in str(fn):
+                return False
+            raise QWebElementNotFoundError('Unable to find element for locator {} in {} sec'.format(
+                locator, timeout))
+        except QWebSearchingMode:
+            pass
+
+    return get_elements_from_dom_content
+
+
+def timeout_decorator_for_actions(fn: Callable[..., Any]) -> Callable[..., Any]:
+
+    @wraps(fn)
+    def perform(*args: Any, **kwargs: Any) -> Callable[..., Any]:
+        params = signature(fn).parameters
+        args, kwargs = _args_to_kwargs(params, args, kwargs)
+        timeout = get_timeout(**kwargs)
+        err = None
+        msg = None
+        performed = False
+        logger.debug('time to run {}'.format(timeout))
+        start = time.time()
+        while time.time() < timeout + start:
+            try:
+                return fn(*args, **kwargs)
+            except QWebValueMismatchError as mismatch:
+                if 'text_appearance' not in str(fn) and 'get_or_compare_text' not in str(fn):
+                    err = QWebValueError
+                    msg = mismatch
+                logger.trace('Value mismatch: {}'.format(mismatch))
+                continue
+            except (QWebElementNotFoundError, UnexpectedAlertPresentException):
+                logger.debug('Not found')
+                time.sleep(SHORT_DELAY)
+            except QWebValueError as ve:
+                if performed:
+                    break
+                raise ve
+            except (QWebStalingElementError, StaleElementReferenceException) as S:
+                if 'execute_click' in str(fn) or 'text_appearance' in str(fn):
+                    logger.debug('Got staling element err from retry click.'
+                                 'Action is probably triggered.')
+                    raise QWebUnexpectedConditionError(S)  # pylint: disable=W0707
+                raise QWebStalingElementError('Staling element')  # pylint: disable=W0707
+            except (WebDriverException, QWebDriverError) as wde:
+                if 'alert' in str(fn):
+                    time.sleep(LONG_DELAY)
+                    logger.debug("Got webdriver exception..{}. Retrying..".format(wde))
+                    err = QWebDriverError  # type: ignore[assignment]
+                    msg = wde  # type: ignore[assignment]
+                else:
+                    raise QWebDriverError(wde)  # pylint: disable=W0707
+        if msg:
+            raise err(msg)  # type: ignore[misc]
+        raise QWebTimeoutError('Timeout exceeded')
+
+    return perform
+
+
+def get_timeout(**kwargs: Any) -> Union[int, float]:
+    timeout = timestr_to_secs(CONFIG["DefaultTimeout"])
+    if 'timeout' in kwargs:
+        if timestr_to_secs(kwargs['timeout']) != 0:
+            timeout = timestr_to_secs(kwargs['timeout'])
+    return timeout
+
+
+def _args_to_kwargs(params: MappingProxyType[str, Any], args: tuple,
+                    kwargs: dict) -> tuple[tuple, dict]:
+    if 'timeout' not in kwargs:
+        for i, p in enumerate(params.values()):
+            if p.name not in kwargs:
+                if len(args) > i:
+                    kwargs[p.name] = args[i]
+                else:
+                    kwargs[p.name] = p.default
+        args = tuple('')
+    return tuple(args), kwargs
+
+
+def _equal_sign_handler(args: Union[tuple, list], kwargs: dict,
+                        function_name: Union[str, Callable[..., Any]]) -> tuple[tuple, dict, str]:
+    try:
+        locator = args[0]
+    except IndexError:
+        for key, value in kwargs.items():
+            # if present any of these is always the first argument
+            # locator can be the 2nd arg but it is handled later on
+            if key in ('locator', 'xpath', 'steps', 'image', 'input_texts', 'input_values', 'text',
+                       'coordinates', 'texts_to_verify', 'url', 'title'):
+                locator = value
+                break
+        else:
+            # index can be unnamed first argument or named argument
+            locator = kwargs.get('index', None)
+
+        # The only decorated method with 'locator' as NOT the first argument
+        if str(function_name) == "scroll_to":
+            locator = kwargs.get('text_to_find', None)
+
+    if locator is None:
+        logger.console(f"args: {args}, \nkwargs: {kwargs}")
+        raise QWebElementNotFoundError("Use \\= instead of = in xpaths")
+    return tuple(args), kwargs, locator
```

### Comparing `QWeb-2.1.2/QWeb/internal/download.py` & `QWeb-2.2.0/QWeb/internal/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/dragdrop.py` & `QWeb-2.2.0/QWeb/internal/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/dropdown.py` & `QWeb-2.2.0/QWeb/internal/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/element.py` & `QWeb-2.2.0/QWeb/internal/element.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/exceptions.py` & `QWeb-2.2.0/QWeb/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/file.py` & `QWeb-2.2.0/QWeb/internal/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/frame.py` & `QWeb-2.2.0/QWeb/internal/frame.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/frame_checker.py` & `QWeb-2.2.0/QWeb/internal/frame_checker.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/icon.py` & `QWeb-2.2.0/QWeb/internal/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/input_.py` & `QWeb-2.2.0/QWeb/internal/input_.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/input_handler.py` & `QWeb-2.2.0/QWeb/internal/input_handler.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/javascript.py` & `QWeb-2.2.0/QWeb/internal/javascript.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/lists.py` & `QWeb-2.2.0/QWeb/internal/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/meas.py` & `QWeb-2.2.0/QWeb/internal/meas.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/platform.py` & `QWeb-2.2.0/QWeb/internal/platform.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/screenshot.py` & `QWeb-2.2.0/QWeb/internal/screenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,28 +198,30 @@
     elif filename == 'screenshot_{}.png':
         name_with_underscores = str(test_name).replace(" ", "_")
         valid_name = _remove_invalid_chars(name_with_underscores)
         filename = "screenshot-" + valid_name + "-{}".format(uuid4()) + '.png'
 
     filepath = os.path.join(screen_shot_dir, filename)
 
+    try:
+        driver = browser.get_current_browser()
+    except QWebDriverError:
+        driver = None
+        config.set_config("OSScreenshots", True)
+
     if pyautog is True or config.get_config("OSScreenshots"):
         # try to remove image, needed for scrot > 0.9
         try:
             os.remove(filepath)
         except OSError:
             pass
 
         pyscreenshot(filepath)
         logger.info('Saved screenshot to {}'.format(filepath))
         return filepath
-    try:
-        driver = browser.get_current_browser()
-    except WebDriverException:
-        driver = None
 
     if driver:
         saved: Union[str, bool]
         try:
             browser_name = driver.capabilities['browserName']
             if not fullpage:
                 saved = driver.save_screenshot(filepath)
```

### Comparing `QWeb-2.1.2/QWeb/internal/search_strategy.py` & `QWeb-2.2.0/QWeb/internal/search_strategy.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/secrets.py` & `QWeb-2.2.0/QWeb/internal/secrets.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/table.py` & `QWeb-2.2.0/QWeb/internal/table.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/text.py` & `QWeb-2.2.0/QWeb/internal/text.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/user.py` & `QWeb-2.2.0/QWeb/internal/user.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/util.py` & `QWeb-2.2.0/QWeb/internal/util.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/window.py` & `QWeb-2.2.0/QWeb/internal/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/internal/xhr.py` & `QWeb-2.2.0/QWeb/internal/xhr.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/ajax.py` & `QWeb-2.2.0/QWeb/keywords/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/alert.py` & `QWeb-2.2.0/QWeb/keywords/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/blocks.py` & `QWeb-2.2.0/QWeb/keywords/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/browser.py` & `QWeb-2.2.0/QWeb/keywords/browser.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/checkbox.py` & `QWeb-2.2.0/QWeb/keywords/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/config.py` & `QWeb-2.2.0/QWeb/keywords/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/cookies.py` & `QWeb-2.2.0/QWeb/keywords/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/debug.py` & `QWeb-2.2.0/QWeb/keywords/debug.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/download.py` & `QWeb-2.2.0/QWeb/keywords/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/dragdrop.py` & `QWeb-2.2.0/QWeb/keywords/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/dropdown.py` & `QWeb-2.2.0/QWeb/keywords/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/element.py` & `QWeb-2.2.0/QWeb/keywords/element.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/file.py` & `QWeb-2.2.0/QWeb/keywords/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/frame.py` & `QWeb-2.2.0/QWeb/keywords/frame.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/icon.py` & `QWeb-2.2.0/QWeb/keywords/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/input_.py` & `QWeb-2.2.0/QWeb/keywords/input_.py`

 * *Files 2% similar despite different names*

```diff
@@ -820,7 +820,76 @@
                   .key_up(key[0]).perform()
         else:
             input_element.send_keys(key)
     except AttributeError as e:
         logger.console(e)
         raise QWebValueError('Could not find key "{}"'.format(key)) from e
     return None
+
+
+@keyword(tags=("Browser", "Interaction"))
+def scroll(locator: str,
+           direction: str = 'pagedown',
+           timeout: Union[int, float, str] = 0, **kwargs) -> None:
+    r"""Scrolls the page/element to given direction.
+
+    Examples
+    --------
+    .. code-block:: robotframework
+
+        # Scroll page down default value (one page)
+        Scroll  //html
+
+        # Scroll page up
+        Scroll  //html      page_up
+
+        # Scroll page right
+        Scroll  //html      right
+
+        # Scroll to the bottom of a list using attribute value and tag
+        Scroll  uiScroller    bottom    tag=div
+
+        # Scroll to the top of a list using attribute value and tag
+        Scroll  uiScroller    top    tag=div
+
+        # Scroll (page) down 3 times in a list
+        Repeat Keyword     3 times    Scroll    uiScroller   down    tag=div
+
+    Parameters
+    ----------
+    locator : str
+        Xpath to scrollable element or attribute value of an scrollable element.
+    direction : str
+        Direction to scroll to (down, up, left, right, top, bottom, page_down, page_up).
+          * Down/up/left/right map to respective ARROW keys.
+          * Top/Bottom map to HOME & END keys.
+          * Page_up/Page_down map to PAGE_UP and PAGE_DOWN keys.
+    timeout : int
+        How long to scroll in seconds, before timing out.
+
+    Raises
+    ------
+    QWebValueError
+        If direction is not given in correct format.
+    QWebElementNotFoundError
+        If the given scrollable element is not found.
+
+    Related keywords
+    ----------------
+    \`ScrollTo\`, \`ScrollText\`
+    """
+
+    keys = {"pagedown": "{PAGE_DOWN}",
+            "pageup": "{PAGE_UP}",
+            "top": "{HOME}",
+            "bottom": "{END}",
+            "up": "{ARROW_UP}",
+            "down": "{ARROW_DOWN}",
+            "left": "{ARROW_LEFT}",
+            "right": "{ARROW_RIGHT}"}
+
+    try:
+        key = keys[direction.lower().replace("_", "")]
+    except KeyError as e:
+        raise QWebValueError("""Unknown 'direction'. Valid values are: page_down,
+                             page_up, down, up, left, right, top, bottom""") from e
+    press_key(locator, key, timeout=timeout, **kwargs)
```

### Comparing `QWeb-2.1.2/QWeb/keywords/javascript.py` & `QWeb-2.2.0/QWeb/keywords/javascript.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/lists.py` & `QWeb-2.2.0/QWeb/keywords/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/screenshot.py` & `QWeb-2.2.0/QWeb/keywords/screenshot.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/search_strategy.py` & `QWeb-2.2.0/QWeb/keywords/search_strategy.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/table.py` & `QWeb-2.2.0/QWeb/keywords/table.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/text.py` & `QWeb-2.2.0/QWeb/keywords/text.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb/keywords/window.py` & `QWeb-2.2.0/QWeb/keywords/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/QWeb.egg-info/PKG-INFO` & `QWeb-2.2.0/QWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 2.1.2
+Version: 2.2.0
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `QWeb-2.1.2/QWeb.egg-info/SOURCES.txt` & `QWeb-2.2.0/QWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/README.md` & `QWeb-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/setup.cfg` & `QWeb-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `QWeb-2.1.2/setup.py` & `QWeb-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     keywords='test automation robot framework',
     author='Qentinel Group',
     author_email='libraries@qentinel.com',
     python_requires= ">3.6,<4.0",
     license= "Apache License 2.0",
     install_requires=["setuptools>=65.5.1",
-                      "pyscreeze>=0.1.28",
+                      "pyscreeze==0.1.28",
                       "pyautogui>=0.9.53",
                       "pynput>=1.7.6",
                       'requests>=2.27.0',
                       "robotframework>=3.2.2,<7",
                       "robotframework-debuglibrary==2.3.0",
                       "selenium==4.6.0",
                       "Pillow==9.3.0",
@@ -58,9 +58,9 @@
                       "scikit-image==0.19.1;python_version=='3.7'",
                       "scikit-image==0.20;python_version>'3.7'",
                       "ply",
                       "opencv-python==4.5.5.62",
                       "slate3k>=0.5.3"],
 
     extras_require={':"linux" in sys_platform': ['xlib'],
-                    ':"darwin" in sys_platform': ['pyobjc-core==8.3', 'pyobjc==8.3']}
+                    ':"darwin" in sys_platform': ['pyobjc-core==9.2', 'pyobjc==9.2']}
 )
```

### Comparing `QWeb-2.1.2/versioneer.py` & `QWeb-2.2.0/versioneer.py`

 * *Files identical despite different names*

