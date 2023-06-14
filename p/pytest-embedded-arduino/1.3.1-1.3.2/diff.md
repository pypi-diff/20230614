# Comparing `tmp/pytest-embedded-arduino-1.3.1.tar.gz` & `tmp/pytest_embedded_arduino-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-embedded-arduino-1.3.1.tar", last modified: Tue Jun  6 08:56:26 2023, max compression
+gzip compressed data, was "pytest_embedded_arduino-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest-embedded-arduino-1.3.1.tar` & `pytest_embedded_arduino-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,8 @@
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1570 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/PKG-INFO
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      516 2023-06-06 08:04:34.000000 pytest-embedded-arduino-1.3.1/README.md
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      116 2023-04-11 02:32:21.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/__init__.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1879 2023-06-06 08:04:34.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/app.py
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1870 2023-06-02 06:32:41.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/serial.py
-drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1570 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/PKG-INFO
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      353 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/SOURCES.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)        1 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/dependency_links.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       67 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/requires.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       24 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/top_level.txt
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       38 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/setup.cfg
--rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1901 2023-06-06 08:49:39.000000 pytest-embedded-arduino-1.3.1/setup.py
+-rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/LICENSE
+-rw-r--r--   0        0        0      516 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/README.md
+-rw-r--r--   0        0        0     3047 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/__init__.py
+-rw-r--r--   0        0        0     1879 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/app.py
+-rw-r--r--   0        0        0     1870 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/serial.py
+-rw-r--r--   0        0        0      747 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/tests/test_arduino.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 pytest_embedded_arduino-1.3.2/PKG-INFO
```

### Comparing `pytest-embedded-arduino-1.3.1/PKG-INFO` & `pytest_embedded_arduino-1.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.3.1
-Summary: pytest embedded plugin for Arduino projects
-Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
-Author: Abdelatif Guettouche
-Author-email: abdelatif.guettouche@espressif.com
-License: MIT
+Version: 1.3.2
+Summary: Make pytest-embedded plugin work with Arduino.
+Author-email: Abdelatif Guettouche <abdelatif.guettouche@espressif.com>, Fu Hanxi <fuhanxi@espressif.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Development Status :: 5 - Production/Stable
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
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: pytest-embedded~=1.3.2
+Requires-Dist: pytest-embedded-serial-esp~=1.3.2 ; extra == "serial"
+Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
+Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
+Project-URL: homepage, https://github.com/espressif/pytest-embedded
+Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: serial
 
 ### pytest-embedded-arduino
 
 pytest embedded service for Arduino project
 
 Extra Functionalities:
@@ -38,7 +41,8 @@
         - `app`: Parse Arduino's build directory and gather more information.
         - `serial`: Auto flash the built binary into the target board at the beginning when running test cases.
 
    .. group-tab:: `pytest-embedded-serial-esp` NOT activated
 
         - `app`: Parse Arduino's build directory and gather more information.
 ```
+
```

### Comparing `pytest-embedded-arduino-1.3.1/README.md` & `pytest_embedded_arduino-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/app.py` & `pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/serial.py` & `pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/serial.py`

 * *Files identical despite different names*

