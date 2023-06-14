# Comparing `tmp/omkar_temp_mail-1.0.5.tar.gz` & `tmp/omkar_temp_mail-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omkar_temp_mail-1.0.5.tar", last modified: Wed Jun 14 07:08:20 2023, max compression
+gzip compressed data, was "omkar_temp_mail-1.0.6.tar", last modified: Wed Jun 14 07:16:40 2023, max compression
```

## Comparing `omkar_temp_mail-1.0.5.tar` & `omkar_temp_mail-1.0.6.tar`

### file list

```diff
@@ -1,2 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:08:20.665641 omkar_temp_mail-1.0.5/
--rw-rw-rw-   0        0        0     4720 2023-06-14 07:08:20.665641 omkar_temp_mail-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:40.084334 omkar_temp_mail-1.0.6/
+-rw-rw-rw-   0        0        0     4720 2023-06-14 07:16:40.084334 omkar_temp_mail-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2687 2023-06-14 06:44:14.826924 omkar_temp_mail-1.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:40.039854 omkar_temp_mail-1.0.6/omkar_temp_mail/
+-rw-rw-rw-   0        0        0       31 2023-06-13 16:07:02.777257 omkar_temp_mail-1.0.6/omkar_temp_mail/__init__.py
+-rw-rw-rw-   0        0        0     5435 2023-06-14 06:27:01.292419 omkar_temp_mail-1.0.6/omkar_temp_mail/temp_mail.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 omkar_temp_mail-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2279 2023-06-14 07:16:31.353223 omkar_temp_mail-1.0.6/setup.py
```

### Comparing `omkar_temp_mail-1.0.5/PKG-INFO` & `omkar_temp_mail-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: omkar_temp_mail
-Version: 1.0.5
+Version: 1.0.6
 Summary: Use Omkar Temporary for receiving temporary emails
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: Omkar Temp Mail
         ===============
```

