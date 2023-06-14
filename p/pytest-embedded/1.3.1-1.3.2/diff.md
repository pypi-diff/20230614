# Comparing `tmp/pytest-embedded-1.3.1.tar.gz` & `tmp/pytest_embedded-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-1.3.1.tar", last modified: Tue Jun  6 08:07:03 2023, max compression
+gzip compressed data, was "pytest_embedded-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest-embedded-1.3.1.tar` & `pytest_embedded-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    50774 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/unity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/setup.py
+-rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/LICENSE
+-rw-r--r--   0        0        0      120 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/README.md
+-rw-r--r--   0        0        0     2950 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/__init__.py
+-rw-r--r--   0        0        0     1095 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/app.py
+-rw-r--r--   0        0        0     6922 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/dut.py
+-rw-r--r--   0        0        0     6886 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/log.py
+-rw-r--r--   0        0        0    50859 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/plugin.py
+-rw-r--r--   0        0        0    11199 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/unity.py
+-rw-r--r--   0        0        0     9950 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/utils.py
+-rw-r--r--   0        0        0    19868 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/tests/test_base.py
+-rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 pytest_embedded-1.3.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-embedded-1.3.1/PKG-INFO` & `pytest_embedded-1.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-embedded
-Version: 1.3.1
-Summary: pytest embedded plugin
-Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
-Author: Fu Hanxi
-Author-email: fuhanxi@espressif.com
-License: MIT
-Description: ### pytest-embedded
-        
-        A pytest plugin for embedded systems. Could activate different services for extra functionalities.
-        
-Platform: UNKNOWN
+Version: 1.3.2
+Summary: A pytest plugin that designed for embedded testing.
+Author-email: Fu Hanxi <fuhanxi@espressif.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: pytest>=7.0
+Requires-Dist: pexpect>=4.4
+Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
+Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
+Project-URL: homepage, https://github.com/espressif/pytest-embedded
+Project-URL: repository, https://github.com/espressif/pytest-embedded
+
+### pytest-embedded
+
+A pytest plugin for embedded systems. Could activate different services for extra functionalities.
+
```

### Comparing `pytest-embedded-1.3.1/pytest_embedded/app.py` & `pytest_embedded-1.3.2/pytest_embedded/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.3.1/pytest_embedded/dut.py` & `pytest_embedded-1.3.2/pytest_embedded/dut.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.3.1/pytest_embedded/log.py` & `pytest_embedded-1.3.2/pytest_embedded/log.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.3.1/pytest_embedded/plugin.py` & `pytest_embedded-1.3.2/pytest_embedded/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1271,21 +1271,25 @@
     cls = _fixture_classes_and_options.classes['gdb']
     kwargs = _fixture_classes_and_options.kwargs['gdb']
     return cls(**_drop_none_kwargs(kwargs))
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
-def qemu(_fixture_classes_and_options: ClassCliOptions) -> t.Optional['Qemu']:
+def qemu(_fixture_classes_and_options: ClassCliOptions, app) -> t.Optional['Qemu']:
     """A qemu subprocess that could read/redirect/write"""
     if 'qemu' not in _fixture_classes_and_options.classes:
         return None
 
     cls = _fixture_classes_and_options.classes['qemu']
     kwargs = _fixture_classes_and_options.kwargs['qemu']
+
+    if 'app' in kwargs and kwargs['app'] is None:
+        kwargs['app'] = app
+
     return cls(**_drop_none_kwargs(kwargs))
 
 
 @pytest.fixture
 @multi_dut_generator_fixture
 def dut(
     _fixture_classes_and_options: ClassCliOptions,
```

### Comparing `pytest-embedded-1.3.1/pytest_embedded/unity.py` & `pytest_embedded-1.3.2/pytest_embedded/unity.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.3.1/pytest_embedded/utils.py` & `pytest_embedded-1.3.2/pytest_embedded/utils.py`

 * *Files identical despite different names*

