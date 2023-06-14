# Comparing `tmp/je_mail_thunder-0.0.8.tar.gz` & `tmp/je_mail_thunder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_mail_thunder-0.0.8.tar", last modified: Sat Jul 16 17:00:33 2022, max compression
+gzip compressed data, was "dist\je_mail_thunder-0.0.9.tar", last modified: Sun Jul 17 09:47:03 2022, max compression
```

## Comparing `je_mail_thunder-0.0.8.tar` & `je_mail_thunder-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/imap/
--rw-rw-rw-   0        0        0     2567 2022-07-05 12:44:35.000000 je_mail_thunder-0.0.8/je_mail_thunder/imap/imap_wrapper.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.8/je_mail_thunder/imap/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/pop/
--rw-rw-rw-   0        0        0      142 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.8/je_mail_thunder/pop/pop_wrapper.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.8/je_mail_thunder/pop/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/smtp/
--rw-rw-rw-   0        0        0     4683 2022-07-07 07:53:41.000000 je_mail_thunder-0.0.8/je_mail_thunder/smtp/smtp_wrapper.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.8/je_mail_thunder/smtp/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/exception/
--rw-rw-rw-   0        0        0      231 2022-07-02 07:59:19.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/exception/exceptions.py
--rw-rw-rw-   0        0        0      693 2022-07-16 16:53:26.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/json_format/
--rw-rw-rw-   0        0        0     1054 2022-06-30 08:20:17.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/json_format/json_process.py
--rw-rw-rw-   0        0        0        0 2022-06-30 12:01:57.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/json_format/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/save_mail_user_content/
--rw-rw-rw-   0        0        0      272 2022-06-30 12:27:35.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_data.py
--rw-rw-rw-   0        0        0     1443 2022-07-02 02:26:48.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py
--rw-rw-rw-   0        0        0      483 2022-07-05 12:00:29.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/save_mail_user_content/save_on_env.py
--rw-rw-rw-   0        0        0        0 2022-06-30 03:21:50.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/save_mail_user_content/__init__.py
--rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.8/je_mail_thunder/utils/__init__.py
--rw-rw-rw-   0        0        0      796 2022-07-07 07:49:21.000000 je_mail_thunder-0.0.8/je_mail_thunder/__init__.py
--rw-rw-rw-   0        0        0     1917 2022-07-16 16:53:26.000000 je_mail_thunder-0.0.8/je_mail_thunder/__main__.py
-drwxrwxrwx   0        0        0        0 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder.egg-info/
--rw-rw-rw-   0        0        0        1 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      868 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      972 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/je_mail_thunder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      868 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      141 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-07-16 17:00:33.000000 je_mail_thunder-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      917 2022-07-16 17:00:24.000000 je_mail_thunder-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/imap/
+-rw-rw-rw-   0        0        0     2567 2022-07-05 12:44:35.000000 je_mail_thunder-0.0.9/je_mail_thunder/imap/imap_wrapper.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.9/je_mail_thunder/imap/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/pop/
+-rw-rw-rw-   0        0        0      142 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.9/je_mail_thunder/pop/pop_wrapper.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.9/je_mail_thunder/pop/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/smtp/
+-rw-rw-rw-   0        0        0     4683 2022-07-07 07:53:41.000000 je_mail_thunder-0.0.9/je_mail_thunder/smtp/smtp_wrapper.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.9/je_mail_thunder/smtp/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/exception/
+-rw-rw-rw-   0        0        0      231 2022-07-02 07:59:19.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/exception/exceptions.py
+-rw-rw-rw-   0        0        0      693 2022-07-16 16:53:26.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/json_format/
+-rw-rw-rw-   0        0        0     1054 2022-06-30 08:20:17.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/json_format/json_process.py
+-rw-rw-rw-   0        0        0        0 2022-06-30 12:01:57.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/json_format/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/save_mail_user_content/
+-rw-rw-rw-   0        0        0      272 2022-06-30 12:27:35.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_data.py
+-rw-rw-rw-   0        0        0     1443 2022-07-02 02:26:48.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py
+-rw-rw-rw-   0        0        0      483 2022-07-05 12:00:29.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/save_mail_user_content/save_on_env.py
+-rw-rw-rw-   0        0        0        0 2022-06-30 03:21:50.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/save_mail_user_content/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.9/je_mail_thunder/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2022-07-07 07:49:21.000000 je_mail_thunder-0.0.9/je_mail_thunder/__init__.py
+-rw-rw-rw-   0        0        0     2153 2022-07-17 09:35:22.000000 je_mail_thunder-0.0.9/je_mail_thunder/__main__.py
+drwxrwxrwx   0        0        0        0 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder.egg-info/
+-rw-rw-rw-   0        0        0        1 2022-07-17 09:47:02.000000 je_mail_thunder-0.0.9/je_mail_thunder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      868 2022-07-17 09:47:02.000000 je_mail_thunder-0.0.9/je_mail_thunder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/je_mail_thunder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2022-07-17 09:47:02.000000 je_mail_thunder-0.0.9/je_mail_thunder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      868 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2022-05-19 03:03:52.000000 je_mail_thunder-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-07-17 09:47:03.000000 je_mail_thunder-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      917 2022-07-17 09:46:31.000000 je_mail_thunder-0.0.9/setup.py
```

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder/imap/imap_wrapper.py` & `je_mail_thunder-0.0.9/je_mail_thunder/imap/imap_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder/smtp/smtp_wrapper.py` & `je_mail_thunder-0.0.9/je_mail_thunder/smtp/smtp_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder/utils/exception/exception_tags.py` & `je_mail_thunder-0.0.9/je_mail_thunder/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder/utils/json_format/json_process.py` & `je_mail_thunder-0.0.9/je_mail_thunder/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py` & `je_mail_thunder-0.0.9/je_mail_thunder/utils/save_mail_user_content/mail_thunder_content_save.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder/__init__.py` & `je_mail_thunder-0.0.9/je_mail_thunder/__init__.py`

 * *Files identical despite different names*

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder/__main__.py` & `je_mail_thunder-0.0.9/je_mail_thunder/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 # argparse
 import argparse
 import json
+import sys
 
 from je_mail_thunder.smtp.smtp_wrapper import SMTPWrapper
 from je_mail_thunder.utils.exception.exception_tags import mail_thunder_login_error, \
     mail_thunder_argparse_get_wrong_function
 from je_mail_thunder.utils.exception.exceptions import MailThunderArgparseException
 
 if __name__ == "__main__":
-    smtp_service = SMTPWrapper()
+    try:
+        smtp_service = SMTPWrapper()
 
-    argparse_service_function_dict = {
-        "send_mail": smtp_service.create_message_and_send,
-        "send_mail_with_attach": smtp_service.create_message_with_attach_and_send,
-        "login_with_env_or_content": smtp_service.try_to_login_with_env_or_content
-    }
-
-    all_param_required_function_list = ["send_mail", "send_mail_with_attach"]
-
-    only_function_param_function_list = [
-        "login_with_env_or_content"
-    ]
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--user", help="set email user")
-    parser.add_argument("--password", help="set email password")
-    parser.add_argument("--function", help="service function", required=True)
-    parser.add_argument("--setting", help="service function setting as json")
-    args = parser.parse_args()
-    args = vars(args)
-    if args.get("function") in all_param_required_function_list:
-        setting = args.get("setting")
-        setting = setting.replace("\"", "").replace("'", '"')
-        for param in args.values():
-            if param is None:
-                raise MailThunderArgparseException(mail_thunder_login_error)
-        smtp_service.login(args.get("user"), args.get("password"))
-        argparse_service_function_dict.get(args.get("function"))(**json.loads(setting))
-    elif args.get("function") in only_function_param_function_list:
-        argparse_service_function_dict.get(args.get("function"))()
-    else:
-        raise MailThunderArgparseException(mail_thunder_argparse_get_wrong_function)
+        argparse_service_function_dict = {
+            "send_mail": smtp_service.create_message_and_send,
+            "send_mail_with_attach": smtp_service.create_message_with_attach_and_send,
+            "login_with_env_or_content": smtp_service.try_to_login_with_env_or_content
+        }
+
+        all_param_required_function_list = ["send_mail", "send_mail_with_attach"]
+
+        only_function_param_function_list = [
+            "login_with_env_or_content"
+        ]
+
+        parser = argparse.ArgumentParser()
+        parser.add_argument("--user", help="set email user")
+        parser.add_argument("--password", help="set email password")
+        parser.add_argument("--function", help="service function", required=True)
+        parser.add_argument("--setting", help="service function setting as json")
+        args = parser.parse_args()
+        args = vars(args)
+        if args.get("function") in all_param_required_function_list:
+            setting = args.get("setting")
+            setting = setting.replace("\"", "").replace("'", '"')
+            for param in args.values():
+                if param is None:
+                    raise MailThunderArgparseException(mail_thunder_login_error)
+            smtp_service.login(args.get("user"), args.get("password"))
+            argparse_service_function_dict.get(args.get("function"))(**json.loads(setting))
+        elif args.get("function") in only_function_param_function_list:
+            argparse_service_function_dict.get(args.get("function"))()
+        else:
+            raise MailThunderArgparseException(mail_thunder_argparse_get_wrong_function)
+    except Exception as error:
+        print(repr(error), file=sys.stderr)
+        sys.exit(1)
```

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder.egg-info/PKG-INFO` & `je_mail_thunder-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: je-mail-thunder
-Version: 0.0.8
+Name: je_mail_thunder
+Version: 0.0.9
 Summary: mail wrapper
 Home-page: https://github.com/JE-Chen/PythonMailWrapper_JE
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Description: # mail thunder a stand python mail module wrapper
```

### Comparing `je_mail_thunder-0.0.8/je_mail_thunder.egg-info/SOURCES.txt` & `je_mail_thunder-0.0.9/je_mail_thunder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_mail_thunder-0.0.8/PKG-INFO` & `je_mail_thunder-0.0.9/je_mail_thunder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: je_mail_thunder
-Version: 0.0.8
+Name: je-mail-thunder
+Version: 0.0.9
 Summary: mail wrapper
 Home-page: https://github.com/JE-Chen/PythonMailWrapper_JE
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Description: # mail thunder a stand python mail module wrapper
```

### Comparing `je_mail_thunder-0.0.8/setup.py` & `je_mail_thunder-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_mail_thunder",
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

