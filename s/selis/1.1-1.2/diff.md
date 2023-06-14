# Comparing `tmp/selis-1.1.tar.gz` & `tmp/selis-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.1.tar", last modified: Wed Jun 14 08:50:25 2023, max compression
+gzip compressed data, was "selis-1.2.tar", last modified: Wed Jun 14 09:00:40 2023, max compression
```

## Comparing `selis-1.1.tar` & `selis-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 08:50:25.924524 selis-1.1/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 08:50:25.924353 selis-1.1/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 08:50:25.922025 selis-1.1/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.1/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     5003 2023-06-14 08:49:48.000000 selis-1.1/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 08:50:25.923875 selis-1.1/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 08:50:25.924574 selis-1.1/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 08:50:14.000000 selis-1.1/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:00:40.757999 selis-1.2/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:00:40.757874 selis-1.2/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:00:40.756807 selis-1.2/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.2/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     5119 2023-06-14 08:59:57.000000 selis-1.2/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:00:40.757689 selis-1.2/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 09:00:40.758045 selis-1.2/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 09:00:21.000000 selis-1.2/setup.py
```

### Comparing `selis-1.1/selis/selis.py` & `selis-1.2/selis/selis.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,31 +72,34 @@
                     print(self.convert_color("[-] Connection is closed", style="FAIL"))
                     self.connection.close()
                     break
                 except:
                     sys.exit()
     
     def process_sending_message(self):
-        while self.is_running:
-            content = input()
-            if content == "/exit":
-                content = f"/exit {self.nickname}"
-                self.send_message(content)
-                self.exit_room()
-                break
-            elif content == "/ls":
-                self.send_message(content)
-            elif "/open-url" in content:
-                self.handle_admin_command(content)
-            elif "/close-sever" == content:
-                self.handle_admin_command(content)
+        try:
+            while self.is_running:
+                content = input()
+                if content == "/exit":
+                    content = f"/exit {self.nickname}"
+                    self.send_message(content)
+                    self.exit_room()
+                    break
+                elif content == "/ls":
+                    self.send_message(content)
+                elif "/open-url" in content:
+                    self.handle_admin_command(content)
+                elif "/close-sever" == content:
+                    self.handle_admin_command(content)
 
-            else:
-                content = self.convert_color(f"({self.nickname}): {content}", style="ENDC")
-                self.send_message(content)
+                else:
+                    content = self.convert_color(f"({self.nickname}): {content}", style="ENDC")
+                    self.send_message(content)
+        except:
+            sys.exit()
 
     def start(self):
         send_threading = threading.Thread(target=self.process_sending_message)
         send_threading.start()
 
         recieve_threading = threading.Thread(target=self.recieve_message)
         recieve_threading.start()
```

