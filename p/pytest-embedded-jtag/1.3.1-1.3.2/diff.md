# Comparing `tmp/pytest-embedded-jtag-1.3.1.tar.gz` & `tmp/pytest_embedded_jtag-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-jtag-1.3.1.tar", last modified: Tue Jun  6 08:07:05 2023, max compression
+gzip compressed data, was "pytest_embedded_jtag-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest-embedded-jtag-1.3.1.tar` & `pytest_embedded_jtag-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/openocd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/setup.py
+-rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.920594 pytest_embedded_jtag-1.3.2/LICENSE
+-rw-r--r--   0        0        0      245 2023-06-14 02:29:37.920594 pytest_embedded_jtag-1.3.2/README.md
+-rw-r--r--   0        0        0     2882 2023-06-14 02:29:37.920594 pytest_embedded_jtag-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      165 2023-06-14 02:29:37.920594 pytest_embedded_jtag-1.3.2/pytest_embedded_jtag/__init__.py
+-rw-r--r--   0        0        0     1845 2023-06-14 02:29:37.920594 pytest_embedded_jtag-1.3.2/pytest_embedded_jtag/gdb.py
+-rw-r--r--   0        0        0     2359 2023-06-14 02:29:37.924594 pytest_embedded_jtag-1.3.2/pytest_embedded_jtag/openocd.py
+-rw-r--r--   0        0        0      930 2023-06-14 02:29:37.924594 pytest_embedded_jtag-1.3.2/tests/test_jtag.py
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 pytest_embedded_jtag-1.3.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-embedded-jtag-1.3.1/PKG-INFO` & `pytest_embedded_jtag-1.3.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-embedded-jtag
-Version: 1.3.1
-Summary: pytest embedded plugin for testing with jtag
-Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
-Author: Fu Hanxi
-Author-email: fuhanxi@espressif.com
-License: MIT
-Description: ### pytest-embedded-jtag
-        
-        pytest embedded service for openocd/gdb utilities
-        
-        Extra Functionalities:
-        
-        - `openocd`: enable the fixture
-        - `gdb`: enable the fixture
-        - `dut`: duplicate the `openocd` output and the `gdb` output to `dut.pexpect_proc`.
-        
-Platform: UNKNOWN
+Version: 1.3.2
+Summary: Make pytest-embedded plugin work with JTAG.
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
+Requires-Dist: pytest-embedded-serial~=1.3.2
+Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
+Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
+Project-URL: homepage, https://github.com/espressif/pytest-embedded
+Project-URL: repository, https://github.com/espressif/pytest-embedded
+
+### pytest-embedded-jtag
+
+pytest embedded service for openocd/gdb utilities
+
+Extra Functionalities:
+
+- `openocd`: enable the fixture
+- `gdb`: enable the fixture
+- `dut`: duplicate the `openocd` output and the `gdb` output to `dut.pexpect_proc`.
+
```

### Comparing `pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/gdb.py` & `pytest_embedded_jtag-1.3.2/pytest_embedded_jtag/gdb.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/openocd.py` & `pytest_embedded_jtag-1.3.2/pytest_embedded_jtag/openocd.py`

 * *Files identical despite different names*

