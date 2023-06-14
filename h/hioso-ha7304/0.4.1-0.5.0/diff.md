# Comparing `tmp/hioso-ha7304-0.4.1.tar.gz` & `tmp/hioso-ha7304-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hioso-ha7304-0.4.1.tar", max compression
+gzip compressed data, was "hioso-ha7304-0.5.0.tar", max compression
```

## Comparing `hioso-ha7304-0.4.1.tar` & `hioso-ha7304-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      133 2023-01-20 13:32:44.329995 hioso-ha7304-0.4.1/hioso_ha7304/__init__.py
--rw-r--r--   0        0        0     3232 2023-01-20 02:01:10.527945 hioso-ha7304-0.4.1/hioso_ha7304/ha7304.py
--rw-r--r--   0        0        0      325 2023-01-17 06:01:29.821348 hioso-ha7304-0.4.1/hioso_ha7304/mac.py
--rw-r--r--   0        0        0     1636 2023-01-20 13:30:05.051257 hioso-ha7304-0.4.1/hioso_ha7304/onu.py
--rw-r--r--   0        0        0    35823 2022-12-15 14:48:20.558101 hioso-ha7304-0.4.1/LICENSE
--rw-r--r--   0        0        0      489 2023-01-20 13:32:18.414797 hioso-ha7304-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      653 2023-01-20 13:33:19.725486 hioso-ha7304-0.4.1/setup.py
--rw-r--r--   0        0        0      477 2023-01-20 13:33:19.725486 hioso-ha7304-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-01-21 02:16:22.535342 hioso-ha7304-0.5.0/hioso_ha7304/__init__.py
+-rw-r--r--   0        0        0     3427 2023-01-21 02:14:35.308386 hioso-ha7304-0.5.0/hioso_ha7304/ha7304.py
+-rw-r--r--   0        0        0      325 2023-01-17 06:01:29.821348 hioso-ha7304-0.5.0/hioso_ha7304/mac.py
+-rw-r--r--   0        0        0     2626 2023-01-21 02:11:03.391849 hioso-ha7304-0.5.0/hioso_ha7304/onu.py
+-rw-r--r--   0        0        0    35823 2022-12-15 14:48:20.558101 hioso-ha7304-0.5.0/LICENSE
+-rw-r--r--   0        0        0      489 2023-01-21 02:15:50.167321 hioso-ha7304-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      653 2023-01-21 02:17:06.285604 hioso-ha7304-0.5.0/setup.py
+-rw-r--r--   0        0        0      477 2023-01-21 02:17:06.285604 hioso-ha7304-0.5.0/PKG-INFO
```

### Comparing `hioso-ha7304-0.4.1/hioso_ha7304/ha7304.py` & `hioso-ha7304-0.5.0/hioso_ha7304/ha7304.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import attr
 from cachetools import Cache, TTLCache, cachedmethod
 from operator import attrgetter
 from requests import Session
 from requests.auth import HTTPBasicAuth
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from . import Mac, Onu
 
 
+OnuOperation = Literal["rebootOp", "activeOp", "noactiveOp", "restoreOp", "cleanLoopOp"]
+
+
 @attr.dataclass(slots=True)
 class Ha7304:
     url: str
     username: str
     password: str
     session: Session = attr.ib(factory=Session)
     cached_onu_time: int = 30
@@ -61,32 +64,32 @@
     def _all_mac_list(self) -> str:
         res = self.session.get(self.url + "/oltMacFdb.asp")
         data = res.text
         data = data.split("'\n);\nfunction Reload()")[0]
         data = data.split("Array(\n'")[1]
         return data
 
-    def setOnu(self, onu: Onu, operation: str):
-        data = {"onuId": onu.id, "onuName": onu.name, "onuOperation": operation}
+    def setOnu(self, onu_id: str, onu_name: str, operation: OnuOperation):
+        data = {"onuId": onu_id, "onuName": onu_name, "onuOperation": operation}
         self.session.post(self.url + "/goform/setOnu", data, allow_redirects=False)
 
     def reboot(self, onu: Onu):
-        return self.setOnu(onu, "rebootOp")
+        return self.setOnu(onu.id, onu.name, "rebootOp")
 
     def activate(self, onu: Onu):
-        return self.setOnu(onu, "activeOp")
+        return self.setOnu(onu.id, onu.name, "activeOp")
 
     def deactivate(self, onu: Onu):
-        return self.setOnu(onu, "noactiveOp")
+        return self.setOnu(onu.id, onu.name, "noactiveOp")
 
     def factory(self, onu: Onu):
-        return self.setOnu(onu, "restoreOp")
+        return self.setOnu(onu.id, onu.name, "restoreOp")
 
     def clean_loop_flag(self, onu: Onu):
-        return self.setOnu(onu, "cleanLoopOp")
+        return self.setOnu(onu.id, onu.name, "cleanLoopOp")
 
     def set_onu_port_vlan(
         self,
         port_id: str,
         vlan_mode: str,
         vlan_id: str,
         port_name: str = None,
```

### Comparing `hioso-ha7304-0.4.1/LICENSE` & `hioso-ha7304-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hioso-ha7304-0.4.1/setup.py` & `hioso-ha7304-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.0.0,<23.0.0', 'cachetools>=5.2.1,<6.0.0', 'requests>=2.28.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'hioso-ha7304',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': '',
     'long_description': None,
     'author': 'hexatester',
     'author_email': 'hexatester@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

