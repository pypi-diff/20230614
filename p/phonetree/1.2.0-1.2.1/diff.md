# Comparing `tmp/phonetree-1.2.0.tar.gz` & `tmp/phonetree-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonetree-1.2.0.tar", last modified: Wed Jun 14 20:54:03 2023, max compression
+gzip compressed data, was "phonetree-1.2.1.tar", last modified: Wed Jun 14 21:00:45 2023, max compression
```

## Comparing `phonetree-1.2.0.tar` & `phonetree-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:54:03.595331 phonetree-1.2.0/
--rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.2.0/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:54:03.595229 phonetree-1.2.0/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.2.0/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:54:03.594396 phonetree-1.2.0/phonetree/
--rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.2.0/phonetree/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)    11421 2023-06-14 20:52:31.000000 phonetree-1.2.0/phonetree/phonetree.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:54:03.595100 phonetree-1.2.0/phonetree.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      241 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       18 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       10 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)      944 2023-06-14 20:53:34.000000 phonetree-1.2.0/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-14 20:54:03.595357 phonetree-1.2.0/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 21:00:45.023933 phonetree-1.2.1/
+-rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.2.1/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 21:00:45.023830 phonetree-1.2.1/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.2.1/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 21:00:45.023015 phonetree-1.2.1/phonetree/
+-rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.2.1/phonetree/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)    11806 2023-06-14 20:59:32.000000 phonetree-1.2.1/phonetree/phonetree.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 21:00:45.023693 phonetree-1.2.1/phonetree.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      241 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       18 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       10 2023-06-14 21:00:45.000000 phonetree-1.2.1/phonetree.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)      944 2023-06-14 21:00:22.000000 phonetree-1.2.1/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-14 21:00:45.023961 phonetree-1.2.1/setup.cfg
```

### Comparing `phonetree-1.2.0/LICENSE` & `phonetree-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phonetree-1.2.0/PKG-INFO` & `phonetree-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.2.0
+Version: 1.2.1
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.2.0/README.md` & `phonetree-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `phonetree-1.2.0/phonetree/phonetree.py` & `phonetree-1.2.1/phonetree/phonetree.py`

 * *Files 6% similar despite different names*

```diff
@@ -208,16 +208,25 @@
         :param tell: The `tell` function for providing information to the user
         """
         current: Menu | Action | None = self
         while current is not None:
             current, state = current.next(state, ask, tell)
 
 
-def menu() -> Menu:
-    return Menu()
+def menu(
+    include_exit: bool = False,
+    include_exit_on_submenus: bool = False,
+) -> Menu:
+    """
+    Create a new menu.
+
+    :param include_exit: Whether to include an Exit option in the menu, defaults to False
+    :param include_exit_on_submenus: Whether to include an Exit option in submenus, defaults to False
+    """
+    return Menu(include_exit=include_exit, include_exit_on_submenus=include_exit_on_submenus)
 
 
 class Action(NextProtocol):
     def __init__(
         self,
         parent: Menu,
     ) -> None:
```

### Comparing `phonetree-1.2.0/phonetree.egg-info/PKG-INFO` & `phonetree-1.2.1/phonetree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.2.0
+Version: 1.2.1
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.2.0/pyproject.toml` & `phonetree-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phonetree"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Leandro Lima", email="leandro@lls-software.com" },
 ]
 description = "A phone-tree like menu system for text-based interfaces"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

