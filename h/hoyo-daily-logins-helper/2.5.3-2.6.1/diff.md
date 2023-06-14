# Comparing `tmp/hoyo-daily-logins-helper-2.5.3.tar.gz` & `tmp/hoyo_daily_logins_helper-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.5.3.tar", last modified: Wed Jun 14 01:10:41 2023, max compression
+gzip compressed data, was "hoyo_daily_logins_helper-2.6.1.tar", max compression
```

## Comparing `hoyo-daily-logins-helper-2.5.3.tar` & `hoyo_daily_logins_helper-2.6.1.tar`

### file list

```diff
@@ -1,35 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.110524 hoyo-daily-logins-helper-2.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.110524 hoyo-daily-logins-helper-2.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/setup.py
+-rw-r--r--   0        0        0    34227 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/LICENSE
+-rw-r--r--   0        0        0     5277 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0        0        0       55 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0        0        0       80 2023-06-14 02:50:15.812923 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0        0        0       27 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0        0        0     6916 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0        0        0     2050 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0        0        0     7180 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0        0        0     3410 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0        0        0     2631 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0        0        0      100 2023-06-14 02:49:50.104569 hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/utils.py
+-rw-r--r--   0        0        0     1396 2023-06-14 02:50:15.812923 hoyo_daily_logins_helper-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 hoyo_daily_logins_helper-2.6.1/PKG-INFO
```

### Comparing `hoyo-daily-logins-helper-2.5.3/LICENSE` & `hoyo_daily_logins_helper-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.3/PKG-INFO` & `hoyo_daily_logins_helper-2.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: hoyo-daily-logins-helper
-Version: 2.5.3
-Summary: Get hoyo daily login rewards automatically!
-Author-email: Christopher Kaster <me@atomicptr.de>
-Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
 ![](https://i.imgur.com/LiWb3EG.png)
 
 ## Usage
@@ -118,15 +107,15 @@
 ```toml
 # you can configurate some things here like the language or the user agent
 # keep in mind that config and every key in there is optional and you can omit it
 [config]
 # i'd recommend against changing this value unless you know what you are doing
 # not setting this will make it look to the developer like we are using a normal
 # web browser while this is very suspicious
-user-agent = "My fancy user agent"
+user_agent = "My fancy user agent"
 # the language of the rewards and presumably return messages from the API
 language = "en-us"
 
 # every account starts with this index/key 
 [[accounts]]
 # accounts can have identifiers for you to differentiate them in the logs
 # you could for instance add your account name or UID here
@@ -177,8 +166,8 @@
 # ....
 ```
 
 ## License
 
 GNU General Public License v3
 
-![](https://www.gnu.org/graphics/gplv3-127x51.png)
+![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.5.3/README.md` & `hoyo_daily_logins_helper-2.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: hoyo-daily-logins-helper
+Version: 2.6.1
+Summary: Get hoyo daily login rewards automatically!
+License: GPLv3
+Author: Christopher Kaster
+Author-email: me@atomicptr.de
+Requires-Python: >=3.11,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: comboparse (>=1.0.1,<2.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: scheduler (>=0.8.4,<0.9.0)
+Description-Content-Type: text/markdown
+
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
 ![](https://i.imgur.com/LiWb3EG.png)
 
 ## Usage
@@ -107,15 +124,15 @@
 ```toml
 # you can configurate some things here like the language or the user agent
 # keep in mind that config and every key in there is optional and you can omit it
 [config]
 # i'd recommend against changing this value unless you know what you are doing
 # not setting this will make it look to the developer like we are using a normal
 # web browser while this is very suspicious
-user-agent = "My fancy user agent"
+user_agent = "My fancy user agent"
 # the language of the rewards and presumably return messages from the API
 language = "en-us"
 
 # every account starts with this index/key 
 [[accounts]]
 # accounts can have identifiers for you to differentiate them in the logs
 # you could for instance add your account name or UID here
@@ -166,8 +183,8 @@
 # ....
 ```
 
 ## License
 
 GNU General Public License v3
 
-![](https://www.gnu.org/graphics/gplv3-127x51.png)
+![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/games.py` & `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/games.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/http.py` & `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/main.py` & `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import sys
-import tomllib
 from pathlib import Path
 
 import comboparse
+import tomllib
 
 from hoyo_daily_logins_helper._version import __version__
 from hoyo_daily_logins_helper.consts import DEFAULT_LANGUAGE
 from hoyo_daily_logins_helper.games import GAMES, game_perform_checkin
 from hoyo_daily_logins_helper.http import http_set_user_agent
 from hoyo_daily_logins_helper.notifications import NotificationManager
 from hoyo_daily_logins_helper.scheduler import run_scheduler
@@ -153,15 +153,25 @@
 
             # parse config from toml file
             language = config_data.get("config", {}).get("language", None)
 
             if language:
                 args.language = language
 
-            user_agent = config_data.get("config", {}).get("user-agent", None)
+            user_agent = config_data.get("config", {}).get("user_agent", None)
+
+            # TODO: remove this eventually
+            if not user_agent:
+                user_agent = config_data.get("config", {})\
+                    .get("user-agent", None)
+                if user_agent:
+                    logging.warning(
+                        "DEPRECATED: using deprecated user-agent configuration"
+                        ", please use user_agent instead!",
+                    )
 
             if user_agent:
                 args.user_agent = user_agent
 
             enable_scheduler = config_data.get("config", {}) \
                 .get("enable_scheduler", False)
```

### Comparing `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/notifications.py` & `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/notifications.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/scheduler.py` & `hoyo_daily_logins_helper-2.6.1/hoyo_daily_logins_helper/scheduler.py`

 * *Files identical despite different names*

