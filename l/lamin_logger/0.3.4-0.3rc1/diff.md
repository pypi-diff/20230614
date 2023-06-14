# Comparing `tmp/lamin_logger-0.3.4.tar.gz` & `tmp/lamin_logger-0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.3rc1.tar", last modified: Wed Feb 22 20:28:20 2023, max compression
```

## Comparing `lamin_logger-0.3.4.tar` & `lamin_logger-0.3rc1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     2368 2023-06-14 17:38:57.246115 lamin_logger-0.3.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.3.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.3.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.3.4/.gitignore
--rw-r--r--   0        0        0     1753 2022-07-20 10:00:56.098007 lamin_logger-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.3.4/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.3.4/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.3.4/docs/api.md
--rw-r--r--   0        0        0     2644 2023-06-14 17:39:30.761012 lamin_logger-0.3.4/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.3.4/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.3.4/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.3.4/lamin-project.yaml
--rw-r--r--   0        0        0      271 2023-06-14 17:39:43.738092 lamin_logger-0.3.4/lamin_logger/__init__.py
--rw-r--r--   0        0        0     2029 2023-05-27 07:28:04.621343 lamin_logger-0.3.4/lamin_logger/_core.py
--rw-r--r--   0        0        0     3662 2023-06-14 17:38:57.246704 lamin_logger-0.3.4/lamin_logger/_lookup.py
--rw-r--r--   0        0        0      681 2023-01-12 04:19:23.176122 lamin_logger-0.3.4/lamin_logger/_python_version.py
--rw-r--r--   0        0        0      323 2023-06-14 17:38:57.247489 lamin_logger-0.3.4/noxfile.py
--rw-r--r--   0        0        0      939 2023-06-14 17:38:57.247643 lamin_logger-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      100 2022-07-20 12:55:43.891932 lamin_logger-0.3.4/tests/test_base.py
--rw-r--r--   0        0        0     1356 2023-06-14 17:38:57.247766 lamin_logger-0.3.4/tests/test_lookup.py
--rw-r--r--   0        0        0      425 2023-06-14 17:38:57.248534 lamin_logger-0.3.4/tests/test_notebooks.py
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 lamin_logger-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     2596 2023-01-12 15:58:49.394646 lamin_logger-0.3rc1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 18:46:24.119961 lamin_logger-0.3rc1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 18:46:24.120069 lamin_logger-0.3rc1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 18:46:24.120174 lamin_logger-0.3rc1/.gitignore
+-rw-r--r--   0        0        0     1753 2022-07-20 18:46:24.120276 lamin_logger-0.3rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-08-08 17:06:33.128130 lamin_logger-0.3rc1/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-20 18:49:33.932419 lamin_logger-0.3rc1/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 18:46:24.120507 lamin_logger-0.3rc1/docs/api.md
+-rw-r--r--   0        0        0     2167 2023-02-22 20:28:00.338633 lamin_logger-0.3rc1/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-23 18:45:50.337637 lamin_logger-0.3rc1/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-08-10 12:38:04.951676 lamin_logger-0.3rc1/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 18:46:24.121862 lamin_logger-0.3rc1/lamin-project.yaml
+-rw-r--r--   0        0        0      314 2023-02-22 20:27:51.255732 lamin_logger-0.3rc1/lamin_logger/__init__.py
+-rw-r--r--   0        0        0      709 2023-02-22 20:26:51.831977 lamin_logger-0.3rc1/lamin_logger/_configure_external.py
+-rw-r--r--   0        0        0     1735 2023-01-24 17:23:21.992935 lamin_logger-0.3rc1/lamin_logger/_core.py
+-rw-r--r--   0        0        0      681 2023-01-12 15:58:49.395447 lamin_logger-0.3rc1/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0      731 2023-01-12 15:58:49.395601 lamin_logger-0.3rc1/noxfile.py
+-rw-r--r--   0        0        0      921 2023-01-12 15:58:49.396381 lamin_logger-0.3rc1/pyproject.toml
+-rw-r--r--   0        0        0      100 2022-07-20 18:46:24.122416 lamin_logger-0.3rc1/tests/test_base.py
+-rw-r--r--   0        0        0      505 2022-07-23 18:45:50.338656 lamin_logger-0.3rc1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 lamin_logger-0.3rc1/PKG-INFO
```

### Comparing `lamin_logger-0.3.4/.github/workflows/build.yml` & `lamin_logger-0.3rc1/.github/workflows/build.yml`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.9"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: Checkout main
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Checkout lndocs
@@ -26,27 +26,34 @@
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
       - name: Setup Python
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Cache pre-commit
+      - name: Cache
         uses: actions/cache@v3
         env:
           cache-name: cache-all
         with:
-          path: ~/.cache/pre-commit
+          path: |
+            .nox
+            ~/.cache/pre-commit
           key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
       - name: Install pip and nox
         run: |
           python -m pip install --upgrade pip
-          pip install laminci
-      - run: nox -s lint
-      - run: nox -s build
+          pip install nox
+      - name: Lint
+        if: matrix.python-version == '3.9'
+        run: |
+          nox -s lint --python ${{ matrix.python-version }}
+      - name: Build
+        run: |
+          nox -s build --python ${{ matrix.python-version }}
       - name: Codecov
         if: matrix.python-version == '3.9'
         uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
       - name: Read lamin-project.yaml
         if: matrix.python-version == '3.9'
```

### Comparing `lamin_logger-0.3.4/.github/workflows/latest-changes.yml` & `lamin_logger-0.3rc1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.3.4/.gitignore` & `lamin_logger-0.3rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.3.4/.pre-commit-config.yaml` & `lamin_logger-0.3rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.3.4/LICENSE` & `lamin_logger-0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.3.4/docs/changelog.md` & `lamin_logger-0.3rc1/docs/changelog.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🚚 Temporarily added lookup | [20](https://github.com/laminlabs/lamin-logger/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.3.4
-✨ Added download level, changed info icon to 💬 | [19](https://github.com/laminlabs/lamin-logger/pull/19) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-27 | 0.3.2
-:sparkles: Add hint level | [17](https://github.com/laminlabs/lamin-logger/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-05 | 0.3.0
 🚸 Add all botocore subloggers | [16](https://github.com/laminlabs/lamin-logger/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-02-22 | 0.3rc1
 🔇 Suppress "Found credentials..." logging in aiobotocore | [15](https://github.com/laminlabs/lamin-logger/pull/15) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-06 | 0.2.4
 🚸 Set default level to INFO | [14](https://github.com/laminlabs/lamin-logger/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-01-24 | 0.2.3
 🔥 Manually provide versions for py_version_warning | [13](https://github.com/laminlabs/lamin-logger/pull/13) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-12 | 0.2.2
 👷 Added python version warning and extened CI to py3.7-3.11 | [12](https://github.com/laminlabs/lamin-logger/pull/12) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-11 | 0.2.0
 ⏪ Revert the previous PR | [11](https://github.com/laminlabs/lamin-logger/pull/11) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-20 | 0.1.5
 🩹 Suppress numexpr warnings | [10](https://github.com/laminlabs/lamin-logger/pull/10) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-20 | 0.1.4
```

### Comparing `lamin_logger-0.3.4/docs/quickstart.ipynb` & `lamin_logger-0.3rc1/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.3.4/lamin_logger/_core.py` & `lamin_logger-0.3rc1/lamin_logger/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,28 @@
 import platform
 import sys
 
 from loguru import logger
 
 if platform.system() == "Windows":
-    format = "{message}"
+    format = "{level.name} {message}"
 else:
     format = "{level.icon} {message}"
 
 default_handler = dict(
     sink=sys.stdout,
     format=format,
-    level=15,
+    level="INFO",
 )
 
 logger.configure(handlers=[default_handler])
 logger.level("SUCCESS", icon="✅")
-logger.level("HINT", icon="💡", no=15)
-logger.level("DOWNLOAD", icon="💾", color="<blue>", no=16)
-logger.level("INFO", icon="💬")
 logger.level("WARNING", icon="🔶")
 
 
-def hint(message):
-    return logger.log("HINT", message)
-
-
-def download(message):
-    return logger.log("DOWNLOAD", message)
-
-
-logger.hint = hint
-logger.download = download
-
 # ANSI color code: https://gist.github.com/iansan5653/c4a0b9f5c30d74258c5f132084b78db9
 ANSI_COLORS = dict(
     bold="\x1b[1m",
     black="\x1b[1;90m",
     red="\x1b[1;91m",
     green="\x1b[1;92m",
     yellow="\x1b[1;93m",
```

### Comparing `lamin_logger-0.3.4/lamin_logger/_python_version.py` & `lamin_logger-0.3rc1/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.3.4/pyproject.toml` & `lamin_logger-0.3rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,28 +12,29 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
+    "nbproject",
     "loguru",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lamin-logger"
 
 [project.optional-dependencies]
 dev = [
-    "pandas",  # lookup
     "pre-commit",
     "nox",
+]
+test = [
     "pytest>=6.0",
     "pytest-cov",
-    "nbproject_test",
 ]
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
```

### Comparing `lamin_logger-0.3.4/PKG-INFO` & `lamin_logger-0.3rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.3.4
+Version: 0.3rc1
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nbproject
 Requires-Dist: loguru
-Requires-Dist: pandas ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
-Requires-Dist: pytest>=6.0 ; extra == "dev"
-Requires-Dist: pytest-cov ; extra == "dev"
-Requires-Dist: nbproject_test ; extra == "dev"
+Requires-Dist: pytest>=6.0 ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lamin-logger
 Provides-Extra: dev
+Provides-Extra: test
 
 [![pypi](https://img.shields.io/pypi/v/lamin-logger?color=%2334D058&label=pypi%20package)](https://pypi.org/project/lamin-logger)
 
 # Lamin Logger: Logging setup
 
 This package is in private beta at this moment!
```

