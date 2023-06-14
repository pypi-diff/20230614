# Comparing `tmp/login_gmail_selenium-1.1.7.tar.gz` & `tmp/login_gmail_selenium-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\login_gmail_selenium-1.1.7.tar", last modified: Tue Mar 28 10:12:47 2023, max compression
+gzip compressed data, was "dist\login_gmail_selenium-1.1.8.tar", last modified: Wed Jun 14 09:45:19 2023, max compression
```

## Comparing `login_gmail_selenium-1.1.7.tar` & `login_gmail_selenium-1.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 10:12:47.397206 login_gmail_selenium-1.1.7/
--rw-rw-rw-   0        0        0     1105 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     2380 2023-03-28 10:12:47.396209 login_gmail_selenium-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2023-03-07 08:43:52.000000 login_gmail_selenium-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 10:12:47.336368 login_gmail_selenium-1.1.7/login_gmail_selenium/
--rw-rw-rw-   0        0        0       42 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:12:47.367288 login_gmail_selenium-1.1.7/login_gmail_selenium/common/
--rw-rw-rw-   0        0        0       24 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/common/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-03-28 10:10:22.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/common/constant.py
--rw-rw-rw-   0        0        0      628 2023-02-27 08:57:32.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/common/log.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:12:47.389228 login_gmail_selenium-1.1.7/login_gmail_selenium/extension/
--rw-rw-rw-   0        0        0    38852 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/extension/always_active.zip
--rw-rw-rw-   0        0        0     5260 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/extension/fingerprint_defender.zip
--rw-rw-rw-   0        0        0   120399 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/extension/spoof_timezone.zip
--rw-rw-rw-   0        0        0  5601639 2023-03-14 08:09:16.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/extension/veepn.zip
--rw-rw-rw-   0        0        0    45183 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/extension/webrtc_control.zip
-drwxrwxrwx   0        0        0        0 2023-03-28 10:12:47.394214 login_gmail_selenium-1.1.7/login_gmail_selenium/util/
--rw-rw-rw-   0        0        0       45 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/util/__init__.py
--rw-rw-rw-   0        0        0      706 2023-03-24 10:39:03.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/util/driver.py
--rw-rw-rw-   0        0        0     4719 2023-03-24 08:28:57.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/util/helper.py
--rw-rw-rw-   0        0        0    16720 2023-03-28 10:12:22.000000 login_gmail_selenium-1.1.7/login_gmail_selenium/util/profile.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:12:47.363297 login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/
--rw-rw-rw-   0        0        0     2380 2023-03-28 10:12:47.000000 login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-03-28 10:12:47.000000 login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 10:12:47.000000 login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-03-28 10:12:47.000000 login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:12:47.000000 login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 10:12:47.397206 login_gmail_selenium-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-03-28 10:12:28.000000 login_gmail_selenium-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:12:47.395212 login_gmail_selenium-1.1.7/test/
--rw-rw-rw-   0        0        0     1230 2023-03-28 10:06:33.000000 login_gmail_selenium-1.1.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.518118 login_gmail_selenium-1.1.8/
+-rw-rw-rw-   0        0        0     1105 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2380 2023-06-14 09:45:19.517122 login_gmail_selenium-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2023-03-07 08:43:52.000000 login_gmail_selenium-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.455288 login_gmail_selenium-1.1.8/login_gmail_selenium/
+-rw-rw-rw-   0        0        0       42 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.481217 login_gmail_selenium-1.1.8/login_gmail_selenium/common/
+-rw-rw-rw-   0        0        0       24 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/common/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-06-14 09:30:06.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/common/constant.py
+-rw-rw-rw-   0        0        0      628 2023-02-27 08:57:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/common/log.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.509143 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/
+-rw-rw-rw-   0        0        0    38852 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/always_active.zip
+-rw-rw-rw-   0        0        0     5260 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/fingerprint_defender.zip
+-rw-rw-rw-   0        0        0   120399 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/spoof_timezone.zip
+-rw-rw-rw-   0        0        0  5601639 2023-03-14 08:09:16.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/veepn.zip
+-rw-rw-rw-   0        0        0    45183 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/webrtc_control.zip
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.514130 login_gmail_selenium-1.1.8/login_gmail_selenium/util/
+-rw-rw-rw-   0        0        0       45 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/__init__.py
+-rw-rw-rw-   0        0        0      706 2023-03-24 10:39:03.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/driver.py
+-rw-rw-rw-   0        0        0     4719 2023-03-24 08:28:57.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/helper.py
+-rw-rw-rw-   0        0        0    17201 2023-06-14 09:43:09.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/profile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.477227 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/
+-rw-rw-rw-   0        0        0     2380 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:45:19.518118 login_gmail_selenium-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-06-14 09:45:15.000000 login_gmail_selenium-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.515130 login_gmail_selenium-1.1.8/test/
+-rw-rw-rw-   0        0        0     1230 2023-03-28 10:06:33.000000 login_gmail_selenium-1.1.8/test/test.py
```

### Comparing `login_gmail_selenium-1.1.7/LICENSE` & `login_gmail_selenium-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/PKG-INFO` & `login_gmail_selenium-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: login_gmail_selenium
-Version: 1.1.7
+Version: 1.1.8
 Summary: A python package for login google by selenium
 Home-page: https://github.com/ngminhhoang1412/LoginGmailSelenium
 Author: Minh Hoang
 Author-email: ngminhhoang1412@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `login_gmail_selenium-1.1.7/README.md` & `login_gmail_selenium-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/common/constant.py` & `login_gmail_selenium-1.1.8/login_gmail_selenium/common/constant.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 WIDE_WAIT = [1, 10]
 PASTE_PERCENTAGE = 50
 DISK_SPACE = 80.0
 CHANGED_PASSWORD_SEPARATOR = '::::'
 PASSWORD_LENGTH = 25
 ACCOUNT_DISABLED_MESSAGE = 'Account disabled'
 ACCOUNT_VERIFICATION_MESSAGE = 'Account required verification steps'
+ACCOUNT_REQUIRED_CAPTCHA = 'Account required captcha'
+ACCOUNT_REJECTED_MESSAGE = 'Account rejected because of suspicious action'
 
 
 def resource_path(relative_path):
     try:
         base_path = sys._MEIPASS
     except (Exception, SyntaxError):
         base_path = os.path.abspath(".")
```

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/common/log.py` & `login_gmail_selenium-1.1.8/login_gmail_selenium/common/log.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/extension/always_active.zip` & `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/always_active.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/extension/fingerprint_defender.zip` & `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/fingerprint_defender.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/extension/spoof_timezone.zip` & `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/spoof_timezone.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/extension/veepn.zip` & `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/veepn.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/extension/webrtc_control.zip` & `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/webrtc_control.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/util/driver.py` & `login_gmail_selenium-1.1.8/login_gmail_selenium/util/driver.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/util/helper.py` & `login_gmail_selenium-1.1.8/login_gmail_selenium/util/helper.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium/util/profile.py` & `login_gmail_selenium-1.1.8/login_gmail_selenium/util/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
             self.cache_folders.append(os.path.join(path, 'MediaFoundationWidevineCdm'))
             self.cache_folders.append(os.path.join(path, 'GrShaderCache'))
             self.cache_folders.append(os.path.join(path, 'ClientSidePhishing'))
             self.cache_folders.append(os.path.join(path, 'hyphen-data'))
             self.cache_folders.append(os.path.join(path, 'ZxcvbnData'))
             self.cache_folders.append(os.path.join(path, 'Safe Browsing'))
         options.add_argument("--start-maximized")
+        options.add_argument("--disable-notifications")
+
         if self.insecure:
             options.add_argument("--disable-web-security")
             options.add_argument("--allow-running-insecure-content")
         # header = Headers(
         #     browser='chrome'
         # ).generate()
         # agent = f"user-agent={header['User-Agent']}"
@@ -229,23 +231,30 @@
             self.check_challenge()
         elif 'disabled/explanation' in driver.current_url:
             self.handle_false_email(Constant.ACCOUNT_DISABLED_MESSAGE)
         elif 'speedbump/changepassword' in driver.current_url:
             self.change_password()
             if 'disabled/explanation' in driver.current_url:
                 self.handle_false_email(Constant.ACCOUNT_DISABLED_MESSAGE)
-        # TODO: need handling for 2 more cases
-        # elif 'rejected'/'ootp' in driver.current_url:
-        #     pass
+        elif 'challenge/recaptcha' in driver.current_url:
+            self.handle_false_email(Constant.ACCOUNT_REQUIRED_CAPTCHA)
+        elif 'signin/rejected' in driver.current_url:
+            self.handle_false_email(Constant.ACCOUNT_REJECTED_MESSAGE)
         elif 'speedbump' in driver.current_url or \
                 'challenge/sk/presend' in driver.current_url or \
-                'challenge/dp' in driver.current_url:
-            # speedbump/idvreenable -> require phone verification ???
-            # challenge/sk/presend -> require phone verification ???
-            # challenge/dp -> select a number ???
+                'challenge/dp' in driver.current_url or \
+                'challenge/ootp' in driver.current_url or \
+                'challenge/ipp' in driver.current_url or \
+                'challenge/iap' in driver.current_url:
+            # speedbump/idvreenable -> require phone verification
+            # challenge/sk/presend -> require phone verification
+            # challenge/dp -> select a number
+            # ootp -> required OTP
+            # ipp -> required OTP
+            # iap -> require phone verification
             self.handle_false_email(Constant.ACCOUNT_VERIFICATION_MESSAGE)
 
     def change_password(self):
         new_pass = helper.create_random_password()
         password_path = '//*[@id="passwd"]/div[1]/div/div[1]/input'
         type_text(driver=self.driver, text=new_pass, xpath=password_path)
         confirm_pass_path = '//*[@id="confirm-passwd"]/div[1]/div/div[1]/input'
```

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/PKG-INFO` & `login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: login-gmail-selenium
-Version: 1.1.7
+Version: 1.1.8
 Summary: A python package for login google by selenium
 Home-page: https://github.com/ngminhhoang1412/LoginGmailSelenium
 Author: Minh Hoang
 Author-email: ngminhhoang1412@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `login_gmail_selenium-1.1.7/login_gmail_selenium.egg-info/SOURCES.txt` & `login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.7/test/test.py` & `login_gmail_selenium-1.1.8/test/test.py`

 * *Files identical despite different names*

