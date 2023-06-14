# Comparing `tmp/argumento-1.0.4.tar.gz` & `tmp/argumento-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PyProjects\OK\config-args\dist\.tmp-i0s5itj7\argumento-1.0.4.tar", last modified: Tue Jun 13 18:25:38 2023, max compression
+gzip compressed data, was "D:\PyProjects\OK\config-args\dist\.tmp-q9gc4k9b\argumento-1.0.5.tar", last modified: Wed Jun 14 20:03:32 2023, max compression
```

## Comparing `argumento-1.0.4.tar` & `argumento-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-05-04 00:20:50.000000 argumento-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1438 2023-06-13 18:25:38.000000 argumento-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-07 09:04:28.000000 argumento-1.0.4/README.md
--rw-rw-rw-   0        0        0      813 2023-06-07 09:07:20.000000 argumento-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 18:25:38.000000 argumento-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento/
--rw-rw-rw-   0        0        0       84 2023-06-06 18:28:39.000000 argumento-1.0.4/src/argumento/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-13 18:23:59.000000 argumento-1.0.4/src/argumento/_version.py
--rw-rw-rw-   0        0        0     4860 2023-06-13 18:23:40.000000 argumento-1.0.4/src/argumento/parsers.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/
--rw-rw-rw-   0        0        0     1438 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 20:03:32.000000 argumento-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-04 00:20:50.000000 argumento-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1438 2023-06-14 20:03:32.000000 argumento-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-07 09:04:28.000000 argumento-1.0.5/README.md
+-rw-rw-rw-   0        0        0      813 2023-06-07 09:07:20.000000 argumento-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:03:32.000000 argumento-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 20:03:32.000000 argumento-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:03:32.000000 argumento-1.0.5/src/argumento/
+-rw-rw-rw-   0        0        0       84 2023-06-06 18:28:39.000000 argumento-1.0.5/src/argumento/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-14 18:19:56.000000 argumento-1.0.5/src/argumento/_version.py
+-rw-rw-rw-   0        0        0     1630 2023-06-14 17:37:46.000000 argumento-1.0.5/src/argumento/namespace_dict.py
+-rw-rw-rw-   0        0        0     4939 2023-06-14 17:59:58.000000 argumento-1.0.5/src/argumento/parsers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:03:32.000000 argumento-1.0.5/src/argumento.egg-info/
+-rw-rw-rw-   0        0        0     1438 2023-06-14 20:03:32.000000 argumento-1.0.5/src/argumento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-14 20:03:32.000000 argumento-1.0.5/src/argumento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:03:32.000000 argumento-1.0.5/src/argumento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-14 20:03:32.000000 argumento-1.0.5/src/argumento.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 20:03:32.000000 argumento-1.0.5/src/argumento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 20:03:32.000000 argumento-1.0.5/tests/
+-rw-rw-rw-   0        0        0     3365 2023-06-14 17:54:47.000000 argumento-1.0.5/tests/test_namespace_dict.py
```

### Comparing `argumento-1.0.4/LICENSE` & `argumento-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `argumento-1.0.4/PKG-INFO` & `argumento-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argumento
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package for combining config and command-line args
 Author-email: OK111 <oleg.khadartsev@gmail.com>
 Project-URL: Homepage, https://github.com/OlegKhadartsev/config-args
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `argumento-1.0.4/README.md` & `argumento-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `argumento-1.0.4/pyproject.toml` & `argumento-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argumento-1.0.4/src/argumento/parsers.py` & `argumento-1.0.5/src/argumento/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 import warnings
 
 import toml
 import yaml
 import builtins
 from argparse import Namespace
 
+from argumento.namespace_dict import NamespaceDict
+
 
 class ParserBase(ABC):
     def __init__(self, config_file: str):
         self._config_file = config_file
 
     @abstractmethod
     def _read_config(self):
         pass
 
-    def parse(self) -> Namespace:
+    def parse(self) -> NamespaceDict:
         cfg_file_dict = self._read_config()
         cmd_arg_parser = self._cmd_args_from_cfg_keys(cfg_file_dict)
         args, _ = cmd_arg_parser.parse_known_args()
-        return args
+        return NamespaceDict(vars(args))
 
     @classmethod
     def _cmd_args_from_cfg_keys(cls,
                                 cfg_file_dict: dict,
                                 parent_cfg_name: str = None,
                                 cmd_parser: argparse.ArgumentParser = None
                                 ) -> argparse.ArgumentParser:
```

### Comparing `argumento-1.0.4/src/argumento.egg-info/PKG-INFO` & `argumento-1.0.5/src/argumento.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argumento
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package for combining config and command-line args
 Author-email: OK111 <oleg.khadartsev@gmail.com>
 Project-URL: Homepage, https://github.com/OlegKhadartsev/config-args
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

