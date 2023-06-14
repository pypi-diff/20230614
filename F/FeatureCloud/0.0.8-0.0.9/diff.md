# Comparing `tmp/FeatureCloud-0.0.8.tar.gz` & `tmp/FeatureCloud-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeatureCloud-0.0.8.tar", last modified: Fri Dec 10 18:22:52 2021, max compression
+gzip compressed data, was "FeatureCloud-0.0.9.tar", last modified: Fri Dec 10 18:34:04 2021, max compression
```

## Comparing `FeatureCloud-0.0.8.tar` & `FeatureCloud-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,41 @@
-drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/
-drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/FeatureCloud/
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 17:12:14.000000 FeatureCloud-0.0.8/FeatureCloud/__init__.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2210 2021-12-10 18:10:24.000000 FeatureCloud-0.0.8/FeatureCloud/__main__.py
-drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/FeatureCloud/api/
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 12:06:59.000000 FeatureCloud-0.0.8/FeatureCloud/api/__init__.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     1432 2021-12-09 10:53:38.000000 FeatureCloud-0.0.8/FeatureCloud/api/http_ctrl.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      495 2021-12-09 10:53:38.000000 FeatureCloud-0.0.8/FeatureCloud/api/http_web.py
-drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/FeatureCloud/apps/
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 12:06:59.000000 FeatureCloud-0.0.8/FeatureCloud/apps/__init__.py
-drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/FeatureCloud/cli/
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 16:50:04.000000 FeatureCloud-0.0.8/FeatureCloud/cli/__init__.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)    12777 2021-12-10 16:50:33.000000 FeatureCloud-0.0.8/FeatureCloud/cli/cli.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      910 2021-10-19 10:44:42.000000 FeatureCloud-0.0.8/FeatureCloud/cli/helper.py
--rwxrwxr-x   0 mohammad  (1000) mohammad  (1000)     1204 2021-12-08 12:06:59.000000 FeatureCloud-0.0.8/FeatureCloud/diagram.py
-drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/FeatureCloud/engine/
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 12:06:59.000000 FeatureCloud-0.0.8/FeatureCloud/engine/__init__.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)    23965 2021-12-08 16:22:26.000000 FeatureCloud-0.0.8/FeatureCloud/engine/app.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     1013 2021-12-08 16:22:26.000000 FeatureCloud-0.0.8/FeatureCloud/engine/library.py
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      340 2021-12-08 12:06:59.000000 FeatureCloud-0.0.8/FeatureCloud/main.py
-drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/FeatureCloud.egg-info/
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2716 2021-12-10 18:22:52.000000 FeatureCloud-0.0.8/FeatureCloud.egg-info/PKG-INFO
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      592 2021-12-10 18:22:52.000000 FeatureCloud-0.0.8/FeatureCloud.egg-info/SOURCES.txt
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        1 2021-12-10 18:22:52.000000 FeatureCloud-0.0.8/FeatureCloud.egg-info/dependency_links.txt
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)       67 2021-12-10 18:22:52.000000 FeatureCloud-0.0.8/FeatureCloud.egg-info/entry_points.txt
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)       13 2021-12-10 18:22:52.000000 FeatureCloud-0.0.8/FeatureCloud.egg-info/top_level.txt
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)    11352 2021-11-16 16:59:45.000000 FeatureCloud-0.0.8/LICENSE
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2716 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/PKG-INFO
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2195 2021-12-10 16:46:54.000000 FeatureCloud-0.0.8/README.md
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)       38 2021-12-10 18:22:52.276248 FeatureCloud-0.0.8/setup.cfg
--rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     1229 2021-12-10 18:22:47.000000 FeatureCloud-0.0.8/setup.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 17:12:14.000000 FeatureCloud-0.0.9/FeatureCloud/__init__.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2210 2021-12-10 18:10:24.000000 FeatureCloud-0.0.9/FeatureCloud/__main__.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/api/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 12:06:59.000000 FeatureCloud-0.0.9/FeatureCloud/api/__init__.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     1432 2021-12-09 10:53:38.000000 FeatureCloud-0.0.9/FeatureCloud/api/http_ctrl.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      495 2021-12-09 10:53:38.000000 FeatureCloud-0.0.9/FeatureCloud/api/http_web.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/apps/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 12:06:59.000000 FeatureCloud-0.0.9/FeatureCloud/apps/__init__.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/cli/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 16:50:04.000000 FeatureCloud-0.0.9/FeatureCloud/cli/__init__.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/cli/api/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-10-19 10:44:42.000000 FeatureCloud-0.0.9/FeatureCloud/cli/api/__init__.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/cli/api/backend/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-10-19 10:44:42.000000 FeatureCloud-0.0.9/FeatureCloud/cli/api/backend/__init__.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     1494 2021-10-19 10:44:42.000000 FeatureCloud-0.0.9/FeatureCloud/cli/api/backend/auth.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2074 2021-10-19 10:44:42.000000 FeatureCloud-0.0.9/FeatureCloud/cli/api/backend/project.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2779 2021-10-19 10:44:42.000000 FeatureCloud-0.0.9/FeatureCloud/cli/api/controller.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)    12777 2021-12-10 16:50:33.000000 FeatureCloud-0.0.9/FeatureCloud/cli/cli.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      910 2021-10-19 10:44:42.000000 FeatureCloud-0.0.9/FeatureCloud/cli/helper.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/cli/tests/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 16:50:29.000000 FeatureCloud-0.0.9/FeatureCloud/cli/tests/__init__.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     3456 2021-10-19 10:44:42.000000 FeatureCloud-0.0.9/FeatureCloud/cli/tests/test_testbed.py
+-rwxrwxr-x   0 mohammad  (1000) mohammad  (1000)     1204 2021-12-08 12:06:59.000000 FeatureCloud-0.0.9/FeatureCloud/diagram.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud/engine/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        0 2021-12-08 12:06:59.000000 FeatureCloud-0.0.9/FeatureCloud/engine/__init__.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)    23965 2021-12-08 16:22:26.000000 FeatureCloud-0.0.9/FeatureCloud/engine/app.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     1013 2021-12-08 16:22:26.000000 FeatureCloud-0.0.9/FeatureCloud/engine/library.py
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      340 2021-12-08 12:06:59.000000 FeatureCloud-0.0.9/FeatureCloud/main.py
+drwxrwxr-x   0 mohammad  (1000) mohammad  (1000)        0 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/FeatureCloud.egg-info/
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2716 2021-12-10 18:34:04.000000 FeatureCloud-0.0.9/FeatureCloud.egg-info/PKG-INFO
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)      852 2021-12-10 18:34:04.000000 FeatureCloud-0.0.9/FeatureCloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)        1 2021-12-10 18:34:04.000000 FeatureCloud-0.0.9/FeatureCloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)       67 2021-12-10 18:34:04.000000 FeatureCloud-0.0.9/FeatureCloud.egg-info/entry_points.txt
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)       13 2021-12-10 18:34:04.000000 FeatureCloud-0.0.9/FeatureCloud.egg-info/top_level.txt
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)    11352 2021-11-16 16:59:45.000000 FeatureCloud-0.0.9/LICENSE
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2716 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/PKG-INFO
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     2195 2021-12-10 16:46:54.000000 FeatureCloud-0.0.9/README.md
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)       38 2021-12-10 18:34:04.484276 FeatureCloud-0.0.9/setup.cfg
+-rw-rw-r--   0 mohammad  (1000) mohammad  (1000)     1338 2021-12-10 18:33:50.000000 FeatureCloud-0.0.9/setup.py
```

### Comparing `FeatureCloud-0.0.8/FeatureCloud/__main__.py` & `FeatureCloud-0.0.9/FeatureCloud/__main__.py`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/FeatureCloud/api/http_ctrl.py` & `FeatureCloud-0.0.9/FeatureCloud/api/http_ctrl.py`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/FeatureCloud/cli/cli.py` & `FeatureCloud-0.0.9/FeatureCloud/cli/cli.py`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/FeatureCloud/cli/helper.py` & `FeatureCloud-0.0.9/FeatureCloud/cli/helper.py`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/FeatureCloud/diagram.py` & `FeatureCloud-0.0.9/FeatureCloud/diagram.py`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/FeatureCloud/engine/app.py` & `FeatureCloud-0.0.9/FeatureCloud/engine/app.py`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/FeatureCloud/engine/library.py` & `FeatureCloud-0.0.9/FeatureCloud/engine/library.py`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/FeatureCloud.egg-info/PKG-INFO` & `FeatureCloud-0.0.9/FeatureCloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureCloud
-Version: 0.0.8
+Version: 0.0.9
 Summary: Secure Federated Learning Platform
 Home-page: https://github.com/FeatureCloud/app-template
 Author: FeatureCloud
 Author-email: mohammad.bakhtiari@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/FeatureCloud/app-template/issues
 Platform: UNKNOWN
```

### Comparing `FeatureCloud-0.0.8/FeatureCloud.egg-info/SOURCES.txt` & `FeatureCloud-0.0.9/FeatureCloud.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,10 +13,17 @@
 FeatureCloud/api/__init__.py
 FeatureCloud/api/http_ctrl.py
 FeatureCloud/api/http_web.py
 FeatureCloud/apps/__init__.py
 FeatureCloud/cli/__init__.py
 FeatureCloud/cli/cli.py
 FeatureCloud/cli/helper.py
+FeatureCloud/cli/api/__init__.py
+FeatureCloud/cli/api/controller.py
+FeatureCloud/cli/api/backend/__init__.py
+FeatureCloud/cli/api/backend/auth.py
+FeatureCloud/cli/api/backend/project.py
+FeatureCloud/cli/tests/__init__.py
+FeatureCloud/cli/tests/test_testbed.py
 FeatureCloud/engine/__init__.py
 FeatureCloud/engine/app.py
 FeatureCloud/engine/library.py
```

### Comparing `FeatureCloud-0.0.8/LICENSE` & `FeatureCloud-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/PKG-INFO` & `FeatureCloud-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureCloud
-Version: 0.0.8
+Version: 0.0.9
 Summary: Secure Federated Learning Platform
 Home-page: https://github.com/FeatureCloud/app-template
 Author: FeatureCloud
 Author-email: mohammad.bakhtiari@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/FeatureCloud/app-template/issues
 Platform: UNKNOWN
```

### Comparing `FeatureCloud-0.0.8/README.md` & `FeatureCloud-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `FeatureCloud-0.0.8/setup.py` & `FeatureCloud-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="FeatureCloud",
-                 version="0.0.8",
+                 version="0.0.9",
                  author="FeatureCloud",
                  author_email="mohammad.bakhtiari@uni-hamburg.de",
                  description="Secure Federated Learning Platform",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/FeatureCloud/app-template",
                  project_urls={
                      "Bug Tracker": "https://github.com/FeatureCloud/app-template/issues",
                  },
                  classifiers=[
                      "Programming Language :: Python :: 3",
                      "Operating System :: OS Independent",
                  ],
-                 packages=['FeatureCloud', 'FeatureCloud.apps', 'FeatureCloud.engine', 'FeatureCloud.api', 'FeatureCloud.cli'],
+                 packages=['FeatureCloud', 'FeatureCloud.apps', 'FeatureCloud.engine', 'FeatureCloud.api', 'FeatureCloud.cli',
+                           'FeatureCloud.cli.api', 'FeatureCloud.cli.api.backend', 'FeatureCloud.cli.tests'],
                  python_requires=">=3.7",
                  entry_points={'console_scripts': ['FeatureCloud = FeatureCloud.__main__:fc_command',
                                                    ]
                                },
 
                  )
```

