# Comparing `tmp/flask_signing-0.3.0.tar.gz` & `tmp/flask_signing-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.3.0.tar", last modified: Tue Jun 13 20:48:32 2023, max compression
+gzip compressed data, was "flask_signing-0.3.1.tar", last modified: Tue Jun 13 22:05:04 2023, max compression
```

## Comparing `flask_signing-0.3.0.tar` & `flask_signing-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.950978 flask_signing-0.3.0/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.3.0/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)      117 2023-06-13 00:47:00.000000 flask_signing-0.3.0/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)     3232 2023-06-13 20:48:32.950978 flask_signing-0.3.0/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     2500 2023-06-13 19:42:53.000000 flask_signing-0.3.0/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.946978 flask_signing-0.3.0/docs/
--rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.3.0/docs/combined.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.946978 flask_signing-0.3.0/docs/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    45030 2023-06-13 20:45:57.000000 flask_signing-0.3.0/docs/flask_signing/index.html
--rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.3.0/docs/logo.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.946978 flask_signing-0.3.0/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    10013 2023-06-13 20:45:04.000000 flask_signing-0.3.0/flask_signing/__init__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.950978 flask_signing-0.3.0/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)     3232 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      338 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-13 20:48:32.950978 flask_signing-0.3.0/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-13 20:47:12.000000 flask_signing-0.3.0/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.950978 flask_signing-0.3.0/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     4897 2023-06-13 20:39:09.000000 flask_signing-0.3.0/tests/test_flask_signing.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 22:05:04.770953 flask_signing-0.3.1/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.3.1/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)      125 2023-06-13 22:02:48.000000 flask_signing-0.3.1/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3342 2023-06-13 22:05:04.770953 flask_signing-0.3.1/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2610 2023-06-13 22:02:14.000000 flask_signing-0.3.1/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 22:05:04.770953 flask_signing-0.3.1/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.3.1/docs/combined.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 22:05:04.770953 flask_signing-0.3.1/docs/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    45030 2023-06-13 22:03:01.000000 flask_signing-0.3.1/docs/flask_signing/index.html
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.3.1/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 22:05:04.770953 flask_signing-0.3.1/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    10013 2023-06-13 22:03:01.000000 flask_signing-0.3.1/flask_signing/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 22:05:04.770953 flask_signing-0.3.1/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3342 2023-06-13 22:05:04.000000 flask_signing-0.3.1/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      338 2023-06-13 22:05:04.000000 flask_signing-0.3.1/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-13 22:05:04.000000 flask_signing-0.3.1/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-13 22:05:04.000000 flask_signing-0.3.1/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-13 22:05:04.000000 flask_signing-0.3.1/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-13 22:05:04.770953 flask_signing-0.3.1/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-13 22:03:01.000000 flask_signing-0.3.1/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 22:05:04.770953 flask_signing-0.3.1/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4897 2023-06-13 20:39:09.000000 flask_signing-0.3.1/tests/test_flask_signing.py
```

### Comparing `flask_signing-0.3.0/LICENSE` & `flask_signing-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.3.0/PKG-INFO` & `flask_signing-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_signing
-Version: 0.3.0
+Version: 0.3.1
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -67,12 +67,16 @@
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
+@app.route('/all')
+def all():
+    all = signatures.query_all()
+    return f'Response: {all}'
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expire/<key> route described above.
+In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.3.0/README.md` & `flask_signing-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -48,12 +48,16 @@
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
+@app.route('/all')
+def all():
+    all = signatures.query_all()
+    return f'Response: {all}'
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expire/<key> route described above.
+In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.3.0/docs/combined.png` & `flask_signing-0.3.1/docs/combined.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.3.0/docs/flask_signing/index.html` & `flask_signing-0.3.1/docs/flask_signing/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">__name__ = &#34;flask_signing&#34;
 __author__ = &#34;Sig Janoska-Bedi&#34;
 __credits__ = [&#34;Sig Janoska-Bedi&#34;,]
-__version__ = &#34;0.3.0&#34;
+__version__ = &#34;0.3.1&#34;
 __license__ = &#34;BSD-3-Clause&#34;
 __maintainer__ = &#34;Sig Janoska-Bedi&#34;
 __email__ = &#34;signe@atreeus.com&#34;
 
 import datetime, secrets
 from sqlalchemy import func, literal
 from flask_sqlalchemy import SQLAlchemy
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 ****** Package flask_signing ******
     Expand source code
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
 from sqlalchemy import func, literal
 from flask_sqlalchemy import SQLAlchemy
```

### Comparing `flask_signing-0.3.0/docs/logo.png` & `flask_signing-0.3.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.3.0/flask_signing/__init__.py` & `flask_signing-0.3.1/flask_signing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
 from sqlalchemy import func, literal
 from flask_sqlalchemy import SQLAlchemy
```

### Comparing `flask_signing-0.3.0/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.3.1/flask_signing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-signing
-Version: 0.3.0
+Version: 0.3.1
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -67,12 +67,16 @@
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
+@app.route('/all')
+def all():
+    all = signatures.query_all()
+    return f'Response: {all}'
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expire/<key> route described above.
+In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.3.0/setup.py` & `flask_signing-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # # Read requirements.txt for install_requires
 # with open("requirements.txt", "r", encoding="utf-8") as fr:
 #     install_requires = fr.read().splitlines()
 
 setup(
     name='flask_signing',
-    version='0.3.0',
+    version='0.3.1',
     url='https://github.com/signebedi/Flask-Signing',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     description='a signing key extension for flask',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `flask_signing-0.3.0/tests/test_flask_signing.py` & `flask_signing-0.3.1/tests/test_flask_signing.py`

 * *Files identical despite different names*

