# Comparing `tmp/automation-common-test-2.0.0.tar.gz` & `tmp/automation-common-test-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-common-test-2.0.0.tar", last modified: Wed May 17 06:51:58 2023, max compression
+gzip compressed data, was "automation-common-test-2.0.2.tar", last modified: Wed Jun 14 14:46:45 2023, max compression
```

## Comparing `automation-common-test-2.0.0.tar` & `automation-common-test-2.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.396601 automation-common-test-2.0.0/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-17 06:51:58.396368 automation-common-test-2.0.0/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-2.0.0/README.md
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.391125 automation-common-test-2.0.0/automation_common_test.egg-info/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      487 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/SOURCES.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/dependency_links.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/top_level.txt
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.393495 automation-common-test-2.0.0/helpers/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-2.0.0/helpers/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     2597 2023-05-16 05:29:45.000000 automation-common-test-2.0.0/helpers/api_operations.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-2.0.0/helpers/base_locator.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-05-17 01:07:02.000000 automation-common-test-2.0.0/helpers/decorator.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     5157 2023-05-17 06:51:42.000000 automation-common-test-2.0.0/helpers/driver_manager.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-2.0.0/helpers/soft_check.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)    65913 2023-05-17 05:05:21.000000 automation-common-test-2.0.0/helpers/web_operations.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-05-17 06:51:58.396649 automation-common-test-2.0.0/setup.cfg
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-05-17 06:51:42.000000 automation-common-test-2.0.0/setup.py
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.395851 automation-common-test-2.0.0/utils/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-2.0.0/utils/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-2.0.0/utils/config_parser.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-2.0.0/utils/encryption_decryption.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     4112 2023-05-17 05:11:54.000000 automation-common-test-2.0.0/utils/json_utils.py
--rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4660 2023-05-09 03:29:52.000000 automation-common-test-2.0.0/utils/post_results_teams.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.816468 automation-common-test-2.0.2/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-06-14 14:46:45.816263 automation-common-test-2.0.2/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-2.0.2/README.md
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.811779 automation-common-test-2.0.2/automation_common_test.egg-info/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      487 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/top_level.txt
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.813944 automation-common-test-2.0.2/helpers/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-2.0.2/helpers/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     2715 2023-06-08 05:41:40.000000 automation-common-test-2.0.2/helpers/api_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-2.0.2/helpers/base_locator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1876 2023-06-08 03:42:00.000000 automation-common-test-2.0.2/helpers/decorator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     5164 2023-05-31 08:38:28.000000 automation-common-test-2.0.2/helpers/driver_manager.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-2.0.2/helpers/soft_check.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)    65913 2023-05-17 05:05:21.000000 automation-common-test-2.0.2/helpers/web_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-06-14 14:46:45.816523 automation-common-test-2.0.2/setup.cfg
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-06-14 14:46:43.000000 automation-common-test-2.0.2/setup.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.815865 automation-common-test-2.0.2/utils/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-2.0.2/utils/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-2.0.2/utils/config_parser.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-2.0.2/utils/encryption_decryption.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     4112 2023-05-17 05:11:54.000000 automation-common-test-2.0.2/utils/json_utils.py
+-rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4660 2023-05-09 03:29:52.000000 automation-common-test-2.0.2/utils/post_results_teams.py
```

### Comparing `automation-common-test-2.0.0/README.md` & `automation-common-test-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.0/helpers/api_operations.py` & `automation-common-test-2.0.2/helpers/api_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 import logging
 import requests
 from requests import Response, request
 import cattr
 
 def post(resource, data=None) -> Response:
     url = get_url(resource)
+    logging.info(url)
     response = request(
         method="POST",
         url=url,
+        # headers={'Content-Type': 'application/json'},
         json=data,
+        # auth=("testUser", "password")
     )
     return response
 
 
 def post_file(resource, data=None) -> Response:
     files = {'file': ('files', data, 'application/vnd.ms-excel', {'Expires': '0'})}
     url = get_url(resource)
```

### Comparing `automation-common-test-2.0.0/helpers/decorator.py` & `automation-common-test-2.0.2/helpers/decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         @wraps(function)
         def inner(*args, **kwargs):
             logger.info(message)
             res = function(*args, **kwargs)
             method = res.request.method
             url = res.request.url
             body = res.request.body
+            logger.info(res)
             status = res.status_code
             body_sep = " "
             log_request = f"Request method: {method}, url: {url}"
             if body is not None:
                 try:
                     json_body = json.loads(res.text)
                     if len(body) > 20:
```

### Comparing `automation-common-test-2.0.0/helpers/driver_manager.py` & `automation-common-test-2.0.2/helpers/driver_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         cap["marionette"] = True
         firefox_options = webdriver.FirefoxOptions()
         firefox_options.set_preference("dom.disable_beforeunload", True)
         driver = webdriver.Firefox(GeckoDriverManager.install(), options=firefox_options, capabilities=cap)
     elif browser_type == "chrome":
         chrome_options = set_chrome_options()
         if run_mode == "yes":
-            options.add_argument("--headless")
+            chrome_options.add_argument("--headless")
             chrome_options.add_argument("--window-size=1920,1080")
         warnings.filterwarnings(action="ignore", message="unclosed", category=ResourceWarning)
         driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=chrome_options)
 
     elif browser_type == "ie":
         cap = DesiredCapabilities.INTERNETEXPLORER
         cap["NATIVE_EVENTS"] = False
```

### Comparing `automation-common-test-2.0.0/helpers/soft_check.py` & `automation-common-test-2.0.2/helpers/soft_check.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.0/helpers/web_operations.py` & `automation-common-test-2.0.2/helpers/web_operations.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.0/utils/encryption_decryption.py` & `automation-common-test-2.0.2/utils/encryption_decryption.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.0/utils/json_utils.py` & `automation-common-test-2.0.2/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.0/utils/post_results_teams.py` & `automation-common-test-2.0.2/utils/post_results_teams.py`

 * *Files identical despite different names*

