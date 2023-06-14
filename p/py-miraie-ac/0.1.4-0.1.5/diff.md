# Comparing `tmp/py-miraie-ac-0.1.4.tar.gz` & `tmp/py-miraie-ac-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.1.4.tar", last modified: Tue Jun 13 07:43:23 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.1.5.tar", last modified: Wed Jun 14 02:47:06 2023, max compression
```

## Comparing `py-miraie-ac-0.1.4.tar` & `py-miraie-ac-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.857454 py-miraie-ac-0.1.4/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1273 2023-06-13 07:43:23.857454 py-miraie-ac-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.4/README.md
--rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-13 07:43:23.858450 py-miraie-ac-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.835462 py-miraie-ac-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.852458 py-miraie-ac-0.1.4/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6716 2023-06-13 07:30:45.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4928 2023-06-11 14:23:54.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      995 2023-06-10 12:09:13.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0     1585 2023-06-13 07:04:26.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/test.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.856449 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1273 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 02:47:06.754564 py-miraie-ac-0.1.5/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1273 2023-06-14 02:47:06.754564 py-miraie-ac-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.5/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-14 02:47:06.755561 py-miraie-ac-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 02:47:06.637737 py-miraie-ac-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 02:47:06.748576 py-miraie-ac-0.1.5/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6714 2023-06-14 02:42:32.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6973 2023-06-14 02:41:55.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4928 2023-06-11 14:23:54.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      995 2023-06-10 12:09:13.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0     1719 2023-06-14 02:45:04.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/test.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.5/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:47:06.753566 py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1273 2023-06-14 02:47:06.000000 py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-14 02:47:06.000000 py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:47:06.000000 py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-14 02:47:06.000000 py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:47:06.000000 py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.1.4/LICENSE` & `py-miraie-ac-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/PKG-INFO` & `py-miraie-ac-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.4/README.md` & `py-miraie-ac-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/setup.cfg` & `py-miraie-ac-0.1.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e34  .version = 0.1.4
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e35  .version = 0.1.5
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/api.py` & `py-miraie-ac-0.1.5/src/py_miraie_ac/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """The MirAIe API module"""
 
 import math
 import random
 import asyncio
 from typing import Callable
-
 import aiohttp
 from py_miraie_ac.broker import MirAIeBroker
 from py_miraie_ac.device import Device
 from py_miraie_ac.constants import DEVICE_DETAILS_URL, HOMES_URL,HTTP_CLIENT_ID,LOGIN_URL,STATUS_URL
 from py_miraie_ac.deviceStatus import DeviceStatus
 from py_miraie_ac.enums import (
     AuthType,
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/device.py` & `py-miraie-ac-0.1.5/src/py_miraie_ac/device.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/deviceStatus.py` & `py-miraie-ac-0.1.5/src/py_miraie_ac/deviceStatus.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.1.5/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/test.py` & `py-miraie-ac-0.1.5/src/py_miraie_ac/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
 
 
 
 
 async def start():
     """Test"""
-    async with MirAIeAPI(auth_type=AuthType.MOBILE, login_id="", password="") as api:
+    async with MirAIeAPI(auth_type=AuthType.MOBILE, login_id="+918861319451", password="Godislove@1") as api:
         await api.initialize()
+        for device in api.devices:
+            print(f"Found {device.friendly_name} in {device.area_name}")
 
         while True:
             await asyncio.sleep(5)
 
 asyncio.get_event_loop().run_until_complete(start())
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/SOURCES.txt` & `py-miraie-ac-0.1.5/src/py_miraie_ac.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/py_miraie_ac/__init__.py
 src/py_miraie_ac/api.py
+src/py_miraie_ac/broker.py
 src/py_miraie_ac/constants.py
 src/py_miraie_ac/device.py
 src/py_miraie_ac/deviceStatus.py
 src/py_miraie_ac/enums.py
 src/py_miraie_ac/exceptions.py
 src/py_miraie_ac/home.py
 src/py_miraie_ac/test.py
```

