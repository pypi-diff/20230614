# Comparing `tmp/ofx_processor-4.4.3.tar.gz` & `tmp/ofx_processor-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofx_processor-4.4.3.tar", max compression
+gzip compressed data, was "ofx_processor-4.4.4.tar", max compression
```

## Comparing `ofx_processor-4.4.3.tar` & `ofx_processor-4.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx_processor-4.4.3/LICENSE
--rw-r--r--   0        0        0     1463 2023-06-14 06:13:48.297259 ofx_processor-4.4.3/README.md
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx_processor-4.4.3/ofx_processor/__init__.py
--rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx_processor-4.4.3/ofx_processor/downloaders/__init__.py
--rw-r--r--   0        0        0     4250 2023-06-14 06:53:37.135330 ofx_processor-4.4.3/ofx_processor/downloaders/lcl.py
--rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx_processor-4.4.3/ofx_processor/main.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx_processor-4.4.3/ofx_processor/processors/__init__.py
--rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx_processor-4.4.3/ofx_processor/processors/bpvf.py
--rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx_processor-4.4.3/ofx_processor/processors/ce.py
--rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx_processor-4.4.3/ofx_processor/processors/lcl.py
--rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx_processor-4.4.3/ofx_processor/processors/revolut.py
--rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx_processor-4.4.3/ofx_processor/senders/__init__.py
--rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx_processor-4.4.3/ofx_processor/senders/email.py
--rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx_processor-4.4.3/ofx_processor/senders/home_assistant.py
--rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx_processor-4.4.3/ofx_processor/senders/sms.py
--rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx_processor-4.4.3/ofx_processor/senders/telegram.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx_processor-4.4.3/ofx_processor/utils/__init__.py
--rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx_processor-4.4.3/ofx_processor/utils/base_ofx.py
--rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx_processor-4.4.3/ofx_processor/utils/base_processor.py
--rw-r--r--   0        0        0     5707 2022-10-10 20:41:41.687648 ofx_processor-4.4.3/ofx_processor/utils/config.py
--rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx_processor-4.4.3/ofx_processor/utils/utils.py
--rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx_processor-4.4.3/ofx_processor/utils/ynab.py
--rw-r--r--   0        0        0     1741 2023-06-14 06:53:47.014282 ofx_processor-4.4.3/pyproject.toml
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 ofx_processor-4.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx_processor-4.4.4/LICENSE
+-rw-r--r--   0        0        0     1463 2023-06-14 06:13:48.297259 ofx_processor-4.4.4/README.md
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx_processor-4.4.4/ofx_processor/__init__.py
+-rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx_processor-4.4.4/ofx_processor/downloaders/__init__.py
+-rw-r--r--   0        0        0     4237 2023-06-14 06:57:24.979025 ofx_processor-4.4.4/ofx_processor/downloaders/lcl.py
+-rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx_processor-4.4.4/ofx_processor/main.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx_processor-4.4.4/ofx_processor/processors/__init__.py
+-rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx_processor-4.4.4/ofx_processor/processors/bpvf.py
+-rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx_processor-4.4.4/ofx_processor/processors/ce.py
+-rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx_processor-4.4.4/ofx_processor/processors/lcl.py
+-rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx_processor-4.4.4/ofx_processor/processors/revolut.py
+-rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx_processor-4.4.4/ofx_processor/senders/__init__.py
+-rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx_processor-4.4.4/ofx_processor/senders/email.py
+-rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx_processor-4.4.4/ofx_processor/senders/home_assistant.py
+-rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx_processor-4.4.4/ofx_processor/senders/sms.py
+-rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx_processor-4.4.4/ofx_processor/senders/telegram.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx_processor-4.4.4/ofx_processor/utils/__init__.py
+-rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx_processor-4.4.4/ofx_processor/utils/base_ofx.py
+-rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx_processor-4.4.4/ofx_processor/utils/base_processor.py
+-rw-r--r--   0        0        0     5844 2023-06-14 06:57:17.688436 ofx_processor-4.4.4/ofx_processor/utils/config.py
+-rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx_processor-4.4.4/ofx_processor/utils/utils.py
+-rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx_processor-4.4.4/ofx_processor/utils/ynab.py
+-rw-r--r--   0        0        0     1741 2023-06-14 06:57:57.766332 ofx_processor-4.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 ofx_processor-4.4.4/PKG-INFO
```

### Comparing `ofx_processor-4.4.3/LICENSE` & `ofx_processor-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/README.md` & `ofx_processor-4.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/downloaders/lcl.py` & `ofx_processor-4.4.4/ofx_processor/downloaders/lcl.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.selenium = webdriver.Firefox(options=options)
         self.selenium.implicitly_wait(30)
 
     def download(self) -> str:
         try:
             return self._download()
         except Exception:
-            screenshot = Path(os.getenv("SCREENSHOT_DIR", default="/tmp")) / "error_download.png"
+            screenshot = Path(self.config.screenshot_dir) / "error_download_lcl.png"
             self.selenium.save_screenshot(screenshot)
             raise
 
     def _download(self) -> str:
         selenium = self.selenium
 
         click.secho("Logging in to LCL...", fg="blue")
```

### Comparing `ofx_processor-4.4.3/ofx_processor/main.py` & `ofx_processor-4.4.4/ofx_processor/main.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/processors/bpvf.py` & `ofx_processor-4.4.4/ofx_processor/processors/bpvf.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/processors/ce.py` & `ofx_processor-4.4.4/ofx_processor/processors/ce.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/processors/lcl.py` & `ofx_processor-4.4.4/ofx_processor/processors/lcl.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/processors/revolut.py` & `ofx_processor-4.4.4/ofx_processor/processors/revolut.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/senders/email.py` & `ofx_processor-4.4.4/ofx_processor/senders/email.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/senders/home_assistant.py` & `ofx_processor-4.4.4/ofx_processor/senders/home_assistant.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/senders/sms.py` & `ofx_processor-4.4.4/ofx_processor/senders/sms.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/senders/telegram.py` & `ofx_processor-4.4.4/ofx_processor/senders/telegram.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/utils/base_ofx.py` & `ofx_processor-4.4.4/ofx_processor/utils/base_ofx.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/utils/base_processor.py` & `ofx_processor-4.4.4/ofx_processor/utils/base_processor.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/utils/config.py` & `ofx_processor-4.4.4/ofx_processor/utils/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 def get_default_config():
     default_config = configparser.ConfigParser()
     default_config["DEFAULT"] = {
         "token": "<YOUR API TOKEN>",
         "budget": "<YOUR BUDGET ID>",
+        "screenshot_dir": "/tmp",
         "mailgun_api_key": "",
         "mailgun_domain": "",
         "mailgun_from": "",
         "email_recipient": "",
     }
     default_config["bpvf"] = {"account": "<YOUR ACCOUNT ID>"}
     default_config["revolut"] = {"account": "<YOUR ACCOUNT ID>"}
@@ -72,14 +73,15 @@
 
 
 @dataclass(frozen=True)
 class Config:
     account: str
     budget_id: str
     token: str
+    screenshot_dir: str
     bank_identifier: Optional[str] = None
     bank_password: Optional[str] = None
     mailgun_api_key: Optional[str] = None
     mailgun_domain: Optional[str] = None
     mailgun_from: Optional[str] = None
     email_recipient: Optional[str] = None
     sms_user: Optional[str] = None
@@ -148,14 +150,15 @@
     except configparser.Error as e:
         return handle_config_file_error(config_file, e)
 
     try:
         section = config[account]
         budget_id = section["budget"]
         token = section["token"]
+        screenshot_dir = section.get("screenshot_dir")
         if account == "DEFAULT":
             ynab_account_id = ""
         else:
             ynab_account_id = section["account"]
         bank_identifier = section.get("bank_identifier")
         bank_password = section.get("bank_password")
         mailgun_api_key = section.get("mailgun_api_key")
@@ -170,14 +173,15 @@
     except KeyError as e:
         return handle_config_file_error(config_file, e)
 
     return Config(
         ynab_account_id,
         budget_id,
         token,
+        screenshot_dir,
         bank_identifier,
         bank_password,
         mailgun_api_key,
         mailgun_domain,
         mailgun_from,
         email_recipient,
         sms_user,
```

### Comparing `ofx_processor-4.4.3/ofx_processor/utils/utils.py` & `ofx_processor-4.4.4/ofx_processor/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/ofx_processor/utils/ynab.py` & `ofx_processor-4.4.4/ofx_processor/utils/ynab.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.3/pyproject.toml` & `ofx_processor-4.4.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofx-processor"
-version = "4.4.3"
+version = "4.4.4"
 description = "Personal ofx processor"
 readme = "README.md"
 authors = ["Gabriel Augendre <gabriel@augendre.info>"]
 homepage = "https://git.augendre.info/gaugendre/ofx-processor"
 repository = "https://git.augendre.info/gaugendre/ofx-processor"
 keywords = [
     "ynab",
```

### Comparing `ofx_processor-4.4.3/PKG-INFO` & `ofx_processor-4.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofx-processor
-Version: 4.4.3
+Version: 4.4.4
 Summary: Personal ofx processor
 Home-page: https://git.augendre.info/gaugendre/ofx-processor
 Keywords: ynab,finances,finance automation
 Author: Gabriel Augendre
 Author-email: gabriel@augendre.info
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
```

