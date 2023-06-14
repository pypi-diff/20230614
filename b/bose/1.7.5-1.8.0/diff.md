# Comparing `tmp/bose-1.7.5.tar.gz` & `tmp/bose-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-1.7.5.tar", last modified: Thu Jun  8 13:08:27 2023, max compression
+gzip compressed data, was "bose-1.8.0.tar", last modified: Wed Jun 14 12:03:00 2023, max compression
```

## Comparing `bose-1.7.5.tar` & `bose-1.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:08:27.870110 bose-1.7.5/
--rw-rw-rw-   0        0        0    14240 2023-06-08 13:08:27.871113 bose-1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-1.7.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-08 13:08:27.869114 bose-1.7.5/bose/
--rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.7.5/bose/__init__.py
--rw-rw-rw-   0        0        0      652 2023-05-25 17:01:27.624054 bose-1.7.5/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.7.5/bose/base_data.py
--rw-rw-rw-   0        0        0     5070 2023-05-25 16:54:25.377864 bose-1.7.5/bose/base_task.py
--rw-rw-rw-   0        0        0     9039 2023-05-22 11:25:15.734584 bose-1.7.5/bose/boss_driver.py
--rw-rw-rw-   0        0        0     9051 2023-05-22 11:25:15.732590 bose-1.7.5/bose/boss_undetected_driver.py
--rw-rw-rw-   0        0        0     7295 2023-06-08 13:07:56.570819 bose-1.7.5/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.7.5/bose/download_driver.py
--rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.7.5/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.7.5/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.7.5/bose/opponent.py
--rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.7.5/bose/output.py
--rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.7.5/bose/task_info.py
--rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.7.5/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.7.5/bose/user_agent.py
--rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.7.5/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.7.5/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.7.5/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.7.5/setup.cfg
--rw-rw-rw-   0        0        0     2329 2023-06-08 13:07:20.397716 bose-1.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:03:00.756936 bose-1.8.0/
+-rw-rw-rw-   0        0        0    14240 2023-06-14 12:03:00.756936 bose-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-1.8.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 12:03:00.756936 bose-1.8.0/bose/
+-rw-rw-rw-   0        0        0      342 2023-06-14 07:55:53.180015 bose-1.8.0/bose/__init__.py
+-rw-rw-rw-   0        0        0     3200 2023-06-14 11:56:24.438623 bose-1.8.0/bose/account_generator.py
+-rw-rw-rw-   0        0        0      652 2023-05-25 17:01:27.624054 bose-1.8.0/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.8.0/bose/base_data.py
+-rw-rw-rw-   0        0        0     5070 2023-06-13 16:14:19.186655 bose-1.8.0/bose/base_task.py
+-rw-rw-rw-   0        0        0     9039 2023-06-13 16:14:04.846297 bose-1.8.0/bose/bose_driver.py
+-rw-rw-rw-   0        0        0     9051 2023-06-13 16:14:04.846297 bose-1.8.0/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     7295 2023-06-13 16:14:19.186655 bose-1.8.0/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.8.0/bose/download_driver.py
+-rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.8.0/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.8.0/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.8.0/bose/opponent.py
+-rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.8.0/bose/output.py
+-rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.8.0/bose/task_info.py
+-rw-rw-rw-   0        0        0     5433 2023-06-14 07:47:40.744829 bose-1.8.0/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.8.0/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.8.0/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.8.0/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.8.0/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     2336 2023-06-14 12:01:44.486327 bose-1.8.0/setup.py
```

### Comparing `bose-1.7.5/PKG-INFO` & `bose-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 1.7.5
+Version: 1.8.0
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-1.7.5/README.rst` & `bose-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/analytics.py` & `bose-1.8.0/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/base_data.py` & `bose-1.8.0/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/base_task.py` & `bose-1.8.0/bose/base_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import traceback
 from .create_driver import BrowserConfig, create_driver
-from .boss_driver import BossDriver
+from .bose_driver import BoseDriver
 from .utils import relative_path, merge_dicts_in_one_dict, write_file, write_html, write_json,get_driver_path
 from .local_storage import LocalStorage
 from .analytics import Analytics
 from .task_info import TaskInfo
 
 
 class RetryException(Exception):
@@ -69,15 +69,15 @@
             def close_driver(driver):
                 print("Closing Browser")                
                 driver.close()
                 print("Closed Browser")                
 
 
             final_image = "final.png"
-            def end_task(driver:BossDriver):
+            def end_task(driver:BoseDriver):
                 task.end()
                 task.set_ip()
                 data = task.data
                 driver.save_screenshot(final_image)
                 
                 html_path  = f'{self.task_path}/page.html'
                 source = get_page_source_safe(driver)
@@ -139,15 +139,15 @@
                     
                 close_driver(driver)
 
                 print(f'Task Failed! View Final Screenshot at {final_image_path}')
 
         return run_task(False, 0)
 
-    def run(self, driver: BossDriver):
+    def run(self, driver: BoseDriver):
         pass
 
 
 class Task(BaseTask):
     def __init__(self):
         pass
```

### Comparing `bose-1.7.5/bose/boss_driver.py` & `bose-1.8.0/bose/bose_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import random
 from time import sleep
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
 from .utils import relative_path, sleep_for_n_seconds, sleep_forever
 
 
-class BossDriver(webdriver.Chrome):
+class BoseDriver(webdriver.Chrome):
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
```

### Comparing `bose-1.7.5/bose/boss_undetected_driver.py` & `bose-1.8.0/bose/bose_undetected_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from time import sleep
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
 from .utils import relative_path, sleep_for_n_seconds, sleep_forever
 from datetime import datetime
 
 
-class BossUndetectedDriver(Chrome):
+class BoseUndetectedDriver(Chrome):
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
```

### Comparing `bose-1.7.5/bose/create_driver.py` & `bose-1.8.0/bose/create_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from selenium.common.exceptions import WebDriverException
 from .user_agent import UserAgentInstance, UserAgent
 from .window_size import WindowSize, WindowSizeInstance
 from .utils import NETWORK_ERRORS, is_windows, relative_path, retry_if_is_error, silentremove
 from selenium.webdriver.chrome.options import Options as GoogleChromeOptions
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from undetected_chromedriver import ChromeOptions
-from .boss_driver import BossDriver
+from .bose_driver import BoseDriver
 
-from .boss_undetected_driver import BossUndetectedDriver
+from .bose_undetected_driver import BoseUndetectedDriver
 import shutil
 import os
 
 class RetryException(Exception):
     pass
 
 
@@ -163,29 +163,29 @@
             desired_capabilities = get_eager_startegy()
         else:
             desired_capabilities = None
         
         print(driver_string)
 
         if is_undetected:
-            driver = BossUndetectedDriver(
+            driver = BoseUndetectedDriver(
                 desired_capabilities=desired_capabilities,
                               options=options
                             )
         else:
             # options.add_experimental_option("prefs",  {"profile.managed_default_content_settings.images": 2})
             hide_automation_flags(options)
             
             # CAPTCHA
             options.arguments.extend(
                 ["--disable-web-security", "--disable-site-isolation-trials", "--disable-application-cache"])
 
             path = relative_path(get_driver_path(), 0)
 
-            driver = BossDriver(
+            driver = BoseDriver(
                 desired_capabilities=desired_capabilities,
                 chrome_options=options,
                 executable_path=path,
             )
 
         if driver_attributes["profile"] is None:
             del driver_attributes["profile"]
```

### Comparing `bose-1.7.5/bose/download_driver.py` & `bose-1.8.0/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/local_storage.py` & `bose-1.8.0/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/local_storage_driver.py` & `bose-1.8.0/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/output.py` & `bose-1.8.0/bose/output.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/task_info.py` & `bose-1.8.0/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/temp_mail.py` & `bose-1.8.0/bose/temp_mail.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,61 @@
+from time import sleep
+import traceback
 import random
 from bs4 import BeautifulSoup
 import requests
 import re
-from .utils import * 
+from urllib.error import ContentTooShortError
+from http.client import RemoteDisconnected
+from urllib.error import ContentTooShortError, URLError
 
+NETWORK_ERRORS = [RemoteDisconnected, URLError,
+                  ConnectionAbortedError, ContentTooShortError,  BlockingIOError]
+
+
+def istuple(el):
+    return type(el) is tuple
+
+
+def is_errors_instance(instances, error):
+    for i in range(len(instances)):
+        ins = instances[i]
+        if isinstance(error, ins):
+            return True, i
+    return False, -1
+
+def retry_if_is_error(func, instances=None, retries=2, wait_time=None):
+    tries = 0
+    errors_only_instances = list(
+        map(lambda el: el[0] if istuple(el) else el, instances))
+
+    while tries < retries:
+        tries += 1
+        try:
+            created_result = func()
+            return created_result
+        except Exception as e:
+            is_valid_error, index = is_errors_instance(
+                errors_only_instances, e)
+
+            if not is_valid_error:
+                raise e
+
+            traceback.print_exc()
+
+            if istuple(instances[index]):
+                instances[index][1]()
+
+            if tries == retries:
+                raise e
+
+            print('Retrying')
+
+            if wait_time is not None:
+                sleep(wait_time)
 def extract_links_from_html(html):
     soup = BeautifulSoup(html, features="html.parser")
     xs = []
     for a in soup.find_all('a', href=True):
         href = a['href']
         if 'http' in href:
             xs.append(href)
@@ -42,16 +90,14 @@
     if domainList is None:
         domainList = requests.get(
             "https://www.1secmail.com/api/v1/?action=getDomainList").json()
     return domainList
 
 
 class TempMail():
-    def get_domains():
-        return get_domains()
 
     def generate_email(username):
         # ['1secmail.com', '1secmail.net', '1secmail.org']
         domain = random.choice(get_domains())
 
         email = f'{username}@{domain}'
         return email
@@ -69,14 +115,17 @@
             'action': 'deleteMailbox',
             'login': f'{login}',
             'domain': f'{domain}'
         }
 
         requests.post(url, data=data)
 
+    def get_domains():
+        return get_domains()
+
     def get_email_link(email):
         def run():
             login, domain = TempMail.extract(email)
             reqLink = f'{API}?action=getMessages&login={login}&domain={domain}'
             req = requests.get(reqLink).json()
 
             if len(req) == 0:
@@ -133,15 +182,19 @@
             # 1
             5
             , 5)
         data = run()
         return data
 
     def get_email_link_and_delete_mailbox(email):
-        TempMail.get_email_link(email)
+        link = TempMail.get_email_link(email)
         TempMail.deleteMailbox(email)
+        return link 
 
 if __name__ == '__main__':
-    print('Running')
-    email = TempMail.generate_email('temp')
-    print(email)
-    print(TempMail.get_email_link_and_delete_mailbox(email))
+    link = TempMail.get_email_link("shyam@1secmail.com")
+    print(link) 
+
+
+    # email = TempMail.generate_email('temp')
+    # print(email)
+    # print(TempMail.get_email_link_and_delete_mailbox(email))
```

### Comparing `bose-1.7.5/bose/user_agent.py` & `bose-1.8.0/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/utils.py` & `bose-1.8.0/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/bose/window_size.py` & `bose-1.8.0/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-1.7.5/setup.py` & `bose-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 def get_description():
     try:
       return open("README.rst", encoding="utf-8").read()
     except:
       return None
     
-
+            
 setup(
     name='bose',
     packages=['bose'],
-    version='1.7.5',
+    version='1.8.0',
     license='MIT',
     project_urls={
-        "Documentation": "https://omkar.cloud/bose/docs/",
-        "Source": "https://github.com/omkarcloud/boss",
-        "Tracker": "https://github.com/omkarcloud/boss/issues",
+        "Documentation": "https://omkar.cloud/bose/",
+        "Source": "https://github.com/omkarcloud/bose",
+        "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
 
     description="The Ultimate Web Scraping Framework",
     long_description=get_description(),
     # long_description_content_type="text/markdown",
     author='Chetan Jain',
     author_email='chetan@omkar.cloud',
```

