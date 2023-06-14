# Comparing `tmp/ma_notification_center-2.1.0.tar.gz` & `tmp/ma_notification_center-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_notification_center-2.1.0.tar", last modified: Wed Jun 14 06:42:48 2023, max compression
+gzip compressed data, was "ma_notification_center-2.1.1.tar", last modified: Wed Jun 14 07:12:57 2023, max compression
```

## Comparing `ma_notification_center-2.1.0.tar` & `ma_notification_center-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:42:48.627827 ma_notification_center-2.1.0/
--rw-rw-rw-   0        0        0     1089 2023-06-14 06:35:41.000000 ma_notification_center-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1567 2023-06-14 06:42:48.626828 ma_notification_center-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-06-14 06:33:54.000000 ma_notification_center-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:42:48.600317 ma_notification_center-2.1.0/ma_notification_center/
--rw-rw-rw-   0        0        0        0 2023-06-14 06:28:51.000000 ma_notification_center-2.1.0/ma_notification_center/__init__.py
--rw-rw-rw-   0        0        0     5651 2023-06-14 06:31:07.000000 ma_notification_center-2.1.0/ma_notification_center/notificationcenter.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:42:48.625832 ma_notification_center-2.1.0/ma_notification_center.egg-info/
--rw-rw-rw-   0        0        0     1567 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-14 06:42:48.000000 ma_notification_center-2.1.0/ma_notification_center.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:42:48.627827 ma_notification_center-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-06-14 06:42:25.000000 ma_notification_center-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:12:57.369867 ma_notification_center-2.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-06-14 06:35:41.000000 ma_notification_center-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1383 2023-06-14 07:12:57.368869 ma_notification_center-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1124 2023-06-14 07:12:05.000000 ma_notification_center-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 07:12:57.338948 ma_notification_center-2.1.1/ma_notification_center/
+-rw-rw-rw-   0        0        0        0 2023-06-14 06:28:51.000000 ma_notification_center-2.1.1/ma_notification_center/__init__.py
+-rw-rw-rw-   0        0        0     5681 2023-06-14 07:12:49.000000 ma_notification_center-2.1.1/ma_notification_center/notificationcenter.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:12:57.367870 ma_notification_center-2.1.1/ma_notification_center.egg-info/
+-rw-rw-rw-   0        0        0     1383 2023-06-14 07:12:57.000000 ma_notification_center-2.1.1/ma_notification_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-06-14 07:12:57.000000 ma_notification_center-2.1.1/ma_notification_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:12:57.000000 ma_notification_center-2.1.1/ma_notification_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-14 07:12:57.000000 ma_notification_center-2.1.1/ma_notification_center.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-14 07:12:57.000000 ma_notification_center-2.1.1/ma_notification_center.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:12:57.370864 ma_notification_center-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-06-14 07:12:12.000000 ma_notification_center-2.1.1/setup.py
```

### Comparing `ma_notification_center-2.1.0/LICENSE` & `ma_notification_center-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ma_notification_center-2.1.0/PKG-INFO` & `ma_notification_center-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma_notification_center
-Version: 2.1.0
+Version: 2.1.1
 Summary: MobileArts Notification Center Package
 Author: Fatima Medlij
 Author-email: medlijfatima@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,37 +16,33 @@
 
 You can install ma-notification-center using pip:
 ```python
 pip install ma_notification_center
 ```
 
 ## Usage
-
 Here's an example of how to use ma-notification-center:
 
 ```python
-from ma_notification_center import Notifications
-
-# Initialize NotificationCenter
-notification_center = Notifications()
+from ma_notification_center import notificationcenter
+notifications = notificationcenter.Notifications()
 
 # Send an email
-notification_center.send_email(
+notifications.send_email(
     to_emails=["recipient1@example.com"],
     cc_emails=["recipient2@example.com"],
     bcc_emails=[],
     subject="Notification",
     body_text="This is a notification email.",
     body_html="<p>This is a notification email.</p>"
 )
 
 # Send a Telegram message
-notification_center.send_telegram(["chat_id"], "Hello from NotificationCenter!")
+notifications.send_telegram(["chat_id"], "Hello from NotificationCenter!")
 
 # Send a Telegram photo
-notification_center.send_telegram_photo(["chat_id"], "https://example.com/photo.jpg", "Check out this photo!")
+notifications.send_telegram_photo(["chat_id"], "https://example.com/photo.jpg", "Check out this photo!")
 
 # Send a Telegram document
-notification_center.send_telegram_document(["chat_id"], "https://example.com/document.pdf", "Important Document")
+notifications.send_telegram_document(["chat_id"], "https://example.com/document.pdf", "Important Document")
 
 
-Make sure to import the Notifications class from notificationcenter.notificationcenter and instantiate it before using the send_ functions.
```

### Comparing `ma_notification_center-2.1.0/README.md` & `ma_notification_center-2.1.1/ma_notification_center.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,48 @@
+Metadata-Version: 2.1
+Name: ma-notification-center
+Version: 2.1.1
+Summary: MobileArts Notification Center Package
+Author: Fatima Medlij
+Author-email: medlijfatima@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ma_notification_center
 
 ma-notifications is a Python package that provides a notification center for sending various types of notifications.
 
 ## Installation
 
 You can install ma-notification-center using pip:
 ```python
 pip install ma_notification_center
 ```
 
 ## Usage
-
 Here's an example of how to use ma-notification-center:
 
 ```python
-from ma_notification_center import Notifications
-
-# Initialize NotificationCenter
-notification_center = Notifications()
+from ma_notification_center import notificationcenter
+notifications = notificationcenter.Notifications()
 
 # Send an email
-notification_center.send_email(
+notifications.send_email(
     to_emails=["recipient1@example.com"],
     cc_emails=["recipient2@example.com"],
     bcc_emails=[],
     subject="Notification",
     body_text="This is a notification email.",
     body_html="<p>This is a notification email.</p>"
 )
 
 # Send a Telegram message
-notification_center.send_telegram(["chat_id"], "Hello from NotificationCenter!")
+notifications.send_telegram(["chat_id"], "Hello from NotificationCenter!")
 
 # Send a Telegram photo
-notification_center.send_telegram_photo(["chat_id"], "https://example.com/photo.jpg", "Check out this photo!")
+notifications.send_telegram_photo(["chat_id"], "https://example.com/photo.jpg", "Check out this photo!")
 
 # Send a Telegram document
-notification_center.send_telegram_document(["chat_id"], "https://example.com/document.pdf", "Important Document")
+notifications.send_telegram_document(["chat_id"], "https://example.com/document.pdf", "Important Document")
 
 
-Make sure to import the Notifications class from notificationcenter.notificationcenter and instantiate it before using the send_ functions.
```

### Comparing `ma_notification_center-2.1.0/ma_notification_center/notificationcenter.py` & `ma_notification_center-2.1.1/ma_notification_center/notificationcenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,62 +9,62 @@
 sqs_client = boto3.client("sqs", region_name="eu-central-1")
 s3_client = boto3.client("s3", region_name="eu-central-1")
 bucket_name = "lambda-testing-fatima-de-serverlessdeploymentbuck-g76sanrcmrse"
 bucket_path = "notifications-email"
 
 
 class Notifications:
-    def send_sms(source: str, phonenumbers: list, text: str):
+    def send_sms(self, source: str, phonenumbers: list, text: str):
         url = arn + "sms"
         if all(validate_phone_number(number) for number in phonenumbers) and validate_text(text):
             sms_params = {
                 "source": source,
                 "phonenumbers": phonenumbers,
                 "text": text
             }
             return push_to_sqs(sms_params, url)
         else:
             return "SMS not sent"
 
-    def send_email(to_emails: list, cc_emails: list, bcc_emails: list, subject: str, body_text: str, body_html: str):
+    def send_email(self, to_emails: list, cc_emails: list, bcc_emails: list, subject: str, body_text: str, body_html: str):
         url = arn + "email"
         if not validate_email_params(to_emails, cc_emails, bcc_emails, subject, body_text, body_html):
             return "Email not sent"
         else:
             email_params = dict(to_emails=to_emails, cc_emails=cc_emails, bcc_emails=bcc_emails, message={
                 "subject": subject,
                 "body_text": body_text,
                 "body_html": body_html
             })
             return push_to_sqs(email_params, url)
 
-    def send_telegram(chat_ids: list, text: str):
+    def send_telegram(self, chat_ids: list, text: str):
         url = arn + "telegram"
         if validate_telegram_params(chat_ids, text):
             telegram_params = {
                 "chat_ids": chat_ids,
                 "text": text
             }
             return push_to_sqs(telegram_params, url)
         else:
             return "Telegram message not sent"
 
-    def send_telegram_photo(chat_ids: list, image_url: str, caption: str):
+    def send_telegram_photo(self, chat_ids: list, image_url: str, caption: str):
         url = arn + "photo-telegram"
         if validate_telegram_media_params(chat_ids, image_url, caption):
             telegram_params = {
                 "chat_ids": chat_ids,
                 "imageurl": image_url,
                 "caption": caption
             }
             return push_to_sqs(telegram_params, url)
         else:
             return "Telegram message not sent"
 
-    def send_telegram_document(chat_ids: list, document_url: str, caption: str):
+    def send_telegram_document(self, chat_ids: list, document_url: str, caption: str):
         url = arn + "document-telegram"
         if validate_telegram_media_params(chat_ids, document_url, caption):
             telegram_params = {
                 "chat_ids": chat_ids,
                 "documenturl": document_url,
                 "caption": caption
             }
```

### Comparing `ma_notification_center-2.1.0/setup.py` & `ma_notification_center-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ma_notification_center",
-    version="2.1.0",
+    version="2.1.1",
     author="Fatima Medlij",
     author_email="medlijfatima@gmail.com",
     description="MobileArts Notification Center Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires  = ['boto3', 'email_validator'],
```

