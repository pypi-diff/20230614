# Comparing `tmp/opening_hours_py-0.6.4.tar.gz` & `tmp/opening_hours_py-0.6.5.tar.gz`

## Comparing `opening_hours_py-0.6.4.tar` & `opening_hours_py-0.6.5.tar`

### file list

```diff
@@ -1,12 +1,68 @@
--rw-r--r--   0     1001      121       40 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/.gitignore
--rw-r--r--   0     1001      121      778 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/Cargo.toml
--rw-r--r--   0     1001      121    10847 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/LICENSE-APACHE
--rw-r--r--   0     1001      121     1056 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/LICENSE-MIT
--rw-r--r--   0     1001      121     1718 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/README.md
--rw-r--r--   0     1001      121     9935 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/poetry.lock
--rw-r--r--   0     1001      121      368 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/pyproject.toml
--rwxr-xr-x   0     1001      121      490 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/run_doctests.py
--rw-r--r--   0     1001      121      692 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/src/errors.rs
--rw-r--r--   0     1001      121     6458 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/src/lib.rs
--rw-r--r--   0     1001      121     4643 2022-08-12 13:32:29.000000 opening_hours_py-0.6.4/src/types.rs
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 opening_hours_py-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/Cargo.toml
+-rw-r--r--   0     1001      123       86 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/.github/codecov.yml
+-rw-r--r--   0     1001      123     2693 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      123     2326 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/.github/workflows/tests.yml
+-rw-r--r--   0     1001      123       49 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/.gitignore
+-rw-r--r--   0     1001      123       22 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/.rustfmt.toml
+-rw-r--r--   0     1001      123    29444 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/Cargo.lock
+-rw-r--r--   0     1001      123    10847 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/LICENSE-MIT
+-rw-r--r--   0     1001      123     2800 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/README.md
+-rw-r--r--   0     1001      123     1996 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/benches/benchmarks.rs
+-rw-r--r--   0     1001      123     2159 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/build.rs
+-rw-r--r--   0     1001      123  4623476 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/data/holidays.txt
+-rwxr-xr-x   0     1001      123     3275 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/scripts/check-version.py
+-rwxr-xr-x   0     1001      123     1092 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/scripts/generate-holidays.py
+-rw-r--r--   0     1001      123    12169 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/scripts/poetry.lock
+-rw-r--r--   0     1001      123      428 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/scripts/pyproject.toml
+-rw-r--r--   0     1001      123     1370 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/bin/schedule.rs
+-rw-r--r--   0     1001      123    12893 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/date_filter.rs
+-rw-r--r--   0     1001      123      400 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/lib.rs
+-rw-r--r--   0     1001      123    11396 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/opening_hours.rs
+-rw-r--r--   0     1001      123     6628 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/schedule.rs
+-rw-r--r--   0     1001      123     9791 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/data/sample.txt
+-rw-r--r--   0     1001      123      824 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/holiday_selector.rs
+-rw-r--r--   0     1001      123      905 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/issues.rs
+-rw-r--r--   0     1001      123     2501 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1487 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/month_selector.rs
+-rw-r--r--   0     1001      123     1528 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/next_change.rs
+-rw-r--r--   0     1001      123      497 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/next_change_hint.rs
+-rw-r--r--   0     1001      123      339 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/parser.rs
+-rw-r--r--   0     1001      123     2790 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/rules.rs
+-rw-r--r--   0     1001      123     3243 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/selective.rs
+-rw-r--r--   0     1001      123     1598 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/time_selector.rs
+-rw-r--r--   0     1001      123     1176 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/week_selector.rs
+-rw-r--r--   0     1001      123     2541 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/weekday_selector.rs
+-rw-r--r--   0     1001      123     1419 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/tests/year_selector.rs
+-rw-r--r--   0     1001      123     3287 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/time_filter.rs
+-rw-r--r--   0     1001      123       22 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/utils/mod.rs
+-rw-r--r--   0     1001      123     3872 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours/src/utils/range.rs
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/Cargo.toml
+-rw-r--r--   0     1001      123    10847 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/LICENSE-MIT
+-rw-r--r--   0     1001      123      874 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/README.md
+-rw-r--r--   0     1001      123      859 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/error.rs
+-rw-r--r--   0     1001      123     2087 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/extended_time.rs
+-rw-r--r--   0     1001      123     6513 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/grammar.pest
+-rw-r--r--   0     1001      123      810 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/lib.rs
+-rw-r--r--   0     1001      123    24312 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/parser.rs
+-rw-r--r--   0     1001      123     4206 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/rules/day.rs
+-rw-r--r--   0     1001      123      584 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/rules/mod.rs
+-rw-r--r--   0     1001      123     1381 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/rules/time.rs
+-rw-r--r--   0     1001      123     4048 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/opening-hours-syntax/src/sorted_vec.rs
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 opening_hours_py-0.6.5/local_dependencies/compact-calendar/Cargo.toml
+-rw-r--r--   0     1001      123     1588 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/compact-calendar/README.md
+-rw-r--r--   0     1001      123    23597 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/local_dependencies/compact-calendar/src/lib.rs
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 opening_hours_py-0.6.5/Cargo.toml
+-rw-r--r--   0     1001      123       40 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/.gitignore
+-rw-r--r--   0     1001      123    10847 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/LICENSE-MIT
+-rw-r--r--   0     1001      123     1718 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/README.md
+-rw-r--r--   0     1001      123    12755 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/poetry.lock
+-rw-r--r--   0     1001      123      374 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/pyproject.toml
+-rwxr-xr-x   0     1001      123      490 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/run_doctests.py
+-rw-r--r--   0     1001      123      692 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/src/errors.rs
+-rw-r--r--   0     1001      123     6474 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/src/lib.rs
+-rw-r--r--   0     1001      123     4967 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/src/types.rs
+-rw-r--r--   0     1001      123    29444 2023-06-14 11:48:50.000000 opening_hours_py-0.6.5/Cargo.lock
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 opening_hours_py-0.6.5/PKG-INFO
```

### Comparing `opening_hours_py-0.6.4/Cargo.toml` & `opening_hours_py-0.6.5/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "opening-hours-py"
-version = "0.6.4"
+version = "0.6.5"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://remi-dupre.github.io/opening-hours-rs/opening_hours.html"
 homepage = "https://github.com/remi-dupre/opening-hours-rs/tree/master/python"
 description = "A parser and toolkit for the opening_hours in OpenStreetMap written in Rust."
@@ -16,13 +16,13 @@
 
 [profile.release]
 codegen-units = 1
 lto = "fat"
 
 [dependencies]
 chrono = "0.4"
-opening-hours = { path = ".." }
-opening-hours-syntax = { path = "../opening-hours-syntax" }
+opening-hours = { path = "local_dependencies/opening-hours" }
+opening-hours-syntax = { path = "local_dependencies/opening-hours-syntax" }
 
 [dependencies.pyo3]
-version = "0.16"
+version = "0.19"
 features = ["extension-module"]
```

### Comparing `opening_hours_py-0.6.4/LICENSE-APACHE` & `opening_hours_py-0.6.5/local_dependencies/opening-hours/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.4/LICENSE-MIT` & `opening_hours_py-0.6.5/local_dependencies/opening-hours/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.4/README.md` & `opening_hours_py-0.6.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Usage
 -----
 
 Install `opening-hours-py` from PyPI, for example using pip:
 
 ```bash
-pip install --user opening-hours-rs
+pip install --user opening-hours-py
 ```
 
 Then, the main object that you will interact with will be `OpeningHours`:
 
 ```python
 from opening_hours import OpeningHours
```

### Comparing `opening_hours_py-0.6.4/poetry.lock` & `opening_hours_py-0.6.5/poetry.lock`

 * *Files 18% similar despite different names*

```diff
@@ -1,138 +1,155 @@
+# This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
+
 [[package]]
 name = "jinja2"
 version = "3.1.2"
 description = "A very fast and expressive template engine."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
+files = [
+    {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
+    {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
+]
 
 [package.dependencies]
 MarkupSafe = ">=2.0"
 
 [package.extras]
 i18n = ["Babel (>=2.7)"]
 
 [[package]]
 name = "markupsafe"
-version = "2.1.1"
+version = "2.1.3"
 description = "Safely add untrusted strings to HTML/XML markup."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
+files = [
+    {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-win32.whl", hash = "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-win_amd64.whl", hash = "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-win32.whl", hash = "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-win_amd64.whl", hash = "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-win32.whl", hash = "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-win_amd64.whl", hash = "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-win32.whl", hash = "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-win_amd64.whl", hash = "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-win32.whl", hash = "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-win_amd64.whl", hash = "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba"},
+    {file = "MarkupSafe-2.1.3.tar.gz", hash = "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad"},
+]
 
 [[package]]
 name = "maturin"
-version = "0.9.4"
+version = "1.1.0"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
-category = "dev"
 optional = false
-python-versions = ">=3.5"
+python-versions = ">=3.7"
+files = [
+    {file = "maturin-1.1.0-py3-none-linux_armv6l.whl", hash = "sha256:eb04f3473b9f283eba51a5dc20dc0bab6f8741048c1bbc5e45f39cc29ad69aa6"},
+    {file = "maturin-1.1.0-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:eee3c9b2cd80adee6938ea1828882795e261a7fc6b5ebaed15003ed4d713adaa"},
+    {file = "maturin-1.1.0-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:9042ea6538529e22954c0a4eefbe55026a9eba45484423882dd8eb97854b29dd"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:4252241c196abf0ede0088e38bc3c181fe0bf073a974d6594493f3ae7232545c"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.musllinux_1_1_x86_64.whl", hash = "sha256:6f63dc6f9dba2081346f0ff40019e67a72eb20af7ee4847dc21174dd3636a981"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.musllinux_1_1_aarch64.whl", hash = "sha256:c0fecd5ae4f8bad703ee648873d837e3bd6eb846f48ff8607bfb0556a2010adc"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.musllinux_1_1_armv7l.whl", hash = "sha256:19332aa0830f23813e461f61e4d2b7d0c6f8ec84c335040232aafea3f068ac31"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.musllinux_1_1_ppc64le.whl", hash = "sha256:3f6f1e8e970f7728c26eeb55b4c38103f2c5d830b9df4c12fd00903eef7a4114"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:7a2398df2d2f5ba4970ac7f670108e7c7e2da39185caf9b9f9e67d14ae4315e2"},
+    {file = "maturin-1.1.0-py3-none-win32.whl", hash = "sha256:32e95212e6b334caf68d278bcc5137dde020a8e84095c2728d9b08d2311e5d64"},
+    {file = "maturin-1.1.0-py3-none-win_amd64.whl", hash = "sha256:47705b6c5b5ec9d883f6b4fb6ae2480a07a77aabbfbc658d6327c9d6cd74c7cf"},
+    {file = "maturin-1.1.0-py3-none-win_arm64.whl", hash = "sha256:a36efcca897b356deee56c7a3c399c595201518a892ec0f20f0f20abb3064ccb"},
+    {file = "maturin-1.1.0.tar.gz", hash = "sha256:4650aeaa8debd004b55aae7afb75248cbd4d61cd7da2dcf4ead8b22b58cecae0"},
+]
 
 [package.dependencies]
-toml = ">=0.10.0,<0.11.0"
+tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
+
+[package.extras]
+patchelf = ["patchelf"]
+zig = ["ziglang (>=0.10.0,<0.11.0)"]
 
 [[package]]
 name = "pdoc"
-version = "12.0.1"
+version = "12.3.1"
 description = "API Documentation for Python Projects"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
+files = [
+    {file = "pdoc-12.3.1-py3-none-any.whl", hash = "sha256:c3f24f31286e634de9c76fa6e67bd5c0c5e74360b41dc91e6b82499831eb52d8"},
+    {file = "pdoc-12.3.1.tar.gz", hash = "sha256:453236f225feddb8a9071428f1982a78d74b9b3da4bc4433aedb64dbd0cc87ab"},
+]
 
 [package.dependencies]
 Jinja2 = ">=2.11.0"
 MarkupSafe = "*"
 pygments = ">=2.12.0"
 
 [package.extras]
-dev = ["flake8", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-timeout", "tox"]
+dev = ["black", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-timeout", "ruff", "tox", "types-pygments"]
 
 [[package]]
 name = "pygments"
-version = "2.12.0"
+version = "2.15.1"
 description = "Pygments is a syntax highlighting package written in Python."
-category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
+files = [
+    {file = "Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
+    {file = "Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
+]
+
+[package.extras]
+plugins = ["importlib-metadata"]
 
 [[package]]
-name = "toml"
-version = "0.10.2"
-description = "Python Library for Tom's Obvious, Minimal Language"
-category = "dev"
+name = "tomli"
+version = "2.0.1"
+description = "A lil' TOML parser"
 optional = false
-python-versions = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
+python-versions = ">=3.7"
+files = [
+    {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
+    {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
+]
 
 [metadata]
-lock-version = "1.1"
+lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "41437d9fce6d729def72d95b718989a2a40102c1e292d4bb0da89db9818359fa"
-
-[metadata.files]
-jinja2 = [
-    {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
-    {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
-]
-markupsafe = [
-    {file = "MarkupSafe-2.1.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-win32.whl", hash = "sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6"},
-    {file = "MarkupSafe-2.1.1-cp310-cp310-win_amd64.whl", hash = "sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-win32.whl", hash = "sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff"},
-    {file = "MarkupSafe-2.1.1-cp37-cp37m-win_amd64.whl", hash = "sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-win32.whl", hash = "sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1"},
-    {file = "MarkupSafe-2.1.1-cp38-cp38-win_amd64.whl", hash = "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-win32.whl", hash = "sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c"},
-    {file = "MarkupSafe-2.1.1-cp39-cp39-win_amd64.whl", hash = "sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247"},
-    {file = "MarkupSafe-2.1.1.tar.gz", hash = "sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b"},
-]
-maturin = [
-    {file = "maturin-0.9.4-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:79ea854e014e8a601fc1b71eb3bb82bf4d81b62890dee69e4a083cba1f738ce9"},
-    {file = "maturin-0.9.4-py3-none-manylinux2010_x86_64.whl", hash = "sha256:e52dfb6bc6f1c1062883fd785466e246d733f9c7eb90a3cd00ff2d4c659d23ca"},
-    {file = "maturin-0.9.4-py3-none-manylinux2014_aarch64.whl", hash = "sha256:ea08990ba22b76da8f83e5cd1a75f0ec08c045fa0149901343eba1fccfc2a406"},
-    {file = "maturin-0.9.4-py3-none-manylinux2014_armv7l.whl", hash = "sha256:213a69ed4976d078439d2bad148f41f82c919ab98fa85d3d54ebc3ba211a5895"},
-    {file = "maturin-0.9.4-py3-none-win32.whl", hash = "sha256:981330c9c46c2e5c6a648ef54809f573fa9bc257151c119089ccf9d3fe9bfb82"},
-    {file = "maturin-0.9.4-py3-none-win_amd64.whl", hash = "sha256:07ed1cc166bff8d66245c2112ae58869d3cb3ae47a057de06945ea0eb10337d6"},
-    {file = "maturin-0.9.4.tar.gz", hash = "sha256:2e0b0c3eb233e7b776c004ee4b980907beaf2babbe21da05a60ac55c1dff46c3"},
-]
-pdoc = [
-    {file = "pdoc-12.0.1-py3-none-any.whl", hash = "sha256:b27467651e5d8afa3cfc67ced2d978fb97e04ce91506579bba4d05b902fad096"},
-    {file = "pdoc-12.0.1.tar.gz", hash = "sha256:39f58c187f668e46485a51e7d4a3410484d054567e21937a5c28471dc03fc6de"},
-]
-pygments = [
-    {file = "Pygments-2.12.0-py3-none-any.whl", hash = "sha256:dc9c10fb40944260f6ed4c688ece0cd2048414940f1cea51b8b226318411c519"},
-    {file = "Pygments-2.12.0.tar.gz", hash = "sha256:5eb116118f9612ff1ee89ac96437bb6b49e8f04d8a13b514ba26f620208e26eb"},
-]
-toml = [
-    {file = "toml-0.10.2-py2.py3-none-any.whl", hash = "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"},
-    {file = "toml-0.10.2.tar.gz", hash = "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"},
-]
+content-hash = "332291e13df8556b5ef6194f642affff2f47b0b4e160db01447c3a9e3039ae00"
```

### Comparing `opening_hours_py-0.6.4/src/errors.rs` & `opening_hours_py-0.6.5/src/errors.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.4/src/lib.rs` & `opening_hours_py-0.6.5/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 use chrono::offset::Local;
 use chrono::NaiveDateTime;
 
 use pyo3::prelude::*;
 use pyo3::wrap_pyfunction;
 
-use types::RangeIterator;
-
 use crate::errors::ParserError;
+use crate::types::RangeIterator;
 use crate::types::{NaiveDateTimeWrapper, State};
 
 fn get_time(datetime: Option<NaiveDateTime>) -> NaiveDateTime {
     datetime.unwrap_or_else(|| Local::now().naive_local())
 }
 
 /// Validate that input string is a correct opening hours description.
@@ -26,15 +25,15 @@
 /// >>> opening_hours.validate("24/7")
 /// True
 /// >>> opening_hours.validate("24/24")
 /// False
 #[pyfunction]
 #[pyo3(text_signature = "(oh, /)")]
 fn validate(oh: &str) -> bool {
-    opening_hours::OpeningHours::parse(oh).is_ok()
+    ::opening_hours::OpeningHours::parse(oh).is_ok()
 }
 
 /// Parse input opening hours description.
 ///
 /// Raises
 /// ------
 /// SyntaxError
@@ -42,25 +41,25 @@
 ///
 /// Examples
 /// --------
 /// >>> oh = OpeningHours("24/7")
 /// >>> oh.is_open()
 /// True
 #[pyclass]
-#[pyo3(text_signature = "(oh, /)")]
 struct OpeningHours {
-    inner: Pin<Arc<opening_hours::OpeningHours>>,
+    inner: Pin<Arc<::opening_hours::OpeningHours>>,
 }
 
 #[pymethods]
 impl OpeningHours {
     #[new]
+    #[pyo3(text_signature = "(oh, /)")]
     fn new(oh: &str) -> PyResult<Self> {
         Ok(Self {
-            inner: Arc::pin(opening_hours::OpeningHours::parse(oh).map_err(ParserError::from)?),
+            inner: Arc::pin(::opening_hours::OpeningHours::parse(oh).map_err(ParserError::from)?),
         })
     }
 
     /// Get current state of the time domain, the state can be either "open",
     /// "closed" or "unknown".
     ///
     /// Parameters
```

### Comparing `opening_hours_py-0.6.4/src/types.rs` & `opening_hours_py-0.6.5/src/types.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use std::convert::TryInto;
 use std::pin::Pin;
 use std::sync::Arc;
 
 use chrono::prelude::*;
 use chrono::NaiveDateTime;
+use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::{PyDateAccess, PyDateTime, PyTimeAccess};
 
 use opening_hours::DateTimeRange;
 use opening_hours_syntax::rules::RuleKind;
 
 // ---
@@ -57,29 +58,38 @@
         Self(dt)
     }
 }
 
 impl<'source> FromPyObject<'source> for NaiveDateTimeWrapper {
     fn extract(ob: &'source PyAny) -> PyResult<Self> {
         let py_datetime: &PyDateTime = ob.downcast()?;
-        Ok({
-            NaiveDateTime::new(
-                NaiveDate::from_ymd(
-                    py_datetime.get_year(),
-                    py_datetime.get_month().into(),
-                    py_datetime.get_day().into(),
-                ),
-                NaiveTime::from_hms(
-                    py_datetime.get_hour().into(),
-                    py_datetime.get_minute().into(),
-                    py_datetime.get_second().into(),
-                ),
+
+        let rs_date = {
+            NaiveDate::from_ymd_opt(
+                py_datetime.get_year(),
+                py_datetime.get_month().into(),
+                py_datetime.get_day().into(),
+            )
+            .ok_or_else(|| {
+                PyErr::new::<PyValueError, _>("Could not convert Python's date to Rust's NaiveDate")
+            })?
+        };
+
+        let rs_time = {
+            NaiveTime::from_hms_opt(
+                py_datetime.get_hour().into(),
+                py_datetime.get_minute().into(),
+                py_datetime.get_second().into(),
             )
-            .into()
-        })
+            .ok_or(PyErr::new::<PyValueError, _>(
+                "Could not convert Python's time to Rust's NaiveTime",
+            ))?
+        };
+
+        Ok(NaiveDateTime::new(rs_date, rs_time).into())
     }
 }
 
 impl IntoPy<PyResult<Py<PyDateTime>>> for NaiveDateTimeWrapper {
     fn into_py(self, py: Python<'_>) -> PyResult<Py<PyDateTime>> {
         PyDateTime::new(
             py,
```

### Comparing `opening_hours_py-0.6.4/PKG-INFO` & `opening_hours_py-0.6.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: opening-hours-py
-Version: 0.6.4
+Version: 0.6.5
 Summary: A parser and toolkit for the opening_hours in OpenStreetMap written in Rust.
 Home-Page: https://github.com/remi-dupre/opening-hours-rs/tree/master/python
 Author: Rémi Dupré <remi@dupre.io>
-Author-Email: Rémi Dupré <remi@dupre.io>
+Author-email: Rémi Dupré <remi@dupre.io>
 License: MIT OR Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/remi-dupre/opening-hours-rs
 
 Python bindings for [OSM Opening Hours](https://github.com/remi-dupre/opening-hours-rs)
 =======================================
 
 [![PyPI](https://img.shields.io/pypi/v/opening-hours-py)](https://pypi.org/project/opening-hours-py/)
 [![Doc](https://img.shields.io/badge/doc-pdoc-blue)](https://remi-dupre.github.io/opening-hours-rs/opening_hours.html)
 
 
 Usage
 -----
 
 Install `opening-hours-py` from PyPI, for example using pip:
 
 ```bash
-pip install --user opening-hours-rs
+pip install --user opening-hours-py
 ```
 
 Then, the main object that you will interact with will be `OpeningHours`:
 
 ```python
 from opening_hours import OpeningHours
```

