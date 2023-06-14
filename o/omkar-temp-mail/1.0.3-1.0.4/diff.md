# Comparing `tmp/omkar-temp-mail-1.0.3.tar.gz` & `tmp/omkar_temp_mail-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omkar-temp-mail-1.0.3.tar", last modified: Wed Jun 14 07:01:59 2023, max compression
+gzip compressed data, was "omkar_temp_mail-1.0.4.tar", last modified: Wed Jun 14 07:05:38 2023, max compression
```

## Comparing `omkar-temp-mail-1.0.3.tar` & `omkar_temp_mail-1.0.4.tar`

### file list

```diff
@@ -1,2 +1,2 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:01:59.569862 omkar-temp-mail-1.0.3/
--rw-rw-rw-   0        0        0     4720 2023-06-14 07:01:59.569862 omkar-temp-mail-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 07:05:38.973616 omkar_temp_mail-1.0.4/
+-rw-rw-rw-   0        0        0     4720 2023-06-14 07:05:38.973616 omkar_temp_mail-1.0.4/PKG-INFO
```

### Comparing `omkar-temp-mail-1.0.3/PKG-INFO` & `omkar_temp_mail-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: omkar-temp-mail
-Version: 1.0.3
+Name: omkar_temp_mail
+Version: 1.0.4
 Summary: Use Omkar Temporary for receiving temporary emails
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: Omkar Temp Mail
         ===============
```

