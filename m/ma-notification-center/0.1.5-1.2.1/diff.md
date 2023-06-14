# Comparing `tmp/ma_notification_center-0.1.5.tar.gz` & `tmp/ma_notification_center-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_notification_center-0.1.5.tar", last modified: Wed Jun 14 06:36:25 2023, max compression
+gzip compressed data, was "ma_notification_center-1.2.1.tar", last modified: Tue Jun 13 12:45:16 2023, max compression
```

## Comparing `ma_notification_center-0.1.5.tar` & `ma_notification_center-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:36:25.923189 ma_notification_center-0.1.5/
--rw-rw-rw-   0        0        0     1089 2023-06-14 06:35:41.000000 ma_notification_center-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1567 2023-06-14 06:36:25.922192 ma_notification_center-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-06-14 06:33:54.000000 ma_notification_center-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:36:25.891587 ma_notification_center-0.1.5/ma_notification_center/
--rw-rw-rw-   0        0        0        0 2023-06-14 06:28:51.000000 ma_notification_center-0.1.5/ma_notification_center/__init__.py
--rw-rw-rw-   0        0        0     5651 2023-06-14 06:31:07.000000 ma_notification_center-0.1.5/ma_notification_center/notificationcenter.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:36:25.921238 ma_notification_center-0.1.5/ma_notification_center.egg-info/
--rw-rw-rw-   0        0        0     1567 2023-06-14 06:36:25.000000 ma_notification_center-0.1.5/ma_notification_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-06-14 06:36:25.000000 ma_notification_center-0.1.5/ma_notification_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:36:25.000000 ma_notification_center-0.1.5/ma_notification_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-14 06:36:25.000000 ma_notification_center-0.1.5/ma_notification_center.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-14 06:36:25.000000 ma_notification_center-0.1.5/ma_notification_center.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:36:25.924188 ma_notification_center-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      539 2023-06-14 06:34:04.000000 ma_notification_center-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:45:16.144971 ma_notification_center-1.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 10:42:17.000000 ma_notification_center-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      640 2023-06-13 12:45:16.144971 ma_notification_center-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-06-13 12:44:11.000000 ma_notification_center-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 12:45:16.143930 ma_notification_center-1.2.1/ma_notification_center.egg-info/
+-rw-rw-rw-   0        0        0      640 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:45:16.000000 ma_notification_center-1.2.1/ma_notification_center.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 12:45:16.145926 ma_notification_center-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      813 2023-06-13 12:44:53.000000 ma_notification_center-1.2.1/setup.py
```

### Comparing `ma_notification_center-0.1.5/LICENSE` & `ma_notification_center-1.2.1/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-MIT License
-
-Copyright (c) 2023 Fatima Medlij
+Copyright (c) 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ma_notification_center-0.1.5/PKG-INFO` & `ma_notification_center-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: ma_notification_center
-Version: 0.1.5
-Summary: MobileArts Notification Center Package
-Author: Fatima Medlij
-Author-email: medlijfatima@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ma_notification_center
 
 ma-notifications is a Python package that provides a notification center for sending various types of notifications.
 
 ## Installation
 
 You can install ma-notification-center using pip:
```

