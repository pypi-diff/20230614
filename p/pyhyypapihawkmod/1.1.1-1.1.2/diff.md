# Comparing `tmp/pyhyypapihawkmod-1.1.1.tar.gz` & `tmp/pyhyypapihawkmod-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.1.tar", last modified: Thu Jun  8 13:30:27 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.2.tar", last modified: Wed Jun 14 05:17:09 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.1.tar` & `pyhyypapihawkmod-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:30:27.893247 pyhyypapihawkmod-1.1.1/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-06-08 13:30:27.892732 pyhyypapihawkmod-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1679 2023-06-08 12:51:40.000000 pyhyypapihawkmod-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 13:30:27.878356 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     7471 2023-06-08 13:27:14.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27687 2023-06-08 12:19:08.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:30:27.890168 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-08 13:30:27.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-06-08 13:30:27.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 13:30:27.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-08 13:30:27.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 13:30:27.000000 pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 13:30:27.893756 pyhyypapihawkmod-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-06-08 13:27:27.000000 pyhyypapihawkmod-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:17:09.778410 pyhyypapihawkmod-1.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      517 2023-06-14 05:17:09.777361 pyhyypapihawkmod-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1866 2023-06-14 05:15:04.000000 pyhyypapihawkmod-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 05:17:09.766050 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     7664 2023-06-14 05:13:01.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27687 2023-06-08 12:19:08.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:17:09.775793 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-06-14 05:17:09.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-06-14 05:17:09.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 05:17:09.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-14 05:17:09.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 05:17:09.000000 pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 05:17:09.778410 pyhyypapihawkmod-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-06-12 15:37:10.000000 pyhyypapihawkmod-1.1.2/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.1/LICENSE.md` & `pyhyypapihawkmod-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/PKG-INFO` & `pyhyypapihawkmod-1.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.1
+Version: 1.1.2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/alarm_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,43 @@
 from typing import TYPE_CHECKING, Any
 from datetime import datetime
 from .constants import EventNumber
 
 if TYPE_CHECKING:
     from .client import HyypClient
 
-_last_notification_check_timestamp = 0
+
 
 class HyypAlarmInfos:
     """Initialize Hyyp alarm objects."""
 
     def __init__(self, client: HyypClient) -> None:
         """init."""
         self._client = client
         self._sync_info: dict = {}
         self._state_info: dict = {}
+        self._notifications: dict = {}
+        self._last_notification_check_timestamp = 0
 
     def _fetch_data(self) -> None:
         """Fetch data via client api."""
         self._sync_info = self._client.get_sync_info()
         self._state_info = self._client.get_state_info()
+        
+    def _fetch_notifications(self, site_id: int) -> dict[Any,Any]:
+        """Fetch and cache site notifications."""
+        self._notifications = self._client.site_notifications(site_id=site_id)
+
 
-    def _last_notice(self, site_id: int) -> dict[Any, Any]:
+    def _last_notice(self) -> dict[Any, Any]:
         """Get last notification."""
         _response: dict[Any, Any] = {"lastNoticeTime": None, "lastNoticeName": None}
 
-        _last_notification = self._client.site_notifications(
-            site_id=site_id, json_key=0
-        )
-
+        _last_notification = self._notifications[0]
+        
         if _last_notification:
 
             _last_event = _last_notification["eventNumber"]
             _last_event_datetime = str(
                 datetime.fromtimestamp(_last_notification["timestamp"] / 1000)
             )  # Epoch in ms
 
@@ -44,42 +49,41 @@
                 "lastNoticeName": EventNumber[str(_last_event)],
             }
 
         return _response
 
 
 
-    def _new_notifications(self, site_id: int) -> Any:
+    def _new_notifications(self) -> Any:
 
-        global _last_notification_check_timestamp   
+        _last_notification_check_timestamp = self._last_notification_check_timestamp   
         _response = []
 
-        _notifications = self._client.site_notifications(
-            site_id=site_id)
+        _notifications = self._notifications
                 
         _current_timestamp = round(datetime.now().timestamp())
             
         for x in _notifications:
             
             _notification_timestamp = round(x['timestamp']/1000)
             if _current_timestamp - _notification_timestamp > 120:
                 continue
             if _notification_timestamp <= (_last_notification_check_timestamp-30):
                 continue
             _response.append(x)
         
-        _last_notification_check_timestamp = _current_timestamp
+        self._last_notification_check_timestamp = _current_timestamp
  
         return _response
 
 
-    def _triggered_zones(self, site_id: int) -> Any:
+    def _triggered_zones(self) -> Any:
            
         triggeredZoneIds = []
-        _new_notifications = self._new_notifications(site_id=site_id)
+        _new_notifications = self._new_notifications()
         
         for _notification in _new_notifications:
             if _notification['eventNumber'] != 5:
                 continue
             triggeredZoneIds.append(_notification['zoneId'])  
                  
         _response = triggeredZoneIds
@@ -106,18 +110,19 @@
         
         trigger_ids = {
             trigger["id"]: trigger for trigger in self._sync_info["triggers"]
         }
         
         for site in site_ids:
             
+            self._fetch_notifications(site_id=site)
             triggered_zones = self._triggered_zones(site_id=site)
 
             # Add last site notification.
-            _last_notice = self._last_notice(site_id=site)
+            _last_notice = self._last_notice()
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
             for trigger_id in trigger_ids:
                 if trigger_id not in site_ids[site]["triggerIds"]:
                     continue
```

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.1
+Version: 1.1.2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.1/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.2/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.1/setup.py` & `pyhyypapihawkmod-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.1",
+    version="1.1.2",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

