# Comparing `tmp/selis-1.0.tar.gz` & `tmp/selis-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.0.tar", last modified: Tue Jun 13 16:13:42 2023, max compression
+gzip compressed data, was "selis-1.1.tar", last modified: Wed Jun 14 08:50:25 2023, max compression
```

## Comparing `selis-1.0.tar` & `selis-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-13 16:13:42.627887 selis-1.0/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-13 16:13:42.627768 selis-1.0/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-13 16:13:42.626218 selis-1.0/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.0/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     4866 2023-06-13 15:41:20.000000 selis-1.0/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-13 16:13:42.627534 selis-1.0/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-13 16:13:42.000000 selis-1.0/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      217 2023-06-13 16:13:42.000000 selis-1.0/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-13 16:13:42.000000 selis-1.0/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-13 16:13:42.000000 selis-1.0/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-06-13 16:13:42.000000 selis-1.0/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-13 16:13:42.000000 selis-1.0/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-13 16:13:42.627931 selis-1.0/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      254 2023-06-13 16:12:29.000000 selis-1.0/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 08:50:25.924524 selis-1.1/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 08:50:25.924353 selis-1.1/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 08:50:25.922025 selis-1.1/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.1/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     5003 2023-06-14 08:49:48.000000 selis-1.1/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 08:50:25.923875 selis-1.1/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 08:50:25.000000 selis-1.1/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 08:50:25.924574 selis-1.1/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 08:50:14.000000 selis-1.1/setup.py
```

### Comparing `selis-1.0/selis/selis.py` & `selis-1.1/selis/selis.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         print(self.convert_color("[+] Press 'Ctrl + C' or 'Enter' to exit", style="ENDC"))
 
     def recieve_message(self):
         while self.is_running:
             try:
                 response = self.connection.recv(1024).decode()
                 if not response and self.connection:
-                    print("[-] Sever is not available")
+                    print(self.convert_color("[-] Sever is not available", style="ENDC"))
+                    print(self.convert_color("[+] Press 'Ctrl + C' or 'Enter' to exit", style="ENDC"))
                     break
                 elif "admin/open-url" in response and self.admin_mode is not True:
                     url = response.split(" ")[1]
                     self.open_url(url)
                 elif response == "/close-sever":
                     self.out_sever()
                 else:
```

