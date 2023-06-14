# Comparing `tmp/nextguild-1.2.4.tar.gz` & `tmp/nextguild-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.2.4.tar", last modified: Wed Jun 14 18:13:36 2023, max compression
+gzip compressed data, was "nextguild-1.2.5.tar", last modified: Wed Jun 14 18:19:52 2023, max compression
```

## Comparing `nextguild-1.2.4.tar` & `nextguild-1.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:13:36.422334 nextguild-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 18:13:21.000000 nextguild-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-14 18:13:36.422334 nextguild-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-14 18:13:21.000000 nextguild-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:13:36.418334 nextguild-1.2.4/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27868 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    42351 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    48087 2023-06-14 18:13:21.000000 nextguild-1.2.4/nextguild/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:13:36.422334 nextguild-1.2.4/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 18:13:36.000000 nextguild-1.2.4/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-14 18:13:21.000000 nextguild-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:13:36.422334 nextguild-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:19:52.191491 nextguild-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 18:19:37.000000 nextguild-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-14 18:19:52.191491 nextguild-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-14 18:19:37.000000 nextguild-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:19:52.191491 nextguild-1.2.5/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 18:19:38.000000 nextguild-1.2.5/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27868 2023-06-14 18:19:38.000000 nextguild-1.2.5/nextguild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42346 2023-06-14 18:19:38.000000 nextguild-1.2.5/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-14 18:19:38.000000 nextguild-1.2.5/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48087 2023-06-14 18:19:38.000000 nextguild-1.2.5/nextguild/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:19:52.191491 nextguild-1.2.5/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-14 18:19:52.000000 nextguild-1.2.5/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 18:19:52.000000 nextguild-1.2.5/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:19:52.000000 nextguild-1.2.5/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 18:19:52.000000 nextguild-1.2.5/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-14 18:19:38.000000 nextguild-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:19:52.191491 nextguild-1.2.5/setup.cfg
```

### Comparing `nextguild-1.2.4/LICENSE` & `nextguild-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.4/PKG-INFO` & `nextguild-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.4
+Version: 1.2.5
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.4/README.md` & `nextguild-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.4/nextguild/classes.py` & `nextguild-1.2.5/nextguild/classes.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.4/nextguild/client.py` & `nextguild-1.2.5/nextguild/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,20 +19,20 @@
             'Content-type': 'application/json',
             'Accept': 'application/json'
         }
         self.base_url = 'https://www.guilded.gg/api/v1'
         self.cache = {}
         self._message_handlers = []
 
-        asyncio.run(self.check_rate_limit())
+        #asyncio.run(self.check_rate_limit())
 
     async def check_rate_limit(self):
         while True:
             try:
-                response = await self._send_request('GET', self.base_url)
+                response = await self.request('GET', self.base_url)
                 if response.status == 429:
                     retry_after = response.headers.get('Retry-After')
                     if retry_after:
                         retry_after = int(retry_after)
                         print(f"Rate limited during initialization. Retrying after {retry_after} seconds...")
                         await asyncio.sleep(retry_after)
                     else:
```

### Comparing `nextguild-1.2.4/nextguild/embed.py` & `nextguild-1.2.5/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.4/nextguild/events.py` & `nextguild-1.2.5/nextguild/events.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.4/nextguild.egg-info/PKG-INFO` & `nextguild-1.2.5/nextguild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.4
+Version: 1.2.5
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.4/pyproject.toml` & `nextguild-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

