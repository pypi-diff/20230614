# Comparing `tmp/PYpirepfepc-0.2.tar.gz` & `tmp/PYpirepfepc-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PYpirepfepc-0.2.tar", last modified: Wed Jun 14 18:05:30 2023, max compression
+gzip compressed data, was "PYpirepfepc-0.3.tar", last modified: Wed Jun 14 20:01:45 2023, max compression
```

## Comparing `PYpirepfepc-0.2.tar` & `PYpirepfepc-0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 18:05:30.352393 PYpirepfepc-0.2/
--rw-rw-rw-   0        0        0      306 2023-06-14 18:05:30.352393 PYpirepfepc-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 18:05:30.350399 PYpirepfepc-0.2/PYpirepfepc.egg-info/
--rw-rw-rw-   0        0        0      306 2023-06-14 18:05:30.000000 PYpirepfepc-0.2/PYpirepfepc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-06-14 18:05:30.000000 PYpirepfepc-0.2/PYpirepfepc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 18:05:30.000000 PYpirepfepc-0.2/PYpirepfepc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 18:05:30.000000 PYpirepfepc-0.2/PYpirepfepc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-14 18:05:30.361371 PYpirepfepc-0.2/setup.cfg
--rw-rw-rw-   0        0        0      341 2023-06-14 18:04:05.000000 PYpirepfepc-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:01:45.275985 PYpirepfepc-0.3/
+-rw-rw-rw-   0        0        0      296 2023-06-14 20:01:45.275985 PYpirepfepc-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 20:01:45.273991 PYpirepfepc-0.3/PYpirepfepc.egg-info/
+-rw-rw-rw-   0        0        0      296 2023-06-14 20:01:45.000000 PYpirepfepc-0.3/PYpirepfepc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-06-14 20:01:45.000000 PYpirepfepc-0.3/PYpirepfepc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:01:45.000000 PYpirepfepc-0.3/PYpirepfepc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:01:45.000000 PYpirepfepc-0.3/PYpirepfepc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-14 20:01:45.279974 PYpirepfepc-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-06-14 19:59:09.000000 PYpirepfepc-0.3/setup.py
```

