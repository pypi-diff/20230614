# Comparing `tmp/ma_notification_center-1.2.1.tar.gz` & `tmp/ma_notification_center-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_notification_center-1.2.1.tar", last modified: Tue Jun 13 12:45:16 2023, max compression
+gzip compressed data, was "ma_notification_center-2.1.0.tar", last modified: Wed Jun 14 06:42:48 2023, max compression
```

## Comparing `ma_notification_center-1.2.1.tar` & `ma_notification_center-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:45:16.144971 ma_notification_center-1.2.1/
--rw-rw-rw-   0        0        0     1091 2023-06-13 10:42:17.000000 ma_notification_center-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      640 2023-06-13 12:45:16.144971 ma_notification_center-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-06-13 12:44:11.000000 ma_notification_center-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 12:45:16.143930 ma_notification_center-1.2.1/ma_notification_center.egg-info/
--rw-rw-rw-   0        0        0      640 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 12:45:16.145926 ma_notification_center-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      813 2023-06-13 12:44:53.000000 ma_notification_center-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:42:48.627827 ma_notification_center-2.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-06-14 06:35:41.000000 ma_notification_center-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1567 2023-06-14 06:42:48.626828 ma_notification_center-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-06-14 06:33:54.000000 ma_notification_center-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:42:48.600317 ma_notification_center-2.1.0/ma_notification_center/
+-rw-rw-rw-   0        0        0        0 2023-06-14 06:28:51.000000 ma_notification_center-2.1.0/ma_notification_center/__init__.py
+-rw-rw-rw-   0        0        0     5651 2023-06-14 06:31:07.000000 ma_notification_center-2.1.0/ma_notification_center/notificationcenter.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:42:48.625832 ma_notification_center-2.1.0/ma_notification_center.egg-info/
+-rw-rw-rw-   0        0        0     1567 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:42:48.627827 ma_notification_center-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-06-14 06:42:25.000000 ma_notification_center-2.1.0/setup.py
```

### Comparing `ma_notification_center-1.2.1/LICENSE` & `ma_notification_center-2.1.0/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
+
+Copyright (c) 2023 Fatima Medlij
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ma_notification_center-1.2.1/README.md` & `ma_notification_center-2.1.0/README.md`

 * *Files identical despite different names*

