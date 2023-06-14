# Comparing `tmp/rubpy-6.1.9.tar.gz` & `tmp/rubpy-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.1.9.tar", last modified: Sat Apr 29 21:28:28 2023, max compression
+gzip compressed data, was "rubpy-6.2.0.tar", last modified: Wed Jun 14 11:37:23 2023, max compression
```

## Comparing `rubpy-6.1.9.tar` & `rubpy-6.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.646915 rubpy-6.1.9/
--rw-rw-rw-   0        0        0     3378 2023-04-29 21:28:28.646915 rubpy-6.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.568778 rubpy-6.1.9/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-29 21:28:06.000000 rubpy-6.1.9/rubpy/__init__.py
--rw-rw-rw-   0        0        0    41309 2023-04-26 17:32:17.000000 rubpy-6.1.9/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.600051 rubpy-6.1.9/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.615675 rubpy-6.1.9/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.9/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.1.9/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25897 2023-04-29 21:27:16.000000 rubpy-6.1.9/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.1.9/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.631263 rubpy-6.1.9/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    11146 2023-04-28 17:39:40.000000 rubpy-6.1.9/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.646915 rubpy-6.1.9/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.646915 rubpy-6.1.9/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.9/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.600051 rubpy-6.1.9/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 21:28:28.646915 rubpy-6.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-29 21:27:46.000000 rubpy-6.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.610397 rubpy-6.2.0/
+-rw-rw-rw-   0        0        0     3378 2023-06-14 11:37:23.610397 rubpy-6.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.563148 rubpy-6.2.0/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-29 21:28:06.000000 rubpy-6.2.0/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    41736 2023-06-14 11:34:41.000000 rubpy-6.2.0/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.598394 rubpy-6.2.0/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.0/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.598394 rubpy-6.2.0/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.2.0/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.0/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25947 2023-06-14 10:41:25.000000 rubpy-6.2.0/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.0/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.598394 rubpy-6.2.0/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    11443 2023-06-14 11:33:50.000000 rubpy-6.2.0/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.610397 rubpy-6.2.0/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.0/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.610397 rubpy-6.2.0/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.0/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.0/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:37:23.598394 rubpy-6.2.0/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-06-14 11:37:23.000000 rubpy-6.2.0/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-06-14 11:37:23.000000 rubpy-6.2.0/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:37:23.000000 rubpy-6.2.0/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-14 11:37:23.000000 rubpy-6.2.0/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 11:37:23.000000 rubpy-6.2.0/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:37:23.610397 rubpy-6.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-06-14 11:37:01.000000 rubpy-6.2.0/setup.py
```

### Comparing `rubpy-6.1.9/PKG-INFO` & `rubpy-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.9
+Version: 6.2.0
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
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.9 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.0 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.9/README.md` & `rubpy-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/client.py` & `rubpy-6.2.0/rubpy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import os
 #import io
 import aiofiles
 #import asyncio
 import logging
 from .crypto import Crypto
 from .structs import Struct
+from Crypto.PublicKey import RSA
 from . import __name__ as logger_name
 from .network import Connection, Proxies
 from .gadgets import exceptions, methods, thumbnail
 from .sessions import StringSession, SQLiteSession
 
 
 class Client:
     configuire = {
         'package': 'web.rubika.ir',
         'platform': 'Web',
         'app_name': 'Main',
         'user_agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
                        'AppleWebKit/537.36 (KHTML, like Gecko)'
                        'Chrome/102.0.0.0 Safari/537.36'),
-        'api_version': '5',
-        'app_version': '4.2.0'
+        'api_version': '6',
+        'app_version': '4.3.3'
     }
 
     def __init__(self,
         session,
         proxy=None,
         logger=None,
         timeout=20,
@@ -90,21 +91,23 @@
 
     async def __call__(self, request: object):
         try:
             result = await self._connection.execute(request)
 
             # update session
             if result.__name__ == 'signIn' and result.status == 'OK':
+                result.auth = Crypto.decrypt_RSA_OAEP(self._private_key, result.auth)
                 self._key = Crypto.passphrase(result.auth)
                 self._auth = result.auth
                 self._session.insert(
                     auth=self._auth,
                     guid=result.user.user_guid,
                     user_agent=self._user_agent,
-                    phone_number=result.user.phone)
+                    phone_number=result.user.phone,
+                    private_key=self._private_key)
 
                 await self(
                     methods.authorisations.RegisterDevice(
                         self._user_agent,
                         lang_code=self._platform['lang_code'],
                         app_version=self._platform['app_version'])
                 )
@@ -125,15 +128,15 @@
     async def start(self, phone_number: str, *args, **kwargs):
         if not hasattr(self, '_connection'):
             await self.connect()
 
         try:
             self._logger.info('user info', extra={'data': await self.get_me()})
 
-        except exceptions.NotRegistrred:
+        except (exceptions.NotRegistrred, exceptions.InvalidInput):
             self._logger.debug('user not registered!')
             if phone_number is None:
                 phone_number = input('Phone Number: ')
                 is_phone_number_true = True
                 while is_phone_number_true:
                     if input(f'Is the {phone_number} correct[y or n] > ').lower() == 'y':
                         is_phone_number_true = False
@@ -158,35 +161,39 @@
                         methods.authorisations.SendCode(
                             phone_number=phone_number,
                             pass_key=pass_key, *args, **kwargs))
 
                     if result.status == 'OK':
                         break
 
+            public_key, self._private_key = Crypto.create_keys()
             while True:
                 phone_code = input('Code: ')
                 result = await self(
                     methods.authorisations.SignIn(
                         phone_code=phone_code,
                         phone_number=phone_number,
                         phone_code_hash=result.phone_code_hash,
+                        public_key=public_key,
                         *args, **kwargs))
 
                 if result.status == 'OK':
                     break
 
         return self
 
     async def connect(self):
         self._connection = Connection(client=self)
         information = self._session.information()
         self._logger.info(f'the session information was read {information}')
         if information:
             self._auth = information[1]
             self._guid = information[2]
+            self._private_key = RSA.import_key(information[-1].encode('utf-8'))
+            print(information)
             if isinstance(information[3], str):
                 self._user_agent = information[3]
 
         return self
 
     async def disconnect(self):
         try:
```

### Comparing `rubpy-6.1.9/rubpy/gadgets/classino.py` & `rubpy-6.2.0/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/gadgets/exceptions.py` & `rubpy-6.2.0/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/gadgets/grouping.py` & `rubpy-6.2.0/rubpy/gadgets/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,15 +620,16 @@
             }
         },
         "SignIn": {
             "tmp_session": True,
             "params": {
                 "phone_code": {"types": "str"},
                 "phone_number": {"types": "str", "func": "get_phone"},
-                "phone_code_hash": {"types": "str"}
+                "phone_code_hash": {"types": "str"},
+                "public_key": {"types": "str"},
             }
         },
         "SendCode": {
             "tmp_session": True,
             "params": {
                 "phone_number": {"types": "str", "func": "get_phone"},
                 "pass_key": {"types": ["str", "optional"], "default": None},
```

### Comparing `rubpy-6.1.9/rubpy/gadgets/methods.py` & `rubpy-6.2.0/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/gadgets/thumbnail.py` & `rubpy-6.2.0/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/network/connection.py` & `rubpy-6.2.0/rubpy/network/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,17 +149,23 @@
             request = {'data_enc': Crypto.encrypt(request, key=self._client._key)}
 
         request['tmp_session' if tmp_session else 'auth'] = self._client._auth
 
         if 'api_version' not in request:
             request['api_version'] = self._client.configuire['api_version']
 
+        if request['api_version'] == '6' and tmp_session == False:
+            request['auth'] = Crypto.decode_auth(request['auth'])
+            request['sign'] = Crypto.sign(self._client._private_key, request['data_enc'])
+
         if not method_urls[0].startswith('https://getdcmess'):
             method_urls = [method_urls[0]] * 3
 
+        print(request)
+
         for _ in range(self._client._request_retries):
             for url in method_urls:
                 try:
                     #async with self._connection.options(url) as result:
                     #    if result.status != 200:
                     #        continue
 
@@ -167,14 +173,15 @@
                         if result.status != 200:
                             continue
 
                         result = await result.json()
                         if result.get('data_enc'):
                             result = Crypto.decrypt(result['data_enc'],
                                                     key=self._client._key)
+                            print(result)
                         status = result['status']
                         status_det = result['status_det']
                         if status == 'OK' and status_det == 'OK':
                             result['data']['_client'] = self._client
                             return results(method, update=result['data'])
 
                         self._client._logger.warning(
```

### Comparing `rubpy-6.1.9/rubpy/network/proxies.py` & `rubpy-6.2.0/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/sessions/sqliteSession.py` & `rubpy-6.2.0/rubpy/sessions/sqliteSession.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,34 +24,34 @@
                 self.upgrade_database(version)
 
         else:
             cursor.execute(
                 'create table version (version integer primary key)')
             cursor.execute('insert into version values (?)', (rbs_version,))
             cursor.execute('create table session (phone text primary key'
-                           ', auth text, guid text, agent text)')
+                           ', auth text, guid text, agent text, private_key text)')
             self._connection.commit()
         cursor.close()
 
     def upgrade_database(self, version):
         pass
 
     def information(self):
         cursor = self._connection.cursor()
         cursor.execute('select * from session')
         result = cursor.fetchone()
         cursor.close()
         return result
 
-    def insert(self, phone_number, auth, guid, user_agent, *args, **kwargs):
+    def insert(self, phone_number, auth, guid, user_agent, private_key, *args, **kwargs):
         cursor = self._connection.cursor()
         cursor.execute(
-            'insert or replace into session (phone, auth, guid, agent)'
-            ' values (?, ?, ?, ?)',
-            (phone_number, auth, guid, user_agent)
+            'insert or replace into session (phone, auth, guid, agent, private_key)'
+            ' values (?, ?, ?, ?, ?)',
+            (phone_number, auth, guid, user_agent, private_key)
         )
         self._connection.commit()
         cursor.close()
 
     @classmethod
     def from_string(cls, session, file_name=None):
         info = session.information()
```

### Comparing `rubpy-6.1.9/rubpy/sessions/stringSession.py` & `rubpy-6.2.0/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/structs/handlers.py` & `rubpy-6.2.0/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/structs/models.py` & `rubpy-6.2.0/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/structs/results.py` & `rubpy-6.2.0/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy/structs/struct.py` & `rubpy-6.2.0/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/rubpy.egg-info/PKG-INFO` & `rubpy-6.2.0/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.9
+Version: 6.2.0
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
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.9 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.0 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.9/rubpy.egg-info/SOURCES.txt` & `rubpy-6.2.0/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.9/setup.py` & `rubpy-6.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.1.9',
+    version = '6.2.0',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

