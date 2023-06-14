# Comparing `tmp/vavacars_data_utils-0.0.8.tar.gz` & `tmp/vavacars_data_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/acg/repositories/Data.Utils/dist/tmp4x397gfb/vavacars_data_utils-0.0.8.tar", last modified: Tue Dec 21 12:33:55 2021, max compression
+gzip compressed data, was "/home/acg/repositories/Data.Utils/dist/tmpp9_thcst/vavacars_data_utils-0.0.9.tar", last modified: Tue Dec 21 14:50:33 2021, max compression
```

## Comparing `vavacars_data_utils-0.0.8.tar` & `vavacars_data_utils-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/
--rw-r--r--   0 acg       (1000) acg       (1000)     1304 2021-12-17 09:48:29.000000 vavacars_data_utils-0.0.8/README.md
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vava_utils/
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vava_utils/turkey/
--rw-r--r--   0 acg       (1000) acg       (1000)      888 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.8/vava_utils/turkey/dates.py
--rw-r--r--   0 acg       (1000) acg       (1000)      148 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.8/vava_utils/turkey/__init__.py
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vava_utils/smartiq/
--rw-r--r--   0 acg       (1000) acg       (1000)     4435 2021-12-21 12:33:24.000000 vavacars_data_utils-0.0.8/vava_utils/smartiq/smartiq_helper.py
--rw-r--r--   0 acg       (1000) acg       (1000)       85 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.8/vava_utils/smartiq/__init__.py
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vava_utils/utils/
--rw-r--r--   0 acg       (1000) acg       (1000)     1277 2021-12-17 09:47:00.000000 vavacars_data_utils-0.0.8/vava_utils/utils/comparisons.py
--rw-r--r--   0 acg       (1000) acg       (1000)       81 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.8/vava_utils/utils/__init__.py
--rw-r--r--   0 acg       (1000) acg       (1000)        0 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.8/vava_utils/__init__.py
--rw-r--r--   0 acg       (1000) acg       (1000)      104 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.8/pyproject.toml
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vavacars_data_utils.egg-info/
--rw-r--r--   0 acg       (1000) acg       (1000)       11 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vavacars_data_utils.egg-info/top_level.txt
--rw-r--r--   0 acg       (1000) acg       (1000)        1 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vavacars_data_utils.egg-info/dependency_links.txt
--rw-r--r--   0 acg       (1000) acg       (1000)      471 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vavacars_data_utils.egg-info/SOURCES.txt
--rw-r--r--   0 acg       (1000) acg       (1000)        7 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vavacars_data_utils.egg-info/requires.txt
--rw-r--r--   0 acg       (1000) acg       (1000)     1810 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/vavacars_data_utils.egg-info/PKG-INFO
--rw-r--r--   0 acg       (1000) acg       (1000)      673 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/setup.cfg
--rw-r--r--   0 acg       (1000) acg       (1000)     1810 2021-12-21 12:33:55.000000 vavacars_data_utils-0.0.8/PKG-INFO
+drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/
+-rw-r--r--   0 acg       (1000) acg       (1000)     1297 2021-12-21 14:42:35.000000 vavacars_data_utils-0.0.9/README.md
+drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/
+drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/turkey/
+-rw-r--r--   0 acg       (1000) acg       (1000)      888 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/turkey/dates.py
+-rw-r--r--   0 acg       (1000) acg       (1000)      148 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/turkey/__init__.py
+drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/smartiq/
+-rw-r--r--   0 acg       (1000) acg       (1000)     4759 2021-12-21 14:49:56.000000 vavacars_data_utils-0.0.9/vava_utils/smartiq/smartiq_helper.py
+-rw-r--r--   0 acg       (1000) acg       (1000)       85 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/smartiq/__init__.py
+drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/utils/
+-rw-r--r--   0 acg       (1000) acg       (1000)     1277 2021-12-21 14:42:35.000000 vavacars_data_utils-0.0.9/vava_utils/utils/comparisons.py
+-rw-r--r--   0 acg       (1000) acg       (1000)       81 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/utils/__init__.py
+-rw-r--r--   0 acg       (1000) acg       (1000)        0 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/__init__.py
+-rw-r--r--   0 acg       (1000) acg       (1000)      104 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/pyproject.toml
+drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/
+-rw-r--r--   0 acg       (1000) acg       (1000)       11 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/top_level.txt
+-rw-r--r--   0 acg       (1000) acg       (1000)        1 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 acg       (1000) acg       (1000)      471 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 acg       (1000) acg       (1000)        7 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/requires.txt
+-rw-r--r--   0 acg       (1000) acg       (1000)     1803 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/PKG-INFO
+-rw-r--r--   0 acg       (1000) acg       (1000)      673 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/setup.cfg
+-rw-r--r--   0 acg       (1000) acg       (1000)     1803 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/PKG-INFO
```

### Comparing `vavacars_data_utils-0.0.8/README.md` & `vavacars_data_utils-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,12 +48,12 @@
 ```
 python3 -m pip install --upgrade twine
 ```
 
 And then you can publish it running (from this folder), it will ask you for credentials in the registry:
 
 ```
-twine upload -r VavaCars.DS dist/*
+twine upload -r pypi dist/*
 ```
 
 For more details, check:
 https://packaging.python.org/en/latest/tutorials/packaging-projects/
```

### Comparing `vavacars_data_utils-0.0.8/vava_utils/turkey/dates.py` & `vavacars_data_utils-0.0.9/vava_utils/turkey/dates.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-0.0.8/vava_utils/smartiq/smartiq_helper.py` & `vavacars_data_utils-0.0.9/vava_utils/smartiq/smartiq_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         self._url_basewizard = url_basewizard
         self._url_quotation = url_quotation
         self._auth_dict = {
             "apiUser": api_user,
             "apiKey": api_key
         }
 
+        self.wizard_cache = {}
+
     def getWizardId(self, query_string, keyname, value):
         '''
         Gets an id using the SmartIQ Wizard. Id could be for year, brand, make, model, fuel, transmission or trim
 
         Parameters:
             query_string (str): query string (including url) to invoke wizard
             keyname (str): "BrandId"/"ModelId"/...
@@ -32,14 +34,19 @@
         Returns:
             new_query_string (str): Next query string (adding &keyname=bestid)
             best_value: value that was a closer match to the one requested
 
         Raises:
             Exception if there is no valid value (similar to the one we are looking)
         '''
+        # Look in cache
+        if value in self.wizard_cache:
+            return f"{query_string}&{keyname}={self.wizard_cache[value]}", value
+
+
         try:
             x = requests.post(query_string, json=self._auth_dict)
         except Exception as e:
             msg = f"Error when querying wizard: {e}"
             raise Exception({'message' : str(e), 'wrong_value': value})
         
         items = json.loads(x.text)['data']['items']
@@ -50,14 +57,20 @@
         if best_score < 0.5:
             msg = f"Wrong combination of features with: {query_string.split('?')[1]} + {keyname}: {value}, best was {best_value} with {best_score}"
             logging.warn(msg)
 
             raise Exception({'message': msg, 'wrong_value': value})
 
         best_id = rev_dic[best_value]
+
+        # Cache values
+        self.wizard_cache.update(rev_dic)
+        if best_value != value:
+            self.wizard_cache[value] = best_id
+
         return f"{query_string}&{keyname}={best_id}", best_value
 
     def get_quotation(self, car):
         '''
         Gets an quotation for a vehicle
 
         Parameters:
```

### Comparing `vavacars_data_utils-0.0.8/vava_utils/utils/comparisons.py` & `vavacars_data_utils-0.0.9/vava_utils/utils/comparisons.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-0.0.8/vavacars_data_utils.egg-info/PKG-INFO` & `vavacars_data_utils-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vavacars-data-utils
-Version: 0.0.8
+Name: vavacars_data_utils
+Version: 0.0.9
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/VavaCars/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 License: UNKNOWN
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/VavaCars/_git/Data.Utils/issues
 Platform: UNKNOWN
@@ -63,14 +63,14 @@
 ```
 python3 -m pip install --upgrade twine
 ```
 
 And then you can publish it running (from this folder), it will ask you for credentials in the registry:
 
 ```
-twine upload -r VavaCars.DS dist/*
+twine upload -r pypi dist/*
 ```
 
 For more details, check:
 https://packaging.python.org/en/latest/tutorials/packaging-projects/
```

### Comparing `vavacars_data_utils-0.0.8/setup.cfg` & `vavacars_data_utils-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vavacars_data_utils
-version = 0.0.8
+version = 0.0.9
 author = Vavacars Data Science Team
 author_email = acg@vava.cars
 description = Package with utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://dev.azure.com/vavacars/VavaCars/_git/Data.Utils
 project_urls =
```

### Comparing `vavacars_data_utils-0.0.8/PKG-INFO` & `vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vavacars_data_utils
-Version: 0.0.8
+Name: vavacars-data-utils
+Version: 0.0.9
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/VavaCars/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 License: UNKNOWN
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/VavaCars/_git/Data.Utils/issues
 Platform: UNKNOWN
@@ -63,14 +63,14 @@
 ```
 python3 -m pip install --upgrade twine
 ```
 
 And then you can publish it running (from this folder), it will ask you for credentials in the registry:
 
 ```
-twine upload -r VavaCars.DS dist/*
+twine upload -r pypi dist/*
 ```
 
 For more details, check:
 https://packaging.python.org/en/latest/tutorials/packaging-projects/
```

