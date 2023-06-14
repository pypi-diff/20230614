# Comparing `tmp/whatsapp-api-client-python-0.0.35.tar.gz` & `tmp/whatsapp-api-client-python-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-client-python-0.0.35.tar", last modified: Wed May 24 07:21:08 2023, max compression
+gzip compressed data, was "whatsapp-api-client-python-0.0.36.tar", last modified: Fri Jun  2 09:21:10 2023, max compression
```

## Comparing `whatsapp-api-client-python-0.0.35.tar` & `whatsapp-api-client-python-0.0.36.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.785300 whatsapp-api-client-python-0.0.35/
--rw-rw-rw-   0        0        0    18130 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/LICENSE
--rw-rw-rw-   0        0        0    20699 2023-05-24 07:21:08.784297 whatsapp-api-client-python-0.0.35/PKG-INFO
--rw-rw-rw-   0        0        0    19661 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 07:21:08.785300 whatsapp-api-client-python-0.0.35/setup.cfg
--rw-rw-rw-   0        0        0     1410 2023-05-24 07:14:52.000000 whatsapp-api-client-python-0.0.35/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.768264 whatsapp-api-client-python-0.0.35/tests/
--rw-rw-rw-   0        0        0      960 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.770323 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/
--rw-rw-rw-   0        0        0     2818 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/API.py
--rw-rw-rw-   0        0        0        0 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/__init__.py
--rw-rw-rw-   0        0        0      336 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/response.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.783295 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/
--rw-rw-rw-   0        0        0        0 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/account.py
--rw-rw-rw-   0        0        0      517 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/device.py
--rw-rw-rw-   0        0        0     4680 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/groups.py
--rw-rw-rw-   0        0        0     2174 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/journals.py
--rw-rw-rw-   0        0        0      598 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/marking.py
--rw-rw-rw-   0        0        0      865 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/queues.py
--rw-rw-rw-   0        0        0     3354 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/receiving.py
--rw-rw-rw-   0        0        0     7412 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/sending.py
--rw-rw-rw-   0        0        0     4254 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/serviceMethods.py
--rw-rw-rw-   0        0        0     1265 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/webhooks.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.775274 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/
--rw-rw-rw-   0        0        0    20699 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      899 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 09:21:10.830917 whatsapp-api-client-python-0.0.36/
+-rw-rw-rw-   0        0        0    18130 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/LICENSE
+-rw-rw-rw-   0        0        0    20645 2023-06-02 09:21:10.830917 whatsapp-api-client-python-0.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0    19607 2023-06-02 09:19:18.000000 whatsapp-api-client-python-0.0.36/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:21:10.830917 whatsapp-api-client-python-0.0.36/setup.cfg
+-rw-rw-rw-   0        0        0     1410 2023-06-02 09:15:39.000000 whatsapp-api-client-python-0.0.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:21:10.729617 whatsapp-api-client-python-0.0.36/tests/
+-rw-rw-rw-   0        0        0     3879 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/tests/test_methods.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:21:10.743654 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/
+-rw-rw-rw-   0        0        0     2822 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/API.py
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/__init__.py
+-rw-rw-rw-   0        0        0      336 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/response.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:21:10.828912 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/account.py
+-rw-rw-rw-   0        0        0      517 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/device.py
+-rw-rw-rw-   0        0        0     4671 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/groups.py
+-rw-rw-rw-   0        0        0     2174 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/journals.py
+-rw-rw-rw-   0        0        0      598 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/marking.py
+-rw-rw-rw-   0        0        0      865 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/queues.py
+-rw-rw-rw-   0        0        0     3354 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/receiving.py
+-rw-rw-rw-   0        0        0     7412 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/sending.py
+-rw-rw-rw-   0        0        0     4254 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/serviceMethods.py
+-rw-rw-rw-   0        0        0     1257 2023-05-30 11:54:45.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/webhooks.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:21:10.768719 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/
+-rw-rw-rw-   0        0        0    20645 2023-06-02 09:21:10.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      902 2023-06-02 09:21:10.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:21:10.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-02 09:21:10.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-02 09:21:10.000000 whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/top_level.txt
```

### Comparing `whatsapp-api-client-python-0.0.35/LICENSE` & `whatsapp-api-client-python-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/PKG-INFO` & `whatsapp-api-client-python-0.0.36/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-client-python
-Version: 0.0.35
+Version: 0.0.36
 Summary: This library helps you easily create a Python application with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-api-client-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,16 +19,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿# whatsapp-api-client-python
 
-[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
+![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-api-client-python)
+![](https://img.shields.io/pypi/pyversions/whatsapp-api-client-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-client-python/python-package.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-api-client-python)
 
 - [Документация на русском языке](README_RUS.md)
 
 Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com/en/) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
 
 ## API
```

### Comparing `whatsapp-api-client-python-0.0.35/README.md` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,37 @@
+Metadata-Version: 2.1
+Name: whatsapp-api-client-python
+Version: 0.0.36
+Summary: This library helps you easily create a Python application with WhatsApp API.
+Home-page: https://github.com/green-api/whatsapp-api-client-python
+Author: GREEN API
+Author-email: support@green-api.com
+License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ﻿# whatsapp-api-client-python
 
-[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
+![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-api-client-python)
+![](https://img.shields.io/pypi/pyversions/whatsapp-api-client-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-client-python/python-package.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-api-client-python)
 
 - [Документация на русском языке](README_RUS.md)
 
 Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com/en/) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
 
 ## API
 
@@ -186,8 +212,8 @@
 
 This work is licensed under a
 [Creative Commons Attribution-NoDerivatives 4.0 International License][cc-by-nd].
 
 [cc-by-nd]: https://creativecommons.org/licenses/by-nd/4.0/
 [cc-by-nd-shield]: https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg
 
-Please see file [LICENSE](LICENSE)
+Please see file [LICENSE](LICENSE)
```

### Comparing `whatsapp-api-client-python-0.0.35/setup.py` & `whatsapp-api-client-python-0.0.36/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-api-client-python",
-    version="0.0.35",
+    version="0.0.36",
     description=(
         "This library helps you easily create"
         " a Python application with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -29,10 +29,10 @@
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
-    install_requires=["requests==2.30.0"],
+    install_requires=["requests==2.31.0"],
     python_requires=">=3.7"
 )
```

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/API.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/API.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         url = url.replace('{{idInstance}}', self.idInstance)
         url = url.replace('{{apiTokenInstance}}', self.apiTokenInstance)
         status_code = 0
         text = ''
         try:
             headers = {}
             payloadData = None
-            if payload != None:
-                if files == None:
+            if payload is not None:
+                if files is None:
                     headers = {
                         'Content-Type': 'application/json'
                     }
                     payloadData = json.dumps(payload)
                 else:
                     payloadData = payload   
             result = requests.request(method, url, headers = headers,
```

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/account.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/account.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/device.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/device.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/groups.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from array import ArrayType, array
 import os.path
+from array import array
+
 from whatsapp_api_client_python.response import Response
 
 
 class Groups:
     def __init__(self, greenApi) -> None:
         self.greenApi = greenApi
```

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/journals.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/journals.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/marking.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/marking.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/queues.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/queues.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/receiving.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/receiving.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/sending.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/sending.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/serviceMethods.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/serviceMethods.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/webhooks.py` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python/tools/webhooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
         self.started = False
 
     
     def job(self, onEvent) -> None:
         print('Incoming notifications are being received. '\
         'To interrupt, press Ctrl+C')
         try:
-            while self.started == True:
+            while self.started:
                 resultReceive = self.greenApi.receiving.receiveNotification()
                 if resultReceive.code == 200:
-                    if resultReceive.data == None:
+                    if resultReceive.data is None:
                         # There are no incoming notifications, 
                         # we send the request again
                         continue
                     body = resultReceive.data['body']
                     typeWebhook = body['typeWebhook']
                     onEvent(typeWebhook, body)    
                     self.greenApi.receiving.deleteNotification(
```

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/PKG-INFO` & `whatsapp-api-client-python-0.0.36/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,14 @@
-Metadata-Version: 2.1
-Name: whatsapp-api-client-python
-Version: 0.0.35
-Summary: This library helps you easily create a Python application with WhatsApp API.
-Home-page: https://github.com/green-api/whatsapp-api-client-python
-Author: GREEN API
-Author-email: support@green-api.com
-License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ﻿# whatsapp-api-client-python
 
-[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
+![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-api-client-python)
+![](https://img.shields.io/pypi/pyversions/whatsapp-api-client-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-client-python/python-package.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-api-client-python)
 
 - [Документация на русском языке](README_RUS.md)
 
 Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com/en/) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
 
 ## API
 
@@ -209,8 +189,8 @@
 
 This work is licensed under a
 [Creative Commons Attribution-NoDerivatives 4.0 International License][cc-by-nd].
 
 [cc-by-nd]: https://creativecommons.org/licenses/by-nd/4.0/
 [cc-by-nd-shield]: https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg
 
-Please see file [LICENSE](LICENSE)
+Please see file [LICENSE](LICENSE)
```

### Comparing `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/SOURCES.txt` & `whatsapp-api-client-python-0.0.36/whatsapp_api_client_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 README.md
 setup.py
-tests/test_main.py
+tests/test_methods.py
 whatsapp_api_client_python/API.py
 whatsapp_api_client_python/__init__.py
 whatsapp_api_client_python/response.py
 whatsapp_api_client_python.egg-info/PKG-INFO
 whatsapp_api_client_python.egg-info/SOURCES.txt
 whatsapp_api_client_python.egg-info/dependency_links.txt
 whatsapp_api_client_python.egg-info/requires.txt
```

