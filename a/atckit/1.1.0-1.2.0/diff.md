# Comparing `tmp/atckit-1.1.0.tar.gz` & `tmp/atckit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atckit-1.1.0.tar", last modified: Tue Jun 13 08:44:23 2023, max compression
+gzip compressed data, was "atckit-1.2.0.tar", last modified: Wed Jun 14 06:07:41 2023, max compression
```

## Comparing `atckit-1.1.0.tar` & `atckit-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:44:23.694717 atckit-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-10 20:52:22.000000 atckit-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.1.0/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-13 08:38:32.000000 atckit-1.1.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-13 08:34:00.000000 atckit-1.1.0/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.1.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.1.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     2873 2023-06-13 08:44:23.694717 atckit-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-10 20:36:02.000000 atckit-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.1.0/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.1.0/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.1.0/icon.png
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-13 08:44:16.000000 atckit-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 08:44:23.694717 atckit-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:44:23.690717 atckit-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:44:23.694717 atckit-1.1.0/src/atckit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 08:43:28.000000 atckit-1.1.0/src/atckit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-06-10 20:40:43.000000 atckit-1.1.0/src/atckit/subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)     5538 2023-06-13 08:38:32.000000 atckit-1.1.0/src/atckit/utilfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:44:23.694717 atckit-1.1.0/src/atckit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2873 2023-06-13 08:44:23.000000 atckit-1.1.0/src/atckit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-13 08:44:23.000000 atckit-1.1.0/src/atckit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:44:23.000000 atckit-1.1.0/src/atckit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-13 08:44:23.000000 atckit-1.1.0/src/atckit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:07:41.776790 atckit-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-10 20:52:22.000000 atckit-1.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.2.0/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-13 08:38:32.000000 atckit-1.2.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-14 06:05:46.000000 atckit-1.2.0/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.2.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.2.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-06-14 06:07:41.776790 atckit-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-10 20:36:02.000000 atckit-1.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.2.0/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.2.0/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.2.0/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-14 06:07:35.000000 atckit-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 06:07:41.776790 atckit-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:07:41.772790 atckit-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:07:41.776790 atckit-1.2.0/src/atckit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 06:06:52.000000 atckit-1.2.0/src/atckit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-14 05:58:15.000000 atckit-1.2.0/src/atckit/subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)     6247 2023-06-14 05:58:15.000000 atckit-1.2.0/src/atckit/utilfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:07:41.776790 atckit-1.2.0/src/atckit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-06-14 06:07:41.000000 atckit-1.2.0/src/atckit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-14 06:07:41.000000 atckit-1.2.0/src/atckit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 06:07:41.000000 atckit-1.2.0/src/atckit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-14 06:07:41.000000 atckit-1.2.0/src/atckit.egg-info/top_level.txt
```

### Comparing `atckit-1.1.0/.gitlab-ci.yml` & `atckit-1.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `atckit-1.1.0/.pylintrc` & `atckit-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `atckit-1.1.0/Doxyfile` & `atckit-1.2.0/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "AccidentallyTheCable's Utility Kit"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.1.0"
+PROJECT_NUMBER = "1.2.0"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `atckit-1.1.0/LICENSE.md` & `atckit-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atckit-1.1.0/Makefile` & `atckit-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `atckit-1.1.0/PKG-INFO` & `atckit-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atckit
-Version: 1.1.0
+Version: 1.2.0
 Summary: AccidentallyTheCable's Utility Kit
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atckit-1.1.0/README.md` & `atckit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `atckit-1.1.0/git-tags.sh` & `atckit-1.2.0/git-tags.sh`

 * *Files identical despite different names*

### Comparing `atckit-1.1.0/icon.png` & `atckit-1.2.0/icon.png`

 * *Files identical despite different names*

### Comparing `atckit-1.1.0/pyproject.toml` & `atckit-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atckit"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "AccidentallyTheCable's Utility Kit"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `atckit-1.1.0/src/atckit/subscriber.py` & `atckit-1.2.0/src/atckit/subscriber.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import logging
-
 from typing import Callable
 import typing_extensions
 
 class FunctionSubscriber:
     """ Function subscriber
 
 
@@ -54,21 +52,19 @@
         self._functions = []
 
     def __iadd__(self,fn:Callable) -> typing_extensions.Self:
         """Inline Add. Subscribe Function
         @param method \c fn Method to Subscribe
         """
         if fn not in self._functions:
-            logging.debug(f"Adding Function {fn.__qualname__}")
             self._functions.append(fn)
         return self
 
     def __isub__(self,fn:Callable) -> typing_extensions.Self:
         """Inline Subtract. Unsubscribe Function
         @param method \c fn Method to Unsubscribe
         """
         if fn not in self._functions:
             return self
         i:int = self._functions.index(fn)
         self._functions.pop(i)
-        logging.debug(f"Removing Function {fn.__qualname__}")
         return self
```

### Comparing `atckit-1.1.0/src/atckit/utilfuncs.py` & `atckit-1.2.0/src/atckit/utilfuncs.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,32 @@
     """Utility Functions
     """
 
     shutdown:bool = False
     restart:bool = False
 
     @staticmethod
+    def create_object_logger(obj:object) -> logging.Logger:
+        """Create logging.Logger with Specified object Class Name
+        @param object \c obj Object to Create Logger for
+        @retval logging.Logger Logger Instance
+        """
+        classname:str = str(obj.__class__)
+        classname = re.sub(r'^\<class \'(.*)\'>',r'\1',classname)
+        return logging.getLogger(classname)
+
+    @staticmethod
+    def create_static_logger(classname:str) -> logging.Logger:
+        """Create logging.Logger with Specified Name
+        @param str \c classname Name of Logger to Create
+        @retval logging.Logger Logger Instance
+        """
+        return logging.getLogger(classname)
+
+    @staticmethod
     def scan_dir(target_path:Path,
                  callback:typing.Callable[[Path,dict[str,typing.Any]],None],
                  callback_data:dict[str,typing.Any],
                  exclude_dirs:typing.Optional[list[re.Pattern]] = None,
                  exclude_files:typing.Optional[list[re.Pattern]] = None,
                  include_files:typing.Optional[list[re.Pattern]] = None
                 ) -> None:
```

### Comparing `atckit-1.1.0/src/atckit.egg-info/PKG-INFO` & `atckit-1.2.0/src/atckit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atckit
-Version: 1.1.0
+Version: 1.2.0
 Summary: AccidentallyTheCable's Utility Kit
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

