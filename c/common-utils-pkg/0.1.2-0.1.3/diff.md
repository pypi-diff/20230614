# Comparing `tmp/common_utils_pkg-0.1.2.tar.gz` & `tmp/common_utils_pkg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_utils_pkg-0.1.2.tar", last modified: Mon Jun 12 09:13:30 2023, max compression
+gzip compressed data, was "common_utils_pkg-0.1.3.tar", last modified: Wed Jun 14 15:34:47 2023, max compression
```

## Comparing `common_utils_pkg-0.1.2.tar` & `common_utils_pkg-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-12 09:13:30.888237 common_utils_pkg-0.1.2/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-12 09:13:30.887844 common_utils_pkg-0.1.2/PKG-INFO
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-12 09:13:30.883303 common_utils_pkg-0.1.2/common_utils_pkg/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      147 2023-06-12 09:08:22.000000 common_utils_pkg-0.1.2/common_utils_pkg/__init__.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)      787 2023-06-12 09:00:48.000000 common_utils_pkg-0.1.2/common_utils_pkg/aws_adapter.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     2628 2023-05-28 07:54:54.000000 common_utils_pkg-0.1.2/common_utils_pkg/logger.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.1.2/common_utils_pkg/notifications.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-05-28 07:55:01.000000 common_utils_pkg-0.1.2/common_utils_pkg/scheduler.py
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-12 09:13:30.887213 common_utils_pkg-0.1.2/common_utils_pkg.egg-info/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-12 09:13:30.000000 common_utils_pkg-0.1.2/common_utils_pkg.egg-info/PKG-INFO
--rw-r--r--   0 nikitagetman   (501) staff       (20)      359 2023-06-12 09:13:30.000000 common_utils_pkg-0.1.2/common_utils_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-06-12 09:13:30.000000 common_utils_pkg-0.1.2/common_utils_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       23 2023-06-12 09:13:30.000000 common_utils_pkg-0.1.2/common_utils_pkg.egg-info/requires.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-06-12 09:13:30.000000 common_utils_pkg-0.1.2/common_utils_pkg.egg-info/top_level.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-06-12 09:13:30.888415 common_utils_pkg-0.1.2/setup.cfg
--rw-r--r--   0 nikitagetman   (501) staff       (20)      802 2023-06-12 09:13:26.000000 common_utils_pkg-0.1.2/setup.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-14 15:34:47.834319 common_utils_pkg-0.1.3/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-14 15:34:47.833971 common_utils_pkg-0.1.3/PKG-INFO
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-14 15:34:47.828897 common_utils_pkg-0.1.3/common_utils_pkg/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      147 2023-06-12 09:08:22.000000 common_utils_pkg-0.1.3/common_utils_pkg/__init__.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      787 2023-06-12 09:00:48.000000 common_utils_pkg-0.1.3/common_utils_pkg/aws_adapter.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     3344 2023-06-14 15:33:57.000000 common_utils_pkg-0.1.3/common_utils_pkg/logger.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.1.3/common_utils_pkg/notifications.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-05-28 07:55:01.000000 common_utils_pkg-0.1.3/common_utils_pkg/scheduler.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-14 15:34:47.833005 common_utils_pkg-0.1.3/common_utils_pkg.egg-info/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-14 15:34:47.000000 common_utils_pkg-0.1.3/common_utils_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      359 2023-06-14 15:34:47.000000 common_utils_pkg-0.1.3/common_utils_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-06-14 15:34:47.000000 common_utils_pkg-0.1.3/common_utils_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       23 2023-06-14 15:34:47.000000 common_utils_pkg-0.1.3/common_utils_pkg.egg-info/requires.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-06-14 15:34:47.000000 common_utils_pkg-0.1.3/common_utils_pkg.egg-info/top_level.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-06-14 15:34:47.834463 common_utils_pkg-0.1.3/setup.cfg
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      802 2023-06-14 15:21:08.000000 common_utils_pkg-0.1.3/setup.py
```

### Comparing `common_utils_pkg-0.1.2/PKG-INFO` & `common_utils_pkg-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common_utils_pkg
-Version: 0.1.2
+Version: 0.1.3
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.1.2/common_utils_pkg/aws_adapter.py` & `common_utils_pkg-0.1.3/common_utils_pkg/aws_adapter.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.2/common_utils_pkg/logger.py` & `common_utils_pkg-0.1.3/common_utils_pkg/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,7 +77,28 @@
         self.log(message, "warning", notify)
 
     def error(self, message, notify=False):
         self.log(message, "error", notify)
 
     def debug(self, message, notify=False):
         self.log(message, "debug", notify)
+
+    def create_prefix(self, prefix):
+        return Prefixer(logger=self, prefix=prefix)
+
+
+class Prefixer(Logger):
+    def __init__(self, logger: Logger, prefix):
+        self.prefix = prefix
+        self.logger = logger
+
+    def info(self, message, notify=False):
+        self.logger.info(message=f"{self.prefix}: {message}", notify=notify)
+
+    def warning(self, message, notify=False):
+        self.logger.warning(message=f"{self.prefix}: {message}", notify=notify)
+
+    def error(self, message, notify=False):
+        self.logger.error(message=f"{self.prefix}: {message}", notify=notify)
+
+    def debug(self, message, notify=False):
+        self.logger.debug(message=f"{self.prefix}: {message}", notify=notify)
```

### Comparing `common_utils_pkg-0.1.2/common_utils_pkg/notifications.py` & `common_utils_pkg-0.1.3/common_utils_pkg/notifications.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.2/common_utils_pkg/scheduler.py` & `common_utils_pkg-0.1.3/common_utils_pkg/scheduler.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.2/common_utils_pkg.egg-info/PKG-INFO` & `common_utils_pkg-0.1.3/common_utils_pkg.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-utils-pkg
-Version: 0.1.2
+Version: 0.1.3
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.1.2/setup.py` & `common_utils_pkg-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 DESCRIPTION = "Common utils package. With some basic classes."
 LONG_DESCRIPTION = "Package with common utils for new projects."
 
 setup(
     name="common_utils_pkg",
     version=VERSION,
     author="John Johny",
```

