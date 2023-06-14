# Comparing `tmp/ofx-processor-4.3.1.tar.gz` & `tmp/ofx_processor-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofx-processor-4.3.1.tar", max compression
+gzip compressed data, was "ofx_processor-4.4.0.tar", max compression
```

## Comparing `ofx-processor-4.3.1.tar` & `ofx_processor-4.4.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx-processor-4.3.1/LICENSE
--rw-r--r--   0        0        0     1463 2022-03-12 07:13:22.250649 ofx-processor-4.3.1/README.md
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx-processor-4.3.1/ofx_processor/__init__.py
--rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx-processor-4.3.1/ofx_processor/downloaders/__init__.py
--rw-r--r--   0        0        0     3684 2022-11-05 19:34:10.031838 ofx-processor-4.3.1/ofx_processor/downloaders/lcl.py
--rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx-processor-4.3.1/ofx_processor/main.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx-processor-4.3.1/ofx_processor/processors/__init__.py
--rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx-processor-4.3.1/ofx_processor/processors/bpvf.py
--rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx-processor-4.3.1/ofx_processor/processors/ce.py
--rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx-processor-4.3.1/ofx_processor/processors/lcl.py
--rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx-processor-4.3.1/ofx_processor/processors/revolut.py
--rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx-processor-4.3.1/ofx_processor/senders/__init__.py
--rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx-processor-4.3.1/ofx_processor/senders/email.py
--rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx-processor-4.3.1/ofx_processor/senders/home_assistant.py
--rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx-processor-4.3.1/ofx_processor/senders/sms.py
--rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx-processor-4.3.1/ofx_processor/senders/telegram.py
--rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx-processor-4.3.1/ofx_processor/utils/__init__.py
--rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx-processor-4.3.1/ofx_processor/utils/base_ofx.py
--rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx-processor-4.3.1/ofx_processor/utils/base_processor.py
--rw-r--r--   0        0        0     5707 2022-10-10 20:41:41.687648 ofx-processor-4.3.1/ofx_processor/utils/config.py
--rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx-processor-4.3.1/ofx_processor/utils/utils.py
--rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx-processor-4.3.1/ofx_processor/utils/ynab.py
--rw-r--r--   0        0        0     1801 2022-11-05 19:34:57.280815 ofx-processor-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     2509 2022-11-05 19:35:27.166356 ofx-processor-4.3.1/setup.py
--rw-r--r--   0        0        0     2748 2022-11-05 19:35:27.166593 ofx-processor-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1212 2022-03-12 07:13:22.250518 ofx_processor-4.4.0/LICENSE
+-rw-r--r--   0        0        0     1463 2023-06-14 06:13:48.297259 ofx_processor-4.4.0/README.md
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.250751 ofx_processor-4.4.0/ofx_processor/__init__.py
+-rw-r--r--   0        0        0       31 2022-03-12 07:13:22.250941 ofx_processor-4.4.0/ofx_processor/downloaders/__init__.py
+-rw-r--r--   0        0        0     3936 2023-06-14 06:02:16.226922 ofx_processor-4.4.0/ofx_processor/downloaders/lcl.py
+-rw-r--r--   0        0        0      562 2022-03-12 07:13:22.251191 ofx_processor-4.4.0/ofx_processor/main.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251308 ofx_processor-4.4.0/ofx_processor/processors/__init__.py
+-rw-r--r--   0        0        0     1165 2022-03-12 07:13:22.251431 ofx_processor-4.4.0/ofx_processor/processors/bpvf.py
+-rw-r--r--   0        0        0     1084 2022-03-12 07:13:22.251562 ofx_processor-4.4.0/ofx_processor/processors/ce.py
+-rw-r--r--   0        0        0     2848 2022-10-10 20:29:32.527872 ofx_processor-4.4.0/ofx_processor/processors/lcl.py
+-rw-r--r--   0        0        0     1802 2022-03-12 07:13:22.251795 ofx_processor-4.4.0/ofx_processor/processors/revolut.py
+-rw-r--r--   0        0        0      206 2022-10-10 20:41:41.686272 ofx_processor-4.4.0/ofx_processor/senders/__init__.py
+-rw-r--r--   0        0        0      742 2022-10-10 20:41:41.686495 ofx_processor-4.4.0/ofx_processor/senders/email.py
+-rw-r--r--   0        0        0      527 2022-10-10 20:41:41.686706 ofx_processor-4.4.0/ofx_processor/senders/home_assistant.py
+-rw-r--r--   0        0        0      587 2022-10-10 20:41:41.686941 ofx_processor-4.4.0/ofx_processor/senders/sms.py
+-rw-r--r--   0        0        0      762 2022-10-10 20:41:41.687135 ofx_processor-4.4.0/ofx_processor/senders/telegram.py
+-rw-r--r--   0        0        0        0 2022-03-12 07:13:22.251892 ofx_processor-4.4.0/ofx_processor/utils/__init__.py
+-rw-r--r--   0        0        0     1688 2022-10-10 20:41:41.687429 ofx_processor-4.4.0/ofx_processor/utils/base_ofx.py
+-rw-r--r--   0        0        0     1976 2022-03-12 07:13:22.252152 ofx_processor-4.4.0/ofx_processor/utils/base_processor.py
+-rw-r--r--   0        0        0     5707 2022-10-10 20:41:41.687648 ofx_processor-4.4.0/ofx_processor/utils/config.py
+-rw-r--r--   0        0        0     3217 2022-10-10 20:41:41.687921 ofx_processor-4.4.0/ofx_processor/utils/utils.py
+-rw-r--r--   0        0        0     1357 2022-03-12 07:13:22.252544 ofx_processor-4.4.0/ofx_processor/utils/ynab.py
+-rw-r--r--   0        0        0     1741 2023-06-14 06:11:00.896889 ofx_processor-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 ofx_processor-4.4.0/PKG-INFO
```

### Comparing `ofx-processor-4.3.1/LICENSE` & `ofx_processor-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/README.md` & `ofx_processor-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/downloaders/lcl.py` & `ofx_processor-4.4.0/ofx_processor/downloaders/lcl.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,20 @@
         self._click(By.CLASS_NAME, "app-cta-button")
         for char in self.config.bank_password:
             self._click(By.CSS_SELECTOR, f".pad-button[value='{char}']")
         self._click(By.CLASS_NAME, "app-cta-button")
         click.secho("Logged in!", fg="green")
 
         try:
+            self._click(By.CSS_SELECTOR, ".app-cta-button--primary")
+            click.secho("Dismissing welcome screen...", fg="blue")
+        except NoSuchElementException:
+            click.secho("No welcome screen found.", fg="blue")
+
+        try:
             self._click(By.CSS_SELECTOR, ".burger-menu-content")
             self._click(By.CSS_SELECTOR, ".return-legacy-button")
             click.secho("Going back to legacy version...", fg="blue")
         except NoSuchElementException:
             click.secho("Probably already on legacy version.", fg="blue")
 
         click.secho("Navigating through archives...", fg="blue")
```

### Comparing `ofx-processor-4.3.1/ofx_processor/main.py` & `ofx_processor-4.4.0/ofx_processor/main.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/processors/bpvf.py` & `ofx_processor-4.4.0/ofx_processor/processors/bpvf.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/processors/ce.py` & `ofx_processor-4.4.0/ofx_processor/processors/ce.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/processors/lcl.py` & `ofx_processor-4.4.0/ofx_processor/processors/lcl.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/processors/revolut.py` & `ofx_processor-4.4.0/ofx_processor/processors/revolut.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/senders/email.py` & `ofx_processor-4.4.0/ofx_processor/senders/email.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/senders/home_assistant.py` & `ofx_processor-4.4.0/ofx_processor/senders/home_assistant.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/senders/sms.py` & `ofx_processor-4.4.0/ofx_processor/senders/sms.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/senders/telegram.py` & `ofx_processor-4.4.0/ofx_processor/senders/telegram.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/utils/base_ofx.py` & `ofx_processor-4.4.0/ofx_processor/utils/base_ofx.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/utils/base_processor.py` & `ofx_processor-4.4.0/ofx_processor/utils/base_processor.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/utils/config.py` & `ofx_processor-4.4.0/ofx_processor/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/utils/utils.py` & `ofx_processor-4.4.0/ofx_processor/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/ofx_processor/utils/ynab.py` & `ofx_processor-4.4.0/ofx_processor/utils/ynab.py`

 * *Files identical despite different names*

### Comparing `ofx-processor-4.3.1/pyproject.toml` & `ofx_processor-4.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofx-processor"
-version = "4.3.1"
+version = "4.4.0"
 description = "Personal ofx processor"
 readme = "README.md"
 authors = ["Gabriel Augendre <gabriel@augendre.info>"]
 homepage = "https://git.augendre.info/gaugendre/ofx-processor"
 repository = "https://git.augendre.info/gaugendre/ofx-processor"
 keywords = [
     "ynab",
@@ -16,34 +16,33 @@
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: The Unlicense (Unlicense)",
     "Natural Language :: English",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: Unix",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4"
+python = ">=3.10,<4"
 ofxtools = ">=0.9.4"
 click = ">=8.0.3"
 dateparser = ">=1.1.0"
 requests = ">=2.24.0"
 selenium = ">=4.0.0"
 python-telegram-bot = {version = ">=20.0a4", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0.1"
 pytest-cov = ">=3.0.0"
-invoke = ">=1.6.0"
+invoke = ">=2.0.0"
 pre-commit = ">=2.15.0"
 tox = ">=3.24.4"
 pdbpp = ">=0.10.3"
 
 [tool.poetry.scripts]
 ynab = 'ofx_processor.main:cli'
 
@@ -53,20 +52,20 @@
 [tool.isort]
 profile = "black"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
-envlist = py38, py39, py310
+envlist = py310, py311
 
 [testenv]
-whitelist_externals = poetry
+allowlist_externals = poetry
 commands =
-    poetry install --remove-untracked
+    poetry install --sync
     poetry run inv test
 """
 
 [tool.coverage.run]
 omit = ["tasks.py"]
 branch = true
```

### Comparing `ofx-processor-4.3.1/PKG-INFO` & `ofx_processor-4.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: ofx-processor
-Version: 4.3.1
+Version: 4.4.0
 Summary: Personal ofx processor
 Home-page: https://git.augendre.info/gaugendre/ofx-processor
 Keywords: ynab,finances,finance automation
 Author: Gabriel Augendre
 Author-email: gabriel@augendre.info
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.0.3)
 Requires-Dist: dateparser (>=1.1.0)
 Requires-Dist: ofxtools (>=0.9.4)
 Requires-Dist: python-telegram-bot (>=20.0a4)
 Requires-Dist: requests (>=2.24.0)
 Requires-Dist: selenium (>=4.0.0)
```

