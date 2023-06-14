# Comparing `tmp/specker-1.1.3.tar.gz` & `tmp/specker-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specker-1.1.3.tar", last modified: Wed Jun 14 05:29:01 2023, max compression
+gzip compressed data, was "specker-1.1.4.tar", last modified: Wed Jun 14 05:38:42 2023, max compression
```

## Comparing `specker-1.1.3.tar` & `specker-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.396848 specker-1.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-14 05:22:18.000000 specker-1.1.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.3/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.3/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.3/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-14 05:22:18.000000 specker-1.1.3/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.3/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.3/Makefile
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-14 05:29:01.392848 specker-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.3/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.3/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.3/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-14 05:28:53.000000 specker-1.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 05:29:01.396848 specker-1.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.384848 specker-1.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/src/specker/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.3/src/specker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3132 2023-06-09 19:33:40.000000 specker-1.1.3/src/specker/content.py
--rw-rw-rw-   0 root         (0) root         (0)     6085 2023-06-14 05:22:18.000000 specker-1.1.3/src/specker/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/src/specker/specs/
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-08 21:00:19.000000 specker-1.1.3/src/specker/specs/SPECFILES.md
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-08 21:00:19.000000 specker-1.1.3/src/specker/specs/specker.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/src/specker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:38:42.216833 specker-1.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-14 05:22:18.000000 specker-1.1.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.4/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.4/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:38:42.216833 specker-1.1.4/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.4/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-14 05:33:57.000000 specker-1.1.4/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.4/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.4/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-14 05:38:42.216833 specker-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.4/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.4/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.4/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-14 05:38:35.000000 specker-1.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 05:38:42.216833 specker-1.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:38:42.212833 specker-1.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:38:42.216833 specker-1.1.4/src/specker/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.4/src/specker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2023-06-09 19:33:40.000000 specker-1.1.4/src/specker/content.py
+-rw-rw-rw-   0 root         (0) root         (0)     6289 2023-06-14 05:33:57.000000 specker-1.1.4/src/specker/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:38:42.216833 specker-1.1.4/src/specker/specs/
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-08 21:00:19.000000 specker-1.1.4/src/specker/specs/SPECFILES.md
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-08 21:00:19.000000 specker-1.1.4/src/specker/specs/specker.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:38:42.216833 specker-1.1.4/src/specker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-14 05:38:42.000000 specker-1.1.4/src/specker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-14 05:38:42.000000 specker-1.1.4/src/specker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 05:38:42.000000 specker-1.1.4/src/specker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-14 05:38:42.000000 specker-1.1.4/src/specker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 05:38:42.000000 specker-1.1.4/src/specker.egg-info/top_level.txt
```

### Comparing `specker-1.1.3/.gitlab-ci.yml` & `specker-1.1.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/.pylintrc` & `specker-1.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/.vscode/extensions.json` & `specker-1.1.4/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/Doxyfile` & `specker-1.1.4/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "Specker JSON Specification Validator"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.1.3"
+PROJECT_NUMBER = "1.1.4"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `specker-1.1.3/LICENSE.md` & `specker-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/Makefile` & `specker-1.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/PKG-INFO` & `specker-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.3
+Version: 1.1.4
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `specker-1.1.3/README.md` & `specker-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/git-tags.sh` & `specker-1.1.4/git-tags.sh`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/icon.png` & `specker-1.1.4/icon.png`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/pyproject.toml` & `specker-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "specker"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "Specker JSON Specification Validator"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `specker-1.1.3/src/specker/__init__.py` & `specker-1.1.4/src/specker/__init__.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/src/specker/content.py` & `specker-1.1.4/src/specker/content.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/src/specker/loader.py` & `specker-1.1.4/src/specker/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,19 +23,23 @@
 class SpecLoader:
     """Spec Loader and Handler
     """
     _specs:dict[str,dict[str,SpecContent]]
     _output:list[str]
     logger:logging.Logger
 
-    def __init__(self,spec_root:Path) -> None:
+    def __init__(self,spec_root:Path,debug:bool = False) -> None:
         """Initializer
         @param Path \c spec_root Location where .spec files are located
+        @param bool \c debug Enable logging.DEBUG (logging.ERROR if False)
         """
         self.logger = logging.Logger("specker.loader.SpecLoader")
+        self.logger.setLevel(logging.ERROR)
+        if debug:
+            self.logger.setLevel(logging.DEBUG)
         self._specs = {}
 
         specs_raw:dict[str,typing.Any] = {}
         spec_name:str = ""
         spec:dict[str,typing.Any] = {}
 
         self._output:list[str] = [
```

### Comparing `specker-1.1.3/src/specker/specs/SPECFILES.md` & `specker-1.1.4/src/specker/specs/SPECFILES.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/src/specker/specs/specker.spec` & `specker-1.1.4/src/specker/specs/specker.spec`

 * *Files identical despite different names*

### Comparing `specker-1.1.3/src/specker.egg-info/PKG-INFO` & `specker-1.1.4/src/specker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.3
+Version: 1.1.4
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

