# Comparing `tmp/hoyo-daily-logins-helper-2.5.2.tar.gz` & `tmp/hoyo-daily-logins-helper-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.5.2.tar", last modified: Sun Jun 11 03:59:18 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.5.3.tar", last modified: Wed Jun 14 01:10:41 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.5.2.tar` & `hoyo-daily-logins-helper-2.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.910649 hoyo-daily-logins-helper-2.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.110524 hoyo-daily-logins-helper-2.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.110524 hoyo-daily-logins-helper-2.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 01:10:41.000000 hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:10:41.114524 hoyo-daily-logins-helper-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:10:22.000000 hoyo-daily-logins-helper-2.5.3/setup.py
```

### Comparing `hoyo-daily-logins-helper-2.5.2/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.5.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.5.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/.gitignore` & `hoyo-daily-logins-helper-2.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/LICENSE` & `hoyo-daily-logins-helper-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/PKG-INFO` & `hoyo-daily-logins-helper-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.5.2
+Version: 2.5.3
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.5.2/README.md` & `hoyo-daily-logins-helper-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.5.3/hoyo-daily-logins-helper.toml.template`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/games.py` & `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/games.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         "event_base_url": "https://sg-public-api.hoyolab.com/event/luna/os",
         "act_id": "e202202281857121",
         "login_url": "https://act.hoyolab.com/bbs/event/signin/nxx/index.html"
                      "?act_id=e202202281857121",
     },
 }
 _CAPTCHA_MESSAGE = """Captcha is required, please sign into the website: %s"""
+_COULD_NOT_CLAIM = (
+    "Could not automatically claim rewards, please log in "
+    "manually again here: %s"
+)
 
 
 def game_perform_checkin(
         account_ident: str,
         game: str,
         cookie_str: str,
         language: str,
@@ -114,16 +118,39 @@
         response = http_post_json(sign_url, headers=headers, data=request_data)
     else:
         response = {
             "retcode": 0,
             "message": "Test Run, skipped actual checkin request",
         }
 
-    # as we logged in for a day, the number of total sign ins has to increase
-    total_sign_in_day += 1
+    # check if info has changed
+    info_list = http_get_json(info_url, headers=headers)
+
+    if not info_list.get("data"):
+        message = info_list.get("message", "None")
+        logging.error(f"Could not retrieve data from API endpoint: {message}")
+        return
+
+    new_total_sign_in_day = info_list.get("data", {}).get("total_sign_day")
+    already_signed_in = info_list.get("data", {}).get("is_sign")
+
+    if not already_signed_in or new_total_sign_in_day == total_sign_in_day:
+        msg = _COULD_NOT_CLAIM % login_url
+        logging.error(msg)
+        if notification_manager:
+            notification_manager.send(Notification(
+                success=False,
+                account_identifier=account_ident,
+                game_name=game_name,
+                message=msg,
+            ))
+        return
+
+    # since everything is good now, set total sign in days to the new value
+    total_sign_in_day = new_total_sign_in_day
 
     code = response.get("retcode", 99999)
 
     logging.debug(f"return code {code}")
 
     if code == RET_CODE_ALREADY_SIGNED_IN:
         logging.info("Already signed in for today...")
```

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/http.py` & `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/main.py` & `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/main.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/notifications.py` & `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/notifications.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/scheduler.py` & `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper/scheduler.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.5.2
+Version: 2.5.3
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.5.3/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/pyproject.toml` & `hoyo-daily-logins-helper-2.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.2/requirements.txt` & `hoyo-daily-logins-helper-2.5.3/requirements.txt`

 * *Files identical despite different names*

