# Comparing `tmp/je_mail_thunder_dev-0.0.8.tar.gz` & `tmp/je_mail_thunder_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_mail_thunder_dev-0.0.8.tar", last modified: Sun Jul  3 19:04:20 2022, max compression
+gzip compressed data, was "dist\je_mail_thunder_dev-0.0.9.tar", last modified: Tue Jul  5 12:20:40 2022, max compression
```

## Comparing `je_mail_thunder_dev-0.0.8.tar` & `je_mail_thunder_dev-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/
--rw-rw-rw-   0        0        0      925 2022-07-03 19:04:18.000000 je_mail_thunder_dev-0.0.8/dev_setup.py
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/imap/
--rw-rw-rw-   0        0        0     1815 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/imap/imap_wrapper.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/imap/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/pop/
--rw-rw-rw-   0        0        0      142 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/pop/pop_wrapper.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/pop/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/smtp/
--rw-rw-rw-   0        0        0     3841 2022-07-03 19:04:18.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/smtp/smtp_wrapper.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/smtp/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/exception/
--rw-rw-rw-   0        0        0      231 2022-07-02 07:59:19.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/exception/exceptions.py
--rw-rw-rw-   0        0        0      613 2022-07-03 19:04:18.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/json_format/
--rw-rw-rw-   0        0        0     1054 2022-06-30 08:20:17.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/json_format/json_process.py
--rw-rw-rw-   0        0        0        0 2022-06-30 12:01:57.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/json_format/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/save_mail_user_content/
--rw-rw-rw-   0        0        0      272 2022-06-30 12:27:35.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_data.py
--rw-rw-rw-   0        0        0     1443 2022-07-02 02:26:48.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py
--rw-rw-rw-   0        0        0        0 2022-06-30 03:21:50.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/save_mail_user_content/__init__.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/__init__.py
--rw-rw-rw-   0        0        0      550 2022-06-30 12:27:35.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/__init__.py
--rw-rw-rw-   0        0        0     1327 2022-07-03 18:39:52.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder/__main__.py
-drwxrwxrwx   0        0        0        0 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder_dev.egg-info/
--rw-rw-rw-   0        0        0        1 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      872 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      941 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/je_mail_thunder_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      872 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      141 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-07-03 19:04:20.000000 je_mail_thunder_dev-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      917 2022-07-01 17:10:42.000000 je_mail_thunder_dev-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/
+-rw-rw-rw-   0        0        0      925 2022-07-05 12:20:38.000000 je_mail_thunder_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/imap/
+-rw-rw-rw-   0        0        0     2512 2022-07-05 06:34:00.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/imap/imap_wrapper.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/imap/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/pop/
+-rw-rw-rw-   0        0        0      142 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/pop/pop_wrapper.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/pop/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/smtp/
+-rw-rw-rw-   0        0        0     4249 2022-07-05 12:20:38.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/smtp/smtp_wrapper.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/smtp/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/exception/
+-rw-rw-rw-   0        0        0      231 2022-07-02 07:59:19.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/exception/exceptions.py
+-rw-rw-rw-   0        0        0      626 2022-07-05 06:28:50.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/json_format/
+-rw-rw-rw-   0        0        0     1054 2022-06-30 08:20:17.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/json_format/json_process.py
+-rw-rw-rw-   0        0        0        0 2022-06-30 12:01:57.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/json_format/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/save_mail_user_content/
+-rw-rw-rw-   0        0        0      272 2022-06-30 12:27:35.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_data.py
+-rw-rw-rw-   0        0        0     1443 2022-07-02 02:26:48.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py
+-rw-rw-rw-   0        0        0      483 2022-07-05 12:00:29.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/save_mail_user_content/save_on_env.py
+-rw-rw-rw-   0        0        0        0 2022-06-30 03:21:50.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/save_mail_user_content/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/__init__.py
+-rw-rw-rw-   0        0        0      746 2022-07-05 06:24:45.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/__init__.py
+-rw-rw-rw-   0        0        0     1327 2022-07-03 18:39:52.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder/__main__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder_dev.egg-info/
+-rw-rw-rw-   0        0        0        1 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      872 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/je_mail_thunder_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      872 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2022-05-19 03:03:52.000000 je_mail_thunder_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-07-05 12:20:40.000000 je_mail_thunder_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      917 2022-07-04 03:28:20.000000 je_mail_thunder_dev-0.0.9/setup.py
```

### Comparing `je_mail_thunder_dev-0.0.8/dev_setup.py` & `je_mail_thunder_dev-0.0.9/dev_setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_mail_thunder_dev",
-    version="0.0.08",
+    version="0.0.09",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="mail wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/PythonMailWrapper_JE",
     packages=setuptools.find_packages(),
```

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder/imap/imap_wrapper.py` & `je_mail_thunder_dev-0.0.9/je_mail_thunder/imap/imap_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,29 @@
+import sys
 from imaplib import IMAP4_SSL
 from email import policy
 from email import message_from_bytes
 from email.header import decode_header
 
+from je_mail_thunder import read_output_content
+from je_mail_thunder.utils.exception.exception_tags import mail_thunder_content_login_failed
+
 
 class IMAPWrapper(IMAP4_SSL):
 
-    def __init__(self, host: str):
+    def __init__(self, host: str = 'imap.gmail.com'):
         super().__init__(host)
+        user_info = read_output_content()
+        try:
+            if user_info is not None and type(user_info) == dict:
+                if "user" in user_info.keys() and "password" in user_info.keys():
+                    if user_info.get("user") is not None and user_info.get("password") is not None:
+                        self.login(user_info.get("user"), user_info.get("password"))
+        except Exception as error:
+            print(repr(error) + " " + mail_thunder_content_login_failed, file=sys.stderr)
 
     def search_mailbox(self, search_str: [str, list] = "ALL", charset: str = None):
         response, mail_number_string = self.search(charset, search_str)
         mail_detail_list = list()
         for num_of_mail in mail_number_string[0].split():
             response, mail_data = self.fetch(num_of_mail, "(RFC822)")
             # [0][1] is message data [0][0] is message decode like RFC822 {565}
```

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder/smtp/smtp_wrapper.py` & `je_mail_thunder_dev-0.0.9/je_mail_thunder/smtp/smtp_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 import smtplib
 import sys
-from smtplib import SMTP_SSL
 from email.message import EmailMessage
 from email.mime.audio import MIMEAudio
 from email.mime.base import MIMEBase
 from email.mime.image import MIMEImage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from mimetypes import guess_type
 from os import path
+from smtplib import SMTP_SSL
 
-from je_mail_thunder.utils.exception.exception_tags import mail_thunder_smtp_content_login_failed
+from je_mail_thunder import get_mail_thunder_os_environ
+from je_mail_thunder.utils.exception.exception_tags import mail_thunder_content_login_failed
 from je_mail_thunder.utils.save_mail_user_content.mail_thunder_content_save import read_output_content
 
 
 class SMTPWrapper(SMTP_SSL):
 
     def __init__(self, host: str = "smtp.gmail.com", port: int = 465):
         super().__init__(host, port)
         user_info = read_output_content()
         try:
             if user_info is not None and type(user_info) == dict:
-                if "user" in user_info.keys() and "password" in user_info.keys():
-                    if user_info.get("user") is not None and user_info.get("password") is not None:
-                        self.login(user_info.get("user"), user_info.get("password"))
+                if user_info.get("user", None) is not None and user_info.get("password", None) is not None:
+                    self.login(user_info.get("user"), user_info.get("password"))
+            else:
+                user_info = get_mail_thunder_os_environ()
+                if user_info is not None and type(user_info) == dict:
+                    if user_info.get("mail_thunder_user", None) is not None and user_info.get(
+                            "mail_thunder_user_password", None) is not None:
+                        self.login(user_info.get("mail_thunder_user"), user_info.get("mail_thunder_user_password"))
         except smtplib.SMTPAuthenticationError as error:
-            print(repr(error) + " " + mail_thunder_smtp_content_login_failed, file=sys.stderr)
+            print(repr(error) + " " + mail_thunder_content_login_failed, file=sys.stderr)
 
     @staticmethod
     def create_message(message_content: str, message_setting_dict: dict, **kwargs):
         message = EmailMessage(**kwargs)
         message.set_content(message_content)
         for key, value in message_setting_dict.items():
             message[key] = value
```

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/exception/exception_tags.py` & `je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/exception/exception_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 mail_thunder_cant_reformat_json_error = "Can't reformat json is type right?"
 mail_thunder_wrong_json_data_error = "Can't parser json"
 """
 content data error
 """
 mail_thunder_content_set_compiler_error = "When set compiler using content make an error"
 mail_thunder_content_file_error = "MailThunder content file error"
+mail_thunder_content_login_failed = "can't login with mail thunder content"
 """
 argparse
 """
 mail_thunder_service_file_error = "service param -s got the wrong data"
 mail_thunder_login_error = "need set --user and --password to login"
 """
 SMTP 
 """
-mail_thunder_smtp_content_login_failed = "can't login with mail thunder content"
+
+"""
+IMAP
+"""
```

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/json_format/json_process.py` & `je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py` & `je_mail_thunder_dev-0.0.9/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder/__main__.py` & `je_mail_thunder_dev-0.0.9/je_mail_thunder/__main__.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder_dev.egg-info/PKG-INFO` & `je_mail_thunder_dev-0.0.9/je_mail_thunder_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-mail-thunder-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: mail wrapper
 Home-page: https://github.com/JE-Chen/PythonMailWrapper_JE
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Description: # mail thunder a stand python mail module wrapper
```

### Comparing `je_mail_thunder_dev-0.0.8/je_mail_thunder_dev.egg-info/SOURCES.txt` & `je_mail_thunder_dev-0.0.9/je_mail_thunder_dev.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 je_mail_thunder/utils/exception/exception_tags.py
 je_mail_thunder/utils/exception/exceptions.py
 je_mail_thunder/utils/json_format/__init__.py
 je_mail_thunder/utils/json_format/json_process.py
 je_mail_thunder/utils/save_mail_user_content/__init__.py
 je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_data.py
 je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py
+je_mail_thunder/utils/save_mail_user_content/save_on_env.py
 je_mail_thunder_dev.egg-info/PKG-INFO
 je_mail_thunder_dev.egg-info/SOURCES.txt
 je_mail_thunder_dev.egg-info/dependency_links.txt
 je_mail_thunder_dev.egg-info/top_level.txt
```

### Comparing `je_mail_thunder_dev-0.0.8/PKG-INFO` & `je_mail_thunder_dev-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_mail_thunder_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: mail wrapper
 Home-page: https://github.com/JE-Chen/PythonMailWrapper_JE
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Description: # mail thunder a stand python mail module wrapper
```

### Comparing `je_mail_thunder_dev-0.0.8/setup.py` & `je_mail_thunder_dev-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_mail_thunder",
-    version="0.0.03",
+    version="0.0.04",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="mail wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/PythonMailWrapper_JE",
     packages=setuptools.find_packages(),
```

