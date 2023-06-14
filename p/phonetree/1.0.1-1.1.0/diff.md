# Comparing `tmp/phonetree-1.0.1.tar.gz` & `tmp/phonetree-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonetree-1.0.1.tar", last modified: Mon Apr 24 16:00:36 2023, max compression
+gzip compressed data, was "phonetree-1.1.0.tar", last modified: Wed Jun 14 20:36:22 2023, max compression
```

## Comparing `phonetree-1.0.1.tar` & `phonetree-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-04-24 16:00:36.791201 phonetree-1.0.1/
--rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.0.1/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     4553 2023-04-24 16:00:36.791096 phonetree-1.0.1/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     3792 2023-04-24 15:53:50.000000 phonetree-1.0.1/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-04-24 16:00:36.790303 phonetree-1.0.1/phonetree/
--rw-r--r--   0 leandro    (501) staff       (20)       78 2023-04-24 15:52:47.000000 phonetree-1.0.1/phonetree/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     5361 2023-04-24 15:48:46.000000 phonetree-1.0.1/phonetree/phonetree.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-04-24 16:00:36.790954 phonetree-1.0.1/phonetree.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     4553 2023-04-24 16:00:36.000000 phonetree-1.0.1/phonetree.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      241 2023-04-24 16:00:36.000000 phonetree-1.0.1/phonetree.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-04-24 16:00:36.000000 phonetree-1.0.1/phonetree.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       18 2023-04-24 16:00:36.000000 phonetree-1.0.1/phonetree.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       10 2023-04-24 16:00:36.000000 phonetree-1.0.1/phonetree.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)      944 2023-04-24 16:00:06.000000 phonetree-1.0.1/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-04-24 16:00:36.791230 phonetree-1.0.1/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:36:22.486078 phonetree-1.1.0/
+-rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.1.0/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:36:22.485975 phonetree-1.1.0/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.1.0/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:36:22.485189 phonetree-1.1.0/phonetree/
+-rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.1.0/phonetree/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)    10274 2023-06-14 20:34:20.000000 phonetree-1.1.0/phonetree/phonetree.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:36:22.485842 phonetree-1.1.0/phonetree.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      241 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       18 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       10 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)      944 2023-06-14 20:34:08.000000 phonetree-1.1.0/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-14 20:36:22.486107 phonetree-1.1.0/setup.cfg
```

### Comparing `phonetree-1.0.1/LICENSE` & `phonetree-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phonetree-1.0.1/PKG-INFO` & `phonetree-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.0.1
+Version: 1.1.0
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -82,15 +82,19 @@
 
 To define a menu, simply use the `@phonetree.menu()` decorator on a function. The function should return a dictionary representing the new state of the menu. This state will be passed on to the next menu or action function call.
 
 To define an action within a menu, use the `@menu.action("Action Name")` decorator on a function. The function should also return a dictionary representing the new state of the menu.
 
 ### Handling User Input and Output
 
-Menu and action functions can take optional "ask" and "tell" callbacks. The "ask" function sends some text to the user and expects an answer, returning the answer as the response of the function call. The "tell" function just sends some text to the user and doesn't return anything back. Both functions are recognized by their names in the menu/action functions argument list.
+Menu and action functions can take optional "ask" and "tell" callbacks.
+
+The "ask" function sends some text to the user and expects an answer, returning the answer as the response of the function call. If the function returns `None`, the program execution is ended.
+
+The "tell" function just sends some text to the user and doesn't return anything back. Both functions are recognized by their names in the menu/action functions argument list.
 
 ### State Management
 
 Menu and action functions can also take a state variable, which can be called anything (except for "ask" and "tell"). This argument is optional, but if passed, should be the first argument of the function. This argument can receive a state of any type.
 
 The function should return the new state of the menu, which will determine what will be passed on as the state for the next menu/action function call. This state can be any object, including `None`, if the user doesn't need to keep any state.
```

### Comparing `phonetree-1.0.1/README.md` & `phonetree-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,19 @@
 
 To define a menu, simply use the `@phonetree.menu()` decorator on a function. The function should return a dictionary representing the new state of the menu. This state will be passed on to the next menu or action function call.
 
 To define an action within a menu, use the `@menu.action("Action Name")` decorator on a function. The function should also return a dictionary representing the new state of the menu.
 
 ### Handling User Input and Output
 
-Menu and action functions can take optional "ask" and "tell" callbacks. The "ask" function sends some text to the user and expects an answer, returning the answer as the response of the function call. The "tell" function just sends some text to the user and doesn't return anything back. Both functions are recognized by their names in the menu/action functions argument list.
+Menu and action functions can take optional "ask" and "tell" callbacks.
+
+The "ask" function sends some text to the user and expects an answer, returning the answer as the response of the function call. If the function returns `None`, the program execution is ended.
+
+The "tell" function just sends some text to the user and doesn't return anything back. Both functions are recognized by their names in the menu/action functions argument list.
 
 ### State Management
 
 Menu and action functions can also take a state variable, which can be called anything (except for "ask" and "tell"). This argument is optional, but if passed, should be the first argument of the function. This argument can receive a state of any type.
 
 The function should return the new state of the menu, which will determine what will be passed on as the state for the next menu/action function call. This state can be any object, including `None`, if the user doesn't need to keep any state.
```

### Comparing `phonetree-1.0.1/phonetree.egg-info/PKG-INFO` & `phonetree-1.1.0/phonetree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.0.1
+Version: 1.1.0
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -82,15 +82,19 @@
 
 To define a menu, simply use the `@phonetree.menu()` decorator on a function. The function should return a dictionary representing the new state of the menu. This state will be passed on to the next menu or action function call.
 
 To define an action within a menu, use the `@menu.action("Action Name")` decorator on a function. The function should also return a dictionary representing the new state of the menu.
 
 ### Handling User Input and Output
 
-Menu and action functions can take optional "ask" and "tell" callbacks. The "ask" function sends some text to the user and expects an answer, returning the answer as the response of the function call. The "tell" function just sends some text to the user and doesn't return anything back. Both functions are recognized by their names in the menu/action functions argument list.
+Menu and action functions can take optional "ask" and "tell" callbacks.
+
+The "ask" function sends some text to the user and expects an answer, returning the answer as the response of the function call. If the function returns `None`, the program execution is ended.
+
+The "tell" function just sends some text to the user and doesn't return anything back. Both functions are recognized by their names in the menu/action functions argument list.
 
 ### State Management
 
 Menu and action functions can also take a state variable, which can be called anything (except for "ask" and "tell"). This argument is optional, but if passed, should be the first argument of the function. This argument can receive a state of any type.
 
 The function should return the new state of the menu, which will determine what will be passed on as the state for the next menu/action function call. This state can be any object, including `None`, if the user doesn't need to keep any state.
```

### Comparing `phonetree-1.0.1/pyproject.toml` & `phonetree-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phonetree"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Leandro Lima", email="leandro@lls-software.com" },
 ]
 description = "A phone-tree like menu system for text-based interfaces"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

