# Comparing `tmp/python_hilo-2023.6.1.tar.gz` & `tmp/python_hilo-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_hilo-2023.6.1.tar", max compression
+gzip compressed data, was "python_hilo-2023.6.2.tar", max compression
```

## Comparing `python_hilo-2023.6.1.tar` & `python_hilo-2023.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2023-02-20 01:13:28.118104 python_hilo-2023.6.1/LICENSE
--rw-r--r--   0        0        0     1124 2023-02-20 01:13:28.118273 python_hilo-2023.6.1/README.md
--rw-r--r--   0        0        0      109 2022-03-03 03:33:56.401543 python_hilo-2023.6.1/pyhilo/__init__.py
--rw-r--r--   0        0        0    28807 2023-06-06 23:21:51.307174 python_hilo-2023.6.1/pyhilo/api.py
--rw-r--r--   0        0        0     6974 2023-06-06 23:21:51.308296 python_hilo-2023.6.1/pyhilo/const.py
--rw-r--r--   0        0        0     9103 2022-03-03 03:33:56.402025 python_hilo-2023.6.1/pyhilo/device/__init__.py
--rw-r--r--   0        0        0     1303 2023-04-07 15:45:29.694634 python_hilo-2023.6.1/pyhilo/device/climate.py
--rw-r--r--   0        0        0      946 2023-04-07 15:43:25.840649 python_hilo-2023.6.1/pyhilo/device/light.py
--rw-r--r--   0        0        0      462 2023-04-07 15:43:10.973680 python_hilo-2023.6.1/pyhilo/device/sensor.py
--rw-r--r--   0        0        0      454 2023-04-07 15:42:51.429777 python_hilo-2023.6.1/pyhilo/device/switch.py
--rw-r--r--   0        0        0     3836 2023-04-07 15:41:59.052538 python_hilo-2023.6.1/pyhilo/devices.py
--rw-r--r--   0        0        0     4013 2022-03-03 03:33:56.402480 python_hilo-2023.6.1/pyhilo/event.py
--rw-r--r--   0        0        0     1191 2022-03-03 03:33:56.402554 python_hilo-2023.6.1/pyhilo/exceptions.py
--rw-r--r--   0        0        0     1257 2022-03-03 03:33:56.402675 python_hilo-2023.6.1/pyhilo/util/__init__.py
--rw-r--r--   0        0        0     2988 2023-02-20 01:13:28.119721 python_hilo-2023.6.1/pyhilo/util/state.py
--rw-r--r--   0        0        0    13020 2023-04-07 15:38:42.902984 python_hilo-2023.6.1/pyhilo/websocket.py
--rw-r--r--   0        0        0     3151 2023-06-06 23:22:07.783549 python_hilo-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 python_hilo-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-02-20 01:13:28.118104 python_hilo-2023.6.2/LICENSE
+-rw-r--r--   0        0        0     1124 2023-02-20 01:13:28.118273 python_hilo-2023.6.2/README.md
+-rw-r--r--   0        0        0      109 2022-03-03 03:33:56.401543 python_hilo-2023.6.2/pyhilo/__init__.py
+-rw-r--r--   0        0        0    28807 2023-06-06 23:21:51.307174 python_hilo-2023.6.2/pyhilo/api.py
+-rw-r--r--   0        0        0     7000 2023-06-14 03:06:54.468104 python_hilo-2023.6.2/pyhilo/const.py
+-rw-r--r--   0        0        0     9103 2022-03-03 03:33:56.402025 python_hilo-2023.6.2/pyhilo/device/__init__.py
+-rw-r--r--   0        0        0     1303 2023-04-07 15:45:29.694634 python_hilo-2023.6.2/pyhilo/device/climate.py
+-rw-r--r--   0        0        0      946 2023-04-07 15:43:25.840649 python_hilo-2023.6.2/pyhilo/device/light.py
+-rw-r--r--   0        0        0      462 2023-04-07 15:43:10.973680 python_hilo-2023.6.2/pyhilo/device/sensor.py
+-rw-r--r--   0        0        0      454 2023-04-07 15:42:51.429777 python_hilo-2023.6.2/pyhilo/device/switch.py
+-rw-r--r--   0        0        0     3836 2023-04-07 15:41:59.052538 python_hilo-2023.6.2/pyhilo/devices.py
+-rw-r--r--   0        0        0     4013 2022-03-03 03:33:56.402480 python_hilo-2023.6.2/pyhilo/event.py
+-rw-r--r--   0        0        0     1191 2022-03-03 03:33:56.402554 python_hilo-2023.6.2/pyhilo/exceptions.py
+-rw-r--r--   0        0        0     1257 2022-03-03 03:33:56.402675 python_hilo-2023.6.2/pyhilo/util/__init__.py
+-rw-r--r--   0        0        0     2988 2023-02-20 01:13:28.119721 python_hilo-2023.6.2/pyhilo/util/state.py
+-rw-r--r--   0        0        0    13020 2023-04-07 15:38:42.902984 python_hilo-2023.6.2/pyhilo/websocket.py
+-rw-r--r--   0        0        0     3151 2023-06-14 03:07:23.448058 python_hilo-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 python_hilo-2023.6.2/PKG-INFO
```

### Comparing `python_hilo-2023.6.1/LICENSE` & `python_hilo-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/README.md` & `python_hilo-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/api.py` & `python_hilo-2023.6.2/pyhilo/api.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/const.py` & `python_hilo-2023.6.2/pyhilo/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,13 +228,15 @@
     "43082",
     "43078",
     "46199",
     "9063",
     "45678",
     "42405",
     "43095",
+    "45853",
 ]
 
 JASCO_OUTLETS: Final = [
     "42405",
     "43095",
+    "45853",
 ]
```

### Comparing `python_hilo-2023.6.1/pyhilo/device/__init__.py` & `python_hilo-2023.6.2/pyhilo/device/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/device/climate.py` & `python_hilo-2023.6.2/pyhilo/device/climate.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/device/light.py` & `python_hilo-2023.6.2/pyhilo/device/light.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/devices.py` & `python_hilo-2023.6.2/pyhilo/devices.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/event.py` & `python_hilo-2023.6.2/pyhilo/event.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/exceptions.py` & `python_hilo-2023.6.2/pyhilo/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/util/__init__.py` & `python_hilo-2023.6.2/pyhilo/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/util/state.py` & `python_hilo-2023.6.2/pyhilo/util/state.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyhilo/websocket.py` & `python_hilo-2023.6.2/pyhilo/websocket.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.6.1/pyproject.toml` & `python_hilo-2023.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 exclude = ".venv/.*"
 
 [tool.poetry]
 name = "python-hilo"
-version = "2023.06.01"
+version = "2023.06.02"
 description = "A Python3, async interface to the Hilo API"
 readme = "README.md"
 authors = ["David Vallee Delisle <me@dvd.dev>"]
 maintainers = ["David Vallee Delisle <me@dvd.dev>"]
 license = "MIT"
 repository = "https://github.com/dvd-dev/python-hilo"
 packages = [
```

### Comparing `python_hilo-2023.6.1/PKG-INFO` & `python_hilo-2023.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hilo
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: A Python3, async interface to the Hilo API
 Home-page: https://github.com/dvd-dev/python-hilo
 License: MIT
 Author: David Vallee Delisle
 Author-email: me@dvd.dev
 Maintainer: David Vallee Delisle
 Maintainer-email: me@dvd.dev
```

