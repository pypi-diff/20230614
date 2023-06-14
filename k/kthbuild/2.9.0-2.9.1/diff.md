# Comparing `tmp/kthbuild-2.9.0.tar.gz` & `tmp/kthbuild-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthbuild-2.9.0.tar", last modified: Fri May 26 09:58:35 2023, max compression
+gzip compressed data, was "kthbuild-2.9.1.tar", last modified: Fri May 26 14:15:03 2023, max compression
```

## Comparing `kthbuild-2.9.0.tar` & `kthbuild-2.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 09:58:35.909338 kthbuild-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-26 09:58:07.000000 kthbuild-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-26 09:58:35.909338 kthbuild-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-26 09:58:07.000000 kthbuild-2.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 09:58:35.909338 kthbuild-2.9.0/kthbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-26 09:58:35.000000 kthbuild-2.9.0/kthbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-26 09:58:35.000000 kthbuild-2.9.0/kthbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-26 09:58:35.000000 kthbuild-2.9.0/kthbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-26 09:58:35.000000 kthbuild-2.9.0/kthbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-26 09:58:35.000000 kthbuild-2.9.0/kthbuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    44530 2023-05-26 09:58:07.000000 kthbuild-2.9.0/kthbuild.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 09:58:35.909338 kthbuild-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-05-26 09:58:07.000000 kthbuild-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:15:03.422568 kthbuild-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-26 14:14:32.000000 kthbuild-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-26 14:15:03.422568 kthbuild-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-26 14:14:32.000000 kthbuild-2.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:15:03.422568 kthbuild-2.9.1/kthbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    44530 2023-05-26 14:14:32.000000 kthbuild-2.9.1/kthbuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 14:15:03.422568 kthbuild-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4872 2023-05-26 14:14:32.000000 kthbuild-2.9.1/setup.py
```

### Comparing `kthbuild-2.9.0/LICENSE` & `kthbuild-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kthbuild-2.9.0/PKG-INFO` & `kthbuild-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 2.9.0
+Version: 2.9.1
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-2.9.0/kthbuild.egg-info/PKG-INFO` & `kthbuild-2.9.1/kthbuild.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 2.9.0
+Version: 2.9.1
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-2.9.0/kthbuild.py` & `kthbuild-2.9.1/kthbuild.py`

 * *Files identical despite different names*

### Comparing `kthbuild-2.9.0/setup.py` & `kthbuild-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 import subprocess
 import os
 import platform
 
 __title__ = "kthbuild"
 __summary__ = "Knuth node build tools"
 __uri__ = "https://github.com/k-nuth/kthbuild"
-__version__ = "2.9.0"
+__version__ = "2.9.1"
 __author__ = "Fernando Pelliccioni"
 __email__ = "fpelliccioni@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2019-2023 Knuth Project"
 
 
 install_requires = [
     "conan>=2.0",
 ]
 
 if platform.machine() == 'x86_64':
-    install_requires.append("microarch >= 0.0.12")
+    install_requires.append("microarch >= 0.1.1")
 
 def running_in_cpt_context():
     # -e CONAN_UPLOAD="https://knuth.jfrog.io/artifactory/api/conan/knuth@True@upload_repo"
     # -e CONAN_REMOTES="https://knuth.jfrog.io/artifactory/api/conan/knuth@True@upload_repo,https://api.bintray.com/conan/bitprim/bitprim@True@remote1"
     # -e CONAN_REFERENCE="kth-infrastructure/0.6.0@kth/feature-ci-marchs"
     # -e CPT_PROFILE="@@include(default)@@@@[settings]@@arch=x86_64@@build_type=Release@@compiler=gcc@@compiler.version=9@@[options]@@kth-infrastructure:shared=False@@kth-infrastructure:march_id=4fZKi37a595hP@@kth-infrastructure:with_tests=False@@kth-infrastructure:with_examples=False@@[env]@@KTH_BRANCH=feature-ci-marchs@@KTH_CONAN_CHANNEL=feature-ci-marchs@@KTH_FULL_BUILD=0@@KTH_CONAN_VERSION=0.6.0@@[build_requires]@@@@"
     return (os.getenv("CONAN_UPLOAD", None) != None or
```

