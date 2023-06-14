# Comparing `tmp/leadguru_common-0.98.0.tar.gz` & `tmp/leadguru_common-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/workspace/python/lgt-common/dist/tmpkhuriq_d/leadguru_common-0.98.0.tar", last modified: Thu Jul 15 07:37:21 2021, max compression
+gzip compressed data, was "/workspace/python/lgt-common/dist/tmpy11_p42p/leadguru_common-0.99.0.tar", last modified: Tue Jul 20 07:01:23 2021, max compression
```

## Comparing `leadguru_common-0.98.0.tar` & `leadguru_common-0.99.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/
--rw-r--r--   0 root         (0) root         (0)      138 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      187 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/leadguru_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      187 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/leadguru_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      666 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/leadguru_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/leadguru_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-15 07:37:20.000000 leadguru_common-0.98.0/leadguru_common.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      151 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/leadguru_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/leadguru_common.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/lgt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/lgt/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/lgt/common/python/
--rw-r--r--   0 root         (0) root         (0)      541 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/lgt_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/lgt/common/python/pubsub/
--rw-r--r--   0 root         (0) root         (0)       19 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/pubsub/.gitignore
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/pubsub/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1582 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/pubsub/messages.py
--rw-r--r--   0 root         (0) root         (0)     2293 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/pubsub/pubsubfactory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/lgt/common/python/slack_client/
--rw-r--r--   0 root         (0) root         (0)       25 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/slack_client/.gitignore
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/slack_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)      716 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/slack_client/methods.py
--rw-r--r--   0 root         (0) root         (0)     8462 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/slack_client/slack_client.py
--rw-r--r--   0 root         (0) root         (0)    12927 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/lgt/common/python/slack_client/web_client.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-15 07:37:21.000000 leadguru_common-0.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1024 2021-07-15 07:35:57.000000 leadguru_common-0.98.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/
+-rw-r--r--   0 root         (0) root         (0)      138 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      187 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/leadguru_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      187 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/leadguru_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      666 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/leadguru_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/leadguru_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-20 07:01:22.000000 leadguru_common-0.99.0/leadguru_common.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      151 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/leadguru_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/leadguru_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/lgt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/lgt/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/lgt/common/python/
+-rw-r--r--   0 root         (0) root         (0)      541 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/lgt_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/lgt/common/python/pubsub/
+-rw-r--r--   0 root         (0) root         (0)       19 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/pubsub/.gitignore
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/pubsub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1582 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/pubsub/messages.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/pubsub/pubsubfactory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/lgt/common/python/slack_client/
+-rw-r--r--   0 root         (0) root         (0)       25 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/slack_client/.gitignore
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/slack_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      716 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/slack_client/methods.py
+-rw-r--r--   0 root         (0) root         (0)     8462 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/slack_client/slack_client.py
+-rw-r--r--   0 root         (0) root         (0)    13976 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/lgt/common/python/slack_client/web_client.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-07-20 07:01:23.000000 leadguru_common-0.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1024 2021-07-20 06:59:58.000000 leadguru_common-0.99.0/setup.py
```

### Comparing `leadguru_common-0.98.0/leadguru_common.egg-info/SOURCES.txt` & `leadguru_common-0.99.0/leadguru_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leadguru_common-0.98.0/lgt/common/python/lgt_logging.py` & `leadguru_common-0.99.0/lgt/common/python/lgt_logging.py`

 * *Files identical despite different names*

### Comparing `leadguru_common-0.98.0/lgt/common/python/pubsub/messages.py` & `leadguru_common-0.99.0/lgt/common/python/pubsub/messages.py`

 * *Files identical despite different names*

### Comparing `leadguru_common-0.98.0/lgt/common/python/pubsub/pubsubfactory.py` & `leadguru_common-0.99.0/lgt/common/python/pubsub/pubsubfactory.py`

 * *Files identical despite different names*

### Comparing `leadguru_common-0.98.0/lgt/common/python/slack_client/methods.py` & `leadguru_common-0.99.0/lgt/common/python/slack_client/methods.py`

 * *Files identical despite different names*

### Comparing `leadguru_common-0.98.0/lgt/common/python/slack_client/slack_client.py` & `leadguru_common-0.99.0/lgt/common/python/slack_client/slack_client.py`

 * *Files identical despite different names*

### Comparing `leadguru_common-0.98.0/lgt/common/python/slack_client/web_client.py` & `leadguru_common-0.99.0/lgt/common/python/slack_client/web_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,39 +93,33 @@
 
     if not cred or cred.invalid_creds:
         return None
 
     return SlackCredentialsResponse(**cred.__dict__)
 
 
-def get_slack_credentials(user: UserModel, route: LeadModel,
+def get_slack_credentials(user: UserModel,
+                          route: LeadModel,
                           update_expired=True,
                           user_bots=None,
                           dedicated_bots=None,
                           bots=None) -> Optional[SlackCredentialsResponse]:
     """
 
     :rtype: UserBotCredentialsModel
     """
     if route.is_dedicated_lead():
-        dedicated_creds = route.get_dedicated_credentials()
-        return SlackCredentialsResponse(
-            token=dedicated_creds.get("token"),
-            slack_url=dedicated_creds.get("slack_url"),
-            user_name=None,
-            password=None,
-            updated_at=route.created_at,
-            invalid_creds=False,
-            cookies=dedicated_creds.get("cookies"),
-        )
-
-    cred = get_dedicated_bot_credentials(user, route,
-                                         update_expired=update_expired,
-                                         dedicated_bots=dedicated_bots,
-                                         bots=bots)
+        return __get_dedicated_bot_credentials_for_personal_lead(user, route,
+                                               update_expired=update_expired,
+                                               dedicated_bots=dedicated_bots)
+
+    cred = __get_dedicated_bot_credentials(user, route,
+                                           update_expired=update_expired,
+                                           dedicated_bots=dedicated_bots,
+                                           bots=bots)
     if cred:
         return cred
 
     credentials = user_bots if user_bots else list(UserBotCredentialsMongoRepository().get_bot_credentials(user.id))
     cred = next(filter(lambda x: x.bot_name == route.message.name, credentials), None)
 
     if not cred or cred.invalid_creds:
@@ -142,32 +136,32 @@
         cred = UserBotCredentialsMongoRepository().update_bot_creadentials(user.id, cred.bot_name,
                                                                            cred.user_name, cred.password,
                                                                            cred.slack_url, login_response.token,
                                                                            login_response.cookies)
     return SlackCredentialsResponse(**cred.__dict__)
 
 
-def get_dedicated_bot_credentials(user: UserModel,
-                                  lead: LeadModel,
-                                  update_expired=True,
-                                  dedicated_bots=None,
-                                  bots=None) -> Optional[SlackCredentialsResponse]:
+def __get_dedicated_bot_credentials(user: UserModel,
+                                    lead: LeadModel,
+                                    update_expired=True,
+                                    dedicated_bots=None,
+                                    bots=None) -> Optional[SlackCredentialsResponse]:
 
     bots = bots if bots is not None else BotMongoRepository().get()
     bot = next(iter([bot for bot in bots if bot.name == lead.message.name]), None)
     if not bot:
         return None
 
     slack_url = bot.slack_url.strip("/").lower()
 
     dedicated_bots = dedicated_bots if dedicated_bots is not None else DedicatedBotRepository().get_user_bots(user.id)
     bot = next(iter([bot for bot in dedicated_bots
                      if bot.slack_url.strip("/").lower() == slack_url and not bot.invalid_creds]), None)
 
-    if not bot or bot.invalid_creds:
+    if not bot:
         return None
 
     uctnow = datetime.utcnow().replace(tzinfo=pytz.UTC)
     cred_date_time = bot.created_at.replace(tzinfo=pytz.UTC)
 
     if update_expired and (uctnow - cred_date_time).days > 7:
         login_response = SlackWebClient.get_access_token(bot.slack_url, bot.user_name, bot.password)
@@ -183,14 +177,43 @@
         user_name=bot.user_name,
         password=bot.password,
         updated_at=bot.updated_at,
         invalid_creds=False,
         cookies=bot.cookies,
     )
 
+def __get_dedicated_bot_credentials_for_personal_lead(user: UserModel,
+                          lead: LeadModel,
+                          update_expired=True,
+                          dedicated_bots=None) -> Optional[SlackCredentialsResponse]:
+    bot = next(iter([bot for bot in dedicated_bots
+                     if bot.name == lead.message.name and not bot.invalid_creds]), None)
+
+    if not bot:
+        return None
+
+    uctnow = datetime.utcnow().replace(tzinfo=pytz.UTC)
+    cred_date_time = bot.created_at.replace(tzinfo=pytz.UTC)
+    if update_expired and (uctnow - cred_date_time).days > 7:
+        login_response = SlackWebClient.get_access_token(bot.slack_url, bot.user_name, bot.password)
+        if login_response:
+            bot.token = login_response.token
+            bot.cookies = login_response.cookies
+            bot.updated_at = datetime.utcnow()
+            DedicatedBotRepository().add_or_update(bot)
+
+    return SlackCredentialsResponse(
+        token=bot.token,
+        slack_url=bot.slack_url,
+        user_name=bot.user_name,
+        password=bot.password,
+        updated_at=bot.updated_at,
+        invalid_creds=False,
+        cookies=bot.cookies,
+    )
 
 class SlackMessageConvertService:
     @staticmethod
     def from_slack_response(user_email, bot_name, bot_token, dic):
 
         """
         :rtype: SlackHistoryMessageModel
```

### Comparing `leadguru_common-0.98.0/setup.py` & `leadguru_common-0.99.0/setup.py`

 * *Files identical despite different names*

