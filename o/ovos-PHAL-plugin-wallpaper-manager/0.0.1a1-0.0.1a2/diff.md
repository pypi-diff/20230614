# Comparing `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.1a1.tar.gz` & `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.1a1.tar", last modified: Tue May 16 20:15:12 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.1a2.tar", last modified: Wed Jun 14 16:39:51 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1.tar` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:12.207867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 20:15:12.207867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:12.203867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 20:15:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:12.203867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-16 20:15:12.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:15:12.207867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:51.227169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 16:39:44.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-14 16:39:51.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:39:50.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:39:51.231169 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-06-14 16:39:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/setup.py
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/LICENSE` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/PKG-INFO` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wallpaper-manager
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wallpaper-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/README.md` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/__init__.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import threading
 import requests
 import hashlib
-from mycroft_bus_client.message import Message
+
+from ovos_bus_client.message import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.log import LOG
 from ovos_utils.skills.settings import PrivateSettings
 from ovos_utils.xdg_utils import xdg_data_home
 from ovos_config.config import Configuration
 from ovos_utils.events import EventSchedulerInterface
 from wallpaper_changer import set_wallpaper
 from ovos_PHAL_plugin_wallpaper_manager.downloadedProvider import DownloadedProvider
 
+
 class WallpaperManager(PHALPlugin):
 
     def __init__(self, bus=None, config=None):
         name = "ovos-PHAL-plugin-wallpaper-manager"
         super().__init__(bus=bus, name=name, config=config)
 
         # this is a XDG compliant json storage object similar to self.settings in MycroftSkill
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wallpaper-manager
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wallpaper-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/setup.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a2/setup.py`

 * *Files identical despite different names*

