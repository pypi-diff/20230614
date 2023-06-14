# Comparing `tmp/AsyncIRCClient-0.0.1.tar.gz` & `tmp/AsyncIRCClient-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsyncIRCClient-0.0.1.tar", last modified: Fri Jun  9 10:28:44 2023, max compression
+gzip compressed data, was "AsyncIRCClient-0.0.2.tar", last modified: Fri Jun  9 10:32:59 2023, max compression
```

## Comparing `AsyncIRCClient-0.0.1.tar` & `AsyncIRCClient-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 10:28:44.698090 AsyncIRCClient-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-09 10:28:44.695090 AsyncIRCClient-0.0.1/AsyncIRCClient.egg-info/
--rw-rw-rw-   0        0        0      142 2023-06-09 10:28:44.000000 AsyncIRCClient-0.0.1/AsyncIRCClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-09 10:28:44.000000 AsyncIRCClient-0.0.1/AsyncIRCClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:28:44.000000 AsyncIRCClient-0.0.1/AsyncIRCClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 10:28:44.000000 AsyncIRCClient-0.0.1/AsyncIRCClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 10:28:44.000000 AsyncIRCClient-0.0.1/AsyncIRCClient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-06-09 10:28:44.698090 AsyncIRCClient-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 10:28:44.697090 AsyncIRCClient-0.0.1/async_irc_client/
--rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.1/async_irc_client/__init__.py
--rw-rw-rw-   0        0        0    30031 2023-06-09 01:56:19.000000 AsyncIRCClient-0.0.1/async_irc_client/async_irc_client.py
--rw-rw-rw-   0        0        0       42 2023-06-09 10:28:44.698090 AsyncIRCClient-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      280 2023-06-09 10:27:38.000000 AsyncIRCClient-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 10:32:59.185791 AsyncIRCClient-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-09 10:32:59.182789 AsyncIRCClient-0.0.2/AsyncIRCClient.egg-info/
+-rw-rw-rw-   0        0        0     1339 2023-06-09 10:32:59.000000 AsyncIRCClient-0.0.2/AsyncIRCClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-09 10:32:59.000000 AsyncIRCClient-0.0.2/AsyncIRCClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 10:32:59.000000 AsyncIRCClient-0.0.2/AsyncIRCClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 10:32:59.000000 AsyncIRCClient-0.0.2/AsyncIRCClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 10:32:59.000000 AsyncIRCClient-0.0.2/AsyncIRCClient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1339 2023-06-09 10:32:59.185791 AsyncIRCClient-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 10:32:59.183789 AsyncIRCClient-0.0.2/async_irc_client/
+-rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.2/async_irc_client/__init__.py
+-rw-rw-rw-   0        0        0    30031 2023-06-09 01:56:19.000000 AsyncIRCClient-0.0.2/async_irc_client/async_irc_client.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 10:32:59.185791 AsyncIRCClient-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      460 2023-06-09 10:32:22.000000 AsyncIRCClient-0.0.2/setup.py
```

### Comparing `AsyncIRCClient-0.0.1/README.md` & `AsyncIRCClient-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AsyncIRCClient-0.0.1/async_irc_client/async_irc_client.py` & `AsyncIRCClient-0.0.2/async_irc_client/async_irc_client.py`

 * *Files identical despite different names*

