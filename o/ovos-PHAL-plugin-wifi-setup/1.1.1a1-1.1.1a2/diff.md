# Comparing `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a1.tar.gz` & `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a1.tar", last modified: Sat Jun 10 02:14:04 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a2.tar", last modified: Wed Jun 14 01:43:14 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a1.tar` & `ovos-PHAL-plugin-wifi-setup-1.1.1a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/
--rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 02:13:58.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:43:14.804878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:43:08.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/setup.py
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a1/LICENSE` & `ovos-PHAL-plugin-wifi-setup-1.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a1/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a1/README.md` & `ovos-PHAL-plugin-wifi-setup-1.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/__init__.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 import random
 import uuid
 from os.path import dirname, join
 from time import sleep
 
-from mycroft_bus_client.message import Message
+from ovos_bus_client.message import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils import create_daemon
 from ovos_utils.device_input import can_use_touch_mouse
 from ovos_utils.enclosure.api import EnclosureAPI
 from ovos_utils.gui import (GUIInterface,
                             is_gui_running, is_gui_connected)
 from ovos_utils.log import LOG
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a1/setup.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a2/setup.py`

 * *Files identical despite different names*

