# Comparing `tmp/pytest-embedded-serial-1.3.1.tar.gz` & `tmp/pytest_embedded_serial-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-serial-1.3.1.tar", last modified: Tue Jun  6 08:07:04 2023, max compression
+gzip compressed data, was "pytest_embedded_serial-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest-embedded-serial-1.3.1.tar` & `pytest_embedded_serial-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/setup.py
+-rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.924594 pytest_embedded_serial-1.3.2/LICENSE
+-rw-r--r--   0        0        0      195 2023-06-14 02:29:37.924594 pytest_embedded_serial-1.3.2/README.md
+-rw-r--r--   0        0        0     2898 2023-06-14 02:29:37.924594 pytest_embedded_serial-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-06-14 02:29:37.924594 pytest_embedded_serial-1.3.2/pytest_embedded_serial/__init__.py
+-rw-r--r--   0        0        0     1271 2023-06-14 02:29:37.924594 pytest_embedded_serial-1.3.2/pytest_embedded_serial/dut.py
+-rw-r--r--   0        0        0     6113 2023-06-14 02:29:37.924594 pytest_embedded_serial-1.3.2/pytest_embedded_serial/serial.py
+-rw-r--r--   0        0        0     1653 2023-06-14 02:29:37.924594 pytest_embedded_serial-1.3.2/tests/test_serial.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.3.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-embedded-serial-1.3.1/pytest_embedded_serial/dut.py` & `pytest_embedded_serial-1.3.2/pytest_embedded_serial/dut.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-serial-1.3.1/pytest_embedded_serial/serial.py` & `pytest_embedded_serial-1.3.2/pytest_embedded_serial/serial.py`

 * *Files identical despite different names*

