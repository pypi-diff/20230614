# Comparing `tmp/specker-1.1.2.tar.gz` & `tmp/specker-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specker-1.1.2.tar", last modified: Sat Jun 10 20:42:51 2023, max compression
+gzip compressed data, was "specker-1.1.3.tar", last modified: Wed Jun 14 05:29:01 2023, max compression
```

## Comparing `specker-1.1.2.tar` & `specker-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.400125 specker-1.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-02 06:34:14.000000 specker-1.1.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.2/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.2/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.364125 specker-1.1.2/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.2/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-09 19:33:40.000000 specker-1.1.2/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.2/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-10 20:42:51.400125 specker-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.2/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.2/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.2/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-10 20:42:38.000000 specker-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 20:42:51.400125 specker-1.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.312125 specker-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.364125 specker-1.1.2/src/specker/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.2/src/specker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3132 2023-06-09 19:33:40.000000 specker-1.1.2/src/specker/content.py
--rw-rw-rw-   0 root         (0) root         (0)     5945 2023-06-02 06:24:00.000000 specker-1.1.2/src/specker/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.388125 specker-1.1.2/src/specker/specs/
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-08 21:00:19.000000 specker-1.1.2/src/specker/specs/SPECFILES.md
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-08 21:00:19.000000 specker-1.1.2/src/specker/specs/specker.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:42:51.368125 specker-1.1.2/src/specker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-10 20:42:51.000000 specker-1.1.2/src/specker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.396848 specker-1.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-14 05:22:18.000000 specker-1.1.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.3/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.3/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.3/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-14 05:22:18.000000 specker-1.1.3/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.3/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-14 05:29:01.392848 specker-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.3/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.3/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.3/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-14 05:28:53.000000 specker-1.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 05:29:01.396848 specker-1.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.384848 specker-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/src/specker/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.3/src/specker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2023-06-09 19:33:40.000000 specker-1.1.3/src/specker/content.py
+-rw-rw-rw-   0 root         (0) root         (0)     6085 2023-06-14 05:22:18.000000 specker-1.1.3/src/specker/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/src/specker/specs/
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-08 21:00:19.000000 specker-1.1.3/src/specker/specs/SPECFILES.md
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-08 21:00:19.000000 specker-1.1.3/src/specker/specs/specker.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:29:01.392848 specker-1.1.3/src/specker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 05:29:01.000000 specker-1.1.3/src/specker.egg-info/top_level.txt
```

### Comparing `specker-1.1.2/.gitlab-ci.yml` & `specker-1.1.3/.gitlab-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-image: debian:bullseye-slim
+image: python:3.9-slim-bullseye
 
 default:
   tags:
     - atc-runner
     - docker
 
 before_script:
   - apt update
-  - DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true apt -y install make python3 python3-pip python3-venv git curl jq
+  - DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true apt -y install make git curl jq
   - make install_build_deps
 
 stages:
   - lint
   - build
   - dist
```

### Comparing `specker-1.1.2/.pylintrc` & `specker-1.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/.vscode/extensions.json` & `specker-1.1.3/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/Doxyfile` & `specker-1.1.3/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "Specker JSON Specification Validator"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.1.2"
+PROJECT_NUMBER = "1.1.3"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `specker-1.1.2/LICENSE.md` & `specker-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/Makefile` & `specker-1.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/PKG-INFO` & `specker-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.2
+Version: 1.1.3
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `specker-1.1.2/README.md` & `specker-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/git-tags.sh` & `specker-1.1.3/git-tags.sh`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/icon.png` & `specker-1.1.3/icon.png`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/pyproject.toml` & `specker-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "specker"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "Specker JSON Specification Validator"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `specker-1.1.2/src/specker/__init__.py` & `specker-1.1.3/src/specker/__init__.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/src/specker/content.py` & `specker-1.1.3/src/specker/content.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/src/specker/loader.py` & `specker-1.1.3/src/specker/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,19 +21,21 @@
     from .content import SpecContent
 
 class SpecLoader:
     """Spec Loader and Handler
     """
     _specs:dict[str,dict[str,SpecContent]]
     _output:list[str]
+    logger:logging.Logger
 
     def __init__(self,spec_root:Path) -> None:
         """Initializer
         @param Path \c spec_root Location where .spec files are located
         """
+        self.logger = logging.Logger("specker.loader.SpecLoader")
         self._specs = {}
 
         specs_raw:dict[str,typing.Any] = {}
         spec_name:str = ""
         spec:dict[str,typing.Any] = {}
 
         self._output:list[str] = [
@@ -43,21 +45,21 @@
 
         # pylint: disable=unused-variable
         for root, subdirs, files in os.walk(spec_root.resolve().as_posix()):
             spec_path:Path = Path(root).resolve()
             for file in files:
                 if not file.endswith(".spec"):
                     continue
-                logging.debug(f"Loading: {file}")
+                self.logger.debug(f"Loading: {file}")
                 try:
                     with open(spec_path.joinpath(file), "r", encoding="utf-8") as f:
                         spec = json.loads(f.read())
                 except BaseException as e:
-                    logging.error(f"Failed loading: {file}, {e}")
-                    logging.debug(e,exc_info=True)
+                    self.logger.error(f"Failed loading: {file}, {e}")
+                    self.logger.debug(e,exc_info=True)
                     continue
                 spec_name = re.sub(r'\.spec',"",file)
                 specs_raw[spec_name] = spec
         for spec_file_name,spec_data in specs_raw.items():
             self._specs[spec_file_name] = {}
             for spec_name,spec in spec_data.items():
                 spec["name"] = spec_name
@@ -74,43 +76,43 @@
         spec_keys:list[str] = list(spec_file.keys())
         config_keys:list[str] = list(content.keys())
 
         spec_pass:bool = True
         for k in content.keys():
             if k not in spec_keys:
                 spec_pass = False
-                logging.error(f"{k}: fail, invalid option")
+                self.logger.error(f"{k}: fail, invalid option")
                 continue
         for k,spec in spec_file.items():
             if spec.get("name") not in config_keys and not spec.get("required"):
-                logging.debug(f"{k} was not defined, using default value")
+                self.logger.debug(f"{k} was not defined, using default value")
                 content[k] = spec.get("default")
             elif spec.get("name") not in config_keys and spec.get("required"):
                 spec_pass = False
-                logging.error(f"{k}: fail, missing required option")
+                self.logger.error(f"{k}: fail, missing required option")
                 continue
             if not spec.get("required") and content[k] is None:
-                logging.debug(f"{k}: pass, not required, but is empty")
+                self.logger.debug(f"{k}: pass, not required, but is empty")
                 continue
             if spec.type != type(content[k]) and spec.type != typing.Any:
                 spec_pass = False
-                logging.error(f"{k}: fail, must be {str(spec.type)}, got: {str(type(content[k]))}")
+                self.logger.error(f"{k}: fail, must be {str(spec.type)}, got: {str(type(content[k]))}")
             else:
-                logging.debug(f"{k}: pass, type match; need:{str(spec.type)}, got:{str(type(content[k]))}")
+                self.logger.debug(f"{k}: pass, type match; need:{str(spec.type)}, got:{str(type(content[k]))}")
             valid_values:list[typing.Any] = spec.get("values")
             if len(valid_values) > 0:
                 values:str = ""
                 for v in valid_values:
                     values += f",{str(v)}"
                 values = values.lstrip(",")
                 if content[k] not in valid_values:
                     spec_pass = False
-                    logging.error(f"{k}: fail, invalid value; must be one of: {values}")
+                    self.logger.error(f"{k}: fail, invalid value; must be one of: {values}")
                 else:
-                    logging.debug(f"{k}: pass, value match, need:{values}, got:{str(content[k])}")
+                    self.logger.debug(f"{k}: pass, value match, need:{values}, got:{str(content[k])}")
         return spec_pass
 
     def defaults(self,spec_file_name:str) -> dict[typing.Any,typing.Any]:
         """Get any Defined Defaults from a Spec
         @param str \c spec_file_name Spec File Name to pull
         @retval dict[Any,Any] Spec Defaults
         """
@@ -139,10 +141,10 @@
         for spec_file_name,spec_data in self._specs.items():
             self._output.append(f"## Spec for {spec_file_name}\n")
             for spec in spec_data.values():
                 self._output.append(str(spec))
 
         output_path:Path = output_file.resolve()
         output_file_str:str = output_path.as_posix()
-        logging.info(f"Writing to file {output_file_str}")
+        self.logger.info(f"Writing to file {output_file_str}")
         with open(output_path,"w", encoding="utf-8") as f:
             f.write("\n".join(self._output))
```

### Comparing `specker-1.1.2/src/specker/specs/SPECFILES.md` & `specker-1.1.3/src/specker/specs/SPECFILES.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/src/specker/specs/specker.spec` & `specker-1.1.3/src/specker/specs/specker.spec`

 * *Files identical despite different names*

### Comparing `specker-1.1.2/src/specker.egg-info/PKG-INFO` & `specker-1.1.3/src/specker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.2
+Version: 1.1.3
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

