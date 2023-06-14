# Comparing `tmp/ovos-PHAL-plugin-oauth-0.0.2a1.tar.gz` & `tmp/ovos-PHAL-plugin-oauth-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.2a1.tar", last modified: Wed Jun 14 01:21:41 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.2a2.tar", last modified: Wed Jun 14 01:44:06 2023, max compression
```

## Comparing `ovos-PHAL-plugin-oauth-0.0.2a1.tar` & `ovos-PHAL-plugin-oauth-0.0.2a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:21:41.600721 ovos-PHAL-plugin-oauth-0.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 01:21:41.600721 ovos-PHAL-plugin-oauth-0.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-14 01:21:31.000000 ovos-PHAL-plugin-oauth-0.0.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:21:41.600721 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth/
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-14 01:21:31.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:21:34.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:21:41.600721 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 01:21:41.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-14 01:21:41.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:21:41.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 01:21:41.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 01:21:41.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 01:21:41.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:21:31.000000 ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:21:41.600721 ovos-PHAL-plugin-oauth-0.0.2a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-14 01:21:31.000000 ovos-PHAL-plugin-oauth-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-14 01:43:55.000000 ovos-PHAL-plugin-oauth-0.0.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-14 01:43:55.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:43:58.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-14 01:43:55.000000 ovos-PHAL-plugin-oauth-0.0.2a2/setup.py
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a1/PKG-INFO` & `ovos-PHAL-plugin-oauth-0.0.2a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-oauth
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-oauth
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a1/README.md` & `ovos-PHAL-plugin-oauth-0.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth/__init__.py` & `ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a1/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO` & `ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-oauth
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-oauth
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a1/setup.py` & `ovos-PHAL-plugin-oauth-0.0.2a2/setup.py`

 * *Files identical despite different names*

