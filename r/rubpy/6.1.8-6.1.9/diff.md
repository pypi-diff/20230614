# Comparing `tmp/rubpy-6.1.8.tar.gz` & `tmp/rubpy-6.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.1.8.tar", last modified: Fri Apr 28 18:38:10 2023, max compression
+gzip compressed data, was "rubpy-6.1.9.tar", last modified: Sat Apr 29 21:28:28 2023, max compression
```

## Comparing `rubpy-6.1.8.tar` & `rubpy-6.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.205638 rubpy-6.1.8/
--rw-rw-rw-   0        0        0     3378 2023-04-28 18:38:10.205638 rubpy-6.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.127544 rubpy-6.1.8/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-28 18:36:18.000000 rubpy-6.1.8/rubpy/__init__.py
--rw-rw-rw-   0        0        0    41309 2023-04-26 17:32:17.000000 rubpy-6.1.8/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.158784 rubpy-6.1.8/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.174401 rubpy-6.1.8/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.8/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.1.8/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.8/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.1.8/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.190020 rubpy-6.1.8/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    11146 2023-04-28 17:39:40.000000 rubpy-6.1.8/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.190020 rubpy-6.1.8/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.205638 rubpy-6.1.8/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.8/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.158784 rubpy-6.1.8/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 18:38:10.205638 rubpy-6.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-28 18:33:31.000000 rubpy-6.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.646915 rubpy-6.1.9/
+-rw-rw-rw-   0        0        0     3378 2023-04-29 21:28:28.646915 rubpy-6.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.568778 rubpy-6.1.9/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-29 21:28:06.000000 rubpy-6.1.9/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    41309 2023-04-26 17:32:17.000000 rubpy-6.1.9/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.600051 rubpy-6.1.9/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.615675 rubpy-6.1.9/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.9/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.1.9/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25897 2023-04-29 21:27:16.000000 rubpy-6.1.9/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.1.9/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.631263 rubpy-6.1.9/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    11146 2023-04-28 17:39:40.000000 rubpy-6.1.9/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.646915 rubpy-6.1.9/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.646915 rubpy-6.1.9/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.9/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.9/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:28:28.600051 rubpy-6.1.9/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 21:28:28.000000 rubpy-6.1.9/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 21:28:28.646915 rubpy-6.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-29 21:27:46.000000 rubpy-6.1.9/setup.py
```

### Comparing `rubpy-6.1.8/PKG-INFO` & `rubpy-6.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.8
+Version: 6.1.9
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
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.8 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.9 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.8/README.md` & `rubpy-6.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/client.py` & `rubpy-6.1.9/rubpy/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/crypto/crypto.py` & `rubpy-6.1.9/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/gadgets/classino.py` & `rubpy-6.1.9/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/gadgets/exceptions.py` & `rubpy-6.1.9/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/gadgets/grouping.py` & `rubpy-6.1.9/rubpy/gadgets/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,15 +609,15 @@
             }
         }
 
     },
     "authorisations": {
         "Values": ["SMS", "Internal"],
         "GetDCs": {
-            "urls": ["https://getdcmess.iranlms.ir/"],
+            "urls": ["https://getdcmess.iranlms.ir/", "https://getdcmess1.iranlms.ir/", "https://getdcmess2.iranlms.ir/"],
             "encrypt": False,
             "params": {
                 "api_version": {"types": ["int", "str"], "func": "to_string", "default": "4"}
             }
         },
         "SignIn": {
             "tmp_session": True,
```

### Comparing `rubpy-6.1.8/rubpy/gadgets/methods.py` & `rubpy-6.1.9/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/gadgets/thumbnail.py` & `rubpy-6.1.9/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/network/connection.py` & `rubpy-6.1.9/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/network/proxies.py` & `rubpy-6.1.9/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/sessions/sqliteSession.py` & `rubpy-6.1.9/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/sessions/stringSession.py` & `rubpy-6.1.9/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/structs/handlers.py` & `rubpy-6.1.9/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/structs/models.py` & `rubpy-6.1.9/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/structs/results.py` & `rubpy-6.1.9/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy/structs/struct.py` & `rubpy-6.1.9/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/rubpy.egg-info/PKG-INFO` & `rubpy-6.1.9/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.8
+Version: 6.1.9
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
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.8 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.9 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.8/rubpy.egg-info/SOURCES.txt` & `rubpy-6.1.9/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.8/setup.py` & `rubpy-6.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.1.8',
+    version = '6.1.9',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

