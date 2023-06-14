# Comparing `tmp/instagpy-0.1.4.tar.gz` & `tmp/instagpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagpy-0.1.4.tar", last modified: Wed Jun  7 14:04:24 2023, max compression
+gzip compressed data, was "instagpy-0.1.5.tar", last modified: Wed Jun 14 11:09:22 2023, max compression
```

## Comparing `instagpy-0.1.4.tar` & `instagpy-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:04:24.915113 instagpy-0.1.4/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3318 2023-06-07 14:04:24.915113 instagpy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:04:24.899485 instagpy-0.1.4/instagpy/
--rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.4/instagpy/__init__.py
--rw-rw-rw-   0        0        0      685 2023-06-07 13:57:25.000000 instagpy-0.1.4/instagpy/config.py
--rw-rw-rw-   0        0        0    21919 2023-06-07 13:08:43.000000 instagpy-0.1.4/instagpy/instagpy.py
--rw-rw-rw-   0        0        0     2086 2023-06-07 10:41:45.000000 instagpy-0.1.4/instagpy/path.py
--rw-rw-rw-   0        0        0     1092 2023-05-31 15:11:43.000000 instagpy-0.1.4/instagpy/request_util.py
--rw-rw-rw-   0        0        0     2722 2023-06-07 13:56:52.000000 instagpy-0.1.4/instagpy/session_util.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 12:34:47.000000 instagpy-0.1.4/instagpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:04:24.915113 instagpy-0.1.4/instagpy.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 14:04:24.000000 instagpy-0.1.4/instagpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:04:24.915113 instagpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-06-07 14:03:30.000000 instagpy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:09:22.836324 instagpy-0.1.5/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3318 2023-06-14 11:09:22.820695 instagpy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 11:09:22.820695 instagpy-0.1.5/instagpy/
+-rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.5/instagpy/__init__.py
+-rw-rw-rw-   0        0        0      685 2023-06-14 11:07:11.000000 instagpy-0.1.5/instagpy/config.py
+-rw-rw-rw-   0        0        0    21964 2023-06-14 11:05:52.000000 instagpy-0.1.5/instagpy/instagpy.py
+-rw-rw-rw-   0        0        0     2086 2023-06-07 10:41:45.000000 instagpy-0.1.5/instagpy/path.py
+-rw-rw-rw-   0        0        0     1332 2023-06-14 10:38:27.000000 instagpy-0.1.5/instagpy/request_util.py
+-rw-rw-rw-   0        0        0     2729 2023-06-07 14:13:48.000000 instagpy-0.1.5/instagpy/session_util.py
+-rw-rw-rw-   0        0        0     2914 2023-06-14 09:37:23.000000 instagpy-0.1.5/instagpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:09:22.820695 instagpy-0.1.5/instagpy.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-06-14 11:09:22.000000 instagpy-0.1.5/instagpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-14 11:09:22.000000 instagpy-0.1.5/instagpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:09:22.000000 instagpy-0.1.5/instagpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-14 11:09:22.000000 instagpy-0.1.5/instagpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 11:09:22.000000 instagpy-0.1.5/instagpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:09:22.836324 instagpy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-06-14 11:07:40.000000 instagpy-0.1.5/setup.py
```

### Comparing `instagpy-0.1.4/LICENSE` & `instagpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.4/PKG-INFO` & `instagpy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.4 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.5 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.4/README.md` & `instagpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.4/instagpy/config.py` & `instagpy-0.1.5/instagpy/config.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.4/instagpy/instagpy.py` & `instagpy-0.1.5/instagpy/instagpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,28 +159,28 @@
             if search_surface is not None:
                 params["search_surface"] = search_surface
             if end_cursor is not None:
                 params["max_id"] = end_cursor
 
         return params
 
-    def login(self, username=None, password=None, show_saved_sessions=True, save_session=True):
+    def login(self, username=None, password=None, show_saved_sessions=False, save_session=True):
         """Login Into a user account for Data Scraping Purpose.
 
         Args:
             username (str, optional): Instgram Username or Email. Defaults to None.
             password (str, optional): Password. Defaults to None.
-            show_saved_sessions (bool, optional): Shows saved sessions before logging into new account. Defaults to True.
+            show_saved_sessions (bool, optional): Shows saved sessions before logging into new account. Defaults to False.
             save_session (bool, optional): Save session if want to use it without logging in manually each time. Defaults to True.
 
         Returns:
             dict: Response from server whether got logged in.
         """
         self.generate_session()
-        if show_saved_sessions:
+        if show_saved_sessions or (username is None and password is None):
             session_util.load_session(session=self.session)
             return
         if username is None:
             username = str(input("Enter Your Username or Email : ")).strip()
         if password is None:
             password = getpass.getpass()
         timestamp = int(datetime.datetime.now().timestamp())
```

### Comparing `instagpy-0.1.4/instagpy/path.py` & `instagpy-0.1.5/instagpy/path.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.4/instagpy/request_util.py` & `instagpy-0.1.5/instagpy/request_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import requests
 import bs4
+from . import utils
 
 
 def make_request(url, session=None, method=None, max_retries=None, timeout=None, **kwargs):
     if method is None:
         method = "GET"
     if max_retries is None:
         max_retries = 3
     if session is None:
         session = requests.Session()
     if timeout is None:
         timeout = 30
-    for retry_count, retry in enumerate(range(max_retries), start=1):
+    for retry_count, _ in enumerate(range(max_retries), start=1):
         try:
+            response_text = ""
             response = session.request(method, url, timeout=timeout, **kwargs)
-            response.raise_for_status()
             soup = bs4.BeautifulSoup(response.content, "lxml")
             if "json" in response.headers["Content-Type"]:
-                return response.json()
+                return utils.check_for_errors(response.json())
+            response_text = "\n".join(
+                [line.strip() for line in soup.text.split("\n") if line.strip()])
+            response.raise_for_status()
             return soup
         except KeyboardInterrupt:
             print("Keyboard Interruption...")
             return
         except requests.exceptions.RequestException as error:
-            print(f"Retry No. ==> {retry_count}", error)
+            print(f"\nRetry No. ==> {retry_count} : {error}\n{response_text}")
         except Exception as error:
-            print(f"Retry No. ==> {retry_count}", error)
+            print(f"\nRetry No. ==> {retry_count} : {error}\n{response_text}")
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `instagpy-0.1.4/instagpy/session_util.py` & `instagpy-0.1.5/instagpy/session_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     if path is None:
         path = create_session_directory()
     all_files = [f"{count}. {file}" for count, file in enumerate(
         os.listdir(path), start=1) if file.endswith(".pkl")]
     all_files.append(
         f"{len(os.listdir(path))+1}. Login with a New Account.")
     for file in all_files:
-        os.path.splitext(file)[0]
+        print(os.path.splitext(file)[0])
     file_number = int(
         input("\nChoose a Number to Load an Exising Session : ").strip())
     if file_number != len(os.listdir(path))+1:
         filename = os.listdir(path)[file_number-1]
     else:
         path, filename = generate_new_session(path)
     return path, filename
```

### Comparing `instagpy-0.1.4/instagpy/utils.py` & `instagpy-0.1.5/instagpy/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,9 +54,21 @@
             continue
         if 'bk.action.array.Make' in value and key.endswith('about_this_account_country'):
             placeholder[key] = value.split(
                 'bk.action.array.Make,')[-1].split(")")[0].replace('"', '').strip()
     return placeholder
 
 
+def check_for_errors(response):
+    if isinstance(response, dict):
+        if "status" in response.keys():
+            if response["status"] == "ok":
+                return response
+            if response["status"] != "ok":
+                if "message" in response.keys():
+                    print(response)
+                    raise Exception(response['message'])
+    return response
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `instagpy-0.1.4/instagpy.egg-info/PKG-INFO` & `instagpy-0.1.5/instagpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.4 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.5 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.4/setup.py` & `instagpy-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 SHORT_DESCRIPTION = "InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

