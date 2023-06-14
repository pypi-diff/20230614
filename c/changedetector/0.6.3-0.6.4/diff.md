# Comparing `tmp/changedetector-0.6.3.tar.gz` & `tmp/changedetector-0.6.4.tar.gz`

## Comparing `changedetector-0.6.3.tar` & `changedetector-0.6.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/__init__.py
--rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/detectchange.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/gobals_variables.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/makeParser.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/menu.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/versionControl.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wrapperComponents.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wrm.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wro.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wrs.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wtch.py
--rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/scripts/detectchange.fish
--rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/scripts/detectchange.sh
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 changedetector-0.6.3/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.6.3/LICENCE
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 changedetector-0.6.3/README.md
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 changedetector-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 changedetector-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/__init__.py
+-rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/detectchange.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/gobals_variables.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/makeParser.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/menu.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/versionControl.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/wrapperComponents.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/wrm.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/wro.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/wrs.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/wtch.py
+-rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/scripts/detectchange.fish
+-rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.6.4/changedetector/scripts/detectchange.sh
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 changedetector-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.6.4/LICENCE
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 changedetector-0.6.4/README.md
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 changedetector-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 changedetector-0.6.4/PKG-INFO
```

### Comparing `changedetector-0.6.3/changedetector/__init__.py` & `changedetector-0.6.4/changedetector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = "changedetector"
 __author__ = "LuxLuth"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2023 LuxLuth"
-__version__ = "0.6.3"
+__version__ = "0.6.4"
```

### Comparing `changedetector-0.6.3/changedetector/detectchange.py` & `changedetector-0.6.4/changedetector/detectchange.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/makeParser.py` & `changedetector-0.6.4/changedetector/makeParser.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/menu.py` & `changedetector-0.6.4/changedetector/menu.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/versionControl.py` & `changedetector-0.6.4/changedetector/versionControl.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/wrapperComponents.py` & `changedetector-0.6.4/changedetector/wrapperComponents.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/wrm.py` & `changedetector-0.6.4/changedetector/wrm.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/wro.py` & `changedetector-0.6.4/changedetector/wro.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/wrs.py` & `changedetector-0.6.4/changedetector/wrs.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/wtch.py` & `changedetector-0.6.4/changedetector/wtch.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/scripts/detectchange.fish` & `changedetector-0.6.4/changedetector/scripts/detectchange.fish`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/changedetector/scripts/detectchange.sh` & `changedetector-0.6.4/changedetector/scripts/detectchange.sh`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/LICENCE` & `changedetector-0.6.4/LICENCE`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/README.md` & `changedetector-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.3/pyproject.toml` & `changedetector-0.6.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 dependencies = [
     "certifi==2023.5.7 ; python_version >= '3.6'",
     "charset-normalizer==3.1.0",
     "click==8.1.3 ; python_version >= '3.7'",
     "colorama==0.4.6",
     "idna==3.4 ; python_version >= '3.5'",
     "inquirerpy==0.3.4",
-    "markdown-it-py==2.2.0 ; python_version >= '3.7'",
+    "markdown-it-py==3.0.0 ; python_version >= '3.8'",
     "mdurl==0.1.2 ; python_version >= '3.7'",
     "pfzy==0.3.4 ; python_version >= '3.7' and python_version < '4.0'",
     "prompt-toolkit==3.0.38 ; python_full_version >= '3.7.0'",
     "pyfiglet==0.8.post1",
     "pygments==2.15.1 ; python_version >= '3.7'",
     "requests==2.31.0",
-    "rich==13.3.5",
+    "rich==13.4.2",
     "shellingham==1.5.0.post1",
     "tomli==2.0.1",
     "typer[all]==0.9.0",
     "typing==3.7.4.3",
-    "typing-extensions==4.6.0 ; python_version >= '3.7'",
-    "urllib3==2.0.2",
+    "typing-extensions==4.6.3 ; python_version >= '3.7'",
+    "urllib3==2.0.3",
     "watchdog==3.0.0",
     "wcwidth==0.2.6",
 ]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/luxluth/changedetector/issues"
 Homepage = "https://github.com/luxluth/changedetector"
```

### Comparing `changedetector-0.6.3/PKG-INFO` & `changedetector-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changedetector
-Version: 0.6.3
+Version: 0.6.4
 Summary: A basic change detector for the Python, Ruby and C++.
 Project-URL: Bug Tracker, https://github.com/luxluth/changedetector/issues
 Project-URL: Homepage, https://github.com/luxluth/changedetector
 Author-email: Lux Luth <luxusluth@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,28 +25,28 @@
 Requires-Python: >=3.7
 Requires-Dist: certifi==2023.5.7; python_version >= '3.6'
 Requires-Dist: charset-normalizer==3.1.0
 Requires-Dist: click==8.1.3; python_version >= '3.7'
 Requires-Dist: colorama==0.4.6
 Requires-Dist: idna==3.4; python_version >= '3.5'
 Requires-Dist: inquirerpy==0.3.4
-Requires-Dist: markdown-it-py==2.2.0; python_version >= '3.7'
+Requires-Dist: markdown-it-py==3.0.0; python_version >= '3.8'
 Requires-Dist: mdurl==0.1.2; python_version >= '3.7'
 Requires-Dist: pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 Requires-Dist: prompt-toolkit==3.0.38; python_full_version >= '3.7.0'
 Requires-Dist: pyfiglet==0.8.post1
 Requires-Dist: pygments==2.15.1; python_version >= '3.7'
 Requires-Dist: requests==2.31.0
-Requires-Dist: rich==13.3.5
+Requires-Dist: rich==13.4.2
 Requires-Dist: shellingham==1.5.0.post1
 Requires-Dist: tomli==2.0.1
 Requires-Dist: typer[all]==0.9.0
-Requires-Dist: typing-extensions==4.6.0; python_version >= '3.7'
+Requires-Dist: typing-extensions==4.6.3; python_version >= '3.7'
 Requires-Dist: typing==3.7.4.3
-Requires-Dist: urllib3==2.0.2
+Requires-Dist: urllib3==2.0.3
 Requires-Dist: watchdog==3.0.0
 Requires-Dist: wcwidth==0.2.6
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # changedetector
```

