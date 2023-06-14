# Comparing `tmp/ofx_processor-4.4.1.tar.gz` & `tmp/ofx_processor-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofx_processor-4.4.1.tar", max compression
+gzip compressed data, was "ofx_processor-4.4.2.tar", max compression
```

## Comparing `ofx_processor-4.4.1.tar` & `ofx_processor-4.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx_processor-4.4.1/LICENSE
--rw-r--r--   0        0        0     1463 2023-06-14 06:13:48.297259 ofx_processor-4.4.1/README.md
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx_processor-4.4.1/ofx_processor/__init__.py
--rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx_processor-4.4.1/ofx_processor/downloaders/__init__.py
--rw-r--r--   0        0        0     3957 2023-06-14 06:35:24.567219 ofx_processor-4.4.1/ofx_processor/downloaders/lcl.py
--rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx_processor-4.4.1/ofx_processor/main.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx_processor-4.4.1/ofx_processor/processors/__init__.py
--rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx_processor-4.4.1/ofx_processor/processors/bpvf.py
--rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx_processor-4.4.1/ofx_processor/processors/ce.py
--rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx_processor-4.4.1/ofx_processor/processors/lcl.py
--rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx_processor-4.4.1/ofx_processor/processors/revolut.py
--rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx_processor-4.4.1/ofx_processor/senders/__init__.py
--rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx_processor-4.4.1/ofx_processor/senders/email.py
--rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx_processor-4.4.1/ofx_processor/senders/home_assistant.py
--rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx_processor-4.4.1/ofx_processor/senders/sms.py
--rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx_processor-4.4.1/ofx_processor/senders/telegram.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx_processor-4.4.1/ofx_processor/utils/__init__.py
--rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx_processor-4.4.1/ofx_processor/utils/base_ofx.py
--rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx_processor-4.4.1/ofx_processor/utils/base_processor.py
--rw-r--r--   0        0        0     5707 2022-10-10 20:41:41.687648 ofx_processor-4.4.1/ofx_processor/utils/config.py
--rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx_processor-4.4.1/ofx_processor/utils/utils.py
--rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx_processor-4.4.1/ofx_processor/utils/ynab.py
--rw-r--r--   0        0        0     1741 2023-06-14 06:35:31.758446 ofx_processor-4.4.1/pyproject.toml
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 ofx_processor-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx_processor-4.4.2/LICENSE
+-rw-r--r--   0        0        0     1463 2023-06-14 06:13:48.297259 ofx_processor-4.4.2/README.md
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx_processor-4.4.2/ofx_processor/__init__.py
+-rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx_processor-4.4.2/ofx_processor/downloaders/__init__.py
+-rw-r--r--   0        0        0     3962 2023-06-14 06:39:45.893419 ofx_processor-4.4.2/ofx_processor/downloaders/lcl.py
+-rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx_processor-4.4.2/ofx_processor/main.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx_processor-4.4.2/ofx_processor/processors/__init__.py
+-rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx_processor-4.4.2/ofx_processor/processors/bpvf.py
+-rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx_processor-4.4.2/ofx_processor/processors/ce.py
+-rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx_processor-4.4.2/ofx_processor/processors/lcl.py
+-rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx_processor-4.4.2/ofx_processor/processors/revolut.py
+-rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx_processor-4.4.2/ofx_processor/senders/__init__.py
+-rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx_processor-4.4.2/ofx_processor/senders/email.py
+-rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx_processor-4.4.2/ofx_processor/senders/home_assistant.py
+-rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx_processor-4.4.2/ofx_processor/senders/sms.py
+-rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx_processor-4.4.2/ofx_processor/senders/telegram.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx_processor-4.4.2/ofx_processor/utils/__init__.py
+-rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx_processor-4.4.2/ofx_processor/utils/base_ofx.py
+-rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx_processor-4.4.2/ofx_processor/utils/base_processor.py
+-rw-r--r--   0        0        0     5707 2022-10-10 20:41:41.687648 ofx_processor-4.4.2/ofx_processor/utils/config.py
+-rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx_processor-4.4.2/ofx_processor/utils/utils.py
+-rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx_processor-4.4.2/ofx_processor/utils/ynab.py
+-rw-r--r--   0        0        0     1741 2023-06-14 06:39:58.981100 ofx_processor-4.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 ofx_processor-4.4.2/PKG-INFO
```

### Comparing `ofx_processor-4.4.1/LICENSE` & `ofx_processor-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/README.md` & `ofx_processor-4.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/downloaders/lcl.py` & `ofx_processor-4.4.2/ofx_processor/downloaders/lcl.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             self._click(By.CSS_SELECTOR, f".pad-button[value='{char}']")
         self._click(By.CLASS_NAME, "app-cta-button")
         click.secho("Logged in!", fg="green")
 
         try:
             self._click(By.CSS_SELECTOR, ".app-cta-button--primary")
             click.secho("Dismissing welcome screen...", fg="blue")
-            sleep(2)
+            time.sleep(2)
         except NoSuchElementException:
             click.secho("No welcome screen found.", fg="blue")
 
         try:
             self._click(By.CSS_SELECTOR, ".burger-menu-content")
             self._click(By.CSS_SELECTOR, ".return-legacy-button")
             click.secho("Going back to legacy version...", fg="blue")
```

### Comparing `ofx_processor-4.4.1/ofx_processor/main.py` & `ofx_processor-4.4.2/ofx_processor/main.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/processors/bpvf.py` & `ofx_processor-4.4.2/ofx_processor/processors/bpvf.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/processors/ce.py` & `ofx_processor-4.4.2/ofx_processor/processors/ce.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/processors/lcl.py` & `ofx_processor-4.4.2/ofx_processor/processors/lcl.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/processors/revolut.py` & `ofx_processor-4.4.2/ofx_processor/processors/revolut.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/senders/email.py` & `ofx_processor-4.4.2/ofx_processor/senders/email.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/senders/home_assistant.py` & `ofx_processor-4.4.2/ofx_processor/senders/home_assistant.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/senders/sms.py` & `ofx_processor-4.4.2/ofx_processor/senders/sms.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/senders/telegram.py` & `ofx_processor-4.4.2/ofx_processor/senders/telegram.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/utils/base_ofx.py` & `ofx_processor-4.4.2/ofx_processor/utils/base_ofx.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/utils/base_processor.py` & `ofx_processor-4.4.2/ofx_processor/utils/base_processor.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/utils/config.py` & `ofx_processor-4.4.2/ofx_processor/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/utils/utils.py` & `ofx_processor-4.4.2/ofx_processor/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/ofx_processor/utils/ynab.py` & `ofx_processor-4.4.2/ofx_processor/utils/ynab.py`

 * *Files identical despite different names*

### Comparing `ofx_processor-4.4.1/pyproject.toml` & `ofx_processor-4.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofx-processor"
-version = "4.4.1"
+version = "4.4.2"
 description = "Personal ofx processor"
 readme = "README.md"
 authors = ["Gabriel Augendre <gabriel@augendre.info>"]
 homepage = "https://git.augendre.info/gaugendre/ofx-processor"
 repository = "https://git.augendre.info/gaugendre/ofx-processor"
 keywords = [
     "ynab",
```

### Comparing `ofx_processor-4.4.1/PKG-INFO` & `ofx_processor-4.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofx-processor
-Version: 4.4.1
+Version: 4.4.2
 Summary: Personal ofx processor
 Home-page: https://git.augendre.info/gaugendre/ofx-processor
 Keywords: ynab,finances,finance automation
 Author: Gabriel Augendre
 Author-email: gabriel@augendre.info
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
```

