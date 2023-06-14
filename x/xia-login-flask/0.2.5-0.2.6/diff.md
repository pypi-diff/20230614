# Comparing `tmp/xia_login_flask-0.2.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_login_flask-0.2.6-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 212717 bytes, number of entries: 7
--rw-r--r--  2.0 unx      109 b- defN 23-Jun-14 05:41 xia_login_flask/__init__.py
--rw-r--r--  2.0 unx   566784 b- defN 23-Jun-14 05:45 xia_login_flask/account.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-14 05:45 xia_login_flask-0.2.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      739 b- defN 23-Jun-14 05:45 xia_login_flask-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-14 05:45 xia_login_flask-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-14 05:45 xia_login_flask-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      612 b- defN 23-Jun-14 05:45 xia_login_flask-0.2.5.dist-info/RECORD
-7 files, 568510 bytes uncompressed, 211619 bytes compressed:  62.8%
+Zip file size: 171203 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-14 06:59 xia_login_flask/__init__.py
+-rw-r--r--  2.0 unx   488664 b- defN 23-Jun-14 06:59 xia_login_flask/account.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-14 06:59 xia_login_flask-0.2.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      702 b- defN 23-Jun-14 06:59 xia_login_flask-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-14 06:59 xia_login_flask-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-14 06:59 xia_login_flask-0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      616 b- defN 23-Jun-14 06:59 xia_login_flask-0.2.6.dist-info/RECORD
+7 files, 490366 bytes uncompressed, 170099 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_login_flask/__init__.py
 Comment: 
 
-Filename: xia_login_flask/account.cp39-win_amd64.pyd
+Filename: xia_login_flask/account.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_login_flask-0.2.5.dist-info/LICENSE.txt
+Filename: xia_login_flask-0.2.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.5.dist-info/METADATA
+Filename: xia_login_flask-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_login_flask-0.2.5.dist-info/WHEEL
+Filename: xia_login_flask-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_login_flask-0.2.5.dist-info/top_level.txt
+Filename: xia_login_flask-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.5.dist-info/RECORD
+Filename: xia_login_flask-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_login_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_login_flask.account import XiaLoginFlask
 
 __all__ = [
     "XiaLoginFlask",
 ]
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
```

## Comparing `xia_login_flask-0.2.5.dist-info/METADATA` & `xia_login_flask-0.2.6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-login-flask
-Version: 0.2.5
+Version: 0.2.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.2.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.2.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: Flask
 Requires-Dist: xia-token-flask
 Requires-Dist: xia-user
 Requires-Dist: xia-mail-sender
@@ -29,9 +27,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

