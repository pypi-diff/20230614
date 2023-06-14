# Comparing `tmp/omkar_temp_mail-1.0.0.tar.gz` & `tmp/omkar_temp_mail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omkar_temp_mail-1.0.0.tar", last modified: Wed Jun 14 06:20:59 2023, max compression
+gzip compressed data, was "omkar_temp_mail-1.0.1.tar", last modified: Wed Jun 14 06:45:26 2023, max compression
```

## Comparing `omkar_temp_mail-1.0.0.tar` & `omkar_temp_mail-1.0.1.tar`

### file list

```diff
@@ -1,2 +1,2 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:59.351020 omkar_temp_mail-1.0.0/
--rw-rw-rw-   0        0        0     1770 2023-06-14 06:20:59.351020 omkar_temp_mail-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 06:45:26.426909 omkar_temp_mail-1.0.1/
+-rw-rw-rw-   0        0        0     4705 2023-06-14 06:45:26.434904 omkar_temp_mail-1.0.1/PKG-INFO
```

