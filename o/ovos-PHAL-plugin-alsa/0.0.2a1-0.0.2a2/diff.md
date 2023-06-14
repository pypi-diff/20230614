# Comparing `tmp/ovos-PHAL-plugin-alsa-0.0.2a1.tar.gz` & `tmp/ovos-PHAL-plugin-alsa-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.2a1.tar", last modified: Tue Apr  4 22:35:13 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.2a2.tar", last modified: Wed Jun 14 21:23:34 2023, max compression
```

## Comparing `ovos-PHAL-plugin-alsa-0.0.2a1.tar` & `ovos-PHAL-plugin-alsa-0.0.2a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:35:13.792384 ovos-PHAL-plugin-alsa-0.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-04 22:35:13.792384 ovos-PHAL-plugin-alsa-0.0.2a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:35:13.792384 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa/
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-04 22:35:06.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 22:35:08.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:35:13.792384 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-04 22:35:13.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-04 22:35:13.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:35:13.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-04 22:35:13.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-04 22:35:13.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 22:35:13.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:35:13.000000 ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:35:13.792384 ovos-PHAL-plugin-alsa-0.0.2a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-04-04 22:35:06.000000 ovos-PHAL-plugin-alsa-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:34.689368 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-14 21:23:25.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 21:23:28.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-06-14 21:23:25.000000 ovos-PHAL-plugin-alsa-0.0.2a2/setup.py
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.2a1/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.2a2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.2a1/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.2a1/setup.py` & `ovos-PHAL-plugin-alsa-0.0.2a2/setup.py`

 * *Files identical despite different names*

