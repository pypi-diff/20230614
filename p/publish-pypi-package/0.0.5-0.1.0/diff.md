# Comparing `tmp/publish_pypi_package-0.0.5.tar.gz` & `tmp/publish_pypi_package-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publish_pypi_package-0.0.5.tar", last modified: Mon Jun 12 12:56:01 2023, max compression
+gzip compressed data, was "publish_pypi_package-0.1.0.tar", last modified: Wed Jun 14 05:09:10 2023, max compression
```

## Comparing `publish_pypi_package-0.0.5.tar` & `publish_pypi_package-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.144092 publish_pypi_package-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 12:56:01.144092 publish_pypi_package-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.140092 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.140092 publish_pypi_package-0.0.5/py_package/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/py_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/py_package/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:56:01.144092 publish_pypi_package-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.140092 publish_pypi_package-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/tests/test_tempertaure.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:09:10.649076 publish_pypi_package-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-23 13:14:22.000000 publish_pypi_package-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      437 2023-06-14 05:09:10.648077 publish_pypi_package-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1744 2023-05-24 11:50:38.000000 publish_pypi_package-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 05:09:10.627076 publish_pypi_package-0.1.0/publish_pypi_package.egg-info/
+-rw-rw-rw-   0        0        0      437 2023-06-14 05:09:10.000000 publish_pypi_package-0.1.0/publish_pypi_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-06-14 05:09:10.000000 publish_pypi_package-0.1.0/publish_pypi_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 05:09:10.000000 publish_pypi_package-0.1.0/publish_pypi_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-14 05:09:10.000000 publish_pypi_package-0.1.0/publish_pypi_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 05:09:10.636082 publish_pypi_package-0.1.0/py_package/
+-rw-rw-rw-   0        0        0       53 2023-06-12 11:46:41.000000 publish_pypi_package-0.1.0/py_package/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-06-12 11:35:14.000000 publish_pypi_package-0.1.0/py_package/temperature.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 05:09:10.649076 publish_pypi_package-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      680 2023-06-14 05:06:57.000000 publish_pypi_package-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:09:10.644078 publish_pypi_package-0.1.0/tests/
+-rw-rw-rw-   0        0        0      142 2023-06-12 11:46:31.000000 publish_pypi_package-0.1.0/tests/test.py
+-rw-rw-rw-   0        0        0      116 2023-06-12 11:39:51.000000 publish_pypi_package-0.1.0/tests/test_tempertaure.py
```

### Comparing `publish_pypi_package-0.0.5/LICENSE` & `publish_pypi_package-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `publish_pypi_package-0.0.5/README.md` & `publish_pypi_package-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# publish-python-package
-
-> Publish the Python package in PyPI
-
-### Building the package files in local
-------------------------
-
-We need to build our python package:
-> Before we begin this step, I should mention that I’m using Python3.
-
-1. In your terminal (at the root of the project) run:
-
-``` 
-python -m pip install --upgrade build
-
-python -m build
-
-python -m pip install --upgrade pip setuptools wheel
-
-python setup.py sdist bdist_wheel
-
-### This commands creates a source distribution and a shareable wheel that can be published on pypi.org.
-```
-
-2. To test this, create a virtual Python environment.
-3. Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
-> Run: pip install <relative-path>python -m pip install .\publish-python-package\dist\package_pypi-0.0.2-py3-none-any.whl
-
-> If need update then run: python -m pip install --upgrade py_package
-
-4. Use the python script named `tests/test_tempertaure.py`,
-run the script while still in the virtual Python environment.
-
-## Using the publish Python package
-https://pypi.org/project/publish-pypi-package/
-
-> pip searches for the package files in the official Python Package Index, on pypi.org.
-
-> Installing Python pip on your system allows you to manage PyPI packages easily.
-
-- There are two installation options, via test pypi or via pypi. </br>Both work and have been tested successfully. </br>
-The way to use:
-```
-## Test PyPi - test.pypi.org
-python -m pip install --upgrade --index-url https://test.pypi.org/simple publish_pypi_package
-
-## PyPi - pypi.org
-python -m pip install publish_pypi_package
-```
-- Run the tests/test_tempertaure.py script
+# publish-python-package
+
+> Publish the Python package in PyPI
+
+### Building the package files in local
+------------------------
+
+We need to build our python package:
+> Before we begin this step, I should mention that I’m using Python3.
+
+1. In your terminal (at the root of the project) run:
+
+``` 
+python -m pip install --upgrade build
+
+python -m build
+
+python -m pip install --upgrade pip setuptools wheel
+
+python setup.py sdist bdist_wheel
+
+### This commands creates a source distribution and a shareable wheel that can be published on pypi.org.
+```
+
+2. To test this, create a virtual Python environment.
+3. Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
+> Run: pip install <relative-path>python -m pip install .\publish-python-package\dist\package_pypi-0.0.2-py3-none-any.whl
+
+> If need update then run: python -m pip install --upgrade py_package
+
+4. Use the python script named `tests/test_tempertaure.py`,
+run the script while still in the virtual Python environment.
+
+## Using the publish Python package
+https://pypi.org/project/publish-pypi-package/
+
+> pip searches for the package files in the official Python Package Index, on pypi.org.
+
+> Installing Python pip on your system allows you to manage PyPI packages easily.
+
+- There are two installation options, via test pypi or via pypi. </br>Both work and have been tested successfully. </br>
+The way to use:
+```
+## Test PyPi - test.pypi.org
+python -m pip install --upgrade --index-url https://test.pypi.org/simple publish_pypi_package
+
+## PyPi - pypi.org
+python -m pip install publish_pypi_package
+```
+- Run the tests/test_tempertaure.py script
```

