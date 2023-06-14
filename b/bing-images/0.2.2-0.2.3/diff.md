# Comparing `tmp/bing_images-0.2.2.tar.gz` & `tmp/bing_images-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bing_images-0.2.2.tar", last modified: Tue Jan 25 07:45:43 2022, max compression
+gzip compressed data, was "bing_images-0.2.3.tar", last modified: Wed Jun 14 02:01:16 2023, max compression
```

## Comparing `bing_images-0.2.2.tar` & `bing_images-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 07:45:43.059242 bing_images-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-25 07:45:29.000000 bing_images-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-01-25 07:45:43.059242 bing_images-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4762 2022-01-25 07:45:29.000000 bing_images-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 07:45:43.059242 bing_images-0.2.2/bing_images/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-25 07:45:29.000000 bing_images-0.2.2/bing_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-01-25 07:45:29.000000 bing_images-0.2.2/bing_images/bing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-01-25 07:45:29.000000 bing_images-0.2.2/bing_images/crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-01-25 07:45:29.000000 bing_images-0.2.2/bing_images/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 07:45:43.059242 bing_images-0.2.2/bing_images.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-01-25 07:45:43.000000 bing_images-0.2.2/bing_images.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-01-25 07:45:43.000000 bing_images-0.2.2/bing_images.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 07:45:43.000000 bing_images-0.2.2/bing_images.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-25 07:45:43.000000 bing_images-0.2.2/bing_images.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-25 07:45:43.000000 bing_images-0.2.2/bing_images.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-01-25 07:45:29.000000 bing_images-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-01-25 07:45:43.059242 bing_images-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:16.337324 bing_images-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 02:01:01.000000 bing_images-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-14 02:01:16.337324 bing_images-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-14 02:01:01.000000 bing_images-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:16.337324 bing_images-0.2.3/bing_images/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 02:01:01.000000 bing_images-0.2.3/bing_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-14 02:01:01.000000 bing_images-0.2.3/bing_images/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-14 02:01:01.000000 bing_images-0.2.3/bing_images/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-14 02:01:01.000000 bing_images-0.2.3/bing_images/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:16.337324 bing_images-0.2.3/bing_images.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-14 02:01:16.000000 bing_images-0.2.3/bing_images.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-14 02:01:16.000000 bing_images-0.2.3/bing_images.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:01:16.000000 bing_images-0.2.3/bing_images.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 02:01:16.000000 bing_images-0.2.3/bing_images.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 02:01:16.000000 bing_images-0.2.3/bing_images.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 02:01:01.000000 bing_images-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-14 02:01:16.337324 bing_images-0.2.3/setup.cfg
```

### Comparing `bing_images-0.2.2/LICENSE` & `bing_images-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bing_images-0.2.2/PKG-INFO` & `bing_images-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: bing_images
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python library to fetch image urls and download using multithreading from Bing.com.
 Home-page: https://github.com/catchzeng/bing_images
 Author: CatchZeng
 Author-email: catchzenghh@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -148,9 +146,7 @@
                       pool_size=20,
                       file_type="png",
                       filters='+filterui:aspect-square+filterui:color2-bw',
                       force_replace=True)
 ```
 
 ![](./images/cat-bw.jpg)
-
-
```

### Comparing `bing_images-0.2.2/README.md` & `bing_images-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bing_images-0.2.2/bing_images/bing.py` & `bing_images-0.2.3/bing_images/bing.py`

 * *Files identical despite different names*

### Comparing `bing_images-0.2.2/bing_images/crawler.py` & `bing_images-0.2.3/bing_images/crawler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,71 @@
 from urllib.parse import quote
 import shutil
-from selenium import webdriver
 import time
 import json
 
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.wait import WebDriverWait
+
 BASE_URL = "https://www.bing.com/images/search?"
 
 
 def gen_query_url(keywords, filters, extra_query_params=''):
     keywords_str = "&q=" + quote(keywords)
     query_url = BASE_URL + keywords_str
     if len(filters) > 0:
         query_url += "&qft="+filters
     query_url += extra_query_params
     return query_url
 
 
-def image_url_from_webpage(driver, max_number=10000):
+def image_url_from_webpage(driver, max_number=10):
     image_urls = list()
 
-    time.sleep(10)
     img_count = 0
 
     while True:
-        image_elements = driver.find_elements_by_class_name("iusc")
+        image_elements = driver.find_elements(By.CLASS_NAME, "iusc")
         if len(image_elements) > max_number:
             break
         if len(image_elements) > img_count:
             img_count = len(image_elements)
             driver.execute_script(
                 "window.scrollTo(0, document.body.scrollHeight);")
         else:
-            smb = driver.find_elements_by_class_name("btn_seemore")
+            smb = driver.find_elements(By.CLASS_NAME, "btn_seemore")
             if len(smb) > 0 and smb[0].is_displayed():
                 smb[0].click()
             else:
                 break
         time.sleep(3)
     for image_element in image_elements:
         m_json_str = image_element.get_attribute("m")
         m_json = json.loads(m_json_str)
         image_urls.append(m_json["murl"])
     return image_urls
 
 
 def crawl_image_urls(keywords, filters, max_number=10000, proxy=None, proxy_type="http", extra_query_params=''):
-    chrome_path = shutil.which("chromedriver")
-    chrome_path = "./bin/chromedriver" if chrome_path is None else chrome_path
-    chrome_options = webdriver.ChromeOptions()
+    chrome_options = Options()
     if proxy is not None and proxy_type is not None:
         chrome_options.add_argument(
             "--proxy-server={}://{}".format(proxy_type, proxy))
-    driver = webdriver.Chrome(chrome_path, chrome_options=chrome_options)
+
+    driver = webdriver.Chrome(options=chrome_options)
 
     query_url = gen_query_url(keywords, filters, extra_query_params=extra_query_params)
     driver.set_window_size(1920, 1080)
+    print("Reading from ", query_url)
     driver.get(query_url)
+    WebDriverWait(driver, timeout=300).until(
+        lambda d: len(d.find_elements(By.CLASS_NAME, "iusc")) > 5)
+    
     image_urls = image_url_from_webpage(driver, max_number)
     driver.close()
 
     if max_number > len(image_urls):
         output_num = len(image_urls)
     else:
         output_num = max_number
```

### Comparing `bing_images-0.2.2/bing_images/util.py` & `bing_images-0.2.3/bing_images/util.py`

 * *Files identical despite different names*

### Comparing `bing_images-0.2.2/bing_images.egg-info/PKG-INFO` & `bing_images-0.2.3/bing_images.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: bing-images
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python library to fetch image urls and download using multithreading from Bing.com.
 Home-page: https://github.com/catchzeng/bing_images
 Author: CatchZeng
 Author-email: catchzenghh@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -148,9 +146,7 @@
                       pool_size=20,
                       file_type="png",
                       filters='+filterui:aspect-square+filterui:color2-bw',
                       force_replace=True)
 ```
 
 ![](./images/cat-bw.jpg)
-
-
```

### Comparing `bing_images-0.2.2/setup.cfg` & `bing_images-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bing_images
-version = 0.2.2
+version = 0.2.3
 author = CatchZeng
 author_email = catchzenghh@gmail.com
 description = Python library to fetch image urls and download using multithreading from Bing.com.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/catchzeng/bing_images
 classifiers =
```

