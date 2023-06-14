# Comparing `tmp/hoyo_daily_logins_helper-2.6.1.tar.gz` & `tmp/hoyo_daily_logins_helper-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo_daily_logins_helper-2.6.1.tar", max compression
+gzip compressed data, was "hoyo_daily_logins_helper-2.6.2.tar", max compression
```

## Comparing `hoyo_daily_logins_helper-2.6.1.tar` & `hoyo_daily_logins_helper-2.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34227 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/LICENSE
--rw-r--r--   0        0        0     5277 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/__init__.py
--rw-r--r--   0        0        0       55 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/__main__.py
--rw-r--r--   0        0        0       80 2023-06-14 02:50:15.812923 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/_version.py
--rw-r--r--   0        0        0       27 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/consts.py
--rw-r--r--   0        0        0     6916 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/games.py
--rw-r--r--   0        0        0     2050 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/http.py
--rw-r--r--   0        0        0     7180 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/main.py
--rw-r--r--   0        0        0     3410 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/notifications.py
--rw-r--r--   0        0        0     2631 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/scheduler.py
--rw-r--r--   0        0        0      100 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/utils.py
--rw-r--r--   0        0        0     1396 2023-06-14 02:50:15.812923 hoyo_daily_logins_helper-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 hoyo_daily_logins_helper-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34227 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/LICENSE
+-rw-r--r--   0        0        0     5277 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0        0        0       55 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0        0        0       80 2023-06-14 03:01:46.477008 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0        0        0       27 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0        0        0     6916 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0        0        0     2050 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0        0        0     7180 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0        0        0     3410 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0        0        0     2631 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0        0        0      100 2023-06-14 03:01:20.736721 hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/utils.py
+-rw-r--r--   0        0        0     1713 2023-06-14 03:01:46.477008 hoyo_daily_logins_helper-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 hoyo_daily_logins_helper-2.6.2/PKG-INFO
```

### Comparing `hoyo_daily_logins_helper-2.6.1/LICENSE` & `hoyo_daily_logins_helper-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.1/README.md` & `hoyo_daily_logins_helper-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/games.py` & `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/games.py`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/http.py` & `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/http.py`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/main.py` & `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/main.py`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/notifications.py` & `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/notifications.py`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/scheduler.py` & `hoyo_daily_logins_helper-2.6.2/hoyo_daily_logins_helper/scheduler.py`

 * *Files identical despite different names*

### Comparing `hoyo_daily_logins_helper-2.6.1/pyproject.toml` & `hoyo_daily_logins_helper-2.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 [tool.poetry]
 name = "hoyo-daily-logins-helper"
 description = "Get hoyo daily login rewards automatically!"
 authors = ["Christopher Kaster <me@atomicptr.de>"]
-license = "GPLv3"
+license = "GPL-3.0-or-later"
+homepage = "https://github.com/atomicptr/hoyo-daily-logins-helper"
+repository = "https://github.com/atomicptr/hoyo-daily-logins-helper"
 readme = "README.md"
 packages = [{include = "hoyo_daily_logins_helper"}]
+keywords = ["genshin", "genshin-impact", "starrail", "honkai-starrail", "game"]
+classifiers = [
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+]
 
 # required, but set automatically by poetry-dynamic-versioning
-version = "2.6.1"
+version = "2.6.2"
 
 [tool.poetry.scripts]
 hoyo-daily-logins-helper = "hoyo_daily_logins_helper.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
```

### Comparing `hoyo_daily_logins_helper-2.6.1/PKG-INFO` & `hoyo_daily_logins_helper-2.6.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.6.1
+Version: 2.6.2
 Summary: Get hoyo daily login rewards automatically!
-License: GPLv3
+Home-page: https://github.com/atomicptr/hoyo-daily-logins-helper
+License: GPL-3.0-or-later
+Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Author: Christopher Kaster
 Author-email: me@atomicptr.de
 Requires-Python: >=3.11,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: comboparse (>=1.0.1,<2.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scheduler (>=0.8.4,<0.9.0)
+Project-URL: Repository, https://github.com/atomicptr/hoyo-daily-logins-helper
 Description-Content-Type: text/markdown
 
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
 ![](https://i.imgur.com/LiWb3EG.png)
```

