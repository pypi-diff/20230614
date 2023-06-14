# Comparing `tmp/pytest-kafka-0.5.1.tar.gz` & `tmp/pytest-kafka-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-kafka-0.5.1.tar", last modified: Sat Oct  1 14:10:14 2022, max compression
+gzip compressed data, was "pytest-kafka-0.6.0.tar", last modified: Wed Jun 14 20:31:08 2023, max compression
```

## Comparing `pytest-kafka-0.5.1.tar` & `pytest-kafka-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-01 14:10:14.550526 pytest-kafka-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1095 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)       16 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4273 2022-10-01 14:10:14.550526 pytest-kafka-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3379 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-01 14:10:14.547526 pytest-kafka-0.5.1/pytest_kafka/
--rw-rw-rw-   0 root         (0) root         (0)      439 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/pytest_kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9813 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/pytest_kafka/_factories.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/pytest_kafka/_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/pytest_kafka/constants.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/pytest_kafka/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-01 14:10:14.549527 pytest-kafka-0.5.1/pytest_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4273 2022-10-01 14:10:14.000000 pytest-kafka-0.5.1/pytest_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      418 2022-10-01 14:10:14.000000 pytest-kafka-0.5.1/pytest_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-01 14:10:14.000000 pytest-kafka-0.5.1/pytest_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2022-10-01 14:10:14.000000 pytest-kafka-0.5.1/pytest_kafka.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-01 14:10:14.000000 pytest-kafka-0.5.1/pytest_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      184 2022-10-01 14:10:14.000000 pytest-kafka-0.5.1/pytest_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-10-01 14:10:14.000000 pytest-kafka-0.5.1/pytest_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-01 14:10:14.550526 pytest-kafka-0.5.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4482 2022-10-01 14:10:04.000000 pytest-kafka-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:31:08.900034 pytest-kafka-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4176 2023-06-14 20:31:08.900034 pytest-kafka-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3282 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:31:08.899034 pytest-kafka-0.6.0/pytest_kafka/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/pytest_kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9813 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/pytest_kafka/_factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/pytest_kafka/_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/pytest_kafka/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/pytest_kafka/install.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/pytest_kafka/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:31:08.900034 pytest-kafka-0.6.0/pytest_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4176 2023-06-14 20:31:08.000000 pytest-kafka-0.6.0/pytest_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-14 20:31:08.000000 pytest-kafka-0.6.0/pytest_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 20:31:08.000000 pytest-kafka-0.6.0/pytest_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-14 20:31:08.000000 pytest-kafka-0.6.0/pytest_kafka.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 20:31:08.000000 pytest-kafka-0.6.0/pytest_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-14 20:31:08.000000 pytest-kafka-0.6.0/pytest_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 20:31:08.000000 pytest-kafka-0.6.0/pytest_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 20:31:08.900034 pytest-kafka-0.6.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2409 2023-06-14 20:31:01.000000 pytest-kafka-0.6.0/setup.py
```

### Comparing `pytest-kafka-0.5.1/LICENCE` & `pytest-kafka-0.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pytest-kafka-0.5.1/PKG-INFO` & `pytest-kafka-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-kafka
-Version: 0.5.1
+Version: 0.6.0
 Summary: Zookeeper, Kafka server, and Kafka consumer fixtures for Pytest
 Home-page: https://gitlab.com/karolinepauls/pytest-kafka
 Author: Karoline Pauls
 Author-email: code@karolinepauls.com
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.com/karolinepauls/pytest-kafka/issues
 Project-URL: Documentation, https://pytest-kafka.readthedocs.io/
@@ -95,20 +95,18 @@
 - a JVM that can run Kafka and Zookeeper
 - Kafka - https://kafka.apache.org/downloads
 
 
 Development
 -----------
 
-Execute ``./setup.py develop`` in a virtualenv. This will take care of:
+.. code:: sh
 
-- installing dependencies
-- updating pip
-- installing dev dependencies
-- installing Kafka to the project dir (for development only)
+   pip install -e .[dev]
+   python ./pytest_kafka/install.py  # will install kafka to ./kafka
 
 
 Acknowledgements
 ----------------
 
 The library has been open-sourced from a codebase belonging to
 `Infectious Media <https://infectiousmedia.com>`__.
```

### Comparing `pytest-kafka-0.5.1/README.rst` & `pytest-kafka-0.6.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -72,20 +72,18 @@
 - a JVM that can run Kafka and Zookeeper
 - Kafka - https://kafka.apache.org/downloads
 
 
 Development
 -----------
 
-Execute ``./setup.py develop`` in a virtualenv. This will take care of:
+.. code:: sh
 
-- installing dependencies
-- updating pip
-- installing dev dependencies
-- installing Kafka to the project dir (for development only)
+   pip install -e .[dev]
+   python ./pytest_kafka/install.py  # will install kafka to ./kafka
 
 
 Acknowledgements
 ----------------
 
 The library has been open-sourced from a codebase belonging to
 `Infectious Media <https://infectiousmedia.com>`__.
```

### Comparing `pytest-kafka-0.5.1/pytest_kafka/_factories.py` & `pytest-kafka-0.6.0/pytest_kafka/_factories.py`

 * *Files identical despite different names*

### Comparing `pytest-kafka-0.5.1/pytest_kafka/_fixtures.py` & `pytest-kafka-0.6.0/pytest_kafka/_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-kafka-0.5.1/pytest_kafka/constants.py` & `pytest-kafka-0.6.0/pytest_kafka/constants.py`

 * *Files identical despite different names*

### Comparing `pytest-kafka-0.5.1/pytest_kafka.egg-info/PKG-INFO` & `pytest-kafka-0.6.0/pytest_kafka.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-kafka
-Version: 0.5.1
+Version: 0.6.0
 Summary: Zookeeper, Kafka server, and Kafka consumer fixtures for Pytest
 Home-page: https://gitlab.com/karolinepauls/pytest-kafka
 Author: Karoline Pauls
 Author-email: code@karolinepauls.com
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.com/karolinepauls/pytest-kafka/issues
 Project-URL: Documentation, https://pytest-kafka.readthedocs.io/
@@ -95,20 +95,18 @@
 - a JVM that can run Kafka and Zookeeper
 - Kafka - https://kafka.apache.org/downloads
 
 
 Development
 -----------
 
-Execute ``./setup.py develop`` in a virtualenv. This will take care of:
+.. code:: sh
 
-- installing dependencies
-- updating pip
-- installing dev dependencies
-- installing Kafka to the project dir (for development only)
+   pip install -e .[dev]
+   python ./pytest_kafka/install.py  # will install kafka to ./kafka
 
 
 Acknowledgements
 ----------------
 
 The library has been open-sourced from a codebase belonging to
 `Infectious Media <https://infectiousmedia.com>`__.
```

