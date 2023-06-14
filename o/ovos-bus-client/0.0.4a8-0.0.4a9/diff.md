# Comparing `tmp/ovos-bus-client-0.0.4a8.tar.gz` & `tmp/ovos-bus-client-0.0.4a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.4a8.tar", last modified: Fri May  5 20:23:01 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.4a9.tar", last modified: Sat May  6 01:20:15 2023, max compression
```

## Comparing `ovos-bus-client-0.0.4a8.tar` & `ovos-bus-client-0.0.4a9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:23:01.954027 ovos-bus-client-0.0.4a8/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 20:23:01.954027 ovos-bus-client-0.0.4a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:23:01.950027 ovos-bus-client-0.0.4a8/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:23:01.954027 ovos-bus-client-0.0.4a8/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:23:01.954027 ovos-bus-client-0.0.4a8/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:23:01.950027 ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 20:23:01.000000 ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-05 20:23:01.000000 ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:23:01.000000 ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-05 20:23:01.000000 ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 20:23:01.000000 ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 20:23:01.000000 ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:23:01.954027 ovos-bus-client-0.0.4a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-05 20:23:00.000000 ovos-bus-client-0.0.4a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15910 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 01:20:15.000000 ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:20:15.494020 ovos-bus-client-0.0.4a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-06 01:20:14.000000 ovos-bus-client-0.0.4a9/setup.py
```

### Comparing `ovos-bus-client-0.0.4a8/LICENSE.md` & `ovos-bus-client-0.0.4a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/PKG-INFO` & `ovos-bus-client-0.0.4a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a8
+Version: 0.0.4a9
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/client/client.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/conf.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/message.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/message.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/session.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 
 
 class UtteranceState(str, enum.Enum):
     INTENT = "intent"  # includes converse
     RESPONSE = "response"
 
 
+def _get_valid_langs():
+    return list(set([get_default_lang()] + Configuration().get("secondary_langs'", [])))
+
+
 class Session:
     """
     An class representing a Mycroft Session Identifier
     """
 
     def __init__(self, session_id=None, expiration_seconds=None, active_skills=None, history=None,
                  max_time=5, max_messages=5, utterance_states=None, lang=None, context=None, valid_langs=None):
         self.session_id = session_id or str(uuid4())
         self.lang = lang or get_default_lang()
 
-        def _get_valid_langs():
-            return list(set([get_default_lang()] + Configuration().get("secondary_langs'", [])))
-
         self.valid_languages = valid_langs or _get_valid_langs()
         self.active_skills = active_skills or []  # [skill_id , timestamp]
         self.history = history or []  # [Message , timestamp]
         self.utterance_states = utterance_states or {}  # {skill_id: UtteranceState}
         self.max_time = max_time  # minutes
         self.max_messages = max_messages
         self.touch_time = int(time.time())
```

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.4a9/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a8
+Version: 0.0.4a9
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a8/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.4a9/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a8/setup.py` & `ovos-bus-client-0.0.4a9/setup.py`

 * *Files identical despite different names*

