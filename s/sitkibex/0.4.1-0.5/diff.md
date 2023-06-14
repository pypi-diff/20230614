# Comparing `tmp/sitkibex-0.4.1.tar.gz` & `tmp/sitkibex-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sitk-ibex/sitk-ibex/dist/.tmp-wtxri0mx/sitkibex-0.4.1.tar", last modified: Thu May 11 15:40:20 2023, max compression
+gzip compressed data, was "sitkibex-0.5.tar", last modified: Wed Jun 14 20:24:14 2023, max compression
```

## Comparing `sitkibex-0.4.1.tar` & `sitkibex-0.5.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 15:39:52.000000 sitkibex-0.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-11 15:39:52.000000 sitkibex-0.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 15:39:52.000000 sitkibex-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 15:39:52.000000 sitkibex-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-11 15:39:52.000000 sitkibex-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-11 15:39:52.000000 sitkibex-0.4.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-11 15:40:20.000000 sitkibex-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-11 15:39:52.000000 sitkibex-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-11 15:39:52.000000 sitkibex-0.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 15:39:52.000000 sitkibex-0.4.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 15:39:52.000000 sitkibex-0.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-11 15:39:52.000000 sitkibex-0.4.1/docs/commandline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-11 15:39:52.000000 sitkibex-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-11 15:39:52.000000 sitkibex-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 15:39:52.000000 sitkibex-0.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-11 15:39:52.000000 sitkibex-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 15:39:52.000000 sitkibex-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 15:39:52.000000 sitkibex-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:40:20.000000 sitkibex-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-11 15:39:52.000000 sitkibex-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/image_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19352 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/registration_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/resample.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4942 2023-05-11 15:39:52.000000 sitkibex-0.4.1/sitkibex/xml_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:40:20.000000 sitkibex-0.4.1/sitkibex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)   516575 2023-05-11 15:39:52.000000 sitkibex-0.4.1/test/data/panel1.nrrd
--rw-r--r--   0 runner    (1001) docker     (123)   411960 2023-05-11 15:39:52.000000 sitkibex-0.4.1/test/data/panel2.nrrd
--rw-r--r--   0 runner    (1001) docker     (123)   655874 2023-05-11 15:39:52.000000 sitkibex-0.4.1/test/data/vpanel1.nrrd
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-11 15:39:52.000000 sitkibex-0.4.1/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-11 15:39:52.000000 sitkibex-0.4.1/test/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-11 15:39:52.000000 sitkibex-0.4.1/test/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-11 15:39:52.000000 sitkibex-0.4.1/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-11 15:39:52.000000 sitkibex-0.4.1/trufflehog3.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:40:20.000000 sitkibex-0.4.1/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2122 2023-05-11 15:39:52.000000 sitkibex-0.4.1/utils/update-gh-pages.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.850467 sitkibex-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-14 20:23:57.000000 sitkibex-0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.838467 sitkibex-0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.842467 sitkibex-0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-14 20:23:57.000000 sitkibex-0.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-14 20:23:57.000000 sitkibex-0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 20:23:57.000000 sitkibex-0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-14 20:23:57.000000 sitkibex-0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-06-14 20:23:57.000000 sitkibex-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-14 20:23:57.000000 sitkibex-0.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-14 20:24:14.850467 sitkibex-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-14 20:23:57.000000 sitkibex-0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.842467 sitkibex-0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 20:23:57.000000 sitkibex-0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.842467 sitkibex-0.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-14 20:23:57.000000 sitkibex-0.5/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 20:23:57.000000 sitkibex-0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-14 20:23:57.000000 sitkibex-0.5/docs/commandline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-14 20:23:57.000000 sitkibex-0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-14 20:23:57.000000 sitkibex-0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 20:23:57.000000 sitkibex-0.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-14 20:23:57.000000 sitkibex-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 20:23:57.000000 sitkibex-0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:24:14.850467 sitkibex-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.846467 sitkibex-0.5/sitkibex/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 20:24:14.000000 sitkibex-0.5/sitkibex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/image_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19352 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/registration_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4942 2023-06-14 20:23:57.000000 sitkibex-0.5/sitkibex/xml_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.846467 sitkibex-0.5/sitkibex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-14 20:24:14.000000 sitkibex-0.5/sitkibex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-14 20:24:14.000000 sitkibex-0.5/sitkibex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:24:14.000000 sitkibex-0.5/sitkibex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 20:24:14.000000 sitkibex-0.5/sitkibex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 20:24:14.000000 sitkibex-0.5/sitkibex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.850467 sitkibex-0.5/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.850467 sitkibex-0.5/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   516575 2023-06-14 20:23:57.000000 sitkibex-0.5/test/data/panel1.nrrd
+-rw-r--r--   0 runner    (1001) docker     (123)   411960 2023-06-14 20:23:57.000000 sitkibex-0.5/test/data/panel2.nrrd
+-rw-r--r--   0 runner    (1001) docker     (123)   655874 2023-06-14 20:23:57.000000 sitkibex-0.5/test/data/vpanel1.nrrd
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-14 20:23:57.000000 sitkibex-0.5/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-14 20:23:57.000000 sitkibex-0.5/test/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-14 20:23:57.000000 sitkibex-0.5/test/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-14 20:23:57.000000 sitkibex-0.5/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-14 20:23:57.000000 sitkibex-0.5/trufflehog3.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:24:14.850467 sitkibex-0.5/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2122 2023-06-14 20:23:57.000000 sitkibex-0.5/utils/update-gh-pages.sh
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sitkibex-0.4.1/.github/workflows/main.yml` & `sitkibex-0.5/.github/workflows/main.yml`

 * *Files 21% similar despite different names*

```diff
@@ -36,62 +36,61 @@
         trufflehog3 -v -c trufflehog3.yml . && echo "tufflehog3 OK"
 
   test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10', '3.11']
+        python-version: [3.8, 3.9, '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -r requirements.txt -r requirements-dev.txt
+        pip install -e .[zarr,dev]
     - name: Test with pytest
       run: |
         python -m pytest
 
   package_docs:
     needs: test
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - name: Set up Python 3.7
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: 3.11
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -r requirements.txt -r docs/requirements.txt twine build
+          python -m pip install -e .[zarr] twine build
       - name: Build package
         run: |
           python -m build --wheel --sdist
           python -m twine check dist/*
           ls -la dist
       - name: Upload package
         if: github.event_name == 'push'
         uses: actions/upload-artifact@v3
         with:
           name: python-packages
           path: dist
       - name: Build Sphinx Documentation
         run: |
-          # install so that setuptools_scm generate version for package
-          pip install -e .
+          pip install -r docs/requirements.txt
           make -C docs html
       - name: Upload documentation
         if: github.event_name == 'push'
         uses: actions/upload-artifact@v3
         with:
           name: sphinx-docs
           path: docs/_build/html
@@ -105,25 +104,7 @@
           ./utils/update-gh-pages.sh docs/_build/html
 
           repo_uri="https://x-access-token:${GITHUB_TOKEN}@github.com/${GITHUB_REPOSITORY}.git"
           git push $repo_uri ${TARGET_BRANCH}
         env:
           GITHUB_TOKEN: ${{ secrets.github_token }}
           TARGET_BRANCH: 'gh-pages'
-
-  github_release:
-    if: startsWith(github.ref, 'refs/tags/v')
-    needs: package_docs
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/download-artifact@v3
-        id: download
-        with:
-          name: python-packages
-      - name: Create Release and Upload
-        if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
-        id: create_release
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        run: |
-          gh release create ${{ github.ref_name }} --repo ${{ github.repository }} --verify-tag --generate-notes --title "Release ${{ github.ref_name }}"
-          gh release upload ${{ github.ref_name }} --repo ${{ github.repository }} ${{steps.download.outputs.download-path}}/*
```

### Comparing `sitkibex-0.4.1/.pre-commit-config.yaml` & `sitkibex-0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/LICENSE` & `sitkibex-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/PKG-INFO` & `sitkibex-0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: sitkibex
-Version: 0.4.1
+Version: 0.5
 Summary: Image registration for iterative fluorescence microscopy
-Home-page: https://github.com/niaid/sitk-ibex
-Author: ['Bradley Lowekamp']
-Author-email: bioinformatics@niaid.nih.gov
-License: Apache 2.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Author-email: Bradley Lowekamp <bioinformatics@niaid.nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: zarr
+Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 
 SITK-IBEX: Aligning images acquired with the IBEX microscopy imaging technique
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-This Python package was implemented as part of the development of the
+This Python package implementation is part of the development of the
 Iterative Bleaching Extends Multiplexity (IBEX) imaging technique. It enables
 the alignment of multiple cycles of fluorescence images, acquired
 using IBEX. A repeated marker is used to register all panels to a
 selected panel (in the registration nomenclature this is the fixed image).
 After registration all panels are resampled onto the fixed image.
 
+More information about the development of the IBEX technique can be found in
+the `IBEX Imaging Community`_,  which is a community of researchers who are developing
+the  IBEX knowledge-base of reagents, protocols, panels, publications, software,
+and datasets.
+
 While this method was developed for a specific imaging protocol, it will likely
 work for other sequential protocols that contain a repeated marker.
 The registration approach is implemented using the
 `SimpleITK toolkit`_ registration framework.
 
 The key implementation aspects include:
 
@@ -48,32 +51,34 @@
 
 Installation
 ------------
 
 
 The Python module is distributed on `PyPI - The Python Package Index`_. The package can be installed by running:
 
- python -m pip install sitkibex
+ python -m pip install sitkibex[zarr]
 
 Wheels from the master branch can be download wheel from `Github Actions`_ in the
 "python-package" artifact.
 
 Dependencies are conventionally specified in `setup.py` and `requirements.txt` and therefore installed as
-dependencies when the wheel is installed. This includes the SimpleITK 2.0 requirement.
+dependencies when the wheel is installed. This includes the SimpleITK 2.0 requirement. The optional "zarr" dependency
+is required for reading OME-NGFF ZARR files, and may be omitted if not needed.
 
 Data
 ----
 
 Sample data is available and described on Zenodo:
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4304786.svg
    :target: https://doi.org/10.5281/zenodo.4304786
 
 Any image and transform file format supported by `SimpleITK's IO <https://simpleitk.readthedocs.io/en/master/IO.html>`_
-can be use by sitk-ibex. The 3D `nrrd` format, and `txt` transform file extension are recommended.
+can be used by sitk-ibex. The NRRD or`NGFF <https://ngff.openmicroscopy.org/latest/>`_ image formats, and `txt` transform file
+extension are recommended.
 
 
 Example
 -------
 
 The following examples uses CD4 marker channel extracted from the "IBEX4_spleen" data set with ImageJ. The panel 2 is
 used as the reference coordinates or the "fixed image". The other panels are registered then resampled to the fixed
@@ -95,14 +100,40 @@
 Then apply the registration transform by resampling all channels of the the input images onto panel 2::
 
  python -m sitkibex resample "spleen_panel2.nrrd@CD4 AF594" spleen_panel2.nrrd tx_p2_to_p1.txt \
         -o spleen_onto_p2_panel1.nrrd
  python -m sitkibex resample "spleen_panel2.nrrd@CD4 AF594" spleen_panel3.nrrd tx_p2_to_p3.txt \
         -o spleen_onto_p2_panel3.nrrd
 
+Additional Example
+------------------
+
+Additional sample data:
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4632320.svg
+   :target: https://doi.org/10.5281/zenodo.4632320
+
+The sample Imaris files can be converted to OME-NGFF ZARR with
+`bioformats2raw <https://github.com/glencoesoftware/bioformats2raw/releases>`_. The ims files contains one series, and
+for simplicity, the structure is generated without a series index in the hierarchy with the following commands::
+
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel1.ims Human_Spleen_Panel1.zarr
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel2.ims Human_Spleen_Panel2.zarr
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel2.ims Human_Spleen_Panel3.zarr
+
+These images will be registered based on the common "Hoechst". The name of the channels are lost in this conversion from
+Imaris to OME-NGFF ZARR. Some conversions produce "omera" metadata in the ZARR file which contains channel labels, which
+can be used. When the channel labels are unavailable, the channel index can be used such as the following commands::
+
+ python -m sitkibex registration --affine "Human_Spleen_Panel2.zarr@3" "Human_Spleen_Panel1.zarr@2" tx_p2_to_p1.txt
+ python -m sitkibex registration --affine "Human_Spleen_Panel2.zarr@3" "Human_Spleen_Panel3.zarr@4" tx_p2_to_p3.txt
+
+The quick 2D visualization can be run similarly to the NRRD example. The OME-NGFF ZARR files are not supported for
+writing, so the resample command can produce NRRD files as well.
+
 
 How to Cite
 -----------
 
 If you use the SITK-IBEX package in your work, please cite us:
 
  A. J. Radtke, E. F. Kandov, B. C. Lowekamp, E. Speranza, C. Chu,
@@ -136,7 +167,8 @@
 .. _Github Actions: https://github.com/niaid/sitk-ibex/actions?query=branch%3Amaster
 .. _NRRD: http://teem.sourceforge.net/nrrd/format.html
 .. _GitHub Issues:  https://github.com/niaid/sitk-ibex
 .. _wheel: https://www.python.org/dev/peps/pep-0427/
 .. _`PyPI - The Python Package Index`: https://pypi.org/project/sitkibex/
 .. _Github Releases: https://github.com/niaid/sitk-ibex/releases
 .. _10.1073/pnas.2018488117: https://www.pnas.org/doi/10.1073/pnas.2018488117
+.. _`IBEX Imaging Community`: https://ibeximagingcommunity.github.io/ibex_imaging_knowledge_base/data_and_software.html
```

### Comparing `sitkibex-0.4.1/README.rst` & `sitkibex-0.5/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 
 SITK-IBEX: Aligning images acquired with the IBEX microscopy imaging technique
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-This Python package was implemented as part of the development of the
+This Python package implementation is part of the development of the
 Iterative Bleaching Extends Multiplexity (IBEX) imaging technique. It enables
 the alignment of multiple cycles of fluorescence images, acquired
 using IBEX. A repeated marker is used to register all panels to a
 selected panel (in the registration nomenclature this is the fixed image).
 After registration all panels are resampled onto the fixed image.
 
+More information about the development of the IBEX technique can be found in
+the `IBEX Imaging Community`_,  which is a community of researchers who are developing
+the  IBEX knowledge-base of reagents, protocols, panels, publications, software,
+and datasets.
+
 While this method was developed for a specific imaging protocol, it will likely
 work for other sequential protocols that contain a repeated marker.
 The registration approach is implemented using the
 `SimpleITK toolkit`_ registration framework.
 
 The key implementation aspects include:
 
@@ -31,32 +36,34 @@
 
 Installation
 ------------
 
 
 The Python module is distributed on `PyPI - The Python Package Index`_. The package can be installed by running:
 
- python -m pip install sitkibex
+ python -m pip install sitkibex[zarr]
 
 Wheels from the master branch can be download wheel from `Github Actions`_ in the
 "python-package" artifact.
 
 Dependencies are conventionally specified in `setup.py` and `requirements.txt` and therefore installed as
-dependencies when the wheel is installed. This includes the SimpleITK 2.0 requirement.
+dependencies when the wheel is installed. This includes the SimpleITK 2.0 requirement. The optional "zarr" dependency
+is required for reading OME-NGFF ZARR files, and may be omitted if not needed.
 
 Data
 ----
 
 Sample data is available and described on Zenodo:
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4304786.svg
    :target: https://doi.org/10.5281/zenodo.4304786
 
 Any image and transform file format supported by `SimpleITK's IO <https://simpleitk.readthedocs.io/en/master/IO.html>`_
-can be use by sitk-ibex. The 3D `nrrd` format, and `txt` transform file extension are recommended.
+can be used by sitk-ibex. The NRRD or`NGFF <https://ngff.openmicroscopy.org/latest/>`_ image formats, and `txt` transform file
+extension are recommended.
 
 
 Example
 -------
 
 The following examples uses CD4 marker channel extracted from the "IBEX4_spleen" data set with ImageJ. The panel 2 is
 used as the reference coordinates or the "fixed image". The other panels are registered then resampled to the fixed
@@ -78,14 +85,40 @@
 Then apply the registration transform by resampling all channels of the the input images onto panel 2::
 
  python -m sitkibex resample "spleen_panel2.nrrd@CD4 AF594" spleen_panel2.nrrd tx_p2_to_p1.txt \
         -o spleen_onto_p2_panel1.nrrd
  python -m sitkibex resample "spleen_panel2.nrrd@CD4 AF594" spleen_panel3.nrrd tx_p2_to_p3.txt \
         -o spleen_onto_p2_panel3.nrrd
 
+Additional Example
+------------------
+
+Additional sample data:
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4632320.svg
+   :target: https://doi.org/10.5281/zenodo.4632320
+
+The sample Imaris files can be converted to OME-NGFF ZARR with
+`bioformats2raw <https://github.com/glencoesoftware/bioformats2raw/releases>`_. The ims files contains one series, and
+for simplicity, the structure is generated without a series index in the hierarchy with the following commands::
+
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel1.ims Human_Spleen_Panel1.zarr
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel2.ims Human_Spleen_Panel2.zarr
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel2.ims Human_Spleen_Panel3.zarr
+
+These images will be registered based on the common "Hoechst". The name of the channels are lost in this conversion from
+Imaris to OME-NGFF ZARR. Some conversions produce "omera" metadata in the ZARR file which contains channel labels, which
+can be used. When the channel labels are unavailable, the channel index can be used such as the following commands::
+
+ python -m sitkibex registration --affine "Human_Spleen_Panel2.zarr@3" "Human_Spleen_Panel1.zarr@2" tx_p2_to_p1.txt
+ python -m sitkibex registration --affine "Human_Spleen_Panel2.zarr@3" "Human_Spleen_Panel3.zarr@4" tx_p2_to_p3.txt
+
+The quick 2D visualization can be run similarly to the NRRD example. The OME-NGFF ZARR files are not supported for
+writing, so the resample command can produce NRRD files as well.
+
 
 How to Cite
 -----------
 
 If you use the SITK-IBEX package in your work, please cite us:
 
  A. J. Radtke, E. F. Kandov, B. C. Lowekamp, E. Speranza, C. Chu,
@@ -119,7 +152,8 @@
 .. _Github Actions: https://github.com/niaid/sitk-ibex/actions?query=branch%3Amaster
 .. _NRRD: http://teem.sourceforge.net/nrrd/format.html
 .. _GitHub Issues:  https://github.com/niaid/sitk-ibex
 .. _wheel: https://www.python.org/dev/peps/pep-0427/
 .. _`PyPI - The Python Package Index`: https://pypi.org/project/sitkibex/
 .. _Github Releases: https://github.com/niaid/sitk-ibex/releases
 .. _10.1073/pnas.2018488117: https://www.pnas.org/doi/10.1073/pnas.2018488117
+.. _`IBEX Imaging Community`: https://ibeximagingcommunity.github.io/ibex_imaging_knowledge_base/data_and_software.html
```

### Comparing `sitkibex-0.4.1/docs/Makefile` & `sitkibex-0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/docs/commandline.rst` & `sitkibex-0.5/docs/commandline.rst`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/docs/conf.py` & `sitkibex-0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/docs/index.rst` & `sitkibex-0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex/__main__.py` & `sitkibex-0.5/sitkibex/__main__.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex/cli.py` & `sitkibex-0.5/sitkibex/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,16 @@
 @click.option(
     "--random/--no-random",
     default=False,
     show_default=True,
     help="Use wall-clock instead of a fixed seed for random initialization.",
 )
 @click.option("--samples-per-parameter", default=5000, type=int, show_default=True)
-@click.argument("fixed_image", type=ImagePathChannel(exists=True, dir_okay=False, resolve_path=True))
-@click.argument("moving_image", type=ImagePathChannel(exists=True, dir_okay=False, resolve_path=True))
+@click.argument("fixed_image", type=ImagePathChannel(exists=True, dir_okay=True, resolve_path=True))
+@click.argument("moving_image", type=ImagePathChannel(exists=True, dir_okay=True, resolve_path=True))
 @click.argument("output_transform", type=click.Path(exists=False, resolve_path=True))
 def reg_cli(fixed_image, moving_image, output_transform, **kwargs):
     """Perform registration to solve for an OUTPUT_TRANSFORM mapping points from the FIXED_IMAGE to the MOVING_IMAGE."""
     from sitkibex.registration import registration
 
     args = _Bunch(kwargs)
 
@@ -214,16 +214,16 @@
 @click.option(
     "-o",
     "--output",
     default=None,
     help="filename for output image, if not provided the SimpleITK Show method is called",
     type=click.Path(exists=False, resolve_path=True),
 )
-@click.argument("fixed_image", type=ImagePathChannel(exists=True, dir_okay=False, resolve_path=True))
-@click.argument("moving_image", type=ImagePathChannel(exists=True, dir_okay=False, resolve_path=True))
+@click.argument("fixed_image", type=ImagePathChannel(exists=True, dir_okay=True, resolve_path=True))
+@click.argument("moving_image", type=ImagePathChannel(exists=True, dir_okay=True, resolve_path=True))
 @click.argument("transform", required=False, type=click.Path(exists=True, dir_okay=False, resolve_path=True))
 def resample_cli(fixed_image, moving_image, transform, **kwargs):
     """Create new image by transforming the MOVING_IMAGE onto the FIXED_IMAGE.
 
     Apply the TRANSFORM results from registration to resample the MOVING_IMAGE onto the coordinate space defined by the
     MOVING_IMAGE.
 
@@ -251,15 +251,15 @@
             return image
 
     moving_image, moving_channel_name = moving_image
     fixed_image, fixed_channel_name = fixed_image
 
     moving_img = binner(im_read_channel(moving_image, moving_channel_name))
 
-    if fixed_channel_name is None:
+    if fixed_channel_name is None and os.path.isfile(fixed_image):
         reader = sitk.ImageFileReader()
         reader.SetFileName(fixed_image)
         reader.ReadImageInformation()
         if reader.GetDimension() > 3:
             if args.fusion:
                 _logger.warning("Automatically selecting first channel with fusion enabled.")
             fixed_channel_name = 0
```

### Comparing `sitkibex-0.4.1/sitkibex/globals.py` & `sitkibex-0.5/sitkibex/globals.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex/image_utilities.py` & `sitkibex-0.5/sitkibex/image_utilities.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex/io.py` & `sitkibex-0.5/sitkibex/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 #  limitations under the License.
 
 import SimpleITK as sitk
 
 import os.path
 import logging
 from .xml_info import XMLInfo, OMEInfo
+from pathlib import Path
+import numpy as np
+
+try:
+    import zarr
+
+    _has_zarr = True
+except ImportError:
+    _has_zarr = False
+
 
 _logger = logging.getLogger(__name__)
 
 _vector_to_scalar = {
     sitk.sitkVectorUInt8: sitk.sitkUInt8,
     sitk.sitkVectorInt8: sitk.sitkInt8,
     sitk.sitkVectorUInt16: sitk.sitkUInt16,
@@ -29,14 +39,66 @@
     sitk.sitkVectorUInt32: sitk.sitkUInt32,
     sitk.sitkVectorInt32: sitk.sitkInt32,
     sitk.sitkVectorFloat32: sitk.sitkFloat32,
     sitk.sitkVectorFloat64: sitk.sitkFloat64,
 }
 
 
+def _zarr_read_channel(filename: Path, channel=None) -> sitk.Image:
+    """
+    Read a channel from a zarr file.
+    """
+
+    store = zarr.DirectoryStore(filename)
+    zarr_group = zarr.open_group(store=store, mode="r")
+
+    axes = zarr_group.attrs["multiscales"][0]["axes"]
+    ds_attr = zarr_group.attrs["multiscales"][0]["datasets"][0]
+
+    arr = zarr_group[ds_attr["path"]]
+    _logger.debug(arr)
+
+    spacing = ds_attr["coordinateTransformations"][0]["scale"]
+
+    axes_names = [ax["name"].upper() for ax in axes]
+
+    if axes_names != list("TCZYX"):
+        raise ValueError(f"Only TCZYX axes are supported, not {axes_names}.")
+
+    if arr.shape[0] > 1:
+        raise ValueError("Only single time point is supported.")
+
+    if channel is None:
+        arr = np.moveaxis(arr[0, ...], 0, -1)
+        img = sitk.GetImageFromArray(arr.astype(arr.dtype.newbyteorder("=")), isVector=True)
+    else:
+
+        if isinstance(channel, int):
+            channel_number = channel
+        else:
+            if "omero" not in zarr_group.attrs or "channels" not in zarr_group.attrs["omero"]:
+                raise ValueError("No OMERO metadata. Only integer channel numbers are supported.")
+            omero_channel_labels = [c["label"] for c in zarr_group.attrs["omero"]["channels"]]
+
+            if channel not in omero_channel_labels:
+                raise Exception(f'Channel name "{channel}" is not in OMERO marker list: {omero_channel_labels}.')
+
+            channel_number = omero_channel_labels.index(channel)
+
+        if channel_number >= arr.shape[1] or channel_number < 0:
+            raise ValueError("Channel number is out of range.")
+
+        arr = arr[0, channel_number, ...]
+        img = sitk.GetImageFromArray(arr.astype(arr.dtype.newbyteorder("=")), isVector=False)
+
+    img.SetSpacing(spacing[2:])
+
+    return img
+
+
 def im_read_channel(filename, channel=None):  # noqa: C901
     """
     Read a channel from an image file.
 
     SimpleITK is used to read a channel from the file. Channel names can be used if the image file contains meta-data
     which can be parsed and provides names for the channels. Otherwise channel index should be used.
 
@@ -44,16 +106,23 @@
     :param channel: An integer for the channel index or string for the name of the channel. If None then all channel are
     read.
 
     :return: A SimpleITK Image.
 
     """
 
+    filename = Path(filename)
+    if filename.is_dir() and (filename / ".zattrs").exists():
+        if _has_zarr:
+            return _zarr_read_channel(filename, channel)
+        else:
+            raise ImportError("zarr is not installed.")
+
     reader = sitk.ImageFileReader()
-    reader.SetFileName(filename)
+    reader.SetFileName(str(filename))
 
     if channel is None:
         _logger.info('Reading whole "{}" image file.'.format(filename))
         return reader.Execute()
 
     ext = os.path.splitext(filename)[1].lower()
     if ext in [".tif", ".tiff"]:
@@ -65,15 +134,14 @@
 
     _logger.debug(reader)
 
     if isinstance(channel, int):
         channel_number = channel
 
     else:
-
         IMAGE_DESCRIPTION = "ImageDescription"
         IMARIS_CHANNEL_INFORMATION = "imaris_channels_information"
 
         if IMAGE_DESCRIPTION in reader.GetMetaDataKeys():
             _logger.info('Found "{}" metadata field in {}.'.format(IMAGE_DESCRIPTION, filename))
 
             image_description = reader.GetMetaData(IMAGE_DESCRIPTION)
```

### Comparing `sitkibex-0.4.1/sitkibex/registration.py` & `sitkibex-0.5/sitkibex/registration.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex/registration_utilities.py` & `sitkibex-0.5/sitkibex/registration_utilities.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex/resample.py` & `sitkibex-0.5/sitkibex/resample.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex/xml_info.py` & `sitkibex-0.5/sitkibex/xml_info.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/sitkibex.egg-info/PKG-INFO` & `sitkibex-0.5/sitkibex.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: sitkibex
-Version: 0.4.1
+Version: 0.5
 Summary: Image registration for iterative fluorescence microscopy
-Home-page: https://github.com/niaid/sitk-ibex
-Author: ['Bradley Lowekamp']
-Author-email: bioinformatics@niaid.nih.gov
-License: Apache 2.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Author-email: Bradley Lowekamp <bioinformatics@niaid.nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: zarr
+Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 
 SITK-IBEX: Aligning images acquired with the IBEX microscopy imaging technique
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-This Python package was implemented as part of the development of the
+This Python package implementation is part of the development of the
 Iterative Bleaching Extends Multiplexity (IBEX) imaging technique. It enables
 the alignment of multiple cycles of fluorescence images, acquired
 using IBEX. A repeated marker is used to register all panels to a
 selected panel (in the registration nomenclature this is the fixed image).
 After registration all panels are resampled onto the fixed image.
 
+More information about the development of the IBEX technique can be found in
+the `IBEX Imaging Community`_,  which is a community of researchers who are developing
+the  IBEX knowledge-base of reagents, protocols, panels, publications, software,
+and datasets.
+
 While this method was developed for a specific imaging protocol, it will likely
 work for other sequential protocols that contain a repeated marker.
 The registration approach is implemented using the
 `SimpleITK toolkit`_ registration framework.
 
 The key implementation aspects include:
 
@@ -48,32 +51,34 @@
 
 Installation
 ------------
 
 
 The Python module is distributed on `PyPI - The Python Package Index`_. The package can be installed by running:
 
- python -m pip install sitkibex
+ python -m pip install sitkibex[zarr]
 
 Wheels from the master branch can be download wheel from `Github Actions`_ in the
 "python-package" artifact.
 
 Dependencies are conventionally specified in `setup.py` and `requirements.txt` and therefore installed as
-dependencies when the wheel is installed. This includes the SimpleITK 2.0 requirement.
+dependencies when the wheel is installed. This includes the SimpleITK 2.0 requirement. The optional "zarr" dependency
+is required for reading OME-NGFF ZARR files, and may be omitted if not needed.
 
 Data
 ----
 
 Sample data is available and described on Zenodo:
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4304786.svg
    :target: https://doi.org/10.5281/zenodo.4304786
 
 Any image and transform file format supported by `SimpleITK's IO <https://simpleitk.readthedocs.io/en/master/IO.html>`_
-can be use by sitk-ibex. The 3D `nrrd` format, and `txt` transform file extension are recommended.
+can be used by sitk-ibex. The NRRD or`NGFF <https://ngff.openmicroscopy.org/latest/>`_ image formats, and `txt` transform file
+extension are recommended.
 
 
 Example
 -------
 
 The following examples uses CD4 marker channel extracted from the "IBEX4_spleen" data set with ImageJ. The panel 2 is
 used as the reference coordinates or the "fixed image". The other panels are registered then resampled to the fixed
@@ -95,14 +100,40 @@
 Then apply the registration transform by resampling all channels of the the input images onto panel 2::
 
  python -m sitkibex resample "spleen_panel2.nrrd@CD4 AF594" spleen_panel2.nrrd tx_p2_to_p1.txt \
         -o spleen_onto_p2_panel1.nrrd
  python -m sitkibex resample "spleen_panel2.nrrd@CD4 AF594" spleen_panel3.nrrd tx_p2_to_p3.txt \
         -o spleen_onto_p2_panel3.nrrd
 
+Additional Example
+------------------
+
+Additional sample data:
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4632320.svg
+   :target: https://doi.org/10.5281/zenodo.4632320
+
+The sample Imaris files can be converted to OME-NGFF ZARR with
+`bioformats2raw <https://github.com/glencoesoftware/bioformats2raw/releases>`_. The ims files contains one series, and
+for simplicity, the structure is generated without a series index in the hierarchy with the following commands::
+
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel1.ims Human_Spleen_Panel1.zarr
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel2.ims Human_Spleen_Panel2.zarr
+ bioformats2raw  --series 0 --scale-format-string '%2$d/'  Human_Spleen_Panel2.ims Human_Spleen_Panel3.zarr
+
+These images will be registered based on the common "Hoechst". The name of the channels are lost in this conversion from
+Imaris to OME-NGFF ZARR. Some conversions produce "omera" metadata in the ZARR file which contains channel labels, which
+can be used. When the channel labels are unavailable, the channel index can be used such as the following commands::
+
+ python -m sitkibex registration --affine "Human_Spleen_Panel2.zarr@3" "Human_Spleen_Panel1.zarr@2" tx_p2_to_p1.txt
+ python -m sitkibex registration --affine "Human_Spleen_Panel2.zarr@3" "Human_Spleen_Panel3.zarr@4" tx_p2_to_p3.txt
+
+The quick 2D visualization can be run similarly to the NRRD example. The OME-NGFF ZARR files are not supported for
+writing, so the resample command can produce NRRD files as well.
+
 
 How to Cite
 -----------
 
 If you use the SITK-IBEX package in your work, please cite us:
 
  A. J. Radtke, E. F. Kandov, B. C. Lowekamp, E. Speranza, C. Chu,
@@ -136,7 +167,8 @@
 .. _Github Actions: https://github.com/niaid/sitk-ibex/actions?query=branch%3Amaster
 .. _NRRD: http://teem.sourceforge.net/nrrd/format.html
 .. _GitHub Issues:  https://github.com/niaid/sitk-ibex
 .. _wheel: https://www.python.org/dev/peps/pep-0427/
 .. _`PyPI - The Python Package Index`: https://pypi.org/project/sitkibex/
 .. _Github Releases: https://github.com/niaid/sitk-ibex/releases
 .. _10.1073/pnas.2018488117: https://www.pnas.org/doi/10.1073/pnas.2018488117
+.. _`IBEX Imaging Community`: https://ibeximagingcommunity.github.io/ibex_imaging_knowledge_base/data_and_software.html
```

### Comparing `sitkibex-0.4.1/sitkibex.egg-info/SOURCES.txt` & `sitkibex-0.5/sitkibex.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 NOTICE
 README.rst
 pyproject.toml
-requirements-dev.txt
 requirements.txt
-setup.py
 trufflehog3.yml
 .github/workflows/main.yml
+.github/workflows/publish.yml
 docs/Makefile
 docs/api.rst
 docs/commandline.rst
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/_templates/layout.html
 sitkibex/__init__.py
 sitkibex/__main__.py
+sitkibex/_version.py
 sitkibex/cli.py
 sitkibex/globals.py
 sitkibex/image_utilities.py
 sitkibex/io.py
 sitkibex/registration.py
 sitkibex/registration_utilities.py
 sitkibex/resample.py
 sitkibex/xml_info.py
 sitkibex.egg-info/PKG-INFO
 sitkibex.egg-info/SOURCES.txt
 sitkibex.egg-info/dependency_links.txt
-sitkibex.egg-info/entry_points.txt
 sitkibex.egg-info/requires.txt
 sitkibex.egg-info/top_level.txt
 test/test_cli.py
 test/test_registration.py
 test/test_resample.py
 test/test_utils.py
 test/data/panel1.nrrd
```

### Comparing `sitkibex-0.4.1/test/data/panel1.nrrd` & `sitkibex-0.5/test/data/panel1.nrrd`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/test/data/panel2.nrrd` & `sitkibex-0.5/test/data/panel2.nrrd`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/test/data/vpanel1.nrrd` & `sitkibex-0.5/test/data/vpanel1.nrrd`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/test/test_cli.py` & `sitkibex-0.5/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/test/test_registration.py` & `sitkibex-0.5/test/test_registration.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/test/test_resample.py` & `sitkibex-0.5/test/test_resample.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/test/test_utils.py` & `sitkibex-0.5/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `sitkibex-0.4.1/utils/update-gh-pages.sh` & `sitkibex-0.5/utils/update-gh-pages.sh`

 * *Files identical despite different names*

