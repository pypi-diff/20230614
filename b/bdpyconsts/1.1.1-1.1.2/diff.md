# Comparing `tmp/bdpyconsts-1.1.1.tar.gz` & `tmp/bdpyconsts-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpyconsts-1.1.1.tar", last modified: Wed Jun 14 07:02:14 2023, max compression
+gzip compressed data, was "bdpyconsts-1.1.2.tar", last modified: Wed Jun 14 07:13:02 2023, max compression
```

## Comparing `bdpyconsts-1.1.1.tar` & `bdpyconsts-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:02:14.008551 bdpyconsts-1.1.1/
--rw-r--r--   0 zhicheng   (501) staff       (20)     1056 2023-06-14 07:02:14.008633 bdpyconsts-1.1.1/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      368 2023-06-14 06:56:56.000000 bdpyconsts-1.1.1/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpyconsts-1.1.1/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      812 2023-06-14 07:02:14.008914 bdpyconsts-1.1.1/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:02:14.006846 bdpyconsts-1.1.1/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:02:14.007563 bdpyconsts-1.1.1/src/bdpyconsts/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2022-09-04 10:23:26.000000 bdpyconsts-1.1.1/src/bdpyconsts/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     1438 2023-06-14 07:01:43.000000 bdpyconsts-1.1.1/src/bdpyconsts/bdpyconsts.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:02:14.008455 bdpyconsts-1.1.1/src/bdpyconsts.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     1056 2023-06-14 07:02:14.000000 bdpyconsts-1.1.1/src/bdpyconsts.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      242 2023-06-14 07:02:14.000000 bdpyconsts-1.1.1/src/bdpyconsts.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-14 07:02:14.000000 bdpyconsts-1.1.1/src/bdpyconsts.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)       11 2023-06-14 07:02:14.000000 bdpyconsts-1.1.1/src/bdpyconsts.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:13:02.978883 bdpyconsts-1.1.2/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1060 2023-06-14 07:13:02.978937 bdpyconsts-1.1.2/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      372 2023-06-14 07:12:30.000000 bdpyconsts-1.1.2/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpyconsts-1.1.2/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      812 2023-06-14 07:13:02.979186 bdpyconsts-1.1.2/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:13:02.977811 bdpyconsts-1.1.2/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:13:02.978351 bdpyconsts-1.1.2/src/bdpyconsts/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2022-09-04 10:23:26.000000 bdpyconsts-1.1.2/src/bdpyconsts/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1455 2023-06-14 07:12:29.000000 bdpyconsts-1.1.2/src/bdpyconsts/bdpyconsts.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-14 07:13:02.978793 bdpyconsts-1.1.2/src/bdpyconsts.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1060 2023-06-14 07:13:02.000000 bdpyconsts-1.1.2/src/bdpyconsts.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      242 2023-06-14 07:13:02.000000 bdpyconsts-1.1.2/src/bdpyconsts.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-14 07:13:02.000000 bdpyconsts-1.1.2/src/bdpyconsts.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)       11 2023-06-14 07:13:02.000000 bdpyconsts-1.1.2/src/bdpyconsts.egg-info/top_level.txt
```

### Comparing `bdpyconsts-1.1.1/PKG-INFO` & `bdpyconsts-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpyconsts
-Version: 1.1.1
+Version: 1.1.2
 Summary: Implement python constant configuration and reading
 Home-page: https://github.com/biandoucheng/bd-py-const
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-const/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpyconsts-example
 Classifier: Programming Language :: Python :: 3.5
@@ -27,10 +27,10 @@
 
     # one way
     consts.unlock()
     consts.ABCD = "abcd"
     consts.locked()
 
     # another way
-    if consts.lock:
+    if not consts.lock:
         onsts.ABCD = "abcd"
 ```
```

### Comparing `bdpyconsts-1.1.1/setup.cfg` & `bdpyconsts-1.1.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpyconsts
-version = 1.1.1
+version = 1.1.2
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Implement python constant configuration and reading
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-const
 project_urls =
```

### Comparing `bdpyconsts-1.1.1/src/bdpyconsts/bdpyconsts.py` & `bdpyconsts-1.1.2/src/bdpyconsts/bdpyconsts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 class ConstError(PermissionError):
     """
     Modify exception
     """
     pass
 
-class ConstFixedError(ConstError):
+class ConstChangedError(ConstError):
     """
     Case exception
     """
     pass
 
 class ConstCaseError(ConstError):
     """
@@ -46,15 +46,15 @@
     
 
     def __setattr__(self, name: str, value):
         """
         Constant setting
         """
         if name in self.__dict__ and self.lock:
-            raise ConstFixedError("Can't change const `%s`" % name)
+            raise ConstChangedError("Can't change the value of const `%s`" % name)
         
         if not name.isupper():
             raise ConstCaseError("Const name `%s` is not all uppercase" % name)
         
         self.__dict__[name] = value
```

### Comparing `bdpyconsts-1.1.1/src/bdpyconsts.egg-info/PKG-INFO` & `bdpyconsts-1.1.2/src/bdpyconsts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpyconsts
-Version: 1.1.1
+Version: 1.1.2
 Summary: Implement python constant configuration and reading
 Home-page: https://github.com/biandoucheng/bd-py-const
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-const/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpyconsts-example
 Classifier: Programming Language :: Python :: 3.5
@@ -27,10 +27,10 @@
 
     # one way
     consts.unlock()
     consts.ABCD = "abcd"
     consts.locked()
 
     # another way
-    if consts.lock:
+    if not consts.lock:
         onsts.ABCD = "abcd"
 ```
```

