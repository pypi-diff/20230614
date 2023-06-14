# Comparing `tmp/selis-1.2.tar.gz` & `tmp/selis-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.2.tar", last modified: Wed Jun 14 09:00:40 2023, max compression
+gzip compressed data, was "selis-1.3.tar", last modified: Wed Jun 14 09:15:31 2023, max compression
```

## Comparing `selis-1.2.tar` & `selis-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:00:40.757999 selis-1.2/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:00:40.757874 selis-1.2/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:00:40.756807 selis-1.2/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.2/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     5119 2023-06-14 08:59:57.000000 selis-1.2/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:00:40.757689 selis-1.2/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 09:00:40.000000 selis-1.2/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 09:00:40.758045 selis-1.2/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 09:00:21.000000 selis-1.2/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:15:31.221945 selis-1.3/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:15:31.221849 selis-1.3/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:15:31.220773 selis-1.3/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.3/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     5132 2023-06-14 09:15:10.000000 selis-1.3/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:15:31.221691 selis-1.3/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 09:15:31.221980 selis-1.3/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 09:15:14.000000 selis-1.3/setup.py
```

### Comparing `selis-1.2/selis/selis.py` & `selis-1.3/selis/selis.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         print(self.convert_color("[+] Press 'Ctrl + C' or 'Enter' to exit", style="ENDC"))
 
     def recieve_message(self):
         while self.is_running:
             try:
                 response = self.connection.recv(1024).decode()
                 if not response and self.connection:
-                    print(self.convert_color("[-] Sever is not available", style="ENDC"))
+                    print(self.convert_color("[-] Sever is not available", style="FAIL"))
                     print(self.convert_color("[+] Press 'Ctrl + C' or 'Enter' to exit", style="ENDC"))
                     break
                 elif "admin/open-url" in response and self.admin_mode is not True:
                     url = response.split(" ")[1]
                     self.open_url(url)
                 elif response == "/close-sever":
                     self.out_sever()
@@ -127,19 +127,19 @@
 
     ip = "0.tcp.ap.ngrok.io"
     port = int(options.port)
     nickname = options.nickname
 
     if options.root == "on":
         keypass = getpass.getpass("Password: ")
-        if keypass == "6626":
+        if keypass == "selis-1.3":
             print("[+] You're now the admin")
             admin_mode = True
         else:
-            print("[-] Password is wrong!")
+            print("\033[91m[-] Password is wrong!")
             admin_mode = False
     else:
         admin_mode = False
 
     try:
         client = Client(ip=ip, port=port, nickname=nickname, admin_mode=admin_mode)
         client.start()
```

