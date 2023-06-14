# Comparing `tmp/purpleair_api-1.0.1a2.tar.gz` & `tmp/purpleair_api-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purpleair_api-1.0.1a2.tar", last modified: Wed Feb 22 05:32:12 2023, max compression
+gzip compressed data, was "purpleair_api-1.0.2a1.tar", last modified: Thu May 18 04:42:14 2023, max compression
```

## Comparing `purpleair_api-1.0.1a2.tar` & `purpleair_api-1.0.2a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 05:32:12.802985 purpleair_api-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-22 05:32:04.000000 purpleair_api-1.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-02-22 05:32:12.802985 purpleair_api-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-02-22 05:32:04.000000 purpleair_api-1.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 05:32:12.798985 purpleair_api-1.0.1a2/purpleair_api/
--rw-r--r--   0 runner    (1001) docker     (123)    43673 2023-02-22 05:32:04.000000 purpleair_api-1.0.1a2/purpleair_api/PurpleAirAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-02-22 05:32:04.000000 purpleair_api-1.0.1a2/purpleair_api/PurpleAirAPIConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 05:32:04.000000 purpleair_api-1.0.1a2/purpleair_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 05:32:12.802985 purpleair_api-1.0.1a2/purpleair_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-02-22 05:32:12.000000 purpleair_api-1.0.1a2/purpleair_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-22 05:32:12.000000 purpleair_api-1.0.1a2/purpleair_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 05:32:12.000000 purpleair_api-1.0.1a2/purpleair_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 05:32:12.000000 purpleair_api-1.0.1a2/purpleair_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 05:32:12.000000 purpleair_api-1.0.1a2/purpleair_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-22 05:32:12.802985 purpleair_api-1.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-22 05:32:04.000000 purpleair_api-1.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/purpleair_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    43928 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPIConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/purpleair_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:42:14.399680 purpleair_api-1.0.2a1/purpleair_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 04:42:14.000000 purpleair_api-1.0.2a1/purpleair_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-18 04:42:14.403680 purpleair_api-1.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 04:42:05.000000 purpleair_api-1.0.2a1/setup.py
```

### Comparing `purpleair_api-1.0.1a2/LICENSE` & `purpleair_api-1.0.2a1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 carlkid1499
+Copyright (c) 2023 carlkidcrypto
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `purpleair_api-1.0.1a2/PKG-INFO` & `purpleair_api-1.0.2a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: purpleair_api
-Version: 1.0.1a2
-Home-page: https://github.com/carlkid1499/purpleair_api
+Version: 1.0.2a1
+Home-page: https://github.com/carlkidcrypto/purpleair_api
 Author: Carlos Santos
-Author-email: 27721404+carlkid1499@users.noreply.github.com
+Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_api,purple air api,purple_air,purple air
 Platform: Windows 32/64
 Platform: Linux 32/64
 Platform: MacOS 32/64
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # purple_air_api (PAA)
 
 This is a python3 wrapper for the new PurpleAirAPI (PAA). Details of the API can be found using this link: <https://api.purpleair.com/#api-welcome>
 To use the PurpleAirAPI (PAA) api keys are required. You can get API keys by sending an email to `contact@purpleair.com` with a first and last name to assign them to.
 
-| [![PyPI Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml) |
+| [![PyPI Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml) |
 | --------------- | --------------- | --------------- |
 
 ## How to Support This Project
 
-<a href="https://www.buymeacoffee.com/carlkid1499" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/carlkidcrypto" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 ## Purpose
 
 This package is designed to be used for making tools around the PurpleAir API.
 
-For example, PAA data loggers - <https://github.com/carlkid1499/purpleair_data_logger>
+For example, PAA data loggers - <https://github.com/carlkidcrypto/purpleair_data_logger>
 
 ## Installation
 
 You can install the PurpleAir API via pip.
 
 ```bash
 python3 -m pip install purple_air_api
 ```
 
 You can install PurpleAir API by cloning down this repo.
 
 ```bash
-git clone https://github.com/carlkid1499/purple_air_api.git
+git clone https://github.com/carlkidcrypto/purple_air_api.git
 cd purple_air_api
 python3 setup.py install
 ```
 
 ## Usage Example
 
 First we need to import the PurpleAir API (PAA)
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: purpleair_api Version: 1.0.1a2 Home-page: https://
-github.com/carlkid1499/purpleair_api Author: Carlos Santos Author-email:
-27721404+carlkid1499@users.noreply.github.com License: MIT Keywords:
-purpleair_api,purple air api,purple_air,purple air Platform: Windows 32/64
-Platform: Linux 32/64 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE # purple_air_api (PAA) This
-is a python3 wrapper for the new PurpleAirAPI (PAA). Details of the API can be
-found using this link:
+Metadata-Version: 2.1 Name: purpleair_api Version: 1.0.2a1 Home-page: https://
+github.com/carlkidcrypto/purpleair_api Author: Carlos Santos Author-email:
+dose.lucky.sake@cloak.id License: MIT Keywords: purpleair_api,purple air
+api,purple_air,purple air Platform: Windows 32/64 Platform: Linux 32/64
+Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE # purple_air_api (PAA) This is a python3 wrapper
+for the new PurpleAirAPI (PAA). Details of the API can be found using this
+link:
 api.purpleair.com/#api-welcome> To use the PurpleAirAPI (PAA) api keys are
 required. You can get API keys by sending an email to `contact@purpleair.com`
 with a first and last name to assign them to. | [![PyPI Distributions](https://
-github.com/carlkid1499/purpleair_api/actions/workflows/
-build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkid1499/
+github.com/carlkidcrypto/purpleair_api/actions/workflows/
+build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/
 purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI
-Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/
-build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkid1499/
-purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black]
-(https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml/
-badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/
-black.yml) | | --------------- | --------------- | --------------- | ## How to
-Support This Project [Buy_Me_A_Coffee] ## Purpose This package is designed to
-be used for making tools around the PurpleAir API. For example, PAA data
-loggers -
-github.com/carlkid1499/purpleair_data_logger> ## Installation You can install
+Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/
+workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/
+carlkidcrypto/purpleair_api/actions/workflows/
+build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/
+carlkidcrypto/purpleair_api/actions/workflows/black.yml/badge.svg)](https://
+github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml) | | -------
+-------- | --------------- | --------------- | ## How to Support This Project
+[Buy_Me_A_Coffee] ## Purpose This package is designed to be used for making
+tools around the PurpleAir API. For example, PAA data loggers -
+github.com/carlkidcrypto/purpleair_data_logger> ## Installation You can install
 the PurpleAir API via pip. ```bash python3 -m pip install purple_air_api ```
 You can install PurpleAir API by cloning down this repo. ```bash git clone
-https://github.com/carlkid1499/purple_air_api.git cd purple_air_api python3
+https://github.com/carlkidcrypto/purple_air_api.git cd purple_air_api python3
 setup.py install ``` ## Usage Example First we need to import the PurpleAir API
 (PAA) ```bash from purpleair_api.PurpleAirAPI ``` Next we need to make an
 instance of PAA. ```bash my_paa = PurpleAirAPI(your_api_read_key,
 your_api_write_key) ``` Now you can use that PAA instance to do things like...
 ```bash retval = my_paa.request_sensor_data(1234) ```
```

### Comparing `purpleair_api-1.0.1a2/README.md` & `purpleair_api-1.0.2a1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # purple_air_api (PAA)
 
 This is a python3 wrapper for the new PurpleAirAPI (PAA). Details of the API can be found using this link: <https://api.purpleair.com/#api-welcome>
 To use the PurpleAirAPI (PAA) api keys are required. You can get API keys by sending an email to `contact@purpleair.com` with a first and last name to assign them to.
 
-| [![PyPI Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml) |
+| [![PyPI Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml) |
 | --------------- | --------------- | --------------- |
 
 ## How to Support This Project
 
-<a href="https://www.buymeacoffee.com/carlkid1499" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/carlkidcrypto" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 ## Purpose
 
 This package is designed to be used for making tools around the PurpleAir API.
 
-For example, PAA data loggers - <https://github.com/carlkid1499/purpleair_data_logger>
+For example, PAA data loggers - <https://github.com/carlkidcrypto/purpleair_data_logger>
 
 ## Installation
 
 You can install the PurpleAir API via pip.
 
 ```bash
 python3 -m pip install purple_air_api
 ```
 
 You can install PurpleAir API by cloning down this repo.
 
 ```bash
-git clone https://github.com/carlkid1499/purple_air_api.git
+git clone https://github.com/carlkidcrypto/purple_air_api.git
 cd purple_air_api
 python3 setup.py install
 ```
 
 ## Usage Example
 
 First we need to import the PurpleAir API (PAA)
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
 # purple_air_api (PAA) This is a python3 wrapper for the new PurpleAirAPI
 (PAA). Details of the API can be found using this link:
 api.purpleair.com/#api-welcome> To use the PurpleAirAPI (PAA) api keys are
 required. You can get API keys by sending an email to `contact@purpleair.com`
 with a first and last name to assign them to. | [![PyPI Distributions](https://
-github.com/carlkid1499/purpleair_api/actions/workflows/
-build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkid1499/
+github.com/carlkidcrypto/purpleair_api/actions/workflows/
+build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/
 purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI
-Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/
-build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkid1499/
-purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black]
-(https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml/
-badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/
-black.yml) | | --------------- | --------------- | --------------- | ## How to
-Support This Project [Buy_Me_A_Coffee] ## Purpose This package is designed to
-be used for making tools around the PurpleAir API. For example, PAA data
-loggers -
-github.com/carlkid1499/purpleair_data_logger> ## Installation You can install
+Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/
+workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/
+carlkidcrypto/purpleair_api/actions/workflows/
+build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/
+carlkidcrypto/purpleair_api/actions/workflows/black.yml/badge.svg)](https://
+github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml) | | -------
+-------- | --------------- | --------------- | ## How to Support This Project
+[Buy_Me_A_Coffee] ## Purpose This package is designed to be used for making
+tools around the PurpleAir API. For example, PAA data loggers -
+github.com/carlkidcrypto/purpleair_data_logger> ## Installation You can install
 the PurpleAir API via pip. ```bash python3 -m pip install purple_air_api ```
 You can install PurpleAir API by cloning down this repo. ```bash git clone
-https://github.com/carlkid1499/purple_air_api.git cd purple_air_api python3
+https://github.com/carlkidcrypto/purple_air_api.git cd purple_air_api python3
 setup.py install ``` ## Usage Example First we need to import the PurpleAir API
 (PAA) ```bash from purpleair_api.PurpleAirAPI ``` Next we need to make an
 instance of PAA. ```bash my_paa = PurpleAirAPI(your_api_read_key,
 your_api_write_key) ``` Now you can use that PAA instance to do things like...
 ```bash retval = my_paa.request_sensor_data(1234) ```
```

### Comparing `purpleair_api-1.0.1a2/purpleair_api/PurpleAirAPI.py` & `purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2023 carlkid1499, All rights reserved.
+    Copyright 2023 carlkidcrypto, All rights reserved.
     A python3 class designed to fetch data from Purple Air's new API.
     https://api.purpleair.com/#api-welcome
 """
 
 import requests
 import json
 from purpleair_api.PurpleAirAPIConstants import (
@@ -795,21 +795,24 @@
                         request_url = request_url + f"&{opt_param}={str(val)}"
 
         # Strip any quotes that might persist
         request_url = request_url.replace('"', "")
         # Strip away any whitespace that might persist
         request_url = request_url.replace(" ", "")
         debug_log(request_url)
+        my_request = None
         my_request = requests.get(
             request_url, headers={"X-API-Key": str(api_key_to_use)}
         )
 
         the_request_text_as_json = self._convert_requests_text_to_json(my_request.text)
 
         if self._verify_request_status_codes(my_request.status_code):
+            my_request.close()
+            del my_request
             return the_request_text_as_json
 
         else:
             raise PurpleAirAPIError(
                 f"""{my_request.status_code}: {the_request_text_as_json['error']} - {the_request_text_as_json['description']}"""
             )
 
@@ -820,14 +823,15 @@
         A class helper to send the url request. It can also add onto the
         'request_url' string if 'optional_parameters_dict' are provided.
 
         :param str request_url: The constructed string url request string.
         """
 
         debug_log(request_url)
+        my_request = None
         if json_post_parameters:
             debug_log(json_post_parameters)
             my_request = requests.post(
                 request_url,
                 headers={"X-API-Key": str(api_key_to_use)},
                 json=json_post_parameters,
             )
@@ -837,14 +841,16 @@
             my_request = requests.post(
                 request_url, headers={"X-API-Key": str(api_key_to_use)}
             )
 
         the_request_text_as_json = self._convert_requests_text_to_json(my_request.text)
 
         if self._verify_request_status_codes(my_request.status_code):
+            my_request.close()
+            del my_request
             return the_request_text_as_json
 
         else:
             raise PurpleAirAPIError(
                 f"""{my_request.status_code}: {the_request_text_as_json['error']} - {the_request_text_as_json['description']}"""
             )
 
@@ -855,14 +861,15 @@
         A class helper to send the url request. It can also add onto the
         'request_url' string if 'optional_parameters_dict' are provided.
 
         :param str request_url: The constructed string url request string.
         """
 
         debug_log(request_url)
+        my_request = None
         if json_post_parameters:
             my_request = requests.delete(
                 request_url,
                 headers={"X-API-Key": str(api_key_to_use)},
                 json=json_post_parameters,
             )
 
@@ -870,14 +877,16 @@
             my_request = requests.delete(
                 request_url, headers={"X-API-Key": str(api_key_to_use)}
             )
 
         the_request_text_as_json = self._convert_requests_text_to_json(my_request.text)
 
         if self._verify_request_status_codes(my_request.status_code):
+            my_request.close()
+            del my_request
             return the_request_text_as_json
 
         else:
             raise PurpleAirAPIError(
                 f"""{my_request.status_code}: {the_request_text_as_json['error']} - {the_request_text_as_json['description']}"""
             )
 
@@ -903,18 +912,19 @@
         :param str text: The request.txt to convert to json
 
         :return dict
         """
 
         the_request_text_as_json = None
         if text:
-            # For now encode as UTF-8. The PAA documentation mentions nothing about what
-            # encoding method they use.
-            the_request_text_as_json = json.loads(text.encode("UTF-8"))
-            debug_log(the_request_text_as_json)
+            debug_log(f"_convert_requests_text_to_json - text: {text}")
+            the_request_text_as_json = json.loads(text)
+            debug_log(
+                f"_convert_requests_text_to_json - json: {the_request_text_as_json}"
+            )
 
         return the_request_text_as_json
 
     @staticmethod
     def _sanitize_sensor_data_from_paa(paa_return_data) -> dict:
         """
         A helper method.
```

### Comparing `purpleair_api-1.0.1a2/purpleair_api/PurpleAirAPIConstants.py` & `purpleair_api-1.0.2a1/purpleair_api/PurpleAirAPIConstants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2023 carlkid1499, All rights reserved.
+    Copyright 2023 carlkidcrypto, All rights reserved.
     A python with constants with for use in PurpleAirAPI.py
 """
 
 #: A constant to see if debug statements are enabled in the PurpleAirAPI module.
 PRINT_DEBUG_MSGS = False
 
 #: Accepted Error Codes
```

### Comparing `purpleair_api-1.0.1a2/purpleair_api.egg-info/PKG-INFO` & `purpleair_api-1.0.2a1/purpleair_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: purpleair-api
-Version: 1.0.1a2
-Home-page: https://github.com/carlkid1499/purpleair_api
+Version: 1.0.2a1
+Home-page: https://github.com/carlkidcrypto/purpleair_api
 Author: Carlos Santos
-Author-email: 27721404+carlkid1499@users.noreply.github.com
+Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_api,purple air api,purple_air,purple air
 Platform: Windows 32/64
 Platform: Linux 32/64
 Platform: MacOS 32/64
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # purple_air_api (PAA)
 
 This is a python3 wrapper for the new PurpleAirAPI (PAA). Details of the API can be found using this link: <https://api.purpleair.com/#api-welcome>
 To use the PurpleAirAPI (PAA) api keys are required. You can get API keys by sending an email to `contact@purpleair.com` with a first and last name to assign them to.
 
-| [![PyPI Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml/badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml) |
+| [![PyPI Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml) |
 | --------------- | --------------- | --------------- |
 
 ## How to Support This Project
 
-<a href="https://www.buymeacoffee.com/carlkid1499" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/carlkidcrypto" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 ## Purpose
 
 This package is designed to be used for making tools around the PurpleAir API.
 
-For example, PAA data loggers - <https://github.com/carlkid1499/purpleair_data_logger>
+For example, PAA data loggers - <https://github.com/carlkidcrypto/purpleair_data_logger>
 
 ## Installation
 
 You can install the PurpleAir API via pip.
 
 ```bash
 python3 -m pip install purple_air_api
 ```
 
 You can install PurpleAir API by cloning down this repo.
 
 ```bash
-git clone https://github.com/carlkid1499/purple_air_api.git
+git clone https://github.com/carlkidcrypto/purple_air_api.git
 cd purple_air_api
 python3 setup.py install
 ```
 
 ## Usage Example
 
 First we need to import the PurpleAir API (PAA)
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: purpleair-api Version: 1.0.1a2 Home-page: https://
-github.com/carlkid1499/purpleair_api Author: Carlos Santos Author-email:
-27721404+carlkid1499@users.noreply.github.com License: MIT Keywords:
-purpleair_api,purple air api,purple_air,purple air Platform: Windows 32/64
-Platform: Linux 32/64 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE # purple_air_api (PAA) This
-is a python3 wrapper for the new PurpleAirAPI (PAA). Details of the API can be
-found using this link:
+Metadata-Version: 2.1 Name: purpleair-api Version: 1.0.2a1 Home-page: https://
+github.com/carlkidcrypto/purpleair_api Author: Carlos Santos Author-email:
+dose.lucky.sake@cloak.id License: MIT Keywords: purpleair_api,purple air
+api,purple_air,purple air Platform: Windows 32/64 Platform: Linux 32/64
+Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE # purple_air_api (PAA) This is a python3 wrapper
+for the new PurpleAirAPI (PAA). Details of the API can be found using this
+link:
 api.purpleair.com/#api-welcome> To use the PurpleAirAPI (PAA) api keys are
 required. You can get API keys by sending an email to `contact@purpleair.com`
 with a first and last name to assign them to. | [![PyPI Distributions](https://
-github.com/carlkid1499/purpleair_api/actions/workflows/
-build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkid1499/
+github.com/carlkidcrypto/purpleair_api/actions/workflows/
+build_and_publish_to_pypi.yml/badge.svg)](https://github.com/carlkidcrypto/
 purpleair_api/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI
-Distributions](https://github.com/carlkid1499/purpleair_api/actions/workflows/
-build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/carlkid1499/
-purpleair_api/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black]
-(https://github.com/carlkid1499/purpleair_api/actions/workflows/black.yml/
-badge.svg)](https://github.com/carlkid1499/purpleair_api/actions/workflows/
-black.yml) | | --------------- | --------------- | --------------- | ## How to
-Support This Project [Buy_Me_A_Coffee] ## Purpose This package is designed to
-be used for making tools around the PurpleAir API. For example, PAA data
-loggers -
-github.com/carlkid1499/purpleair_data_logger> ## Installation You can install
+Distributions](https://github.com/carlkidcrypto/purpleair_api/actions/
+workflows/build_and_publish_to_test_pypi.yml/badge.svg)](https://github.com/
+carlkidcrypto/purpleair_api/actions/workflows/
+build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/
+carlkidcrypto/purpleair_api/actions/workflows/black.yml/badge.svg)](https://
+github.com/carlkidcrypto/purpleair_api/actions/workflows/black.yml) | | -------
+-------- | --------------- | --------------- | ## How to Support This Project
+[Buy_Me_A_Coffee] ## Purpose This package is designed to be used for making
+tools around the PurpleAir API. For example, PAA data loggers -
+github.com/carlkidcrypto/purpleair_data_logger> ## Installation You can install
 the PurpleAir API via pip. ```bash python3 -m pip install purple_air_api ```
 You can install PurpleAir API by cloning down this repo. ```bash git clone
-https://github.com/carlkid1499/purple_air_api.git cd purple_air_api python3
+https://github.com/carlkidcrypto/purple_air_api.git cd purple_air_api python3
 setup.py install ``` ## Usage Example First we need to import the PurpleAir API
 (PAA) ```bash from purpleair_api.PurpleAirAPI ``` Next we need to make an
 instance of PAA. ```bash my_paa = PurpleAirAPI(your_api_read_key,
 your_api_write_key) ``` Now you can use that PAA instance to do things like...
 ```bash retval = my_paa.request_sensor_data(1234) ```
```

### Comparing `purpleair_api-1.0.1a2/setup.py` & `purpleair_api-1.0.2a1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
         os.path.join(os.path.dirname(__file__), filename), encoding="utf-8"
     ) as file:
         return file.read()
 
 
 setup(
     name="purpleair_api",
-    version="1.0.1a2",
+    version="1.0.2a1",
     license="MIT",
     author="Carlos Santos",
-    author_email="27721404+carlkid1499@users.noreply.github.com",
+    author_email="dose.lucky.sake@cloak.id",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     packages=["purpleair_api"],
-    url="https://github.com/carlkid1499/purpleair_api",
+    url="https://github.com/carlkidcrypto/purpleair_api",
     keywords=["purpleair_api", "purple air api", "purple_air", "purple air"],
     install_requires=["requests"],
     platforms=["Windows 32/64", "Linux 32/64", "MacOS 32/64"],
 )
```

