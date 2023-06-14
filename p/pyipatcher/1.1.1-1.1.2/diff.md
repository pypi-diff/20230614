# Comparing `tmp/pyipatcher-1.1.1.tar.gz` & `tmp/pyipatcher-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyipatcher-1.1.1.tar", max compression
+gzip compressed data, was "pyipatcher-1.1.2.tar", max compression
```

## Comparing `pyipatcher-1.1.1.tar` & `pyipatcher-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-1.1.1/LICENSE
--rw-r--r--   0        0        0     1029 2023-06-07 13:50:28.051937 pyipatcher-1.1.1/README.md
--rw-r--r--   0        0        0      200 2023-06-10 09:58:56.044644 pyipatcher-1.1.1/pyipatcher/__init__.py
--rw-r--r--   0        0        0      346 2023-06-07 05:10:10.736779 pyipatcher-1.1.1/pyipatcher/__main__.py
--rw-r--r--   0        0        0     2740 2023-06-09 12:31:48.365994 pyipatcher-1.1.1/pyipatcher/cli/ibootpatcher.py
--rw-r--r--   0        0        0     2231 2023-06-09 12:31:43.011240 pyipatcher-1.1.1/pyipatcher/cli/kernelpatcher.py
--rw-r--r--   0        0        0     1529 2023-06-09 12:31:43.012870 pyipatcher-1.1.1/pyipatcher/cli/ramdiskpatcher.py
--rw-r--r--   0        0        0     4610 2023-06-10 13:51:26.219007 pyipatcher-1.1.1/pyipatcher/ipatcher.py
--rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-1.1.1/pyipatcher/logger.py
--rw-r--r--   0        0        0     1509 2023-06-10 13:49:18.286869 pyipatcher-1.1.1/pyipatcher/patchfinder/asrpatchfinder.py
--rw-r--r--   0        0        0    23722 2023-06-10 13:49:18.285024 pyipatcher-1.1.1/pyipatcher/patchfinder/ibootpatchfinder.py
--rw-r--r--   0        0        0     8738 2023-06-07 11:30:09.571267 pyipatcher-1.1.1/pyipatcher/patchfinder/insn.py
--rwxr-xr-x   0        0        0     5187 2023-06-10 13:49:18.294098 pyipatcher-1.1.1/pyipatcher/patchfinder/kernelpatchfinder.py
--rw-r--r--   0        0        0     5542 2023-06-07 03:32:51.657221 pyipatcher-1.1.1/pyipatcher/patchfinder/patchfinder64.py
--rw-r--r--   0        0        0     2084 2023-06-10 13:49:18.295150 pyipatcher-1.1.1/pyipatcher/patchfinder/rextpatchfinder.py
--rw-r--r--   0        0        0     1827 2023-06-10 12:50:47.362374 pyipatcher-1.1.1/pyipatcher/wikiproxy.py
--rw-r--r--   0        0        0      911 2023-06-10 14:07:25.255025 pyipatcher-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 pyipatcher-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1029 2023-06-10 14:08:14.786228 pyipatcher-1.1.2/README.md
+-rw-r--r--   0        0        0      200 2023-06-10 09:58:56.044644 pyipatcher-1.1.2/pyipatcher/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-07 05:10:10.736779 pyipatcher-1.1.2/pyipatcher/__main__.py
+-rw-r--r--   0        0        0     2740 2023-06-09 12:31:48.365994 pyipatcher-1.1.2/pyipatcher/cli/ibootpatcher.py
+-rw-r--r--   0        0        0     2231 2023-06-09 12:31:43.011240 pyipatcher-1.1.2/pyipatcher/cli/kernelpatcher.py
+-rw-r--r--   0        0        0     1529 2023-06-09 12:31:43.012870 pyipatcher-1.1.2/pyipatcher/cli/ramdiskpatcher.py
+-rw-r--r--   0        0        0     4610 2023-06-10 13:51:26.219007 pyipatcher-1.1.2/pyipatcher/ipatcher.py
+-rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-1.1.2/pyipatcher/logger.py
+-rw-r--r--   0        0        0     1509 2023-06-10 13:49:18.286869 pyipatcher-1.1.2/pyipatcher/patchfinder/asrpatchfinder.py
+-rw-r--r--   0        0        0    23722 2023-06-10 13:49:18.285024 pyipatcher-1.1.2/pyipatcher/patchfinder/ibootpatchfinder.py
+-rw-r--r--   0        0        0     8738 2023-06-07 11:30:09.571267 pyipatcher-1.1.2/pyipatcher/patchfinder/insn.py
+-rwxr-xr-x   0        0        0     5187 2023-06-10 13:49:18.294098 pyipatcher-1.1.2/pyipatcher/patchfinder/kernelpatchfinder.py
+-rw-r--r--   0        0        0     5542 2023-06-07 03:32:51.657221 pyipatcher-1.1.2/pyipatcher/patchfinder/patchfinder64.py
+-rw-r--r--   0        0        0     2084 2023-06-10 13:49:18.295150 pyipatcher-1.1.2/pyipatcher/patchfinder/rextpatchfinder.py
+-rw-r--r--   0        0        0     1827 2023-06-10 12:50:47.362374 pyipatcher-1.1.2/pyipatcher/wikiproxy.py
+-rw-r--r--   0        0        0      927 2023-06-14 04:11:57.814853 pyipatcher-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 pyipatcher-1.1.2/PKG-INFO
```

### Comparing `pyipatcher-1.1.1/LICENSE` & `pyipatcher-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/README.md` & `pyipatcher-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 git clone https://github.com/Mini-Exploit/pyipatcher
 cd pyipatcher
 ./install.sh
 ```
 ## Usage
 ```
 $ pyipatcher
-pyipatcher version: 1.1.0
+pyipatcher version: 1.1.1
 Usage: pyipatcher [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -h, --help  Show this message and exit.
 
 Commands:
   ibootpatcher
```

### Comparing `pyipatcher-1.1.1/pyipatcher/cli/ibootpatcher.py` & `pyipatcher-1.1.2/pyipatcher/cli/ibootpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/cli/kernelpatcher.py` & `pyipatcher-1.1.2/pyipatcher/cli/kernelpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/cli/ramdiskpatcher.py` & `pyipatcher-1.1.2/pyipatcher/cli/ramdiskpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/ipatcher.py` & `pyipatcher-1.1.2/pyipatcher/ipatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/logger.py` & `pyipatcher-1.1.2/pyipatcher/logger.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/patchfinder/asrpatchfinder.py` & `pyipatcher-1.1.2/pyipatcher/patchfinder/asrpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/patchfinder/ibootpatchfinder.py` & `pyipatcher-1.1.2/pyipatcher/patchfinder/ibootpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/patchfinder/insn.py` & `pyipatcher-1.1.2/pyipatcher/patchfinder/insn.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/patchfinder/kernelpatchfinder.py` & `pyipatcher-1.1.2/pyipatcher/patchfinder/kernelpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/patchfinder/patchfinder64.py` & `pyipatcher-1.1.2/pyipatcher/patchfinder/patchfinder64.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/patchfinder/rextpatchfinder.py` & `pyipatcher-1.1.2/pyipatcher/patchfinder/rextpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyipatcher/wikiproxy.py` & `pyipatcher-1.1.2/pyipatcher/wikiproxy.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.1.1/pyproject.toml` & `pyipatcher-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "pyipatcher"
-version = "1.1.1"
+version = "1.1.2"
 description = "iOS ARM64 patchfinder & iOS ARM64 bootchain patcher"
 authors = ["mini_exploit <61931266+Mini-Exploit@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/Mini-Exploit/pyipatcher"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1.3"
 pyquery = "^2.0.0"
+pyimg4 = "^0.7"
 
 [tool.poetry.scripts]
 pyipatcher = "pyipatcher.__main__:cli"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
```

### Comparing `pyipatcher-1.1.1/PKG-INFO` & `pyipatcher-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyipatcher
-Version: 1.1.1
+Version: 1.1.2
 Summary: iOS ARM64 patchfinder & iOS ARM64 bootchain patcher
 Home-page: https://github.com/Mini-Exploit/pyipatcher
 License: GPL-3.0-only
 Author: mini_exploit
 Author-email: 61931266+Mini-Exploit@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pyimg4 (>=0.7,<0.8)
 Requires-Dist: pyquery (>=2.0.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/Mini-Exploit/pyipatcher/issues
 Project-URL: Repository, https://github.com/Mini-Exploit/pyipatcher
 Description-Content-Type: text/markdown
 
 # pyipatcher
 Incomplete iOS bootchain patchers in Python
@@ -37,15 +38,15 @@
 git clone https://github.com/Mini-Exploit/pyipatcher
 cd pyipatcher
 ./install.sh
 ```
 ## Usage
 ```
 $ pyipatcher
-pyipatcher version: 1.1.0
+pyipatcher version: 1.1.1
 Usage: pyipatcher [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -h, --help  Show this message and exit.
 
 Commands:
   ibootpatcher
```

