# Comparing `tmp/rubpy-6.2.1.tar.gz` & `tmp/rubpy-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.2.1.tar", last modified: Wed Jun 14 11:45:55 2023, max compression
+gzip compressed data, was "rubpy-6.2.2.tar", last modified: Wed Jun 14 19:18:24 2023, max compression
```

## Comparing `rubpy-6.2.1.tar` & `rubpy-6.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.812287 rubpy-6.2.1/
--rw-rw-rw-   0        0        0     3378 2023-06-14 11:45:55.812287 rubpy-6.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.765422 rubpy-6.2.1/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-29 21:28:06.000000 rubpy-6.2.1/rubpy/__init__.py
--rw-rw-rw-   0        0        0    41671 2023-06-14 11:43:24.000000 rubpy-6.2.1/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.796665 rubpy-6.2.1/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.1/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.796665 rubpy-6.2.1/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.2.1/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.1/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25947 2023-06-14 10:41:25.000000 rubpy-6.2.1/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.1/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.812287 rubpy-6.2.1/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    11374 2023-06-14 11:44:44.000000 rubpy-6.2.1/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.812287 rubpy-6.2.1/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.1/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.812287 rubpy-6.2.1/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.1/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.1/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:45:55.796665 rubpy-6.2.1/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-06-14 11:45:55.000000 rubpy-6.2.1/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-06-14 11:45:55.000000 rubpy-6.2.1/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:45:55.000000 rubpy-6.2.1/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-14 11:45:55.000000 rubpy-6.2.1/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 11:45:55.000000 rubpy-6.2.1/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 11:45:55.812287 rubpy-6.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-06-14 11:45:30.000000 rubpy-6.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/
+-rw-rw-rw-   0        0        0     3378 2023-06-14 19:18:24.262907 rubpy-6.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.236270 rubpy-6.2.2/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-06-14 19:18:12.000000 rubpy-6.2.2/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    42576 2023-06-14 18:57:48.000000 rubpy-6.2.2/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.247281 rubpy-6.2.2/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.2/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.2/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.2/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    26944 2023-06-14 18:58:42.000000 rubpy-6.2.2/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.2/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    11374 2023-06-14 11:44:44.000000 rubpy-6.2.2/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.2/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.2/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.247281 rubpy-6.2.2/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 19:18:24.262907 rubpy-6.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-06-14 19:18:00.000000 rubpy-6.2.2/setup.py
```

### Comparing `rubpy-6.2.1/PKG-INFO` & `rubpy-6.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.1
+Version: 6.2.2
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.1 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.2 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.1/README.md` & `rubpy-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/client.py` & `rubpy-6.2.2/rubpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,14 +313,32 @@
 
     async def get_object_by_username(self, username: str):
         return await self(methods.extras.GetObjectByUsername(username.replace('@', '')))
 
     async def get_link_from_app_url(self, app_url: str):
         return await self(methods.extras.GetLinkFromAppUrl(app_url))
 
+    async def create_voice_call(self, object_guid: str):
+        if object_guid.startswith('c'):
+            return await self(methods.channels.CreateChannelVoiceChat(object_guid))
+        elif object_guid.startswith('g'):
+            return await self(methods.groups.CreateGroupVoiceChat(object_guid))
+        else:
+            print('Invalid Object Guid')
+            return False
+
+    async def set_voice_chat_setting(self, object_guid: str, voice_chat_id: str, title: str = None):
+        if object_guid.startswith('c'):
+            return await self(methods.channels.SetChannelVoiceChatSetting(object_guid, voice_chat_id, title, ['title']))
+        elif object_guid.startswith('g'):
+            return await self(methods.groups.SetGroupVoiceChatSetting(object_guid, voice_chat_id, title, ['title']))
+        else:
+            print('Invalid Object Guid')
+            return False
+
 # ---------------- Groups Methods ----------------
 
     async def add_group(self, title: str, member_guids: list):
         return await self(methods.groups.AddGroup(title, member_guids))
 
     async def join_group(self, link: str):
         return await self(methods.groups.JoinGroup(link))
@@ -630,15 +648,15 @@
         if object_guid.lower() in ('me', 'self', 'cloud'):
             object_guid = self._guid
 
         if type(video) != bytes:
             async with aiofiles.open(video, 'rb') as file:
                 file_name = os.path.basename(video)
                 kwargs['file_name'] = kwargs.get('file_name', file_name)
-                file = await file.read()
+                video = await file.read()
                 await file.close()
         else:
             kwargs['file_name'] = kwargs.get('file_name', file_name)
 
         file_inline = await self.upload(video, *args, **kwargs)
         file_inline['type'] = 'Video'
```

### Comparing `rubpy-6.2.1/rubpy/crypto/crypto.py` & `rubpy-6.2.2/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/gadgets/classino.py` & `rubpy-6.2.2/rubpy/gadgets/classino.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                     f' "{name}", "{result}"? correct it')
 
         if result is not None or not exception:
             if result is None:
                 result = name
             return type(result, __base, {'__name__': result, **kwargs})
 
-        raise AttributeError(f'module has no attribute ({name})')
+        print(f'module has no attribute ({name})')
```

### Comparing `rubpy-6.2.1/rubpy/gadgets/exceptions.py` & `rubpy-6.2.2/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/gadgets/grouping.py` & `rubpy-6.2.2/rubpy/gadgets/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,28 @@
             }
         },
         "GetGroupAdminAccessList": {
             "params": {
                 "group_guid": {"types": "str"},
                 "member_guid": {"types": "str"}
             }
+        },
+        "CreateGroupVoiceChat": {
+            "params": {
+                "group_guid": {"types": "str"},
+            }
+        },
+        "SetGroupVoiceChatSetting": {
+            "updated_parameters": True,
+            "params": {
+                "group_guid": {"types": "str"},
+                "voice_chat_id": {"types": "str"},
+                "title": {"types": "str"},
+                "updated_parameters": {"types": ["list"], "alloweds": ["title"]}
+            }
         }
     },
     "messages": {
         "Values": [
             "Pin","Unpin", "Text", "Gif", "File", "Image", "Voice", "Music", "Video", "FileInline", "Quiz", "Regular", "FromMin", "FromMax", "Local", "Global"], 
         "SendMessage": {
             "params": {
@@ -458,14 +472,28 @@
             }
         },
         "GetChannelAdminAccessList": {
             "params": {
                 "channel_guid": {"types": "str"},
                 "member_guid": {"types": "str"}
             }
+        },
+        "CreateChannelVoiceChat": {
+            "params": {
+                "object_guid": {"types": "str"},
+            }
+        },
+        "SetChannelVoiceChatSetting": {
+            "updated_parameters": True,
+            "params": {
+                "channel_guid": {"types": "str"},
+                "voice_chat_id": {"types": "str"},
+                "title": {"types": "str"},
+                "updated_parameters": {"types": ["list"], "alloweds": ["title"]}
+            }
         }
     },
     "contacts": {
         "Values": [],
         "DeleteContact": {
             "params": {
                 "user_guid": {"types": "str"}
```

### Comparing `rubpy-6.2.1/rubpy/gadgets/methods.py` & `rubpy-6.2.2/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/gadgets/thumbnail.py` & `rubpy-6.2.2/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/network/connection.py` & `rubpy-6.2.2/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/network/proxies.py` & `rubpy-6.2.2/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/sessions/sqliteSession.py` & `rubpy-6.2.2/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/sessions/stringSession.py` & `rubpy-6.2.2/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/structs/handlers.py` & `rubpy-6.2.2/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/structs/models.py` & `rubpy-6.2.2/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/structs/results.py` & `rubpy-6.2.2/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy/structs/struct.py` & `rubpy-6.2.2/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/rubpy.egg-info/PKG-INFO` & `rubpy-6.2.2/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.1
+Version: 6.2.2
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.1 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.2 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.1/rubpy.egg-info/SOURCES.txt` & `rubpy-6.2.2/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.1/setup.py` & `rubpy-6.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.2.1',
+    version = '6.2.2',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

