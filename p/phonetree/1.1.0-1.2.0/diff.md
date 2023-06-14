# Comparing `tmp/phonetree-1.1.0.tar.gz` & `tmp/phonetree-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonetree-1.1.0.tar", last modified: Wed Jun 14 20:36:22 2023, max compression
+gzip compressed data, was "phonetree-1.2.0.tar", last modified: Wed Jun 14 20:54:03 2023, max compression
```

## Comparing `phonetree-1.1.0.tar` & `phonetree-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:36:22.486078 phonetree-1.1.0/
--rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.1.0/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:36:22.485975 phonetree-1.1.0/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.1.0/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:36:22.485189 phonetree-1.1.0/phonetree/
--rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.1.0/phonetree/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)    10274 2023-06-14 20:34:20.000000 phonetree-1.1.0/phonetree/phonetree.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:36:22.485842 phonetree-1.1.0/phonetree.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      241 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       18 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       10 2023-06-14 20:36:22.000000 phonetree-1.1.0/phonetree.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)      944 2023-06-14 20:34:08.000000 phonetree-1.1.0/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-14 20:36:22.486107 phonetree-1.1.0/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:54:03.595331 phonetree-1.2.0/
+-rw-r--r--   0 leandro    (501) staff       (20)     1105 2023-04-10 17:55:51.000000 phonetree-1.2.0/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:54:03.595229 phonetree-1.2.0/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     3858 2023-06-14 20:32:54.000000 phonetree-1.2.0/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:54:03.594396 phonetree-1.2.0/phonetree/
+-rw-r--r--   0 leandro    (501) staff       (20)       78 2023-06-14 20:34:15.000000 phonetree-1.2.0/phonetree/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)    11421 2023-06-14 20:52:31.000000 phonetree-1.2.0/phonetree/phonetree.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-14 20:54:03.595100 phonetree-1.2.0/phonetree.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     4619 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      241 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       18 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       10 2023-06-14 20:54:03.000000 phonetree-1.2.0/phonetree.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)      944 2023-06-14 20:53:34.000000 phonetree-1.2.0/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-14 20:54:03.595357 phonetree-1.2.0/setup.cfg
```

### Comparing `phonetree-1.1.0/LICENSE` & `phonetree-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phonetree-1.1.0/PKG-INFO` & `phonetree-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.1.0
+Version: 1.2.0
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.1.0/README.md` & `phonetree-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `phonetree-1.1.0/phonetree/phonetree.py` & `phonetree-1.2.0/phonetree/phonetree.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,35 +49,41 @@
         ...
 
 
 class Menu(NextProtocol):
     def __init__(
         self,
         parent: Menu | None = None,
+        include_exit: bool = False,
+        include_exit_on_submenus: bool = False,
     ) -> None:
         """
         Initialize method for the Menu class.
 
         :param parent: The parent menu object if any, defaults to None
+        :param include_exit: Whether to include an Exit option in the menu, defaults to False
+        :param include_exit_on_submenus: Whether to include an Exit option in submenus, defaults to False
         """
         self._items: list[tuple[str, Menu | Action]] = []
         self.parent: Menu | None = parent
+        self.include_exit: bool = include_exit
+        self.include_exit_on_submenus: bool = include_exit_on_submenus
         self.callback: NormalizedActionCallback | None = None
 
     @property
     def _items_list(self) -> Sequence[tuple[str, Menu | Action | None]]:
         """
-        Get the list of menu items including the parent menu or Exit option.
+        Get the list of menu items including the parent menu and / or Exit option.
 
         :return: A list containing tuples with menu item names and their corresponding Menu or Action objects
         """
         items: list[tuple[str, Menu | Action | None]] = list(self._items)
         if (parent := self.parent) is not None:
             items.append(("Return to previous menu", parent))
-        else:
+        if parent is None or self.include_exit:
             items.append(("Exit", None))
         return items
 
     @property
     def _menu(self) -> Iterator[str]:
         """
         Generator function for iterating over the menu item names with their numerical indices.
@@ -114,22 +120,39 @@
 
         :param callback: The callback function to be called when the menu is opened
         :return: The menu object itself for method chaining
         """
         self.callback = normalize_callback(callback) if callback is not None else None
         return self
 
-    def menu(self, name: str) -> Menu:
+    def menu(
+        self,
+        name: str,
+        include_exit: bool | None = None,
+        include_exit_on_submenus: bool | None = None,
+    ) -> Menu:
         """
         Add a submenu to the current menu.
 
         :param name: The name of the submenu
+        :param include_exit: Whether to include an Exit option in the submenu,
+            defaults to self.include_exit_on_submenus
+        :param include_exit_on_submenus: Whether to include an Exit option in submenus,
+            defaults to self.include_exit_on_submenus
         :return: The submenu object
         """
-        submenu = Menu(parent=self)
+        submenu = Menu(
+            parent=self,
+            include_exit=include_exit
+            if include_exit is not None
+            else self.include_exit_on_submenus,
+            include_exit_on_submenus=include_exit_on_submenus
+            if include_exit_on_submenus is not None
+            else self.include_exit_on_submenus,
+        )
         self._items.append((name, submenu))
         return submenu
 
     def action(
         self,
         name: str,
     ) -> Action:
```

### Comparing `phonetree-1.1.0/phonetree.egg-info/PKG-INFO` & `phonetree-1.2.0/phonetree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonetree
-Version: 1.1.0
+Version: 1.2.0
 Summary: A phone-tree like menu system for text-based interfaces
 Author-email: Leandro Lima <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/phonetree
 Project-URL: Bug Tracker, https://github.com/leandropls/phonetree/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `phonetree-1.1.0/pyproject.toml` & `phonetree-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phonetree"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Leandro Lima", email="leandro@lls-software.com" },
 ]
 description = "A phone-tree like menu system for text-based interfaces"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

