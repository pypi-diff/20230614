# Comparing `tmp/bcvcontext-0.1.7.tar.gz` & `tmp/bcvcontext-0.1.8.tar.gz`

## Comparing `bcvcontext-0.1.7.tar` & `bcvcontext-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/src/bcvContext/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/src/bcvContext/bcvContext.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/README.md
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.8/src/bcvContext/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 bcvcontext-0.1.8/src/bcvContext/bcvContext.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 bcvcontext-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.8/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.8/README.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.8/PKG-INFO
```

### Comparing `bcvcontext-0.1.7/src/bcvContext/bcvContext.py` & `bcvcontext-0.1.8/src/bcvContext/bcvContext.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 notarizationPath = ""
 isToCache = 1
 
 def init(_notarizationPath, _isToCache) :
     global notarizationPath, isToCache
     notarizationPath = _notarizationPath
-    isToCache = _isToCache
+    isToCache = int(_isToCache)
 
 def scriptContext(_filename) :
     return _filename
 
 def notarizationContextRawfile():
     return "../.." + notarizationPath + "/../rawFile.csv"
 
@@ -26,14 +26,20 @@
     return "../.." + notarizationPath + "/../../Day" + str(day) + "/Notarization" + str(lastNotarization) + "/" + _filename
 
 def finish(*args) :
     call(["rm", "-r","../__cache__"])
     if isToCache == 1 :
         call(["mkdir","../__cache__"])
         for i in args :
-            call(["mv",str(i),"../__cache__"])
+            try :
+                call(["mv",str(i),"../__cache__"])
+            except :
+                print("Warning : ", str(i), "not found")
         print("Final result at :", "../__cache__")
 
     else : 
         for i in args : 
-            call(["mv",str(i),"../.." + notarizationPath])
+            try : 
+                call(["mv",str(i),"../.." + notarizationPath])
+            except :
+                print("Warning : ", str(i), "not found")
         print("Final result at :", "../.." + notarizationPath)
```

### Comparing `bcvcontext-0.1.7/.gitignore` & `bcvcontext-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.7/LICENSE` & `bcvcontext-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.7/PKG-INFO` & `bcvcontext-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcvContext
-Version: 0.1.7
+Version: 0.1.8
 Summary: A small package to handle context path for the BCV generic workflow
 Author-email: CEA <thomas.marques@cea.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

