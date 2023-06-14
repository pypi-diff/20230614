# Comparing `tmp/ovos-PHAL-plugin-oauth-0.0.0a2.tar.gz` & `tmp/ovos-PHAL-plugin-oauth-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.0a2.tar", last modified: Thu Feb  2 23:16:50 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.1.tar", last modified: Wed Mar  8 23:59:24 2023, max compression
```

## Comparing `ovos-PHAL-plugin-oauth-0.0.0a2.tar` & `ovos-PHAL-plugin-oauth-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:16:50.529039 ovos-PHAL-plugin-oauth-0.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-02 23:16:50.529039 ovos-PHAL-plugin-oauth-0.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-02-02 23:16:42.000000 ovos-PHAL-plugin-oauth-0.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:16:50.529039 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth/
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-02-02 23:16:42.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-02 23:16:45.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:16:50.529039 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-02 23:16:50.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-02 23:16:50.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 23:16:50.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-02 23:16:50.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-02 23:16:50.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-02 23:16:50.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 23:16:50.000000 ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 23:16:50.529039 ovos-PHAL-plugin-oauth-0.0.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-02-02 23:16:42.000000 ovos-PHAL-plugin-oauth-0.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:59:24.053559 ovos-PHAL-plugin-oauth-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-08 23:59:24.053559 ovos-PHAL-plugin-oauth-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-03-08 23:59:12.000000 ovos-PHAL-plugin-oauth-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:59:24.053559 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-03-08 23:59:12.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-08 23:59:16.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:59:24.053559 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-08 23:59:23.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-08 23:59:24.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 23:59:23.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-08 23:59:23.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-08 23:59:23.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-08 23:59:23.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 23:59:12.000000 ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 23:59:24.053559 ovos-PHAL-plugin-oauth-0.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-03-08 23:59:12.000000 ovos-PHAL-plugin-oauth-0.0.1/setup.py
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.0a2/PKG-INFO` & `ovos-PHAL-plugin-oauth-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-oauth
-Version: 0.0.0a2
+Version: 0.0.1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-oauth
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.0a2/README.md` & `ovos-PHAL-plugin-oauth-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth/__init__.py` & `ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-oauth-0.0.0a2/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO` & `ovos-PHAL-plugin-oauth-0.0.1/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-oauth
-Version: 0.0.0a2
+Version: 0.0.1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-oauth
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.0a2/setup.py` & `ovos-PHAL-plugin-oauth-0.0.1/setup.py`

 * *Files identical despite different names*

