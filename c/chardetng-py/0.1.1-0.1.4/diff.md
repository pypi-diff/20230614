# Comparing `tmp/chardetng_py-0.1.1.tar.gz` & `tmp/chardetng_py-0.1.4.tar.gz`

## Comparing `chardetng_py-0.1.1.tar` & `chardetng_py-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,34 @@
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 chardetng_py-0.1.1/Cargo.toml
--rw-rw-r--   0     1000     1000     2809 2023-04-23 03:38:01.000000 chardetng_py-0.1.1/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      685 2023-04-23 03:38:01.000000 chardetng_py-0.1.1/.gitignore
--rw-rw-r--   0     1000     1000      849 2023-04-24 19:34:57.000000 chardetng_py-0.1.1/README.md
--rw-rw-r--   0     1000     1000     2095 2023-04-24 19:15:16.000000 chardetng_py-0.1.1/bench/bench.py
--rw-rw-r--   0     1000     1000     2395 2023-04-24 19:15:08.000000 chardetng_py-0.1.1/bench/compare.py
--rw-rw-r--   0     1000     1000      510 2023-04-24 19:36:17.000000 chardetng_py-0.1.1/pyproject.toml
--rw-rw-r--   0     1000     1000      615 2023-04-24 18:09:44.000000 chardetng_py-0.1.1/src/lib.rs
--rw-rw-r--   0     1000     1000     8353 2023-04-24 19:37:10.000000 chardetng_py-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 chardetng_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 chardetng_py-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123      446 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.cookiecutter.json
+-rw-r--r--   0     1001      123       19 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.gitattributes
+-rw-r--r--   0     1001      123      461 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.github/dependabot.yml
+-rw-r--r--   0     1001      123     1799 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.github/labels.yml
+-rw-r--r--   0     1001      123      728 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.github/release-drafter.yml
+-rw-r--r--   0     1001      123     2793 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.gitignore
+-rw-r--r--   0     1001      123      936 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123      208 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/.readthedocs.yml
+-rw-r--r--   0     1001      123     5524 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123     2870 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1067 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/LICENSE
+-rw-r--r--   0     1001      123     2942 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/README.md
+-rw-r--r--   0     1001      123       40 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/codeofconduct.md
+-rw-r--r--   0     1001      123      328 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/conf.py
+-rw-r--r--   0     1001      123      111 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/contributing.md
+-rw-r--r--   0     1001      123      348 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/index.md
+-rw-r--r--   0     1001      123       69 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/license.md
+-rw-r--r--   0     1001      123      220 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/reference.md
+-rw-r--r--   0     1001      123       85 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/requirements.txt
+-rw-r--r--   0     1001      123      492 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/docs/usage.md
+-rw-r--r--   0     1001      123    97250 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/poetry.lock
+-rw-r--r--   0     1001      123     2057 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/pyproject.toml
+-rw-r--r--   0     1001      123      277 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/python/chardetng_py/__init__.py
+-rw-r--r--   0     1001      123       55 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/python/chardetng_py/_rust.pyi
+-rw-r--r--   0     1001      123     1198 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/python/chardetng_py/api.py
+-rw-r--r--   0     1001      123     1183 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/python/chardetng_py/compat.py
+-rw-r--r--   0     1001      123        0 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/python/chardetng_py/py.typed
+-rw-r--r--   0     1001      123      662 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123       47 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/tests/__init__.py
+-rw-r--r--   0     1001      123      211 2023-04-27 00:29:36.000000 chardetng_py-0.1.4/tests/test_decode.py
+-rw-r--r--   0     1001      123     8337 2023-04-27 00:30:31.000000 chardetng_py-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 chardetng_py-0.1.4/PKG-INFO
```

### Comparing `chardetng_py-0.1.1/.github/workflows/CI.yml` & `chardetng_py-0.1.4/.github/workflows/CI.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 on:
   push:
     branches:
       - main
       - master
     tags:
-      - '*'
-  pull_request:
+      - "*"
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
   linux:
@@ -24,21 +23,21 @@
     strategy:
       matrix:
         target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: "3.10"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
-          sccache: 'true'
+          sccache: "true"
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
@@ -47,22 +46,22 @@
     strategy:
       matrix:
         target: [x64, x86]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: "3.10"
           architecture: ${{ matrix.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
-          sccache: 'true'
+          sccache: "true"
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   macos:
@@ -70,21 +69,21 @@
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: "3.10"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
-          sccache: 'true'
+          sccache: "true"
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   sdist:
```

### Comparing `chardetng_py-0.1.1/.gitignore` & `chardetng_py-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `chardetng_py-0.1.1/Cargo.lock` & `chardetng_py-0.1.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,17 @@
  "cfg-if",
  "encoding_rs",
  "memchr",
 ]
 
 [[package]]
 name = "chardetng_py"
-version = "0.1.1"
+version = "0.1.4"
 dependencies = [
  "chardetng",
- "encoding_rs",
  "pyo3",
 ]
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -223,17 +222,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
```

