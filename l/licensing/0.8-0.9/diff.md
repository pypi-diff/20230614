# Comparing `tmp/licensing-0.8.tar.gz` & `tmp/licensing-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\licensing-0.8.tar", last modified: Thu Apr 11 09:15:00 2019, max compression
+gzip compressed data, was "dist\licensing-0.9.tar", last modified: Wed Apr 24 07:04:34 2019, max compression
```

## Comparing `licensing-0.8.tar` & `licensing-0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2019-04-11 09:15:00.000000 licensing-0.8/
-drwxrwxrwx   0        0        0        0 2019-04-11 09:15:00.000000 licensing-0.8/licensing/
--rw-rw-rw-   0        0        0     2107 2019-02-13 15:55:10.000000 licensing-0.8/licensing/internal.py
--rw-rw-rw-   0        0        0     5229 2019-04-11 09:12:35.000000 licensing-0.8/licensing/methods.py
--rw-rw-rw-   0        0        0     6272 2019-04-11 08:23:12.000000 licensing-0.8/licensing/models.py
--rw-rw-rw-   0        0        0        0 2019-01-25 08:25:37.000000 licensing-0.8/licensing/__init__.py
--rw-rw-rw-   0        0        0      761 2019-04-11 09:15:00.000000 licensing-0.8/PKG-INFO
--rw-rw-rw-   0        0        0       63 2019-01-25 08:39:00.000000 licensing-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1693 2019-04-11 09:12:35.000000 licensing-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2019-04-24 07:04:34.000000 licensing-0.9/
+drwxrwxrwx   0        0        0        0 2019-04-24 07:04:34.000000 licensing-0.9/licensing/
+-rw-rw-rw-   0        0        0     2107 2019-02-13 15:55:10.000000 licensing-0.9/licensing/internal.py
+-rw-rw-rw-   0        0        0     6487 2019-04-24 06:57:25.000000 licensing-0.9/licensing/methods.py
+-rw-rw-rw-   0        0        0     6272 2019-04-11 08:23:12.000000 licensing-0.9/licensing/models.py
+-rw-rw-rw-   0        0        0        0 2019-01-25 08:25:37.000000 licensing-0.9/licensing/__init__.py
+-rw-rw-rw-   0        0        0      761 2019-04-24 07:04:34.000000 licensing-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2019-01-25 08:39:00.000000 licensing-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1693 2019-04-24 06:59:50.000000 licensing-0.9/setup.py
```

### Comparing `licensing-0.8/licensing/internal.py` & `licensing-0.9/licensing/internal.py`

 * *Files identical despite different names*

### Comparing `licensing-0.8/licensing/methods.py` & `licensing-0.9/licensing/methods.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,14 +82,45 @@
         if jobj == None or jobj["result"] == "1":
             if jobj != None:
                 return (None, jobj["message"])
             else:
                return (None, "Could not contact the server.")
            
         return (jobj["key"], "")
+    
+    
+    def deactivate(token, product_id, key, machine_code, floating = False):
+        """
+        Calls the Deactivate method in Web API 3 and returns a tuple containing
+        (Success, Message). If an error occurs, Success will be False. If
+        everything went well, Sucess is true and no message will be returned.
+        
+        More docs: https://app.cryptolens.io/docs/api/v3/Deactivate
+        """
+        
+        response = ""
+        
+        try:
+            response = HelperMethods.send_request("key/deactivate", {"token":token,\
+                                                  "ProductId":product_id,\
+                                                  "Key" : key,\
+                                                  "Floating" : floating,\
+                                                  "MachineCode":machine_code})
+        except Exception:
+            return (False, "Could not contact the server.")
+        
+        jobj = json.loads(response)
+
+        if jobj == None or jobj["result"] == "1":
+            if jobj != None:
+                return (False, jobj["message"])
+            else:
+               return (False, "Could not contact the server.")
+           
+        return (True, "")
 
             
             
 class Helpers:
     
     def GetMachineCode():
```

### Comparing `licensing-0.8/licensing/models.py` & `licensing-0.9/licensing/models.py`

 * *Files identical despite different names*

### Comparing `licensing-0.8/PKG-INFO` & `licensing-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: licensing
-Version: 0.8
+Version: 0.9
 Summary: Client library for Cryptolens licensing Web API.
 Home-page: https://cryptolens.io
 Author: Cryptolens AB
 Author-email: support@cryptolens.io
 License: MIT
-Download-URL: https://github.com/Cryptolens/cryptolens-python/archive/v_08.tar.gz
+Download-URL: https://github.com/Cryptolens/cryptolens-python/archive/v_09.tar.gz
 Description: UNKNOWN
 Keywords: software licensing,licensing library,cryptolens
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensing-0.8/setup.py` & `licensing-0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'licensing',         # How you named your package folder (MyLib)
   packages = ['licensing'],   # Chose the same as "name"
-  version = '0.8',      # Start with a small number and increase it with every change you make
+  version = '0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Client library for Cryptolens licensing Web API.',   # Give a short description about your library
   author = 'Cryptolens AB',                   # Type in your name
   author_email = 'support@cryptolens.io',      # Type in your E-Mail
   url = 'https://cryptolens.io',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/Cryptolens/cryptolens-python/archive/v_08.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/Cryptolens/cryptolens-python/archive/v_09.tar.gz',    # I explain this later on
   keywords = ['software licensing', 'licensing library', 'cryptolens'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pycryptodome'
       ],
   classifiers=[
     #'Development Status :: 5 - Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

