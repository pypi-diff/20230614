# Comparing `tmp/masterthermconnect-2.2.3.tar.gz` & `tmp/masterthermconnect-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterthermconnect-2.2.3.tar", last modified: Thu Mar 23 15:31:32 2023, max compression
+gzip compressed data, was "masterthermconnect-2.2.4.tar", last modified: Tue Jun 13 19:06:34 2023, max compression
```

## Comparing `masterthermconnect-2.2.3.tar` & `masterthermconnect-2.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:31:32.333258 masterthermconnect-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-03-23 15:31:32.333258 masterthermconnect-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:31:32.329259 masterthermconnect-2.2.3/masterthermconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/datamapread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/datamapwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/masterthermconnect/special.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:31:32.333258 masterthermconnect-2.2.3/masterthermconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-03-23 15:31:32.000000 masterthermconnect-2.2.3/masterthermconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-23 15:31:32.000000 masterthermconnect-2.2.3/masterthermconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 15:31:32.000000 masterthermconnect-2.2.3/masterthermconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-23 15:31:32.000000 masterthermconnect-2.2.3/masterthermconnect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-23 15:31:32.000000 masterthermconnect-2.2.3/masterthermconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-23 15:31:32.000000 masterthermconnect-2.2.3/masterthermconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-23 15:31:32.333258 masterthermconnect-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:31:32.333258 masterthermconnect-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/tests/test_api_new.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/tests/test_api_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/tests/test_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28374 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-03-23 15:30:56.000000 masterthermconnect-2.2.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/masterthermconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/datamapread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/datamapwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/special.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/masterthermconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 19:06:34.235447 masterthermconnect-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_api_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_api_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29214 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_main.py
```

### Comparing `masterthermconnect-2.2.3/LICENSE` & `masterthermconnect-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/PKG-INFO` & `masterthermconnect-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.3 Summary: Python 3
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.4 Summary: Python 3
 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `masterthermconnect-2.2.3/README.md` & `masterthermconnect-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/__init__.py` & `masterthermconnect-2.2.4/masterthermconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/__main__.py` & `masterthermconnect-2.2.4/masterthermconnect/__main__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/api.py` & `masterthermconnect-2.2.4/masterthermconnect/api.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/const.py` & `masterthermconnect-2.2.4/masterthermconnect/const.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/controller.py` & `masterthermconnect-2.2.4/masterthermconnect/controller.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/datamapread.py` & `masterthermconnect-2.2.4/masterthermconnect/datamapread.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         Special(str, Special.FORMULA),
         [
             (
                 "'dhw' if {0} else "
                 "'pool' if {1} else "
                 "'aux_heater' if not ({2} or {3}) and ({4} or {5}) else "
                 "'dpc' if {6} else "
-                "'cooling' if {7} else "
+                "'cooling' if {7} or {12} or {13} else"
                 "'heating' if {8} or {9} or {10} or {11} else "
                 "'idle'"
             ),
             [
                 [bool, "D_66"],  # 0 - domestic hot water
                 [bool, "D_43"],  # 1 - pool
                 [bool, "D_20"],  # 2 - some_error
@@ -310,14 +310,16 @@
                 [bool, "D_7"],  # 5 - aux heater 2
                 [bool, "D_196"],  # 6 - Dew Point
                 [bool, "D_4"],  # 7 - Cooling Mode
                 [bool, "D_5"],  # 8 - Compressor 1
                 [bool, "D_32"],  # 9 - Compressor 2
                 [bool, "D_10"],  # 10 - Ciculation
                 [bool, "D_8"],  # 11 - Fan
+                [bool, "D_277"],  # 12 - Cooling Pump On
+                [bool, "D_193"],  # 13 - Requested Mode
             ],
         ],
     ],
     "season": {
         "mode": [
             Special(str, Special.FORMULA),
             [
@@ -339,16 +341,16 @@
         "requested_min": [float, "A_299"],
         "requested_max": [float, "A_207"],
         "outside_min": [float, "A_300"],
         "outside_max": [float, "A_301"],
     },
     "control_curve_cooling": {
         "setpoint_a_outside": [float, "A_47"],
-        "setpoint_a_requested": [float, "A_48"],
-        "setpoint_b_outside": [float, "A_49"],
+        "setpoint_a_requested": [float, "A_49"],
+        "setpoint_b_outside": [float, "A_48"],
         "setpoint_b_requested": [float, "A_50"],
         "requested_min": [float, "A_305"],
         "requested_max": [float, "A_306"],
         "outside_min": [float, "A_307"],
         "outside_max": [float, "A_308"],
     },
     "domestic_hot_water": {
```

### Comparing `masterthermconnect-2.2.3/masterthermconnect/datamapwrite.py` & `masterthermconnect-2.2.4/masterthermconnect/datamapwrite.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/exceptions.py` & `masterthermconnect-2.2.4/masterthermconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect/special.py` & `masterthermconnect-2.2.4/masterthermconnect/special.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/masterthermconnect.egg-info/PKG-INFO` & `masterthermconnect-2.2.4/masterthermconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.3 Summary: Python 3
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.4 Summary: Python 3
 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `masterthermconnect-2.2.3/masterthermconnect.egg-info/SOURCES.txt` & `masterthermconnect-2.2.4/masterthermconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/pyproject.toml` & `masterthermconnect-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masterthermconnect"
-version = "2.2.3"
+version = "2.2.4"
 description = "Python 3 API wrapper for Mastertherm API"
 readme = "README.md"
 authors = [{ name = "Richard Holmes", email = "richard@shedc.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -24,15 +24,15 @@
 [project.urls]
 Homepage = "https://github.com/sHedC/python-masterthermconnect"
 
 [project.scripts]
 masterthermconnect = "masterthermconnect.__main__:main"
 
 [tool.bumpver]
-current_version = "2.2.3"
+current_version = "2.2.4"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `masterthermconnect-2.2.3/setup.cfg` & `masterthermconnect-2.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/tests/test_api_new.py` & `masterthermconnect-2.2.4/tests/test_api_new.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/tests/test_api_old.py` & `masterthermconnect-2.2.4/tests/test_api_old.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/tests/test_config_data.py` & `masterthermconnect-2.2.4/tests/test_config_data.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.3/tests/test_controller.py` & `masterthermconnect-2.2.4/tests/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,39 @@
     assert len(mock_get_device_data.mock_calls) > 0
 
     data = controller.get_device_data("0524", "4")
 
     assert data["operating_mode"] == "idle"
 
 
+async def test_operating_mode_cooling():
+    """Test the Passive Cooling Operating Mode."""
+    controller = MasterthermController(
+        VALID_LOGIN["uname"], VALID_LOGIN["upwd"], ClientSession()
+    )
+    mockconnect = ConnectionMock(api_version="v2")
+
+    with patch(
+        "masterthermconnect.api.MasterthermAPI.connect",
+        return_value=mockconnect.connect(),
+    ), patch(
+        "masterthermconnect.api.MasterthermAPI.get_device_info",
+        side_effect=mockconnect.get_device_info,
+    ), patch(
+        "masterthermconnect.api.MasterthermAPI.get_device_data",
+        side_effect=mockconnect.get_device_data,
+    ):
+        assert await controller.connect() is True
+        assert await controller.refresh() is True
+
+    data = controller.get_device_data("10021", "2")
+
+    assert data["operating_mode"] == "cooling"
+
+
 async def test_operating_mode_heating():
     """Test the Controller Operating Mode."""
     controller = MasterthermController(
         VALID_LOGIN["uname"], VALID_LOGIN["upwd"], ClientSession()
     )
     mockconnect = ConnectionMock()
```

### Comparing `masterthermconnect-2.2.3/tests/test_main.py` & `masterthermconnect-2.2.4/tests/test_main.py`

 * *Files identical despite different names*

