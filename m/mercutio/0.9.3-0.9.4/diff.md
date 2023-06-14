# Comparing `tmp/mercutio-0.9.3.tar.gz` & `tmp/mercutio-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mercutio-0.9.3.tar", last modified: Thu Sep 17 21:29:00 2020, max compression
+gzip compressed data, was "dist/mercutio-0.9.4.tar", last modified: Thu Sep 17 22:34:43 2020, max compression
```

## Comparing `mercutio-0.9.3.tar` & `mercutio-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 21:29:00.060126 mercutio-0.9.3/
--rw-r--r--   0 sig       (1000) sig       (1000)       24 2020-09-05 20:46:04.000000 mercutio-0.9.3/MANIFEST.in
--rw-r--r--   0 sig       (1000) sig       (1000)     1427 2020-09-17 21:29:00.060126 mercutio-0.9.3/PKG-INFO
--rw-r--r--   0 sig       (1000) sig       (1000)      870 2020-09-06 18:41:02.000000 mercutio-0.9.3/README.md
--rw-r--r--   0 sig       (1000) sig       (1000)      214 2020-09-04 16:42:55.000000 mercutio-0.9.3/requirements.txt
--rw-r--r--   0 sig       (1000) sig       (1000)       38 2020-09-17 21:29:00.060126 mercutio-0.9.3/setup.cfg
--rw-r--r--   0 sig       (1000) sig       (1000)     1929 2020-09-13 22:59:24.000000 mercutio-0.9.3/setup.py
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 21:29:00.056792 mercutio-0.9.3/src/
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 21:29:00.056792 mercutio-0.9.3/src/mercutio/
--rw-r--r--   0 sig       (1000) sig       (1000)    18015 2020-09-17 21:15:10.000000 mercutio-0.9.3/src/mercutio/__init__.py
--rw-r--r--   0 sig       (1000) sig       (1000)      247 2020-09-13 22:33:35.000000 mercutio-0.9.3/src/mercutio/_metadata.py
--rw-r--r--   0 sig       (1000) sig       (1000)       21 2020-09-17 21:28:50.000000 mercutio-0.9.3/src/mercutio/_version.py
--rw-r--r--   0 sig       (1000) sig       (1000)     9661 2020-09-17 21:28:34.000000 mercutio-0.9.3/src/mercutio/defaults.py
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 21:29:00.056792 mercutio-0.9.3/src/mercutio.egg-info/
--rw-r--r--   0 sig       (1000) sig       (1000)     1427 2020-09-17 21:28:59.000000 mercutio-0.9.3/src/mercutio.egg-info/PKG-INFO
--rw-r--r--   0 sig       (1000) sig       (1000)      327 2020-09-17 21:28:59.000000 mercutio-0.9.3/src/mercutio.egg-info/SOURCES.txt
--rw-r--r--   0 sig       (1000) sig       (1000)        1 2020-09-17 21:28:59.000000 mercutio-0.9.3/src/mercutio.egg-info/dependency_links.txt
--rw-r--r--   0 sig       (1000) sig       (1000)      214 2020-09-17 21:28:59.000000 mercutio-0.9.3/src/mercutio.egg-info/requires.txt
--rw-r--r--   0 sig       (1000) sig       (1000)        9 2020-09-17 21:28:59.000000 mercutio-0.9.3/src/mercutio.egg-info/top_level.txt
+drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 22:34:43.368723 mercutio-0.9.4/
+-rw-r--r--   0 sig       (1000) sig       (1000)       24 2020-09-05 20:46:04.000000 mercutio-0.9.4/MANIFEST.in
+-rw-r--r--   0 sig       (1000) sig       (1000)     1427 2020-09-17 22:34:43.368723 mercutio-0.9.4/PKG-INFO
+-rw-r--r--   0 sig       (1000) sig       (1000)      870 2020-09-06 18:41:02.000000 mercutio-0.9.4/README.md
+-rw-r--r--   0 sig       (1000) sig       (1000)      214 2020-09-04 16:42:55.000000 mercutio-0.9.4/requirements.txt
+-rw-r--r--   0 sig       (1000) sig       (1000)       38 2020-09-17 22:34:43.368723 mercutio-0.9.4/setup.cfg
+-rw-r--r--   0 sig       (1000) sig       (1000)     1929 2020-09-13 22:59:24.000000 mercutio-0.9.4/setup.py
+drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 22:34:43.365390 mercutio-0.9.4/src/
+drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 22:34:43.365390 mercutio-0.9.4/src/mercutio/
+-rw-r--r--   0 sig       (1000) sig       (1000)    20520 2020-09-17 22:27:36.000000 mercutio-0.9.4/src/mercutio/__init__.py
+-rw-r--r--   0 sig       (1000) sig       (1000)      247 2020-09-13 22:33:35.000000 mercutio-0.9.4/src/mercutio/_metadata.py
+-rw-r--r--   0 sig       (1000) sig       (1000)       21 2020-09-17 21:29:33.000000 mercutio-0.9.4/src/mercutio/_version.py
+-rw-r--r--   0 sig       (1000) sig       (1000)     9661 2020-09-17 21:28:34.000000 mercutio-0.9.4/src/mercutio/defaults.py
+drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-09-17 22:34:43.368723 mercutio-0.9.4/src/mercutio.egg-info/
+-rw-r--r--   0 sig       (1000) sig       (1000)     1427 2020-09-17 22:34:43.000000 mercutio-0.9.4/src/mercutio.egg-info/PKG-INFO
+-rw-r--r--   0 sig       (1000) sig       (1000)      327 2020-09-17 22:34:43.000000 mercutio-0.9.4/src/mercutio.egg-info/SOURCES.txt
+-rw-r--r--   0 sig       (1000) sig       (1000)        1 2020-09-17 22:34:43.000000 mercutio-0.9.4/src/mercutio.egg-info/dependency_links.txt
+-rw-r--r--   0 sig       (1000) sig       (1000)      214 2020-09-17 22:34:43.000000 mercutio-0.9.4/src/mercutio.egg-info/requires.txt
+-rw-r--r--   0 sig       (1000) sig       (1000)        9 2020-09-17 22:34:43.000000 mercutio-0.9.4/src/mercutio.egg-info/top_level.txt
```

### Comparing `mercutio-0.9.3/PKG-INFO` & `mercutio-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercutio
-Version: 0.9.3
+Version: 0.9.4
 Summary: yet another character creation engine
 Home-page: https://github.com/signebedi/mercutio
 Author: Sig Janoska-Bedi
 Author-email: signe@siftingwinnowing.com
 License: MIT
 Description:
```

### Comparing `mercutio-0.9.3/README.md` & `mercutio-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `mercutio-0.9.3/setup.py` & `mercutio-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `mercutio-0.9.3/src/mercutio/__init__.py` & `mercutio-0.9.4/src/mercutio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -356,14 +356,78 @@
                                         try:
                                             self.armor[attribute] += item['proficiencies'][attribute]
                                         except Exception as e: print(e)
 
                     # print(f'\nSuccessfully added buff for the player {dimension} called {name}')
                     break
                 # print(f'\nUnable to find an appropriate for the player {dimension} called {name}')
+
+
+    def distribute(self, dimension=None):
+        break_var = 0
+        if dimension=='skills':
+            for key in self.skills:
+                while self.skills[key] > 1:
+                    test = rd.choice(self.skills_options)
+                    if self.skills[test] == 0:
+                        self.skills[test] += 1
+                        self.skills[key] -= 1
+                    else: break_var += 1
+                    
+                    if break_var == 100: break
+
+        if dimension=='armor':
+            for key in self.armor:
+                while self.armor[key] > 1:
+                    test = rd.choice(self.armor_options)
+                    if self.armor[test] == 0:
+                        self.armor[test] += 1
+                        self.armor[key] -= 1
+                    else: break_var += 1
+                    if break_var == 100: break
+
+        if dimension=='weapons':
+            for key in self.weapons:
+                while self.weapons[key] > 1:
+                    test = rd.choice(self.weapons_options)
+                    if self.weapons[test] == 0:
+                        self.weapons[test] += 1
+                        self.weapons[key] -= 1
+                    else: break_var += 1
+                    if break_var == 100: break
+
+        else: # if no argument is passed, then apply to all skill, weapon, and armor proficiencies
+            for key in self.skills:
+                while self.skills[key] > 1:
+                    test = rd.choice(self.skills_options)
+                    if self.skills[test] == 0:
+                        self.skills[test] += 1
+                        self.skills[key] -= 1
+                    else: break_var += 1
+                    
+                    if break_var == 100: break
+
+            for key in self.armor:
+                while self.armor[key] > 1:
+                    test = rd.choice(self.armor_options)
+                    if self.armor[test] == 0:
+                        self.armor[test] += 1
+                        self.armor[key] -= 1
+                    else: break_var += 1
+                    if break_var == 100: break
+
+            for key in self.weapons:
+                while self.weapons[key] > 1:
+                    test = rd.choice(self.weapons_options)
+                    if self.weapons[test] == 0:
+                        self.weapons[test] += 1
+                        self.weapons[key] -= 1
+                    else: break_var += 1
+                    if break_var == 100: break
+
 class Roll:
     def __init__(self):
         print('\nCreated a dice roller object')
     def four(self):
         return rd.randint(1,4)
     def six(self):
         return rd.randint(1,6)
```

### Comparing `mercutio-0.9.3/src/mercutio/defaults.py` & `mercutio-0.9.4/src/mercutio/defaults.py`

 * *Files identical despite different names*

### Comparing `mercutio-0.9.3/src/mercutio.egg-info/PKG-INFO` & `mercutio-0.9.4/src/mercutio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercutio
-Version: 0.9.3
+Version: 0.9.4
 Summary: yet another character creation engine
 Home-page: https://github.com/signebedi/mercutio
 Author: Sig Janoska-Bedi
 Author-email: signe@siftingwinnowing.com
 License: MIT
 Description:
```

