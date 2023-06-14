# Comparing `tmp/archbuilder-0.1.2.tar.gz` & `tmp/archbuilder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archbuilder-0.1.2.tar", last modified: Wed Jun 14 12:02:49 2023, max compression
+gzip compressed data, was "archbuilder-0.1.3.tar", last modified: Wed Jun 14 11:26:53 2023, max compression
```

## Comparing `archbuilder-0.1.2.tar` & `archbuilder-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.614005 archbuilder-0.1.2/
--rw-rw-rw-   0        0        0       29 2023-06-14 09:02:15.000000 archbuilder-0.1.2/.coveragerc
--rw-rw-rw-   0        0        0       80 2023-06-14 09:02:15.000000 archbuilder-0.1.2/.flake8
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.558155 archbuilder-0.1.2/.github/
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.581092 archbuilder-0.1.2/.github/workflows/
--rw-rw-rw-   0        0        0      896 2023-06-14 10:38:08.000000 archbuilder-0.1.2/.github/workflows/pypi-publish.yml
--rw-rw-rw-   0        0        0     1013 2023-06-14 10:38:15.000000 archbuilder-0.1.2/.github/workflows/testpypi-publish.yml
--rw-rw-rw-   0        0        0      295 2023-06-14 09:02:15.000000 archbuilder-0.1.2/.gitignore
--rw-rw-rw-   0        0        0        8 2023-06-14 09:02:15.000000 archbuilder-0.1.2/.python-version
--rw-rw-rw-   0        0        0     1497 2023-06-14 12:02:49.613007 archbuilder-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-06-14 09:02:15.000000 archbuilder-0.1.2/Pipfile
--rw-rw-rw-   0        0        0    33603 2023-06-14 09:02:15.000000 archbuilder-0.1.2/Pipfile.lock
--rw-rw-rw-   0        0        0     1195 2023-06-14 09:02:15.000000 archbuilder-0.1.2/README.md
--rw-rw-rw-   0        0        0      493 2023-06-14 12:02:30.000000 archbuilder-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      154 2023-06-14 09:02:15.000000 archbuilder-0.1.2/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-06-14 12:02:49.614005 archbuilder-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.562144 archbuilder-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.582090 archbuilder-0.1.2/src/archbuilder/
--rw-rw-rw-   0        0        0      686 2023-06-14 10:32:57.000000 archbuilder-0.1.2/src/archbuilder/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.604031 archbuilder-0.1.2/src/archbuilder.egg-info/
--rw-rw-rw-   0        0        0     1497 2023-06-14 12:02:49.000000 archbuilder-0.1.2/src/archbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-06-14 12:02:49.000000 archbuilder-0.1.2/src/archbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 12:02:49.000000 archbuilder-0.1.2/src/archbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-14 12:02:49.000000 archbuilder-0.1.2/src/archbuilder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-14 12:02:49.000000 archbuilder-0.1.2/src/archbuilder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.607024 archbuilder-0.1.2/src/builder/
--rw-rw-rw-   0        0        0       30 2023-06-14 09:02:15.000000 archbuilder-0.1.2/src/builder/__init__.py
--rw-rw-rw-   0        0        0      738 2023-06-14 10:32:57.000000 archbuilder-0.1.2/src/builder/builder.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.609018 archbuilder-0.1.2/src/template/
--rw-rw-rw-   0        0        0       32 2023-06-14 09:02:15.000000 archbuilder-0.1.2/src/template/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-06-14 09:02:15.000000 archbuilder-0.1.2/src/template/template.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.563141 archbuilder-0.1.2/tests/
-drwxrwxrwx   0        0        0        0 2023-06-14 12:02:49.612012 archbuilder-0.1.2/tests/unit/
--rw-rw-rw-   0        0        0      392 2023-06-14 10:32:57.000000 archbuilder-0.1.2/tests/unit/test_builder.py
--rw-rw-rw-   0        0        0      608 2023-06-14 09:30:28.000000 archbuilder-0.1.2/tests/unit/test_template.py
--rw-rw-rw-   0        0        0      782 2023-06-14 09:02:15.000000 archbuilder-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.168307 archbuilder-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.160307 archbuilder-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.github/workflows/testpypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-14 11:26:53.168307 archbuilder-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 11:26:37.000000 archbuilder-0.1.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    33014 2023-06-14 11:26:37.000000 archbuilder-0.1.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-14 11:26:37.000000 archbuilder-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 11:26:37.000000 archbuilder-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 11:26:37.000000 archbuilder-0.1.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:26:53.168307 archbuilder-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.160307 archbuilder-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/src/archbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/archbuilder/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/src/archbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/src/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.168307 archbuilder-0.1.3/src/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/template/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.160307 archbuilder-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.168307 archbuilder-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-14 11:26:37.000000 archbuilder-0.1.3/tests/unit/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 11:26:37.000000 archbuilder-0.1.3/tests/unit/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 11:26:37.000000 archbuilder-0.1.3/tox.ini
```

### Comparing `archbuilder-0.1.2/.github/workflows/pypi-publish.yml` & `archbuilder-0.1.3/.github/workflows/pypi-publish.yml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# This workflow will upload the Python Package to PyPI using Twine when a release is created
-
-name: Publish Package To PyPI
-run-name: Publishing package to PyPI
-
-on:
-  release:
-    types: [published]
-
-jobs:
-  pypi-publish:
-    name: Upload release to PyPI
-    runs-on: ubuntu-latest
-
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: '3.x'
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python3 -m pip install build --user
-
-    - name: Build package
-      run: python3 -m build --sdist --wheel --outdir dist/ .
-
-    - name: Publish package distributions to PyPI
-      if: startsWith(github.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
+# This workflow will upload the Python Package to PyPI using Twine when a release is created
+
+name: Publish Package To PyPI
+run-name: Publishing package to PyPI
+
+on:
+  release:
+    types: [published]
+
+jobs:
+  pypi-publish:
+    name: Upload release to PyPI
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: '3.x'
+
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        python3 -m pip install build --user
+
+    - name: Build package
+      run: python3 -m build --sdist --wheel --outdir dist/ .
+
+    - name: Publish package distributions to PyPI
+      if: startsWith(github.ref, 'refs/tags')
+      uses: pypa/gh-action-pypi-publish@release/v1
+      with:
+        password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `archbuilder-0.1.2/.github/workflows/testpypi-publish.yml` & `archbuilder-0.1.3/.github/workflows/testpypi-publish.yml`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# This workflow will upload the Python Package to TestPyPI using Twine when a push is made to "develop"
-
-name: Upload Package To TestPyPI
-run-name: Uploading package to TestPyPI
-
-on:
-  push:
-    branches:
-      - develop
-
-jobs:
-  testpypi-publish:
-    name: Upload package to TestPyPI
-    runs-on: ubuntu-latest
-
-    steps:
-      - uses: actions/checkout@v3
-
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python3 -m pip install build --user
-
-      - name: Build a binary wheel and a source tarball
-        run: python3 -m build --sdist --wheel --outdir dist/ .
-        
-      - name: Publish package distributions to TestPyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository-url: https://test.pypi.org/legacy/
+# This workflow will upload the Python Package to TestPyPI using Twine when a push is made to "develop"
+
+name: Upload Package To TestPyPI
+run-name: Uploading package to TestPyPI
+
+on:
+  push:
+    branches:
+      - develop
+
+jobs:
+  testpypi-publish:
+    name: Upload package to TestPyPI
+    runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.x"
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python3 -m pip install build --user
+
+      - name: Build a binary wheel and a source tarball
+        run: python3 -m build --sdist --wheel --outdir dist/ .
+        
+      - name: Publish package distributions to TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `archbuilder-0.1.2/PKG-INFO` & `archbuilder-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1
-Name: archbuilder
-Version: 0.1.2
-Summary: A tool to enable developers set up their projects quickly
-Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-
-# Archbuilder
-
-Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
-```bash
-  pip install archbuilder
-```
-    
-## Usage
-
-##### 1. By using a python script
-```python
-# Import archbuilder
-from builder import Builder
-from template import Template
-
-# Create a template from a json file
-template = Template('sass.json')
-
-# Create the project tree from the template
-project = Builder('sass', template)
-project.build()
-```
-
-##### 2. By using the command-line
-Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
-```bash
-archbuilder sass sass.json
-```
-
-## Contributing
-
-Contributions are always welcome!
-
-For major changes, please open an issue first
-to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-## License
-
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: archbuilder
+Version: 0.1.3
+Summary: A tool to enable developers set up their projects quickly
+Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+
+# Archbuilder
+
+Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
+```bash
+  pip install archbuilder
+```
+    
+## Usage
+
+##### 1. By using a python script
+```python
+# Import archbuilder
+from builder import Builder
+from template import Template
+
+# Create a template from a json file
+template = Template('sass.json')
+
+# Create the project tree from the template
+project = Builder('sass', template)
+project.build()
+```
+
+##### 2. By using the command-line
+Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
+```bash
+archbuilder sass sass.json
+```
+
+## Contributing
+
+Contributions are always welcome!
+
+For major changes, please open an issue first
+to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+## License
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
```

### Comparing `archbuilder-0.1.2/Pipfile.lock` & `archbuilder-0.1.3/Pipfile.lock`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 21% similar despite different names*

```diff
@@ -1,2101 +1,2064 @@
-00000000: 7b0d 0a20 2020 2022 5f6d 6574 6122 3a20  {..    "_meta": 
-00000010: 7b0d 0a20 2020 2020 2020 2022 6861 7368  {..        "hash
-00000020: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00000030: 2020 2273 6861 3235 3622 3a20 2234 3136    "sha256": "416
-00000040: 6364 3039 3736 6138 3031 6637 3364 3633  cd0976a801f73d63
-00000050: 3737 3662 3038 6261 6465 3835 3934 6463  776b08bade8594dc
-00000060: 6534 3835 3463 3564 3233 3161 3664 3738  e4854c5d231a6d78
-00000070: 3761 3961 6237 6161 3235 6137 3622 0d0a  7a9ab7aa25a76"..
-00000080: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00000090: 2020 2020 2270 6970 6669 6c65 2d73 7065      "pipfile-spe
-000000a0: 6322 3a20 362c 0d0a 2020 2020 2020 2020  c": 6,..        
-000000b0: 2272 6571 7569 7265 7322 3a20 7b0d 0a20  "requires": {.. 
-000000c0: 2020 2020 2020 2020 2020 2022 7079 7468             "pyth
-000000d0: 6f6e 5f76 6572 7369 6f6e 223a 2022 332e  on_version": "3.
-000000e0: 3131 220d 0a20 2020 2020 2020 207d 2c0d  11"..        },.
-000000f0: 0a20 2020 2020 2020 2022 736f 7572 6365  .        "source
-00000100: 7322 3a20 5b0d 0a20 2020 2020 2020 2020  s": [..         
-00000110: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00000120: 2020 2020 2020 226e 616d 6522 3a20 2270        "name": "p
-00000130: 7970 6922 2c0d 0a20 2020 2020 2020 2020  ypi",..         
-00000140: 2020 2020 2020 2022 7572 6c22 3a20 2268         "url": "h
-00000150: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000160: 7369 6d70 6c65 222c 0d0a 2020 2020 2020  simple",..      
-00000170: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
-00000180: 795f 7373 6c22 3a20 7472 7565 0d0a 2020  y_ssl": true..  
-00000190: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-000001a0: 2020 2020 205d 0d0a 2020 2020 7d2c 0d0a       ]..    },..
-000001b0: 2020 2020 2264 6566 6175 6c74 223a 207b      "default": {
-000001c0: 7d2c 0d0a 2020 2020 2264 6576 656c 6f70  },..    "develop
-000001d0: 223a 207b 0d0a 2020 2020 2020 2020 2262  ": {..        "b
-000001e0: 6c61 636b 223a 207b 0d0a 2020 2020 2020  lack": {..      
-000001f0: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
-00000200: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-00000210: 2020 2022 7368 6132 3536 3a30 3634 3130     "sha256:06410
-00000220: 3137 3438 6166 6131 3261 6432 3239 3163  1748afa12ad2291c
-00000230: 3262 3931 6339 3630 6265 3238 6238 3137  2b91c960be28b817
-00000240: 6330 6337 6561 6133 3562 6563 3039 6363  c0c7eaa35bec09cc
-00000250: 3633 6161 3536 3439 3363 3522 2c0d 0a20  63aa56493c5",.. 
-00000260: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000270: 7368 6132 3536 3a30 3934 3565 3133 3530  sha256:0945e1350
-00000280: 3662 6535 3862 6637 6462 3933 6565 3538  6be58bf7db93ee58
-00000290: 3533 3234 3365 6233 3638 6163 6531 6330  53243eb368ace1c0
-000002a0: 3861 3234 6336 3563 6531 3038 3938 3665  8a24c65ce108986e
-000002b0: 6163 3635 3931 3522 2c0d 0a20 2020 2020  ac65915",..     
-000002c0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-000002d0: 3536 3a31 3163 3431 3066 3731 6238 3736  56:11c410f71b876
-000002e0: 6639 3631 6431 6465 3737 6239 3639 3961  f961d1de77b9699a
-000002f0: 6431 3966 3933 3930 3934 6333 6136 3737  d19f939094c3a677
-00000300: 3332 3366 3433 6437 6132 3938 3535 6665  323f43d7a29855fe
-00000310: 3332 3622 2c0d 0a20 2020 2020 2020 2020  326",..         
-00000320: 2020 2020 2020 2022 7368 6132 3536 3a31         "sha256:1
-00000330: 6337 6238 6436 3036 6537 3238 6134 3165  c7b8d606e728a41e
-00000340: 6131 6363 6264 3732 3634 3637 3765 3439  a1ccbd7264677e49
-00000350: 3465 3837 6366 3633 3065 3339 3932 3632  4e87cf630e399262
-00000360: 6365 6439 3264 3461 3864 6163 3934 3022  ced92d4a8dac940"
-00000370: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000380: 2020 2022 7368 6132 3536 3a31 6430 3636     "sha256:1d066
-00000390: 3931 6631 6562 3864 6539 3163 6431 6233  91f1eb8de91cd1b3
-000003a0: 3232 6632 3165 3362 6663 3965 6665 3063  22f21e3bfc9efe0c
-000003b0: 3763 6131 6630 6531 6562 3164 6234 3465  7ca1f0e1eb1db44e
-000003c0: 6133 3637 6466 6636 3536 6222 2c0d 0a20  a367dff656b",.. 
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000003e0: 7368 6132 3536 3a33 3233 3866 3261 6163  sha256:3238f2aac
-000003f0: 6638 3237 6431 3864 3236 6462 3037 3532  f827d18d26db0752
-00000400: 3465 3434 3734 3132 3333 6165 3039 6135  4e44741233ae09a5
-00000410: 3834 3237 3361 6130 3539 3036 3664 3634  84273aa059066d64
-00000420: 3463 6137 6233 3022 2c0d 0a20 2020 2020  4ca7b30",..     
-00000430: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00000440: 3536 3a33 3264 6161 3937 3833 3130 3663  56:32daa9783106c
-00000450: 3238 3831 3564 3035 6237 3234 3233 3865  28815d05b724238e
-00000460: 3330 3731 3866 3334 3135 3536 3533 6434  30718f34155653d4
-00000470: 6436 6531 3235 6463 3764 6165 6338 6532  d6e125dc7daec8e2
-00000480: 3630 6322 2c0d 0a20 2020 2020 2020 2020  60c",..         
-00000490: 2020 2020 2020 2022 7368 6132 3536 3a33         "sha256:3
-000004a0: 3564 3133 3831 6437 6132 3263 6335 6232  5d1381d7a22cc5b2
-000004b0: 6265 3266 3732 6337 6466 6461 6534 3037  be2f72c7dfdae407
-000004c0: 3261 3333 3336 3036 3036 3335 3731 3863  2a3336060635718c
-000004d0: 6337 6531 6564 6532 3432 3231 6436 6322  c7e1ede24221d6c"
-000004e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000004f0: 2020 2022 7368 6132 3536 3a33 6131 3530     "sha256:3a150
-00000500: 3534 3261 3230 3431 3234 6564 3030 3638  542a204124ed0068
-00000510: 3366 3064 6231 6635 6366 3163 3261 6161  3f0db1f5cf1c2aaa
-00000520: 6139 6363 3334 3935 6237 6133 6235 3937  a9cc3495b7a3b597
-00000530: 3666 6231 3336 3039 3061 6222 2c0d 0a20  6fb136090ab",.. 
-00000540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000550: 7368 6132 3536 3a34 3866 3964 3334 3536  sha256:48f9d3456
-00000560: 3735 6262 3766 6263 3364 6438 3538 3231  75bb7fbc3dd85821
-00000570: 6231 3234 3837 6531 6239 6137 3532 3432  b12487e1b9a75242
-00000580: 3032 3861 6461 6430 3333 3363 6533 3665  028adad0333ce36e
-00000590: 6432 6136 6432 3722 2c0d 0a20 2020 2020  d2a6d27",..     
-000005a0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-000005b0: 3536 3a35 3063 6233 3363 6163 3838 3137  56:50cb33cac8817
-000005c0: 3636 6135 6364 3939 3133 6531 3066 6637  66a5cd9913e10ff7
-000005d0: 3562 3165 3865 6237 3162 6162 6634 6337  5b1e8eb71babf4c7
-000005e0: 3130 3466 3265 3963 3532 6461 3166 6237  104f2e9c52da1fb7
-000005f0: 6465 3222 2c0d 0a20 2020 2020 2020 2020  de2",..         
-00000600: 2020 2020 2020 2022 7368 6132 3536 3a35         "sha256:5
-00000610: 3632 6264 3361 3730 3439 3566 6163 6635  62bd3a70495facf5
-00000620: 3638 3134 3239 3331 3439 6535 3161 6131  6814293149e51aa1
-00000630: 6265 3939 3331 3536 3734 3734 3939 3363  be9931567474993c
-00000640: 3739 3432 6666 3764 3335 3333 3936 3122  7942ff7d3533961"
-00000650: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000660: 2020 2022 7368 6132 3536 3a36 3764 6538     "sha256:67de8
-00000670: 6430 6332 3039 6562 3562 3333 3063 6365  d0c209eb5b330cce
-00000680: 3234 3639 3530 3364 6531 3162 6361 3430  2469503de11bca40
-00000690: 3835 3838 3064 3632 6631 3632 3862 6439  85880d62f1628bd9
-000006a0: 3937 3263 6333 3336 3662 3922 2c0d 0a20  972cc3366b9",.. 
-000006b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000006c0: 7368 6132 3536 3a36 6233 3961 6264 6662  sha256:6b39abdfb
-000006d0: 3430 3230 3032 6238 6137 6430 3330 6363  402002b8a7d030cc
-000006e0: 6338 3563 6635 6166 6666 3634 6565 3930  c85cf5afff64ee90
-000006f0: 6661 3463 3561 6562 6335 3331 6533 6164  fa4c5aebc531e3ad
-00000700: 3031 3735 6464 6222 2c0d 0a20 2020 2020  0175ddb",..     
-00000710: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00000720: 3536 3a36 6633 6333 3333 6561 3164 6436  56:6f3c333ea1dd6
-00000730: 3737 3162 3264 3337 3737 3438 3234 3239  771b2d3777482429
-00000740: 3836 3466 3865 3235 3838 3939 6636 6666  864f8e258899f6ff
-00000750: 3035 3832 3663 3361 3466 6363 3563 6533  05826c3a4fcc5ce3
-00000760: 6637 3022 2c0d 0a20 2020 2020 2020 2020  f70",..         
-00000770: 2020 2020 2020 2022 7368 6132 3536 3a37         "sha256:7
-00000780: 3134 3239 3034 3930 6331 3866 6230 3132  14290490c18fb012
-00000790: 3662 6161 3066 6361 3061 3534 6565 3739  6baa0fca0a54ee79
-000007a0: 3566 3735 3032 6234 3431 3737 6531 6365  5f7502b44177e1ce
-000007b0: 3736 3234 6261 3163 3030 6632 3333 3122  7624ba1c00f2331"
-000007c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000007d0: 2020 2022 7368 6132 3536 3a37 6333 6562     "sha256:7c3eb
-000007e0: 3763 6561 3233 3930 3433 3939 3836 3663  7cea23904399866c
-000007f0: 3535 3832 3662 3331 6331 6635 3562 6263  55826b31c1f55bbc
-00000800: 6433 3839 3063 6532 3266 6637 3034 3636  d3890ce22ff70466
-00000810: 6239 3037 6236 3737 3563 3222 2c0d 0a20  b907b6775c2",.. 
-00000820: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000830: 7368 6132 3536 3a39 3263 3534 3366 3638  sha256:92c543f68
-00000840: 3534 6332 3861 3363 3766 3339 6634 6439  54c28a3c7f39f4d9
-00000850: 6237 3639 3466 3961 3665 6239 6433 6335  b7694f9a6eb9d3c5
-00000860: 6532 6563 6534 3838 6333 3237 6236 6537  e2ece488c327b6e7
-00000870: 6561 3962 3236 3622 2c0d 0a20 2020 2020  ea9b266",..     
-00000880: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00000890: 3536 3a61 3666 3638 3836 6339 3836 3964  56:a6f6886c9869d
-000008a0: 3464 6161 6532 6431 3731 3563 6533 3461  4daae2d1715ce34a
-000008b0: 3139 6262 6334 6239 3530 3036 6432 3065  19bbc4b95006d20e
-000008c0: 6437 3835 6361 3030 6661 3033 6362 6133  d785ca00fa03cba3
-000008d0: 3132 6422 2c0d 0a20 2020 2020 2020 2020  12d",..         
-000008e0: 2020 2020 2020 2022 7368 6132 3536 3a61         "sha256:a
-000008f0: 3861 3936 3831 3235 6430 6136 6134 3034  8a968125d0a6a404
-00000900: 3834 3266 6131 6266 3062 3334 3961 3536  842fa1bf0b349a56
-00000910: 3836 3334 6638 3536 6161 3038 6666 6166  8634f856aa08ffaf
-00000920: 6634 3061 6530 6466 6135 3265 3763 3622  f40ae0dfa52e7c6"
-00000930: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000940: 2020 2022 7368 6132 3536 3a63 3761 6235     "sha256:c7ab5
-00000950: 3739 3033 3333 6334 3438 3930 3363 3462  790333c448903c4b
-00000960: 3732 3162 3539 6330 6438 3062 3131 6665  721b59c0d80b11fe
-00000970: 3565 3938 3033 6438 3730 3365 3834 6463  5e9803d8703e84dc
-00000980: 6238 6461 3536 6665 6331 6222 2c0d 0a20  b8da56fec1b",.. 
-00000990: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000009a0: 7368 6132 3536 3a65 3131 3434 3230 6266  sha256:e114420bf
-000009b0: 3236 6239 3064 3462 3964 6161 3539 3733  26b90d4b9daa5973
-000009c0: 3531 3333 3737 3632 6236 3330 3339 3735  51337762b6303975
-000009d0: 3262 6466 3732 6266 3336 3133 3634 6331  2bdf72bf361364c1
-000009e0: 6161 3035 3932 3522 2c0d 0a20 2020 2020  aa05925",..     
-000009f0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00000a00: 3536 3a65 3139 3863 6632 3738 3838 6164  56:e198cf27888ad
-00000a10: 3666 3466 6633 3331 6361 3163 3438 6666  6f4ff331ca1c48ff
-00000a20: 6330 3338 3834 3865 6139 6630 3331 6133  c038848ea9f031a3
-00000a30: 6234 3062 6133 3661 6365 6437 6532 3266  b40ba36aced7e22f
-00000a40: 3263 3822 2c0d 0a20 2020 2020 2020 2020  2c8",..         
-00000a50: 2020 2020 2020 2022 7368 6132 3536 3a65         "sha256:e
-00000a60: 6337 3531 3431 3830 3232 3138 3562 3063  c751418022185b0c
-00000a70: 3162 6237 6437 3733 3665 3639 3333 6434  1bb7d7736e6933d4
-00000a80: 3062 6262 3134 6331 3461 3061 6263 6639  0bbb14c14a0abcf9
-00000a90: 3132 3364 3162 3135 3966 3938 6464 3422  123d1b159f98dd4"
-00000aa0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000ab0: 2020 2022 7368 6132 3536 3a66 3062 6432     "sha256:f0bd2
-00000ac0: 6634 6135 3864 3636 3636 3530 3035 3432  f4a58d6666500542
-00000ad0: 6232 3633 3534 3937 3832 3138 6139 6261  b26354978218a9ba
-00000ae0: 6263 6463 3937 3237 3232 6634 6266 3930  bcdc972722f4bf90
-00000af0: 3737 3935 3234 3531 3566 3322 0d0a 2020  779524515f3"..  
-00000b00: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00000b10: 2020 2020 2020 2020 2020 2269 6e64 6578            "index
-00000b20: 223a 2022 7079 7069 222c 0d0a 2020 2020  ": "pypi",..    
-00000b30: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-00000b40: 223a 2022 3d3d 3233 2e33 2e30 220d 0a20  ": "==23.3.0".. 
-00000b50: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00000b60: 2020 2022 626c 6561 6368 223a 207b 0d0a     "bleach": {..
-00000b70: 2020 2020 2020 2020 2020 2020 2268 6173              "has
-00000b80: 6865 7322 3a20 5b0d 0a20 2020 2020 2020  hes": [..       
-00000b90: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
-00000ba0: 3a31 6131 6138 3563 3135 3935 6530 3764  :1a1a85c1595e07d
-00000bb0: 3864 6231 3463 3566 3039 6630 3965 3634  8db14c5f09f09e64
-00000bc0: 3333 3530 3263 3531 6335 3935 3937 3065  33502c51c595970e
-00000bd0: 6463 3039 3035 3531 6630 6462 3939 3431  dc090551f0db9941
-00000be0: 3422 2c0d 0a20 2020 2020 2020 2020 2020  4",..           
-00000bf0: 2020 2020 2022 7368 6132 3536 3a33 3363       "sha256:33c
-00000c00: 3136 6533 3335 3364 6264 3133 3032 3861  16e3353dbd13028a
-00000c10: 6234 3739 3961 3066 3839 6138 3366 3131  b4799a0f89a83f11
-00000c20: 3334 3035 6337 3636 6539 6331 3232 6466  3405c766e9c122df
-00000c30: 3861 3036 6635 6238 3562 3366 3422 0d0a  8a06f5b85b3f4"..
-00000c40: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-00000c50: 2020 2020 2020 2020 2020 2020 226d 6172              "mar
-00000c60: 6b65 7273 223a 2022 7079 7468 6f6e 5f76  kers": "python_v
-00000c70: 6572 7369 6f6e 203e 3d20 2733 2e37 2722  ersion >= '3.7'"
-00000c80: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000c90: 7665 7273 696f 6e22 3a20 223d 3d36 2e30  version": "==6.0
-00000ca0: 2e30 220d 0a20 2020 2020 2020 207d 2c0d  .0"..        },.
-00000cb0: 0a20 2020 2020 2020 2022 6361 6368 6574  .        "cachet
-00000cc0: 6f6f 6c73 223a 207b 0d0a 2020 2020 2020  ools": {..      
-00000cd0: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
-00000ce0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-00000cf0: 2020 2022 7368 6132 3536 3a39 3565 6636     "sha256:95ef6
-00000d00: 3331 6565 6165 6131 3462 6132 6533 3666  31eeaea14ba2e36f
-00000d10: 3036 3433 3766 3336 3436 3361 6163 3361  06437f36463aac3a
-00000d20: 3039 3637 3939 6538 3736 6565 3535 6535  096799e876ee55e5
-00000d30: 6364 6363 6231 3032 3539 3022 2c0d 0a20  cdccb102590",.. 
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000d50: 7368 6132 3536 3a64 6365 3833 6632 6439  sha256:dce83f2d9
-00000d60: 6234 6531 6637 3332 6138 6364 3434 6166  b4e1f732a8cd44af
-00000d70: 3865 3866 6162 3264 6265 3436 3230 3134  8e8fab2dbe462014
-00000d80: 3637 6663 3938 6233 6566 3866 3236 3930  67fc98b3ef8f2690
-00000d90: 3932 6266 3632 6222 0d0a 2020 2020 2020  92bf62b"..      
-00000da0: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
-00000db0: 2020 2020 2020 226d 6172 6b65 7273 223a        "markers":
-00000dc0: 2022 7079 7468 6f6e 5f76 6572 7369 6f6e   "python_version
-00000dd0: 203e 3d20 2733 2e37 2722 2c0d 0a20 2020   >= '3.7'",..   
-00000de0: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
-00000df0: 6e22 3a20 223d 3d35 2e33 2e31 220d 0a20  n": "==5.3.1".. 
-00000e00: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00000e10: 2020 2022 6365 7274 6966 6922 3a20 7b0d     "certifi": {.
-00000e20: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
-00000e30: 7368 6573 223a 205b 0d0a 2020 2020 2020  shes": [..      
-00000e40: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00000e50: 363a 3066 3064 3536 6463 3561 3661 6435  6:0f0d56dc5a6ad5
-00000e60: 3666 6434 6261 3336 3438 3464 3663 6333  6fd4ba36484d6cc3
-00000e70: 3434 3531 6531 6336 3534 3863 3631 6461  4451e1c6548c61da
-00000e80: 6164 3863 3332 3031 3639 6639 3165 6464  ad8c320169f91edd
-00000e90: 6337 222c 0d0a 2020 2020 2020 2020 2020  c7",..          
-00000ea0: 2020 2020 2020 2273 6861 3235 363a 6336        "sha256:c6
-00000eb0: 6332 6539 3866 3563 3738 3639 6566 6361  c2e98f5c7869efca
-00000ec0: 3166 3839 3136 6665 6432 3238 6464 3931  1f8916fed228dd91
-00000ed0: 3533 3966 3966 3162 3434 3463 3331 3463  539f9f1b444c314c
-00000ee0: 3036 6565 6630 3239 3830 6337 3136 220d  06eef02980c716".
-00000ef0: 0a20 2020 2020 2020 2020 2020 205d 2c0d  .            ],.
-00000f00: 0a20 2020 2020 2020 2020 2020 2022 6d61  .            "ma
-00000f10: 726b 6572 7322 3a20 2270 7974 686f 6e5f  rkers": "python_
-00000f20: 7665 7273 696f 6e20 3e3d 2027 332e 3627  version >= '3.6'
-00000f30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000f40: 2276 6572 7369 6f6e 223a 2022 3d3d 3230  "version": "==20
-00000f50: 3233 2e35 2e37 220d 0a20 2020 2020 2020  23.5.7"..       
-00000f60: 207d 2c0d 0a20 2020 2020 2020 2022 6368   },..        "ch
-00000f70: 6172 6465 7422 3a20 7b0d 0a20 2020 2020  ardet": {..     
-00000f80: 2020 2020 2020 2022 6861 7368 6573 223a         "hashes":
-00000f90: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00000fa0: 2020 2020 2273 6861 3235 363a 3064 3632      "sha256:0d62
-00000fb0: 3731 3262 3935 3662 6331 3534 6638 3566  712b956bc154f85f
-00000fc0: 6230 6132 3636 6532 6133 6335 3931 3363  b0a266e2a3c5913c
-00000fd0: 3239 3637 6530 3033 3438 3730 3162 3332  2967e00348701b32
-00000fe0: 3431 3164 3664 6566 3331 6535 222c 0d0a  411d6def31e5",..
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2273 6861 3235 363a 3336 3237 3737 6662  "sha256:362777fb
-00001010: 3031 3461 6635 3936 6164 3331 3333 3466  014af596ad31334f
-00001020: 6465 3165 3863 3332 3764 6664 6230 3736  de1e8c327dfdb076
-00001030: 6531 3936 3064 3136 3934 3636 3264 3436  e1960d1694662d46
-00001040: 6136 3931 3761 6239 220d 0a20 2020 2020  a6917ab9"..     
-00001050: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-00001060: 2020 2020 2020 2022 6d61 726b 6572 7322         "markers"
-00001070: 3a20 2270 7974 686f 6e5f 7665 7273 696f  : "python_versio
-00001080: 6e20 3e3d 2027 332e 3727 222c 0d0a 2020  n >= '3.7'",..  
-00001090: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
-000010a0: 6f6e 223a 2022 3d3d 352e 312e 3022 0d0a  on": "==5.1.0"..
-000010b0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000010c0: 2020 2020 2263 6861 7273 6574 2d6e 6f72      "charset-nor
-000010d0: 6d61 6c69 7a65 7222 3a20 7b0d 0a20 2020  malizer": {..   
-000010e0: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
-000010f0: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00001100: 2020 2020 2020 2273 6861 3235 363a 3034        "sha256:04
-00001110: 6166 6136 3338 3765 3262 3238 3263 6637  afa6387e2b282cf7
-00001120: 3866 6633 6462 6365 3230 6630 6363 3037  8ff3dbce20f0cc07
-00001130: 3163 3132 6463 3866 3638 3562 6434 3039  1c12dc8f685bd409
-00001140: 3630 6363 3638 3634 3463 6665 6136 222c  60cc68644cfea6",
-00001150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001160: 2020 2273 6861 3235 363a 3034 6565 6663    "sha256:04eefc
-00001170: 6565 3039 3566 3538 6561 6162 6536 6463  ee095f58eaabe6dc
-00001180: 3363 6332 3236 3266 3362 6364 3737 3664  3cc2262f3bcd776d
-00001190: 3263 3637 3030 3538 3830 3839 3466 3434  2c67005880894f44
-000011a0: 3762 3366 3263 6239 6331 222c 0d0a 2020  7b3f2cb9c1",..  
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000011c0: 6861 3235 363a 3062 6536 3563 6366 3631  ha256:0be65ccf61
-000011d0: 3863 3165 3761 6339 6238 3439 6333 3135  8c1e7ac9b849c315
-000011e0: 6363 3265 3861 3837 3531 6439 6366 6461  cc2e8a8751d9cfda
-000011f0: 6134 3330 3237 6434 6636 3632 3462 6435  a43027d4f6624bd5
-00001200: 3837 6162 3765 222c 0d0a 2020 2020 2020  87ab7e",..      
-00001210: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001220: 363a 3063 3935 6631 3262 3734 3638 3165  6:0c95f12b74681e
-00001230: 3961 6531 3237 3732 3866 3765 3534 3039  9ae127728f7e5409
-00001240: 6362 6265 6639 6364 3931 3464 3538 3936  cbbef9cd914d5896
-00001250: 6566 3233 3863 6337 3739 6238 3135 3233  ef238cc779b81523
-00001260: 3733 222c 0d0a 2020 2020 2020 2020 2020  73",..          
-00001270: 2020 2020 2020 2273 6861 3235 363a 3063        "sha256:0c
-00001280: 6135 3634 3630 3664 3263 6161 6662 3061  a564606d2caafb0a
-00001290: 6265 3664 3162 3533 3131 6332 3634 3965  be6d1b5311c2649e
-000012a0: 3830 3731 6562 3234 3162 3264 3634 6537  8071eb241b2d64e7
-000012b0: 3561 3064 3030 3635 3130 3765 3632 222c  5a0d0065107e62",
-000012c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000012d0: 2020 2273 6861 3235 363a 3130 6339 3336    "sha256:10c936
-000012e0: 3238 6437 3439 3763 3831 3638 3665 3865  28d7497c81686e8e
-000012f0: 3565 3535 3761 6166 6137 3866 3233 3063  5e557aafa78f230c
-00001300: 6439 6537 3764 6430 6334 3030 3332 6566  d9e77dd0c40032ef
-00001310: 3930 6331 3866 3232 3330 222c 0d0a 2020  90c18f2230",..  
-00001320: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001330: 6861 3235 363a 3131 6431 3137 6536 6336  ha256:11d117e6c6
-00001340: 3365 3866 3439 3534 3132 6433 3765 3764  3e8f495412d37e7d
-00001350: 6332 6532 6666 6630 3963 3334 6232 6430  c2e2fff09c34b2d0
-00001360: 3964 6265 3262 6565 3363 3632 3239 3537  9dbe2bee3c622957
-00001370: 3738 3138 6265 222c 0d0a 2020 2020 2020  7818be",..      
+00000000: 7b0a 2020 2020 225f 6d65 7461 223a 207b  {.    "_meta": {
+00000010: 0a20 2020 2020 2020 2022 6861 7368 223a  .        "hash":
+00000020: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000030: 7368 6132 3536 223a 2022 3431 3663 6430  sha256": "416cd0
+00000040: 3937 3661 3830 3166 3733 6436 3337 3736  976a801f73d63776
+00000050: 6230 3862 6164 6538 3539 3464 6365 3438  b08bade8594dce48
+00000060: 3534 6335 6432 3331 6136 6437 3837 6139  54c5d231a6d787a9
+00000070: 6162 3761 6132 3561 3736 220a 2020 2020  ab7aa25a76".    
+00000080: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000090: 7069 7066 696c 652d 7370 6563 223a 2036  pipfile-spec": 6
+000000a0: 2c0a 2020 2020 2020 2020 2272 6571 7569  ,.        "requi
+000000b0: 7265 7322 3a20 7b0a 2020 2020 2020 2020  res": {.        
+000000c0: 2020 2020 2270 7974 686f 6e5f 7665 7273      "python_vers
+000000d0: 696f 6e22 3a20 2233 2e31 3122 0a20 2020  ion": "3.11".   
+000000e0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000000f0: 2273 6f75 7263 6573 223a 205b 0a20 2020  "sources": [.   
+00000100: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00000110: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+00000120: 223a 2022 7079 7069 222c 0a20 2020 2020  ": "pypi",.     
+00000130: 2020 2020 2020 2020 2020 2022 7572 6c22             "url"
+00000140: 3a20 2268 7474 7073 3a2f 2f70 7970 692e  : "https://pypi.
+00000150: 6f72 672f 7369 6d70 6c65 222c 0a20 2020  org/simple",.   
+00000160: 2020 2020 2020 2020 2020 2020 2022 7665               "ve
+00000170: 7269 6679 5f73 736c 223a 2074 7275 650a  rify_ssl": true.
+00000180: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000190: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
+000001a0: 2020 2022 6465 6661 756c 7422 3a20 7b7d     "default": {}
+000001b0: 2c0a 2020 2020 2264 6576 656c 6f70 223a  ,.    "develop":
+000001c0: 207b 0a20 2020 2020 2020 2022 626c 6163   {.        "blac
+000001d0: 6b22 3a20 7b0a 2020 2020 2020 2020 2020  k": {.          
+000001e0: 2020 2268 6173 6865 7322 3a20 5b0a 2020    "hashes": [.  
+000001f0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00000200: 6861 3235 363a 3036 3431 3031 3734 3861  ha256:064101748a
+00000210: 6661 3132 6164 3232 3931 6332 6239 3163  fa12ad2291c2b91c
+00000220: 3936 3062 6532 3862 3831 3763 3063 3765  960be28b817c0c7e
+00000230: 6161 3335 6265 6330 3963 6336 3361 6135  aa35bec09cc63aa5
+00000240: 3634 3933 6335 222c 0a20 2020 2020 2020  6493c5",.       
+00000250: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00000260: 3a30 3934 3565 3133 3530 3662 6535 3862  :0945e13506be58b
+00000270: 6637 6462 3933 6565 3538 3533 3234 3365  f7db93ee5853243e
+00000280: 6233 3638 6163 6531 6330 3861 3234 6336  b368ace1c08a24c6
+00000290: 3563 6531 3038 3938 3665 6163 3635 3931  5ce108986eac6591
+000002a0: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
+000002b0: 2020 2020 2273 6861 3235 363a 3131 6334      "sha256:11c4
+000002c0: 3130 6637 3162 3837 3666 3936 3164 3164  10f71b876f961d1d
+000002d0: 6537 3762 3936 3939 6164 3139 6639 3339  e77b9699ad19f939
+000002e0: 3039 3463 3361 3637 3733 3233 6634 3364  094c3a677323f43d
+000002f0: 3761 3239 3835 3566 6533 3236 222c 0a20  7a29855fe326",. 
+00000300: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000310: 7368 6132 3536 3a31 6337 6238 6436 3036  sha256:1c7b8d606
+00000320: 6537 3238 6134 3165 6131 6363 6264 3732  e728a41ea1ccbd72
+00000330: 3634 3637 3765 3439 3465 3837 6366 3633  64677e494e87cf63
+00000340: 3065 3339 3932 3632 6365 6439 3264 3461  0e399262ced92d4a
+00000350: 3864 6163 3934 3022 2c0a 2020 2020 2020  8dac940",.      
+00000360: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00000370: 363a 3164 3036 3639 3166 3165 6238 6465  6:1d06691f1eb8de
+00000380: 3931 6364 3162 3332 3266 3231 6533 6266  91cd1b322f21e3bf
+00000390: 6339 6566 6530 6337 6361 3166 3065 3165  c9efe0c7ca1f0e1e
+000003a0: 6231 6462 3434 6561 3336 3764 6666 3635  b1db44ea367dff65
+000003b0: 3662 222c 0a20 2020 2020 2020 2020 2020  6b",.           
+000003c0: 2020 2020 2022 7368 6132 3536 3a33 3233       "sha256:323
+000003d0: 3866 3261 6163 6638 3237 6431 3864 3236  8f2aacf827d18d26
+000003e0: 6462 3037 3532 3465 3434 3734 3132 3333  db07524e44741233
+000003f0: 6165 3039 6135 3834 3237 3361 6130 3539  ae09a584273aa059
+00000400: 3036 3664 3634 3463 6137 6233 3022 2c0a  066d644ca7b30",.
+00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000420: 2273 6861 3235 363a 3332 6461 6139 3738  "sha256:32daa978
+00000430: 3331 3036 6332 3838 3135 6430 3562 3732  3106c28815d05b72
+00000440: 3432 3338 6533 3037 3138 6633 3431 3535  4238e30718f34155
+00000450: 3635 3364 3464 3665 3132 3564 6337 6461  653d4d6e125dc7da
+00000460: 6563 3865 3236 3063 222c 0a20 2020 2020  ec8e260c",.     
+00000470: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00000480: 3536 3a33 3564 3133 3831 6437 6132 3263  56:35d1381d7a22c
+00000490: 6335 6232 6265 3266 3732 6337 6466 6461  c5b2be2f72c7dfda
+000004a0: 6534 3037 3261 3333 3336 3036 3036 3335  e4072a3336060635
+000004b0: 3731 3863 6337 6531 6564 6532 3432 3231  718cc7e1ede24221
+000004c0: 6436 6322 2c0a 2020 2020 2020 2020 2020  d6c",.          
+000004d0: 2020 2020 2020 2273 6861 3235 363a 3361        "sha256:3a
+000004e0: 3135 3035 3432 6132 3034 3132 3465 6430  150542a204124ed0
+000004f0: 3036 3833 6630 6462 3166 3563 6631 6332  0683f0db1f5cf1c2
+00000500: 6161 6161 3963 6333 3439 3562 3761 3362  aaaa9cc3495b7a3b
+00000510: 3539 3736 6662 3133 3630 3930 6162 222c  5976fb136090ab",
+00000520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000530: 2022 7368 6132 3536 3a34 3866 3964 3334   "sha256:48f9d34
+00000540: 3536 3735 6262 3766 6263 3364 6438 3538  5675bb7fbc3dd858
+00000550: 3231 6231 3234 3837 6531 6239 6137 3532  21b12487e1b9a752
+00000560: 3432 3032 3861 6461 6430 3333 3363 6533  42028adad0333ce3
+00000570: 3665 6432 6136 6432 3722 2c0a 2020 2020  6ed2a6d27",.    
+00000580: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00000590: 3235 363a 3530 6362 3333 6361 6338 3831  256:50cb33cac881
+000005a0: 3736 3661 3563 6439 3931 3365 3130 6666  766a5cd9913e10ff
+000005b0: 3735 6231 6538 6562 3731 6261 6266 3463  75b1e8eb71babf4c
+000005c0: 3731 3034 6632 6539 6335 3264 6131 6662  7104f2e9c52da1fb
+000005d0: 3764 6532 222c 0a20 2020 2020 2020 2020  7de2",.         
+000005e0: 2020 2020 2020 2022 7368 6132 3536 3a35         "sha256:5
+000005f0: 3632 6264 3361 3730 3439 3566 6163 6635  62bd3a70495facf5
+00000600: 3638 3134 3239 3331 3439 6535 3161 6131  6814293149e51aa1
+00000610: 6265 3939 3331 3536 3734 3734 3939 3363  be9931567474993c
+00000620: 3739 3432 6666 3764 3335 3333 3936 3122  7942ff7d3533961"
+00000630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000640: 2020 2273 6861 3235 363a 3637 6465 3864    "sha256:67de8d
+00000650: 3063 3230 3965 6235 6233 3330 6363 6532  0c209eb5b330cce2
+00000660: 3436 3935 3033 6465 3131 6263 6134 3038  469503de11bca408
+00000670: 3538 3830 6436 3266 3136 3238 6264 3939  5880d62f1628bd99
+00000680: 3732 6363 3333 3636 6239 222c 0a20 2020  72cc3366b9",.   
+00000690: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+000006a0: 6132 3536 3a36 6233 3961 6264 6662 3430  a256:6b39abdfb40
+000006b0: 3230 3032 6238 6137 6430 3330 6363 6338  2002b8a7d030ccc8
+000006c0: 3563 6635 6166 6666 3634 6565 3930 6661  5cf5afff64ee90fa
+000006d0: 3463 3561 6562 6335 3331 6533 6164 3031  4c5aebc531e3ad01
+000006e0: 3735 6464 6222 2c0a 2020 2020 2020 2020  75ddb",.        
+000006f0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00000700: 3666 3363 3333 3365 6131 6464 3637 3731  6f3c333ea1dd6771
+00000710: 6232 6433 3737 3734 3832 3432 3938 3634  b2d3777482429864
+00000720: 6638 6532 3538 3839 3966 3666 6630 3538  f8e258899f6ff058
+00000730: 3236 6333 6134 6663 6335 6365 3366 3730  26c3a4fcc5ce3f70
+00000740: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000750: 2020 2022 7368 6132 3536 3a37 3134 3239     "sha256:71429
+00000760: 3034 3930 6331 3866 6230 3132 3662 6161  0490c18fb0126baa
+00000770: 3066 6361 3061 3534 6565 3739 3566 3735  0fca0a54ee795f75
+00000780: 3032 6234 3431 3737 6531 6365 3736 3234  02b44177e1ce7624
+00000790: 6261 3163 3030 6632 3333 3122 2c0a 2020  ba1c00f2331",.  
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000007b0: 6861 3235 363a 3763 3365 6237 6365 6132  ha256:7c3eb7cea2
+000007c0: 3339 3034 3339 3938 3636 6335 3538 3236  3904399866c55826
+000007d0: 6233 3163 3166 3535 6262 6364 3338 3930  b31c1f55bbcd3890
+000007e0: 6365 3232 6666 3730 3436 3662 3930 3762  ce22ff70466b907b
+000007f0: 3637 3735 6332 222c 0a20 2020 2020 2020  6775c2",.       
+00000800: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00000810: 3a39 3263 3534 3366 3638 3534 6332 3861  :92c543f6854c28a
+00000820: 3363 3766 3339 6634 6439 6237 3639 3466  3c7f39f4d9b7694f
+00000830: 3961 3665 6239 6433 6335 6532 6563 6534  9a6eb9d3c5e2ece4
+00000840: 3838 6333 3237 6236 6537 6561 3962 3236  88c327b6e7ea9b26
+00000850: 3622 2c0a 2020 2020 2020 2020 2020 2020  6",.            
+00000860: 2020 2020 2273 6861 3235 363a 6136 6636      "sha256:a6f6
+00000870: 3838 3663 3938 3639 6434 6461 6165 3264  886c9869d4daae2d
+00000880: 3137 3135 6365 3334 6131 3962 6263 3462  1715ce34a19bbc4b
+00000890: 3935 3030 3664 3230 6564 3738 3563 6130  95006d20ed785ca0
+000008a0: 3066 6130 3363 6261 3331 3264 222c 0a20  0fa03cba312d",. 
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000008c0: 7368 6132 3536 3a61 3861 3936 3831 3235  sha256:a8a968125
+000008d0: 6430 6136 6134 3034 3834 3266 6131 6266  d0a6a404842fa1bf
+000008e0: 3062 3334 3961 3536 3836 3334 6638 3536  0b349a568634f856
+000008f0: 6161 3038 6666 6166 6634 3061 6530 6466  aa08ffaff40ae0df
+00000900: 6135 3265 3763 3622 2c0a 2020 2020 2020  a52e7c6",.      
+00000910: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00000920: 363a 6337 6162 3537 3930 3333 3363 3434  6:c7ab5790333c44
+00000930: 3839 3033 6334 6237 3231 6235 3963 3064  8903c4b721b59c0d
+00000940: 3830 6231 3166 6535 6539 3830 3364 3837  80b11fe5e9803d87
+00000950: 3033 6538 3464 6362 3864 6135 3666 6563  03e84dcb8da56fec
+00000960: 3162 222c 0a20 2020 2020 2020 2020 2020  1b",.           
+00000970: 2020 2020 2022 7368 6132 3536 3a65 3131       "sha256:e11
+00000980: 3434 3230 6266 3236 6239 3064 3462 3964  4420bf26b90d4b9d
+00000990: 6161 3539 3733 3531 3333 3737 3632 6236  aa597351337762b6
+000009a0: 3330 3339 3735 3262 6466 3732 6266 3336  3039752bdf72bf36
+000009b0: 3133 3634 6331 6161 3035 3932 3522 2c0a  1364c1aa05925",.
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2273 6861 3235 363a 6531 3938 6366 3237  "sha256:e198cf27
+000009e0: 3838 3861 6436 6634 6666 3333 3163 6131  888ad6f4ff331ca1
+000009f0: 6334 3866 6663 3033 3838 3438 6561 3966  c48ffc038848ea9f
+00000a00: 3033 3161 3362 3430 6261 3336 6163 6564  031a3b40ba36aced
+00000a10: 3765 3232 6632 6338 222c 0a20 2020 2020  7e22f2c8",.     
+00000a20: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00000a30: 3536 3a65 6337 3531 3431 3830 3232 3138  56:ec75141802218
+00000a40: 3562 3063 3162 6237 6437 3733 3665 3639  5b0c1bb7d7736e69
+00000a50: 3333 6434 3062 6262 3134 6331 3461 3061  33d40bbb14c14a0a
+00000a60: 6263 6639 3132 3364 3162 3135 3966 3938  bcf9123d1b159f98
+00000a70: 6464 3422 2c0a 2020 2020 2020 2020 2020  dd4",.          
+00000a80: 2020 2020 2020 2273 6861 3235 363a 6630        "sha256:f0
+00000a90: 6264 3266 3461 3538 6436 3636 3635 3030  bd2f4a58d6666500
+00000aa0: 3534 3262 3236 3335 3439 3738 3231 3861  542b26354978218a
+00000ab0: 3962 6162 6364 6339 3732 3732 3266 3462  9babcdc972722f4b
+00000ac0: 6639 3037 3739 3532 3435 3135 6633 220a  f90779524515f3".
+00000ad0: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00000ae0: 2020 2020 2020 2020 2020 2022 696e 6465             "inde
+00000af0: 7822 3a20 2270 7970 6922 2c0a 2020 2020  x": "pypi",.    
+00000b00: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+00000b10: 223a 2022 3d3d 3233 2e33 2e30 220a 2020  ": "==23.3.0".  
+00000b20: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000b30: 2022 626c 6561 6368 223a 207b 0a20 2020   "bleach": {.   
+00000b40: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
+00000b50: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00000b60: 2020 2020 2022 7368 6132 3536 3a31 6131       "sha256:1a1
+00000b70: 6138 3563 3135 3935 6530 3764 3864 6231  a85c1595e07d8db1
+00000b80: 3463 3566 3039 6630 3965 3634 3333 3530  4c5f09f09e643350
+00000b90: 3263 3531 6335 3935 3937 3065 6463 3039  2c51c595970edc09
+00000ba0: 3035 3531 6630 6462 3939 3431 3422 2c0a  0551f0db99414",.
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bc0: 2273 6861 3235 363a 3333 6331 3665 3333  "sha256:33c16e33
+00000bd0: 3533 6462 6431 3330 3238 6162 3437 3939  53dbd13028ab4799
+00000be0: 6130 6638 3961 3833 6631 3133 3430 3563  a0f89a83f113405c
+00000bf0: 3736 3665 3963 3132 3264 6638 6130 3666  766e9c122df8a06f
+00000c00: 3562 3835 6233 6634 220a 2020 2020 2020  5b85b3f4".      
+00000c10: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00000c20: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
+00000c30: 2270 7974 686f 6e5f 7665 7273 696f 6e20  "python_version 
+00000c40: 3e3d 2027 332e 3727 222c 0a20 2020 2020  >= '3.7'",.     
+00000c50: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
+00000c60: 3a20 223d 3d36 2e30 2e30 220a 2020 2020  : "==6.0.0".    
+00000c70: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000c80: 6361 6368 6574 6f6f 6c73 223a 207b 0a20  cachetools": {. 
+00000c90: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+00000ca0: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
+00000cb0: 2020 2020 2020 2022 7368 6132 3536 3a39         "sha256:9
+00000cc0: 3565 6636 3331 6565 6165 6131 3462 6132  5ef631eeaea14ba2
+00000cd0: 6533 3666 3036 3433 3766 3336 3436 3361  e36f06437f36463a
+00000ce0: 6163 3361 3039 3637 3939 6538 3736 6565  ac3a096799e876ee
+00000cf0: 3535 6535 6364 6363 6231 3032 3539 3022  55e5cdccb102590"
+00000d00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000d10: 2020 2273 6861 3235 363a 6463 6538 3366    "sha256:dce83f
+00000d20: 3264 3962 3465 3166 3733 3261 3863 6434  2d9b4e1f732a8cd4
+00000d30: 3461 6638 6538 6661 6232 6462 6534 3632  4af8e8fab2dbe462
+00000d40: 3031 3436 3766 6339 3862 3365 6638 6632  01467fc98b3ef8f2
+00000d50: 3639 3039 3262 6636 3262 220a 2020 2020  69092bf62b".    
+00000d60: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00000d70: 2020 2020 2020 2022 6d61 726b 6572 7322         "markers"
+00000d80: 3a20 2270 7974 686f 6e5f 7665 7273 696f  : "python_versio
+00000d90: 6e20 3e3d 2027 332e 3727 222c 0a20 2020  n >= '3.7'",.   
+00000da0: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
+00000db0: 6e22 3a20 223d 3d35 2e33 2e31 220a 2020  n": "==5.3.1".  
+00000dc0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000dd0: 2022 6365 7274 6966 6922 3a20 7b0a 2020   "certifi": {.  
+00000de0: 2020 2020 2020 2020 2020 2268 6173 6865            "hashe
+00000df0: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+00000e00: 2020 2020 2020 2273 6861 3235 363a 3066        "sha256:0f
+00000e10: 3064 3536 6463 3561 3661 6435 3666 6434  0d56dc5a6ad56fd4
+00000e20: 6261 3336 3438 3464 3663 6333 3434 3531  ba36484d6cc34451
+00000e30: 6531 6336 3534 3863 3631 6461 6164 3863  e1c6548c61daad8c
+00000e40: 3332 3031 3639 6639 3165 6464 6337 222c  320169f91eddc7",
+00000e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e60: 2022 7368 6132 3536 3a63 3663 3265 3938   "sha256:c6c2e98
+00000e70: 6635 6337 3836 3965 6663 6131 6638 3931  f5c7869efca1f891
+00000e80: 3666 6564 3232 3864 6439 3135 3339 6639  6fed228dd91539f9
+00000e90: 6631 6234 3434 6333 3134 6330 3665 6566  f1b444c314c06eef
+00000ea0: 3032 3938 3063 3731 3622 0a20 2020 2020  02980c716".     
+00000eb0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00000ec0: 2020 2020 2020 226d 6172 6b65 7273 223a        "markers":
+00000ed0: 2022 7079 7468 6f6e 5f76 6572 7369 6f6e   "python_version
+00000ee0: 203e 3d20 2733 2e36 2722 2c0a 2020 2020   >= '3.6'",.    
+00000ef0: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+00000f00: 223a 2022 3d3d 3230 3233 2e35 2e37 220a  ": "==2023.5.7".
+00000f10: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000f20: 2020 2022 6368 6172 6465 7422 3a20 7b0a     "chardet": {.
+00000f30: 2020 2020 2020 2020 2020 2020 2268 6173              "has
+00000f40: 6865 7322 3a20 5b0a 2020 2020 2020 2020  hes": [.        
+00000f50: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00000f60: 3064 3632 3731 3262 3935 3662 6331 3534  0d62712b956bc154
+00000f70: 6638 3566 6230 6132 3636 6532 6133 6335  f85fb0a266e2a3c5
+00000f80: 3931 3363 3239 3637 6530 3033 3438 3730  913c2967e0034870
+00000f90: 3162 3332 3431 3164 3664 6566 3331 6535  1b32411d6def31e5
+00000fa0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000fb0: 2020 2022 7368 6132 3536 3a33 3632 3737     "sha256:36277
+00000fc0: 3766 6230 3134 6166 3539 3661 6433 3133  7fb014af596ad313
+00000fd0: 3334 6664 6531 6538 6333 3237 6466 6462  34fde1e8c327dfdb
+00000fe0: 3037 3665 3139 3630 6431 3639 3436 3632  076e1960d1694662
+00000ff0: 6434 3661 3639 3137 6162 3922 0a20 2020  d46a6917ab9".   
+00001000: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00001010: 2020 2020 2020 2020 226d 6172 6b65 7273          "markers
+00001020: 223a 2022 7079 7468 6f6e 5f76 6572 7369  ": "python_versi
+00001030: 6f6e 203e 3d20 2733 2e37 2722 2c0a 2020  on >= '3.7'",.  
+00001040: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
+00001050: 6f6e 223a 2022 3d3d 352e 312e 3022 0a20  on": "==5.1.0". 
+00001060: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001070: 2020 2263 6861 7273 6574 2d6e 6f72 6d61    "charset-norma
+00001080: 6c69 7a65 7222 3a20 7b0a 2020 2020 2020  lizer": {.      
+00001090: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
+000010a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000010b0: 2020 2273 6861 3235 363a 3034 6166 6136    "sha256:04afa6
+000010c0: 3338 3765 3262 3238 3263 6637 3866 6633  387e2b282cf78ff3
+000010d0: 6462 6365 3230 6630 6363 3037 3163 3132  dbce20f0cc071c12
+000010e0: 6463 3866 3638 3562 6434 3039 3630 6363  dc8f685bd40960cc
+000010f0: 3638 3634 3463 6665 6136 222c 0a20 2020  68644cfea6",.   
+00001100: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00001110: 6132 3536 3a30 3465 6566 6365 6530 3935  a256:04eefcee095
+00001120: 6635 3865 6161 6265 3664 6333 6363 3232  f58eaabe6dc3cc22
+00001130: 3632 6633 6263 6437 3736 6432 6336 3730  62f3bcd776d2c670
+00001140: 3035 3838 3038 3934 6634 3437 6233 6632  05880894f447b3f2
+00001150: 6362 3963 3122 2c0a 2020 2020 2020 2020  cb9c1",.        
+00001160: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00001170: 3062 6536 3563 6366 3631 3863 3165 3761  0be65ccf618c1e7a
+00001180: 6339 6238 3439 6333 3135 6363 3265 3861  c9b849c315cc2e8a
+00001190: 3837 3531 6439 6366 6461 6134 3330 3237  8751d9cfdaa43027
+000011a0: 6434 6636 3632 3462 6435 3837 6162 3765  d4f6624bd587ab7e
+000011b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000011c0: 2020 2022 7368 6132 3536 3a30 6339 3566     "sha256:0c95f
+000011d0: 3132 6237 3436 3831 6539 6165 3132 3737  12b74681e9ae1277
+000011e0: 3238 6637 6535 3430 3963 6262 6566 3963  28f7e5409cbbef9c
+000011f0: 6439 3134 6435 3839 3665 6632 3338 6363  d914d5896ef238cc
+00001200: 3737 3962 3831 3532 3337 3322 2c0a 2020  779b8152373",.  
+00001210: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001220: 6861 3235 363a 3063 6135 3634 3630 3664  ha256:0ca564606d
+00001230: 3263 6161 6662 3061 6265 3664 3162 3533  2caafb0abe6d1b53
+00001240: 3131 6332 3634 3965 3830 3731 6562 3234  11c2649e8071eb24
+00001250: 3162 3264 3634 6537 3561 3064 3030 3635  1b2d64e75a0d0065
+00001260: 3130 3765 3632 222c 0a20 2020 2020 2020  107e62",.       
+00001270: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00001280: 3a31 3063 3933 3632 3864 3734 3937 6338  :10c93628d7497c8
+00001290: 3136 3836 6538 6535 6535 3537 6161 6661  1686e8e5e557aafa
+000012a0: 3738 6632 3330 6364 3965 3737 6464 3063  78f230cd9e77dd0c
+000012b0: 3430 3033 3265 6639 3063 3138 6632 3233  40032ef90c18f223
+000012c0: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+000012d0: 2020 2020 2273 6861 3235 363a 3131 6431      "sha256:11d1
+000012e0: 3137 6536 6336 3365 3866 3439 3534 3132  17e6c63e8f495412
+000012f0: 6433 3765 3764 6332 6532 6666 6630 3963  d37e7dc2e2fff09c
+00001300: 3334 6232 6430 3964 6265 3262 6565 3363  34b2d09dbe2bee3c
+00001310: 3632 3239 3537 3738 3138 6265 222c 0a20  6229577818be",. 
+00001320: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001330: 7368 6132 3536 3a31 3164 3362 6362 3762  sha256:11d3bcb7b
+00001340: 6533 3565 3762 3162 6261 3263 3233 6265  e35e7b1bba2c23be
+00001350: 6564 6163 3831 6565 3839 3361 6339 3837  edac81ee893ac987
+00001360: 3164 3062 6137 3965 6666 6337 6663 3031  1d0ba79effc7fc01
+00001370: 3136 3764 6236 6322 2c0a 2020 2020 2020  167db6c",.      
 00001380: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001390: 363a 3131 6433 6263 6237 6265 3335 6537  6:11d3bcb7be35e7
-000013a0: 6231 6262 6132 6332 3362 6565 6461 6338  b1bba2c23beedac8
-000013b0: 3165 6538 3933 6163 3938 3731 6430 6261  1ee893ac9871d0ba
-000013c0: 3739 6566 6663 3766 6330 3131 3637 6462  79effc7fc01167db
-000013d0: 3663 222c 0d0a 2020 2020 2020 2020 2020  6c",..          
-000013e0: 2020 2020 2020 2273 6861 3235 363a 3132        "sha256:12
-000013f0: 6132 6235 3631 6166 3132 3265 3364 3934  a2b561af122e3d94
-00001400: 6364 6239 3766 6536 6662 3262 6232 6238  cdb97fe6fb2bb2b8
-00001410: 3263 6566 3063 6463 6131 3331 3634 3666  2cef0cdca131646f
-00001420: 6462 3934 3061 3165 6461 3034 6630 222c  db940a1eda04f0",
-00001430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001440: 2020 2273 6861 3235 363a 3132 6431 6133    "sha256:12d1a3
-00001450: 3961 6136 6238 6336 6636 3234 3862 6235  9aa6b8c6f6248bb5
-00001460: 3435 3530 6566 6363 3163 3338 6365 3064  4550efcc1c38ce0d
-00001470: 3830 3936 6131 3436 3633 3866 6434 3733  8096a146638fd473
-00001480: 3865 3432 3238 3434 3438 222c 0d0a 2020  8e42284448",..  
-00001490: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000014a0: 6861 3235 363a 3134 3335 6165 3135 3130  ha256:1435ae1510
-000014b0: 3862 3163 6236 6666 6662 6365 6132 6166  8b1cb6fffbcea2af
-000014c0: 3364 3436 3836 3833 6237 6166 6564 3031  3d468683b7afed01
-000014d0: 3639 6164 3731 3834 3531 6638 6462 3564  69ad718451f8db5d
-000014e0: 3161 6666 3666 222c 0d0a 2020 2020 2020  1aff6f",..      
-000014f0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001500: 363a 3163 3630 6239 6332 3032 6430 3030  6:1c60b9c202d000
-00001510: 3532 3138 3363 3962 6538 3565 3565 6166  52183c9be85e5eaf
-00001520: 3138 6134 6164 6130 6134 3764 3138 3861  18a4ada0a47d188a
-00001530: 3833 6338 6635 6335 6232 3332 3532 6636  83c8f5c5b23252f6
-00001540: 3439 222c 0d0a 2020 2020 2020 2020 2020  49",..          
-00001550: 2020 2020 2020 2273 6861 3235 363a 3165        "sha256:1e
-00001560: 3866 6364 6438 6636 3732 6131 6334 6663  8fcdd8f672a1c4fc
-00001570: 3864 3062 6433 6132 6235 3736 6231 3532  8d0bd3a2b576b152
-00001580: 6432 6133 3439 3738 3264 3165 6230 6636  d2a349782d1eb0f6
-00001590: 6238 6535 3265 3939 3534 3733 3164 222c  b8e52e9954731d",
-000015a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000015b0: 2020 2273 6861 3235 363a 3230 3036 3465    "sha256:20064e
-000015c0: 6164 3037 3137 6366 3961 3733 6136 6431  ad0717cf9a73a6d1
-000015d0: 6537 3739 6232 3364 3134 3962 3533 6461  e779b23d149b53da
-000015e0: 6639 3731 3136 3932 3839 6564 3265 6434  f971169289ed2ed4
-000015f0: 3361 3731 6538 6433 6230 222c 0d0a 2020  3a71e8d3b0",..  
-00001600: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001610: 6861 3235 363a 3231 6661 3535 3839 3936  ha256:21fa558996
-00001620: 3738 3266 6332 3236 6235 3239 6664 6432  782fc226b529fdd2
-00001630: 6564 3738 3636 6332 6336 6563 3931 6365  ed7866c2c6ec91ce
-00001640: 6538 3237 3335 6339 3861 3139 3766 6165  e82735c98a197fae
-00001650: 3339 6637 3036 222c 0d0a 2020 2020 2020  39f706",..      
-00001660: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001670: 363a 3232 3930 3838 3931 6133 3830 6435  6:22908891a380d5
-00001680: 3037 3338 6531 6639 3738 3636 3735 3336  0738e1f978667536
-00001690: 6636 6336 6235 3236 6132 3036 3431 3536  f6c6b526a2064156
-000016a0: 3230 3364 3431 3866 3438 3536 6436 6538  203d418f4856d6e8
-000016b0: 3661 222c 0d0a 2020 2020 2020 2020 2020  6a",..          
-000016c0: 2020 2020 2020 2273 6861 3235 363a 3331        "sha256:31
-000016d0: 3630 6130 6664 3937 3534 6161 6237 6434  60a0fd9754aab7d4
-000016e0: 3766 3935 6136 6236 3361 6233 3535 3338  7f95a6b63ab35538
-000016f0: 3864 3839 3031 3633 6562 3033 6232 6432  8d890163eb03b2d2
-00001700: 6238 3761 6230 6133 3063 6661 3539 222c  b87ab0a30cfa59",
-00001710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001720: 2020 2273 6861 3235 363a 3332 3231 3032    "sha256:322102
-00001730: 6364 6631 6162 3638 3265 6363 3764 3962  cdf1ab682ecc7d9b
-00001740: 3163 3565 6564 3465 6335 3936 3537 6136  1c5eed4ec59657a6
-00001750: 3565 3163 3134 3661 3064 6133 3432 6237  5e1c146a0da342b7
-00001760: 3866 3431 3132 6462 3233 222c 0d0a 2020  8f4112db23",..  
-00001770: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001780: 6861 3235 363a 3334 6530 6132 6639 6333  ha256:34e0a2f9c3
-00001790: 3730 6562 3935 3539 3761 6165 3633 6266  70eb95597aae63bf
-000017a0: 3835 6562 3565 3936 3832 3664 3831 6533  85eb5e96826d81e3
-000017b0: 6463 6638 3862 3838 3836 3031 3239 3036  dcf88b8886012906
-000017c0: 6635 3039 6235 222c 0d0a 2020 2020 2020  f509b5",..      
-000017d0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000017e0: 363a 3335 3733 6433 3736 3435 3464 3935  6:3573d376454d95
-000017f0: 3635 3533 6333 3536 6466 3435 6262 3832  6553c356df45bb82
-00001800: 3432 3632 6333 3937 6336 6532 3663 6534  4262c397c6e26ce4
-00001810: 3365 3832 3033 6334 6335 3430 6565 3061  3e8203c4c540ee0a
-00001820: 6362 222c 0d0a 2020 2020 2020 2020 2020  cb",..          
-00001830: 2020 2020 2020 2273 6861 3235 363a 3337        "sha256:37
-00001840: 3437 3434 3362 3661 3930 3430 3031 3437  47443b6a90400147
-00001850: 3333 3730 6437 3831 3061 6131 3963 3361  3370d7810aa19c3a
-00001860: 3138 3063 6364 3532 6137 3135 3761 6163  180ccd52a7157aac
-00001870: 6332 3634 6135 6163 3739 3236 3565 222c  c264a5ac79265e",
-00001880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001890: 2020 2273 6861 3235 363a 3338 6538 3132    "sha256:38e812
-000018a0: 6131 3937 6266 3865 3731 6135 3966 6535  a197bf8e71a59fe5
-000018b0: 3562 3735 3761 3834 6331 6639 3436 6430  5b757a84c1f946d0
-000018c0: 6163 3131 3461 6361 6661 6166 6166 3231  ac114acafaafaf21
-000018d0: 3636 3761 3765 3136 3965 222c 0d0a 2020  667a7e169e",..  
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000018f0: 6861 3235 363a 3361 3036 6633 3263 3936  ha256:3a06f32c96
-00001900: 3334 6138 3730 3566 3463 6139 3934 3664  34a8705f4ca9946d
-00001910: 3636 3736 3039 6635 3263 6631 3330 6435  667609f52cf130d5
-00001920: 3534 3838 3831 3430 3166 3165 6232 6333  548881401f1eb2c3
-00001930: 3962 3165 3263 222c 0d0a 2020 2020 2020  9b1e2c",..      
-00001940: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001950: 363a 3361 3566 6337 3866 3965 3366 3530  6:3a5fc78f9e3f50
-00001960: 3161 3136 3134 6139 3866 3763 3534 6433  1a1614a98f7c54d3
-00001970: 3936 3966 3361 6439 6262 6138 6261 3364  969f3ad9bba8ba3d
-00001980: 3962 3433 3863 3362 6335 6430 3437 6464  9b438c3bc5d047dd
-00001990: 3238 222c 0d0a 2020 2020 2020 2020 2020  28",..          
-000019a0: 2020 2020 2020 2273 6861 3235 363a 3364        "sha256:3d
-000019b0: 3930 3938 6234 3739 6537 3863 3835 3038  9098b479e78c8508
-000019c0: 3063 3938 6531 6533 3566 6634 3062 3461  0c98e1e35ff40b4a
-000019d0: 3331 6438 3935 3331 3032 6262 3066 6437  31d8953102bb0fd7
-000019e0: 6431 6236 6638 6132 3131 3161 3364 222c  d1b6f8a2111a3d",
-000019f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001a00: 2020 2273 6861 3235 363a 3364 6335 6236    "sha256:3dc5b6
-00001a10: 6138 6563 6664 6335 3734 3861 3765 3432  a8ecfdc5748a7e42
-00001a20: 3937 3832 3539 3865 3466 3137 6566 3337  9782598e4f17ef37
-00001a30: 3865 3365 3237 3265 6562 3133 3430 6561  8e3e272eeb1340ea
-00001a40: 3537 6339 3130 3966 3431 222c 0d0a 2020  57c9109f41",..  
-00001a50: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001a60: 6861 3235 363a 3431 3535 6235 3161 6530  ha256:4155b51ae0
-00001a70: 3565 6434 3731 3939 6463 3562 3261 3465  5ed47199dc5b2a4e
-00001a80: 3632 6162 6363 6232 3734 6365 6536 6230  62abccb274cee6b0
-00001a90: 3164 6135 6238 3935 3039 3962 3631 6231  1da5b895099b61b1
-00001aa0: 3938 3239 3734 222c 0d0a 2020 2020 2020  982974",..      
-00001ab0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001ac0: 363a 3439 3931 3966 3834 3030 6235 6534  6:49919f8400b5e4
-00001ad0: 3965 3936 3166 3332 3063 3733 3533 3838  9e961f320c735388
-00001ae0: 6565 3638 3661 3632 3332 3765 3737 3366  ee686a62327e773f
-00001af0: 6135 6233 6365 3637 3231 6637 6537 3835  a5b3ce6721f7e785
-00001b00: 6365 222c 0d0a 2020 2020 2020 2020 2020  ce",..          
-00001b10: 2020 2020 2020 2273 6861 3235 363a 3533        "sha256:53
-00001b20: 6430 6133 6661 3566 3861 6639 3861 3165  d0a3fa5f8af98a1e
-00001b30: 3236 3164 6536 6133 3934 3363 6136 3331  261de6a3943ca631
-00001b40: 6335 3236 3633 3565 6235 3831 3761 3837  c526635eb5817a87
-00001b50: 6135 3964 3961 3537 6562 6634 3866 222c  a59d9a57ebf48f",
-00001b60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001b70: 2020 2273 6861 3235 363a 3566 3030 3835    "sha256:5f0085
-00001b80: 3235 6530 3239 3038 6232 3065 3034 3730  25e02908b20e0470
-00001b90: 3761 3466 3730 3463 6432 3836 6439 3437  7a4f704cd286d947
-00001ba0: 3138 6634 3862 6233 3365 6464 6463 3764  18f48bb33edddc7d
-00001bb0: 3762 3538 3464 6464 6331 222c 0d0a 2020  7b584dddc1",..  
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001bd0: 6861 3235 363a 3632 3863 3938 3561 6662  ha256:628c985afb
-00001be0: 3263 3764 3237 6134 3830 3062 6662 3630  2c7d27a4800bfb60
-00001bf0: 3965 3033 3938 3561 6165 6362 3432 6639  9e03985aaecb42f9
-00001c00: 3535 3034 3939 3537 3831 3465 3034 3931  55049957814e0491
-00001c10: 6434 3030 3664 222c 0d0a 2020 2020 2020  d4006d",..      
-00001c20: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001c30: 363a 3635 6564 3932 3366 3834 6136 3834  6:65ed923f84a684
-00001c40: 3464 6535 6664 3239 3732 3662 3838 3865  4de5fd29726b888e
-00001c50: 3538 6336 3238 3230 6530 3736 3962 3736  58c62820e0769b76
-00001c60: 3536 3534 3830 6531 6664 6333 6430 3632  565480e1fdc3d062
-00001c70: 6638 222c 0d0a 2020 2020 2020 2020 2020  f8",..          
-00001c80: 2020 2020 2020 2273 6861 3235 363a 3637        "sha256:67
-00001c90: 3334 6536 3036 3335 3538 3334 6631 3334  34e606355834f134
-00001ca0: 3435 6236 6164 6333 3862 3533 6330 6664  45b6adc38b53c0fd
-00001cb0: 3435 6631 6135 3661 3962 6130 3663 3230  45f1a56a9ba06c20
-00001cc0: 3538 6638 3638 3933 6165 3830 3137 222c  58f86893ae8017",
-00001cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001ce0: 2020 2273 6861 3235 363a 3662 6166 3062    "sha256:6baf0b
-00001cf0: 6166 3064 3564 3236 3566 6137 3934 3466  af0d5d265fa7944f
-00001d00: 6562 3966 3734 3531 6363 3331 3662 6665  eb9f7451cc316bfe
-00001d10: 3330 6538 6466 3161 3631 6231 6262 3038  30e8df1a61b1bb08
-00001d20: 3537 3763 3535 3466 3331 222c 0d0a 2020  577c554f31",..  
-00001d30: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001d40: 6861 3235 363a 3666 3466 3436 3638 6531  ha256:6f4f4668e1
-00001d50: 3833 3138 3530 6562 6363 3266 6430 6231  831850ebcc2fd0b1
-00001d60: 6364 3131 3732 3139 3437 6236 6463 3763  cd11721947b6dc7c
-00001d70: 3030 6266 3163 3662 6433 6339 3239 6165  00bf1c6bd3c929ae
-00001d80: 3134 6632 6337 222c 0d0a 2020 2020 2020  14f2c7",..      
-00001d90: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001da0: 363a 3666 3563 3265 3762 6338 6134 6266  6:6f5c2e7bc8a4bf
-00001db0: 3763 3432 3635 3939 3736 3562 3162 6433  7c426599765b1bd3
-00001dc0: 3332 3137 6563 3834 3032 3330 3333 3637  3217ec8402303367
-00001dd0: 3263 3165 3961 3862 3335 6561 6561 6161  2c1e9a8b35eaeaaa
-00001de0: 6638 222c 0d0a 2020 2020 2020 2020 2020  f8",..          
-00001df0: 2020 2020 2020 2273 6861 3235 363a 3666        "sha256:6f
-00001e00: 3663 3761 3861 3537 6539 3430 3563 6164  6c7a8a57e9405cad
-00001e10: 3734 3835 6634 6339 6433 3137 3261 6534  7485f4c9d3172ae4
-00001e20: 3836 6366 6566 3133 3434 6235 6464 6438  86cfef1344b5ddd8
-00001e30: 6535 3233 3935 3832 6437 3335 3565 222c  e5239582d7355e",
-00001e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001e50: 2020 2273 6861 3235 363a 3733 3831 6336    "sha256:7381c6
-00001e60: 3665 3035 3631 6335 3735 3766 6665 3631  6e0561c5757ffe61
-00001e70: 3661 6638 3639 6239 3136 6338 6234 6534  6af869b916c8b4e4
-00001e80: 3262 3336 3761 6232 3966 6564 6339 3834  2b367ab29fedc984
-00001e90: 3831 6431 6537 3465 3134 222c 0d0a 2020  81d1e74e14",..  
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001eb0: 6861 3235 363a 3733 6463 3033 6136 6137  ha256:73dc03a6a7
-00001ec0: 6533 3062 3765 6463 3562 3031 6236 3031  e30b7edc5b01b601
-00001ed0: 6535 3365 3766 6339 3234 6230 3465 3138  e53e7fc924b04e18
-00001ee0: 3335 6538 6534 3037 6331 3263 3033 3765  35e8e407c12c037e
-00001ef0: 3831 6164 6264 222c 0d0a 2020 2020 2020  81adbd",..      
-00001f00: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00001f10: 363a 3734 6462 3030 3532 6439 3835 6366  6:74db0052d985cf
-00001f20: 3337 6661 3131 3138 3238 6430 6464 3233  37fa111828d0dd23
-00001f30: 3037 3736 6163 3939 6337 3430 6531 6137  0776ac99c740e1a7
-00001f40: 3538 6164 3939 3039 3462 6534 6631 3830  58ad99094be4f180
-00001f50: 3364 222c 0d0a 2020 2020 2020 2020 2020  3d",..          
-00001f60: 2020 2020 2020 2273 6861 3235 363a 3735        "sha256:75
-00001f70: 6632 3536 3862 3431 3839 6464 6131 6335  f2568b4189dda1c5
-00001f80: 3637 3333 3962 3438 6362 6134 6163 3733  67339b48cba4ac73
-00001f90: 3834 6163 6362 3963 3261 3765 6436 3535  84accb9c2a7ed655
-00001fa0: 6364 3836 6230 3430 3535 6337 3935 222c  cd86b04055c795",
-00001fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001fc0: 2020 2273 6861 3235 363a 3738 6361 6364    "sha256:78cacd
-00001fd0: 3033 6537 3964 3030 3964 3935 3633 3565  03e79d009d95635e
-00001fe0: 3764 3666 6631 3263 3231 6562 3839 6238  7d6ff12c21eb89b8
-00001ff0: 3934 6333 3534 6264 3262 3265 6430 6234  94c354bd2b2ed0b4
-00002000: 3736 3333 3733 3639 3362 222c 0d0a 2020  763373693b",..  
-00002010: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002020: 6861 3235 363a 3830 6431 3534 3364 3538  ha256:80d1543d58
-00002030: 6264 3364 3663 3237 3162 3636 6162 6634  bd3d6c271b66abf4
-00002040: 3534 6434 3337 6134 3338 6466 6630 3163  54d437a438dff01c
-00002050: 3365 3632 6664 6263 6436 3866 3261 3131  3e62fdbcd68f2a11
-00002060: 3331 3064 3462 222c 0d0a 2020 2020 2020  310d4b",..      
-00002070: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00002080: 363a 3833 3064 3239 3438 6135 6563 3337  6:830d2948a5ec37
-00002090: 6333 3836 6433 3137 3063 3438 3330 3633  c386d3170c483063
-000020a0: 3739 3864 3738 3739 3033 3734 3932 3534  798d787903749254
-000020b0: 3066 3130 6134 3735 6533 6664 3666 3234  0f10a475e3fd6f24
-000020c0: 3462 222c 0d0a 2020 2020 2020 2020 2020  4b",..          
-000020d0: 2020 2020 2020 2273 6861 3235 363a 3839        "sha256:89
-000020e0: 3163 6639 6234 3837 3736 6235 6336 3163  1cf9b48776b5c61c
-000020f0: 3730 3062 3535 6135 3938 3632 3166 6462  700b55a598621fdb
-00002100: 3762 3165 3330 3161 3535 3033 3635 3537  7b1e301a55036557
-00002110: 3165 3936 3234 6632 3730 6332 3033 222c  1e9624f270c203",
-00002120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002130: 2020 2273 6861 3235 363a 3866 3235 6531    "sha256:8f25e1
-00002140: 3761 6233 3033 3962 3035 6637 3632 6230  7ab3039b05f762b0
-00002150: 6135 3561 6530 6233 3633 3262 3265 3037  a55ae0b3632b2e07
-00002160: 3364 3963 3866 6338 3865 3839 6163 6133  3d9c8fc88e89aca3
-00002170: 3161 3631 3938 6538 3866 222c 0d0a 2020  1a6198e88f",..  
-00002180: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002190: 6861 3235 363a 3961 3332 3637 3632 3038  ha256:9a32676208
-000021a0: 3636 6339 6431 3762 3935 3961 3834 6464  66c9d17b959a84dd
-000021b0: 3062 6432 6434 3537 3139 6238 3137 3234  0bd2d45719b81724
-000021c0: 3565 3439 3337 3165 6164 3739 6564 3466  5e49371ead79ed4f
-000021d0: 3731 3064 3139 222c 0d0a 2020 2020 2020  710d19",..      
-000021e0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000021f0: 363a 6130 3466 3836 6634 3161 3839 3136  6:a04f86f41a8916
-00002200: 6665 3435 6163 3530 3234 6563 3437 3766  fe45ac5024ec477f
-00002210: 3431 6638 3836 6233 6334 3335 6461 3264  41f886b3c435da2d
-00002220: 3465 3364 3237 3039 6232 3261 6230 3261  4e3d2709b22ab02a
-00002230: 6631 222c 0d0a 2020 2020 2020 2020 2020  f1",..          
-00002240: 2020 2020 2020 2273 6861 3235 363a 6161        "sha256:aa
-00002250: 6635 3361 3663 6562 6164 3065 6165 3537  f53a6cebad0eae57
-00002260: 3866 3036 3263 3764 3436 3231 3535 6561  8f062c7d462155ea
-00002270: 6461 3963 3137 3262 6438 6334 6432 3530  da9c172bd8c4d250
-00002280: 6238 6331 6438 6562 3766 3931 3661 222c  b8c1d8eb7f916a",
-00002290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000022a0: 2020 2273 6861 3235 363a 6162 6331 3138    "sha256:abc118
-000022b0: 3564 3739 6634 3763 3061 3761 6166 3765  5d79f47c0a7aaf7e
-000022c0: 3234 3132 6130 6562 3263 3033 6237 3234  2412a0eb2c03b724
-000022d0: 3538 3131 3339 3139 3364 3264 3832 6233  581139193d2d82b3
-000022e0: 6164 3863 6262 3030 6163 222c 0d0a 2020  ad8cbb00ac",..  
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002300: 6861 3235 363a 6163 3061 6136 6364 3533  ha256:ac0aa6cd53
-00002310: 6162 3961 3331 6433 3937 6638 3330 3366  ab9a31d397f8303f
-00002320: 3932 6334 3266 3533 3436 3933 3532 3866  92c42f534693528f
-00002330: 6166 6264 6239 3937 6338 3262 6165 3665  afbdb997c82bae6e
-00002340: 3437 3761 6439 222c 0d0a 2020 2020 2020  477ad9",..      
-00002350: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00002360: 363a 6163 3337 3735 6533 3331 3136 3631  6:ac3775e3311661
-00002370: 6434 6164 6163 6533 3639 3761 3532 6163  d4adace3697a52ac
-00002380: 3062 6162 3137 6564 6431 3636 3038 3764  0bab17edd166087d
-00002390: 3439 3362 3532 6434 6634 6635 3533 6639  493b52d4f4f553f9
-000023a0: 6630 222c 0d0a 2020 2020 2020 2020 2020  f0",..          
-000023b0: 2020 2020 2020 2273 6861 3235 363a 6230        "sha256:b0
-000023c0: 3666 3064 3362 6630 3435 3135 3864 3266  6f0d3bf045158d2f
-000023d0: 6238 3833 3763 3537 3835 6665 3966 6639  b8837c5785fe9ff9
-000023e0: 6238 6339 3333 3538 6265 3634 3436 3161  b8c93358be64461a
-000023f0: 3130 3839 6635 6461 3938 3331 3337 222c  1089f5da983137",
-00002400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002410: 2020 2273 6861 3235 363a 6231 3136 3530    "sha256:b11650
-00002420: 3230 3837 6365 3861 3662 3761 3566 3138  2087ce8a6b7a5f18
-00002430: 3134 3536 3863 6362 6430 6539 6636 6366  14568ccbd0e9f6cf
-00002440: 6439 3939 3438 6161 3539 6230 6532 3431  d99948aa59b0e241
-00002450: 6463 3537 6366 3733 3966 222c 0d0a 2020  dc57cf739f",..  
-00002460: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002470: 6861 3235 363a 6238 3266 6162 3738 6530  ha256:b82fab78e0
-00002480: 6231 3332 3965 3138 3361 3635 3236 3035  b1329e183a652605
-00002490: 3831 6465 3433 3735 6636 3139 3136 3734  81de4375f6191674
-000024a0: 3738 6464 6461 6235 3130 6336 6336 6662  78dddab510c6c6fb
-000024b0: 3034 6439 6236 222c 0d0a 2020 2020 2020  04d9b6",..      
-000024c0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000024d0: 363a 6264 3731 3633 3138 3231 3333 6330  6:bd7163182133c0
-000024e0: 6337 3730 3162 3235 6536 3034 6366 3136  c7701b25e604cf16
-000024f0: 3131 6330 6438 3737 3132 6535 3665 3838  11c0d87712e56e88
-00002500: 6537 6565 3564 3732 6465 6162 3365 3736  e7ee5d72deab3e76
-00002510: 6235 222c 0d0a 2020 2020 2020 2020 2020  b5",..          
-00002520: 2020 2020 2020 2273 6861 3235 363a 6333        "sha256:c3
-00002530: 3662 6362 6330 6435 3137 3461 3830 6436  6bcbc0d5174a80d6
-00002540: 6363 6366 3433 6130 6563 6163 6134 3465  cccf43a0ecaca44e
-00002550: 3831 6432 3562 6534 6237 6639 3066 3065  81d25be4b7f90f0e
-00002560: 6437 6263 6662 6235 6130 3039 3039 222c  d7bcfbb5a00909",
-00002570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002580: 2020 2273 6861 3235 363a 6333 6166 3865    "sha256:c3af8e
-00002590: 3066 3037 3339 3964 3331 3736 6231 3739  0f07399d3176b179
-000025a0: 6632 6532 3633 3463 3363 6539 6331 3330  f2e2634c3ce9c130
-000025b0: 3133 3739 6136 6238 6339 6339 6165 6563  1379a6b8c9c9aeec
-000025c0: 6434 3831 6461 3439 3466 222c 0d0a 2020  d481da494f",..  
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000025e0: 6861 3235 363a 6338 3431 3332 6135 3463  ha256:c84132a54c
-000025f0: 3735 3066 6461 3537 3732 3964 3165 3235  750fda57729d1e25
-00002600: 3939 6262 3539 3866 3566 6130 3334 3430  99bb598f5fa03440
-00002610: 3835 6462 6465 3530 3033 6261 3432 3961  85dbde5003ba429a
-00002620: 3437 3938 6330 222c 0d0a 2020 2020 2020  4798c0",..      
-00002630: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00002640: 363a 6362 3762 3261 6230 3138 3838 3239  6:cb7b2ab0188829
-00002650: 3539 3362 3964 6536 3436 3534 3531 3735  593b9de646545175
-00002660: 3534 3761 3730 6439 6136 6532 6236 3362  547a70d9a6e2b63b
-00002670: 6632 6364 3837 6130 6133 3931 3539 3933  f2cd87a0a3915993
-00002680: 3234 222c 0d0a 2020 2020 2020 2020 2020  24",..          
-00002690: 2020 2020 2020 2273 6861 3235 363a 6363        "sha256:cc
-000026a0: 6134 6465 6635 3736 6634 3761 3039 6139  a4def576f47a09a9
-000026b0: 3433 3636 3662 3866 3832 3936 3036 6263  43666b8f829606bc
-000026c0: 6231 3765 3262 6332 6435 3931 3161 3436  b17e2bc2d5911a46
-000026d0: 6338 6638 6461 3435 6635 3637 3535 222c  c8f8da45f56755",
-000026e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000026f0: 2020 2273 6861 3235 363a 6366 3635 3131    "sha256:cf6511
-00002700: 6566 6134 3830 3162 3962 3338 6463 3535  efa4801b9b38dc55
-00002710: 3436 6437 3534 3764 3562 3563 3665 6634  46d7547d5b5c6ef4
-00002720: 6230 3831 6336 3062 3233 6534 6439 3431  b081c60b23e4d941
-00002730: 6430 6562 6139 6362 6562 222c 0d0a 2020  d0eba9cbeb",..  
-00002740: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002750: 6861 3235 363a 6431 3666 6435 3235 3266  ha256:d16fd5252f
-00002760: 3838 3365 6230 3734 6361 3535 6362 3632  883eb074ca55cb62
-00002770: 3262 6330 6265 6534 3962 3937 3961 6534  2bc0bee49b979ae4
-00002780: 6538 3633 3966 6666 3663 6133 6666 3434  e8639fff6ca3ff44
-00002790: 6639 6638 3534 222c 0d0a 2020 2020 2020  f9f854",..      
-000027a0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000027b0: 363a 6432 3638 3666 3931 3631 3166 3965  6:d2686f91611f9e
-000027c0: 3137 6634 3534 3864 6266 3035 3065 3735  17f4548dbf050e75
-000027d0: 6230 3739 6262 6332 6138 3262 6535 3635  b079bbc2a82be565
-000027e0: 3833 3262 6338 6561 3930 3437 6236 3163  832bc8ea9047b61c
-000027f0: 3863 222c 0d0a 2020 2020 2020 2020 2020  8c",..          
-00002800: 2020 2020 2020 2273 6861 3235 363a 6437        "sha256:d7
-00002810: 6663 3366 6361 3031 6461 3138 6662 6162  fc3fca01da18fbab
-00002820: 6534 3632 3564 3634 6262 3631 3262 3533  e4625d64bb612b53
-00002830: 3335 3333 6564 3130 3034 3561 3261 6333  3533ed10045a2ac3
-00002840: 6464 3139 3462 6661 3635 3662 3630 222c  dd194bfa656b60",
-00002850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002860: 2020 2273 6861 3235 363a 6464 3536 3533    "sha256:dd5653
-00002870: 6536 3762 3134 3935 3033 6336 3863 3430  e67b149503c68c40
-00002880: 3138 6266 3037 6534 3265 6565 6436 6234  18bf07e42eeed6b4
-00002890: 6539 3536 6232 3463 3030 6363 6466 3933  e956b24c00ccdf93
-000028a0: 6163 3739 6364 6666 3834 222c 0d0a 2020  ac79cdff84",..  
-000028b0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000028c0: 6861 3235 363a 6465 3536 3935 6136 6631  ha256:de5695a6f1
-000028d0: 6438 3334 3062 3132 6135 6436 6434 3438  d8340b12a5d6d448
-000028e0: 3432 3930 6565 3734 6436 3165 3436 3763  4290ee74d61e467c
-000028f0: 3339 6666 3033 6233 3965 3330 6466 3632  39ff03b39e30df62
-00002900: 6366 3833 6130 222c 0d0a 2020 2020 2020  cf83a0",..      
-00002910: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00002920: 363a 6530 6163 3839 3539 6339 3239 3539  6:e0ac8959c92959
-00002930: 3366 6565 3338 6461 3163 3262 3634 6565  3fee38da1c2b64ee
-00002940: 3937 3738 3733 3363 6466 3033 6334 3832  9778733cdf03c482
-00002950: 6339 6666 3164 3530 3862 3662 3539 3362  c9ff1d508b6b593b
-00002960: 3262 222c 0d0a 2020 2020 2020 2020 2020  2b",..          
-00002970: 2020 2020 2020 2273 6861 3235 363a 6531        "sha256:e1
-00002980: 6232 3565 3361 6436 6339 3039 6633 3938  b25e3ad6c909f398
-00002990: 6466 3839 3231 3738 3064 3661 3364 3132  df8921780d6a3d12
-000029a0: 3064 3863 3039 3436 3637 3230 3232 3666  0d8c09466720226f
-000029b0: 6336 3231 3630 3562 3666 3932 6231 222c  c621605b6f92b1",
-000029c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000029d0: 2020 2273 6861 3235 363a 6536 3333 3934    "sha256:e63394
-000029e0: 3066 3238 6331 6539 3133 3631 3566 6436  0f28c1e913615fd6
-000029f0: 3234 6663 6464 3732 6664 6261 3830 3762  24fcdd72fdba807b
-00002a00: 6635 3365 6136 3932 3564 3661 3538 3865  f53ea6925d6a588e
-00002a10: 3834 6531 3135 3135 3331 222c 0d0a 2020  84e1151531",..  
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002a30: 6861 3235 363a 6538 3964 6632 3935 3865  ha256:e89df2958e
-00002a40: 3531 3539 6238 3131 6166 3966 6630 6639  5159b811af9ff0f9
-00002a50: 3236 3134 6461 6266 3466 6636 3137 6330  2614dabf4ff617c0
-00002a60: 3361 3463 3163 3666 6635 3362 6631 6333  3a4c1c6ff53bf1c3
-00002a70: 3939 6530 6531 222c 0d0a 2020 2020 2020  99e0e1",..      
-00002a80: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00002a90: 363a 6561 3966 3963 3630 3334 6561 3264  6:ea9f9c6034ea2d
-00002aa0: 3933 6439 3134 3738 3138 6631 3763 3261  93d9147818f17c2a
-00002ab0: 3038 3630 6434 3162 3731 6333 3862 3963  0860d41b71c38b9c
-00002ac0: 6534 6435 3566 3231 6236 6639 3136 3561  e4d55f21b6f9165a
-00002ad0: 3131 222c 0d0a 2020 2020 2020 2020 2020  11",..          
-00002ae0: 2020 2020 2020 2273 6861 3235 363a 6636        "sha256:f6
-00002af0: 3435 6361 6166 3030 3038 6261 6366 3334  45caaf0008bacf34
-00002b00: 3938 3735 6139 3734 3232 3066 3166 3164  9875a974220f1f1d
-00002b10: 6133 3439 6335 6462 6537 6334 6563 3933  a349c5dbe7c4ec93
-00002b20: 3034 3863 6463 3738 3561 3333 3236 222c  048cdc785a3326",
-00002b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002b40: 2020 2273 6861 3235 363a 6638 3330 3334    "sha256:f83034
-00002b50: 3134 6337 6230 3366 3739 3433 3437 6164  14c7b03f794347ad
-00002b60: 3036 3263 3035 3136 6365 6530 6531 3566  062c0516cee0e15f
-00002b70: 3761 3631 3261 6264 3063 6531 6532 3563  7a612abd0ce1e25c
-00002b80: 6166 3663 6562 3437 6466 222c 0d0a 2020  af6ceb47df",..  
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002ba0: 6861 3235 363a 6663 6136 3261 3833 3031  ha256:fca62a8301
-00002bb0: 6236 3035 6239 3534 6164 3265 3963 3336  b605b954ad2e9c36
-00002bc0: 3636 6639 6439 3766 3633 3837 3261 6134  66f9d97f63872aa4
-00002bd0: 6566 6361 6535 3439 3262 6163 6132 3035  efcae5492baca205
-00002be0: 3662 3734 6162 220d 0a20 2020 2020 2020  6b74ab"..       
-00002bf0: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-00002c00: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
-00002c10: 2270 7974 686f 6e5f 6675 6c6c 5f76 6572  "python_full_ver
-00002c20: 7369 6f6e 203e 3d20 2733 2e37 2e30 2722  sion >= '3.7.0'"
-00002c30: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002c40: 7665 7273 696f 6e22 3a20 223d 3d33 2e31  version": "==3.1
-00002c50: 2e30 220d 0a20 2020 2020 2020 207d 2c0d  .0"..        },.
-00002c60: 0a20 2020 2020 2020 2022 636c 6963 6b22  .        "click"
-00002c70: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00002c80: 2022 6861 7368 6573 223a 205b 0d0a 2020   "hashes": [..  
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002ca0: 6861 3235 363a 3736 3832 6463 3861 6662  ha256:7682dc8afb
-00002cb0: 3330 3239 3730 3031 3637 3435 3735 6561  30297001674575ea
-00002cc0: 3030 6431 3831 3464 3830 3864 3661 3336  00d1814d808d6a36
-00002cd0: 6166 3431 3561 3832 6264 3438 3164 3337  af415a82bd481d37
-00002ce0: 6261 3762 3865 222c 0d0a 2020 2020 2020  ba7b8e",..      
-00002cf0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00002d00: 363a 6262 3464 3831 3333 6362 3135 6136  6:bb4d8133cb15a6
-00002d10: 3039 6634 3465 3832 3133 6439 6233 3931  09f44e8213d9b391
-00002d20: 6230 3830 3937 3935 3036 3239 3133 6233  b0809795062913b3
-00002d30: 3833 6336 3262 6530 6565 3935 6231 6462  83c62be0ee95b1db
-00002d40: 3438 220d 0a20 2020 2020 2020 2020 2020  48"..           
-00002d50: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
-00002d60: 2022 6d61 726b 6572 7322 3a20 2270 7974   "markers": "pyt
-00002d70: 686f 6e5f 7665 7273 696f 6e20 3e3d 2027  hon_version >= '
-00002d80: 332e 3727 222c 0d0a 2020 2020 2020 2020  3.7'",..        
-00002d90: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
-00002da0: 3d3d 382e 312e 3322 0d0a 2020 2020 2020  ==8.1.3"..      
-00002db0: 2020 7d2c 0d0a 2020 2020 2020 2020 2263    },..        "c
-00002dc0: 6f6c 6f72 616d 6122 3a20 7b0d 0a20 2020  olorama": {..   
-00002dd0: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
-00002de0: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00002df0: 2020 2020 2020 2273 6861 3235 363a 3038        "sha256:08
-00002e00: 3639 3566 3563 6237 6564 3665 3035 3331  695f5cb7ed6e0531
-00002e10: 6132 3035 3732 3639 3732 3937 3237 3363  a20572697297273c
-00002e20: 3437 6238 6361 6535 6136 3366 6663 3664  47b8cae5a63ffc6d
-00002e30: 3665 6435 6332 3031 6265 3665 3434 222c  6ed5c201be6e44",
-00002e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e50: 2020 2273 6861 3235 363a 3466 3164 3939    "sha256:4f1d99
-00002e60: 3931 6635 6163 6330 6361 3131 3966 3964  91f5acc0ca119f9d
-00002e70: 3434 3336 3230 6237 3766 3964 3662 3333  443620b77f9d6b33
-00002e80: 3730 3365 3531 3031 3163 3136 6261 6635  703e51011c16baf5
-00002e90: 3761 6662 3238 3566 6336 220d 0a20 2020  7afb285fc6"..   
-00002ea0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00002eb0: 2020 2020 2020 2020 2022 6d61 726b 6572           "marker
-00002ec0: 7322 3a20 2273 7973 5f70 6c61 7466 6f72  s": "sys_platfor
-00002ed0: 6d20 3d3d 2027 7769 6e33 3227 222c 0d0a  m == 'win32'",..
-00002ee0: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
-00002ef0: 7369 6f6e 223a 2022 3d3d 302e 342e 3622  sion": "==0.4.6"
-00002f00: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00002f10: 2020 2020 2020 2263 6f76 6572 6167 6522        "coverage"
-00002f20: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00002f30: 2022 6861 7368 6573 223a 205b 0d0a 2020   "hashes": [..  
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002f50: 6861 3235 363a 3036 6139 6132 6265 3062  ha256:06a9a2be0b
-00002f60: 3562 3537 3663 3366 3138 6631 6132 3431  5b576c3f18f1a241
-00002f70: 6630 3437 3335 3735 6334 6132 3630 3231  f0473575c4a26021
-00002f80: 6235 3262 3261 3835 3236 3361 3030 6630  b52b2a85263a00f0
-00002f90: 3334 6435 3166 222c 0d0a 2020 2020 2020  34d51f",..      
+00001390: 363a 3132 6132 6235 3631 6166 3132 3265  6:12a2b561af122e
+000013a0: 3364 3934 6364 6239 3766 6536 6662 3262  3d94cdb97fe6fb2b
+000013b0: 6232 6238 3263 6566 3063 6463 6131 3331  b2b82cef0cdca131
+000013c0: 3634 3666 6462 3934 3061 3165 6461 3034  646fdb940a1eda04
+000013d0: 6630 222c 0a20 2020 2020 2020 2020 2020  f0",.           
+000013e0: 2020 2020 2022 7368 6132 3536 3a31 3264       "sha256:12d
+000013f0: 3161 3339 6161 3662 3863 3666 3632 3438  1a39aa6b8c6f6248
+00001400: 6262 3534 3535 3065 6663 6331 6333 3863  bb54550efcc1c38c
+00001410: 6530 6438 3039 3661 3134 3636 3338 6664  e0d8096a146638fd
+00001420: 3437 3338 6534 3232 3834 3434 3822 2c0a  4738e42284448",.
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2273 6861 3235 363a 3134 3335 6165 3135  "sha256:1435ae15
+00001450: 3130 3862 3163 6236 6666 6662 6365 6132  108b1cb6fffbcea2
+00001460: 6166 3364 3436 3836 3833 6237 6166 6564  af3d468683b7afed
+00001470: 3031 3639 6164 3731 3834 3531 6638 6462  0169ad718451f8db
+00001480: 3564 3161 6666 3666 222c 0a20 2020 2020  5d1aff6f",.     
+00001490: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+000014a0: 3536 3a31 6336 3062 3963 3230 3264 3030  56:1c60b9c202d00
+000014b0: 3035 3231 3833 6339 6265 3835 6535 6561  052183c9be85e5ea
+000014c0: 6631 3861 3461 6461 3061 3437 6431 3838  f18a4ada0a47d188
+000014d0: 6138 3363 3866 3563 3562 3233 3235 3266  a83c8f5c5b23252f
+000014e0: 3634 3922 2c0a 2020 2020 2020 2020 2020  649",.          
+000014f0: 2020 2020 2020 2273 6861 3235 363a 3165        "sha256:1e
+00001500: 3866 6364 6438 6636 3732 6131 6334 6663  8fcdd8f672a1c4fc
+00001510: 3864 3062 6433 6132 6235 3736 6231 3532  8d0bd3a2b576b152
+00001520: 6432 6133 3439 3738 3264 3165 6230 6636  d2a349782d1eb0f6
+00001530: 6238 6535 3265 3939 3534 3733 3164 222c  b8e52e9954731d",
+00001540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001550: 2022 7368 6132 3536 3a32 3030 3634 6561   "sha256:20064ea
+00001560: 6430 3731 3763 6639 6137 3361 3664 3165  d0717cf9a73a6d1e
+00001570: 3737 3962 3233 6431 3439 6235 3364 6166  779b23d149b53daf
+00001580: 3937 3131 3639 3238 3965 6432 6564 3433  971169289ed2ed43
+00001590: 6137 3165 3864 3362 3022 2c0a 2020 2020  a71e8d3b0",.    
+000015a0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+000015b0: 3235 363a 3231 6661 3535 3839 3936 3738  256:21fa55899678
+000015c0: 3266 6332 3236 6235 3239 6664 6432 6564  2fc226b529fdd2ed
+000015d0: 3738 3636 6332 6336 6563 3931 6365 6538  7866c2c6ec91cee8
+000015e0: 3237 3335 6339 3861 3139 3766 6165 3339  2735c98a197fae39
+000015f0: 6637 3036 222c 0a20 2020 2020 2020 2020  f706",.         
+00001600: 2020 2020 2020 2022 7368 6132 3536 3a32         "sha256:2
+00001610: 3239 3038 3839 3161 3338 3064 3530 3733  2908891a380d5073
+00001620: 3865 3166 3937 3836 3637 3533 3666 3663  8e1f978667536f6c
+00001630: 3662 3532 3661 3230 3634 3135 3632 3033  6b526a2064156203
+00001640: 6434 3138 6634 3835 3664 3665 3836 6122  d418f4856d6e86a"
+00001650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001660: 2020 2273 6861 3235 363a 3331 3630 6130    "sha256:3160a0
+00001670: 6664 3937 3534 6161 6237 6434 3766 3935  fd9754aab7d47f95
+00001680: 6136 6236 3361 6233 3535 3338 3864 3839  a6b63ab355388d89
+00001690: 3031 3633 6562 3033 6232 6432 6238 3761  0163eb03b2d2b87a
+000016a0: 6230 6133 3063 6661 3539 222c 0a20 2020  b0a30cfa59",.   
+000016b0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+000016c0: 6132 3536 3a33 3232 3130 3263 6466 3161  a256:322102cdf1a
+000016d0: 6236 3832 6563 6337 6439 6231 6335 6565  b682ecc7d9b1c5ee
+000016e0: 6434 6563 3539 3635 3761 3635 6531 6331  d4ec59657a65e1c1
+000016f0: 3436 6130 6461 3334 3262 3738 6634 3131  46a0da342b78f411
+00001700: 3264 6232 3322 2c0a 2020 2020 2020 2020  2db23",.        
+00001710: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00001720: 3334 6530 6132 6639 6333 3730 6562 3935  34e0a2f9c370eb95
+00001730: 3539 3761 6165 3633 6266 3835 6562 3565  597aae63bf85eb5e
+00001740: 3936 3832 3664 3831 6533 6463 6638 3862  96826d81e3dcf88b
+00001750: 3838 3836 3031 3239 3036 6635 3039 6235  8886012906f509b5
+00001760: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001770: 2020 2022 7368 6132 3536 3a33 3537 3364     "sha256:3573d
+00001780: 3337 3634 3534 6439 3536 3535 3363 3335  376454d956553c35
+00001790: 3664 6634 3562 6238 3234 3236 3263 3339  6df45bb824262c39
+000017a0: 3763 3665 3236 6365 3433 6538 3230 3363  7c6e26ce43e8203c
+000017b0: 3463 3534 3065 6530 6163 6222 2c0a 2020  4c540ee0acb",.  
+000017c0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000017d0: 6861 3235 363a 3337 3437 3434 3362 3661  ha256:3747443b6a
+000017e0: 3930 3430 3031 3437 3333 3730 6437 3831  904001473370d781
+000017f0: 3061 6131 3963 3361 3138 3063 6364 3532  0aa19c3a180ccd52
+00001800: 6137 3135 3761 6163 6332 3634 6135 6163  a7157aacc264a5ac
+00001810: 3739 3236 3565 222c 0a20 2020 2020 2020  79265e",.       
+00001820: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00001830: 3a33 3865 3831 3261 3139 3762 6638 6537  :38e812a197bf8e7
+00001840: 3161 3539 6665 3535 6237 3537 6138 3463  1a59fe55b757a84c
+00001850: 3166 3934 3664 3061 6331 3134 6163 6166  1f946d0ac114acaf
+00001860: 6161 6661 6632 3136 3637 6137 6531 3639  aafaf21667a7e169
+00001870: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00001880: 2020 2020 2273 6861 3235 363a 3361 3036      "sha256:3a06
+00001890: 6633 3263 3936 3334 6138 3730 3566 3463  f32c9634a8705f4c
+000018a0: 6139 3934 3664 3636 3736 3039 6635 3263  a9946d667609f52c
+000018b0: 6631 3330 6435 3534 3838 3831 3430 3166  f130d5548881401f
+000018c0: 3165 6232 6333 3962 3165 3263 222c 0a20  1eb2c39b1e2c",. 
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000018e0: 7368 6132 3536 3a33 6135 6663 3738 6639  sha256:3a5fc78f9
+000018f0: 6533 6635 3031 6131 3631 3461 3938 6637  e3f501a1614a98f7
+00001900: 6335 3464 3339 3639 6633 6164 3962 6261  c54d3969f3ad9bba
+00001910: 3862 6133 6439 6234 3338 6333 6263 3564  8ba3d9b438c3bc5d
+00001920: 3034 3764 6432 3822 2c0a 2020 2020 2020  047dd28",.      
+00001930: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00001940: 363a 3364 3930 3938 6234 3739 6537 3863  6:3d9098b479e78c
+00001950: 3835 3038 3063 3938 6531 6533 3566 6634  85080c98e1e35ff4
+00001960: 3062 3461 3331 6438 3935 3331 3032 6262  0b4a31d8953102bb
+00001970: 3066 6437 6431 6236 6638 6132 3131 3161  0fd7d1b6f8a2111a
+00001980: 3364 222c 0a20 2020 2020 2020 2020 2020  3d",.           
+00001990: 2020 2020 2022 7368 6132 3536 3a33 6463       "sha256:3dc
+000019a0: 3562 3661 3865 6366 6463 3537 3438 6137  5b6a8ecfdc5748a7
+000019b0: 6534 3239 3738 3235 3938 6534 6631 3765  e429782598e4f17e
+000019c0: 6633 3738 6533 6532 3732 6565 6231 3334  f378e3e272eeb134
+000019d0: 3065 6135 3763 3931 3039 6634 3122 2c0a  0ea57c9109f41",.
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019f0: 2273 6861 3235 363a 3431 3535 6235 3161  "sha256:4155b51a
+00001a00: 6530 3565 6434 3731 3939 6463 3562 3261  e05ed47199dc5b2a
+00001a10: 3465 3632 6162 6363 6232 3734 6365 6536  4e62abccb274cee6
+00001a20: 6230 3164 6135 6238 3935 3039 3962 3631  b01da5b895099b61
+00001a30: 6231 3938 3239 3734 222c 0a20 2020 2020  b1982974",.     
+00001a40: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00001a50: 3536 3a34 3939 3139 6638 3430 3062 3565  56:49919f8400b5e
+00001a60: 3439 6539 3631 6633 3230 6337 3335 3338  49e961f320c73538
+00001a70: 3865 6536 3836 6136 3233 3237 6537 3733  8ee686a62327e773
+00001a80: 6661 3562 3363 6536 3732 3166 3765 3738  fa5b3ce6721f7e78
+00001a90: 3563 6522 2c0a 2020 2020 2020 2020 2020  5ce",.          
+00001aa0: 2020 2020 2020 2273 6861 3235 363a 3533        "sha256:53
+00001ab0: 6430 6133 6661 3566 3861 6639 3861 3165  d0a3fa5f8af98a1e
+00001ac0: 3236 3164 6536 6133 3934 3363 6136 3331  261de6a3943ca631
+00001ad0: 6335 3236 3633 3565 6235 3831 3761 3837  c526635eb5817a87
+00001ae0: 6135 3964 3961 3537 6562 6634 3866 222c  a59d9a57ebf48f",
+00001af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b00: 2022 7368 6132 3536 3a35 6630 3038 3532   "sha256:5f00852
+00001b10: 3565 3032 3930 3862 3230 6530 3437 3037  5e02908b20e04707
+00001b20: 6134 6637 3034 6364 3238 3664 3934 3731  a4f704cd286d9471
+00001b30: 3866 3438 6262 3333 6564 6464 6337 6437  8f48bb33edddc7d7
+00001b40: 6235 3834 6464 6463 3122 2c0a 2020 2020  b584dddc1",.    
+00001b50: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00001b60: 3235 363a 3632 3863 3938 3561 6662 3263  256:628c985afb2c
+00001b70: 3764 3237 6134 3830 3062 6662 3630 3965  7d27a4800bfb609e
+00001b80: 3033 3938 3561 6165 6362 3432 6639 3535  03985aaecb42f955
+00001b90: 3034 3939 3537 3831 3465 3034 3931 6434  049957814e0491d4
+00001ba0: 3030 3664 222c 0a20 2020 2020 2020 2020  006d",.         
+00001bb0: 2020 2020 2020 2022 7368 6132 3536 3a36         "sha256:6
+00001bc0: 3565 6439 3233 6638 3461 3638 3434 6465  5ed923f84a6844de
+00001bd0: 3566 6432 3937 3236 6238 3838 6535 3863  5fd29726b888e58c
+00001be0: 3632 3832 3065 3037 3639 6237 3635 3635  62820e0769b76565
+00001bf0: 3438 3065 3166 6463 3364 3036 3266 3822  480e1fdc3d062f8"
+00001c00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001c10: 2020 2273 6861 3235 363a 3637 3334 6536    "sha256:6734e6
+00001c20: 3036 3335 3538 3334 6631 3334 3435 6236  06355834f13445b6
+00001c30: 6164 6333 3862 3533 6330 6664 3435 6631  adc38b53c0fd45f1
+00001c40: 6135 3661 3962 6130 3663 3230 3538 6638  a56a9ba06c2058f8
+00001c50: 3638 3933 6165 3830 3137 222c 0a20 2020  6893ae8017",.   
+00001c60: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00001c70: 6132 3536 3a36 6261 6630 6261 6630 6435  a256:6baf0baf0d5
+00001c80: 6432 3635 6661 3739 3434 6665 6239 6637  d265fa7944feb9f7
+00001c90: 3435 3163 6333 3136 6266 6533 3065 3864  451cc316bfe30e8d
+00001ca0: 6631 6136 3162 3162 6230 3835 3737 6335  f1a61b1bb08577c5
+00001cb0: 3534 6633 3122 2c0a 2020 2020 2020 2020  54f31",.        
+00001cc0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00001cd0: 3666 3466 3436 3638 6531 3833 3138 3530  6f4f4668e1831850
+00001ce0: 6562 6363 3266 6430 6231 6364 3131 3732  ebcc2fd0b1cd1172
+00001cf0: 3139 3437 6236 6463 3763 3030 6266 3163  1947b6dc7c00bf1c
+00001d00: 3662 6433 6339 3239 6165 3134 6632 6337  6bd3c929ae14f2c7
+00001d10: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001d20: 2020 2022 7368 6132 3536 3a36 6635 6332     "sha256:6f5c2
+00001d30: 6537 6263 3861 3462 6637 6334 3236 3539  e7bc8a4bf7c42659
+00001d40: 3937 3635 6231 6264 3333 3231 3765 6338  9765b1bd33217ec8
+00001d50: 3430 3233 3033 3336 3732 6331 6539 6138  4023033672c1e9a8
+00001d60: 6233 3565 6165 6161 6166 3822 2c0a 2020  b35eaeaaaf8",.  
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001d80: 6861 3235 363a 3666 3663 3761 3861 3537  ha256:6f6c7a8a57
+00001d90: 6539 3430 3563 6164 3734 3835 6634 6339  e9405cad7485f4c9
+00001da0: 6433 3137 3261 6534 3836 6366 6566 3133  d3172ae486cfef13
+00001db0: 3434 6235 6464 6438 6535 3233 3935 3832  44b5ddd8e5239582
+00001dc0: 6437 3335 3565 222c 0a20 2020 2020 2020  d7355e",.       
+00001dd0: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00001de0: 3a37 3338 3163 3636 6530 3536 3163 3537  :7381c66e0561c57
+00001df0: 3537 6666 6536 3136 6166 3836 3962 3931  57ffe616af869b91
+00001e00: 3663 3862 3465 3432 6233 3637 6162 3239  6c8b4e42b367ab29
+00001e10: 6665 6463 3938 3438 3164 3165 3734 6531  fedc98481d1e74e1
+00001e20: 3422 2c0a 2020 2020 2020 2020 2020 2020  4",.            
+00001e30: 2020 2020 2273 6861 3235 363a 3733 6463      "sha256:73dc
+00001e40: 3033 6136 6137 6533 3062 3765 6463 3562  03a6a7e30b7edc5b
+00001e50: 3031 6236 3031 6535 3365 3766 6339 3234  01b601e53e7fc924
+00001e60: 6230 3465 3138 3335 6538 6534 3037 6331  b04e1835e8e407c1
+00001e70: 3263 3033 3765 3831 6164 6264 222c 0a20  2c037e81adbd",. 
+00001e80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001e90: 7368 6132 3536 3a37 3464 6230 3035 3264  sha256:74db0052d
+00001ea0: 3938 3563 6633 3766 6131 3131 3832 3864  985cf37fa111828d
+00001eb0: 3064 6432 3330 3737 3661 6339 3963 3734  0dd230776ac99c74
+00001ec0: 3065 3161 3735 3861 6439 3930 3934 6265  0e1a758ad99094be
+00001ed0: 3466 3138 3033 6422 2c0a 2020 2020 2020  4f1803d",.      
+00001ee0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00001ef0: 363a 3735 6632 3536 3862 3431 3839 6464  6:75f2568b4189dd
+00001f00: 6131 6335 3637 3333 3962 3438 6362 6134  a1c567339b48cba4
+00001f10: 6163 3733 3834 6163 6362 3963 3261 3765  ac7384accb9c2a7e
+00001f20: 6436 3535 6364 3836 6230 3430 3535 6337  d655cd86b04055c7
+00001f30: 3935 222c 0a20 2020 2020 2020 2020 2020  95",.           
+00001f40: 2020 2020 2022 7368 6132 3536 3a37 3863       "sha256:78c
+00001f50: 6163 6430 3365 3739 6430 3039 6439 3536  acd03e79d009d956
+00001f60: 3335 6537 6436 6666 3132 6332 3165 6238  35e7d6ff12c21eb8
+00001f70: 3962 3839 3463 3335 3462 6432 6232 6564  9b894c354bd2b2ed
+00001f80: 3062 3437 3633 3337 3336 3933 6222 2c0a  0b4763373693b",.
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2273 6861 3235 363a 3830 6431 3534 3364  "sha256:80d1543d
+00001fb0: 3538 6264 3364 3663 3237 3162 3636 6162  58bd3d6c271b66ab
+00001fc0: 6634 3534 6434 3337 6134 3338 6466 6630  f454d437a438dff0
+00001fd0: 3163 3365 3632 6664 6263 6436 3866 3261  1c3e62fdbcd68f2a
+00001fe0: 3131 3331 3064 3462 222c 0a20 2020 2020  11310d4b",.     
+00001ff0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00002000: 3536 3a38 3330 6432 3934 3861 3565 6333  56:830d2948a5ec3
+00002010: 3763 3338 3664 3331 3730 6334 3833 3036  7c386d3170c48306
+00002020: 3337 3938 6437 3837 3930 3337 3439 3235  3798d78790374925
+00002030: 3430 6631 3061 3437 3565 3366 6436 6632  40f10a475e3fd6f2
+00002040: 3434 6222 2c0a 2020 2020 2020 2020 2020  44b",.          
+00002050: 2020 2020 2020 2273 6861 3235 363a 3839        "sha256:89
+00002060: 3163 6639 6234 3837 3736 6235 6336 3163  1cf9b48776b5c61c
+00002070: 3730 3062 3535 6135 3938 3632 3166 6462  700b55a598621fdb
+00002080: 3762 3165 3330 3161 3535 3033 3635 3537  7b1e301a55036557
+00002090: 3165 3936 3234 6632 3730 6332 3033 222c  1e9624f270c203",
+000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020b0: 2022 7368 6132 3536 3a38 6632 3565 3137   "sha256:8f25e17
+000020c0: 6162 3330 3339 6230 3566 3736 3262 3061  ab3039b05f762b0a
+000020d0: 3535 6165 3062 3336 3332 6232 6530 3733  55ae0b3632b2e073
+000020e0: 6439 6338 6663 3838 6538 3961 6361 3331  d9c8fc88e89aca31
+000020f0: 6136 3139 3865 3838 6622 2c0a 2020 2020  a6198e88f",.    
+00002100: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00002110: 3235 363a 3961 3332 3637 3632 3038 3636  256:9a3267620866
+00002120: 6339 6431 3762 3935 3961 3834 6464 3062  c9d17b959a84dd0b
+00002130: 6432 6434 3537 3139 6238 3137 3234 3565  d2d45719b817245e
+00002140: 3439 3337 3165 6164 3739 6564 3466 3731  49371ead79ed4f71
+00002150: 3064 3139 222c 0a20 2020 2020 2020 2020  0d19",.         
+00002160: 2020 2020 2020 2022 7368 6132 3536 3a61         "sha256:a
+00002170: 3034 6638 3666 3431 6138 3931 3666 6534  04f86f41a8916fe4
+00002180: 3561 6335 3032 3465 6334 3737 6634 3166  5ac5024ec477f41f
+00002190: 3838 3662 3363 3433 3564 6132 6434 6533  886b3c435da2d4e3
+000021a0: 6432 3730 3962 3232 6162 3032 6166 3122  d2709b22ab02af1"
+000021b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000021c0: 2020 2273 6861 3235 363a 6161 6635 3361    "sha256:aaf53a
+000021d0: 3663 6562 6164 3065 6165 3537 3866 3036  6cebad0eae578f06
+000021e0: 3263 3764 3436 3231 3535 6561 6461 3963  2c7d462155eada9c
+000021f0: 3137 3262 6438 6334 6432 3530 6238 6331  172bd8c4d250b8c1
+00002200: 6438 6562 3766 3931 3661 222c 0a20 2020  d8eb7f916a",.   
+00002210: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00002220: 6132 3536 3a61 6263 3131 3835 6437 3966  a256:abc1185d79f
+00002230: 3437 6330 6137 6161 6637 6532 3431 3261  47c0a7aaf7e2412a
+00002240: 3065 6232 6330 3362 3732 3435 3831 3133  0eb2c03b72458113
+00002250: 3931 3933 6432 6438 3262 3361 6438 6362  9193d2d82b3ad8cb
+00002260: 6230 3061 6322 2c0a 2020 2020 2020 2020  b00ac",.        
+00002270: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00002280: 6163 3061 6136 6364 3533 6162 3961 3331  ac0aa6cd53ab9a31
+00002290: 6433 3937 6638 3330 3366 3932 6334 3266  d397f8303f92c42f
+000022a0: 3533 3436 3933 3532 3866 6166 6264 6239  534693528fafbdb9
+000022b0: 3937 6338 3262 6165 3665 3437 3761 6439  97c82bae6e477ad9
+000022c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000022d0: 2020 2022 7368 6132 3536 3a61 6333 3737     "sha256:ac377
+000022e0: 3565 3333 3131 3636 3164 3461 6461 6365  5e3311661d4adace
+000022f0: 3336 3937 6135 3261 6330 6261 6231 3765  3697a52ac0bab17e
+00002300: 6464 3136 3630 3837 6434 3933 6235 3264  dd166087d493b52d
+00002310: 3466 3466 3535 3366 3966 3022 2c0a 2020  4f4f553f9f0",.  
+00002320: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00002330: 6861 3235 363a 6230 3666 3064 3362 6630  ha256:b06f0d3bf0
+00002340: 3435 3135 3864 3266 6238 3833 3763 3537  45158d2fb8837c57
+00002350: 3835 6665 3966 6639 6238 6339 3333 3538  85fe9ff9b8c93358
+00002360: 6265 3634 3436 3161 3130 3839 6635 6461  be64461a1089f5da
+00002370: 3938 3331 3337 222c 0a20 2020 2020 2020  983137",.       
+00002380: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00002390: 3a62 3131 3635 3032 3038 3763 6538 6136  :b116502087ce8a6
+000023a0: 6237 6135 6631 3831 3435 3638 6363 6264  b7a5f1814568ccbd
+000023b0: 3065 3966 3663 6664 3939 3934 3861 6135  0e9f6cfd99948aa5
+000023c0: 3962 3065 3234 3164 6335 3763 6637 3339  9b0e241dc57cf739
+000023d0: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
+000023e0: 2020 2020 2273 6861 3235 363a 6238 3266      "sha256:b82f
+000023f0: 6162 3738 6530 6231 3332 3965 3138 3361  ab78e0b1329e183a
+00002400: 3635 3236 3035 3831 6465 3433 3735 6636  65260581de4375f6
+00002410: 3139 3136 3734 3738 6464 6461 6235 3130  19167478dddab510
+00002420: 6336 6336 6662 3034 6439 6236 222c 0a20  c6c6fb04d9b6",. 
+00002430: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002440: 7368 6132 3536 3a62 6437 3136 3331 3832  sha256:bd7163182
+00002450: 3133 3363 3063 3737 3031 6232 3565 3630  133c0c7701b25e60
+00002460: 3463 6631 3631 3163 3064 3837 3731 3265  4cf1611c0d87712e
+00002470: 3536 6538 3865 3765 6535 6437 3264 6561  56e88e7ee5d72dea
+00002480: 6233 6537 3662 3522 2c0a 2020 2020 2020  b3e76b5",.      
+00002490: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+000024a0: 363a 6333 3662 6362 6330 6435 3137 3461  6:c36bcbc0d5174a
+000024b0: 3830 6436 6363 6366 3433 6130 6563 6163  80d6cccf43a0ecac
+000024c0: 6134 3465 3831 6432 3562 6534 6237 6639  a44e81d25be4b7f9
+000024d0: 3066 3065 6437 6263 6662 6235 6130 3039  0f0ed7bcfbb5a009
+000024e0: 3039 222c 0a20 2020 2020 2020 2020 2020  09",.           
+000024f0: 2020 2020 2022 7368 6132 3536 3a63 3361       "sha256:c3a
+00002500: 6638 6530 6630 3733 3939 6433 3137 3662  f8e0f07399d3176b
+00002510: 3137 3966 3265 3236 3334 6333 6365 3963  179f2e2634c3ce9c
+00002520: 3133 3031 3337 3961 3662 3863 3963 3961  1301379a6b8c9c9a
+00002530: 6565 6364 3438 3164 6134 3934 6622 2c0a  eecd481da494f",.
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 2273 6861 3235 363a 6338 3431 3332 6135  "sha256:c84132a5
+00002560: 3463 3735 3066 6461 3537 3732 3964 3165  4c750fda57729d1e
+00002570: 3235 3939 6262 3539 3866 3566 6130 3334  2599bb598f5fa034
+00002580: 3430 3835 6462 6465 3530 3033 6261 3432  4085dbde5003ba42
+00002590: 3961 3437 3938 6330 222c 0a20 2020 2020  9a4798c0",.     
+000025a0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+000025b0: 3536 3a63 6237 6232 6162 3031 3838 3832  56:cb7b2ab018882
+000025c0: 3935 3933 6239 6465 3634 3635 3435 3137  9593b9de64654517
+000025d0: 3535 3437 6137 3064 3961 3665 3262 3633  5547a70d9a6e2b63
+000025e0: 6266 3263 6438 3761 3061 3339 3135 3939  bf2cd87a0a391599
+000025f0: 3332 3422 2c0a 2020 2020 2020 2020 2020  324",.          
+00002600: 2020 2020 2020 2273 6861 3235 363a 6363        "sha256:cc
+00002610: 6134 6465 6635 3736 6634 3761 3039 6139  a4def576f47a09a9
+00002620: 3433 3636 3662 3866 3832 3936 3036 6263  43666b8f829606bc
+00002630: 6231 3765 3262 6332 6435 3931 3161 3436  b17e2bc2d5911a46
+00002640: 6338 6638 6461 3435 6635 3637 3535 222c  c8f8da45f56755",
+00002650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002660: 2022 7368 6132 3536 3a63 6636 3531 3165   "sha256:cf6511e
+00002670: 6661 3438 3031 6239 6233 3864 6335 3534  fa4801b9b38dc554
+00002680: 3664 3735 3437 6435 6235 6336 6566 3462  6d7547d5b5c6ef4b
+00002690: 3038 3163 3630 6232 3365 3464 3934 3164  081c60b23e4d941d
+000026a0: 3065 6261 3963 6265 6222 2c0a 2020 2020  0eba9cbeb",.    
+000026b0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+000026c0: 3235 363a 6431 3666 6435 3235 3266 3838  256:d16fd5252f88
+000026d0: 3365 6230 3734 6361 3535 6362 3632 3262  3eb074ca55cb622b
+000026e0: 6330 6265 6534 3962 3937 3961 6534 6538  c0bee49b979ae4e8
+000026f0: 3633 3966 6666 3663 6133 6666 3434 6639  639fff6ca3ff44f9
+00002700: 6638 3534 222c 0a20 2020 2020 2020 2020  f854",.         
+00002710: 2020 2020 2020 2022 7368 6132 3536 3a64         "sha256:d
+00002720: 3236 3836 6639 3136 3131 6639 6531 3766  2686f91611f9e17f
+00002730: 3435 3438 6462 6630 3530 6537 3562 3037  4548dbf050e75b07
+00002740: 3962 6263 3261 3832 6265 3536 3538 3332  9bbc2a82be565832
+00002750: 6263 3865 6139 3034 3762 3631 6338 6322  bc8ea9047b61c8c"
+00002760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002770: 2020 2273 6861 3235 363a 6437 6663 3366    "sha256:d7fc3f
+00002780: 6361 3031 6461 3138 6662 6162 6534 3632  ca01da18fbabe462
+00002790: 3564 3634 6262 3631 3262 3533 3335 3333  5d64bb612b533533
+000027a0: 6564 3130 3034 3561 3261 6333 6464 3139  ed10045a2ac3dd19
+000027b0: 3462 6661 3635 3662 3630 222c 0a20 2020  4bfa656b60",.   
+000027c0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+000027d0: 6132 3536 3a64 6435 3635 3365 3637 6231  a256:dd5653e67b1
+000027e0: 3439 3530 3363 3638 6334 3031 3862 6630  49503c68c4018bf0
+000027f0: 3765 3432 6565 6564 3662 3465 3935 3662  7e42eeed6b4e956b
+00002800: 3234 6330 3063 6364 6639 3361 6337 3963  24c00ccdf93ac79c
+00002810: 6466 6638 3422 2c0a 2020 2020 2020 2020  dff84",.        
+00002820: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00002830: 6465 3536 3935 6136 6631 6438 3334 3062  de5695a6f1d8340b
+00002840: 3132 6135 6436 6434 3438 3432 3930 6565  12a5d6d4484290ee
+00002850: 3734 6436 3165 3436 3763 3339 6666 3033  74d61e467c39ff03
+00002860: 6233 3965 3330 6466 3632 6366 3833 6130  b39e30df62cf83a0
+00002870: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002880: 2020 2022 7368 6132 3536 3a65 3061 6338     "sha256:e0ac8
+00002890: 3935 3963 3932 3935 3933 6665 6533 3864  959c929593fee38d
+000028a0: 6131 6332 6236 3465 6539 3737 3837 3333  a1c2b64ee9778733
+000028b0: 6364 6630 3363 3438 3263 3966 6631 6435  cdf03c482c9ff1d5
+000028c0: 3038 6236 6235 3933 6232 6222 2c0a 2020  08b6b593b2b",.  
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000028e0: 6861 3235 363a 6531 6232 3565 3361 6436  ha256:e1b25e3ad6
+000028f0: 6339 3039 6633 3938 6466 3839 3231 3738  c909f398df892178
+00002900: 3064 3661 3364 3132 3064 3863 3039 3436  0d6a3d120d8c0946
+00002910: 3637 3230 3232 3666 6336 3231 3630 3562  6720226fc621605b
+00002920: 3666 3932 6231 222c 0a20 2020 2020 2020  6f92b1",.       
+00002930: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00002940: 3a65 3633 3339 3430 6632 3863 3165 3931  :e633940f28c1e91
+00002950: 3336 3135 6664 3632 3466 6364 6437 3266  3615fd624fcdd72f
+00002960: 6462 6138 3037 6266 3533 6561 3639 3235  dba807bf53ea6925
+00002970: 6436 6135 3838 6538 3465 3131 3531 3533  d6a588e84e115153
+00002980: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+00002990: 2020 2020 2273 6861 3235 363a 6538 3964      "sha256:e89d
+000029a0: 6632 3935 3865 3531 3539 6238 3131 6166  f2958e5159b811af
+000029b0: 3966 6630 6639 3236 3134 6461 6266 3466  9ff0f92614dabf4f
+000029c0: 6636 3137 6330 3361 3463 3163 3666 6635  f617c03a4c1c6ff5
+000029d0: 3362 6631 6333 3939 6530 6531 222c 0a20  3bf1c399e0e1",. 
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000029f0: 7368 6132 3536 3a65 6139 6639 6336 3033  sha256:ea9f9c603
+00002a00: 3465 6132 6439 3364 3931 3437 3831 3866  4ea2d93d9147818f
+00002a10: 3137 6332 6130 3836 3064 3431 6237 3163  17c2a0860d41b71c
+00002a20: 3338 6239 6365 3464 3535 6632 3162 3666  38b9ce4d55f21b6f
+00002a30: 3931 3635 6131 3122 2c0a 2020 2020 2020  9165a11",.      
+00002a40: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00002a50: 363a 6636 3435 6361 6166 3030 3038 6261  6:f645caaf0008ba
+00002a60: 6366 3334 3938 3735 6139 3734 3232 3066  cf349875a974220f
+00002a70: 3166 3164 6133 3439 6335 6462 6537 6334  1f1da349c5dbe7c4
+00002a80: 6563 3933 3034 3863 6463 3738 3561 3333  ec93048cdc785a33
+00002a90: 3236 222c 0a20 2020 2020 2020 2020 2020  26",.           
+00002aa0: 2020 2020 2022 7368 6132 3536 3a66 3833       "sha256:f83
+00002ab0: 3033 3431 3463 3762 3033 6637 3934 3334  03414c7b03f79434
+00002ac0: 3761 6430 3632 6330 3531 3663 6565 3065  7ad062c0516cee0e
+00002ad0: 3135 6637 6136 3132 6162 6430 6365 3165  15f7a612abd0ce1e
+00002ae0: 3235 6361 6636 6365 6234 3764 6622 2c0a  25caf6ceb47df",.
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b00: 2273 6861 3235 363a 6663 6136 3261 3833  "sha256:fca62a83
+00002b10: 3031 6236 3035 6239 3534 6164 3265 3963  01b605b954ad2e9c
+00002b20: 3336 3636 6639 6439 3766 3633 3837 3261  3666f9d97f63872a
+00002b30: 6134 6566 6361 6535 3439 3262 6163 6132  a4efcae5492baca2
+00002b40: 3035 3662 3734 6162 220a 2020 2020 2020  056b74ab".      
+00002b50: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00002b60: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
+00002b70: 2270 7974 686f 6e5f 6675 6c6c 5f76 6572  "python_full_ver
+00002b80: 7369 6f6e 203e 3d20 2733 2e37 2e30 2722  sion >= '3.7.0'"
+00002b90: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+00002ba0: 6572 7369 6f6e 223a 2022 3d3d 332e 312e  ersion": "==3.1.
+00002bb0: 3022 0a20 2020 2020 2020 207d 2c0a 2020  0".        },.  
+00002bc0: 2020 2020 2020 2263 6c69 636b 223a 207b        "click": {
+00002bd0: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
+00002be0: 7368 6573 223a 205b 0a20 2020 2020 2020  shes": [.       
+00002bf0: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00002c00: 3a37 3638 3264 6338 6166 6233 3032 3937  :7682dc8afb30297
+00002c10: 3030 3136 3734 3537 3565 6130 3064 3138  001674575ea00d18
+00002c20: 3134 6438 3038 6436 6133 3661 6634 3135  14d808d6a36af415
+00002c30: 6138 3262 6434 3831 6433 3762 6137 6238  a82bd481d37ba7b8
+00002c40: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00002c50: 2020 2020 2273 6861 3235 363a 6262 3464      "sha256:bb4d
+00002c60: 3831 3333 6362 3135 6136 3039 6634 3465  8133cb15a609f44e
+00002c70: 3832 3133 6439 6233 3931 6230 3830 3937  8213d9b391b08097
+00002c80: 3935 3036 3239 3133 6233 3833 6336 3262  95062913b383c62b
+00002c90: 6530 6565 3935 6231 6462 3438 220a 2020  e0ee95b1db48".  
+00002ca0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00002cb0: 2020 2020 2020 2020 2022 6d61 726b 6572           "marker
+00002cc0: 7322 3a20 2270 7974 686f 6e5f 7665 7273  s": "python_vers
+00002cd0: 696f 6e20 3e3d 2027 332e 3727 222c 0a20  ion >= '3.7'",. 
+00002ce0: 2020 2020 2020 2020 2020 2022 7665 7273             "vers
+00002cf0: 696f 6e22 3a20 223d 3d38 2e31 2e33 220a  ion": "==8.1.3".
+00002d00: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002d10: 2020 2022 636f 6c6f 7261 6d61 223a 207b     "colorama": {
+00002d20: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
+00002d30: 7368 6573 223a 205b 0a20 2020 2020 2020  shes": [.       
+00002d40: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00002d50: 3a30 3836 3935 6635 6362 3765 6436 6530  :08695f5cb7ed6e0
+00002d60: 3533 3161 3230 3537 3236 3937 3239 3732  531a205726972972
+00002d70: 3733 6334 3762 3863 6165 3561 3633 6666  73c47b8cae5a63ff
+00002d80: 6336 6436 6564 3563 3230 3162 6536 6534  c6d6ed5c201be6e4
+00002d90: 3422 2c0a 2020 2020 2020 2020 2020 2020  4",.            
+00002da0: 2020 2020 2273 6861 3235 363a 3466 3164      "sha256:4f1d
+00002db0: 3939 3931 6635 6163 6330 6361 3131 3966  9991f5acc0ca119f
+00002dc0: 3964 3434 3336 3230 6237 3766 3964 3662  9d443620b77f9d6b
+00002dd0: 3333 3730 3365 3531 3031 3163 3136 6261  33703e51011c16ba
+00002de0: 6635 3761 6662 3238 3566 6336 220a 2020  f57afb285fc6".  
+00002df0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00002e00: 2020 2020 2020 2020 2022 6d61 726b 6572           "marker
+00002e10: 7322 3a20 2273 7973 5f70 6c61 7466 6f72  s": "sys_platfor
+00002e20: 6d20 3d3d 2027 7769 6e33 3227 222c 0a20  m == 'win32'",. 
+00002e30: 2020 2020 2020 2020 2020 2022 7665 7273             "vers
+00002e40: 696f 6e22 3a20 223d 3d30 2e34 2e36 220a  ion": "==0.4.6".
+00002e50: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002e60: 2020 2022 636f 7665 7261 6765 223a 207b     "coverage": {
+00002e70: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
+00002e80: 7368 6573 223a 205b 0a20 2020 2020 2020  shes": [.       
+00002e90: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00002ea0: 3a30 3661 3961 3262 6530 6235 6235 3736  :06a9a2be0b5b576
+00002eb0: 6333 6631 3866 3161 3234 3166 3034 3733  c3f18f1a241f0473
+00002ec0: 3537 3563 3461 3236 3032 3162 3532 6232  575c4a26021b52b2
+00002ed0: 6138 3532 3633 6130 3066 3033 3464 3531  a85263a00f034d51
+00002ee0: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
+00002ef0: 2020 2020 2273 6861 3235 363a 3036 6662      "sha256:06fb
+00002f00: 3138 3265 3639 6633 3366 3663 6431 6433  182e69f33f6cd1d3
+00002f10: 3961 3663 3539 3732 3934 6366 6633 3134  9a6c597294cff314
+00002f20: 3335 3534 6236 3462 3938 3235 6431 6463  3554b64b9825d1dc
+00002f30: 3639 6431 3863 6332 6666 6632 222c 0a20  69d18cc2fff2",. 
+00002f40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002f50: 7368 6132 3536 3a30 6135 6639 6531 6462  sha256:0a5f9e1db
+00002f60: 6437 6662 6533 3031 3936 3537 3863 6133  d7fbe30196578ca3
+00002f70: 3666 3366 6261 3735 3337 3666 6239 3938  6f3fba75376fb998
+00002f80: 3838 6333 3935 6335 3838 3062 3335 3565  88c395c5880b355e
+00002f90: 3238 3735 6638 6122 2c0a 2020 2020 2020  2875f8a",.      
 00002fa0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00002fb0: 363a 3036 6662 3138 3265 3639 6633 3366  6:06fb182e69f33f
-00002fc0: 3663 6431 6433 3961 3663 3539 3732 3934  6cd1d39a6c597294
-00002fd0: 6366 6633 3134 3335 3534 6236 3462 3938  cff3143554b64b98
-00002fe0: 3235 6431 6463 3639 6431 3863 6332 6666  25d1dc69d18cc2ff
-00002ff0: 6632 222c 0d0a 2020 2020 2020 2020 2020  f2",..          
-00003000: 2020 2020 2020 2273 6861 3235 363a 3061        "sha256:0a
-00003010: 3566 3965 3164 6264 3766 6265 3330 3139  5f9e1dbd7fbe3019
-00003020: 3635 3738 6361 3336 6633 6662 6137 3533  6578ca36f3fba753
-00003030: 3736 6662 3939 3838 3863 3339 3563 3538  76fb99888c395c58
-00003040: 3830 6233 3535 6532 3837 3566 3861 222c  80b355e2875f8a",
-00003050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003060: 2020 2273 6861 3235 363a 3065 3166 3932    "sha256:0e1f92
-00003070: 3865 6166 3534 3639 6331 3165 3838 3666  8eaf5469c11e886f
-00003080: 6530 3838 3561 6432 6266 3165 6336 3036  e0885ad2bf1ec606
-00003090: 3433 3465 3739 3834 3261 3837 3932 3737  434e79842a879277
-000030a0: 3839 3561 3530 3934 3261 222c 0d0a 2020  895a50942a",..  
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000030c0: 6861 3235 363a 3137 3137 3137 6337 6362  ha256:171717c7cb
-000030d0: 3662 3435 3361 6562 6163 3961 3265 6636  6b453aebac9a2ef6
-000030e0: 3033 3639 3964 6132 3337 6633 3431 6233  03699da237f341b3
-000030f0: 3865 6562 6665 6539 6265 3735 6432 3764  8eebfee9be75d27d
-00003100: 6333 3865 3031 222c 0d0a 2020 2020 2020  c38e01",..      
-00003110: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003120: 363a 3165 3964 3638 3334 3236 3436 3465  6:1e9d683426464e
-00003130: 3461 3235 3262 6637 3063 3334 3938 3735  4a252bf70c349875
-00003140: 3630 3535 3031 3666 3939 6464 6165 6333  6055016f99ddaec3
-00003150: 3737 3462 6633 3638 6537 3662 6265 3032  774bf368e76bbe02
-00003160: 6236 222c 0d0a 2020 2020 2020 2020 2020  b6",..          
-00003170: 2020 2020 2020 2273 6861 3235 363a 3230        "sha256:20
-00003180: 3165 3733 3839 3539 3161 6634 3039 3530  1e7389591af40950
-00003190: 6136 3438 3062 6439 6564 6661 3865 6430  a6480bd9edfa8ed0
-000031a0: 3433 3436 6666 3830 3030 3263 6563 3161  4346ff80002cec1a
-000031b0: 3636 6361 6334 3534 3963 3161 6437 222c  66cac4549c1ad7",
-000031c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000031d0: 2020 2273 6861 3235 363a 3234 3531 3637    "sha256:245167
-000031e0: 6464 3236 3138 3061 6234 6339 3164 3565  dd26180ab4c91d5e
-000031f0: 3134 3936 6133 3062 6534 6364 3732 3161  1496a30be4cd721a
-00003200: 3563 6632 6162 6635 3239 3734 6639 3635  5cf2abf52974f965
-00003210: 6631 3066 3131 3431 3966 222c 0d0a 2020  f10f11419f",..  
-00003220: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003230: 6861 3235 363a 3261 6565 3237 3463 3436  ha256:2aee274c46
-00003240: 3539 3037 3137 6633 3861 6535 6534 3635  590717f38ae5e465
-00003250: 3039 3838 6431 6166 3334 3066 6530 3631  0988d1af340fe061
-00003260: 3637 3534 3663 6333 3266 6532 6635 3865  67546cc32fe2f58e
-00003270: 6430 3562 3032 222c 0d0a 2020 2020 2020  d05b02",..      
-00003280: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003290: 363a 3265 3037 6235 3432 3834 6533 3831  6:2e07b54284e381
-000032a0: 3533 3163 3837 6637 3835 6636 3133 6238  531c87f785f613b8
-000032b0: 3333 3536 3963 3134 6563 6163 6463 6238  33569c14ecacdcb8
-000032c0: 3564 3536 6232 3563 3436 3232 6331 3663  5d56b25c4622c16c
-000032d0: 3363 222c 0d0a 2020 2020 2020 2020 2020  3c",..          
-000032e0: 2020 2020 2020 2273 6861 3235 363a 3331        "sha256:31
-000032f0: 3536 3365 3937 6461 6535 3539 3835 3536  563e97dae5598556
-00003300: 3630 3034 3636 6164 3962 6565 6133 3966  600466ad9beea39f
-00003310: 6230 3465 3032 3239 6536 3163 3132 6561  b04e0229e61c12ea
-00003320: 6132 3036 6530 6161 3230 3230 3633 222c  a206e0aa202063",
-00003330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003340: 2020 2273 6861 3235 363a 3333 6436 6433    "sha256:33d6d3
-00003350: 6561 3239 6435 6233 6131 6136 3332 6233  ea29d5b3a1a632b3
-00003360: 6334 6534 6634 6563 6165 3234 6566 3137  c4e4f4ecae24ef17
-00003370: 3062 3062 3965 6534 3933 3838 3366 3264  0b0b9ee493883f2d
-00003380: 6631 3030 3339 3935 3961 222c 0d0a 2020  f10039959a",..  
-00003390: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000033a0: 6861 3235 363a 3364 3337 3664 6635 3863  ha256:3d376df58c
-000033b0: 6331 3131 6463 3865 3231 6533 6236 6532  c111dc8e21e3b6e2
-000033c0: 3436 3036 6235 6262 3564 6565 3630 3234  4606b5bb5dee6024
-000033d0: 6634 3661 3561 6263 6139 3931 3234 6232  f46a5abca99124b2
-000033e0: 3232 3965 6635 222c 0d0a 2020 2020 2020  229ef5",..      
-000033f0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003400: 363a 3431 3962 6664 3263 6161 6532 3638  6:419bfd2caae268
-00003410: 3632 3364 6434 3639 6566 6639 3664 3531  623dd469eff96d51
-00003420: 3061 3932 3063 3930 3932 3862 3630 6632  0a920c90928b60f2
-00003430: 3037 3364 3739 6638 6665 3262 6263 3539  073d79f8fe2bbc59
-00003440: 3539 222c 0d0a 2020 2020 2020 2020 2020  59",..          
-00003450: 2020 2020 2020 2273 6861 3235 363a 3438        "sha256:48
-00003460: 6331 3964 3231 3539 6434 3333 6363 6339  c19d2159d433ccc9
-00003470: 3965 3732 3963 6561 6537 6435 3239 3366  9e729ceae7d5293f
-00003480: 6266 6661 3062 6462 3934 3935 3264 3335  bffa0bdb94952d35
-00003490: 3739 3938 3364 3163 3863 3964 3937 222c  79983d1c8c9d97",
-000034a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000034b0: 2020 2273 6861 3235 363a 3439 3936 3961    "sha256:49969a
-000034c0: 3966 3766 6661 3038 3664 3937 3364 3931  9f7ffa086d973d91
-000034d0: 6365 6338 6432 6533 3130 3830 3433 3665  cec8d2e31080436e
-000034e0: 6630 6662 3461 3335 3963 6165 3932 3765  f0fb4a359cae927e
-000034f0: 3734 3261 6266 6161 6136 222c 0d0a 2020  742abfaaa6",..  
-00003500: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003510: 6861 3235 363a 3532 6564 6331 6136 3063  ha256:52edc1a60c
-00003520: 3064 3334 6166 6134 3231 6339 6333 3730  0d34afa421c9c370
-00003530: 3738 3831 3762 3265 3637 6133 3932 6361  78817b2e67a392ca
-00003540: 6231 3764 3937 3238 3362 3634 6335 3833  b17d97283b64c583
-00003550: 3366 3432 3766 222c 0d0a 2020 2020 2020  3f427f",..      
-00003560: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003570: 363a 3533 3738 3931 6165 3863 6535 3965  6:537891ae8ce59e
-00003580: 6636 3364 3031 3233 6637 6163 3965 3261  f63d0123f7ac9e2a
-00003590: 6530 6663 3862 3732 6337 6363 6265 3532  e0fc8b72c7ccbe52
-000035a0: 3936 6665 6334 3566 6436 3839 3637 6236  96fec45fd68967b6
-000035b0: 6339 222c 0d0a 2020 2020 2020 2020 2020  c9",..          
-000035c0: 2020 2020 2020 2273 6861 3235 363a 3534        "sha256:54
-000035d0: 6238 3936 3337 3661 6235 3633 6264 3338  b896376ab563bd38
-000035e0: 3435 3363 6563 6238 3133 6332 3935 6366  453cecb813c295cf
-000035f0: 3334 3763 6635 3930 3665 3862 3431 6433  347cf5906e8b41d3
-00003600: 3430 6230 3332 3161 3534 3333 6535 222c  40b0321a5433e5",
-00003610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003620: 2020 2273 6861 3235 363a 3538 6332 6363    "sha256:58c2cc
-00003630: 6332 6630 3065 6362 3531 3235 3363 6265  c2f00ecb51253cbe
-00003640: 3564 3864 3731 3232 6133 3435 3930 6661  5d8d7122a34590fa
-00003650: 6339 3634 3661 3936 3064 3134 3330 6435  c9646a960d1430d5
-00003660: 6231 3533 3231 6439 3566 222c 0d0a 2020  b15321d95f",..  
-00003670: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003680: 6861 3235 363a 3562 3735 3430 3136 3137  ha256:5b75401617
-00003690: 3930 6232 6632 3831 3433 3139 3166 3566  90b2f28143191f5f
-000036a0: 3865 6330 3266 6231 3332 3636 3066 6631  8ec02fb132660ff1
-000036b0: 3735 6237 3734 3762 3935 6463 6237 3761  75b7747b95dcb77a
-000036c0: 6332 3635 3632 222c 0d0a 2020 2020 2020  c26562",..      
-000036d0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000036e0: 363a 3562 6161 3036 3432 3066 3833 3731  6:5baa06420f8371
-000036f0: 3834 3133 3037 3532 6237 6335 6561 3038  84130752b7c5ea08
-00003700: 3038 3736 3230 3833 6266 3334 3837 6235  08762083bf3487b5
-00003710: 3033 3864 3638 6230 3132 6535 3933 3764  038d68b012e5937d
-00003720: 6265 222c 0d0a 2020 2020 2020 2020 2020  be",..          
-00003730: 2020 2020 2020 2273 6861 3235 363a 3565        "sha256:5e
-00003740: 3333 3066 6337 3962 6437 3230 3765 3436  330fc79bd7207e46
-00003750: 6337 6437 6664 3262 6234 6166 3239 3633  c7d7fd2bb4af2963
-00003760: 6635 6636 3335 3730 3339 3235 3534 3361  f5f635703925543a
-00003770: 3730 6239 3935 3734 6230 6665 6139 222c  70b99574b0fea9",
-00003780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003790: 2020 2273 6861 3235 363a 3631 6239 6135    "sha256:61b9a5
-000037a0: 3238 6662 3334 3833 3733 6334 3333 6538  28fb348373c433e8
-000037b0: 3936 3635 3335 3037 3462 3830 3263 3761  966535074b802c7a
-000037c0: 3564 3766 3233 6334 6634 3231 6536 6336  5d7f23c4f421e6c6
-000037d0: 6532 6631 3639 3761 3666 222c 0d0a 2020  e2f1697a6f",..  
-000037e0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000037f0: 6861 3235 363a 3633 3432 3637 3036 3131  ha256:6342670611
-00003800: 3862 3766 3563 6636 6262 3663 3839 3564  8b7f5cf6bb6c895d
-00003810: 6332 3135 6438 6134 3138 6435 3935 3235  c215d8a418d59525
-00003820: 3434 3034 3263 3861 3264 3966 6538 3766  44042c8a2d9fe87f
-00003830: 6366 3039 6362 222c 0d0a 2020 2020 2020  cf09cb",..      
-00003840: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003850: 363a 3664 3034 3065 6637 6339 3835 3962  6:6d040ef7c9859b
-00003860: 6231 3164 6665 6230 3536 6666 3562 3338  b11dfeb056ff5b38
-00003870: 3732 3433 3665 3362 3565 3430 3138 3137  72436e3b5e401817
-00003880: 6438 3761 3331 6531 3735 3062 3961 6532  d87a31e1750b9ae2
-00003890: 6662 222c 0d0a 2020 2020 2020 2020 2020  fb",..          
-000038a0: 2020 2020 2020 2273 6861 3235 363a 3666        "sha256:6f
-000038b0: 3438 3335 3164 3636 3537 3566 3533 3536  48351d66575f5356
-000038c0: 3639 3330 3661 6137 6436 6436 6637 3162  69306aa7d6d6f71b
-000038d0: 6334 3333 3732 3437 3362 3534 6138 3332  c43372473b54a832
-000038e0: 3232 3238 3033 6562 3935 3666 6431 222c  222803eb956fd1",
-000038f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003900: 2020 2273 6861 3235 363a 3765 6537 6439    "sha256:7ee7d9
-00003910: 6434 3832 3263 3861 6363 3734 6135 6532  d4822c8acc74a5e2
-00003920: 3663 3530 3630 3464 6666 3832 3437 3130  6c50604dff824710
-00003930: 6263 3864 6534 3234 3930 3463 3039 3832  bc8de424904c0982
-00003940: 6532 3563 3339 6336 6362 222c 0d0a 2020  e25c39c6cb",..  
-00003950: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003960: 6861 3235 363a 3831 6331 3361 3166 6337  ha256:81c13a1fc7
-00003970: 3436 3863 3430 6631 3334 3230 3733 3238  468c40f134207328
-00003980: 3035 6134 6333 3861 3130 3564 3839 3834  05a4c38a105d8984
-00003990: 3862 3763 3130 6166 3635 6139 3062 6566  8b7c10af65a90bef
-000039a0: 6632 3532 3530 222c 0d0a 2020 2020 2020  f25250",..      
-000039b0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000039c0: 363a 3864 3133 6336 3465 6532 6433 3365  6:8d13c64ee2d33e
-000039d0: 6363 6637 3433 3739 3631 6236 6561 3761  ccf7437961b6ea7a
-000039e0: 6438 3637 3365 3262 6530 3430 6234 6637  d8673e2be040b4f7
-000039f0: 6664 3466 6434 6434 6432 3864 3963 6362  fd4fd4d4d28d9ccb
-00003a00: 3165 222c 0d0a 2020 2020 2020 2020 2020  1e",..          
-00003a10: 2020 2020 2020 2273 6861 3235 363a 3864        "sha256:8d
-00003a20: 6538 6262 3065 3561 6431 3033 3838 3864  e8bb0e5ad103888d
-00003a30: 3635 6162 6566 3862 6361 3431 6162 3933  65abef8bca41ab93
-00003a40: 3732 3136 3437 3539 3061 3366 3734 3031  721647590a3f7401
-00003a50: 3030 6364 3635 6333 6230 3035 3131 222c  00cd65c3b00511",
-00003a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003a70: 2020 2273 6861 3235 363a 3866 6130 3362    "sha256:8fa03b
-00003a80: 6365 3962 6662 6565 6566 3966 3362 3136  ce9bfbeeef9f3b16
-00003a90: 3061 3862 6564 3339 6132 3231 6438 3233  0a8bed39a221d823
-00003aa0: 3038 6234 3135 3262 3237 6438 3264 3864  08b4152b27d82d8d
-00003ab0: 6161 3730 3431 6665 6535 222c 0d0a 2020  aa7041fee5",..  
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003ad0: 6861 3235 363a 3932 3464 3934 3239 3163  ha256:924d94291c
-00003ae0: 6136 3734 3930 3566 6539 3438 3166 3132  a674905fe9481f12
-00003af0: 3239 3465 6231 3166 3264 3364 3366 6431  294eb11f2d3d3fd1
-00003b00: 6164 6232 3033 3134 6261 3839 6539 3466  adb20314ba89e94f
-00003b10: 3434 6564 3539 222c 0d0a 2020 2020 2020  44ed59",..      
-00003b20: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003b30: 363a 3937 3564 3730 6162 3765 3363 3830  6:975d70ab7e3c80
-00003b40: 6133 6665 3836 3030 3164 3837 3531 6636  a3fe86001d8751f6
-00003b50: 3737 3839 3035 6563 3732 3366 3562 3131  778905ec723f5b11
-00003b60: 3061 6564 3165 3435 3064 6139 6434 6237  0aed1e450da9d4b7
-00003b70: 6632 222c 0d0a 2020 2020 2020 2020 2020  f2",..          
-00003b80: 2020 2020 2020 2273 6861 3235 363a 3937        "sha256:97
-00003b90: 3662 3963 3432 6662 3261 3433 6562 6633  6b9c42fb2a43ebf3
-00003ba0: 3034 6661 3764 3461 3331 3065 3566 3136  04fa7d4a310e5f16
-00003bb0: 6363 3939 3939 3266 3333 6563 6564 3931  cc99992f33eced91
-00003bc0: 6566 3666 3930 3862 6438 6633 3364 222c  ef6f908bd8f33d",
-00003bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003be0: 2020 2273 6861 3235 363a 3965 3331 6362    "sha256:9e31cb
-00003bf0: 3634 6437 6465 3662 3666 3039 3730 3262  64d7de6b6f09702b
-00003c00: 6232 3763 3032 6431 3930 3462 3361 6562  b27c02d1904b3aeb
-00003c10: 6663 6136 3130 6331 3237 3732 3435 3263  fca610c12772452c
-00003c20: 3465 3663 3231 6130 6433 222c 0d0a 2020  4e6c21a0d3",..  
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003c40: 6861 3235 363a 6133 3432 3234 3266 6532  ha256:a342242fe2
-00003c50: 3234 3037 6633 6331 3766 3462 3439 3932  2407f3c17f4b4992
-00003c60: 3736 6130 3262 3031 6538 3066 3836 3166  76a02b01e80f861f
-00003c70: 3136 3832 6164 3164 3935 6230 3430 3138  1682ad1d95b04018
-00003c80: 6530 6330 6434 222c 0d0a 2020 2020 2020  e0c0d4",..      
-00003c90: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003ca0: 363a 6133 6433 3361 3662 3365 6165 3837  6:a3d33a6b3eae87
-00003cb0: 6365 6165 6661 3931 6666 6463 3133 3062  ceaefa91ffdc130b
-00003cc0: 3565 3835 3336 3138 3263 6436 6466 6462  5e8536182cd6dfdb
-00003cd0: 6663 3161 6135 3662 3436 6666 3863 3836  fc1aa56b46ff8c86
-00003ce0: 6465 222c 0d0a 2020 2020 2020 2020 2020  de",..          
-00003cf0: 2020 2020 2020 2273 6861 3235 363a 6138        "sha256:a8
-00003d00: 3935 6663 6337 6231 3563 3366 6337 3262  95fcc7b15c3fc72b
-00003d10: 6562 3433 6364 6362 6466 3064 6462 3764  eb43cdcbdf0ddb7d
-00003d20: 3265 6263 3935 3965 6461 6339 6365 6633  2ebc959edac9cef3
-00003d30: 3930 6230 6431 3466 3339 6638 6139 222c  90b0d14f39f8a9",
-00003d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003d50: 2020 2273 6861 3235 363a 6166 6231 3766    "sha256:afb17f
-00003d60: 3834 6435 3630 3638 6137 6332 3966 3566  84d56068a7c29f5f
-00003d70: 6133 3762 6664 3338 6435 6162 6136 3965  a37bfd38d5aba69e
-00003d80: 3333 3034 6166 3038 6565 3934 6461 3865  3304af08ee94da8e
-00003d90: 6435 6230 3836 3538 3333 222c 0d0a 2020  d5b0865833",..  
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003db0: 6861 3235 363a 6231 6335 3436 6163 6130  ha256:b1c546aca0
-00003dc0: 6361 3464 3032 3839 3031 6438 3235 3031  ca4d028901d82501
-00003dd0: 3564 6338 6534 6435 3661 6163 3462 3534  5dc8e4d56aac4b54
-00003de0: 3138 3737 3639 3065 6237 3634 3930 6631  1877690eb76490f1
-00003df0: 6463 3865 6430 222c 0d0a 2020 2020 2020  dc8ed0",..      
-00003e00: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003e10: 363a 6232 3930 3139 6337 3630 3339 6463  6:b29019c76039dc
-00003e20: 3363 3066 6438 3135 6334 3133 3932 6130  3c0fd815c41392a0
-00003e30: 3434 6365 3535 3564 3962 6364 6433 3862  44ce555d9bcdd38b
-00003e40: 3066 6236 3066 6234 6364 3865 3437 3562  0fb60fb4cd8e475b
-00003e50: 6139 222c 0d0a 2020 2020 2020 2020 2020  a9",..          
-00003e60: 2020 2020 2020 2273 6861 3235 363a 6234        "sha256:b4
-00003e70: 3635 3137 6330 3263 6364 3038 3039 3266  6517c02ccd08092f
-00003e80: 3466 6139 3966 3234 6333 6238 3364 3866  4fa99f24c3b83d8f
-00003e90: 3932 6637 3339 6234 3635 3762 3066 3134  92f739b4657b0f14
-00003ea0: 3632 3436 6130 6361 3661 3833 3164 222c  6246a0ca6a831d",
-00003eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003ec0: 2020 2273 6861 3235 363a 6237 6161 3566    "sha256:b7aa5f
-00003ed0: 3861 3431 3231 3733 3630 6536 3030 6461  8a41217360e600da
-00003ee0: 3634 3630 3034 6638 3738 3235 3061 3064  646004f878250a0d
-00003ef0: 3637 3338 6263 6463 3131 6130 6133 3939  6738bcdc11a0a399
-00003f00: 3238 6437 6463 3230 3530 222c 0d0a 2020  28d7dc2050",..  
-00003f10: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003f20: 6861 3235 363a 6237 6234 6339 3731 6630  ha256:b7b4c971f0
-00003f30: 3565 3661 6534 3930 6665 6638 3532 6332  5e6ae490fef852c2
-00003f40: 3138 6230 6537 3964 3465 3532 6637 3965  18b0e79d4e52f79e
-00003f50: 6630 6338 3437 3535 3636 3538 3461 3866  f0c8475566584a8f
-00003f60: 6233 6530 3164 222c 0d0a 2020 2020 2020  b3e01d",..      
-00003f70: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00003f80: 363a 6261 3930 6139 3536 3362 6134 3461  6:ba90a9563ba44a
-00003f90: 3732 6664 6132 6538 3533 3032 6333 6162  72fda2e85302c3ab
-00003fa0: 6337 3163 3535 3839 6365 6136 3038 6361  c71c5589cea608ca
-00003fb0: 3136 6332 3262 3938 3034 3236 3261 6165  16c22b9804262aae
-00003fc0: 6236 222c 0d0a 2020 2020 2020 2020 2020  b6",..          
-00003fd0: 2020 2020 2020 2273 6861 3235 363a 6362        "sha256:cb
-00003fe0: 3031 3766 6431 6232 3630 3365 6635 3965  017fd1b2603ef59e
-00003ff0: 3337 3462 6132 3036 3366 3539 3361 6265  374ba2063f593abe
-00004000: 3066 6334 3566 3261 6439 6162 6464 6535  0fc45f2ad9abdde5
-00004010: 6234 6438 3362 6439 3232 6133 3533 222c  b4d83bd922a353",
-00004020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004030: 2020 2273 6861 3235 363a 6432 3236 3536    "sha256:d22656
-00004040: 3336 3866 3065 3631 3839 6532 3437 3232  368f0e6189e24722
-00004050: 3231 3465 6438 6436 3662 3830 3232 6462  214ed8d66b8022db
-00004060: 3139 6431 3832 3932 3762 3961 3234 3861  19d182927b9a248a
-00004070: 3261 3861 3266 3637 6562 222c 0d0a 2020  2a8a2f67eb",..  
-00004080: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00004090: 6861 3235 363a 6432 6332 6462 3766 6438  ha256:d2c2db7fd8
-000040a0: 3265 3962 3732 3933 3739 3639 6263 6561  2e9b72937969bcea
-000040b0: 6334 6436 6361 3839 3636 3064 6230 6130  c4d6ca89660db0a0
-000040c0: 3936 3736 3134 6365 3234 3831 6538 3161  967614ce2481e81a
-000040d0: 3062 3737 3165 222c 0d0a 2020 2020 2020  0b771e",..      
-000040e0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000040f0: 363a 6433 3962 3562 3466 3261 3636 6363  6:d39b5b4f2a66cc
-00004100: 6165 3862 3732 3633 6163 3363 3831 3730  ae8b7263ac3c8170
-00004110: 3939 3462 3635 3236 3637 3937 6662 3936  994b65266797fb96
-00004120: 6362 6266 6433 6662 3562 3233 3932 3164  cbbfd3fb5b23921d
-00004130: 6238 222c 0d0a 2020 2020 2020 2020 2020  b8",..          
-00004140: 2020 2020 2020 2273 6861 3235 363a 6436        "sha256:d6
-00004150: 3261 3563 3764 6164 3131 3031 3563 3636  2a5c7dad11015c66
-00004160: 6662 6239 6438 3831 6263 3463 6161 3562  fbb9d881bc4caa5b
-00004170: 3132 6631 3632 3932 6638 3537 3834 3264  12f16292f857842d
-00004180: 3964 3138 3731 3539 3566 3434 3935 222c  9d1871595f4495",
-00004190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000041a0: 2020 2273 6861 3235 363a 6537 6439 3430    "sha256:e7d940
-000041b0: 3532 3931 6336 3932 3836 3139 3430 3364  5291c6928619403d
-000041c0: 6231 6431 3062 6430 3738 3838 3838 3865  b1d10bd07888888e
-000041d0: 6331 6162 6362 6439 3734 3866 6461 6139  c1abcbd9748fdaa9
-000041e0: 3731 6437 6436 3631 6232 222c 0d0a 2020  71d7d661b2",..  
-000041f0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00004200: 6861 3235 363a 6538 3436 3036 6237 3465  ha256:e84606b74e
-00004210: 6237 6465 3666 6635 3831 6137 3931 3565  b7de6ff581a7915e
-00004220: 3264 6162 3761 3238 6130 3531 3766 6265  2dab7a28a0517fbe
-00004230: 3163 3932 3339 6562 3232 3765 3133 3534  1c9239eb227e1354
-00004240: 3036 3464 6364 222c 0d0a 2020 2020 2020  064dcd",..      
-00004250: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00004260: 363a 6562 3339 3365 3565 6263 3835 3234  6:eb393e5ebc8524
-00004270: 3533 3437 3935 3031 3433 3936 3962 3234  5347950143969b24
-00004280: 3164 3038 6235 3262 3838 6133 6463 3339  1d08b52b88a3dc39
-00004290: 3437 3938 3232 6530 3733 6131 6138 6562  479822e073a1a8eb
-000042a0: 3237 222c 0d0a 2020 2020 2020 2020 2020  27",..          
-000042b0: 2020 2020 2020 2273 6861 3235 363a 6562        "sha256:eb
-000042c0: 6261 3163 6433 3038 6566 3131 3539 3235  ba1cd308ef115925
-000042d0: 3432 3164 3365 3661 3538 3665 3635 3563  421d3e6a586e655c
-000042e0: 6135 6137 3762 3562 6634 3165 3032 6562  a5a77b5bf41e02eb
-000042f0: 3065 3435 3632 6131 3131 6632 6431 222c  0e4562a111f2d1",
-00004300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004310: 2020 2273 6861 3235 363a 6565 3537 3139    "sha256:ee5719
-00004320: 3066 3234 6662 6137 3936 6533 3662 6236  0f24fba796e36bb6
-00004330: 6433 6161 3861 3837 3833 6336 3433 6438  d3aa8a8783c643d8
-00004340: 6661 3937 3630 6338 3966 3761 3938 6162  fa9760c89f7a98ab
-00004350: 3534 3535 6662 6638 3138 222c 0d0a 2020  5455fbf818",..  
-00004360: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00004370: 6861 3235 363a 6632 6636 3766 6531 3262  ha256:f2f67fe12b
-00004380: 3232 6364 3133 3064 3334 6430 6566 3739  22cd130d34d0ef79
-00004390: 3230 3630 3631 6266 6235 6564 6135 3266  206061bfb5eda52f
-000043a0: 6562 3663 6530 6462 6130 3634 3465 3230  eb6ce0dba0644e20
-000043b0: 6130 3363 6634 222c 0d0a 2020 2020 2020  a03cf4",..      
-000043c0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000043d0: 363a 6636 3935 3134 3037 3339 3162 3633  6:f6951407391b63
-000043e0: 3935 3034 6533 6233 6265 3531 6237 6261  9504e3b3be51b7ba
-000043f0: 3566 3335 3238 6164 6266 3161 3861 6333  5f3528adbf1a8ac3
-00004400: 3330 3262 3638 3765 6361 6261 6266 3932  302b687ecababf92
-00004410: 3965 222c 0d0a 2020 2020 2020 2020 2020  9e",..          
-00004420: 2020 2020 2020 2273 6861 3235 363a 6637        "sha256:f7
-00004430: 3566 3731 3638 6162 3235 6464 3933 3131  5f7168ab25dd9311
-00004440: 3063 3861 3831 3137 6132 3234 3530 6331  0c8a8117a22450c1
-00004450: 3939 3736 6166 6263 3434 3233 3463 6266  9976afbc44234cbf
-00004460: 3731 3438 3130 3934 6331 6238 3530 222c  71481094c1b850",
-00004470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004480: 2020 2273 6861 3235 363a 6664 6563 3965    "sha256:fdec9e
-00004490: 3863 6266 3133 6135 6266 3633 3239 3066  8cbf13a5bf63290f
-000044a0: 6336 3031 3364 3231 3661 3463 3732 3332  c6013d216a4c7232
-000044b0: 6566 6235 3135 3438 3539 3463 6133 3633  efb51548594ca363
-000044c0: 3161 3766 3133 6333 6133 220d 0a20 2020  1a7f13c3a3"..   
-000044d0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-000044e0: 2020 2020 2020 2020 2022 696e 6465 7822           "index"
-000044f0: 3a20 2270 7970 6922 2c0d 0a20 2020 2020  : "pypi",..     
-00004500: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-00004510: 3a20 223d 3d37 2e32 2e37 220d 0a20 2020  : "==7.2.7"..   
-00004520: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00004530: 2022 6469 7374 6c69 6222 3a20 7b0d 0a20   "distlib": {.. 
-00004540: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
-00004550: 6573 223a 205b 0d0a 2020 2020 2020 2020  es": [..        
-00004560: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00004570: 3134 6261 6432 6439 6230 3464 3361 3336  14bad2d9b04d3a36
-00004580: 3132 3761 6339 3766 3330 6231 3261 3139  127ac97f30b12a19
-00004590: 3236 3866 3231 3130 3633 6438 6638 6565  268f211063d8f8ee
-000045a0: 3466 3437 3130 3838 3936 6531 3162 3436  4f47108896e11b46
-000045b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000045c0: 2020 2020 2273 6861 3235 363a 6633 3563      "sha256:f35c
-000045d0: 3462 3639 3235 3432 6361 3131 3064 6537  4b692542ca110de7
-000045e0: 6566 3062 6561 3434 6437 3339 3831 6361  ef0bea44d73981ca
-000045f0: 6562 3334 6361 3062 3962 3662 3265 3664  eb34ca0b9b6b2e6d
-00004600: 3737 3930 6464 6138 6638 3065 220d 0a20  7790dda8f80e".. 
-00004610: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00004620: 2020 2020 2020 2020 2020 2022 7665 7273             "vers
-00004630: 696f 6e22 3a20 223d 3d30 2e33 2e36 220d  ion": "==0.3.6".
-00004640: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00004650: 2020 2020 2022 646f 6375 7469 6c73 223a       "docutils":
-00004660: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00004670: 2268 6173 6865 7322 3a20 5b0d 0a20 2020  "hashes": [..   
-00004680: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00004690: 6132 3536 3a39 3666 3338 3761 3263 3535  a256:96f387a2c55
-000046a0: 3632 6462 3434 3736 6630 3966 3133 6262  62db4476f09f13bb
-000046b0: 6162 3231 3932 6537 3634 6361 6330 3865  ab2192e764cac08e
-000046c0: 6262 6633 6133 3461 3935 6439 6231 6534  bbf3a34a95d9b1e4
-000046d0: 6135 3964 3622 2c0d 0a20 2020 2020 2020  a59d6",..       
-000046e0: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
-000046f0: 3a66 3038 6134 6532 3736 6333 6131 3538  :f08a4e276c3a158
-00004700: 3361 3836 6463 6533 6533 3461 6261 3366  3a86dce3e34aba3f
-00004710: 6530 3464 3032 6262 6132 6464 3531 6564  e04d02bba2dd51ed
-00004720: 3136 3130 3632 3434 6538 6139 3233 6533  16106244e8a923e3
-00004730: 6222 0d0a 2020 2020 2020 2020 2020 2020  b"..            
-00004740: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00004750: 226d 6172 6b65 7273 223a 2022 7079 7468  "markers": "pyth
-00004760: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2733  on_version >= '3
-00004770: 2e37 2722 2c0d 0a20 2020 2020 2020 2020  .7'",..         
-00004780: 2020 2022 7665 7273 696f 6e22 3a20 223d     "version": "=
-00004790: 3d30 2e32 302e 3122 0d0a 2020 2020 2020  =0.20.1"..      
-000047a0: 2020 7d2c 0d0a 2020 2020 2020 2020 2266    },..        "f
-000047b0: 696c 656c 6f63 6b22 3a20 7b0d 0a20 2020  ilelock": {..   
-000047c0: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
-000047d0: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-000047e0: 2020 2020 2020 2273 6861 3235 363a 3432        "sha256:42
-000047f0: 6631 6534 6666 3262 3439 3733 3131 3231  f1e4ff2b49731121
-00004800: 3364 3631 6164 3761 6163 3566 6564 3930  3d61ad7aac5fed90
-00004810: 3530 3630 3865 3533 3039 3537 3366 3130  50608e5309573f10
-00004820: 3165 6566 6139 3431 3433 3133 3461 222c  1eefa94143134a",
-00004830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004840: 2020 2273 6861 3235 363a 3832 6231 6637    "sha256:82b1f7
-00004850: 6461 3436 6630 6165 3432 6162 6631 6263  da46f0ae42abf1bc
-00004860: 3738 6535 3438 3636 3766 3438 3461 6335  78e548667f484ac5
-00004870: 3964 3262 6365 6333 3863 3731 3363 6565  9d2bcec38c713cee
-00004880: 3765 3265 6235 3165 3833 220d 0a20 2020  7e2eb51e83"..   
-00004890: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-000048a0: 2020 2020 2020 2020 2022 6d61 726b 6572           "marker
-000048b0: 7322 3a20 2270 7974 686f 6e5f 7665 7273  s": "python_vers
-000048c0: 696f 6e20 3e3d 2027 332e 3727 222c 0d0a  ion >= '3.7'",..
-000048d0: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
-000048e0: 7369 6f6e 223a 2022 3d3d 332e 3132 2e31  sion": "==3.12.1
-000048f0: 220d 0a20 2020 2020 2020 207d 2c0d 0a20  "..        },.. 
-00004900: 2020 2020 2020 2022 666c 616b 6538 223a         "flake8":
-00004910: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00004920: 2268 6173 6865 7322 3a20 5b0d 0a20 2020  "hashes": [..   
-00004930: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00004940: 6132 3536 3a33 3833 3337 3934 6532 3766  a256:3833794e27f
-00004950: 6636 3465 6134 6539 6366 3564 3431 3030  f64ea4e9cf5d4100
-00004960: 3832 6138 6239 3766 6631 6130 3663 3136  82a8b97ff1a06c16
-00004970: 6161 3364 3230 3237 3333 3963 6430 6631  aa3d2027339cd0f1
-00004980: 3139 3563 3722 2c0d 0a20 2020 2020 2020  195c7",..       
-00004990: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
-000049a0: 3a63 3631 3030 3765 3736 3635 3561 6637  :c61007e76655af7
-000049b0: 3565 3637 3835 6139 3331 6634 3532 3931  5e6785a931f45291
-000049c0: 3562 3337 3164 6334 3866 3536 6566 6437  5b371dc48f56efd7
-000049d0: 3635 3234 3763 3866 6536 3866 3262 3138  65247c8fe68f2b18
-000049e0: 3122 0d0a 2020 2020 2020 2020 2020 2020  1"..            
-000049f0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00004a00: 2269 6e64 6578 223a 2022 7079 7069 222c  "index": "pypi",
-00004a10: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-00004a20: 6572 7369 6f6e 223a 2022 3d3d 362e 302e  ersion": "==6.0.
-00004a30: 3022 0d0a 2020 2020 2020 2020 7d2c 0d0a  0"..        },..
-00004a40: 2020 2020 2020 2020 2269 646e 6122 3a20          "idna": 
-00004a50: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00004a60: 6861 7368 6573 223a 205b 0d0a 2020 2020  hashes": [..    
-00004a70: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00004a80: 3235 363a 3831 3466 3532 3865 3864 6561  256:814f528e8dea
-00004a90: 6437 6433 3239 3833 3362 3931 6335 6661  d7d329833b91c5fa
-00004aa0: 6138 3764 3630 6266 3731 3832 3463 6431  a87d60bf71824cd1
-00004ab0: 3261 3735 3330 6235 3532 3630 3633 6430  2a7530b5526063d0
-00004ac0: 3263 6234 222c 0d0a 2020 2020 2020 2020  2cb4",..        
-00004ad0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00004ae0: 3930 6237 3765 3739 6561 6133 6562 6136  90b77e79eaa3eba6
-00004af0: 6465 3831 3961 3063 3434 3263 3062 3463  de819a0c442c0b4c
-00004b00: 6565 6663 3334 3161 3761 3261 6237 3764  eefc341a7a2ab77d
-00004b10: 3735 3632 6266 3439 6634 3235 6335 6332  7562bf49f425c5c2
-00004b20: 220d 0a20 2020 2020 2020 2020 2020 205d  "..            ]
-00004b30: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00004b40: 6d61 726b 6572 7322 3a20 2270 7974 686f  markers": "pytho
-00004b50: 6e5f 7665 7273 696f 6e20 3e3d 2027 332e  n_version >= '3.
-00004b60: 3527 222c 0d0a 2020 2020 2020 2020 2020  5'",..          
-00004b70: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
-00004b80: 332e 3422 0d0a 2020 2020 2020 2020 7d2c  3.4"..        },
-00004b90: 0d0a 2020 2020 2020 2020 2269 6d70 6f72  ..        "impor
-00004ba0: 746c 6962 2d6d 6574 6164 6174 6122 3a20  tlib-metadata": 
-00004bb0: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00004bc0: 6861 7368 6573 223a 205b 0d0a 2020 2020  hashes": [..    
-00004bd0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00004be0: 3235 363a 3433 6464 3238 3661 3263 6438  256:43dd286a2cd8
-00004bf0: 3939 3564 3565 6165 6637 6665 6532 3036  995d5eaef7fee206
-00004c00: 3633 3430 3432 3362 3831 3865 6433 6664  6340423b818ed3fd
-00004c10: 3730 6164 6630 6261 6435 6631 6661 6335  70adf0bad5f1fac5
-00004c20: 3366 6564 222c 0d0a 2020 2020 2020 2020  3fed",..        
-00004c30: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00004c40: 3932 3530 3163 6466 3963 6336 3665 6264  92501cdf9cc66ebd
-00004c50: 3365 3631 3266 3162 3466 3063 3037 3635  3e612f1b4f0c0765
-00004c60: 6466 6134 3266 3066 6133 3866 6662 3331  dfa42f0fa38ffb31
-00004c70: 3962 3662 6438 3464 6436 3735 6437 3035  9b6bd84dd675d705
-00004c80: 220d 0a20 2020 2020 2020 2020 2020 205d  "..            ]
-00004c90: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00004ca0: 6d61 726b 6572 7322 3a20 2270 7974 686f  markers": "pytho
-00004cb0: 6e5f 7665 7273 696f 6e20 3e3d 2027 332e  n_version >= '3.
-00004cc0: 3727 222c 0d0a 2020 2020 2020 2020 2020  7'",..          
-00004cd0: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
-00004ce0: 362e 362e 3022 0d0a 2020 2020 2020 2020  6.6.0"..        
-00004cf0: 7d2c 0d0a 2020 2020 2020 2020 2269 6e69  },..        "ini
-00004d00: 636f 6e66 6967 223a 207b 0d0a 2020 2020  config": {..    
-00004d10: 2020 2020 2020 2020 2268 6173 6865 7322          "hashes"
-00004d20: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
-00004d30: 2020 2020 2022 7368 6132 3536 3a32 6439       "sha256:2d9
-00004d40: 3165 3133 3562 6637 3264 3331 6134 3130  1e135bf72d31a410
-00004d50: 6231 3763 3136 6461 3631 3061 3832 6362  b17c16da610a82cb
-00004d60: 3535 6636 6230 3437 3764 3161 3930 3231  55f6b0477d1a9021
-00004d70: 3334 6232 3461 3435 3562 3862 3322 2c0d  34b24a455b8b3",.
-00004d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d90: 2022 7368 6132 3536 3a62 3661 3835 3837   "sha256:b6a8587
-00004da0: 3161 3739 6432 6533 6232 3264 3264 3162  1a79d2e3b22d2d1b
-00004db0: 3934 6163 3238 3234 3232 3661 3633 6336  94ac2824226a63c6
-00004dc0: 6237 3431 6338 3866 3761 6539 3735 6631  b741c88f7ae975f1
-00004dd0: 3862 3637 3738 3337 3422 0d0a 2020 2020  8b6778374"..    
-00004de0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00004df0: 2020 2020 2020 2020 226d 6172 6b65 7273          "markers
-00004e00: 223a 2022 7079 7468 6f6e 5f76 6572 7369  ": "python_versi
-00004e10: 6f6e 203e 3d20 2733 2e37 2722 2c0d 0a20  on >= '3.7'",.. 
-00004e20: 2020 2020 2020 2020 2020 2022 7665 7273             "vers
-00004e30: 696f 6e22 3a20 223d 3d32 2e30 2e30 220d  ion": "==2.0.0".
-00004e40: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00004e50: 2020 2020 2022 6973 6f72 7422 3a20 7b0d       "isort": {.
-00004e60: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
-00004e70: 7368 6573 223a 205b 0d0a 2020 2020 2020  shes": [..      
-00004e80: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-00004e90: 363a 3862 6566 3764 6465 3234 3132 3738  6:8bef7dde241278
-00004ea0: 3832 3461 3664 3833 6634 3461 3534 3437  824a6d83f44a5447
-00004eb0: 3039 6230 3635 3139 3162 3935 6236 6535  09b065191b95b6e5
-00004ec0: 3038 3934 6264 6337 3232 6663 6261 3035  0894bdc722fcba05
-00004ed0: 3034 222c 0d0a 2020 2020 2020 2020 2020  04",..          
-00004ee0: 2020 2020 2020 2273 6861 3235 363a 6638        "sha256:f8
-00004ef0: 3463 3238 3138 3337 3665 3636 6366 3834  4c2818376e66cf84
-00004f00: 3364 3439 3734 3836 6561 3866 6564 3837  3d497486ea8fed87
-00004f10: 3030 6233 3430 6633 3038 6630 3736 6336  00b340f308f076c6
-00004f20: 6662 3132 3239 6466 6633 3138 6236 220d  fb1229dff318b6".
-00004f30: 0a20 2020 2020 2020 2020 2020 205d 2c0d  .            ],.
-00004f40: 0a20 2020 2020 2020 2020 2020 2022 696e  .            "in
-00004f50: 6465 7822 3a20 2270 7970 6922 2c0d 0a20  dex": "pypi",.. 
-00004f60: 2020 2020 2020 2020 2020 2022 7665 7273             "vers
-00004f70: 696f 6e22 3a20 223d 3d35 2e31 322e 3022  ion": "==5.12.0"
-00004f80: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00004f90: 2020 2020 2020 226a 6172 6163 6f2e 636c        "jaraco.cl
-00004fa0: 6173 7365 7322 3a20 7b0d 0a20 2020 2020  asses": {..     
-00004fb0: 2020 2020 2020 2022 6861 7368 6573 223a         "hashes":
-00004fc0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00004fd0: 2020 2020 2273 6861 3235 363a 3233 3533      "sha256:2353
-00004fe0: 6465 3332 3838 6263 3662 3832 3132 3037  de3288bc6b821207
-00004ff0: 3532 3230 3163 3662 3163 3161 3134 6230  52201c6b1c1a14b0
-00005000: 3538 3236 3766 6134 3234 6564 3563 6535  58267fa424ed5ce5
-00005010: 3938 3465 3362 3932 3231 3538 222c 0d0a  984e3b922158",..
-00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 2273 6861 3235 363a 3839 3535 3966 6135  "sha256:89559fa5
-00005040: 6331 6433 6333 3465 6666 3666 3633 3161  c1d3c34eff6f631a
-00005050: 6438 3062 6232 3166 3337 3864 6263 6262  d80bb21f378dbcbb
-00005060: 3335 6464 3136 3166 6432 6336 6239 3366  35dd161fd2c6b93f
-00005070: 3562 6532 6639 3861 220d 0a20 2020 2020  5be2f98a"..     
-00005080: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-00005090: 2020 2020 2020 2022 6d61 726b 6572 7322         "markers"
-000050a0: 3a20 2270 7974 686f 6e5f 7665 7273 696f  : "python_versio
-000050b0: 6e20 3e3d 2027 332e 3727 222c 0d0a 2020  n >= '3.7'",..  
-000050c0: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
-000050d0: 6f6e 223a 2022 3d3d 332e 322e 3322 0d0a  on": "==3.2.3"..
-000050e0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000050f0: 2020 2020 226b 6579 7269 6e67 223a 207b      "keyring": {
-00005100: 0d0a 2020 2020 2020 2020 2020 2020 2268  ..            "h
-00005110: 6173 6865 7322 3a20 5b0d 0a20 2020 2020  ashes": [..     
-00005120: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00005130: 3536 3a37 3731 6564 3261 3931 3930 3933  56:771ed2a919093
-00005140: 3839 6564 3631 3438 3633 3164 6536 3738  89ed6148631de678
-00005150: 6638 3264 6463 3733 3733 3764 3835 6139  f82ddc73737d85a9
-00005160: 3237 6633 3832 6138 6131 6231 3537 3839  27f382a8a1b15789
-00005170: 3863 6422 2c0d 0a20 2020 2020 2020 2020  8cd",..         
-00005180: 2020 2020 2020 2022 7368 6132 3536 3a62         "sha256:b
-00005190: 6132 6531 3561 3962 3335 6532 3139 3038  a2e15a9b35e21908
-000051a0: 6430 6161 6634 6530 6134 3761 6363 3532  d0aaf4e0a47acc52
-000051b0: 6436 6165 3333 3434 3464 6630 6461 3262  d6ae33444df0da2b
-000051c0: 3439 6434 3161 3436 6566 3664 3637 3822  49d41a46ef6d678"
-000051d0: 0d0a 2020 2020 2020 2020 2020 2020 5d2c  ..            ],
-000051e0: 0d0a 2020 2020 2020 2020 2020 2020 226d  ..            "m
-000051f0: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
-00005200: 5f76 6572 7369 6f6e 203e 3d20 2733 2e37  _version >= '3.7
-00005210: 2722 2c0d 0a20 2020 2020 2020 2020 2020  '",..           
-00005220: 2022 7665 7273 696f 6e22 3a20 223d 3d32   "version": "==2
-00005230: 332e 3133 2e31 220d 0a20 2020 2020 2020  3.13.1"..       
-00005240: 207d 2c0d 0a20 2020 2020 2020 2022 6d61   },..        "ma
-00005250: 726b 646f 776e 2d69 742d 7079 223a 207b  rkdown-it-py": {
-00005260: 0d0a 2020 2020 2020 2020 2020 2020 2268  ..            "h
-00005270: 6173 6865 7322 3a20 5b0d 0a20 2020 2020  ashes": [..     
-00005280: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00005290: 3536 3a33 3535 3231 3638 3435 6336 3062  56:355216845c60b
-000052a0: 6439 3632 3332 6364 3864 3863 3430 6538  d96232cd8d8c40e8
-000052b0: 6639 3736 3563 6338 3666 3436 3838 3065  f9765cc86f46880e
-000052c0: 3433 6138 6664 3232 6463 3161 3161 3863  43a8fd22dc1a1a8c
-000052d0: 6162 3122 2c0d 0a20 2020 2020 2020 2020  ab1",..         
-000052e0: 2020 2020 2020 2022 7368 6132 3536 3a65         "sha256:e
-000052f0: 3366 3630 6139 3466 6130 3636 6463 3532  3f60a94fa066dc52
-00005300: 6563 3736 3636 3165 3337 6338 3531 6362  ec76661e37c851cb
-00005310: 3233 3264 3932 6639 3838 3662 3135 6362  232d92f9886b15cb
-00005320: 3536 3061 6161 6461 3264 6638 6665 6222  560aaada2df8feb"
-00005330: 0d0a 2020 2020 2020 2020 2020 2020 5d2c  ..            ],
-00005340: 0d0a 2020 2020 2020 2020 2020 2020 226d  ..            "m
-00005350: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
-00005360: 5f76 6572 7369 6f6e 203e 3d20 2733 2e38  _version >= '3.8
-00005370: 2722 2c0d 0a20 2020 2020 2020 2020 2020  '",..           
-00005380: 2022 7665 7273 696f 6e22 3a20 223d 3d33   "version": "==3
-00005390: 2e30 2e30 220d 0a20 2020 2020 2020 207d  .0.0"..        }
-000053a0: 2c0d 0a20 2020 2020 2020 2022 6d63 6361  ,..        "mcca
-000053b0: 6265 223a 207b 0d0a 2020 2020 2020 2020  be": {..        
-000053c0: 2020 2020 2268 6173 6865 7322 3a20 5b0d      "hashes": [.
-000053d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000053e0: 2022 7368 6132 3536 3a33 3438 6530 3234   "sha256:348e024
-000053f0: 3063 3333 6236 3062 6264 6634 6535 3233  0c33b60bbdf4e523
-00005400: 3139 3265 6639 3139 6632 3863 6232 6333  192ef919f28cb2c3
-00005410: 6437 6435 6337 3739 3466 3734 3030 3932  d7d5c7794f740092
-00005420: 3930 6632 3336 3332 3522 2c0d 0a20 2020  90f236325",..   
-00005430: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00005440: 6132 3536 3a36 6332 6433 3061 6236 6265  a256:6c2d30ab6be
-00005450: 3065 3461 3436 3931 3937 3831 3830 3762  0e4a46919781807b
-00005460: 3466 3064 3833 3465 6264 6436 6336 6533  4f0d834ebdd6c6e3
-00005470: 6463 6130 6264 6135 6131 3566 3836 3334  dca0bda5a15f8634
-00005480: 3237 6236 6522 0d0a 2020 2020 2020 2020  27b6e"..        
-00005490: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
-000054a0: 2020 2020 226d 6172 6b65 7273 223a 2022      "markers": "
-000054b0: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
-000054c0: 3d20 2733 2e36 2722 2c0d 0a20 2020 2020  = '3.6'",..     
-000054d0: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-000054e0: 3a20 223d 3d30 2e37 2e30 220d 0a20 2020  : "==0.7.0"..   
-000054f0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00005500: 2022 6d64 7572 6c22 3a20 7b0d 0a20 2020   "mdurl": {..   
-00005510: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
-00005520: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00005530: 2020 2020 2020 2273 6861 3235 363a 3834        "sha256:84
-00005540: 3030 3861 3431 6535 3136 3135 6134 3966  008a41e51615a49f
-00005550: 6339 3936 3631 3931 6666 3931 3530 3965  c9966191ff91509e
-00005560: 3363 3430 6239 3339 3137 3665 3634 3366  3c40b939176e643f
-00005570: 6435 3061 3563 3231 3936 6238 6638 222c  d50a5c2196b8f8",
-00005580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005590: 2020 2273 6861 3235 363a 6262 3431 3364    "sha256:bb413d
-000055a0: 3239 6635 6565 6133 3866 3331 6464 3437  29f5eea38f31dd47
-000055b0: 3534 6464 3733 3737 6434 3436 3531 3136  54dd7377d4465116
-000055c0: 6662 3230 3735 3835 6639 3762 6639 3235  fb207585f97bf925
-000055d0: 3538 3836 3837 6331 6261 220d 0a20 2020  588687c1ba"..   
-000055e0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-000055f0: 2020 2020 2020 2020 2022 6d61 726b 6572           "marker
-00005600: 7322 3a20 2270 7974 686f 6e5f 7665 7273  s": "python_vers
-00005610: 696f 6e20 3e3d 2027 332e 3727 222c 0d0a  ion >= '3.7'",..
-00005620: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
-00005630: 7369 6f6e 223a 2022 3d3d 302e 312e 3222  sion": "==0.1.2"
-00005640: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00005650: 2020 2020 2020 226d 6f72 652d 6974 6572        "more-iter
-00005660: 746f 6f6c 7322 3a20 7b0d 0a20 2020 2020  tools": {..     
-00005670: 2020 2020 2020 2022 6861 7368 6573 223a         "hashes":
-00005680: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00005690: 2020 2020 2273 6861 3235 363a 6361 6261      "sha256:caba
-000056a0: 6133 3431 6164 3033 3839 6561 3833 6331  a341ad0389ea83c1
-000056b0: 3761 3934 3536 3661 3533 6165 3463 3964  7a94566a53ae4c9d
-000056c0: 3037 3334 3938 3631 6563 6231 3464 6336  07349861ecb14dc6
-000056d0: 6430 3334 3563 6639 6163 3564 222c 0d0a  d0345cf9ac5d",..
-000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2273 6861 3235 363a 6432 6263 3766 3032  "sha256:d2bc7f02
-00005700: 3434 3665 3836 6136 3839 3131 6535 3864  446e86a68911e58d
-00005710: 6564 3736 6436 3536 3165 6561 3030 6364  ed76d6561eea00cd
-00005720: 6466 6232 6139 3165 3730 3139 6262 6235  dfb2a91e7019bbb5
-00005730: 3836 6337 3939 6633 220d 0a20 2020 2020  86c799f3"..     
-00005740: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-00005750: 2020 2020 2020 2022 6d61 726b 6572 7322         "markers"
-00005760: 3a20 2270 7974 686f 6e5f 7665 7273 696f  : "python_versio
-00005770: 6e20 3e3d 2027 332e 3727 222c 0d0a 2020  n >= '3.7'",..  
-00005780: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
-00005790: 6f6e 223a 2022 3d3d 392e 312e 3022 0d0a  on": "==9.1.0"..
-000057a0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000057b0: 2020 2020 226d 7970 7922 3a20 7b0d 0a20      "mypy": {.. 
-000057c0: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
-000057d0: 6573 223a 205b 0d0a 2020 2020 2020 2020  es": [..        
-000057e0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-000057f0: 3163 3463 3432 6336 3061 3831 3033 6561  1c4c42c60a8103ea
-00005800: 6434 6331 6330 3630 6163 3363 6464 3366  d4c1c060ac3cdd3f
-00005810: 6630 3165 3138 6664 6463 6536 6631 3031  f01e18fddce6f101
-00005820: 3665 3038 3933 3936 3437 6130 6537 3033  6e08939647a0e703
-00005830: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005840: 2020 2020 2273 6861 3235 363a 3434 3739      "sha256:4479
-00005850: 3764 3033 3161 3431 3531 3666 6366 3563  7d031a41516fcf5c
-00005860: 6266 6136 3532 3236 3562 6239 3934 6535  bfa652265bb994e5
-00005870: 3365 3531 3939 3463 3162 6436 3439 6666  3e51994c1bd649ff
-00005880: 6364 3063 3361 3765 6363 6266 222c 0d0a  cd0c3a7eccbf",..
-00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058a0: 2273 6861 3235 363a 3437 3331 3137 6533  "sha256:473117e3
-000058b0: 3130 6665 6265 3633 3264 6466 3130 6537  10febe632ddf10e7
-000058c0: 3435 6133 3535 3731 3465 3737 3166 6665  45a355714e771ffe
-000058d0: 3533 3466 3036 6462 3430 3730 3237 3735  534f06db40702775
-000058e0: 3035 3636 3134 6334 222c 0d0a 2020 2020  056614c4",..    
-000058f0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00005900: 3235 363a 3463 3939 6333 6563 6632 3233  256:4c99c3ecf223
-00005910: 6366 3239 3532 3633 3864 6139 6364 3832  cf2952638da9cd82
-00005920: 3739 3364 3866 3363 3063 3566 6138 6236  793d8f3c0c5fa8b6
-00005930: 6165 3262 3264 3965 6431 6531 6666 3531  ae2b2d9ed1e1ff51
-00005940: 6261 3835 222c 0d0a 2020 2020 2020 2020  ba85",..        
-00005950: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00005960: 3535 3061 3862 3361 3139 6262 3635 3839  550a8b3a19bb6589
-00005970: 3637 3961 3763 3363 3331 6636 3433 3132  679a7c3c31f64312
-00005980: 6537 6666 3438 3261 3831 3663 3936 6530  e7ff482a816c96e0
-00005990: 6365 6365 6339 6164 3361 3735 3634 6464  cecec9ad3a7564dd
-000059a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000059b0: 2020 2020 2273 6861 3235 363a 3635 3866      "sha256:658f
-000059c0: 6537 6236 3734 3736 3961 3037 3730 6434  e7b674769a0770d4
-000059d0: 6232 3663 6234 6436 6630 3035 6538 3861  b26cb4d6f005e88a
-000059e0: 3434 3266 6538 3234 3436 6630 3230 6265  442fe82446f020be
-000059f0: 3865 3566 3565 6662 3266 6165 222c 0d0a  8e5f5efb2fae",..
+00002fb0: 363a 3065 3166 3932 3865 6166 3534 3639  6:0e1f928eaf5469
+00002fc0: 6331 3165 3838 3666 6530 3838 3561 6432  c11e886fe0885ad2
+00002fd0: 6266 3165 6336 3036 3433 3465 3739 3834  bf1ec606434e7984
+00002fe0: 3261 3837 3932 3737 3839 3561 3530 3934  2a879277895a5094
+00002ff0: 3261 222c 0a20 2020 2020 2020 2020 2020  2a",.           
+00003000: 2020 2020 2022 7368 6132 3536 3a31 3731       "sha256:171
+00003010: 3731 3763 3763 6236 6234 3533 6165 6261  717c7cb6b453aeba
+00003020: 6339 6132 6566 3630 3336 3939 6461 3233  c9a2ef603699da23
+00003030: 3766 3334 3162 3338 6565 6266 6565 3962  7f341b38eebfee9b
+00003040: 6537 3564 3237 6463 3338 6530 3122 2c0a  e75d27dc38e01",.
+00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003060: 2273 6861 3235 363a 3165 3964 3638 3334  "sha256:1e9d6834
+00003070: 3236 3436 3465 3461 3235 3262 6637 3063  26464e4a252bf70c
+00003080: 3334 3938 3735 3630 3535 3031 3666 3939  3498756055016f99
+00003090: 6464 6165 6333 3737 3462 6633 3638 6537  ddaec3774bf368e7
+000030a0: 3662 6265 3032 6236 222c 0a20 2020 2020  6bbe02b6",.     
+000030b0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+000030c0: 3536 3a32 3031 6537 3338 3935 3931 6166  56:201e7389591af
+000030d0: 3430 3935 3061 3634 3830 6264 3965 6466  40950a6480bd9edf
+000030e0: 6138 6564 3034 3334 3666 6638 3030 3032  a8ed04346ff80002
+000030f0: 6365 6331 6136 3663 6163 3435 3439 6331  cec1a66cac4549c1
+00003100: 6164 3722 2c0a 2020 2020 2020 2020 2020  ad7",.          
+00003110: 2020 2020 2020 2273 6861 3235 363a 3234        "sha256:24
+00003120: 3531 3637 6464 3236 3138 3061 6234 6339  5167dd26180ab4c9
+00003130: 3164 3565 3134 3936 6133 3062 6534 6364  1d5e1496a30be4cd
+00003140: 3732 3161 3563 6632 6162 6635 3239 3734  721a5cf2abf52974
+00003150: 6639 3635 6631 3066 3131 3431 3966 222c  f965f10f11419f",
+00003160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003170: 2022 7368 6132 3536 3a32 6165 6532 3734   "sha256:2aee274
+00003180: 6334 3635 3930 3731 3766 3338 6165 3565  c46590717f38ae5e
+00003190: 3436 3530 3938 3864 3161 6633 3430 6665  4650988d1af340fe
+000031a0: 3036 3136 3735 3436 6363 3332 6665 3266  06167546cc32fe2f
+000031b0: 3538 6564 3035 6230 3222 2c0a 2020 2020  58ed05b02",.    
+000031c0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+000031d0: 3235 363a 3265 3037 6235 3432 3834 6533  256:2e07b54284e3
+000031e0: 3831 3533 3163 3837 6637 3835 6636 3133  81531c87f785f613
+000031f0: 6238 3333 3536 3963 3134 6563 6163 6463  b833569c14ecacdc
+00003200: 6238 3564 3536 6232 3563 3436 3232 6331  b85d56b25c4622c1
+00003210: 3663 3363 222c 0a20 2020 2020 2020 2020  6c3c",.         
+00003220: 2020 2020 2020 2022 7368 6132 3536 3a33         "sha256:3
+00003230: 3135 3633 6539 3764 6165 3535 3938 3535  1563e97dae559855
+00003240: 3636 3030 3436 3661 6439 6265 6561 3339  6600466ad9beea39
+00003250: 6662 3034 6530 3232 3965 3631 6331 3265  fb04e0229e61c12e
+00003260: 6161 3230 3665 3061 6132 3032 3036 3322  aa206e0aa202063"
+00003270: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003280: 2020 2273 6861 3235 363a 3333 6436 6433    "sha256:33d6d3
+00003290: 6561 3239 6435 6233 6131 6136 3332 6233  ea29d5b3a1a632b3
+000032a0: 6334 6534 6634 6563 6165 3234 6566 3137  c4e4f4ecae24ef17
+000032b0: 3062 3062 3965 6534 3933 3838 3366 3264  0b0b9ee493883f2d
+000032c0: 6631 3030 3339 3935 3961 222c 0a20 2020  f10039959a",.   
+000032d0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+000032e0: 6132 3536 3a33 6433 3736 6466 3538 6363  a256:3d376df58cc
+000032f0: 3131 3164 6338 6532 3165 3362 3665 3234  111dc8e21e3b6e24
+00003300: 3630 3662 3562 6235 6465 6536 3032 3466  606b5bb5dee6024f
+00003310: 3436 6135 6162 6361 3939 3132 3462 3232  46a5abca99124b22
+00003320: 3239 6566 3522 2c0a 2020 2020 2020 2020  29ef5",.        
+00003330: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00003340: 3431 3962 6664 3263 6161 6532 3638 3632  419bfd2caae26862
+00003350: 3364 6434 3639 6566 6639 3664 3531 3061  3dd469eff96d510a
+00003360: 3932 3063 3930 3932 3862 3630 6632 3037  920c90928b60f207
+00003370: 3364 3739 6638 6665 3262 6263 3539 3539  3d79f8fe2bbc5959
+00003380: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003390: 2020 2022 7368 6132 3536 3a34 3863 3139     "sha256:48c19
+000033a0: 6432 3135 3964 3433 3363 6363 3939 6537  d2159d433ccc99e7
+000033b0: 3239 6365 6165 3764 3532 3933 6662 6666  29ceae7d5293fbff
+000033c0: 6130 6264 6239 3439 3532 6433 3537 3939  a0bdb94952d35799
+000033d0: 3833 6431 6338 6339 6439 3722 2c0a 2020  83d1c8c9d97",.  
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000033f0: 6861 3235 363a 3439 3936 3961 3966 3766  ha256:49969a9f7f
+00003400: 6661 3038 3664 3937 3364 3931 6365 6338  fa086d973d91cec8
+00003410: 6432 6533 3130 3830 3433 3665 6630 6662  d2e31080436ef0fb
+00003420: 3461 3335 3963 6165 3932 3765 3734 3261  4a359cae927e742a
+00003430: 6266 6161 6136 222c 0a20 2020 2020 2020  bfaaa6",.       
+00003440: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00003450: 3a35 3265 6463 3161 3630 6330 6433 3461  :52edc1a60c0d34a
+00003460: 6661 3432 3163 3963 3337 3037 3838 3137  fa421c9c37078817
+00003470: 6232 6536 3761 3339 3263 6162 3137 6439  b2e67a392cab17d9
+00003480: 3732 3833 6236 3463 3538 3333 6634 3237  7283b64c5833f427
+00003490: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
+000034a0: 2020 2020 2273 6861 3235 363a 3533 3738      "sha256:5378
+000034b0: 3931 6165 3863 6535 3965 6636 3364 3031  91ae8ce59ef63d01
+000034c0: 3233 6637 6163 3965 3261 6530 6663 3862  23f7ac9e2ae0fc8b
+000034d0: 3732 6337 6363 6265 3532 3936 6665 6334  72c7ccbe5296fec4
+000034e0: 3566 6436 3839 3637 6236 6339 222c 0a20  5fd68967b6c9",. 
+000034f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003500: 7368 6132 3536 3a35 3462 3839 3633 3736  sha256:54b896376
+00003510: 6162 3536 3362 6433 3834 3533 6365 6362  ab563bd38453cecb
+00003520: 3831 3363 3239 3563 6633 3437 6366 3539  813c295cf347cf59
+00003530: 3036 6538 6234 3164 3334 3062 3033 3231  06e8b41d340b0321
+00003540: 6135 3433 3365 3522 2c0a 2020 2020 2020  a5433e5",.      
+00003550: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00003560: 363a 3538 6332 6363 6332 6630 3065 6362  6:58c2ccc2f00ecb
+00003570: 3531 3235 3363 6265 3564 3864 3731 3232  51253cbe5d8d7122
+00003580: 6133 3435 3930 6661 6339 3634 3661 3936  a34590fac9646a96
+00003590: 3064 3134 3330 6435 6231 3533 3231 6439  0d1430d5b15321d9
+000035a0: 3566 222c 0a20 2020 2020 2020 2020 2020  5f",.           
+000035b0: 2020 2020 2022 7368 6132 3536 3a35 6237       "sha256:5b7
+000035c0: 3534 3031 3631 3739 3062 3266 3238 3134  540161790b2f2814
+000035d0: 3331 3931 6635 6638 6563 3032 6662 3133  3191f5f8ec02fb13
+000035e0: 3236 3630 6666 3137 3562 3737 3437 6239  2660ff175b7747b9
+000035f0: 3564 6362 3737 6163 3236 3536 3222 2c0a  5dcb77ac26562",.
+00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003610: 2273 6861 3235 363a 3562 6161 3036 3432  "sha256:5baa0642
+00003620: 3066 3833 3731 3834 3133 3037 3532 6237  0f837184130752b7
+00003630: 6335 6561 3038 3038 3736 3230 3833 6266  c5ea0808762083bf
+00003640: 3334 3837 6235 3033 3864 3638 6230 3132  3487b5038d68b012
+00003650: 6535 3933 3764 6265 222c 0a20 2020 2020  e5937dbe",.     
+00003660: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00003670: 3536 3a35 6533 3330 6663 3739 6264 3732  56:5e330fc79bd72
+00003680: 3037 6534 3663 3764 3766 6432 6262 3461  07e46c7d7fd2bb4a
+00003690: 6632 3936 3366 3566 3633 3537 3033 3932  f2963f5f63570392
+000036a0: 3535 3433 6137 3062 3939 3537 3462 3066  5543a70b99574b0f
+000036b0: 6561 3922 2c0a 2020 2020 2020 2020 2020  ea9",.          
+000036c0: 2020 2020 2020 2273 6861 3235 363a 3631        "sha256:61
+000036d0: 6239 6135 3238 6662 3334 3833 3733 6334  b9a528fb348373c4
+000036e0: 3333 6538 3936 3635 3335 3037 3462 3830  33e8966535074b80
+000036f0: 3263 3761 3564 3766 3233 6334 6634 3231  2c7a5d7f23c4f421
+00003700: 6536 6336 6532 6631 3639 3761 3666 222c  e6c6e2f1697a6f",
+00003710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003720: 2022 7368 6132 3536 3a36 3334 3236 3730   "sha256:6342670
+00003730: 3631 3138 6237 6635 6366 3662 6236 6338  6118b7f5cf6bb6c8
+00003740: 3935 6463 3231 3564 3861 3431 3864 3539  95dc215d8a418d59
+00003750: 3532 3534 3430 3432 6338 6132 6439 6665  52544042c8a2d9fe
+00003760: 3837 6663 6630 3963 6222 2c0a 2020 2020  87fcf09cb",.    
+00003770: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00003780: 3235 363a 3664 3034 3065 6637 6339 3835  256:6d040ef7c985
+00003790: 3962 6231 3164 6665 6230 3536 6666 3562  9bb11dfeb056ff5b
+000037a0: 3338 3732 3433 3665 3362 3565 3430 3138  3872436e3b5e4018
+000037b0: 3137 6438 3761 3331 6531 3735 3062 3961  17d87a31e1750b9a
+000037c0: 6532 6662 222c 0a20 2020 2020 2020 2020  e2fb",.         
+000037d0: 2020 2020 2020 2022 7368 6132 3536 3a36         "sha256:6
+000037e0: 6634 3833 3531 6436 3635 3735 6635 3335  f48351d66575f535
+000037f0: 3636 3933 3036 6161 3764 3664 3666 3731  669306aa7d6d6f71
+00003800: 6263 3433 3337 3234 3733 6235 3461 3833  bc43372473b54a83
+00003810: 3232 3232 3830 3365 6239 3536 6664 3122  2222803eb956fd1"
+00003820: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003830: 2020 2273 6861 3235 363a 3765 6537 6439    "sha256:7ee7d9
+00003840: 6434 3832 3263 3861 6363 3734 6135 6532  d4822c8acc74a5e2
+00003850: 3663 3530 3630 3464 6666 3832 3437 3130  6c50604dff824710
+00003860: 6263 3864 6534 3234 3930 3463 3039 3832  bc8de424904c0982
+00003870: 6532 3563 3339 6336 6362 222c 0a20 2020  e25c39c6cb",.   
+00003880: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00003890: 6132 3536 3a38 3163 3133 6131 6663 3734  a256:81c13a1fc74
+000038a0: 3638 6334 3066 3133 3432 3037 3332 3830  68c40f1342073280
+000038b0: 3561 3463 3338 6131 3035 6438 3938 3438  5a4c38a105d89848
+000038c0: 6237 6331 3061 6636 3561 3930 6265 6666  b7c10af65a90beff
+000038d0: 3235 3235 3022 2c0a 2020 2020 2020 2020  25250",.        
+000038e0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+000038f0: 3864 3133 6336 3465 6532 6433 3365 6363  8d13c64ee2d33ecc
+00003900: 6637 3433 3739 3631 6236 6561 3761 6438  f7437961b6ea7ad8
+00003910: 3637 3365 3262 6530 3430 6234 6637 6664  673e2be040b4f7fd
+00003920: 3466 6434 6434 6432 3864 3963 6362 3165  4fd4d4d28d9ccb1e
+00003930: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003940: 2020 2022 7368 6132 3536 3a38 6465 3862     "sha256:8de8b
+00003950: 6230 6535 6164 3130 3338 3838 6436 3561  b0e5ad103888d65a
+00003960: 6265 6638 6263 6134 3161 6239 3337 3231  bef8bca41ab93721
+00003970: 3634 3735 3930 6133 6637 3430 3130 3063  647590a3f740100c
+00003980: 6436 3563 3362 3030 3531 3122 2c0a 2020  d65c3b00511",.  
+00003990: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000039a0: 6861 3235 363a 3866 6130 3362 6365 3962  ha256:8fa03bce9b
+000039b0: 6662 6565 6566 3966 3362 3136 3061 3862  fbeeef9f3b160a8b
+000039c0: 6564 3339 6132 3231 6438 3233 3038 6234  ed39a221d82308b4
+000039d0: 3135 3262 3237 6438 3264 3864 6161 3730  152b27d82d8daa70
+000039e0: 3431 6665 6535 222c 0a20 2020 2020 2020  41fee5",.       
+000039f0: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00003a00: 3a39 3234 6439 3432 3931 6361 3637 3439  :924d94291ca6749
+00003a10: 3035 6665 3934 3831 6631 3232 3934 6562  05fe9481f12294eb
+00003a20: 3131 6632 6433 6433 6664 3161 6462 3230  11f2d3d3fd1adb20
+00003a30: 3331 3462 6138 3965 3934 6634 3465 6435  314ba89e94f44ed5
+00003a40: 3922 2c0a 2020 2020 2020 2020 2020 2020  9",.            
+00003a50: 2020 2020 2273 6861 3235 363a 3937 3564      "sha256:975d
+00003a60: 3730 6162 3765 3363 3830 6133 6665 3836  70ab7e3c80a3fe86
+00003a70: 3030 3164 3837 3531 6636 3737 3839 3035  001d8751f6778905
+00003a80: 6563 3732 3366 3562 3131 3061 6564 3165  ec723f5b110aed1e
+00003a90: 3435 3064 6139 6434 6237 6632 222c 0a20  450da9d4b7f2",. 
+00003aa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003ab0: 7368 6132 3536 3a39 3736 6239 6334 3266  sha256:976b9c42f
+00003ac0: 6232 6134 3365 6266 3330 3466 6137 6434  b2a43ebf304fa7d4
+00003ad0: 6133 3130 6535 6631 3663 6339 3939 3932  a310e5f16cc99992
+00003ae0: 6633 3365 6365 6439 3165 6636 6639 3038  f33eced91ef6f908
+00003af0: 6264 3866 3333 6422 2c0a 2020 2020 2020  bd8f33d",.      
+00003b00: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00003b10: 363a 3965 3331 6362 3634 6437 6465 3662  6:9e31cb64d7de6b
+00003b20: 3666 3039 3730 3262 6232 3763 3032 6431  6f09702bb27c02d1
+00003b30: 3930 3462 3361 6562 6663 6136 3130 6331  904b3aebfca610c1
+00003b40: 3237 3732 3435 3263 3465 3663 3231 6130  2772452c4e6c21a0
+00003b50: 6433 222c 0a20 2020 2020 2020 2020 2020  d3",.           
+00003b60: 2020 2020 2022 7368 6132 3536 3a61 3334       "sha256:a34
+00003b70: 3232 3432 6665 3232 3430 3766 3363 3137  2242fe22407f3c17
+00003b80: 6634 6234 3939 3237 3661 3032 6230 3165  f4b499276a02b01e
+00003b90: 3830 6638 3631 6631 3638 3261 6431 6439  80f861f1682ad1d9
+00003ba0: 3562 3034 3031 3865 3063 3064 3422 2c0a  5b04018e0c0d4",.
+00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bc0: 2273 6861 3235 363a 6133 6433 3361 3662  "sha256:a3d33a6b
+00003bd0: 3365 6165 3837 6365 6165 6661 3931 6666  3eae87ceaefa91ff
+00003be0: 6463 3133 3062 3565 3835 3336 3138 3263  dc130b5e8536182c
+00003bf0: 6436 6466 6462 6663 3161 6135 3662 3436  d6dfdbfc1aa56b46
+00003c00: 6666 3863 3836 6465 222c 0a20 2020 2020  ff8c86de",.     
+00003c10: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00003c20: 3536 3a61 3839 3566 6363 3762 3135 6333  56:a895fcc7b15c3
+00003c30: 6663 3732 6265 6234 3363 6463 6264 6630  fc72beb43cdcbdf0
+00003c40: 6464 6237 6432 6562 6339 3539 6564 6163  ddb7d2ebc959edac
+00003c50: 3963 6566 3339 3062 3064 3134 6633 3966  9cef390b0d14f39f
+00003c60: 3861 3922 2c0a 2020 2020 2020 2020 2020  8a9",.          
+00003c70: 2020 2020 2020 2273 6861 3235 363a 6166        "sha256:af
+00003c80: 6231 3766 3834 6435 3630 3638 6137 6332  b17f84d56068a7c2
+00003c90: 3966 3566 6133 3762 6664 3338 6435 6162  9f5fa37bfd38d5ab
+00003ca0: 6136 3965 3333 3034 6166 3038 6565 3934  a69e3304af08ee94
+00003cb0: 6461 3865 6435 6230 3836 3538 3333 222c  da8ed5b0865833",
+00003cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cd0: 2022 7368 6132 3536 3a62 3163 3534 3661   "sha256:b1c546a
+00003ce0: 6361 3063 6134 6430 3238 3930 3164 3832  ca0ca4d028901d82
+00003cf0: 3530 3135 6463 3865 3464 3536 6161 6334  5015dc8e4d56aac4
+00003d00: 6235 3431 3837 3736 3930 6562 3736 3439  b541877690eb7649
+00003d10: 3066 3164 6338 6564 3022 2c0a 2020 2020  0f1dc8ed0",.    
+00003d20: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00003d30: 3235 363a 6232 3930 3139 6337 3630 3339  256:b29019c76039
+00003d40: 6463 3363 3066 6438 3135 6334 3133 3932  dc3c0fd815c41392
+00003d50: 6130 3434 6365 3535 3564 3962 6364 6433  a044ce555d9bcdd3
+00003d60: 3862 3066 6236 3066 6234 6364 3865 3437  8b0fb60fb4cd8e47
+00003d70: 3562 6139 222c 0a20 2020 2020 2020 2020  5ba9",.         
+00003d80: 2020 2020 2020 2022 7368 6132 3536 3a62         "sha256:b
+00003d90: 3436 3531 3763 3032 6363 6430 3830 3932  46517c02ccd08092
+00003da0: 6634 6661 3939 6632 3463 3362 3833 6438  f4fa99f24c3b83d8
+00003db0: 6639 3266 3733 3962 3436 3537 6230 6631  f92f739b4657b0f1
+00003dc0: 3436 3234 3661 3063 6136 6138 3331 6422  46246a0ca6a831d"
+00003dd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003de0: 2020 2273 6861 3235 363a 6237 6161 3566    "sha256:b7aa5f
+00003df0: 3861 3431 3231 3733 3630 6536 3030 6461  8a41217360e600da
+00003e00: 3634 3630 3034 6638 3738 3235 3061 3064  646004f878250a0d
+00003e10: 3637 3338 6263 6463 3131 6130 6133 3939  6738bcdc11a0a399
+00003e20: 3238 6437 6463 3230 3530 222c 0a20 2020  28d7dc2050",.   
+00003e30: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00003e40: 6132 3536 3a62 3762 3463 3937 3166 3035  a256:b7b4c971f05
+00003e50: 6536 6165 3439 3066 6566 3835 3263 3231  e6ae490fef852c21
+00003e60: 3862 3065 3739 6434 6535 3266 3739 6566  8b0e79d4e52f79ef
+00003e70: 3063 3834 3735 3536 3635 3834 6138 6662  0c8475566584a8fb
+00003e80: 3365 3031 6422 2c0a 2020 2020 2020 2020  3e01d",.        
+00003e90: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00003ea0: 6261 3930 6139 3536 3362 6134 3461 3732  ba90a9563ba44a72
+00003eb0: 6664 6132 6538 3533 3032 6333 6162 6337  fda2e85302c3abc7
+00003ec0: 3163 3535 3839 6365 6136 3038 6361 3136  1c5589cea608ca16
+00003ed0: 6332 3262 3938 3034 3236 3261 6165 6236  c22b9804262aaeb6
+00003ee0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003ef0: 2020 2022 7368 6132 3536 3a63 6230 3137     "sha256:cb017
+00003f00: 6664 3162 3236 3033 6566 3539 6533 3734  fd1b2603ef59e374
+00003f10: 6261 3230 3633 6635 3933 6162 6530 6663  ba2063f593abe0fc
+00003f20: 3435 6632 6164 3961 6264 6465 3562 3464  45f2ad9abdde5b4d
+00003f30: 3833 6264 3932 3261 3335 3322 2c0a 2020  83bd922a353",.  
+00003f40: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00003f50: 6861 3235 363a 6432 3236 3536 3336 3866  ha256:d22656368f
+00003f60: 3065 3631 3839 6532 3437 3232 3231 3465  0e6189e24722214e
+00003f70: 6438 6436 3662 3830 3232 6462 3139 6431  d8d66b8022db19d1
+00003f80: 3832 3932 3762 3961 3234 3861 3261 3861  82927b9a248a2a8a
+00003f90: 3266 3637 6562 222c 0a20 2020 2020 2020  2f67eb",.       
+00003fa0: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00003fb0: 3a64 3263 3264 6237 6664 3832 6539 6237  :d2c2db7fd82e9b7
+00003fc0: 3239 3337 3936 3962 6365 6163 3464 3663  2937969bceac4d6c
+00003fd0: 6138 3936 3630 6462 3061 3039 3637 3631  a89660db0a096761
+00003fe0: 3463 6532 3438 3165 3831 6130 6237 3731  4ce2481e81a0b771
+00003ff0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00004000: 2020 2020 2273 6861 3235 363a 6433 3962      "sha256:d39b
+00004010: 3562 3466 3261 3636 6363 6165 3862 3732  5b4f2a66ccae8b72
+00004020: 3633 6163 3363 3831 3730 3939 3462 3635  63ac3c8170994b65
+00004030: 3236 3637 3937 6662 3936 6362 6266 6433  266797fb96cbbfd3
+00004040: 6662 3562 3233 3932 3164 6238 222c 0a20  fb5b23921db8",. 
+00004050: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004060: 7368 6132 3536 3a64 3632 6135 6337 6461  sha256:d62a5c7da
+00004070: 6431 3130 3135 6336 3666 6262 3964 3838  d11015c66fbb9d88
+00004080: 3162 6334 6361 6135 6231 3266 3136 3239  1bc4caa5b12f1629
+00004090: 3266 3835 3738 3432 6439 6431 3837 3135  2f857842d9d18715
+000040a0: 3935 6634 3439 3522 2c0a 2020 2020 2020  95f4495",.      
+000040b0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+000040c0: 363a 6537 6439 3430 3532 3931 6336 3932  6:e7d9405291c692
+000040d0: 3836 3139 3430 3364 6231 6431 3062 6430  8619403db1d10bd0
+000040e0: 3738 3838 3838 3865 6331 6162 6362 6439  7888888ec1abcbd9
+000040f0: 3734 3866 6461 6139 3731 6437 6436 3631  748fdaa971d7d661
+00004100: 6232 222c 0a20 2020 2020 2020 2020 2020  b2",.           
+00004110: 2020 2020 2022 7368 6132 3536 3a65 3834       "sha256:e84
+00004120: 3630 3662 3734 6562 3764 6536 6666 3538  606b74eb7de6ff58
+00004130: 3161 3739 3135 6532 6461 6237 6132 3861  1a7915e2dab7a28a
+00004140: 3035 3137 6662 6531 6339 3233 3965 6232  0517fbe1c9239eb2
+00004150: 3237 6531 3335 3430 3634 6463 6422 2c0a  27e1354064dcd",.
+00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004170: 2273 6861 3235 363a 6562 3339 3365 3565  "sha256:eb393e5e
+00004180: 6263 3835 3234 3533 3437 3935 3031 3433  bc85245347950143
+00004190: 3936 3962 3234 3164 3038 6235 3262 3838  969b241d08b52b88
+000041a0: 6133 6463 3339 3437 3938 3232 6530 3733  a3dc39479822e073
+000041b0: 6131 6138 6562 3237 222c 0a20 2020 2020  a1a8eb27",.     
+000041c0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+000041d0: 3536 3a65 6262 6131 6364 3330 3865 6631  56:ebba1cd308ef1
+000041e0: 3135 3932 3534 3231 6433 6536 6135 3836  15925421d3e6a586
+000041f0: 6536 3535 6361 3561 3737 6235 6266 3431  e655ca5a77b5bf41
+00004200: 6530 3265 6230 6534 3536 3261 3131 3166  e02eb0e4562a111f
+00004210: 3264 3122 2c0a 2020 2020 2020 2020 2020  2d1",.          
+00004220: 2020 2020 2020 2273 6861 3235 363a 6565        "sha256:ee
+00004230: 3537 3139 3066 3234 6662 6137 3936 6533  57190f24fba796e3
+00004240: 3662 6236 6433 6161 3861 3837 3833 6336  6bb6d3aa8a8783c6
+00004250: 3433 6438 6661 3937 3630 6338 3966 3761  43d8fa9760c89f7a
+00004260: 3938 6162 3534 3535 6662 6638 3138 222c  98ab5455fbf818",
+00004270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004280: 2022 7368 6132 3536 3a66 3266 3637 6665   "sha256:f2f67fe
+00004290: 3132 6232 3263 6431 3330 6433 3464 3065  12b22cd130d34d0e
+000042a0: 6637 3932 3036 3036 3162 6662 3565 6461  f79206061bfb5eda
+000042b0: 3532 6665 6236 6365 3064 6261 3036 3434  52feb6ce0dba0644
+000042c0: 6532 3061 3033 6366 3422 2c0a 2020 2020  e20a03cf4",.    
+000042d0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+000042e0: 3235 363a 6636 3935 3134 3037 3339 3162  256:f6951407391b
+000042f0: 3633 3935 3034 6533 6233 6265 3531 6237  639504e3b3be51b7
+00004300: 6261 3566 3335 3238 6164 6266 3161 3861  ba5f3528adbf1a8a
+00004310: 6333 3330 3262 3638 3765 6361 6261 6266  c3302b687ecababf
+00004320: 3932 3965 222c 0a20 2020 2020 2020 2020  929e",.         
+00004330: 2020 2020 2020 2022 7368 6132 3536 3a66         "sha256:f
+00004340: 3735 6637 3136 3861 6232 3564 6439 3331  75f7168ab25dd931
+00004350: 3130 6338 6138 3131 3761 3232 3435 3063  10c8a8117a22450c
+00004360: 3139 3937 3661 6662 6334 3432 3334 6362  19976afbc44234cb
+00004370: 6637 3134 3831 3039 3463 3162 3835 3022  f71481094c1b850"
+00004380: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004390: 2020 2273 6861 3235 363a 6664 6563 3965    "sha256:fdec9e
+000043a0: 3863 6266 3133 6135 6266 3633 3239 3066  8cbf13a5bf63290f
+000043b0: 6336 3031 3364 3231 3661 3463 3732 3332  c6013d216a4c7232
+000043c0: 6566 6235 3135 3438 3539 3463 6133 3633  efb51548594ca363
+000043d0: 3161 3766 3133 6333 6133 220a 2020 2020  1a7f13c3a3".    
+000043e0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+000043f0: 2020 2020 2020 2022 696e 6465 7822 3a20         "index": 
+00004400: 2270 7970 6922 2c0a 2020 2020 2020 2020  "pypi",.        
+00004410: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
+00004420: 3d3d 372e 322e 3722 0a20 2020 2020 2020  ==7.2.7".       
+00004430: 207d 2c0a 2020 2020 2020 2020 2264 6973   },.        "dis
+00004440: 746c 6962 223a 207b 0a20 2020 2020 2020  tlib": {.       
+00004450: 2020 2020 2022 6861 7368 6573 223a 205b       "hashes": [
+00004460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004470: 2022 7368 6132 3536 3a31 3462 6164 3264   "sha256:14bad2d
+00004480: 3962 3034 6433 6133 3631 3237 6163 3937  9b04d3a36127ac97
+00004490: 6633 3062 3132 6131 3932 3638 6632 3131  f30b12a19268f211
+000044a0: 3036 3364 3866 3865 6534 6634 3731 3038  063d8f8ee4f47108
+000044b0: 3839 3665 3131 6234 3622 2c0a 2020 2020  896e11b46",.    
+000044c0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+000044d0: 3235 363a 6633 3563 3462 3639 3235 3432  256:f35c4b692542
+000044e0: 6361 3131 3064 6537 6566 3062 6561 3434  ca110de7ef0bea44
+000044f0: 6437 3339 3831 6361 6562 3334 6361 3062  d73981caeb34ca0b
+00004500: 3962 3662 3265 3664 3737 3930 6464 6138  9b6b2e6d7790dda8
+00004510: 6638 3065 220a 2020 2020 2020 2020 2020  f80e".          
+00004520: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+00004530: 2022 7665 7273 696f 6e22 3a20 223d 3d30   "version": "==0
+00004540: 2e33 2e36 220a 2020 2020 2020 2020 7d2c  .3.6".        },
+00004550: 0a20 2020 2020 2020 2022 646f 6375 7469  .        "docuti
+00004560: 6c73 223a 207b 0a20 2020 2020 2020 2020  ls": {.         
+00004570: 2020 2022 6861 7368 6573 223a 205b 0a20     "hashes": [. 
+00004580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004590: 7368 6132 3536 3a39 3666 3338 3761 3263  sha256:96f387a2c
+000045a0: 3535 3632 6462 3434 3736 6630 3966 3133  5562db4476f09f13
+000045b0: 6262 6162 3231 3932 6537 3634 6361 6330  bbab2192e764cac0
+000045c0: 3865 6262 6633 6133 3461 3935 6439 6231  8ebbf3a34a95d9b1
+000045d0: 6534 6135 3964 3622 2c0a 2020 2020 2020  e4a59d6",.      
+000045e0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+000045f0: 363a 6630 3861 3465 3237 3663 3361 3135  6:f08a4e276c3a15
+00004600: 3833 6138 3664 6365 3365 3334 6162 6133  83a86dce3e34aba3
+00004610: 6665 3034 6430 3262 6261 3264 6435 3165  fe04d02bba2dd51e
+00004620: 6431 3631 3036 3234 3465 3861 3932 3365  d16106244e8a923e
+00004630: 3362 220a 2020 2020 2020 2020 2020 2020  3b".            
+00004640: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00004650: 6d61 726b 6572 7322 3a20 2270 7974 686f  markers": "pytho
+00004660: 6e5f 7665 7273 696f 6e20 3e3d 2027 332e  n_version >= '3.
+00004670: 3727 222c 0a20 2020 2020 2020 2020 2020  7'",.           
+00004680: 2022 7665 7273 696f 6e22 3a20 223d 3d30   "version": "==0
+00004690: 2e32 302e 3122 0a20 2020 2020 2020 207d  .20.1".        }
+000046a0: 2c0a 2020 2020 2020 2020 2266 696c 656c  ,.        "filel
+000046b0: 6f63 6b22 3a20 7b0a 2020 2020 2020 2020  ock": {.        
+000046c0: 2020 2020 2268 6173 6865 7322 3a20 5b0a      "hashes": [.
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2273 6861 3235 363a 3432 6631 6534 6666  "sha256:42f1e4ff
+000046f0: 3262 3439 3733 3131 3231 3364 3631 6164  2b497311213d61ad
+00004700: 3761 6163 3566 6564 3930 3530 3630 3865  7aac5fed9050608e
+00004710: 3533 3039 3537 3366 3130 3165 6566 6139  5309573f101eefa9
+00004720: 3431 3433 3133 3461 222c 0a20 2020 2020  4143134a",.     
+00004730: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00004740: 3536 3a38 3262 3166 3764 6134 3666 3061  56:82b1f7da46f0a
+00004750: 6534 3261 6266 3162 6337 3865 3534 3836  e42abf1bc78e5486
+00004760: 3637 6634 3834 6163 3539 6432 6263 6563  67f484ac59d2bcec
+00004770: 3338 6337 3133 6365 6537 6532 6562 3531  38c713cee7e2eb51
+00004780: 6538 3322 0a20 2020 2020 2020 2020 2020  e83".           
+00004790: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+000047a0: 226d 6172 6b65 7273 223a 2022 7079 7468  "markers": "pyth
+000047b0: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2733  on_version >= '3
+000047c0: 2e37 2722 2c0a 2020 2020 2020 2020 2020  .7'",.          
+000047d0: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
+000047e0: 332e 3132 2e31 220a 2020 2020 2020 2020  3.12.1".        
+000047f0: 7d2c 0a20 2020 2020 2020 2022 666c 616b  },.        "flak
+00004800: 6538 223a 207b 0a20 2020 2020 2020 2020  e8": {.         
+00004810: 2020 2022 6861 7368 6573 223a 205b 0a20     "hashes": [. 
+00004820: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004830: 7368 6132 3536 3a33 3833 3337 3934 6532  sha256:3833794e2
+00004840: 3766 6636 3465 6134 6539 6366 3564 3431  7ff64ea4e9cf5d41
+00004850: 3030 3832 6138 6239 3766 6631 6130 3663  0082a8b97ff1a06c
+00004860: 3136 6161 3364 3230 3237 3333 3963 6430  16aa3d2027339cd0
+00004870: 6631 3139 3563 3722 2c0a 2020 2020 2020  f1195c7",.      
+00004880: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00004890: 363a 6336 3130 3037 6537 3636 3535 6166  6:c61007e76655af
+000048a0: 3735 6536 3738 3561 3933 3166 3435 3239  75e6785a931f4529
+000048b0: 3135 6233 3731 6463 3438 6635 3665 6664  15b371dc48f56efd
+000048c0: 3736 3532 3437 6338 6665 3638 6632 6231  765247c8fe68f2b1
+000048d0: 3831 220a 2020 2020 2020 2020 2020 2020  81".            
+000048e0: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+000048f0: 696e 6465 7822 3a20 2270 7970 6922 2c0a  index": "pypi",.
+00004900: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
+00004910: 7369 6f6e 223a 2022 3d3d 362e 302e 3022  sion": "==6.0.0"
+00004920: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00004930: 2020 2020 2269 646e 6122 3a20 7b0a 2020      "idna": {.  
+00004940: 2020 2020 2020 2020 2020 2268 6173 6865            "hashe
+00004950: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+00004960: 2020 2020 2020 2273 6861 3235 363a 3831        "sha256:81
+00004970: 3466 3532 3865 3864 6561 6437 6433 3239  4f528e8dead7d329
+00004980: 3833 3362 3931 6335 6661 6138 3764 3630  833b91c5faa87d60
+00004990: 6266 3731 3832 3463 6431 3261 3735 3330  bf71824cd12a7530
+000049a0: 6235 3532 3630 3633 6430 3263 6234 222c  b5526063d02cb4",
+000049b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000049c0: 2022 7368 6132 3536 3a39 3062 3737 6537   "sha256:90b77e7
+000049d0: 3965 6161 3365 6261 3664 6538 3139 6130  9eaa3eba6de819a0
+000049e0: 6334 3432 6330 6234 6365 6566 6333 3431  c442c0b4ceefc341
+000049f0: 6137 6132 6162 3737 6437 3536 3262 6634  a7a2ab77d7562bf4
+00004a00: 3966 3432 3563 3563 3222 0a20 2020 2020  9f425c5c2".     
+00004a10: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00004a20: 2020 2020 2020 226d 6172 6b65 7273 223a        "markers":
+00004a30: 2022 7079 7468 6f6e 5f76 6572 7369 6f6e   "python_version
+00004a40: 203e 3d20 2733 2e35 2722 2c0a 2020 2020   >= '3.5'",.    
+00004a50: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+00004a60: 223a 2022 3d3d 332e 3422 0a20 2020 2020  ": "==3.4".     
+00004a70: 2020 207d 2c0a 2020 2020 2020 2020 2269     },.        "i
+00004a80: 6d70 6f72 746c 6962 2d6d 6574 6164 6174  mportlib-metadat
+00004a90: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00004aa0: 2020 2268 6173 6865 7322 3a20 5b0a 2020    "hashes": [.  
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00004ac0: 6861 3235 363a 3433 6464 3238 3661 3263  ha256:43dd286a2c
+00004ad0: 6438 3939 3564 3565 6165 6637 6665 6532  d8995d5eaef7fee2
+00004ae0: 3036 3633 3430 3432 3362 3831 3865 6433  066340423b818ed3
+00004af0: 6664 3730 6164 6630 6261 6435 6631 6661  fd70adf0bad5f1fa
+00004b00: 6335 3366 6564 222c 0a20 2020 2020 2020  c53fed",.       
+00004b10: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00004b20: 3a39 3235 3031 6364 6639 6363 3636 6562  :92501cdf9cc66eb
+00004b30: 6433 6536 3132 6631 6234 6630 6330 3736  d3e612f1b4f0c076
+00004b40: 3564 6661 3432 6630 6661 3338 6666 6233  5dfa42f0fa38ffb3
+00004b50: 3139 6236 6264 3834 6464 3637 3564 3730  19b6bd84dd675d70
+00004b60: 3522 0a20 2020 2020 2020 2020 2020 205d  5".            ]
+00004b70: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+00004b80: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
+00004b90: 5f76 6572 7369 6f6e 203e 3d20 2733 2e37  _version >= '3.7
+00004ba0: 2722 2c0a 2020 2020 2020 2020 2020 2020  '",.            
+00004bb0: 2276 6572 7369 6f6e 223a 2022 3d3d 362e  "version": "==6.
+00004bc0: 362e 3022 0a20 2020 2020 2020 207d 2c0a  6.0".        },.
+00004bd0: 2020 2020 2020 2020 2269 6e69 636f 6e66          "iniconf
+00004be0: 6967 223a 207b 0a20 2020 2020 2020 2020  ig": {.         
+00004bf0: 2020 2022 6861 7368 6573 223a 205b 0a20     "hashes": [. 
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004c10: 7368 6132 3536 3a32 6439 3165 3133 3562  sha256:2d91e135b
+00004c20: 6637 3264 3331 6134 3130 6231 3763 3136  f72d31a410b17c16
+00004c30: 6461 3631 3061 3832 6362 3535 6636 6230  da610a82cb55f6b0
+00004c40: 3437 3764 3161 3930 3231 3334 6232 3461  477d1a902134b24a
+00004c50: 3435 3562 3862 3322 2c0a 2020 2020 2020  455b8b3",.      
+00004c60: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00004c70: 363a 6236 6138 3538 3731 6137 3964 3265  6:b6a85871a79d2e
+00004c80: 3362 3232 6432 6431 6239 3461 6332 3832  3b22d2d1b94ac282
+00004c90: 3432 3236 6136 3363 3662 3734 3163 3838  4226a63c6b741c88
+00004ca0: 6637 6165 3937 3566 3138 6236 3737 3833  f7ae975f18b67783
+00004cb0: 3734 220a 2020 2020 2020 2020 2020 2020  74".            
+00004cc0: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00004cd0: 6d61 726b 6572 7322 3a20 2270 7974 686f  markers": "pytho
+00004ce0: 6e5f 7665 7273 696f 6e20 3e3d 2027 332e  n_version >= '3.
+00004cf0: 3727 222c 0a20 2020 2020 2020 2020 2020  7'",.           
+00004d00: 2022 7665 7273 696f 6e22 3a20 223d 3d32   "version": "==2
+00004d10: 2e30 2e30 220a 2020 2020 2020 2020 7d2c  .0.0".        },
+00004d20: 0a20 2020 2020 2020 2022 6973 6f72 7422  .        "isort"
+00004d30: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00004d40: 2268 6173 6865 7322 3a20 5b0a 2020 2020  "hashes": [.    
+00004d50: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00004d60: 3235 363a 3862 6566 3764 6465 3234 3132  256:8bef7dde2412
+00004d70: 3738 3832 3461 3664 3833 6634 3461 3534  78824a6d83f44a54
+00004d80: 3437 3039 6230 3635 3139 3162 3935 6236  4709b065191b95b6
+00004d90: 6535 3038 3934 6264 6337 3232 6663 6261  e50894bdc722fcba
+00004da0: 3035 3034 222c 0a20 2020 2020 2020 2020  0504",.         
+00004db0: 2020 2020 2020 2022 7368 6132 3536 3a66         "sha256:f
+00004dc0: 3834 6332 3831 3833 3736 6536 3663 6638  84c2818376e66cf8
+00004dd0: 3433 6434 3937 3438 3665 6138 6665 6438  43d497486ea8fed8
+00004de0: 3730 3062 3334 3066 3330 3866 3037 3663  700b340f308f076c
+00004df0: 3666 6231 3232 3964 6666 3331 3862 3622  6fb1229dff318b6"
+00004e00: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+00004e10: 2020 2020 2020 2020 2020 2020 2269 6e64              "ind
+00004e20: 6578 223a 2022 7079 7069 222c 0a20 2020  ex": "pypi",.   
+00004e30: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
+00004e40: 6e22 3a20 223d 3d35 2e31 322e 3022 0a20  n": "==5.12.0". 
+00004e50: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00004e60: 2020 226a 6172 6163 6f2e 636c 6173 7365    "jaraco.classe
+00004e70: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00004e80: 2020 2268 6173 6865 7322 3a20 5b0a 2020    "hashes": [.  
+00004e90: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00004ea0: 6861 3235 363a 3233 3533 6465 3332 3838  ha256:2353de3288
+00004eb0: 6263 3662 3832 3132 3037 3532 3230 3163  bc6b82120752201c
+00004ec0: 3662 3163 3161 3134 6230 3538 3236 3766  6b1c1a14b058267f
+00004ed0: 6134 3234 6564 3563 6535 3938 3465 3362  a424ed5ce5984e3b
+00004ee0: 3932 3231 3538 222c 0a20 2020 2020 2020  922158",.       
+00004ef0: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00004f00: 3a38 3935 3539 6661 3563 3164 3363 3334  :89559fa5c1d3c34
+00004f10: 6566 6636 6636 3331 6164 3830 6262 3231  eff6f631ad80bb21
+00004f20: 6633 3738 6462 6362 6233 3564 6431 3631  f378dbcbb35dd161
+00004f30: 6664 3263 3662 3933 6635 6265 3266 3938  fd2c6b93f5be2f98
+00004f40: 6122 0a20 2020 2020 2020 2020 2020 205d  a".            ]
+00004f50: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+00004f60: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
+00004f70: 5f76 6572 7369 6f6e 203e 3d20 2733 2e37  _version >= '3.7
+00004f80: 2722 2c0a 2020 2020 2020 2020 2020 2020  '",.            
+00004f90: 2276 6572 7369 6f6e 223a 2022 3d3d 332e  "version": "==3.
+00004fa0: 322e 3322 0a20 2020 2020 2020 207d 2c0a  2.3".        },.
+00004fb0: 2020 2020 2020 2020 226b 6579 7269 6e67          "keyring
+00004fc0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00004fd0: 2022 6861 7368 6573 223a 205b 0a20 2020   "hashes": [.   
+00004fe0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00004ff0: 6132 3536 3a37 3731 6564 3261 3931 3930  a256:771ed2a9190
+00005000: 3933 3839 6564 3631 3438 3633 3164 6536  9389ed6148631de6
+00005010: 3738 6638 3264 6463 3733 3733 3764 3835  78f82ddc73737d85
+00005020: 6139 3237 6633 3832 6138 6131 6231 3537  a927f382a8a1b157
+00005030: 3839 3863 6422 2c0a 2020 2020 2020 2020  898cd",.        
+00005040: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00005050: 6261 3265 3135 6139 6233 3565 3231 3930  ba2e15a9b35e2190
+00005060: 3864 3061 6166 3465 3061 3437 6163 6335  8d0aaf4e0a47acc5
+00005070: 3264 3661 6533 3334 3434 6466 3064 6132  2d6ae33444df0da2
+00005080: 6234 3964 3431 6134 3665 6636 6436 3738  b49d41a46ef6d678
+00005090: 220a 2020 2020 2020 2020 2020 2020 5d2c  ".            ],
+000050a0: 0a20 2020 2020 2020 2020 2020 2022 6d61  .            "ma
+000050b0: 726b 6572 7322 3a20 2270 7974 686f 6e5f  rkers": "python_
+000050c0: 7665 7273 696f 6e20 3e3d 2027 332e 3727  version >= '3.7'
+000050d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000050e0: 7665 7273 696f 6e22 3a20 223d 3d32 332e  version": "==23.
+000050f0: 3133 2e31 220a 2020 2020 2020 2020 7d2c  13.1".        },
+00005100: 0a20 2020 2020 2020 2022 6d61 726b 646f  .        "markdo
+00005110: 776e 2d69 742d 7079 223a 207b 0a20 2020  wn-it-py": {.   
+00005120: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
+00005130: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00005140: 2020 2020 2022 7368 6132 3536 3a33 3535       "sha256:355
+00005150: 3231 3638 3435 6336 3062 6439 3632 3332  216845c60bd96232
+00005160: 6364 3864 3863 3430 6538 6639 3736 3563  cd8d8c40e8f9765c
+00005170: 6338 3666 3436 3838 3065 3433 6138 6664  c86f46880e43a8fd
+00005180: 3232 6463 3161 3161 3863 6162 3122 2c0a  22dc1a1a8cab1",.
+00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051a0: 2273 6861 3235 363a 6533 6636 3061 3934  "sha256:e3f60a94
+000051b0: 6661 3036 3664 6335 3265 6337 3636 3631  fa066dc52ec76661
+000051c0: 6533 3763 3835 3163 6232 3332 6439 3266  e37c851cb232d92f
+000051d0: 3938 3836 6231 3563 6235 3630 6161 6164  9886b15cb560aaad
+000051e0: 6132 6466 3866 6562 220a 2020 2020 2020  a2df8feb".      
+000051f0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00005200: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
+00005210: 2270 7974 686f 6e5f 7665 7273 696f 6e20  "python_version 
+00005220: 3e3d 2027 332e 3827 222c 0a20 2020 2020  >= '3.8'",.     
+00005230: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
+00005240: 3a20 223d 3d33 2e30 2e30 220a 2020 2020  : "==3.0.0".    
+00005250: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00005260: 6d63 6361 6265 223a 207b 0a20 2020 2020  mccabe": {.     
+00005270: 2020 2020 2020 2022 6861 7368 6573 223a         "hashes":
+00005280: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00005290: 2020 2022 7368 6132 3536 3a33 3438 6530     "sha256:348e0
+000052a0: 3234 3063 3333 6236 3062 6264 6634 6535  240c33b60bbdf4e5
+000052b0: 3233 3139 3265 6639 3139 6632 3863 6232  23192ef919f28cb2
+000052c0: 6333 6437 6435 6337 3739 3466 3734 3030  c3d7d5c7794f7400
+000052d0: 3932 3930 6632 3336 3332 3522 2c0a 2020  9290f236325",.  
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000052f0: 6861 3235 363a 3663 3264 3330 6162 3662  ha256:6c2d30ab6b
+00005300: 6530 6534 6134 3639 3139 3738 3138 3037  e0e4a46919781807
+00005310: 6234 6630 6438 3334 6562 6464 3663 3665  b4f0d834ebdd6c6e
+00005320: 3364 6361 3062 6461 3561 3135 6638 3633  3dca0bda5a15f863
+00005330: 3432 3762 3665 220a 2020 2020 2020 2020  427b6e".        
+00005340: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00005350: 2020 2022 6d61 726b 6572 7322 3a20 2270     "markers": "p
+00005360: 7974 686f 6e5f 7665 7273 696f 6e20 3e3d  ython_version >=
+00005370: 2027 332e 3627 222c 0a20 2020 2020 2020   '3.6'",.       
+00005380: 2020 2020 2022 7665 7273 696f 6e22 3a20       "version": 
+00005390: 223d 3d30 2e37 2e30 220a 2020 2020 2020  "==0.7.0".      
+000053a0: 2020 7d2c 0a20 2020 2020 2020 2022 6d64    },.        "md
+000053b0: 7572 6c22 3a20 7b0a 2020 2020 2020 2020  url": {.        
+000053c0: 2020 2020 2268 6173 6865 7322 3a20 5b0a      "hashes": [.
+000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053e0: 2273 6861 3235 363a 3834 3030 3861 3431  "sha256:84008a41
+000053f0: 6535 3136 3135 6134 3966 6339 3936 3631  e51615a49fc99661
+00005400: 3931 6666 3931 3530 3965 3363 3430 6239  91ff91509e3c40b9
+00005410: 3339 3137 3665 3634 3366 6435 3061 3563  39176e643fd50a5c
+00005420: 3231 3936 6238 6638 222c 0a20 2020 2020  2196b8f8",.     
+00005430: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00005440: 3536 3a62 6234 3133 6432 3966 3565 6561  56:bb413d29f5eea
+00005450: 3338 6633 3164 6434 3735 3464 6437 3337  38f31dd4754dd737
+00005460: 3764 3434 3635 3131 3666 6232 3037 3538  7d4465116fb20758
+00005470: 3566 3937 6266 3932 3535 3838 3638 3763  5f97bf925588687c
+00005480: 3162 6122 0a20 2020 2020 2020 2020 2020  1ba".           
+00005490: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+000054a0: 226d 6172 6b65 7273 223a 2022 7079 7468  "markers": "pyth
+000054b0: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2733  on_version >= '3
+000054c0: 2e37 2722 2c0a 2020 2020 2020 2020 2020  .7'",.          
+000054d0: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
+000054e0: 302e 312e 3222 0a20 2020 2020 2020 207d  0.1.2".        }
+000054f0: 2c0a 2020 2020 2020 2020 226d 6f72 652d  ,.        "more-
+00005500: 6974 6572 746f 6f6c 7322 3a20 7b0a 2020  itertools": {.  
+00005510: 2020 2020 2020 2020 2020 2268 6173 6865            "hashe
+00005520: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+00005530: 2020 2020 2020 2273 6861 3235 363a 6361        "sha256:ca
+00005540: 6261 6133 3431 6164 3033 3839 6561 3833  baa341ad0389ea83
+00005550: 6331 3761 3934 3536 3661 3533 6165 3463  c17a94566a53ae4c
+00005560: 3964 3037 3334 3938 3631 6563 6231 3464  9d07349861ecb14d
+00005570: 6336 6430 3334 3563 6639 6163 3564 222c  c6d0345cf9ac5d",
+00005580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005590: 2022 7368 6132 3536 3a64 3262 6337 6630   "sha256:d2bc7f0
+000055a0: 3234 3436 6538 3661 3638 3931 3165 3538  2446e86a68911e58
+000055b0: 6465 6437 3664 3635 3631 6565 6130 3063  ded76d6561eea00c
+000055c0: 6464 6662 3261 3931 6537 3031 3962 6262  ddfb2a91e7019bbb
+000055d0: 3538 3663 3739 3966 3322 0a20 2020 2020  586c799f3".     
+000055e0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+000055f0: 2020 2020 2020 226d 6172 6b65 7273 223a        "markers":
+00005600: 2022 7079 7468 6f6e 5f76 6572 7369 6f6e   "python_version
+00005610: 203e 3d20 2733 2e37 2722 2c0a 2020 2020   >= '3.7'",.    
+00005620: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+00005630: 223a 2022 3d3d 392e 312e 3022 0a20 2020  ": "==9.1.0".   
+00005640: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00005650: 226d 7970 7922 3a20 7b0a 2020 2020 2020  "mypy": {.      
+00005660: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
+00005670: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00005680: 2020 2273 6861 3235 363a 3163 3463 3432    "sha256:1c4c42
+00005690: 6336 3061 3831 3033 6561 6434 6331 6330  c60a8103ead4c1c0
+000056a0: 3630 6163 3363 6464 3366 6630 3165 3138  60ac3cdd3ff01e18
+000056b0: 6664 6463 6536 6631 3031 3665 3038 3933  fddce6f1016e0893
+000056c0: 3936 3437 6130 6537 3033 222c 0a20 2020  9647a0e703",.   
+000056d0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+000056e0: 6132 3536 3a34 3437 3937 6430 3331 6134  a256:44797d031a4
+000056f0: 3135 3136 6663 6635 6362 6661 3635 3232  1516fcf5cbfa6522
+00005700: 3635 6262 3939 3465 3533 6535 3139 3934  65bb994e53e51994
+00005710: 6331 6264 3634 3966 6663 6430 6333 6137  c1bd649ffcd0c3a7
+00005720: 6563 6362 6622 2c0a 2020 2020 2020 2020  eccbf",.        
+00005730: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00005740: 3437 3331 3137 6533 3130 6665 6265 3633  473117e310febe63
+00005750: 3264 6466 3130 6537 3435 6133 3535 3731  2ddf10e745a35571
+00005760: 3465 3737 3166 6665 3533 3466 3036 6462  4e771ffe534f06db
+00005770: 3430 3730 3237 3735 3035 3636 3134 6334  40702775056614c4
+00005780: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005790: 2020 2022 7368 6132 3536 3a34 6339 3963     "sha256:4c99c
+000057a0: 3365 6366 3232 3363 6632 3935 3236 3338  3ecf223cf2952638
+000057b0: 6461 3963 6438 3237 3933 6438 6633 6330  da9cd82793d8f3c0
+000057c0: 6335 6661 3862 3661 6532 6232 6439 6564  c5fa8b6ae2b2d9ed
+000057d0: 3165 3166 6635 3162 6138 3522 2c0a 2020  1e1ff51ba85",.  
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000057f0: 6861 3235 363a 3535 3061 3862 3361 3139  ha256:550a8b3a19
+00005800: 6262 3635 3839 3637 3961 3763 3363 3331  bb6589679a7c3c31
+00005810: 6636 3433 3132 6537 6666 3438 3261 3831  f64312e7ff482a81
+00005820: 3663 3936 6530 6365 6365 6339 6164 3361  6c96e0cecec9ad3a
+00005830: 3735 3634 6464 222c 0a20 2020 2020 2020  7564dd",.       
+00005840: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00005850: 3a36 3538 6665 3762 3637 3437 3639 6130  :658fe7b674769a0
+00005860: 3737 3064 3462 3236 6362 3464 3666 3030  770d4b26cb4d6f00
+00005870: 3565 3838 6134 3432 6665 3832 3434 3666  5e88a442fe82446f
+00005880: 3032 3062 6538 6535 6635 6566 6232 6661  020be8e5f5efb2fa
+00005890: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+000058a0: 2020 2020 2273 6861 3235 363a 3665 3333      "sha256:6e33
+000058b0: 6262 3862 3236 3133 3631 3461 3333 6466  bb8b2613614a33df
+000058c0: 6637 3035 3635 6634 6338 3033 6638 3839  f70565f4c803f889
+000058d0: 6562 6432 6638 3539 3436 3665 3432 6234  ebd2f859466e42b4
+000058e0: 3665 3164 6637 3630 3138 6464 222c 0a20  6e1df76018dd",. 
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005900: 7368 6132 3536 3a36 6534 3264 3239 6533  sha256:6e42d29e3
+00005910: 3234 6364 6461 3631 6461 6165 6332 3333  24cdda61daaec233
+00005920: 3663 3432 3531 3265 3539 6337 6333 3735  6c42512e59c7c375
+00005930: 3334 3062 6432 3032 6566 6131 6665 3066  340bd202efa1fe0f
+00005940: 3762 3866 3863 6122 2c0a 2020 2020 2020  7b8f8ca",.      
+00005950: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00005960: 363a 3734 6263 3962 3665 3065 3739 3830  6:74bc9b6e0e7980
+00005970: 3862 6638 3637 3864 3736 3738 6232 6165  8bf8678d7678b2ae
+00005980: 3337 3336 6561 3732 6435 3665 6564 6533  3736ea72d56eede3
+00005990: 3832 3062 6433 3834 3938 3233 6537 6633  820bd3849823e7f3
+000059a0: 3035 222c 0a20 2020 2020 2020 2020 2020  05",.           
+000059b0: 2020 2020 2022 7368 6132 3536 3a37 3665       "sha256:76e
+000059c0: 6337 3731 6532 3334 3266 3162 3535 3863  c771e2342f1b558c
+000059d0: 3336 6434 3939 3030 6466 6538 3164 3134  36d49900dfe81d14
+000059e0: 3033 3631 6464 3064 3264 6636 6364 3731  0361dd0d2df6cd71
+000059f0: 6233 6462 3162 6531 3535 3430 3922 2c0a  b3db1be155409",.
 00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2273 6861 3235 363a 3665 3333 6262 3862  "sha256:6e33bb8b
-00005a20: 3236 3133 3631 3461 3333 6466 6637 3035  2613614a33dff705
-00005a30: 3635 6634 6338 3033 6638 3839 6562 6432  65f4c803f889ebd2
-00005a40: 6638 3539 3436 3665 3432 6234 3665 3164  f859466e42b46e1d
-00005a50: 6637 3630 3138 6464 222c 0d0a 2020 2020  f76018dd",..    
-00005a60: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00005a70: 3235 363a 3665 3432 6432 3965 3332 3463  256:6e42d29e324c
-00005a80: 6464 6136 3164 6161 6563 3233 3336 6334  dda61daaec2336c4
-00005a90: 3235 3132 6535 3963 3763 3337 3533 3430  2512e59c7c375340
-00005aa0: 6264 3230 3265 6661 3166 6530 6637 6238  bd202efa1fe0f7b8
-00005ab0: 6638 6361 222c 0d0a 2020 2020 2020 2020  f8ca",..        
-00005ac0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00005ad0: 3734 6263 3962 3665 3065 3739 3830 3862  74bc9b6e0e79808b
-00005ae0: 6638 3637 3864 3736 3738 6232 6165 3337  f8678d7678b2ae37
-00005af0: 3336 6561 3732 6435 3665 6564 6533 3832  36ea72d56eede382
-00005b00: 3062 6433 3834 3938 3233 6537 6633 3035  0bd3849823e7f305
-00005b10: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005b20: 2020 2020 2273 6861 3235 363a 3736 6563      "sha256:76ec
-00005b30: 3737 3165 3233 3432 6631 6235 3538 6333  771e2342f1b558c3
-00005b40: 3664 3439 3930 3064 6665 3831 6431 3430  6d49900dfe81d140
-00005b50: 3336 3164 6430 6432 6466 3663 6437 3162  361dd0d2df6cd71b
-00005b60: 3364 6231 6265 3135 3534 3039 222c 0d0a  3db1be155409",..
-00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b80: 2273 6861 3235 363a 3764 3233 3337 3064  "sha256:7d23370d
-00005b90: 3261 3662 3761 3731 6463 3635 6431 3236  2a6b7a71dc65d126
-00005ba0: 3666 3961 3334 6534 6364 6539 6538 6532  6f9a34e4cde9e8e2
-00005bb0: 3135 3131 3332 3234 3135 6462 3462 3236  1511322415db4b26
-00005bc0: 6634 3666 3662 3863 222c 0d0a 2020 2020  f46f6b8c",..    
-00005bd0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00005be0: 3235 363a 3837 6466 3434 3935 3463 3331  256:87df44954c31
-00005bf0: 6438 3664 6639 3663 3862 6436 6538 3064  d86df96c8bd6e80d
-00005c00: 6663 6437 3733 3437 3365 3837 3761 6336  fcd773473e877ac6
-00005c10: 3137 3661 3865 3239 3839 3862 6662 3335  176a8e29898bfb35
-00005c20: 3031 6362 222c 0d0a 2020 2020 2020 2020  01cb",..        
-00005c30: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00005c40: 3863 3539 3739 6430 6465 6232 3765 3066  8c5979d0deb27e0f
-00005c50: 3434 3739 6265 6531 3865 6130 6638 3337  4479bee18ea0f837
-00005c60: 3332 6138 3933 6538 3162 3738 6536 3265  32a893e81b78e62e
-00005c70: 3264 6461 3365 3765 3531 3863 3932 6565  2dda3e7e518c92ee
-00005c80: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005c90: 2020 2020 2273 6861 3235 363a 3935 6438      "sha256:95d8
-00005ca0: 6433 3161 3737 3133 3531 3036 3835 6230  d31a7713510685b0
-00005cb0: 3566 6262 3138 6436 6163 3238 3761 3536  5fbb18d6ac287a56
-00005cc0: 6338 6636 3535 3464 3838 6331 3965 3733  c8f6554d88c19e73
-00005cd0: 6637 3234 6134 3435 3434 3861 222c 0d0a  f724a445448a",..
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2273 6861 3235 363a 6132 3234 3335 3633  "sha256:a2243563
-00005d00: 3237 3130 6134 6663 6638 6163 6638 3663  2710a4fcf8acf86c
-00005d10: 6264 3064 3639 6636 3861 6333 3839 6133  bd0d69f68ac389a3
-00005d20: 3839 3263 6232 3366 6261 6431 3736 6431  892cb23fbad176d1
-00005d30: 6364 6461 6632 3238 222c 0d0a 2020 2020  cddaf228",..    
-00005d40: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00005d50: 3235 363a 6138 3736 3365 3732 6435 6439  256:a8763e72d5d9
-00005d60: 3537 3464 3435 6365 3538 3831 3936 3262  574d45ce5881962b
-00005d70: 6338 6539 3034 3662 6637 6233 3735 6230  c8e9046bf7b375b0
-00005d80: 6162 6630 3331 6633 6536 3831 3137 3332  abf031f3e6811732
-00005d90: 6138 3937 222c 0d0a 2020 2020 2020 2020  a897",..        
-00005da0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00005db0: 6331 6562 3438 3563 6561 3533 6634 6635  c1eb485cea53f4f5
-00005dc0: 3238 3465 3562 6166 3932 3930 3263 6430  284e5baf92902cd0
-00005dd0: 3038 3862 3234 3938 3466 3432 3039 6532  088b24984f4209e2
-00005de0: 3539 3831 6363 3335 3964 3634 3434 3864  5981cc359d64448d
-00005df0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005e00: 2020 2020 2273 6861 3235 363a 6335 6432      "sha256:c5d2
-00005e10: 6363 3534 3137 3562 6162 3437 3031 3162  cc54175bab47011b
-00005e20: 3039 3638 3862 3431 3864 6237 3134 3033  09688b418db71403
-00005e30: 6165 6661 6430 3763 6263 6436 3264 3434  aefad07cbcd62d44
-00005e40: 3031 3035 3433 6663 3134 3366 222c 0d0a  010543fc143f",..
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2273 6861 3235 363a 6362 6330 3732 3436  "sha256:cbc07246
-00005e70: 3235 3362 3965 3364 3764 3734 6339 6666  253b9e3d7d74c9ff
-00005e80: 3934 3863 6430 6664 3761 3731 6166 6363  948cd0fd7a71afcc
-00005e90: 3262 3737 6337 6630 6135 3963 3236 6539  2b77c7f0a59c26e9
-00005ea0: 3339 3563 6231 3532 222c 0d0a 2020 2020  395cb152",..    
-00005eb0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00005ec0: 3235 363a 6430 6236 6336 3232 3036 6530  256:d0b6c62206e0
-00005ed0: 3430 3631 6532 3730 3039 3438 3163 6230  4061e27009481cb0
-00005ee0: 6563 3936 3666 3764 3631 3732 6235 6239  ec966f7d6172b5b9
-00005ef0: 3336 6633 6561 6433 6437 3466 3239 6665  36f3ead3d74f29fe
-00005f00: 3364 6366 222c 0d0a 2020 2020 2020 2020  3dcf",..        
-00005f10: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00005f20: 6464 6165 3066 3339 6361 3134 3639 3732  ddae0f39ca146972
-00005f30: 6666 3662 6234 3339 3966 3362 3239 3433  ff6bb4399f3b2943
-00005f40: 3838 3461 3737 3462 3837 3731 6561 3061  884a774b8771ea0a
-00005f50: 3866 3530 6539 3731 6635 6561 3562 6138  8f50e971f5ea5ba8
-00005f60: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005f70: 2020 2020 2273 6861 3235 363a 6531 6634      "sha256:e1f4
-00005f80: 6431 3665 3239 3666 3531 3335 3632 3462  d16e296f5135624b
-00005f90: 3334 6538 6662 3734 3165 6230 6561 6465  34e8fb741eb0eade
-00005fa0: 6463 6139 3038 3632 3430 3562 3166 3166  dca90862405b1f1f
-00005fb0: 6465 3230 3430 6239 6264 3131 222c 0d0a  de2040b9bd11",..
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 2273 6861 3235 363a 6538 3663 3263 3638  "sha256:e86c2c68
-00005fe0: 3532 6636 3266 3866 3262 3234 6362 3761  52f62f8f2b24cb7a
-00005ff0: 3631 3365 6265 3865 3063 3764 6331 3430  613ebe8e0c7dc140
-00006000: 3263 3631 6433 3661 3630 3931 3734 6636  2c61d36a609174f6
-00006010: 3365 3066 6630 3137 222c 0d0a 2020 2020  3e0ff017",..    
-00006020: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00006030: 3235 363a 6562 6339 3566 3833 3836 3331  256:ebc95f838631
-00006040: 3432 3732 6262 6338 3137 3032 3666 3863  4272bbc817026f8c
-00006050: 6538 6634 6630 6432 6566 3761 6534 3466  e8f4f0d2ef7ae44f
-00006060: 3934 3763 3436 3634 6566 6163 3961 6465  947c4664efac9ade
-00006070: 6339 3239 222c 0d0a 2020 2020 2020 2020  c929",..        
-00006080: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00006090: 6639 6463 6131 6532 3537 6434 6363 3132  f9dca1e257d4cc12
-000060a0: 3935 3137 3737 3932 3236 3735 3364 6265  9517779226753dbe
-000060b0: 6662 3466 3232 3636 6334 6561 6164 3631  fb4f2266c4eaad61
-000060c0: 3066 6331 3563 3661 3765 3134 3238 3365  0fc15c6a7e14283e
-000060d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000060e0: 2020 2020 2273 6861 3235 363a 6661 6666      "sha256:faff
-000060f0: 3836 6161 3130 6331 6161 3461 3130 6531  86aa10c1aa4a10e1
-00006100: 6133 3031 6465 3136 3066 3364 3866 6338  a301de160f3d8fc8
-00006110: 3730 3362 3838 6337 6539 3864 6534 3662  703b88c7e98de46b
-00006120: 3533 3166 6631 3237 3661 3961 220d 0a20  531ff1276a9a".. 
-00006130: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00006140: 2020 2020 2020 2020 2020 2022 696e 6465             "inde
-00006150: 7822 3a20 2270 7970 6922 2c0d 0a20 2020  x": "pypi",..   
-00006160: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
-00006170: 6e22 3a20 223d 3d31 2e33 2e30 220d 0a20  n": "==1.3.0".. 
-00006180: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00006190: 2020 2022 6d79 7079 2d65 7874 656e 7369     "mypy-extensi
-000061a0: 6f6e 7322 3a20 7b0d 0a20 2020 2020 2020  ons": {..       
-000061b0: 2020 2020 2022 6861 7368 6573 223a 205b       "hashes": [
-000061c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000061d0: 2020 2273 6861 3235 363a 3433 3932 6636    "sha256:4392f6
-000061e0: 6330 6562 3861 3536 3638 6136 3965 3233  c0eb8a5668a69e23
-000061f0: 6431 3638 6666 6137 3066 3062 6539 6363  d168ffa70f0be9cc
-00006200: 6664 3332 6235 6363 3264 3236 6133 3461  fd32b5cc2d26a34a
-00006210: 6535 6238 3434 3535 3264 222c 0d0a 2020  e5b844552d",..  
-00006220: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00006230: 6861 3235 363a 3735 6462 6638 3935 3564  ha256:75dbf8955d
-00006240: 6330 3034 3432 6134 3338 6663 3464 3036  c00442a438fc4d06
-00006250: 3636 3530 3861 3961 3937 6236 6264 3431  66508a9a97b6bd41
-00006260: 6161 3266 3066 6665 3964 3266 3237 3235  aa2f0ffe9d2f2725
-00006270: 6166 3037 3832 220d 0a20 2020 2020 2020  af0782"..       
-00006280: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-00006290: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
-000062a0: 2270 7974 686f 6e5f 7665 7273 696f 6e20  "python_version 
-000062b0: 3e3d 2027 332e 3527 222c 0d0a 2020 2020  >= '3.5'",..    
-000062c0: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-000062d0: 223a 2022 3d3d 312e 302e 3022 0d0a 2020  ": "==1.0.0"..  
-000062e0: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-000062f0: 2020 2270 6163 6b61 6769 6e67 223a 207b    "packaging": {
-00006300: 0d0a 2020 2020 2020 2020 2020 2020 2268  ..            "h
-00006310: 6173 6865 7322 3a20 5b0d 0a20 2020 2020  ashes": [..     
-00006320: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00006330: 3536 3a39 3934 3739 3361 6634 3239 3530  56:994793af42950
-00006340: 3263 3465 6132 6562 6636 6266 3636 3436  2c4ea2ebf6bf6646
-00006350: 3239 6430 3763 3161 3966 6539 3734 6166  29d07c1a9fe974af
-00006360: 3932 3936 3665 3462 3864 3264 6637 6564  92966e4b8d2df7ed
-00006370: 6336 3122 2c0d 0a20 2020 2020 2020 2020  c61",..         
-00006380: 2020 2020 2020 2022 7368 6132 3536 3a61         "sha256:a
-00006390: 3339 3239 3830 6432 6236 6366 6661 3634  392980d2b6cffa64
-000063a0: 3434 3331 3839 3862 6535 3462 3030 3435  4431898be54b0045
-000063b0: 3135 3133 3139 6431 6537 6563 3334 6630  151319d1e7ec34f0
-000063c0: 6366 6564 3438 3736 3764 6433 3334 6622  cfed48767dd334f"
-000063d0: 0d0a 2020 2020 2020 2020 2020 2020 5d2c  ..            ],
-000063e0: 0d0a 2020 2020 2020 2020 2020 2020 226d  ..            "m
-000063f0: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
-00006400: 5f76 6572 7369 6f6e 203e 3d20 2733 2e37  _version >= '3.7
-00006410: 2722 2c0d 0a20 2020 2020 2020 2020 2020  '",..           
-00006420: 2022 7665 7273 696f 6e22 3a20 223d 3d32   "version": "==2
-00006430: 332e 3122 0d0a 2020 2020 2020 2020 7d2c  3.1"..        },
-00006440: 0d0a 2020 2020 2020 2020 2270 6174 6873  ..        "paths
-00006450: 7065 6322 3a20 7b0d 0a20 2020 2020 2020  pec": {..       
-00006460: 2020 2020 2022 6861 7368 6573 223a 205b       "hashes": [
-00006470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006480: 2020 2273 6861 3235 363a 3237 3938 6465    "sha256:2798de
-00006490: 3830 3066 6139 3237 3830 6533 3361 6363  800fa92780e33acc
-000064a0: 6139 3235 3934 3565 3961 3139 6131 3333  a925945e9a19a133
-000064b0: 6237 3135 3036 3763 6631 3635 6238 3836  b715067cf165b886
-000064c0: 3663 3135 6133 3136 3837 222c 0d0a 2020  6c15a31687",..  
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000064e0: 6861 3235 363a 6438 6166 3730 6166 3736  ha256:d8af70af76
-000064f0: 3635 3235 3534 6264 3133 3463 3232 6233  652554bd134c22b3
-00006500: 6538 6131 6363 3436 6564 3764 3931 6564  e8a1cc46ed7d91ed
-00006510: 6364 6437 3231 6566 3161 3063 3531 6138  cdd721ef1a0c51a8
-00006520: 3461 3532 3933 220d 0a20 2020 2020 2020  4a5293"..       
-00006530: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-00006540: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
-00006550: 2270 7974 686f 6e5f 7665 7273 696f 6e20  "python_version 
-00006560: 3e3d 2027 332e 3727 222c 0d0a 2020 2020  >= '3.7'",..    
-00006570: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-00006580: 223a 2022 3d3d 302e 3131 2e31 220d 0a20  ": "==0.11.1".. 
-00006590: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000065a0: 2020 2022 706b 6769 6e66 6f22 3a20 7b0d     "pkginfo": {.
-000065b0: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
-000065c0: 7368 6573 223a 205b 0d0a 2020 2020 2020  shes": [..      
-000065d0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
-000065e0: 363a 3462 3761 3535 3561 3664 3561 3232  6:4b7a555a6d5a22
-000065f0: 3136 3966 6363 3963 6637 6266 6437 3864  169fcc9cf7bfd78d
-00006600: 3239 3662 3033 3631 6164 6164 3431 3261  296b0361adad412a
-00006610: 3334 3663 3132 3236 3834 3961 6635 6535  346c1226849af5e5
-00006620: 3436 222c 0d0a 2020 2020 2020 2020 2020  46",..          
-00006630: 2020 2020 2020 2273 6861 3235 363a 3866        "sha256:8f
-00006640: 6435 3839 3665 3837 3138 6134 3337 3266  d5896e8718a4372f
-00006650: 3065 6139 6363 3964 3936 6636 3431 3763  0ea9cc9d96f6417c
-00006660: 3962 3938 3665 3233 6134 6431 3136 6464  9b986e23a4d116dd
-00006670: 6132 3662 3632 6363 3239 6430 3436 220d  a26b62cc29d046".
-00006680: 0a20 2020 2020 2020 2020 2020 205d 2c0d  .            ],.
-00006690: 0a20 2020 2020 2020 2020 2020 2022 6d61  .            "ma
-000066a0: 726b 6572 7322 3a20 2270 7974 686f 6e5f  rkers": "python_
-000066b0: 7665 7273 696f 6e20 3e3d 2027 332e 3627  version >= '3.6'
-000066c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000066d0: 2276 6572 7369 6f6e 223a 2022 3d3d 312e  "version": "==1.
-000066e0: 392e 3622 0d0a 2020 2020 2020 2020 7d2c  9.6"..        },
-000066f0: 0d0a 2020 2020 2020 2020 2270 6c61 7466  ..        "platf
-00006700: 6f72 6d64 6972 7322 3a20 7b0d 0a20 2020  ormdirs": {..   
-00006710: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
-00006720: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00006730: 2020 2020 2020 2273 6861 3235 363a 3061        "sha256:0a
-00006740: 6465 3938 6134 3839 3565 3837 6463 3531  de98a4895e87dc51
-00006750: 6434 3731 3531 6637 6432 6563 3239 3033  d47151f7d2ec2903
-00006760: 3635 6135 3835 3135 3164 3937 6234 6438  65a585151d97b4d8
-00006770: 6436 3331 3265 6436 3133 3266 6564 222c  d6312ed6132fed",
-00006780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006790: 2020 2273 6861 3235 363a 6534 3866 6162    "sha256:e48fab
-000067a0: 6438 3764 6238 6633 6137 6466 3731 3530  d87db8f3a7df7150
-000067b0: 6134 6135 6561 3232 6335 3436 6565 3862  a4a5ea22c546ee8b
-000067c0: 6333 3962 6332 3437 3332 3434 3733 3064  c39bc2473244730d
-000067d0: 3462 3536 6432 6363 3465 220d 0a20 2020  4b56d2cc4e"..   
-000067e0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-000067f0: 2020 2020 2020 2020 2022 6d61 726b 6572           "marker
-00006800: 7322 3a20 2270 7974 686f 6e5f 7665 7273  s": "python_vers
-00006810: 696f 6e20 3e3d 2027 332e 3727 222c 0d0a  ion >= '3.7'",..
-00006820: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
-00006830: 7369 6f6e 223a 2022 3d3d 332e 352e 3322  sion": "==3.5.3"
-00006840: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00006850: 2020 2020 2020 2270 6c75 6767 7922 3a20        "pluggy": 
-00006860: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00006870: 6861 7368 6573 223a 205b 0d0a 2020 2020  hashes": [..    
+00005a10: 2273 6861 3235 363a 3764 3233 3337 3064  "sha256:7d23370d
+00005a20: 3261 3662 3761 3731 6463 3635 6431 3236  2a6b7a71dc65d126
+00005a30: 3666 3961 3334 6534 6364 6539 6538 6532  6f9a34e4cde9e8e2
+00005a40: 3135 3131 3332 3234 3135 6462 3462 3236  1511322415db4b26
+00005a50: 6634 3666 3662 3863 222c 0a20 2020 2020  f46f6b8c",.     
+00005a60: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00005a70: 3536 3a38 3764 6634 3439 3534 6333 3164  56:87df44954c31d
+00005a80: 3836 6466 3936 6338 6264 3665 3830 6466  86df96c8bd6e80df
+00005a90: 6364 3737 3334 3733 6538 3737 6163 3631  cd773473e877ac61
+00005aa0: 3736 6138 6532 3938 3938 6266 6233 3530  76a8e29898bfb350
+00005ab0: 3163 6222 2c0a 2020 2020 2020 2020 2020  1cb",.          
+00005ac0: 2020 2020 2020 2273 6861 3235 363a 3863        "sha256:8c
+00005ad0: 3539 3739 6430 6465 6232 3765 3066 3434  5979d0deb27e0f44
+00005ae0: 3739 6265 6531 3865 6130 6638 3337 3332  79bee18ea0f83732
+00005af0: 6138 3933 6538 3162 3738 6536 3265 3264  a893e81b78e62e2d
+00005b00: 6461 3365 3765 3531 3863 3932 6565 222c  da3e7e518c92ee",
+00005b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b20: 2022 7368 6132 3536 3a39 3564 3864 3331   "sha256:95d8d31
+00005b30: 6137 3731 3335 3130 3638 3562 3035 6662  a7713510685b05fb
+00005b40: 6231 3864 3661 6332 3837 6135 3663 3866  b18d6ac287a56c8f
+00005b50: 3635 3534 6438 3863 3139 6537 3366 3732  6554d88c19e73f72
+00005b60: 3461 3434 3534 3438 6122 2c0a 2020 2020  4a445448a",.    
+00005b70: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00005b80: 3235 363a 6132 3234 3335 3633 3237 3130  256:a22435632710
+00005b90: 6134 6663 6638 6163 6638 3663 6264 3064  a4fcf8acf86cbd0d
+00005ba0: 3639 6636 3861 6333 3839 6133 3839 3263  69f68ac389a3892c
+00005bb0: 6232 3366 6261 6431 3736 6431 6364 6461  b23fbad176d1cdda
+00005bc0: 6632 3238 222c 0a20 2020 2020 2020 2020  f228",.         
+00005bd0: 2020 2020 2020 2022 7368 6132 3536 3a61         "sha256:a
+00005be0: 3837 3633 6537 3264 3564 3935 3734 6434  8763e72d5d9574d4
+00005bf0: 3563 6535 3838 3139 3632 6263 3865 3930  5ce5881962bc8e90
+00005c00: 3436 6266 3762 3337 3562 3061 6266 3033  46bf7b375b0abf03
+00005c10: 3166 3365 3638 3131 3733 3261 3839 3722  1f3e6811732a897"
+00005c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005c30: 2020 2273 6861 3235 363a 6331 6562 3438    "sha256:c1eb48
+00005c40: 3563 6561 3533 6634 6635 3238 3465 3562  5cea53f4f5284e5b
+00005c50: 6166 3932 3930 3263 6430 3038 3862 3234  af92902cd0088b24
+00005c60: 3938 3466 3432 3039 6532 3539 3831 6363  984f4209e25981cc
+00005c70: 3335 3964 3634 3434 3864 222c 0a20 2020  359d64448d",.   
+00005c80: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00005c90: 6132 3536 3a63 3564 3263 6335 3431 3735  a256:c5d2cc54175
+00005ca0: 6261 6234 3730 3131 6230 3936 3838 6234  bab47011b09688b4
+00005cb0: 3138 6462 3731 3430 3361 6566 6164 3037  18db71403aefad07
+00005cc0: 6362 6364 3632 6434 3430 3130 3534 3366  cbcd62d44010543f
+00005cd0: 6331 3433 6622 2c0a 2020 2020 2020 2020  c143f",.        
+00005ce0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00005cf0: 6362 6330 3732 3436 3235 3362 3965 3364  cbc07246253b9e3d
+00005d00: 3764 3734 6339 6666 3934 3863 6430 6664  7d74c9ff948cd0fd
+00005d10: 3761 3731 6166 6363 3262 3737 6337 6630  7a71afcc2b77c7f0
+00005d20: 6135 3963 3236 6539 3339 3563 6231 3532  a59c26e9395cb152
+00005d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005d40: 2020 2022 7368 6132 3536 3a64 3062 3663     "sha256:d0b6c
+00005d50: 3632 3230 3665 3034 3036 3165 3237 3030  62206e04061e2700
+00005d60: 3934 3831 6362 3065 6339 3636 6637 6436  9481cb0ec966f7d6
+00005d70: 3137 3262 3562 3933 3666 3365 6164 3364  172b5b936f3ead3d
+00005d80: 3734 6632 3966 6533 6463 6622 2c0a 2020  74f29fe3dcf",.  
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00005da0: 6861 3235 363a 6464 6165 3066 3339 6361  ha256:ddae0f39ca
+00005db0: 3134 3639 3732 6666 3662 6234 3339 3966  146972ff6bb4399f
+00005dc0: 3362 3239 3433 3838 3461 3737 3462 3837  3b2943884a774b87
+00005dd0: 3731 6561 3061 3866 3530 6539 3731 6635  71ea0a8f50e971f5
+00005de0: 6561 3562 6138 222c 0a20 2020 2020 2020  ea5ba8",.       
+00005df0: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00005e00: 3a65 3166 3464 3136 6532 3936 6635 3133  :e1f4d16e296f513
+00005e10: 3536 3234 6233 3465 3866 6237 3431 6562  5624b34e8fb741eb
+00005e20: 3065 6164 6564 6361 3930 3836 3234 3035  0eadedca90862405
+00005e30: 6231 6631 6664 6532 3034 3062 3962 6431  b1f1fde2040b9bd1
+00005e40: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+00005e50: 2020 2020 2273 6861 3235 363a 6538 3663      "sha256:e86c
+00005e60: 3263 3638 3532 6636 3266 3866 3262 3234  2c6852f62f8f2b24
+00005e70: 6362 3761 3631 3365 6265 3865 3063 3764  cb7a613ebe8e0c7d
+00005e80: 6331 3430 3263 3631 6433 3661 3630 3931  c1402c61d36a6091
+00005e90: 3734 6636 3365 3066 6630 3137 222c 0a20  74f63e0ff017",. 
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005eb0: 7368 6132 3536 3a65 6263 3935 6638 3338  sha256:ebc95f838
+00005ec0: 3633 3134 3237 3262 6263 3831 3730 3236  6314272bbc817026
+00005ed0: 6638 6365 3866 3466 3064 3265 6637 6165  f8ce8f4f0d2ef7ae
+00005ee0: 3434 6639 3437 6334 3636 3465 6661 6339  44f947c4664efac9
+00005ef0: 6164 6563 3932 3922 2c0a 2020 2020 2020  adec929",.      
+00005f00: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00005f10: 363a 6639 6463 6131 6532 3537 6434 6363  6:f9dca1e257d4cc
+00005f20: 3132 3935 3137 3737 3932 3236 3735 3364  129517779226753d
+00005f30: 6265 6662 3466 3232 3636 6334 6561 6164  befb4f2266c4eaad
+00005f40: 3631 3066 6331 3563 3661 3765 3134 3238  610fc15c6a7e1428
+00005f50: 3365 222c 0a20 2020 2020 2020 2020 2020  3e",.           
+00005f60: 2020 2020 2022 7368 6132 3536 3a66 6166       "sha256:faf
+00005f70: 6638 3661 6131 3063 3161 6134 6131 3065  f86aa10c1aa4a10e
+00005f80: 3161 3330 3164 6531 3630 6633 6438 6663  1a301de160f3d8fc
+00005f90: 3837 3033 6238 3863 3765 3938 6465 3436  8703b88c7e98de46
+00005fa0: 6235 3331 6666 3132 3736 6139 6122 0a20  b531ff1276a9a". 
+00005fb0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+00005fc0: 2020 2020 2020 2020 2020 2269 6e64 6578            "index
+00005fd0: 223a 2022 7079 7069 222c 0a20 2020 2020  ": "pypi",.     
+00005fe0: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
+00005ff0: 3a20 223d 3d31 2e33 2e30 220a 2020 2020  : "==1.3.0".    
+00006000: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00006010: 6d79 7079 2d65 7874 656e 7369 6f6e 7322  mypy-extensions"
+00006020: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00006030: 2268 6173 6865 7322 3a20 5b0a 2020 2020  "hashes": [.    
+00006040: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00006050: 3235 363a 3433 3932 6636 6330 6562 3861  256:4392f6c0eb8a
+00006060: 3536 3638 6136 3965 3233 6431 3638 6666  5668a69e23d168ff
+00006070: 6137 3066 3062 6539 6363 6664 3332 6235  a70f0be9ccfd32b5
+00006080: 6363 3264 3236 6133 3461 6535 6238 3434  cc2d26a34ae5b844
+00006090: 3535 3264 222c 0a20 2020 2020 2020 2020  552d",.         
+000060a0: 2020 2020 2020 2022 7368 6132 3536 3a37         "sha256:7
+000060b0: 3564 6266 3839 3535 6463 3030 3434 3261  5dbf8955dc00442a
+000060c0: 3433 3866 6334 6430 3636 3635 3038 6139  438fc4d0666508a9
+000060d0: 6139 3762 3662 6434 3161 6132 6630 6666  a97b6bd41aa2f0ff
+000060e0: 6539 6432 6632 3732 3561 6630 3738 3222  e9d2f2725af0782"
+000060f0: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+00006100: 2020 2020 2020 2020 2020 2020 226d 6172              "mar
+00006110: 6b65 7273 223a 2022 7079 7468 6f6e 5f76  kers": "python_v
+00006120: 6572 7369 6f6e 203e 3d20 2733 2e35 2722  ersion >= '3.5'"
+00006130: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+00006140: 6572 7369 6f6e 223a 2022 3d3d 312e 302e  ersion": "==1.0.
+00006150: 3022 0a20 2020 2020 2020 207d 2c0a 2020  0".        },.  
+00006160: 2020 2020 2020 2270 6163 6b61 6769 6e67        "packaging
+00006170: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00006180: 2022 6861 7368 6573 223a 205b 0a20 2020   "hashes": [.   
+00006190: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+000061a0: 6132 3536 3a39 3934 3739 3361 6634 3239  a256:994793af429
+000061b0: 3530 3263 3465 6132 6562 6636 6266 3636  502c4ea2ebf6bf66
+000061c0: 3436 3239 6430 3763 3161 3966 6539 3734  4629d07c1a9fe974
+000061d0: 6166 3932 3936 3665 3462 3864 3264 6637  af92966e4b8d2df7
+000061e0: 6564 6336 3122 2c0a 2020 2020 2020 2020  edc61",.        
+000061f0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00006200: 6133 3932 3938 3064 3262 3663 6666 6136  a392980d2b6cffa6
+00006210: 3434 3433 3138 3938 6265 3534 6230 3034  44431898be54b004
+00006220: 3531 3531 3331 3964 3165 3765 6333 3466  5151319d1e7ec34f
+00006230: 3063 6665 6434 3837 3637 6464 3333 3466  0cfed48767dd334f
+00006240: 220a 2020 2020 2020 2020 2020 2020 5d2c  ".            ],
+00006250: 0a20 2020 2020 2020 2020 2020 2022 6d61  .            "ma
+00006260: 726b 6572 7322 3a20 2270 7974 686f 6e5f  rkers": "python_
+00006270: 7665 7273 696f 6e20 3e3d 2027 332e 3727  version >= '3.7'
+00006280: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00006290: 7665 7273 696f 6e22 3a20 223d 3d32 332e  version": "==23.
+000062a0: 3122 0a20 2020 2020 2020 207d 2c0a 2020  1".        },.  
+000062b0: 2020 2020 2020 2270 6174 6873 7065 6322        "pathspec"
+000062c0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000062d0: 2268 6173 6865 7322 3a20 5b0a 2020 2020  "hashes": [.    
+000062e0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+000062f0: 3235 363a 3237 3938 6465 3830 3066 6139  256:2798de800fa9
+00006300: 3237 3830 6533 3361 6363 6139 3235 3934  2780e33acca92594
+00006310: 3565 3961 3139 6131 3333 6237 3135 3036  5e9a19a133b71506
+00006320: 3763 6631 3635 6238 3836 3663 3135 6133  7cf165b8866c15a3
+00006330: 3136 3837 222c 0a20 2020 2020 2020 2020  1687",.         
+00006340: 2020 2020 2020 2022 7368 6132 3536 3a64         "sha256:d
+00006350: 3861 6637 3061 6637 3636 3532 3535 3462  8af70af76652554b
+00006360: 6431 3334 6332 3262 3365 3861 3163 6334  d134c22b3e8a1cc4
+00006370: 3665 6437 6439 3165 6463 6464 3732 3165  6ed7d91edcdd721e
+00006380: 6631 6130 6335 3161 3834 6135 3239 3322  f1a0c51a84a5293"
+00006390: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+000063a0: 2020 2020 2020 2020 2020 2020 226d 6172              "mar
+000063b0: 6b65 7273 223a 2022 7079 7468 6f6e 5f76  kers": "python_v
+000063c0: 6572 7369 6f6e 203e 3d20 2733 2e37 2722  ersion >= '3.7'"
+000063d0: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+000063e0: 6572 7369 6f6e 223a 2022 3d3d 302e 3131  ersion": "==0.11
+000063f0: 2e31 220a 2020 2020 2020 2020 7d2c 0a20  .1".        },. 
+00006400: 2020 2020 2020 2022 706b 6769 6e66 6f22         "pkginfo"
+00006410: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00006420: 2268 6173 6865 7322 3a20 5b0a 2020 2020  "hashes": [.    
+00006430: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00006440: 3235 363a 3462 3761 3535 3561 3664 3561  256:4b7a555a6d5a
+00006450: 3232 3136 3966 6363 3963 6637 6266 6437  22169fcc9cf7bfd7
+00006460: 3864 3239 3662 3033 3631 6164 6164 3431  8d296b0361adad41
+00006470: 3261 3334 3663 3132 3236 3834 3961 6635  2a346c1226849af5
+00006480: 6535 3436 222c 0a20 2020 2020 2020 2020  e546",.         
+00006490: 2020 2020 2020 2022 7368 6132 3536 3a38         "sha256:8
+000064a0: 6664 3538 3936 6538 3731 3861 3433 3732  fd5896e8718a4372
+000064b0: 6630 6561 3963 6339 6439 3666 3634 3137  f0ea9cc9d96f6417
+000064c0: 6339 6239 3836 6532 3361 3464 3131 3664  c9b986e23a4d116d
+000064d0: 6461 3236 6236 3263 6332 3964 3034 3622  da26b62cc29d046"
+000064e0: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+000064f0: 2020 2020 2020 2020 2020 2020 226d 6172              "mar
+00006500: 6b65 7273 223a 2022 7079 7468 6f6e 5f76  kers": "python_v
+00006510: 6572 7369 6f6e 203e 3d20 2733 2e36 2722  ersion >= '3.6'"
+00006520: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+00006530: 6572 7369 6f6e 223a 2022 3d3d 312e 392e  ersion": "==1.9.
+00006540: 3622 0a20 2020 2020 2020 207d 2c0a 2020  6".        },.  
+00006550: 2020 2020 2020 2270 6c61 7466 6f72 6d64        "platformd
+00006560: 6972 7322 3a20 7b0a 2020 2020 2020 2020  irs": {.        
+00006570: 2020 2020 2268 6173 6865 7322 3a20 5b0a      "hashes": [.
+00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006590: 2273 6861 3235 363a 3061 6465 3938 6134  "sha256:0ade98a4
+000065a0: 3839 3565 3837 6463 3531 6434 3731 3531  895e87dc51d47151
+000065b0: 6637 6432 6563 3239 3033 3635 6135 3835  f7d2ec290365a585
+000065c0: 3135 3164 3937 6234 6438 6436 3331 3265  151d97b4d8d6312e
+000065d0: 6436 3133 3266 6564 222c 0a20 2020 2020  d6132fed",.     
+000065e0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+000065f0: 3536 3a65 3438 6661 6264 3837 6462 3866  56:e48fabd87db8f
+00006600: 3361 3764 6637 3135 3061 3461 3565 6132  3a7df7150a4a5ea2
+00006610: 3263 3534 3665 6538 6263 3339 6263 3234  2c546ee8bc39bc24
+00006620: 3733 3234 3437 3330 6434 6235 3664 3263  73244730d4b56d2c
+00006630: 6334 6522 0a20 2020 2020 2020 2020 2020  c4e".           
+00006640: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+00006650: 226d 6172 6b65 7273 223a 2022 7079 7468  "markers": "pyth
+00006660: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2733  on_version >= '3
+00006670: 2e37 2722 2c0a 2020 2020 2020 2020 2020  .7'",.          
+00006680: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
+00006690: 332e 352e 3322 0a20 2020 2020 2020 207d  3.5.3".        }
+000066a0: 2c0a 2020 2020 2020 2020 2270 6c75 6767  ,.        "plugg
+000066b0: 7922 3a20 7b0a 2020 2020 2020 2020 2020  y": {.          
+000066c0: 2020 2268 6173 6865 7322 3a20 5b0a 2020    "hashes": [.  
+000066d0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000066e0: 6861 3235 363a 3432 3234 3337 3362 6163  ha256:4224373bac
+000066f0: 6365 3535 6639 3535 6138 3738 6266 3963  ce55f955a878bf9c
+00006700: 6661 3736 3363 3165 3336 3038 3538 6533  fa763c1e360858e3
+00006710: 3330 3037 3230 3539 6531 3062 6164 3638  30072059e10bad68
+00006720: 3533 3131 3539 222c 0a20 2020 2020 2020  531159",.       
+00006730: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00006740: 3a37 3431 3334 6262 6634 3537 6630 3331  :74134bbf457f031
+00006750: 6133 3664 3638 3431 3665 3135 3039 6633  a36d68416e1509f3
+00006760: 3462 6435 6363 6330 3139 6630 6263 6339  4bd5ccc019f0bcc9
+00006770: 3532 6337 6239 3039 6430 3662 3337 6264  52c7b909d06b37bd
+00006780: 3322 0a20 2020 2020 2020 2020 2020 205d  3".            ]
+00006790: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+000067a0: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
+000067b0: 5f76 6572 7369 6f6e 203e 3d20 2733 2e36  _version >= '3.6
+000067c0: 2722 2c0a 2020 2020 2020 2020 2020 2020  '",.            
+000067d0: 2276 6572 7369 6f6e 223a 2022 3d3d 312e  "version": "==1.
+000067e0: 302e 3022 0a20 2020 2020 2020 207d 2c0a  0.0".        },.
+000067f0: 2020 2020 2020 2020 2270 7963 6f64 6573          "pycodes
+00006800: 7479 6c65 223a 207b 0a20 2020 2020 2020  tyle": {.       
+00006810: 2020 2020 2022 6861 7368 6573 223a 205b       "hashes": [
+00006820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006830: 2022 7368 6132 3536 3a33 3437 3138 3762   "sha256:347187b
+00006840: 6462 3437 3633 3239 6439 3866 3639 3563  db476329d98f695c
+00006850: 3231 3364 3732 3935 6138 3436 6431 3135  213d7295a846d115
+00006860: 3266 6634 6665 3962 6163 6238 6139 3539  2ff4fe9bacb8a959
+00006870: 3062 3865 6537 3035 3322 2c0a 2020 2020  0b8ee7053",.    
 00006880: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00006890: 3235 363a 3432 3234 3337 3362 6163 6365  256:4224373bacce
-000068a0: 3535 6639 3535 6138 3738 6266 3963 6661  55f955a878bf9cfa
-000068b0: 3736 3363 3165 3336 3038 3538 6533 3330  763c1e360858e330
-000068c0: 3037 3230 3539 6531 3062 6164 3638 3533  072059e10bad6853
-000068d0: 3131 3539 222c 0d0a 2020 2020 2020 2020  1159",..        
-000068e0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-000068f0: 3734 3133 3462 6266 3435 3766 3033 3161  74134bbf457f031a
-00006900: 3336 6436 3834 3136 6531 3530 3966 3334  36d68416e1509f34
-00006910: 6264 3563 6363 3031 3966 3062 6363 3935  bd5ccc019f0bcc95
-00006920: 3263 3762 3930 3964 3036 6233 3762 6433  2c7b909d06b37bd3
-00006930: 220d 0a20 2020 2020 2020 2020 2020 205d  "..            ]
-00006940: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00006950: 6d61 726b 6572 7322 3a20 2270 7974 686f  markers": "pytho
-00006960: 6e5f 7665 7273 696f 6e20 3e3d 2027 332e  n_version >= '3.
-00006970: 3627 222c 0d0a 2020 2020 2020 2020 2020  6'",..          
-00006980: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
-00006990: 312e 302e 3022 0d0a 2020 2020 2020 2020  1.0.0"..        
-000069a0: 7d2c 0d0a 2020 2020 2020 2020 2270 7963  },..        "pyc
-000069b0: 6f64 6573 7479 6c65 223a 207b 0d0a 2020  odestyle": {..  
-000069c0: 2020 2020 2020 2020 2020 2268 6173 6865            "hashe
-000069d0: 7322 3a20 5b0d 0a20 2020 2020 2020 2020  s": [..         
-000069e0: 2020 2020 2020 2022 7368 6132 3536 3a33         "sha256:3
-000069f0: 3437 3138 3762 6462 3437 3633 3239 6439  47187bdb476329d9
-00006a00: 3866 3639 3563 3231 3364 3732 3935 6138  8f695c213d7295a8
-00006a10: 3436 6431 3135 3266 6634 6665 3962 6163  46d1152ff4fe9bac
-00006a20: 6238 6139 3539 3062 3865 6537 3035 3322  b8a9590b8ee7053"
-00006a30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006a40: 2020 2022 7368 6132 3536 3a38 6134 6561     "sha256:8a4ea
-00006a50: 6630 6430 3439 3563 3733 3935 6264 6162  f0d0495c7395bdab
-00006a60: 3335 3839 6163 3264 6236 3032 3739 3764  3589ac2db602797d
-00006a70: 3736 3230 3732 3432 6331 3764 3437 3031  76207242c17d4701
-00006a80: 3836 3831 3537 3036 3631 3022 0d0a 2020  86815706610"..  
-00006a90: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00006aa0: 2020 2020 2020 2020 2020 226d 6172 6b65            "marke
-00006ab0: 7273 223a 2022 7079 7468 6f6e 5f76 6572  rs": "python_ver
-00006ac0: 7369 6f6e 203e 3d20 2733 2e36 2722 2c0d  sion >= '3.6'",.
-00006ad0: 0a20 2020 2020 2020 2020 2020 2022 7665  .            "ve
-00006ae0: 7273 696f 6e22 3a20 223d 3d32 2e31 302e  rsion": "==2.10.
-00006af0: 3022 0d0a 2020 2020 2020 2020 7d2c 0d0a  0"..        },..
-00006b00: 2020 2020 2020 2020 2270 7966 6c61 6b65          "pyflake
-00006b10: 7322 3a20 7b0d 0a20 2020 2020 2020 2020  s": {..         
-00006b20: 2020 2022 6861 7368 6573 223a 205b 0d0a     "hashes": [..
-00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b40: 2273 6861 3235 363a 6563 3535 6266 3766  "sha256:ec55bf7f
-00006b50: 6532 3166 6666 3766 3161 6432 6637 6461  e21fff7f1ad2f7da
-00006b60: 3632 3336 3364 3734 3965 3261 3437 3035  62363d749e2a4705
-00006b70: 3030 6561 6231 6235 3535 3333 3462 3637  00eab1b555334b67
-00006b80: 6161 3165 6638 6366 222c 0d0a 2020 2020  aa1ef8cf",..    
-00006b90: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00006ba0: 3235 363a 6563 3862 3237 3661 3662 3630  256:ec8b276a6b60
-00006bb0: 6264 3830 6465 6665 6432 3561 6464 3765  bd80defed25add7e
-00006bc0: 3433 3938 3831 6331 3965 3634 3835 3061  439881c19e64850a
-00006bd0: 6664 3962 3334 3632 3833 6434 3136 3566  fd9b346283d4165f
-00006be0: 6430 6664 220d 0a20 2020 2020 2020 2020  d0fd"..         
-00006bf0: 2020 205d 2c0d 0a20 2020 2020 2020 2020     ],..         
-00006c00: 2020 2022 6d61 726b 6572 7322 3a20 2270     "markers": "p
-00006c10: 7974 686f 6e5f 7665 7273 696f 6e20 3e3d  ython_version >=
-00006c20: 2027 332e 3627 222c 0d0a 2020 2020 2020   '3.6'",..      
-00006c30: 2020 2020 2020 2276 6572 7369 6f6e 223a        "version":
-00006c40: 2022 3d3d 332e 302e 3122 0d0a 2020 2020   "==3.0.1"..    
-00006c50: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00006c60: 2270 7967 6d65 6e74 7322 3a20 7b0d 0a20  "pygments": {.. 
-00006c70: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
-00006c80: 6573 223a 205b 0d0a 2020 2020 2020 2020  es": [..        
-00006c90: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00006ca0: 3861 6365 3464 3363 3164 6434 3831 3839  8ace4d3c1dd48189
-00006cb0: 3462 3230 3035 6635 3630 6561 6430 6639  4b2005f560ead0f9
-00006cc0: 6631 3965 6536 3466 6539 3833 3336 3662  f19ee64fe983366b
-00006cd0: 6531 6132 3165 3137 3164 3132 3737 3563  e1a21e171d12775c
-00006ce0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00006cf0: 2020 2020 2273 6861 3235 363a 6462 3264      "sha256:db2d
-00006d00: 6233 6465 6234 6234 3137 3966 3339 3961  b3deb4b4179f399a
-00006d10: 3039 3035 3462 3032 3362 3661 3538 3662  09054b023b6a586b
-00006d20: 3736 3439 3964 3336 3936 3538 3133 6337  76499d36965813c7
-00006d30: 3161 6138 6564 3762 3566 6431 220d 0a20  1aa8ed7b5fd1".. 
-00006d40: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00006d50: 2020 2020 2020 2020 2020 2022 6d61 726b             "mark
-00006d60: 6572 7322 3a20 2270 7974 686f 6e5f 7665  ers": "python_ve
-00006d70: 7273 696f 6e20 3e3d 2027 332e 3727 222c  rsion >= '3.7'",
-00006d80: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-00006d90: 6572 7369 6f6e 223a 2022 3d3d 322e 3135  ersion": "==2.15
-00006da0: 2e31 220d 0a20 2020 2020 2020 207d 2c0d  .1"..        },.
-00006db0: 0a20 2020 2020 2020 2022 7079 7072 6f6a  .        "pyproj
-00006dc0: 6563 742d 6170 6922 3a20 7b0d 0a20 2020  ect-api": {..   
-00006dd0: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
-00006de0: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00006df0: 2020 2020 2020 2273 6861 3235 363a 3433        "sha256:43
-00006e00: 3566 3436 3534 3761 3966 6632 3263 6634  5f46547a9ff22cf4
-00006e10: 3230 3865 6532 3734 6663 6133 6532 3836  208ee274fca3e286
-00006e20: 3961 6562 3036 3261 3438 3334 6164 6663  9aeb062a4834adfc
-00006e30: 3939 6134 6464 3634 6166 3363 6639 222c  99a4dd64af3cf9",
-00006e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006e50: 2020 2273 6861 3235 363a 3436 3938 6133    "sha256:4698a3
-00006e60: 3737 3763 3265 3066 3662 3632 3466 3861  777c2e0f6b624f8a
-00006e70: 3435 3939 3133 3165 3261 3235 3337 3664  4599131e2a25376d
-00006e80: 3930 6665 3864 3134 3664 3761 6337 3463  90fe8d146d7ac74c
-00006e90: 3637 6336 6639 3763 3433 220d 0a20 2020  67c6f97c43"..   
-00006ea0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00006eb0: 2020 2020 2020 2020 2022 6d61 726b 6572           "marker
-00006ec0: 7322 3a20 2270 7974 686f 6e5f 7665 7273  s": "python_vers
-00006ed0: 696f 6e20 3e3d 2027 332e 3727 222c 0d0a  ion >= '3.7'",..
-00006ee0: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
-00006ef0: 7369 6f6e 223a 2022 3d3d 312e 352e 3122  sion": "==1.5.1"
-00006f00: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00006f10: 2020 2020 2020 2270 7974 6573 7422 3a20        "pytest": 
-00006f20: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00006f30: 6861 7368 6573 223a 205b 0d0a 2020 2020  hashes": [..    
-00006f40: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00006f50: 3235 363a 6364 6362 6430 3132 6339 3331  256:cdcbd012c931
-00006f60: 3232 3538 3932 3266 3863 6433 6631 6236  2258922f8cd3f1b6
-00006f70: 3261 3635 3830 6664 6365 6431 3764 6236  2a6580fdced17db6
-00006f80: 3031 3438 3936 3035 3364 3437 6364 6466  014896053d47cddf
-00006f90: 3932 3935 222c 0d0a 2020 2020 2020 2020  9295",..        
-00006fa0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00006fb0: 6565 3939 3061 3363 6335 3562 6138 3038  ee990a3cc55ba808
-00006fc0: 6238 3037 3935 6137 3939 3434 3735 3666  b80795a79944756f
-00006fd0: 3331 3563 3637 6331 3262 3536 6162 6433  315c67c12b56abd3
-00006fe0: 6163 3939 3361 3762 3863 3137 3033 3062  ac993a7b8c17030b
-00006ff0: 220d 0a20 2020 2020 2020 2020 2020 205d  "..            ]
-00007000: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00007010: 696e 6465 7822 3a20 2270 7970 6922 2c0d  index": "pypi",.
-00007020: 0a20 2020 2020 2020 2020 2020 2022 7665  .            "ve
-00007030: 7273 696f 6e22 3a20 223d 3d37 2e33 2e32  rsion": "==7.3.2
-00007040: 220d 0a20 2020 2020 2020 207d 2c0d 0a20  "..        },.. 
-00007050: 2020 2020 2020 2022 7079 7769 6e33 322d         "pywin32-
-00007060: 6374 7970 6573 223a 207b 0d0a 2020 2020  ctypes": {..    
-00007070: 2020 2020 2020 2020 2268 6173 6865 7322          "hashes"
-00007080: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
-00007090: 2020 2020 2022 7368 6132 3536 3a32 3466       "sha256:24f
-000070a0: 6663 3362 3334 3164 3435 3764 3438 6538  fc3b341d457d48e8
-000070b0: 3932 3233 3532 3133 3063 6632 3634 3430  922352130cf26440
-000070c0: 3234 6134 6666 3039 3736 3261 3232 3631  24a4ff09762a2261
-000070d0: 6664 3334 6333 3665 6535 3934 3222 2c0d  fd34c36ee5942",.
-000070e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000070f0: 2022 7368 6132 3536 3a39 6463 3264 3939   "sha256:9dc2d99
-00007100: 3162 3334 3739 6363 3264 6631 3539 3330  1b3479cc2df15930
-00007110: 3935 3862 3637 3461 3438 6132 3237 6435  958b674a48a227d5
-00007120: 3336 3164 3431 3338 3237 6134 6366 6430  361d413827a4cfd0
-00007130: 6235 3837 3666 6339 3822 0d0a 2020 2020  b5876fc98"..    
-00007140: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00007150: 2020 2020 2020 2020 226d 6172 6b65 7273          "markers
-00007160: 223a 2022 7379 735f 706c 6174 666f 726d  ": "sys_platform
-00007170: 203d 3d20 2777 696e 3332 2722 2c0d 0a20   == 'win32'",.. 
-00007180: 2020 2020 2020 2020 2020 2022 7665 7273             "vers
-00007190: 696f 6e22 3a20 223d 3d30 2e32 2e30 220d  ion": "==0.2.0".
-000071a0: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-000071b0: 2020 2020 2022 7265 6164 6d65 2d72 656e       "readme-ren
-000071c0: 6465 7265 7222 3a20 7b0d 0a20 2020 2020  derer": {..     
-000071d0: 2020 2020 2020 2022 6861 7368 6573 223a         "hashes":
-000071e0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-000071f0: 2020 2020 2273 6861 3235 363a 6364 3635      "sha256:cd65
-00007200: 3331 3836 6466 6337 3330 3535 3635 3666  3186dfc73055656f
-00007210: 3039 3066 3232 3766 3563 6232 3261 3034  090f227f5cb22a04
-00007220: 3664 3766 3731 6138 3431 6466 6133 3035  6d7f71a841dfa305
-00007230: 6635 3563 3961 3531 3332 3733 222c 0d0a  f55c9a513273",..
-00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007250: 2273 6861 3235 363a 6636 3761 3136 6361  "sha256:f67a16ca
-00007260: 6564 6661 3731 6565 6634 3861 3331 6233  edfa71eef48a31b3
-00007270: 3937 3038 3633 3761 3666 3436 3634 6334  9708637a6f4664c4
-00007280: 3339 3438 3031 6137 6230 6436 3433 3264  394801a7b0d6432d
-00007290: 3133 3930 3733 3433 220d 0a20 2020 2020  13907343"..     
-000072a0: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-000072b0: 2020 2020 2020 2022 6d61 726b 6572 7322         "markers"
-000072c0: 3a20 2270 7974 686f 6e5f 7665 7273 696f  : "python_versio
-000072d0: 6e20 3e3d 2027 332e 3727 222c 0d0a 2020  n >= '3.7'",..  
-000072e0: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
-000072f0: 6f6e 223a 2022 3d3d 3337 2e33 220d 0a20  on": "==37.3".. 
-00007300: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00007310: 2020 2022 7265 7175 6573 7473 223a 207b     "requests": {
-00007320: 0d0a 2020 2020 2020 2020 2020 2020 2268  ..            "h
-00007330: 6173 6865 7322 3a20 5b0d 0a20 2020 2020  ashes": [..     
-00007340: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
-00007350: 3536 3a35 3863 6432 3138 3763 3031 6537  56:58cd2187c01e7
-00007360: 3065 3665 3236 3530 3562 6361 3735 3137  0e6e26505bca7517
-00007370: 3737 6161 3966 3265 6530 6237 6634 3330  77aa9f2ee0b7f430
-00007380: 3039 3838 6237 3039 6634 3465 3031 3330  0988b709f44e0130
-00007390: 3033 6622 2c0d 0a20 2020 2020 2020 2020  03f",..         
-000073a0: 2020 2020 2020 2022 7368 6132 3536 3a39         "sha256:9
-000073b0: 3432 6335 6137 3538 6639 3864 3739 3065  42c5a758f98d790e
-000073c0: 6165 6431 6132 3963 6236 6565 6663 3766  aed1a29cb6eefc7f
-000073d0: 6662 3064 3163 6637 6166 3035 6333 6432  fb0d1cf7af05c3d2
-000073e0: 3739 3136 3536 6462 6436 6164 3165 3122  791656dbd6ad1e1"
-000073f0: 0d0a 2020 2020 2020 2020 2020 2020 5d2c  ..            ],
-00007400: 0d0a 2020 2020 2020 2020 2020 2020 226d  ..            "m
-00007410: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
-00007420: 5f76 6572 7369 6f6e 203e 3d20 2733 2e37  _version >= '3.7
-00007430: 2722 2c0d 0a20 2020 2020 2020 2020 2020  '",..           
-00007440: 2022 7665 7273 696f 6e22 3a20 223d 3d32   "version": "==2
-00007450: 2e33 312e 3022 0d0a 2020 2020 2020 2020  .31.0"..        
-00007460: 7d2c 0d0a 2020 2020 2020 2020 2272 6571  },..        "req
-00007470: 7565 7374 732d 746f 6f6c 6265 6c74 223a  uests-toolbelt":
-00007480: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00007490: 2268 6173 6865 7322 3a20 5b0d 0a20 2020  "hashes": [..   
-000074a0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-000074b0: 6132 3536 3a37 3638 3161 3061 3364 3034  a256:7681a0a3d04
-000074c0: 3730 3132 6235 6264 6330 6565 3337 6437  7012b5bdc0ee37d7
-000074d0: 6638 6630 3765 6265 3736 6162 3038 6361  f8f07ebe76ab08ca
-000074e0: 6563 6366 6333 3932 3163 6532 3363 3838  eccfc3921ce23c88
-000074f0: 6435 6263 3622 2c0d 0a20 2020 2020 2020  d5bc6",..       
-00007500: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
-00007510: 3a63 6363 6664 6436 3635 6630 6132 3466  :cccfdd665f0a24f
-00007520: 6366 3437 3236 6536 3930 6636 3536 3339  cf4726e690f65639
-00007530: 6432 3732 6262 3036 3337 6239 6239 3264  d272bb0637b9b92d
-00007540: 6664 3931 6135 3536 3863 6366 3662 6430  fd91a5568ccf6bd0
-00007550: 3622 0d0a 2020 2020 2020 2020 2020 2020  6"..            
-00007560: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00007570: 226d 6172 6b65 7273 223a 2022 7079 7468  "markers": "pyth
-00007580: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2732  on_version >= '2
-00007590: 2e37 2720 616e 6420 7079 7468 6f6e 5f76  .7' and python_v
-000075a0: 6572 7369 6f6e 206e 6f74 2069 6e20 2733  ersion not in '3
-000075b0: 2e30 2c20 332e 312c 2033 2e32 2c20 332e  .0, 3.1, 3.2, 3.
-000075c0: 3327 222c 0d0a 2020 2020 2020 2020 2020  3'",..          
-000075d0: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
-000075e0: 312e 302e 3022 0d0a 2020 2020 2020 2020  1.0.0"..        
-000075f0: 7d2c 0d0a 2020 2020 2020 2020 2272 6663  },..        "rfc
-00007600: 3339 3836 223a 207b 0d0a 2020 2020 2020  3986": {..      
-00007610: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
-00007620: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-00007630: 2020 2022 7368 6132 3536 3a35 3062 3135     "sha256:50b15
-00007640: 3032 6236 3065 3238 3963 6233 3738 3833  02b60e289cb37883
-00007650: 6633 6466 6433 3435 3332 6238 3837 3363  f3dfd34532b8873c
-00007660: 3764 6539 6634 3962 6235 3436 3634 3163  7de9f49bb546641c
-00007670: 6539 6362 6432 3536 6562 6422 2c0d 0a20  e9cbd256ebd",.. 
-00007680: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007690: 7368 6132 3536 3a39 3761 6163 6639 6462  sha256:97aacf9db
-000076a0: 6434 6266 6438 3239 6261 6164 3665 3633  d4bfd829baad6e63
-000076b0: 3039 6661 3635 3733 6161 6631 6265 3366  09fa6573aaf1be3f
-000076c0: 3666 6137 3335 6338 6162 3035 6534 3663  6fa735c8ab05e46c
-000076d0: 6563 6232 3631 6322 0d0a 2020 2020 2020  ecb261c"..      
-000076e0: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
-000076f0: 2020 2020 2020 226d 6172 6b65 7273 223a        "markers":
-00007700: 2022 7079 7468 6f6e 5f76 6572 7369 6f6e   "python_version
-00007710: 203e 3d20 2733 2e37 2722 2c0d 0a20 2020   >= '3.7'",..   
-00007720: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
-00007730: 6e22 3a20 223d 3d32 2e30 2e30 220d 0a20  n": "==2.0.0".. 
-00007740: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00007750: 2020 2022 7269 6368 223a 207b 0d0a 2020     "rich": {..  
-00007760: 2020 2020 2020 2020 2020 2268 6173 6865            "hashe
-00007770: 7322 3a20 5b0d 0a20 2020 2020 2020 2020  s": [..         
-00007780: 2020 2020 2020 2022 7368 6132 3536 3a38         "sha256:8
-00007790: 6638 3762 6337 6565 3534 3637 3537 3332  f87bc7ee54675732
-000077a0: 6661 3636 6130 3565 6266 6534 3839 6532  fa66a05ebfe489e2
-000077b0: 3732 3634 6361 6565 6666 3337 3238 6339  7264caeeff3728c9
-000077c0: 3435 6432 3539 3731 6236 3438 3565 6322  45d25971b6485ec"
-000077d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000077e0: 2020 2022 7368 6132 3536 3a64 3635 3364     "sha256:d653d
-000077f0: 3662 6363 6564 6535 3834 3433 3034 6336  6bccede5844304c6
-00007800: 3035 6435 6161 6338 3032 6337 6366 3936  05d5aac802c7cf96
-00007810: 3231 6566 6437 3030 6234 3663 3765 6332  21efd700b46c7ec2
-00007820: 6235 3165 6139 3134 3839 3822 0d0a 2020  b51ea914898"..  
-00007830: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00007840: 2020 2020 2020 2020 2020 226d 6172 6b65            "marke
-00007850: 7273 223a 2022 7079 7468 6f6e 5f66 756c  rs": "python_ful
-00007860: 6c5f 7665 7273 696f 6e20 3e3d 2027 332e  l_version >= '3.
-00007870: 372e 3027 222c 0d0a 2020 2020 2020 2020  7.0'",..        
-00007880: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
-00007890: 3d3d 3133 2e34 2e32 220d 0a20 2020 2020  ==13.4.2"..     
-000078a0: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
-000078b0: 7369 7822 3a20 7b0d 0a20 2020 2020 2020  six": {..       
-000078c0: 2020 2020 2022 6861 7368 6573 223a 205b       "hashes": [
-000078d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000078e0: 2020 2273 6861 3235 363a 3165 3631 6333    "sha256:1e61c3
-000078f0: 3734 3737 6131 3632 3634 3538 6533 3666  7477a1626458e36f
-00007900: 3762 3164 3832 6161 3563 3962 3039 3466  7b1d82aa5c9b094f
-00007910: 6134 3830 3238 3932 3037 3265 3439 6465  a4802892072e49de
-00007920: 3963 3630 6334 6339 3236 222c 0d0a 2020  9c60c4c926",..  
-00007930: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00007940: 6861 3235 363a 3861 6262 3266 3164 3836  ha256:8abb2f1d86
-00007950: 3839 3061 3264 6662 3938 3966 3961 3737  890a2dfb989f9a77
-00007960: 6366 6366 6433 6534 3763 3261 3335 3462  cfcfd3e47c2a354b
-00007970: 3031 3131 3137 3731 3332 3666 3861 6132  01111771326f8aa2
-00007980: 3665 3032 3534 220d 0a20 2020 2020 2020  6e0254"..       
-00007990: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-000079a0: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
-000079b0: 2270 7974 686f 6e5f 7665 7273 696f 6e20  "python_version 
-000079c0: 3e3d 2027 322e 3727 2061 6e64 2070 7974  >= '2.7' and pyt
-000079d0: 686f 6e5f 7665 7273 696f 6e20 6e6f 7420  hon_version not 
-000079e0: 696e 2027 332e 302c 2033 2e31 2c20 332e  in '3.0, 3.1, 3.
-000079f0: 322c 2033 2e33 2722 2c0d 0a20 2020 2020  2, 3.3'",..     
-00007a00: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-00007a10: 3a20 223d 3d31 2e31 362e 3022 0d0a 2020  : "==1.16.0"..  
-00007a20: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00007a30: 2020 2274 6f78 223a 207b 0d0a 2020 2020    "tox": {..    
-00007a40: 2020 2020 2020 2020 2268 6173 6865 7322          "hashes"
-00007a50: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
-00007a60: 2020 2020 2022 7368 6132 3536 3a34 3837       "sha256:487
-00007a70: 3430 3030 3435 3365 3633 3761 3837 6361  4000453e637a87ca
-00007a80: 3839 3266 3937 3434 6132 6162 3961 3764  892f9744a2ab9a7d
-00007a90: 3234 3036 3464 6164 3162 3065 6362 6635  24064dad1b0ecbf5
-00007aa0: 6134 6333 6331 3436 6363 3733 3222 2c0d  a4c3c146cc732",.
-00007ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ac0: 2022 7368 6132 3536 3a39 3534 6631 6636   "sha256:954f1f6
-00007ad0: 3437 6636 3766 3438 3164 3233 3961 3139  47f67f481d239a19
-00007ae0: 3332 3838 3938 3332 3432 6136 3135 3262  3288983242a6152b
-00007af0: 3637 3530 3363 3461 3536 6231 3961 3461  67503c4a56b19a4a
-00007b00: 6166 6161 3239 3733 3622 0d0a 2020 2020  afaa29736"..    
-00007b10: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00007b20: 2020 2020 2020 2020 2269 6e64 6578 223a          "index":
-00007b30: 2022 7079 7069 222c 0d0a 2020 2020 2020   "pypi",..      
-00007b40: 2020 2020 2020 2276 6572 7369 6f6e 223a        "version":
-00007b50: 2022 3d3d 342e 362e 3022 0d0a 2020 2020   "==4.6.0"..    
-00007b60: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00007b70: 2274 7769 6e65 223a 207b 0d0a 2020 2020  "twine": {..    
-00007b80: 2020 2020 2020 2020 2268 6173 6865 7322          "hashes"
-00007b90: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
-00007ba0: 2020 2020 2022 7368 6132 3536 3a39 3239       "sha256:929
-00007bb0: 6263 3363 3238 3030 3333 3334 3761 3030  bc3c280033347a00
-00007bc0: 6638 3437 3233 3635 3634 6431 6335 3261  f847236564d1c52a
-00007bd0: 3365 3631 6231 6163 3235 3136 6339 3763  3e61b1ac2516c97c
-00007be0: 3438 6633 6365 6162 3735 3664 3822 2c0d  48f3ceab756d8",.
-00007bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007c00: 2022 7368 6132 3536 3a39 6531 3032 6566   "sha256:9e102ef
-00007c10: 3566 6464 3561 3230 3636 3165 6238 3866  5fdd5a20661eb88f
-00007c20: 6164 3436 3333 3838 3036 6333 6264 3332  ad46338806c3bd32
-00007c30: 6366 3164 6237 3239 3630 3366 6533 3639  cf1db729603fe369
-00007c40: 3762 3162 6338 3363 3822 0d0a 2020 2020  7b1bc83c8"..    
-00007c50: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00007c60: 2020 2020 2020 2020 2269 6e64 6578 223a          "index":
-00007c70: 2022 7079 7069 222c 0d0a 2020 2020 2020   "pypi",..      
-00007c80: 2020 2020 2020 2276 6572 7369 6f6e 223a        "version":
-00007c90: 2022 3d3d 342e 302e 3222 0d0a 2020 2020   "==4.0.2"..    
-00007ca0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00007cb0: 2274 7970 696e 672d 6578 7465 6e73 696f  "typing-extensio
-00007cc0: 6e73 223a 207b 0d0a 2020 2020 2020 2020  ns": {..        
-00007cd0: 2020 2020 2268 6173 6865 7322 3a20 5b0d      "hashes": [.
-00007ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007cf0: 2022 7368 6132 3536 3a38 3861 3431 3533   "sha256:88a4153
-00007d00: 6438 3530 3561 6162 6262 3465 3133 6161  d8505aabbb4e13aa
-00007d10: 6362 3763 3438 3663 3262 3461 3333 6361  cb7c486c2b4a33ca
-00007d20: 3362 3366 3830 3739 3134 6139 6234 6338  3b3f807914a9b4c8
-00007d30: 3434 6334 3731 6332 3622 2c0d 0a20 2020  44c471c26",..   
-00007d40: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00007d50: 6132 3536 3a64 3931 6435 3931 3933 3537  a256:d91d5919357
-00007d60: 6665 3766 3638 3161 3966 3262 3562 3463  fe7f681a9f2b5b4c
-00007d70: 6232 6135 6631 6566 3061 3165 3966 3539  b2a5f1ef0a1e9f59
-00007d80: 6334 6438 6666 3064 3334 3931 6530 3563  c4d8ff0d3491e05c
-00007d90: 3066 6664 3522 0d0a 2020 2020 2020 2020  0ffd5"..        
-00007da0: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
-00007db0: 2020 2020 226d 6172 6b65 7273 223a 2022      "markers": "
-00007dc0: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
-00007dd0: 3d20 2733 2e37 2722 2c0d 0a20 2020 2020  = '3.7'",..     
-00007de0: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-00007df0: 3a20 223d 3d34 2e36 2e33 220d 0a20 2020  : "==4.6.3"..   
-00007e00: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00007e10: 2022 7572 6c6c 6962 3322 3a20 7b0d 0a20   "urllib3": {.. 
-00007e20: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
-00007e30: 6573 223a 205b 0d0a 2020 2020 2020 2020  es": [..        
-00007e40: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
-00007e50: 3438 6537 6661 6661 3430 3331 3964 3335  48e7fafa40319d35
-00007e60: 3838 3438 6531 6263 3638 3039 6232 3038  8848e1bc6809b208
-00007e70: 3334 3066 6166 6532 3039 3666 3137 3235  340fafe2096f1725
-00007e80: 6430 3564 3637 3434 3364 3034 3833 6431  d05d67443d0483d1
-00007e90: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00007ea0: 2020 2020 2273 6861 3235 363a 6265 6532      "sha256:bee2
-00007eb0: 3862 3565 3536 6164 6462 3832 3236 6339  8b5e56addb8226c9
-00007ec0: 3666 3766 3133 6163 3238 6362 3463 3330  6f7f13ac28cb4c30
-00007ed0: 3164 6435 6561 3861 3663 6131 3739 6330  1dd5ea8a6ca179c0
-00007ee0: 6239 3833 3565 3033 3238 3235 220d 0a20  b9835e032825".. 
-00007ef0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00007f00: 2020 2020 2020 2020 2020 2022 6d61 726b             "mark
-00007f10: 6572 7322 3a20 2270 7974 686f 6e5f 7665  ers": "python_ve
-00007f20: 7273 696f 6e20 3e3d 2027 332e 3727 222c  rsion >= '3.7'",
-00007f30: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-00007f40: 6572 7369 6f6e 223a 2022 3d3d 322e 302e  ersion": "==2.0.
-00007f50: 3322 0d0a 2020 2020 2020 2020 7d2c 0d0a  3"..        },..
-00007f60: 2020 2020 2020 2020 2276 6972 7475 616c          "virtual
-00007f70: 656e 7622 3a20 7b0d 0a20 2020 2020 2020  env": {..       
-00007f80: 2020 2020 2022 6861 7368 6573 223a 205b       "hashes": [
-00007f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007fa0: 2020 2273 6861 3235 363a 3661 6265 6337    "sha256:6abec7
-00007fb0: 3637 3065 3538 3032 6135 3238 3335 3766  670e5802a528357f
-00007fc0: 6463 3735 6232 3662 3966 3537 6435 6439  dc75b26b9f57d5d9
-00007fd0: 3266 3239 6335 3436 3262 6130 6662 6534  2f29c5462ba0fbe4
-00007fe0: 3566 6561 6363 3638 3565 222c 0d0a 2020  5feacc685e",..  
-00007ff0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00008000: 6861 3235 363a 6138 3563 6161 3535 3463  ha256:a85caa554c
-00008010: 6564 3063 3061 6662 6430 6436 3338 6537  ed0c0afbd0d638e7
-00008020: 6532 6437 6235 6639 3264 3233 3437 3864  e2d7b5f92d23478d
-00008030: 3035 6431 3761 3736 6461 6561 6338 6632  05d17a76daeac8f2
-00008040: 3739 6639 3234 220d 0a20 2020 2020 2020  79f924"..       
-00008050: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-00008060: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
-00008070: 2270 7974 686f 6e5f 7665 7273 696f 6e20  "python_version 
-00008080: 3e3d 2027 332e 3727 222c 0d0a 2020 2020  >= '3.7'",..    
-00008090: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-000080a0: 223a 2022 3d3d 3230 2e32 332e 3022 0d0a  ": "==20.23.0"..
-000080b0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000080c0: 2020 2020 2277 6562 656e 636f 6469 6e67      "webencoding
-000080d0: 7322 3a20 7b0d 0a20 2020 2020 2020 2020  s": {..         
-000080e0: 2020 2022 6861 7368 6573 223a 205b 0d0a     "hashes": [..
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2273 6861 3235 363a 6130 6166 3132 3133  "sha256:a0af1213
-00008110: 6633 6332 3232 3634 3937 6139 3765 3262  f3c2226497a97e2b
-00008120: 3361 6130 3161 3765 3462 6565 3466 3430  3aa01a7e4bee4f40
-00008130: 3366 3935 6265 3136 6663 3961 6364 3239  3f95be16fc9acd29
-00008140: 3437 3531 3461 3738 222c 0d0a 2020 2020  47514a78",..    
-00008150: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00008160: 3235 363a 6233 3661 3163 3234 3566 3264  256:b36a1c245f2d
-00008170: 3330 3439 3635 6562 3465 3061 3832 3834  304965eb4e0a8284
-00008180: 3833 3739 3234 3164 6330 3462 3836 3561  8379241dc04b865a
-00008190: 6663 6334 6161 6231 3637 3438 3538 3765  fcc4aab16748587e
-000081a0: 3139 3233 220d 0a20 2020 2020 2020 2020  1923"..         
-000081b0: 2020 205d 2c0d 0a20 2020 2020 2020 2020     ],..         
-000081c0: 2020 2022 7665 7273 696f 6e22 3a20 223d     "version": "=
-000081d0: 3d30 2e35 2e31 220d 0a20 2020 2020 2020  =0.5.1"..       
-000081e0: 207d 2c0d 0a20 2020 2020 2020 2022 7a69   },..        "zi
-000081f0: 7070 223a 207b 0d0a 2020 2020 2020 2020  pp": {..        
-00008200: 2020 2020 2268 6173 6865 7322 3a20 5b0d      "hashes": [.
-00008210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008220: 2022 7368 6132 3536 3a31 3132 3932 3961   "sha256:112929a
-00008230: 6436 3439 6461 3934 3163 3233 6465 3530  d649da941c23de50
-00008240: 6633 3536 6132 6235 3537 3063 3935 3462  f356a2b5570c954b
-00008250: 3635 3135 3036 3432 6263 6364 6436 3662  65150642bccdd66b
-00008260: 6631 3934 6432 3234 6222 2c0d 0a20 2020  f194d224b",..   
-00008270: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00008280: 6132 3536 3a34 3839 3034 6663 3736 6136  a256:48904fc76a6
-00008290: 3065 3534 3261 6631 3531 6164 6564 3935  0e542af151aded95
-000082a0: 3732 3663 3161 3563 3334 6564 3433 6162  726c1a5c34ed43ab
-000082b0: 3431 3334 6235 3937 3636 3563 3836 6437  4134b597665c86d7
-000082c0: 6164 3535 3622 0d0a 2020 2020 2020 2020  ad556"..        
-000082d0: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
-000082e0: 2020 2020 226d 6172 6b65 7273 223a 2022      "markers": "
-000082f0: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
-00008300: 3d20 2733 2e37 2722 2c0d 0a20 2020 2020  = '3.7'",..     
-00008310: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-00008320: 3a20 223d 3d33 2e31 352e 3022 0d0a 2020  : "==3.15.0"..  
-00008330: 2020 2020 2020 7d0d 0a20 2020 207d 0d0a        }..    }..
-00008340: 7d0d 0a                                  }..
+00006890: 3235 363a 3861 3465 6166 3064 3034 3935  256:8a4eaf0d0495
+000068a0: 6337 3339 3562 6461 6233 3538 3961 6332  c7395bdab3589ac2
+000068b0: 6462 3630 3237 3937 6437 3632 3037 3234  db602797d7620724
+000068c0: 3263 3137 6434 3730 3138 3638 3135 3730  2c17d47018681570
+000068d0: 3636 3130 220a 2020 2020 2020 2020 2020  6610".          
+000068e0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+000068f0: 2022 6d61 726b 6572 7322 3a20 2270 7974   "markers": "pyt
+00006900: 686f 6e5f 7665 7273 696f 6e20 3e3d 2027  hon_version >= '
+00006910: 332e 3627 222c 0a20 2020 2020 2020 2020  3.6'",.         
+00006920: 2020 2022 7665 7273 696f 6e22 3a20 223d     "version": "=
+00006930: 3d32 2e31 302e 3022 0a20 2020 2020 2020  =2.10.0".       
+00006940: 207d 2c0a 2020 2020 2020 2020 2270 7966   },.        "pyf
+00006950: 6c61 6b65 7322 3a20 7b0a 2020 2020 2020  lakes": {.      
+00006960: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
+00006970: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00006980: 2020 2273 6861 3235 363a 6563 3535 6266    "sha256:ec55bf
+00006990: 3766 6532 3166 6666 3766 3161 6432 6637  7fe21fff7f1ad2f7
+000069a0: 6461 3632 3336 3364 3734 3965 3261 3437  da62363d749e2a47
+000069b0: 3035 3030 6561 6231 6235 3535 3333 3462  0500eab1b555334b
+000069c0: 3637 6161 3165 6638 6366 222c 0a20 2020  67aa1ef8cf",.   
+000069d0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+000069e0: 6132 3536 3a65 6338 6232 3736 6136 6236  a256:ec8b276a6b6
+000069f0: 3062 6438 3064 6566 6564 3235 6164 6437  0bd80defed25add7
+00006a00: 6534 3339 3838 3163 3139 6536 3438 3530  e439881c19e64850
+00006a10: 6166 6439 6233 3436 3238 3364 3431 3635  afd9b346283d4165
+00006a20: 6664 3066 6422 0a20 2020 2020 2020 2020  fd0fd".         
+00006a30: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+00006a40: 2020 226d 6172 6b65 7273 223a 2022 7079    "markers": "py
+00006a50: 7468 6f6e 5f76 6572 7369 6f6e 203e 3d20  thon_version >= 
+00006a60: 2733 2e36 2722 2c0a 2020 2020 2020 2020  '3.6'",.        
+00006a70: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
+00006a80: 3d3d 332e 302e 3122 0a20 2020 2020 2020  ==3.0.1".       
+00006a90: 207d 2c0a 2020 2020 2020 2020 2270 7967   },.        "pyg
+00006aa0: 6d65 6e74 7322 3a20 7b0a 2020 2020 2020  ments": {.      
+00006ab0: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
+00006ac0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00006ad0: 2020 2273 6861 3235 363a 3861 6365 3464    "sha256:8ace4d
+00006ae0: 3363 3164 6434 3831 3839 3462 3230 3035  3c1dd481894b2005
+00006af0: 6635 3630 6561 6430 6639 6631 3965 6536  f560ead0f9f19ee6
+00006b00: 3466 6539 3833 3336 3662 6531 6132 3165  4fe983366be1a21e
+00006b10: 3137 3164 3132 3737 3563 222c 0a20 2020  171d12775c",.   
+00006b20: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00006b30: 6132 3536 3a64 6232 6462 3364 6562 3462  a256:db2db3deb4b
+00006b40: 3431 3739 6633 3939 6130 3930 3534 6230  4179f399a09054b0
+00006b50: 3233 6236 6135 3836 6237 3634 3939 6433  23b6a586b76499d3
+00006b60: 3639 3635 3831 3363 3731 6161 3865 6437  6965813c71aa8ed7
+00006b70: 6235 6664 3122 0a20 2020 2020 2020 2020  b5fd1".         
+00006b80: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+00006b90: 2020 226d 6172 6b65 7273 223a 2022 7079    "markers": "py
+00006ba0: 7468 6f6e 5f76 6572 7369 6f6e 203e 3d20  thon_version >= 
+00006bb0: 2733 2e37 2722 2c0a 2020 2020 2020 2020  '3.7'",.        
+00006bc0: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
+00006bd0: 3d3d 322e 3135 2e31 220a 2020 2020 2020  ==2.15.1".      
+00006be0: 2020 7d2c 0a20 2020 2020 2020 2022 7079    },.        "py
+00006bf0: 7072 6f6a 6563 742d 6170 6922 3a20 7b0a  project-api": {.
+00006c00: 2020 2020 2020 2020 2020 2020 2268 6173              "has
+00006c10: 6865 7322 3a20 5b0a 2020 2020 2020 2020  hes": [.        
+00006c20: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+00006c30: 3433 3566 3436 3534 3761 3966 6632 3263  435f46547a9ff22c
+00006c40: 6634 3230 3865 6532 3734 6663 6133 6532  f4208ee274fca3e2
+00006c50: 3836 3961 6562 3036 3261 3438 3334 6164  869aeb062a4834ad
+00006c60: 6663 3939 6134 6464 3634 6166 3363 6639  fc99a4dd64af3cf9
+00006c70: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006c80: 2020 2022 7368 6132 3536 3a34 3639 3861     "sha256:4698a
+00006c90: 3337 3737 6332 6530 6636 6236 3234 6638  3777c2e0f6b624f8
+00006ca0: 6134 3539 3931 3331 6532 6132 3533 3736  a4599131e2a25376
+00006cb0: 6439 3066 6538 6431 3436 6437 6163 3734  d90fe8d146d7ac74
+00006cc0: 6336 3763 3666 3937 6334 3322 0a20 2020  c67c6f97c43".   
+00006cd0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00006ce0: 2020 2020 2020 2020 226d 6172 6b65 7273          "markers
+00006cf0: 223a 2022 7079 7468 6f6e 5f76 6572 7369  ": "python_versi
+00006d00: 6f6e 203e 3d20 2733 2e37 2722 2c0a 2020  on >= '3.7'",.  
+00006d10: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
+00006d20: 6f6e 223a 2022 3d3d 312e 352e 3122 0a20  on": "==1.5.1". 
+00006d30: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00006d40: 2020 2270 7974 6573 7422 3a20 7b0a 2020    "pytest": {.  
+00006d50: 2020 2020 2020 2020 2020 2268 6173 6865            "hashe
+00006d60: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+00006d70: 2020 2020 2020 2273 6861 3235 363a 6364        "sha256:cd
+00006d80: 6362 6430 3132 6339 3331 3232 3538 3932  cbd012c931225892
+00006d90: 3266 3863 6433 6631 6236 3261 3635 3830  2f8cd3f1b62a6580
+00006da0: 6664 6365 6431 3764 6236 3031 3438 3936  fdced17db6014896
+00006db0: 3035 3364 3437 6364 6466 3932 3935 222c  053d47cddf9295",
+00006dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006dd0: 2022 7368 6132 3536 3a65 6539 3930 6133   "sha256:ee990a3
+00006de0: 6363 3535 6261 3830 3862 3830 3739 3561  cc55ba808b80795a
+00006df0: 3739 3934 3437 3536 6633 3135 6336 3763  79944756f315c67c
+00006e00: 3132 6235 3661 6264 3361 6339 3933 6137  12b56abd3ac993a7
+00006e10: 6238 6331 3730 3330 6222 0a20 2020 2020  b8c17030b".     
+00006e20: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00006e30: 2020 2020 2020 2269 6e64 6578 223a 2022        "index": "
+00006e40: 7079 7069 222c 0a20 2020 2020 2020 2020  pypi",.         
+00006e50: 2020 2022 7665 7273 696f 6e22 3a20 223d     "version": "=
+00006e60: 3d37 2e33 2e32 220a 2020 2020 2020 2020  =7.3.2".        
+00006e70: 7d2c 0a20 2020 2020 2020 2022 7079 7769  },.        "pywi
+00006e80: 6e33 322d 6374 7970 6573 223a 207b 0a20  n32-ctypes": {. 
+00006e90: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+00006ea0: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
+00006eb0: 2020 2020 2020 2022 7368 6132 3536 3a32         "sha256:2
+00006ec0: 3466 6663 3362 3334 3164 3435 3764 3438  4ffc3b341d457d48
+00006ed0: 6538 3932 3233 3532 3133 3063 6632 3634  e8922352130cf264
+00006ee0: 3430 3234 6134 6666 3039 3736 3261 3232  4024a4ff09762a22
+00006ef0: 3631 6664 3334 6333 3665 6535 3934 3222  61fd34c36ee5942"
+00006f00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006f10: 2020 2273 6861 3235 363a 3964 6332 6439    "sha256:9dc2d9
+00006f20: 3931 6233 3437 3963 6332 6466 3135 3933  91b3479cc2df1593
+00006f30: 3039 3538 6236 3734 6134 3861 3232 3764  0958b674a48a227d
+00006f40: 3533 3631 6434 3133 3832 3761 3463 6664  5361d413827a4cfd
+00006f50: 3062 3538 3736 6663 3938 220a 2020 2020  0b5876fc98".    
+00006f60: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00006f70: 2020 2020 2020 2022 6d61 726b 6572 7322         "markers"
+00006f80: 3a20 2273 7973 5f70 6c61 7466 6f72 6d20  : "sys_platform 
+00006f90: 3d3d 2027 7769 6e33 3227 222c 0a20 2020  == 'win32'",.   
+00006fa0: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
+00006fb0: 6e22 3a20 223d 3d30 2e32 2e30 220a 2020  n": "==0.2.0".  
+00006fc0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00006fd0: 2022 7265 6164 6d65 2d72 656e 6465 7265   "readme-rendere
+00006fe0: 7222 3a20 7b0a 2020 2020 2020 2020 2020  r": {.          
+00006ff0: 2020 2268 6173 6865 7322 3a20 5b0a 2020    "hashes": [.  
+00007000: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00007010: 6861 3235 363a 6364 3635 3331 3836 6466  ha256:cd653186df
+00007020: 6337 3330 3535 3635 3666 3039 3066 3232  c73055656f090f22
+00007030: 3766 3563 6232 3261 3034 3664 3766 3731  7f5cb22a046d7f71
+00007040: 6138 3431 6466 6133 3035 6635 3563 3961  a841dfa305f55c9a
+00007050: 3531 3332 3733 222c 0a20 2020 2020 2020  513273",.       
+00007060: 2020 2020 2020 2020 2022 7368 6132 3536           "sha256
+00007070: 3a66 3637 6131 3663 6165 6466 6137 3165  :f67a16caedfa71e
+00007080: 6566 3438 6133 3162 3339 3730 3836 3337  ef48a31b39708637
+00007090: 6136 6634 3636 3463 3433 3934 3830 3161  a6f4664c4394801a
+000070a0: 3762 3064 3634 3332 6431 3339 3037 3334  7b0d6432d1390734
+000070b0: 3322 0a20 2020 2020 2020 2020 2020 205d  3".            ]
+000070c0: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+000070d0: 6172 6b65 7273 223a 2022 7079 7468 6f6e  arkers": "python
+000070e0: 5f76 6572 7369 6f6e 203e 3d20 2733 2e37  _version >= '3.7
+000070f0: 2722 2c0a 2020 2020 2020 2020 2020 2020  '",.            
+00007100: 2276 6572 7369 6f6e 223a 2022 3d3d 3337  "version": "==37
+00007110: 2e33 220a 2020 2020 2020 2020 7d2c 0a20  .3".        },. 
+00007120: 2020 2020 2020 2022 7265 7175 6573 7473         "requests
+00007130: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00007140: 2022 6861 7368 6573 223a 205b 0a20 2020   "hashes": [.   
+00007150: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00007160: 6132 3536 3a35 3863 6432 3138 3763 3031  a256:58cd2187c01
+00007170: 6537 3065 3665 3236 3530 3562 6361 3735  e70e6e26505bca75
+00007180: 3137 3737 6161 3966 3265 6530 6237 6634  1777aa9f2ee0b7f4
+00007190: 3330 3039 3838 6237 3039 6634 3465 3031  300988b709f44e01
+000071a0: 3330 3033 6622 2c0a 2020 2020 2020 2020  3003f",.        
+000071b0: 2020 2020 2020 2020 2273 6861 3235 363a          "sha256:
+000071c0: 3934 3263 3561 3735 3866 3938 6437 3930  942c5a758f98d790
+000071d0: 6561 6564 3161 3239 6362 3665 6566 6337  eaed1a29cb6eefc7
+000071e0: 6666 6230 6431 6366 3761 6630 3563 3364  ffb0d1cf7af05c3d
+000071f0: 3237 3931 3635 3664 6264 3661 6431 6531  2791656dbd6ad1e1
+00007200: 220a 2020 2020 2020 2020 2020 2020 5d2c  ".            ],
+00007210: 0a20 2020 2020 2020 2020 2020 2022 6d61  .            "ma
+00007220: 726b 6572 7322 3a20 2270 7974 686f 6e5f  rkers": "python_
+00007230: 7665 7273 696f 6e20 3e3d 2027 332e 3727  version >= '3.7'
+00007240: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00007250: 7665 7273 696f 6e22 3a20 223d 3d32 2e33  version": "==2.3
+00007260: 312e 3022 0a20 2020 2020 2020 207d 2c0a  1.0".        },.
+00007270: 2020 2020 2020 2020 2272 6571 7565 7374          "request
+00007280: 732d 746f 6f6c 6265 6c74 223a 207b 0a20  s-toolbelt": {. 
+00007290: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+000072a0: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
+000072b0: 2020 2020 2020 2022 7368 6132 3536 3a37         "sha256:7
+000072c0: 3638 3161 3061 3364 3034 3730 3132 6235  681a0a3d047012b5
+000072d0: 6264 6330 6565 3337 6437 6638 6630 3765  bdc0ee37d7f8f07e
+000072e0: 6265 3736 6162 3038 6361 6563 6366 6333  be76ab08caeccfc3
+000072f0: 3932 3163 6532 3363 3838 6435 6263 3622  921ce23c88d5bc6"
+00007300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007310: 2020 2273 6861 3235 363a 6363 6366 6464    "sha256:cccfdd
+00007320: 3636 3566 3061 3234 6663 6634 3732 3665  665f0a24fcf4726e
+00007330: 3639 3066 3635 3633 3964 3237 3262 6230  690f65639d272bb0
+00007340: 3633 3762 3962 3932 6466 6439 3161 3535  637b9b92dfd91a55
+00007350: 3638 6363 6636 6264 3036 220a 2020 2020  68ccf6bd06".    
+00007360: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00007370: 2020 2020 2020 2022 6d61 726b 6572 7322         "markers"
+00007380: 3a20 2270 7974 686f 6e5f 7665 7273 696f  : "python_versio
+00007390: 6e20 3e3d 2027 322e 3727 2061 6e64 2070  n >= '2.7' and p
+000073a0: 7974 686f 6e5f 7665 7273 696f 6e20 6e6f  ython_version no
+000073b0: 7420 696e 2027 332e 302c 2033 2e31 2c20  t in '3.0, 3.1, 
+000073c0: 332e 322c 2033 2e33 2722 2c0a 2020 2020  3.2, 3.3'",.    
+000073d0: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+000073e0: 223a 2022 3d3d 312e 302e 3022 0a20 2020  ": "==1.0.0".   
+000073f0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00007400: 2272 6663 3339 3836 223a 207b 0a20 2020  "rfc3986": {.   
+00007410: 2020 2020 2020 2020 2022 6861 7368 6573           "hashes
+00007420: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00007430: 2020 2020 2022 7368 6132 3536 3a35 3062       "sha256:50b
+00007440: 3135 3032 6236 3065 3238 3963 6233 3738  1502b60e289cb378
+00007450: 3833 6633 6466 6433 3435 3332 6238 3837  83f3dfd34532b887
+00007460: 3363 3764 6539 6634 3962 6235 3436 3634  3c7de9f49bb54664
+00007470: 3163 6539 6362 6432 3536 6562 6422 2c0a  1ce9cbd256ebd",.
+00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007490: 2273 6861 3235 363a 3937 6161 6366 3964  "sha256:97aacf9d
+000074a0: 6264 3462 6664 3832 3962 6161 6436 6536  bd4bfd829baad6e6
+000074b0: 3330 3966 6136 3537 3361 6166 3162 6533  309fa6573aaf1be3
+000074c0: 6636 6661 3733 3563 3861 6230 3565 3436  f6fa735c8ab05e46
+000074d0: 6365 6362 3236 3163 220a 2020 2020 2020  cecb261c".      
+000074e0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+000074f0: 2020 2020 2022 6d61 726b 6572 7322 3a20       "markers": 
+00007500: 2270 7974 686f 6e5f 7665 7273 696f 6e20  "python_version 
+00007510: 3e3d 2027 332e 3727 222c 0a20 2020 2020  >= '3.7'",.     
+00007520: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
+00007530: 3a20 223d 3d32 2e30 2e30 220a 2020 2020  : "==2.0.0".    
+00007540: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00007550: 7269 6368 223a 207b 0a20 2020 2020 2020  rich": {.       
+00007560: 2020 2020 2022 6861 7368 6573 223a 205b       "hashes": [
+00007570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007580: 2022 7368 6132 3536 3a38 6638 3762 6337   "sha256:8f87bc7
+00007590: 6565 3534 3637 3537 3332 6661 3636 6130  ee54675732fa66a0
+000075a0: 3565 6266 6534 3839 6532 3732 3634 6361  5ebfe489e27264ca
+000075b0: 6565 6666 3337 3238 6339 3435 6432 3539  eeff3728c945d259
+000075c0: 3731 6236 3438 3565 6322 2c0a 2020 2020  71b6485ec",.    
+000075d0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+000075e0: 3235 363a 6436 3533 6436 6263 6365 6465  256:d653d6bccede
+000075f0: 3538 3434 3330 3463 3630 3564 3561 6163  5844304c605d5aac
+00007600: 3830 3263 3763 6639 3632 3165 6664 3730  802c7cf9621efd70
+00007610: 3062 3436 6337 6563 3262 3531 6561 3931  0b46c7ec2b51ea91
+00007620: 3438 3938 220a 2020 2020 2020 2020 2020  4898".          
+00007630: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+00007640: 2022 6d61 726b 6572 7322 3a20 2270 7974   "markers": "pyt
+00007650: 686f 6e5f 6675 6c6c 5f76 6572 7369 6f6e  hon_full_version
+00007660: 203e 3d20 2733 2e37 2e30 2722 2c0a 2020   >= '3.7.0'",.  
+00007670: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
+00007680: 6f6e 223a 2022 3d3d 3133 2e34 2e32 220a  on": "==13.4.2".
+00007690: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000076a0: 2020 2022 7369 7822 3a20 7b0a 2020 2020     "six": {.    
+000076b0: 2020 2020 2020 2020 2268 6173 6865 7322          "hashes"
+000076c0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+000076d0: 2020 2020 2273 6861 3235 363a 3165 3631      "sha256:1e61
+000076e0: 6333 3734 3737 6131 3632 3634 3538 6533  c37477a1626458e3
+000076f0: 3666 3762 3164 3832 6161 3563 3962 3039  6f7b1d82aa5c9b09
+00007700: 3466 6134 3830 3238 3932 3037 3265 3439  4fa4802892072e49
+00007710: 6465 3963 3630 6334 6339 3236 222c 0a20  de9c60c4c926",. 
+00007720: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007730: 7368 6132 3536 3a38 6162 6232 6631 6438  sha256:8abb2f1d8
+00007740: 3638 3930 6132 6466 6239 3839 6639 6137  6890a2dfb989f9a7
+00007750: 3763 6663 6664 3365 3437 6332 6133 3534  7cfcfd3e47c2a354
+00007760: 6230 3131 3131 3737 3133 3236 6638 6161  b01111771326f8aa
+00007770: 3236 6530 3235 3422 0a20 2020 2020 2020  26e0254".       
+00007780: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00007790: 2020 2020 226d 6172 6b65 7273 223a 2022      "markers": "
+000077a0: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
+000077b0: 3d20 2732 2e37 2720 616e 6420 7079 7468  = '2.7' and pyth
+000077c0: 6f6e 5f76 6572 7369 6f6e 206e 6f74 2069  on_version not i
+000077d0: 6e20 2733 2e30 2c20 332e 312c 2033 2e32  n '3.0, 3.1, 3.2
+000077e0: 2c20 332e 3327 222c 0a20 2020 2020 2020  , 3.3'",.       
+000077f0: 2020 2020 2022 7665 7273 696f 6e22 3a20       "version": 
+00007800: 223d 3d31 2e31 362e 3022 0a20 2020 2020  "==1.16.0".     
+00007810: 2020 207d 2c0a 2020 2020 2020 2020 2274     },.        "t
+00007820: 6f78 223a 207b 0a20 2020 2020 2020 2020  ox": {.         
+00007830: 2020 2022 6861 7368 6573 223a 205b 0a20     "hashes": [. 
+00007840: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007850: 7368 6132 3536 3a34 3837 3430 3030 3435  sha256:487400045
+00007860: 3365 3633 3761 3837 6361 3839 3266 3937  3e637a87ca892f97
+00007870: 3434 6132 6162 3961 3764 3234 3036 3464  44a2ab9a7d24064d
+00007880: 6164 3162 3065 6362 6635 6134 6333 6331  ad1b0ecbf5a4c3c1
+00007890: 3436 6363 3733 3222 2c0a 2020 2020 2020  46cc732",.      
+000078a0: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+000078b0: 363a 3935 3466 3166 3634 3766 3637 6634  6:954f1f647f67f4
+000078c0: 3831 6432 3339 6131 3933 3238 3839 3833  81d239a193288983
+000078d0: 3234 3261 3631 3532 6236 3735 3033 6334  242a6152b67503c4
+000078e0: 6135 3662 3139 6134 6161 6661 6132 3937  a56b19a4aafaa297
+000078f0: 3336 220a 2020 2020 2020 2020 2020 2020  36".            
+00007900: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00007910: 696e 6465 7822 3a20 2270 7970 6922 2c0a  index": "pypi",.
+00007920: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
+00007930: 7369 6f6e 223a 2022 3d3d 342e 362e 3022  sion": "==4.6.0"
+00007940: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00007950: 2020 2020 2274 7769 6e65 223a 207b 0a20      "twine": {. 
+00007960: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+00007970: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
+00007980: 2020 2020 2020 2022 7368 6132 3536 3a39         "sha256:9
+00007990: 3239 6263 3363 3238 3030 3333 3334 3761  29bc3c280033347a
+000079a0: 3030 6638 3437 3233 3635 3634 6431 6335  00f847236564d1c5
+000079b0: 3261 3365 3631 6231 6163 3235 3136 6339  2a3e61b1ac2516c9
+000079c0: 3763 3438 6633 6365 6162 3735 3664 3822  7c48f3ceab756d8"
+000079d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000079e0: 2020 2273 6861 3235 363a 3965 3130 3265    "sha256:9e102e
+000079f0: 6635 6664 6435 6132 3036 3631 6562 3838  f5fdd5a20661eb88
+00007a00: 6661 6434 3633 3338 3830 3663 3362 6433  fad46338806c3bd3
+00007a10: 3263 6631 6462 3732 3936 3033 6665 3336  2cf1db729603fe36
+00007a20: 3937 6231 6263 3833 6338 220a 2020 2020  97b1bc83c8".    
+00007a30: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00007a40: 2020 2020 2020 2022 696e 6465 7822 3a20         "index": 
+00007a50: 2270 7970 6922 2c0a 2020 2020 2020 2020  "pypi",.        
+00007a60: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
+00007a70: 3d3d 342e 302e 3222 0a20 2020 2020 2020  ==4.0.2".       
+00007a80: 207d 2c0a 2020 2020 2020 2020 2274 7970   },.        "typ
+00007a90: 696e 672d 6578 7465 6e73 696f 6e73 223a  ing-extensions":
+00007aa0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00007ab0: 6861 7368 6573 223a 205b 0a20 2020 2020  hashes": [.     
+00007ac0: 2020 2020 2020 2020 2020 2022 7368 6132             "sha2
+00007ad0: 3536 3a38 3861 3431 3533 6438 3530 3561  56:88a4153d8505a
+00007ae0: 6162 6262 3465 3133 6161 6362 3763 3438  abbb4e13aacb7c48
+00007af0: 3663 3262 3461 3333 6361 3362 3366 3830  6c2b4a33ca3b3f80
+00007b00: 3739 3134 6139 6234 6338 3434 6334 3731  7914a9b4c844c471
+00007b10: 6332 3622 2c0a 2020 2020 2020 2020 2020  c26",.          
+00007b20: 2020 2020 2020 2273 6861 3235 363a 6439        "sha256:d9
+00007b30: 3164 3539 3139 3335 3766 6537 6636 3831  1d5919357fe7f681
+00007b40: 6139 6632 6235 6234 6362 3261 3566 3165  a9f2b5b4cb2a5f1e
+00007b50: 6630 6131 6539 6635 3963 3464 3866 6630  f0a1e9f59c4d8ff0
+00007b60: 6433 3439 3165 3035 6330 6666 6435 220a  d3491e05c0ffd5".
+00007b70: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00007b80: 2020 2020 2020 2020 2020 2022 6d61 726b             "mark
+00007b90: 6572 7322 3a20 2270 7974 686f 6e5f 7665  ers": "python_ve
+00007ba0: 7273 696f 6e20 3e3d 2027 332e 3727 222c  rsion >= '3.7'",
+00007bb0: 0a20 2020 2020 2020 2020 2020 2022 7665  .            "ve
+00007bc0: 7273 696f 6e22 3a20 223d 3d34 2e36 2e33  rsion": "==4.6.3
+00007bd0: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
+00007be0: 2020 2020 2022 7572 6c6c 6962 3322 3a20       "urllib3": 
+00007bf0: 7b0a 2020 2020 2020 2020 2020 2020 2268  {.            "h
+00007c00: 6173 6865 7322 3a20 5b0a 2020 2020 2020  ashes": [.      
+00007c10: 2020 2020 2020 2020 2020 2273 6861 3235            "sha25
+00007c20: 363a 3438 6537 6661 6661 3430 3331 3964  6:48e7fafa40319d
+00007c30: 3335 3838 3438 6531 6263 3638 3039 6232  358848e1bc6809b2
+00007c40: 3038 3334 3066 6166 6532 3039 3666 3137  08340fafe2096f17
+00007c50: 3235 6430 3564 3637 3434 3364 3034 3833  25d05d67443d0483
+00007c60: 6431 222c 0a20 2020 2020 2020 2020 2020  d1",.           
+00007c70: 2020 2020 2022 7368 6132 3536 3a62 6565       "sha256:bee
+00007c80: 3238 6235 6535 3661 6464 6238 3232 3663  28b5e56addb8226c
+00007c90: 3936 6637 6631 3361 6332 3863 6234 6333  96f7f13ac28cb4c3
+00007ca0: 3031 6464 3565 6138 6136 6361 3137 3963  01dd5ea8a6ca179c
+00007cb0: 3062 3938 3335 6530 3332 3832 3522 0a20  0b9835e032825". 
+00007cc0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+00007cd0: 2020 2020 2020 2020 2020 226d 6172 6b65            "marke
+00007ce0: 7273 223a 2022 7079 7468 6f6e 5f76 6572  rs": "python_ver
+00007cf0: 7369 6f6e 203e 3d20 2733 2e37 2722 2c0a  sion >= '3.7'",.
+00007d00: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
+00007d10: 7369 6f6e 223a 2022 3d3d 322e 302e 3322  sion": "==2.0.3"
+00007d20: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00007d30: 2020 2020 2276 6972 7475 616c 656e 7622      "virtualenv"
+00007d40: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00007d50: 2268 6173 6865 7322 3a20 5b0a 2020 2020  "hashes": [.    
+00007d60: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00007d70: 3235 363a 3661 6265 6337 3637 3065 3538  256:6abec7670e58
+00007d80: 3032 6135 3238 3335 3766 6463 3735 6232  02a528357fdc75b2
+00007d90: 3662 3966 3537 6435 6439 3266 3239 6335  6b9f57d5d92f29c5
+00007da0: 3436 3262 6130 6662 6534 3566 6561 6363  462ba0fbe45feacc
+00007db0: 3638 3565 222c 0a20 2020 2020 2020 2020  685e",.         
+00007dc0: 2020 2020 2020 2022 7368 6132 3536 3a61         "sha256:a
+00007dd0: 3835 6361 6135 3534 6365 6430 6330 6166  85caa554ced0c0af
+00007de0: 6264 3064 3633 3865 3765 3264 3762 3566  bd0d638e7e2d7b5f
+00007df0: 3932 6432 3334 3738 6430 3564 3137 6137  92d23478d05d17a7
+00007e00: 3664 6165 6163 3866 3237 3966 3932 3422  6daeac8f279f924"
+00007e10: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+00007e20: 2020 2020 2020 2020 2020 2020 226d 6172              "mar
+00007e30: 6b65 7273 223a 2022 7079 7468 6f6e 5f76  kers": "python_v
+00007e40: 6572 7369 6f6e 203e 3d20 2733 2e37 2722  ersion >= '3.7'"
+00007e50: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+00007e60: 6572 7369 6f6e 223a 2022 3d3d 3230 2e32  ersion": "==20.2
+00007e70: 332e 3022 0a20 2020 2020 2020 207d 2c0a  3.0".        },.
+00007e80: 2020 2020 2020 2020 2277 6562 656e 636f          "webenco
+00007e90: 6469 6e67 7322 3a20 7b0a 2020 2020 2020  dings": {.      
+00007ea0: 2020 2020 2020 2268 6173 6865 7322 3a20        "hashes": 
+00007eb0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00007ec0: 2020 2273 6861 3235 363a 6130 6166 3132    "sha256:a0af12
+00007ed0: 3133 6633 6332 3232 3634 3937 6139 3765  13f3c2226497a97e
+00007ee0: 3262 3361 6130 3161 3765 3462 6565 3466  2b3aa01a7e4bee4f
+00007ef0: 3430 3366 3935 6265 3136 6663 3961 6364  403f95be16fc9acd
+00007f00: 3239 3437 3531 3461 3738 222c 0a20 2020  2947514a78",.   
+00007f10: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00007f20: 6132 3536 3a62 3336 6131 6332 3435 6632  a256:b36a1c245f2
+00007f30: 6433 3034 3936 3565 6234 6530 6138 3238  d304965eb4e0a828
+00007f40: 3438 3337 3932 3431 6463 3034 6238 3635  48379241dc04b865
+00007f50: 6166 6363 3461 6162 3136 3734 3835 3837  afcc4aab16748587
+00007f60: 6531 3932 3322 0a20 2020 2020 2020 2020  e1923".         
+00007f70: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+00007f80: 2020 2276 6572 7369 6f6e 223a 2022 3d3d    "version": "==
+00007f90: 302e 352e 3122 0a20 2020 2020 2020 207d  0.5.1".        }
+00007fa0: 2c0a 2020 2020 2020 2020 227a 6970 7022  ,.        "zipp"
+00007fb0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00007fc0: 2268 6173 6865 7322 3a20 5b0a 2020 2020  "hashes": [.    
+00007fd0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
+00007fe0: 3235 363a 3131 3239 3239 6164 3634 3964  256:112929ad649d
+00007ff0: 6139 3431 6332 3364 6535 3066 3335 3661  a941c23de50f356a
+00008000: 3262 3535 3730 6339 3534 6236 3531 3530  2b5570c954b65150
+00008010: 3634 3262 6363 6464 3636 6266 3139 3464  642bccdd66bf194d
+00008020: 3232 3462 222c 0a20 2020 2020 2020 2020  224b",.         
+00008030: 2020 2020 2020 2022 7368 6132 3536 3a34         "sha256:4
+00008040: 3839 3034 6663 3736 6136 3065 3534 3261  8904fc76a60e542a
+00008050: 6631 3531 6164 6564 3935 3732 3663 3161  f151aded95726c1a
+00008060: 3563 3334 6564 3433 6162 3431 3334 6235  5c34ed43ab4134b5
+00008070: 3937 3636 3563 3836 6437 6164 3535 3622  97665c86d7ad556"
+00008080: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+00008090: 2020 2020 2020 2020 2020 2020 226d 6172              "mar
+000080a0: 6b65 7273 223a 2022 7079 7468 6f6e 5f76  kers": "python_v
+000080b0: 6572 7369 6f6e 203e 3d20 2733 2e37 2722  ersion >= '3.7'"
+000080c0: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+000080d0: 6572 7369 6f6e 223a 2022 3d3d 332e 3135  ersion": "==3.15
+000080e0: 2e30 220a 2020 2020 2020 2020 7d0a 2020  .0".        }.  
+000080f0: 2020 7d0a 7d0a                             }.}.
```

### Comparing `archbuilder-0.1.2/README.md` & `archbuilder-0.1.3/src/archbuilder.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,54 @@
-
-# Archbuilder
-
-Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
-```bash
-  pip install archbuilder
-```
-    
-## Usage
-
-##### 1. By using a python script
-```python
-# Import archbuilder
-from builder import Builder
-from template import Template
-
-# Create a template from a json file
-template = Template('sass.json')
-
-# Create the project tree from the template
-project = Builder('sass', template)
-project.build()
-```
-
-##### 2. By using the command-line
-Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
-```bash
-archbuilder sass sass.json
-```
-
-## Contributing
-
-Contributions are always welcome!
-
-For major changes, please open an issue first
-to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-## License
-
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: archbuilder
+Version: 0.1.3
+Summary: A tool to enable developers set up their projects quickly
+Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+
+# Archbuilder
+
+Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
+```bash
+  pip install archbuilder
+```
+    
+## Usage
+
+##### 1. By using a python script
+```python
+# Import archbuilder
+from builder import Builder
+from template import Template
+
+# Create a template from a json file
+template = Template('sass.json')
+
+# Create the project tree from the template
+project = Builder('sass', template)
+project.build()
+```
+
+##### 2. By using the command-line
+Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
+```bash
+archbuilder sass sass.json
+```
+
+## Contributing
+
+Contributions are always welcome!
+
+For major changes, please open an issue first
+to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+## License
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
```

### Comparing `archbuilder-0.1.2/src/archbuilder/__main__.py` & `archbuilder-0.1.3/src/archbuilder/__main__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""
-"""
-
-import argparse
-
-from builder import Builder
-from template import Template
-
-
-def get_args():
-    parser = argparse.ArgumentParser(
-        prog="archbuilder",
-        description="Use '%(prog)s' to quickly build project structures from JSON templates",
-    )
-    parser.add_argument("project", type=str)
-    parser.add_argument("template", type=str)
-    parser.add_argument("-o", "--output", type=str, default="build")
-
-    return parser.parse_args()
-
-
-def main():
-    args = get_args()
-
-    template = Template(args.template)
-    project = Builder(args.project, template, args.output)
-    project.build()
-
-
-if __name__ == "__main__":
-    main()
+"""
+"""
+
+import argparse
+
+from builder import Builder
+from template import Template
+
+
+def get_args():
+    parser = argparse.ArgumentParser(
+        prog="archbuilder",
+        description="Use '%(prog)s' to quickly build project structures from JSON templates",
+    )
+    parser.add_argument("project", type=str)
+    parser.add_argument("template", type=str)
+    parser.add_argument("-o", "--output", type=str, default="build")
+
+    return parser.parse_args()
+
+
+def main():
+    args = get_args()
+
+    template = Template(args.template)
+    project = Builder(args.project, template, args.output)
+    project.build()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `archbuilder-0.1.2/src/archbuilder.egg-info/PKG-INFO` & `archbuilder-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-Metadata-Version: 2.1
-Name: archbuilder
-Version: 0.1.2
-Summary: A tool to enable developers set up their projects quickly
-Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-
-# Archbuilder
-
-Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
-```bash
-  pip install archbuilder
-```
-    
-## Usage
-
-##### 1. By using a python script
-```python
-# Import archbuilder
-from builder import Builder
-from template import Template
-
-# Create a template from a json file
-template = Template('sass.json')
-
-# Create the project tree from the template
-project = Builder('sass', template)
-project.build()
-```
-
-##### 2. By using the command-line
-Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
-```bash
-archbuilder sass sass.json
-```
-
-## Contributing
-
-Contributions are always welcome!
-
-For major changes, please open an issue first
-to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-## License
-
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+
+# Archbuilder
+
+Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
+```bash
+  pip install archbuilder
+```
+    
+## Usage
+
+##### 1. By using a python script
+```python
+# Import archbuilder
+from builder import Builder
+from template import Template
+
+# Create a template from a json file
+template = Template('sass.json')
+
+# Create the project tree from the template
+project = Builder('sass', template)
+project.build()
+```
+
+##### 2. By using the command-line
+Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
+```bash
+archbuilder sass sass.json
+```
+
+## Contributing
+
+Contributions are always welcome!
+
+For major changes, please open an issue first
+to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+## License
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
```

### Comparing `archbuilder-0.1.2/src/archbuilder.egg-info/SOURCES.txt` & `archbuilder-0.1.3/src/archbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archbuilder-0.1.2/src/builder/builder.py` & `archbuilder-0.1.3/src/builder/builder.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""
-"""
-
-from pathlib import Path
-
-
-class Builder:
-    """"""
-
-    def __init__(self, project, template, output="build", root=Path.cwd()):
-        """"""
-        self.project = project
-        self.template = template
-        self.output = output
-        self.root = root
-
-    def build(self):
-        """"""
-        for path in self.paths():
-            if not path.exists():
-                path.parent.mkdir(parents=True, exist_ok=True)
-                path.touch(exist_ok=True)
-
-    def paths(self):
-        """"""
-        paths = list()
-        for tail in self.template.tails():
-            path = Path(self.root / self.output / self.project / tail)
-            paths.append(path)
-        return paths
+"""
+"""
+
+from pathlib import Path
+
+
+class Builder:
+    """"""
+
+    def __init__(self, project, template, output="build", root=Path.cwd()):
+        """"""
+        self.project = project
+        self.template = template
+        self.output = output
+        self.root = root
+
+    def build(self):
+        """"""
+        for path in self.paths():
+            if not path.exists():
+                path.parent.mkdir(parents=True, exist_ok=True)
+                path.touch(exist_ok=True)
+
+    def paths(self):
+        """"""
+        paths = list()
+        for tail in self.template.tails():
+            path = Path(self.root / self.output / self.project / tail)
+            paths.append(path)
+        return paths
```

