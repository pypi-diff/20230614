# Comparing `tmp/selis-1.3.tar.gz` & `tmp/selis-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.3.tar", last modified: Wed Jun 14 09:15:31 2023, max compression
+gzip compressed data, was "selis-1.5.tar", last modified: Wed Jun 14 09:20:27 2023, max compression
```

## Comparing `selis-1.3.tar` & `selis-1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:15:31.221945 selis-1.3/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:15:31.221849 selis-1.3/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:15:31.220773 selis-1.3/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.3/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     5132 2023-06-14 09:15:10.000000 selis-1.3/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:15:31.221691 selis-1.3/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 09:15:31.000000 selis-1.3/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 09:15:31.221980 selis-1.3/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 09:15:14.000000 selis-1.3/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:20:27.849025 selis-1.5/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:20:27.848650 selis-1.5/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:20:27.847362 selis-1.5/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.5/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4958 2023-06-14 09:20:15.000000 selis-1.5/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:20:27.848409 selis-1.5/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:20:27.000000 selis-1.5/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 09:20:27.000000 selis-1.5/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 09:20:27.000000 selis-1.5/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 09:20:27.000000 selis-1.5/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 09:20:27.000000 selis-1.5/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 09:20:27.000000 selis-1.5/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 09:20:27.849184 selis-1.5/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 09:20:07.000000 selis-1.5/setup.py
```

### Comparing `selis-1.3/selis/selis.py` & `selis-1.5/selis/selis.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,35 +107,32 @@
         send_threading.join()
         recieve_threading.join()
 
 def main():
     def return_error(parser, options):
         if not options.port:
             parser.error("[-] Port not found")
-        if not options.nickname:
-            parser.error("[-] Nickname not found")
 
     def return_arguments():
         parser = OptionParser()
         parser.add_option("-p", "--port", dest="port", help="Connect to sever through this port")
-        parser.add_option("-n", "--nickname", dest="nickname", help="Choose your name or a nickname")
         parser.add_option("-r", "--root", dest="root", help="Use root [on/off] to become the admin")
         (options, arguments) = parser.parse_args()
         return_error(parser, options)
         return options
 
     options = return_arguments()
 
     ip = "0.tcp.ap.ngrok.io"
     port = int(options.port)
-    nickname = options.nickname
+    nickname = input("[+] Choose a name: ")
 
     if options.root == "on":
         keypass = getpass.getpass("Password: ")
-        if keypass == "selis-1.3":
+        if keypass == "selis-1.5":
             print("[+] You're now the admin")
             admin_mode = True
         else:
             print("\033[91m[-] Password is wrong!")
             admin_mode = False
     else:
         admin_mode = False
```

