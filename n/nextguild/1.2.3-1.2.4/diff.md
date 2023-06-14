# Comparing `tmp/nextguild-1.2.3.tar.gz` & `tmp/nextguild-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.2.3.tar", last modified: Sat Jun 10 22:58:01 2023, max compression
+gzip compressed data, was "nextguild-1.2.4.tar", last modified: Wed Jun 14 18:13:36 2023, max compression
```

## Comparing `nextguild-1.2.3.tar` & `nextguild-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:58:01.720759 nextguild-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 22:57:51.000000 nextguild-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:58:01.720759 nextguild-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-10 22:57:51.000000 nextguild-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:58:01.720759 nextguild-1.2.3/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26747 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    41054 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:58:01.720759 nextguild-1.2.3/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 22:57:51.000000 nextguild-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:58:01.720759 nextguild-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:13:36.422334 nextguild-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 18:13:21.000000 nextguild-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-14 18:13:36.422334 nextguild-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-14 18:13:21.000000 nextguild-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:13:36.418334 nextguild-1.2.4/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27868 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42351 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48087 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:13:36.422334 nextguild-1.2.4/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-14 18:13:21.000000 nextguild-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:13:36.422334 nextguild-1.2.4/setup.cfg
```

### Comparing `nextguild-1.2.3/LICENSE` & `nextguild-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.3/PKG-INFO` & `nextguild-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.3
+Version: 1.2.4
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.3/README.md` & `nextguild-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.3/nextguild/classes.py` & `nextguild-1.2.4/nextguild/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,17 @@
         self.is_mentionable = self._get_is_mentionable(event_data)
         self.permissions = self._get_permissions(event_data)
         self.colors = self._get_colors(event_data)
         self.icon = self._get_icon(event_data)
         self.position = self._get_position(event_data)
         self.is_base = self._get_is_base(event_data)
         self.bot_user_id = self._get_bot_user_id(event_data)
+        self.last_message_id = self._get_last_message_id(event_data)
+        self.bot_id = self._get_bot_id(event_data)
+        self.heartbeat_interval = self._get_heartbeat_interval(event_data)
 
     def _scenario(self, event_data, scenarios):
         data = ''
         for scenario in scenarios:
             if len(scenario) == 1:
                 data = event_data.get(scenario[0], '')
             if len(scenario) == 2:
@@ -139,14 +142,15 @@
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_user_id(self, event_data: dict):
         scenarios = [
             ('socialLink', 'userId'),
             ('calendarEventRsvp', 'userId'),
+            ('d', 'user', 'id'),
         ]
         return self._scenario(event_data, scenarios)
 
     def _get_server_id(self, event_data: dict):
         scenarios = [
             ('reaction', 'serverId'),
             ('serverId',),
@@ -201,14 +205,15 @@
             ('calendarEventRsvp', 'createdBy'),
             ('listItem', 'createdBy'),
             ('listItem', 'note', 'createdBy'),
             ('calendarEventComment', 'createdBy'),
             ('group', 'createdBy'),
             ('announcement', 'createdBy'),
             ('announcementComment', 'createdBy'),
+            ('d', 'user', 'createdBy')
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_deleted_by(self, event_data: dict):
         scenarios = [
             ('deletedBy',),
         ]
@@ -224,27 +229,29 @@
         scenarios = [
             ('server', 'type'),
             ('message', 'type'),
             ('member', 'user', 'type'),
             ('serverMemberBan', 'user', 'type'),
             ('channel', 'type'),
             ('socialLink', 'type'),
+            ('d', 'user', 'type'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_name(self, event_data: dict):
         scenarios = [
             ('server', 'name'),
             ('member', 'user', 'name'),
             ('serverMemberBan', 'user', 'name'),
             ('webhook', 'name'),
             ('calendarEvent', 'name'),
             ('reaction', 'emote', 'name'),
             ('group', 'name'),
             ('role', 'name'),
+            ('d', 'user', 'name')
         ]
         return self._scenario(event_data, scenarios)
             
     def _get_url(self, event_data: dict):
         scenarios = [
             ('server', 'url'),
             ('calendarEvent', 'url'),
@@ -261,21 +268,23 @@
     def _get_avatar(self, event_data: dict):
         scenarios = [
             ('server', 'avatar'),
             ('member', 'user', 'avatar'),
             ('serverMemberBan', 'user', 'avatar'),
             ('webhook', 'avatar'),
             ('group', 'avatar'),
+            ('d', 'user', 'avatar')
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_banner(self, event_data: dict):
         scenarios = [
             ('server', 'banner'),
-            ('member', 'user', 'banner')
+            ('member', 'user', 'banner'),
+            ('d', 'user', 'banner')
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_timezone(self, event_data: dict):
         scenarios = [
             ('server', 'timezone'),
         ]
@@ -311,14 +320,15 @@
             ('listItem', 'createdAt'),
             ('listItem', 'note', 'createdAt'),
             ('calendarEventComment', 'createdAt'),
             ('group', 'createdAt'),
             ('announcement', 'createdAt'),
             ('announcementComment', 'createdAt'),
             ('role', 'createdAt'),
+            ('d', 'user', 'createdAt')
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_updated_at(self, event_data: dict):
         scenarios = [
             ('message', 'updatedAt'),
             ('doc', 'updatedAt'),
@@ -397,14 +407,15 @@
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_status(self, event_data: dict):
         scenarios = [
             ('member', 'user', 'status', 'content'),
             ('calendarEventRsvp', 'status'),
+            ('d', 'user', 'status', 'content')
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_status_emote(self, event_data: dict):
         scenarios = [
             ('member', 'user', 'status', 'emoteId'),
         ]
@@ -694,20 +705,22 @@
             ('reaction', 'docId'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_emote_id(self, event_data: dict):
         scenarios = [
             ('group', 'emoteId'),
+            ('d', 'user', 'status', 'emoteId')
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_announcement_id(self, event_data: dict):
         scenarios = [
             ('reaction', 'announcementId'),
+            ('announcementComment', 'announcementId'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_is_displayed_separately(self, event_data: dict):
         scenarios = [
             ('role', 'isDisplayedSeparately'),
         ]
@@ -762,7 +775,25 @@
         return self._scenario(event_data, scenarios)
     
     def _get_bot_user_id(self, event_data: dict):
         scenarios = [
             ('role', 'botUserId'),
         ]
         return self._scenario(event_data, scenarios)
+    
+    def _get_last_message_id(self, event_data: dict):
+        scenarios = [
+            ('d', 'lastMessageId'),
+        ]
+        return self._scenario(event_data, scenarios)
+    
+    def _get_bot_id(self, event_data: dict):
+        scenarios = [
+            ('d', 'botId'),
+        ]
+        return self._scenario(event_data, scenarios)
+    
+    def _get_heartbeat_interval(self, event_data: dict):
+        scenarios = [
+            ('heartbeatInterval'),
+        ]
+        return self._scenario(event_data, scenarios)
```

### Comparing `nextguild-1.2.3/nextguild/client.py` & `nextguild-1.2.4/nextguild/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
+import asyncio
 import json
 import time
 from datetime import datetime
 
 import requests
 
-from .embed import Embed
 from .classes import Data
+from .embed import Embed
 
 
 class Client:
     def __init__(self, token: str) -> None:
         self.token = token
         self.headers = {
             'Authorization': f'Bearer {self.token}',
@@ -18,14 +19,43 @@
             'Content-type': 'application/json',
             'Accept': 'application/json'
         }
         self.base_url = 'https://www.guilded.gg/api/v1'
         self.cache = {}
         self._message_handlers = []
 
+        asyncio.run(self.check_rate_limit())
+
+    async def check_rate_limit(self):
+        while True:
+            try:
+                response = await self._send_request('GET', self.base_url)
+                if response.status == 429:
+                    retry_after = response.headers.get('Retry-After')
+                    if retry_after:
+                        retry_after = int(retry_after)
+                        print(f"Rate limited during initialization. Retrying after {retry_after} seconds...")
+                        await asyncio.sleep(retry_after)
+                    else:
+                        print("Rate limited during initialization. Retrying with exponential backoff...")
+                        await self._exponential_backoff()
+                    continue
+                break
+            except Exception as e:
+                print(f"Error occurred during initialization: {e}")
+                await asyncio.sleep(1)
+
+    async def _exponential_backoff(self):
+        retries = 0
+        while True:
+            delay = (2 ** retries)
+            print(f"Retrying in {delay} seconds...")
+            await asyncio.sleep(delay)
+            retries += 1
+
     def send_message(
             self,
             channel_id: str,
             content: str = None,
             *,
             embed: Embed = None,
             is_private: bool = False,
@@ -328,86 +358,86 @@
             user_id: str
     ):
         response = self.request(
             'POST',
             f'{self.base_url}/servers/{server_id}/bans/{user_id}'
         )
         return response
-    
+
     def create_role(
             self,
             server_id: str,
             name: str,
             is_displayed_separately: bool = False,
             is_self_assignable: bool = False,
             is_mentionable: bool = False,
             permissions: list[str] = [],
-            colors = []
+            colors=[]
     ):
         data = {
             'name': name,
             'isDisplayedSeparately': str(is_displayed_separately).lower(),
             'isSelfAssignable': str(is_self_assignable).lower(),
             'isMentionable': str(is_mentionable).lower(),
             'permissions': permissions,
             'colors': colors
-                }
+        }
         response = self.request(
             'POST',
             f'{self.base_url}/servers/{server_id}/roles',
             json=data
         )
         return response
-    
+
     def get_role(
             self,
             server_id: str,
             role_id: int
     ):
         response = self.request(
             'GET',
             f'{self.base_url}/servers/{server_id}/roles/{role_id}'
         )
         return response
-    
+
     def get_roles(
             self,
             server_id: str
     ):
         response = self.request(
             'GET',
             f'{self.base_url}/servers/{server_id}/roles'
         )
         return response
-    
+
     def update_role(
             self,
             server_id: str,
             role_id: int,
             name: str = None,
             is_displayed_separately: bool = False,
             is_self_assignable: bool = False,
             is_mentionable: bool = False,
             permissions: list[str] = [],
-            colors = []
+            colors=[]
     ):
         response = self.request(
             'PATCH',
             f'{self.base_url}/servers/{server_id}/roles/{role_id}',
             json={
                 'name': name,
                 'isDisplayedSeparately': str(is_displayed_separately).lower(),
                 'isSelfAssignable': str(is_self_assignable).lower(),
                 'isMentionable': str(is_mentionable).lower(),
                 'permissions': permissions,
                 'colors': colors
             }
         )
         return response
-    
+
     def delete_role(
             self,
             server_id: str,
             role_id: int
     ):
         response = self.request(
             'DELETE',
@@ -1444,53 +1474,50 @@
         try:
             print(r)
             response = r['server']['defaultChannelId']
         except:
             response = 'No default channel found'
         return response
 
-
     def create_group(self, server_id: str, name: str, description: str, emote_id: int, is_public: bool):
-        response = self.request('POST', f'{self.base_url}/servers/{server_id}/groups', json={'name': name, 'description': description, 'emoteId': emote_id, 'isPublic': is_public})
+        response = self.request('POST', f'{self.base_url}/servers/{server_id}/groups',
+                                json={'name': name, 'description': description, 'emoteId': emote_id,
+                                      'isPublic': is_public})
         return response
 
     def get_groups(self, server_id: str):
         response = self.request('GET', f'{self.base_url}/servers/{server_id}/groups')
         return response
 
-
     def get_group(self, server_id: str, group_id: str):
         response = self.request('GET', f'{self.base_url}/servers/{server_id}/groups/{group_id}')
         return response
 
     def update_group(self, server_id: str, group_id: str, name: str, description: str, emote_id: int, is_public: bool):
 
-        response = self.request('PATCH', f'{self.base_url}/servers/{server_id}/groups/{group_id}', json={'name': name, 'description': description, 'emoteId': emote_id, 'isPublic': is_public})
+        response = self.request('PATCH', f'{self.base_url}/servers/{server_id}/groups/{group_id}',
+                                json={'name': name, 'description': description, 'emoteId': emote_id,
+                                      'isPublic': is_public})
         return response
 
-
     def delete_group(self, server_id: str, group_id: str):
         response = self.request('DELETE', f'{self.base_url}/servers/{server_id}/groups/{group_id}')
         return response
 
-
-
     def update_status(self, content: str, emote_id: int, expires_at: str = None):
         json = {'content': content, 'emoteId': emote_id}
         if expires_at:
             json.update({'expiresAt': expires_at})
         response = self.request('PUT', f'{self.base_url}/users/@me/status', json=json)
         return response
 
-
     def delete_status(self):
         response = self.request('DELETE', f'{self.base_url}/users/@me/status')
         return response
 
-
     def member_has_role(self, server_id: str, user_id: str, role_id: int or list, type: str = 'any'):
         r = self.get_member_roles(server_id, user_id)
         if isinstance(role_id, list):
             if type == 'any':
                 for i in role_id:
                     if i in r:
                         return True
@@ -1507,11 +1534,7 @@
 
     def member_is_owner(self, server_id: str, user_id: str):
         r = self.get_server(server_id)
         if r['server']['ownerId'] == user_id:
             return True
         else:
             return False
-
-
-
-
```

### Comparing `nextguild-1.2.3/nextguild/embed.py` & `nextguild-1.2.4/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.3/nextguild/events.py` & `nextguild-1.2.4/nextguild/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import json
 from functools import wraps
-
+import time
 import websockets
 
 from .classes import Data
 
 
 class Events:
     def __init__(self, client):
@@ -27,15 +27,15 @@
         self._calendar_event_reaction_create_handlers = []
         self._calendar_event_reaction_delete_handlers = []
         self._channel_create_handlers = []
         self._channel_delete_handlers = []
         self._channel_update_handlers = []
         self._webhook_create_handlers = []
         self._webhook_delete_handlers = []
-        self._webhook_update_handlers = []   
+        self._webhook_update_handlers = []
         self._bot_server_join_handlers = []
         self._bot_server_leave_handlers = []
         self._member_update_handlers = []
         self._roles_update_handlers = []
         self._member_social_create_handlers = []
         self._member_social_update_handlers = []
         self._member_social_delete_handlers = []
@@ -97,15 +97,15 @@
         self._group_delete_handlers = []
         self._user_status_create_handlers = []
         self._user_status_delete_handlers = []
         self._role_create_handlers = []
         self._role_update_handlers = []
         self._role_delete_handlers = []
         self.client = client
-    
+
     def on_bot_membership_created(self, func):
         @wraps(func)
         def wrapper(server):
             return func(server)
 
         self._bot_server_join_handlers.append(wrapper)
         return wrapper
@@ -113,297 +113,271 @@
     def on_bot_membership_deleted(self, func):
         @wraps(func)
         def wrapper(server):
             return func(server)
 
         self._bot_server_leave_handlers.append(wrapper)
         return wrapper
-    
+
     def on_member_updated(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_roles_updated(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._roles_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_member_social_create(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_social_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_member_social_update(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_social_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_member_social_delete(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_social_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_delete(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._doc_deleted_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_update(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._doc_updated_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_create(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._doc_created_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_comment_create(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._doc_comment_created_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_comment_update(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._doc_comment_updated_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_comment_delete(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._doc_comment_deleted_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_delete_handlers.append(wrapper)
         return wrapper
-    
 
     def on_message(self, func):
         @wraps(func)
         def wrapper(message):
             return func(message)
 
         self._message_create_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_message_update(self, func):
         @wraps(func)
         def wrapper(message):
             return func(message)
 
         self._message_update_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_message_delete(self, func):
         @wraps(func)
         def wrapper(message):
             return func(message)
 
         self._message_delete_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_member_join(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_join_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_member_leave(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_leave_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_member_banned(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_banned_handlers.append(wrapper)
         return wrapper
 
-
     def on_member_unbanned(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_unbanned_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_ready(self, func):
         @wraps(func)
-        async def wrapper():
-            return await func()
+        async def wrapper(ready):
+            return await func(ready)
 
         self._ready_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_forum_topic_comment_reaction_create(self, func):
         @wraps(func)
         def wrapper(reaction):
             return func(reaction)
 
         self._forum_topic_comment_reaction_create_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_forum_topic_comment_reaction_delete(self, func):
         @wraps(func)
         def wrapper(reaction):
             return func(reaction)
 
         self._forum_topic_comment_reaction_delete_handlers.append(wrapper)
         return wrapper
 
-
     def on_calendar_event_reaction_create(self, func):
         @wraps(func)
         def wrapper(reaction):
             return func(reaction)
 
         self._calendar_event_reaction_create_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_calendar_event_reaction_delete(self, func):
         @wraps(func)
         def wrapper(reaction):
             return func(reaction)
 
         self._calendar_event_reaction_delete_handlers.append(wrapper)
         return wrapper
 
-
-
     def on_channel_create(self, func):
         @wraps(func)
         def wrapper(channel):
             return func(channel)
 
         self._channel_create_handlers.append(wrapper)
         return wrapper
 
-
     def on_channel_delete(self, func):
         @wraps(func)
         def wrapper(channel):
             return func(channel)
 
         self._channel_delete_handlers.append(wrapper)
         return wrapper
 
-
     def on_channel_update(self, func):
         @wraps(func)
         def wrapper(channel):
             return func(channel)
 
         self._channel_update_handlers.append(wrapper)
         return wrapper
 
-
     def on_webhook_create(self, func):
         @wraps(func)
         def wrapper(webhook):
             return func(webhook)
 
         self._webhook_create_handlers.append(wrapper)
         return wrapper
@@ -411,39 +385,39 @@
     def on_webhook_update(self, func):
         @wraps(func)
         def wrapper(webhook):
             return func(webhook)
 
         self._webhook_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_pin(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_pinned_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_unpin(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_unpinned_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_reaction_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_reaction_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_reaction_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_reaction_delete_handlers.append(wrapper)
         return wrapper
@@ -451,119 +425,119 @@
     def on_forum_topic_lock(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_lock_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_unlock(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_unlock_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_comment_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_comment_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_comment_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_comment_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_forum_topic_comment_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._forum_topic_comment_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_rsvp_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_rsvp_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_rsvp_many_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_rsvp_many_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_rsvp_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_rsvp_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_list_item_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._list_item_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_list_item_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._list_item_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_list_item_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._list_item_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_list_item_complete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._list_item_complete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_list_item_uncomplete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._list_item_uncomplete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_channel_message_reaction_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._channel_message_reaction_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_channel_message_reaction_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._channel_message_reaction_delete_handlers.append(wrapper)
         return wrapper
@@ -571,339 +545,337 @@
     def on_channel_message_reaction_many_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._channel_message_reaction_many_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_comment_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_comment_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_comment_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_comment_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_comment_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_comment_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_comment_reaction_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_comment_reaction_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_comment_reaction_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_comment_reaction_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_reaction_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._doc_reaction_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_reaction_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._doc_reaction_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_comment_reaction_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._doc_comment_reaction_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_doc_comment_reaction_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._doc_comment_reaction_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_series_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_series_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_calendar_event_series_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._calendar_event_series_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_reaction_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_reaction_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_reaction_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_reaction_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_comment_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_comment_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_comment_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_comment_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_comment_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_comment_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_comment_reaction_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_comment_reaction_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_announcement_comment_reaction_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_comment_reaction_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_group_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._group_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_group_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._group_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_group_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._group_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_user_status_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._user_status_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_user_status_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._user_status_delete_handlers.append(wrapper)
         return wrapper
-    
+
     def on_role_create(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._role_create_handlers.append(wrapper)
         return wrapper
-    
+
     def on_role_update(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._role_update_handlers.append(wrapper)
         return wrapper
-    
+
     def on_role_delete(self, func):
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._role_delete_handlers.append(wrapper)
         return wrapper
-    
-
 
     async def _handle_bot_server_membership_created(self, event_data):
         event = Data(event_data)
         for handler in self._bot_server_join_handlers:
             await handler(event)
-    
+
     async def _handle_bot_server_membership_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._bot_server_leave_handlers:
             await handler(event)
-        
+
     async def _handle_server_member_updated(self, event_data):
         event = Data(event_data)
         for handler in self._member_update_handlers:
             await handler(event)
 
     async def _handle_server_roles_updated(self, event_data):
         event = Data(event_data)
         for handler in self._roles_update_handlers:
             await handler(event)
 
     async def _handle_server_member_social_links_created(self, event_data):
         event = Data(event_data)
         for handler in self._member_social_create_handlers:
             await handler(event)
-    
+
     async def _handle_server_member_social_links_updated(self, event_data):
         event = Data(event_data)
         for handler in self._member_social_update_handlers:
             await handler(event)
-    
+
     async def _handle_server_member_social_links_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._member_social_delete_handlers:
             await handler(event)
 
     async def _handle_doc_created(self, event_data):
         event = Data(event_data)
         for handler in self._doc_create_handlers:
             await handler(event)
-    
+
     async def _handle_doc_updated(self, event_data):
         event = Data(event_data)
         for handler in self._doc_update_handlers:
             await handler(event)
-    
+
     async def _handle_doc_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._doc_delete_handlers:
             await handler(event)
 
     async def _handle_doc_comment_updated(self, event_data):
         event = Data(event_data)
         for handler in self._doc_comment_update_handlers:
             await handler(event)
-    
+
     async def _handle_doc_comment_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._doc_comment_delete_handlers:
             await handler(event)
-    
+
     async def _handle_doc_comment_created(self, event_data):
         event = Data(event_data)
         for handler in self._doc_comment_create_handlers:
             await handler(event)
-    
+
     async def _handle_calendar_event_created(self, event_data):
         event = Data(event_data)
         for handler in self._calendar_event_create_handlers:
             await handler(event)
-    
+
     async def _handle_calendar_event_updated(self, event_data):
         event = Data(event_data)
         for handler in self._calendar_event_update_handlers:
             await handler(event)
-    
+
     async def _handle_calendar_event_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._calendar_event_delete_handlers:
             await handler(event)
-    
+
     async def _handle_forum_topic_created(self, event_data):
         event = Data(event_data)
         for handler in self._forum_topic_create_handlers:
             await handler(event)
-    
+
     async def _handle_forum_topic_updated(self, event_data):
         event = Data(event_data)
         for handler in self._forum_topic_update_handlers:
             await handler(event)
-    
+
     async def _handle_forum_topic_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._forum_topic_delete_handlers:
             await handler(event)
 
     async def _handle_server_member_banned(self, event_data):
         event = Data(event_data)
@@ -941,17 +913,18 @@
             await handler(event)
 
     async def _handle_member_unbanned(self, event_data):
         event = Data(event_data)
         for handler in self._member_unbanned_handlers:
             await handler(event)
 
-    async def _handle_ready(self):
+    async def _handle_ready(self, event_data):
+        event = Data(event_data)
         for handler in self._ready_handlers:
-            await handler()
+            await handler(event)
 
     async def _handle_create_reaction(self, event_data):
         event = Data(event_data)
         for handler in self._reaction_create_handlers:
             await handler(event)
 
     async def _handle_delete_reaction(self, event_data):
@@ -984,20 +957,20 @@
         for handler in self._channel_create_handlers:
             await handler(event)
 
     async def _handle_delete_channel(self, event_data):
         event = Data(event_data)
         for handler in self._channel_delete_handlers:
             await handler(event)
-    
+
     async def _handle_update_channel(self, event_data):
         event = Data(event_data)
         for handler in self._channel_update_handlers:
             await handler(event)
-    
+
     async def _handle_create_webhook(self, event_data):
         event = Data(event_data)
         for handler in self._webhook_create_handlers:
             await handler(event)
 
     async def _handle_update_webhook(self, event_data):
         event = Data(event_data)
@@ -1039,25 +1012,25 @@
         for handler in self._forum_topic_comment_create_handlers:
             await handler(event)
 
     async def _handle_forum_topic_comment_updated(self, event_data):
         event = Data(event_data)
         for handler in self._forum_topic_comment_update_handlers:
             await handler(event)
-    
+
     async def _handle_forum_topic_comment_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._forum_topic_comment_delete_handlers:
             await handler(event)
 
     async def _handle_calendar_event_rsvp_updated(self, event_data):
         event = Data(event_data)
         for handler in self._calendar_event_rsvp_update_handlers:
             await handler(event)
-    
+
     async def _handle_calendar_event_rsvp_many_updated(self, event_data):
         event = Data(event_data)
         for handler in self._calendar_event_rsvp_many_update_handlers:
             await handler(event)
 
     async def _handle_calendar_event_rsvp_deleted(self, event_data):
         event = Data(event_data)
@@ -1099,15 +1072,15 @@
         for handler in self._channel_message_reaction_delete_handlers:
             await handler(event)
 
     async def _handle_channel_message_reaction_many_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._channel_message_reaction_many_delete_handlers:
             await handler(event)
-    
+
     async def _handle_calendar_event_comment_created(self, event_data):
         event = Data(event_data)
         for handler in self._calendar_event_comment_create_handlers:
             await handler(event)
 
     async def _handle_calendar_event_comment_updated(self, event_data):
         event = Data(event_data)
@@ -1139,15 +1112,15 @@
         for handler in self._doc_reaction_delete_handlers:
             await handler(event)
 
     async def _handle_doc_comment_reaction_created(self, event_data):
         event = Data(event_data)
         for handler in self._doc_comment_reaction_create_handlers:
             await handler(event)
-    
+
     async def _handle_doc_comment_reaction_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._doc_comment_reaction_delete_handlers:
             await handler(event)
 
     async def _handle_calendar_event_series_updated(self, event_data):
         event = Data(event_data)
@@ -1219,15 +1192,15 @@
         for handler in self._group_update_handlers:
             await handler(event)
 
     async def _handle_group_deleted(self, event_data):
         event = Data(event_data)
         for handler in self._group_delete_handlers:
             await handler(event)
-    
+
     async def _handle_user_status_created(self, event_data):
         event = Data(event_data)
         for handler in self._user_status_create_handlers:
             await handler(event)
 
     async def _handle_user_status_deleted(self, event_data):
         event = Data(event_data)
@@ -1252,15 +1225,17 @@
     async def start(self):
         async with websockets.connect(
                 'wss://www.guilded.gg/websocket/v1',
                 extra_headers={
                     'Authorization': f'Bearer {self.client.token}'
                 }
         ) as websocket:
-            await self._handle_ready()
+            response = await websocket.recv()
+            data = json.loads(response)
+            await self._handle_ready(data)
             while True:
                 data = await websocket.recv()
                 json_data = json.loads(data)
 
                 if 't' in json_data and 'd' in json_data:
                     event_type, event_data = json_data['t'], json_data['d']
                 else:
@@ -1350,19 +1325,27 @@
                     'GroupDeleted': self._handle_group_deleted,
                     'UserStatusCreated': self._handle_user_status_created,
                     'UserStatusDeleted': self._handle_user_status_deleted,
                     'RoleCreated': self._handle_role_created,
                     'RoleUpdated': self._handle_role_updated,
                     'RoleDeleted': self._handle_role_deleted,
 
-
                 }
                 handler = event_handlers.get(event_type)
                 if handler:
                     await handler(event_data)
 
+    async def on_disconnect(self):
+        while True:
+            try:
+                await self.start()
+                break
+            except Exception as e:
+                print(f"Reconnection failed: {e}")
+                time.sleep(10)
+
     def run(self):
         try:
-            asyncio.run(self.start())
+            asyncio.run(self.on_disconnect())
         except KeyboardInterrupt:
             # TODO Handle standard exit
             pass
```

### Comparing `nextguild-1.2.3/nextguild.egg-info/PKG-INFO` & `nextguild-1.2.4/nextguild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.3
+Version: 1.2.4
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.3/pyproject.toml` & `nextguild-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

