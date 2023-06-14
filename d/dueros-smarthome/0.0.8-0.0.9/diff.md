# Comparing `tmp/dueros_smarthome-0.0.8.tar.gz` & `tmp/dueros_smarthome-0.0.9.tar.gz`

## Comparing `dueros_smarthome-0.0.8.tar` & `dueros_smarthome-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/__init__.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/client.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/const.py
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/models.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/LICENSE
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/README.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/src/dueros_smarthome/__init__.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/src/dueros_smarthome/client.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/src/dueros_smarthome/const.py
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/src/dueros_smarthome/models.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/LICENSE
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/README.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.9/PKG-INFO
```

### Comparing `dueros_smarthome-0.0.8/.github/workflows/publish-to-pypi.yml` & `dueros_smarthome-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dueros_smarthome-0.0.8/src/dueros_smarthome/client.py` & `dueros_smarthome-0.0.9/src/dueros_smarthome/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 class SmartHomeClient:
     def __init__(self, bduss: str, host: str = const.DEFAULT_HOST, schema: str = const.DEFAULT_SCHEMA) -> None:
         self._host = host
         self._schema = schema
         self._bduss = bduss
         self._cookies = httpx.Cookies()
         self._cookies.set(const.BDUSS_COOKIE_KEY, self._bduss, domain = self._host)
+        for key in const.ADDITIONAL_COOKIES:
+            self._cookies.set(key, const.ADDITIONAL_COOKIES[key], domain = self._host)
     
     @property
     def host(self):
         return self._host
     
     def _get_device_list_url(self) -> str:
         return f'{self._schema}{self._host}{const.DEVICE_LIST_QUERY}'
```

### Comparing `dueros_smarthome-0.0.8/src/dueros_smarthome/const.py` & `dueros_smarthome-0.0.9/src/dueros_smarthome/const.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 DEFAULT_SCHEMA = "https://"
 DEFAULT_HOST = "xiaodu.baidu.com"
 
 DEFAULT_PAYLOAD_VERSION = 3
 
-DEVICE_LIST_QUERY = "/saiya/smarthome/devicelist?form=h5_control&generalscene=2"
+DEVICE_LIST_QUERY = "/saiya/smarthome/devicelist?from=h5_control&withscene=1&generalscene=3"
 DEVICE_ACTION_QUERY = "/saiya/smarthome/directivesend?from=h5_control"
 
 BDUSS_COOKIE_KEY = "BDUSS"
 
 REQUEST_HEADER = "header"
 REQUEST_HEADER_NAMESPACE = "namespace"
 REQUEST_HEADER_NAME = "name"
@@ -16,14 +16,16 @@
 PROXY_CONNECT_STATUS = "proxyConnectionStatus"
 REQUEST_PAYLOAD = "payload"
 APPLIANCE = "appliance"
 CONTROL_REQUEST_NAMESPACE = "DuerOS.ConnectedHome.Control"
 ATTRIBUTE = "attribute"
 ATTRIBUTE_VALUE = "attributeValue"
 
+ADDITIONAL_COOKIES = {"smarthome-curtain-device-detail-new": "1"}
+
 STATUS = "status"
 MSG = "msg"
 LOGID = "logid"
 DATA = "data"
 APPLIANCES = "appliances"
 BOT_NAME = "botName"
 BOT_ID = "botId"
```

### Comparing `dueros_smarthome-0.0.8/src/dueros_smarthome/models.py` & `dueros_smarthome-0.0.9/src/dueros_smarthome/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     
     @property
     def timestamp_of_sample(self):
         return self._timestamp_of_sample
 
 class ConnectivitySetting:
     def __init__(self, connectivity_setting: dict):
-        self._connectivity = connectivity_setting[const.VALUE]
+        self._value = connectivity_setting[const.VALUE]
         self._time = connectivity_setting[const.TIME]
     
     @property
-    def connectivity(self):
-        return self._connectivity
+    def value(self):
+        return self._value
 
     @property
     def time(self):
         return self._time
 
 class TurnOnState(Enum):
     NONE = auto()
@@ -45,20 +45,23 @@
 
     @staticmethod
     def from_str(label: str):
         return TurnOnState[label]
     
 class TurnOnStateSetting:
     def __init__(self, turn_on_state_setting: dict):
-        self._turn_on_state = TurnOnState.from_str(turn_on_state_setting[const.VALUE])
+        if turn_on_state_setting[const.VALUE]:
+            self._value = TurnOnState.from_str(turn_on_state_setting[const.VALUE])
+        else:
+            self._value = None
         self._time = turn_on_state_setting[const.TIME]
 
     @property
-    def turn_on_state(self):
-        return self._turn_on_state
+    def value(self):
+        return self._value
 
     @property
     def time(self):
         return self._time
 
 class ApplianceType(Enum):
     NONE = auto()
@@ -266,20 +269,23 @@
 
     @property
     def percentage(self) -> int:
         return self._value
 
 class BrightnessSetting:
     def __init__(self, brightness_setting: dict):
-        self._brightness = Brightness(brightness_setting[const.VALUE])
+        if brightness_setting[const.VALUE]:
+            self._value = Brightness(brightness_setting[const.VALUE])
+        else:
+            self._value = None
         self._time = brightness_setting[const.TIME]
 
     @property
-    def brightness(self):
-        return self._brightness
+    def value(self):
+        return self._value
     
     @property
     def time(self):
         return self._time
 
 class ColorTemperatureInKelvin(Num):
     def __init__(self, value: int, kelvin_min: int = '2700', kelvin_max: int = '6500'):
@@ -303,20 +309,23 @@
     
     @property
     def kelvin_max(self):
         return self._kelvin_max
 
 class ColorTemperatureInKelvinSetting:
     def __init__(self, setting: dict):
-        self._color_temperature_in_kelvin = ColorTemperatureInKelvin(setting[const.VALUE])
+        if setting[const.VALUE]:
+            self._value = ColorTemperatureInKelvin(setting[const.VALUE])
+        else:
+            self._value = None
         self._time = setting[const.TIME]
     
     @property
-    def color_temperature_in_kelvin(self):
-        return self._color_temperature_in_kelvin
+    def value(self):
+        return self._value
 
     @property
     def time(self):
         return self._time
 
 class LightMode:
     def __init__(self, mode_info: dict):
@@ -346,14 +355,16 @@
     def icon_url(self):
         return self._icon
 
 class ApplianceAttributes:
     def __init__(self, attributes: dict):
         if const.CONNECTIVITY in attributes:
             self._connectivity = ConnectivityAttribute(attributes[const.CONNECTIVITY])
+        else:
+            self._connectivity = None
 
     @property
     def connectivity(self):
         return self._connectivity
 
 class BrightnessAndColorTemperatureMode:
     def __init__(self, mode: dict):
@@ -386,20 +397,20 @@
     @property
     def icon_url(self):
         return self._icon_url
 
 class ApplianceModes:
     def __init__(self, modes: dict):
         if const.BRIGHTNESS_AND_COLOR_TEMPERATURE in modes:
-            self._brightness_and_color_temperature = {mode: BrightnessAndColorTemperatureMode(mode_setting) for (mode, mode_setting) in modes[const.BRIGHTNESS_AND_COLOR_TEMPERATURE]}
+            self._brightness_and_color_temperature = {mode: BrightnessAndColorTemperatureMode(modes[const.BRIGHTNESS_AND_COLOR_TEMPERATURE][mode]) for mode in modes[const.BRIGHTNESS_AND_COLOR_TEMPERATURE]}
         else:
             self._brightness_and_color_temperature = None
 
         if const.BRIGHTNESS_AND_COLOR_TEMPERATURE_WITH_ICON in modes:
-            self._brightness_and_color_temperature_with_icon = {mode: BrightnessAndColorTemperatureWithIconMode(mode_setting) for (mode, mode_setting) in modes[const.BRIGHTNESS_AND_COLOR_TEMPERATURE_WITH_ICON]}
+            self._brightness_and_color_temperature_with_icon = {mode: BrightnessAndColorTemperatureWithIconMode(modes[const.BRIGHTNESS_AND_COLOR_TEMPERATURE_WITH_ICON][mode]) for mode in modes[const.BRIGHTNESS_AND_COLOR_TEMPERATURE_WITH_ICON]}
         else:
             self._brightness_and_color_temperature_with_icon = None
 
     @property
     def brightness_and_color_temperature(self):
         return self._brightness_and_color_temperature
     
@@ -472,14 +483,15 @@
         self._friendly_name = appliance_info[const.FRIENDLY_NAME]
         self._group_name = appliance_info[const.GROUP_NAME]
         self._group_id = appliance_info[const.GROUP_ID]
         self._room_name = appliance_info[const.ROOM_NAME]
         self._room_id = appliance_info[const.ROOM_ID]
         self._floor_id = appliance_info[const.FLOOR_ID]
         self._attributes = ApplianceAttributes(appliance_info[const.ATTRIBUTES])
+        self._state_settings = ApplianceStateSettings(appliance_info[const.STATE_SETTING])
         self._icon_urls = [icon_url for icon_url in appliance_info[const.ICON_URLS].values()] 
         self._status = appliance_info[const.STATUS]
     
     @property
     def bot_name(self):
         return self._bot_name
     
@@ -536,13 +548,17 @@
         return self._floor_id
     
     @property
     def attributes(self):
         return self._attributes
     
     @property
+    def state_settings(self):
+        return self._state_settings
+    
+    @property
     def icon_urls(self):
         return self._icon_urls
     
     @property
     def status(self):
         return self._status
```

### Comparing `dueros_smarthome-0.0.8/.gitignore` & `dueros_smarthome-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dueros_smarthome-0.0.8/LICENSE` & `dueros_smarthome-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dueros_smarthome-0.0.8/pyproject.toml` & `dueros_smarthome-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dueros_smarthome"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Shaoyu Zhang", email="zsy056@gmail.com" },
 ]
 description = "Duer OS SmartHome APIs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dueros_smarthome-0.0.8/PKG-INFO` & `dueros_smarthome-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dueros_smarthome
-Version: 0.0.8
+Version: 0.0.9
 Summary: Duer OS SmartHome APIs
 Project-URL: Homepage, https://github.com/zsy056/dueros-smarthome
 Project-URL: Bug Tracker, https://github.com/zsy056/dueros-smarthome/issues
 Author-email: Shaoyu Zhang <zsy056@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

