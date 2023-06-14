# Comparing `tmp/ofx_processor-4.4.2.tar.gz` & `tmp/ofx_processor-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofx_processor-4.4.2.tar", max compression
+gzip compressed data, was "ofx_processor-4.4.3.tar", max compression
```

## Comparing `ofx_processor-4.4.2.tar` & `ofx_processor-4.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx_processor-4.4.2/LICENSE
--rw-r--r--   0        0        0     1463 2023-06-14 06:13:48.297259 ofx_processor-4.4.2/README.md
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx_processor-4.4.2/ofx_processor/__init__.py
--rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx_processor-4.4.2/ofx_processor/downloaders/__init__.py
--rw-r--r--   0        0        0     3962 2023-06-14 06:39:45.893419 ofx_processor-4.4.2/ofx_processor/downloaders/lcl.py
--rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx_processor-4.4.2/ofx_processor/main.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx_processor-4.4.2/ofx_processor/processors/__init__.py
--rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx_processor-4.4.2/ofx_processor/processors/bpvf.py
--rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx_processor-4.4.2/ofx_processor/processors/ce.py
--rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx_processor-4.4.2/ofx_processor/processors/lcl.py
--rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx_processor-4.4.2/ofx_processor/processors/revolut.py
--rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx_processor-4.4.2/ofx_processor/senders/__init__.py
--rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx_processor-4.4.2/ofx_processor/senders/email.py
--rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx_processor-4.4.2/ofx_processor/senders/home_assistant.py
--rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx_processor-4.4.2/ofx_processor/senders/sms.py
--rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx_processor-4.4.2/ofx_processor/senders/telegram.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx_processor-4.4.2/ofx_processor/utils/__init__.py
--rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx_processor-4.4.2/ofx_processor/utils/base_ofx.py
--rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx_processor-4.4.2/ofx_processor/utils/base_processor.py
--rw-r--r--   0        0        0     5707 2022-10-10 20:41:41.687648 ofx_processor-4.4.2/ofx_processor/utils/config.py
--rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx_processor-4.4.2/ofx_processor/utils/utils.py
--rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx_processor-4.4.2/ofx_processor/utils/ynab.py
--rw-r--r--   0        0        0     1741 2023-06-14 06:39:58.981100 ofx_processor-4.4.2/pyproject.toml
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 ofx_processor-4.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx_processor-4.4.3/LICENSE
+-rw-r--r--   0        0        0     1463 2023-06-14 06:13:48.297259 ofx_processor-4.4.3/README.md
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx_processor-4.4.3/ofx_processor/__init__.py
+-rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx_processor-4.4.3/ofx_processor/downloaders/__init__.py
+-rw-r--r--   0        0        0     4250 2023-06-14 06:53:37.135330 ofx_processor-4.4.3/ofx_processor/downloaders/lcl.py
+-rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx_processor-4.4.3/ofx_processor/main.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx_processor-4.4.3/ofx_processor/processors/__init__.py
+-rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx_processor-4.4.3/ofx_processor/processors/bpvf.py
+-rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx_processor-4.4.3/ofx_processor/processors/ce.py
+-rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx_processor-4.4.3/ofx_processor/processors/lcl.py
+-rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx_processor-4.4.3/ofx_processor/processors/revolut.py
+-rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx_processor-4.4.3/ofx_processor/senders/__init__.py
+-rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx_processor-4.4.3/ofx_processor/senders/email.py
+-rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx_processor-4.4.3/ofx_processor/senders/home_assistant.py
+-rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx_processor-4.4.3/ofx_processor/senders/sms.py
+-rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx_processor-4.4.3/ofx_processor/senders/telegram.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx_processor-4.4.3/ofx_processor/utils/__init__.py
+-rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx_processor-4.4.3/ofx_processor/utils/base_ofx.py
+-rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx_processor-4.4.3/ofx_processor/utils/base_processor.py
+-rw-r--r--   0        0        0     5707 2022-10-10 20:41:41.687648 ofx_processor-4.4.3/ofx_processor/utils/config.py
+-rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx_processor-4.4.3/ofx_processor/utils/utils.py
+-rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx_processor-4.4.3/ofx_processor/utils/ynab.py
+-rw-r--r--   0        0        0     1741 2023-06-14 06:53:47.014282 ofx_processor-4.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 ofx_processor-4.4.3/PKG-INFO
```

### Comparing `ofx_processor-4.4.2/LICENSE` & `ofx_processor-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/README.md` & `ofx_processor-4.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/downloaders/lcl.py` & `ofx_processor-4.4.3/ofx_processor/downloaders/lcl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import time
 from pathlib import Path
 
 import click
 from selenium import webdriver
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.common.by import By
@@ -31,14 +32,22 @@
         options.set_preference(
             "browser.helperApps.neverAsk.saveToDisk", "application/x-ofx"
         )
         self.selenium = webdriver.Firefox(options=options)
         self.selenium.implicitly_wait(30)
 
     def download(self) -> str:
+        try:
+            return self._download()
+        except Exception:
+            screenshot = Path(os.getenv("SCREENSHOT_DIR", default="/tmp")) / "error_download.png"
+            self.selenium.save_screenshot(screenshot)
+            raise
+
+    def _download(self) -> str:
         selenium = self.selenium
 
         click.secho("Logging in to LCL...", fg="blue")
         selenium.get("https://monespace.lcl.fr/connexion")
         try:
             self._click(By.ID, "popin_tc_privacy_button_2")
             click.secho("Accepting privacy policy...", fg="blue")
```

### Comparing `ofx_processor-4.4.2/ofx_processor/main.py` & `ofx_processor-4.4.3/ofx_processor/main.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/processors/bpvf.py` & `ofx_processor-4.4.3/ofx_processor/processors/bpvf.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/processors/ce.py` & `ofx_processor-4.4.3/ofx_processor/processors/ce.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/processors/lcl.py` & `ofx_processor-4.4.3/ofx_processor/processors/lcl.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/processors/revolut.py` & `ofx_processor-4.4.3/ofx_processor/processors/revolut.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/senders/email.py` & `ofx_processor-4.4.3/ofx_processor/senders/email.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/senders/home_assistant.py` & `ofx_processor-4.4.3/ofx_processor/senders/home_assistant.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/senders/sms.py` & `ofx_processor-4.4.3/ofx_processor/senders/sms.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/senders/telegram.py` & `ofx_processor-4.4.3/ofx_processor/senders/telegram.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/utils/base_ofx.py` & `ofx_processor-4.4.3/ofx_processor/utils/base_ofx.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/utils/base_processor.py` & `ofx_processor-4.4.3/ofx_processor/utils/base_processor.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/utils/config.py` & `ofx_processor-4.4.3/ofx_processor/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/utils/utils.py` & `ofx_processor-4.4.3/ofx_processor/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/ofx_processor/utils/ynab.py` & `ofx_processor-4.4.3/ofx_processor/utils/ynab.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.2/pyproject.toml` & `ofx_processor-4.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofx-processor"
-version = "4.4.2"
+version = "4.4.3"
 description = "Personal ofx processor"
 readme = "README.md"
 authors = ["Gabriel Augendre <gabriel@augendre.info>"]
 homepage = "https://git.augendre.info/gaugendre/ofx-processor"
 repository = "https://git.augendre.info/gaugendre/ofx-processor"
 keywords = [
     "ynab",
```

### Comparing `ofx_processor-4.4.2/PKG-INFO` & `ofx_processor-4.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofx-processor
-Version: 4.4.2
+Version: 4.4.3
 Summary: Personal ofx processor
 Home-page: https://git.augendre.info/gaugendre/ofx-processor
 Keywords: ynab,finances,finance automation
 Author: Gabriel Augendre
 Author-email: gabriel@augendre.info
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
```

