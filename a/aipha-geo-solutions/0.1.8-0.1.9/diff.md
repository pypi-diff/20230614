# Comparing `tmp/aipha_geo_solutions-0.1.8.tar.gz` & `tmp/aipha_geo_solutions-0.1.9.tar.gz`

## Comparing `aipha_geo_solutions-0.1.8.tar` & `aipha_geo_solutions-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/example.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/__init__.py
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/operators.py
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/webservice_api.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/LICENSE
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/example.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/__init__.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/operators.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/webservice_api.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/LICENSE
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/PKG-INFO
```

### Comparing `aipha_geo_solutions-0.1.8/example.py` & `aipha_geo_solutions-0.1.9/example.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/operators.py` & `aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/operators.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.8/src/aipha_geo_solutions/webservice_api.py` & `aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/webservice_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,22 @@
           'customerPassword': password, \
             }
   url = 'https://' + server_address +':443/get-running-services'
   r = requests.post(url, json=payload, verify=verifySSL)
   try:
     result = json.loads(r.text)
     if 'error' in result:
-      raise RuntimeError('AIPHAProcessingError: ' + result['error'])
+      for idx in range(10): #10 times retry
+        time.sleep(60)
+        r = requests.post(url, json=payload, verify=verifySSL)
+        result = json.loads(r.text)
+        if not 'error' in result:
+            break
+      if 'error' in result:
+        raise RuntimeError('AIPHAProcessingError: ' + str(result['error']))
   except:
       raise RuntimeError('AIPHAProcessingError: ' + r.text)
   return result
 
 def check_services_completed(
         username,
         password,
```

### Comparing `aipha_geo_solutions-0.1.8/LICENSE` & `aipha_geo_solutions-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.8/pyproject.toml` & `aipha_geo_solutions-0.1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aipha_geo_solutions"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Timo Hackel", email="timo.hackel@aipha.ch" },
 ]
 description = "A python API to the AIPHA webservices"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `aipha_geo_solutions-0.1.8/PKG-INFO` & `aipha_geo_solutions-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipha_geo_solutions
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python API to the AIPHA webservices
 Project-URL: Homepage, https://github.com/AIPHA-Geo-Solutions/
 Project-URL: Bug Tracker, https://github.com/AIPHA-Geo-Solutions/AIPHAPythonAPI/issues
 Author-email: Timo Hackel <timo.hackel@aipha.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

